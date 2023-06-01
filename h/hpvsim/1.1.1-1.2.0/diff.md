# Comparing `tmp/hpvsim-1.1.1.tar.gz` & `tmp/hpvsim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpvsim-1.1.1.tar", last modified: Fri Mar 10 03:17:24 2023, max compression
+gzip compressed data, was "hpvsim-1.2.0.tar", last modified: Thu Jun  1 02:46:34 2023, max compression
```

## Comparing `hpvsim-1.1.1.tar` & `hpvsim-1.2.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.397435 hpvsim-1.1.1/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12337 2023-03-10 03:16:55.000000 hpvsim-1.1.1/CHANGELOG.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3501 2022-07-29 04:56:27.000000 hpvsim-1.1.1/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1087 2023-01-30 16:47:35.000000 hpvsim-1.1.1/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      205 2022-12-16 01:30:01.000000 hpvsim-1.1.1/MANIFEST.in
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-03-10 03:17:24.397435 hpvsim-1.1.1/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2715 2023-02-01 00:00:08.000000 hpvsim-1.1.1/README.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.393435 hpvsim-1.1.1/docs/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.analysis.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.base.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.calibration.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.data.get_data.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.data.loaders.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      224 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.data.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.defaults.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.immunity.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.interventions.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.misc.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.parameters.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.people.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.plotting.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.population.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.run.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.settings.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.sim.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.utils.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/hpvsim.version.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      312 2022-12-16 01:30:01.000000 hpvsim-1.1.1/docs/index.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      523 2023-01-31 21:47:37.000000 hpvsim-1.1.1/docs/modules.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2022-08-31 16:50:17.000000 hpvsim-1.1.1/docs/overview.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2022-08-31 16:50:17.000000 hpvsim-1.1.1/docs/requirements.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.393435 hpvsim-1.1.1/docs/tutorials/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      345 2022-12-16 01:30:01.000000 hpvsim-1.1.1/docs/tutorials/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      299 2023-02-01 00:00:08.000000 hpvsim-1.1.1/docs/tutorials.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       29 2022-08-31 16:50:17.000000 hpvsim-1.1.1/docs/whats-new.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.393435 hpvsim-1.1.1/hpvsim/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1048 2023-01-30 16:47:35.000000 hpvsim-1.1.1/hpvsim/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    56642 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/analysis.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    83597 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    36126 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/calibration.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.393435 hpvsim-1.1.1/hpvsim/data/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       46 2022-08-31 16:50:17.000000 hpvsim-1.1.1/hpvsim/data/__init__.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.393435 hpvsim-1.1.1/hpvsim/data/files/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       87 2022-10-04 15:39:45.000000 hpvsim-1.1.1/hpvsim/data/files/metadata.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7461 2022-12-16 01:30:01.000000 hpvsim-1.1.1/hpvsim/data/get_data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    11896 2023-01-30 16:47:35.000000 hpvsim-1.1.1/hpvsim/data/loaders.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12633 2023-01-30 16:47:35.000000 hpvsim-1.1.1/hpvsim/data/products_dx.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4283 2023-01-30 16:47:35.000000 hpvsim-1.1.1/hpvsim/data/products_tx.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      908 2022-12-16 01:30:01.000000 hpvsim-1.1.1/hpvsim/data/products_vx.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21198 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/defaults.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22826 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/hiv.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9860 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/immunity.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    65673 2023-01-30 16:47:35.000000 hpvsim-1.1.1/hpvsim/interventions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28482 2022-12-16 01:30:01.000000 hpvsim-1.1.1/hpvsim/misc.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    35865 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/parameters.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    43942 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    44025 2023-01-30 16:47:35.000000 hpvsim-1.1.1/hpvsim/plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    17785 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/population.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.393435 hpvsim-1.1.1/hpvsim/regression/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22216 2022-10-12 05:00:20.000000 hpvsim-1.1.1/hpvsim/regression/pars_v0.2.6.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22085 2022-12-16 01:30:01.000000 hpvsim-1.1.1/hpvsim/regression/pars_v0.2.9.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21901 2022-12-16 01:30:01.000000 hpvsim-1.1.1/hpvsim/regression/pars_v0.3.0.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23231 2022-12-16 01:30:01.000000 hpvsim-1.1.1/hpvsim/regression/pars_v0.3.1.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    71922 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/run.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22131 2022-12-16 01:30:01.000000 hpvsim-1.1.1/hpvsim/settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    65327 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/sim.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21804 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      233 2023-03-10 03:16:55.000000 hpvsim-1.1.1/hpvsim/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.393435 hpvsim-1.1.1/hpvsim.egg-info/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-03-10 03:17:24.000000 hpvsim-1.1.1/hpvsim.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1501 2023-03-10 03:17:24.000000 hpvsim-1.1.1/hpvsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2023-03-10 03:17:24.000000 hpvsim-1.1.1/hpvsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2023-03-10 03:17:24.000000 hpvsim-1.1.1/hpvsim.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        7 2023-03-10 03:17:24.000000 hpvsim-1.1.1/hpvsim.egg-info/top_level.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2023-03-10 03:17:24.397435 hpvsim-1.1.1/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1565 2023-01-30 16:47:35.000000 hpvsim-1.1.1/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-03-10 03:17:24.397435 hpvsim-1.1.1/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       50 2023-01-30 16:47:35.000000 hpvsim-1.1.1/tests/requirements.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13532 2023-06-01 02:46:05.000000 hpvsim-1.2.0/CHANGELOG.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3501 2022-07-29 04:56:27.000000 hpvsim-1.2.0/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1087 2023-01-30 16:47:35.000000 hpvsim-1.2.0/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      205 2022-12-16 01:30:01.000000 hpvsim-1.2.0/MANIFEST.in
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-06-01 02:46:34.346614 hpvsim-1.2.0/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2715 2023-02-01 00:00:08.000000 hpvsim-1.2.0/README.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/docs/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.analysis.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.base.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.calibration.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.data.get_data.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.data.loaders.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      224 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.data.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.defaults.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.immunity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.interventions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.misc.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.parameters.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.people.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.plotting.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.population.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.run.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.settings.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.sim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.utils.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.version.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      312 2022-12-16 01:30:01.000000 hpvsim-1.2.0/docs/index.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      523 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/modules.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2022-08-31 16:50:17.000000 hpvsim-1.2.0/docs/overview.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2022-08-31 16:50:17.000000 hpvsim-1.2.0/docs/requirements.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/docs/tutorials/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      345 2022-12-16 01:30:01.000000 hpvsim-1.2.0/docs/tutorials/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      299 2023-02-01 00:00:08.000000 hpvsim-1.2.0/docs/tutorials.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       29 2022-08-31 16:50:17.000000 hpvsim-1.2.0/docs/whats-new.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/hpvsim/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1048 2023-01-30 16:47:35.000000 hpvsim-1.2.0/hpvsim/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    55482 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/analysis.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    83229 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/base.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    37175 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/calibration.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/hpvsim/data/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       46 2022-08-31 16:50:17.000000 hpvsim-1.2.0/hpvsim/data/__init__.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/hpvsim/data/files/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       87 2022-10-04 15:39:45.000000 hpvsim-1.2.0/hpvsim/data/files/metadata.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7459 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/get_data.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12106 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/loaders.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18870 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_dx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1871 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_tx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      197 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_txvx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      369 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_vx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21237 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/defaults.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22876 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/hiv.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13902 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/immunity.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    67175 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28482 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/misc.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    40694 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    48721 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/people.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    44030 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/plotting.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    17813 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/population.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/hpvsim/regression/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22216 2022-10-12 05:00:20.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.2.6.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22085 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.2.9.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21901 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.3.0.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23231 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.3.1.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    71932 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/run.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22131 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    67290 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24398 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      233 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/hpvsim.egg-info/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1531 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        7 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/top_level.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2023-06-01 02:46:34.346614 hpvsim-1.2.0/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1566 2023-06-01 02:46:05.000000 hpvsim-1.2.0/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       50 2023-01-30 16:47:35.000000 hpvsim-1.2.0/tests/requirements.txt
```

### Comparing `hpvsim-1.1.1/CHANGELOG.rst` & `hpvsim-1.2.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,40 @@
 
 All notable changes to the codebase are documented in this file. Changes that may result in differences in model output, or are required in order to run an old parameter set with the current version, are flagged with the term "Regression information".
 
 .. contents:: **Contents**
    :local:
    :depth: 1
 
+Version 1.2.0 (2023-05-31)
+---------------------------
+- Changes to improve run speed, most notably changes to how migration is applied
+- Additional tests to ensure consistency between calibration results, age analyzer results, and sim results
+- Updates to natural history to prevent people progressing too quickly to cancer
+- *Github info* PR `576 <https://github.com/amath-idm/hpvsim/pull/550>`__
+
+Version 1.1.5 (2023-03-23)
+---------------------------
+- Adds cross-protection functionality to t-cell immunity and adds `sev_imm` attribute to people
+- *Github info* PR `564 <https://github.com/amath-idm/hpvsim/pull/564>`__
+
+Version 1.1.4 (2023-03-15)
+---------------------------
+- Fixes bug that caused location data to be loaded twice
+- *Github info* PR `546 <https://github.com/amath-idm/hpvsim/pull/546>`__
+
+Version 1.1.3 (2023-03-14)
+---------------------------
+- Fixes bug that misses some ways you can specify sex for vaccination
+- *Github info* PR `555 <https://github.com/amath-idm/hpvsim/pull/555>`__
+
+Version 1.1.2 (2023-03-13)
+---------------------------
+- Fixes bug that never computed cancer deaths by age
+- *Github info* PR `554 <https://github.com/amath-idm/hpvsim/pull/554>`__
 
 Version 1.1.1 (2023-03-01)
 ---------------------------
 - Sets time to and date of HIV death for those not on ART and who fail on ART
 - Moves all HIV attributes, parameters, and results into hivsim class instance
 - Merges HIV results with sim.results at conclusion of simulation
 - Adds HIV pars as an argument to calibration as well as HIV-specific results to age-results analyzer
```

### Comparing `hpvsim-1.1.1/CODE_OF_CONDUCT.rst` & `hpvsim-1.2.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/LICENSE` & `hpvsim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/PKG-INFO` & `hpvsim-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpvsim
-Version: 1.1.1
+Version: 1.2.0
 Summary: HPVsim: Human Papillomavirus Simulator
 Home-page: http://hpvsim.org
 Author: Robyn Stuart, Jamie Cohen, Cliff Kerr, Romesh Abeysuriya, Mariah Boudreau, Daniel Klein, Hao Hu
 Author-email: robyn.stuart@gatesfoundation.org
 Keywords: HPV,agent-based model,simulation
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `hpvsim-1.1.1/README.rst` & `hpvsim-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/docs/modules.rst` & `hpvsim-1.2.0/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/__init__.py` & `hpvsim-1.2.0/hpvsim/__init__.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/analysis.py` & `hpvsim-1.2.0/hpvsim/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -509,161 +509,204 @@
 
 
 class age_results(Analyzer):
     '''
     Constructs results by age at specified points within the sim. Can be used with data
 
     Args:
-        result_args (dict): dict of results to generate and associated timepoints/age-bins to generate each result as well as whether to compute_fit
-        result_keys (list): list of results to generate - used to construct result_args is result_args is not provided
-        timepoints  (list): list of timepoints - used to construct result_args is result_args is not provided
-        edges       (arr): list of edges of age bins - used to construct result_args is result_args is not provided
+        result_args (dict): dict of results to generate and associated years/age-bins to generate each result as well as whether to compute_fit
         die         (bool): whether or not to raise an exception if errors are found
         kwargs      (dict): passed to :py:class:`Analyzer`
 
     **Example**::
 
-        # Construct your own result_args if you want different timepoints / age buckets for each one
-
         result_args=sc.objdict(
             hpv_prevalence=sc.objdict(
                 timepoints=[1990],
                 edges=np.array([0.,20.,25.,30.,40.,45.,50.,55.,65.,100.]),
             ),
             hpv_incidence=sc.objdict(
                 timepoints=[1990, 2000],
                 edges=np.array([0.,20.,30.,40.,50.,60.,70.,80.,100.])
             )
         sim = hpv.Sim(analyzers=hpv.age_results(result_args=result_args))
         sim.run()
         age_results = sim['analyzers'][0]
 
-        # Alternatively, use standard timepoints and age buckets across all results
-
-        sim = hpv.Sim(analyzers=hpv.age_results(result_keys=['cancers']))
-
     '''
 
-    def __init__(self, result_keys=None, die=False, edges=None, timepoints=None, result_args=None, **kwargs):
+    def __init__(self, result_args=None, die=False, **kwargs):
         super().__init__(**kwargs) # Initialize the Analyzer object
-        self.mismatch       = 0
+        self.mismatch       = 0 # TODO, should this be set to np.nan initially?
         self.die            = die  # Whether or not to raise an exception
-        self.start          = None # Store the start year of the simulation
-        self.edges          = edges or np.array([0., 15., 20., 25., 30., 35., 40., 45., 50., 55., 60., 65., 70., 75., 80., 85., 100.])
-        self.timepoints     = timepoints
-        self.result_keys    = result_keys or ['infections', 'cancers']
-        self.results        = sc.odict() # Store the age results
+        self.results        = sc.objdict() # Store the age results
         self.result_args    = result_args
         return
 
 
     def initialize(self, sim):
 
         super().initialize()
 
-        # Handle timepoints and dates
-        self.start = sim['start']  # Store the simulation start
-        self.end = sim['end']  # Store simulation end
-        if self.timepoints is None:
-            self.timepoints = [f'{sim["end"]}']
-            self.timepoints, self.dates = sim.get_t(self.timepoints, return_date_format='str') # Ensure timepoints and dates are in the right format
-
         # Handle which results to make. Specification of the results to make is stored in result_args
-        if self.result_args is None: # Make defaults if none are provided
-            self.result_args = sc.objdict()
-            for rkey in self.result_keys:
-                self.result_args[rkey] = sc.objdict(timepoints=self.dates, edges=self.edges)
-        elif sc.checktype(self.result_args, dict): # Ensure it's an object dict
+        if sc.checktype(self.result_args, dict): # Ensure it's an object dict
             self.result_args = sc.objdict(self.result_args)
         else: # Raise an error
-            errormsg = f'result_args must be a dict with keys for the timepoints and edges you want to compute, not {type(self.result_args)}.'
+            errormsg = f'result_args must be a dict with keys for the years and edges you want to compute, not {type(self.result_args)}.'
             raise TypeError(errormsg)
+        self.result_keys = self.result_args.keys()
 
         # Handle dt - if we're storing annual results we'll need to aggregate them over several consecutive timesteps
         self.dt = sim['dt']
         self.resfreq = sim.resfreq
 
-        self.validate_results(sim)
-
         # Store genotypes
         self.ng = sim['n_genotypes']
         self.glabels = [g.upper() for g in sim['genotype_map'].values()]
 
+        # Initialize result structure and validate the result variable arguments
+        self.validate_variables(sim)
+
         # Store colors
         for rkey in self.result_args.keys():
             if 'hiv' in rkey:
                 self.result_args[rkey].color = sim.hivsim.results[rkey].color
                 self.result_args[rkey].name = sim.hivsim.results[rkey].name
             else:
                 self.result_args[rkey].color = sim.results[rkey].color
                 self.result_args[rkey].name = sim.results[rkey].name
 
         self.initialized = True
 
         return
 
 
-    def validate_results(self, sim):
+    def validate_variables(self, sim):
+        '''
+        Check that the variables in result_args are valid, and initialize the result structure
+        '''
         choices = sim.result_keys('total')+[k for k in sim.result_keys('genotype')]
         if sim['model_hiv']:
             choices += list(sim.hivsim.results.keys())
+
         for rk, rdict in self.result_args.items():
             if rk not in choices:
                 strm = '\n'.join(choices)
                 errormsg = f'Cannot compute age results for {rk}. Please enter one of the standard sim result_keys to the age_results analyzer; choices are {strm}.'
                 raise ValueError(errormsg)
             else:
-                self.results[rk] = sc.objdict()
+                self.results[rk] = dict() # Store the results. Not an odict because keyed by year
 
-            # Handle the data file
-            # If data is provided, extract timepoints, edges, age bins and labels from that
+            # If a datafile has been provided, read it in and get the age bins and years
             if 'datafile' in rdict.keys():
                 if sc.isstring(rdict.datafile):
                     rdict.data = hpm.load_data(rdict.datafile, check_date=False)
                 else:
                     rdict.data = rdict.datafile  # Use it directly
                     rdict.datafile = None
 
-                # extract edges, age bins and labels from that
-                # Handle edges, age bins, and labels
-                rdict.timepoints = rdict.data.year.unique()
-                rdict.age_labels = []
-                rdict.edges = np.array(rdict.data.age.unique(), dtype=float)
-                rdict.edges = np.append(rdict.edges, 100)
-                rdict.bins = rdict.edges[:-1]  # Don't include the last edge in the bins
+                # Get edges, age bins, and labels from datafile. This assumes
+                # that the datafile has bins, and we make the edges by appending
+                # the last point of the sim age bin edges.
+                rdict.years = rdict.data.year.unique()
+                rdict.bins = np.array(rdict.data.age.unique(), dtype=float)
+                rdict.edges = np.append(rdict.bins, sim['age_bin_edges'][-1])
                 self.results[rk]['bins'] = rdict.bins
-                rdict.age_labels = [f'{int(rdict.bins[i])}-{int(rdict.bins[i + 1])}' for i in
-                                        range(len(rdict.bins) - 1)]
-                rdict.age_labels.append(f'{int(rdict.bins[-1])}+')
 
             else:
-                # Handle edges, age bins, and labels
-                rdict.age_labels = []
+
+                # Use years and age bin edges provided, or use defaults from sim
                 if (not hasattr(rdict,'edges')) or rdict.edges is None:  # Default age bins
-                    rdict.edges = np.linspace(0, 100, 11)
+                    warnmsg = f'Did not provide edges for age analyzer {rk}'
+                    if self.die:
+                        raise ValueError(warnmsg)
+                    else:
+                        warnmsg += ', using age bin edges from sim'
+                        hpm.warn(warnmsg)
+                        rdict.edges = sim['age_bin_edges']
                 rdict.bins = rdict.edges[:-1]  # Don't include the last edge in the bins
                 self.results[rk]['bins'] = rdict.bins
-                rdict.age_labels = [f'{int(rdict.bins[i])}-{int(rdict.bins[i + 1])}' for i in
-                                    range(len(rdict.bins) - 1)]
-                rdict.age_labels.append(f'{int(rdict.bins[-1])}+')
-                if 'timepoints' not in rdict.keys():
-                    errormsg = 'Did not provide timepoints for this age analyzer'
-                    raise ValueError(errormsg)
 
-            if not rdict.get('dates') or rdict.dates is None:
-                rdict.timepoints, rdict.dates = sim.get_t(rdict.timepoints, return_date_format='str')  # Ensure timepoints and dates are in the right format
+                if 'years' not in rdict.keys():
+                    warnmsg = f'Did not provide years for age analyzer {rk}'
+                    if self.die:
+                        raise ValueError(warnmsg)
+                    else:
+                        warnmsg += ', using final year of sim'
+                        hpm.warn(warnmsg)
+                        rdict.years = sim['end']
+                rdict.years = sc.promotetoarray(rdict.years)
+
+            # Construct age labels used for plotting
+            rdict.age_labels = [f'{int(rdict.bins[i])}-{int(rdict.bins[i + 1])}' for i in
+                                range(len(rdict.bins) - 1)]
+            rdict.age_labels.append(f'{int(rdict.bins[-1])}+')
+
+            # Construct timepoints
+            if not rdict.get('timepoints') or rdict.timepoints is None:
+                rdict.timepoints = []
+                for y in rdict.years:
+                    rdict.timepoints.append(sc.findinds(sim.yearvec, y)[0] + int(1 / sim['dt']) - 1)
+
+            # Check that the requested timepoints are in the sim
             max_hist_time = rdict.timepoints[-1]
-            max_sim_time = sim['end']
+            max_sim_time = sim.tvec[-1]
             if max_hist_time > max_sim_time:
-                errormsg = f'Cannot create age results for {rdict.dates[-1]} ({max_hist_time}) because the simulation ends on {self.end} ({max_sim_time})'
+                errormsg = f'Cannot create age results for {rdict.years[-1]} ({max_hist_time}) because the simulation ends on {self.end} ({max_sim_time})'
                 raise ValueError(errormsg)
 
-            rdict.calcpoints = []
-            for tpi, tp in enumerate(rdict.timepoints):
-                rdict.calcpoints += [tp + i for i in range(int(1 / self.dt))]
+            # Translate the name of the result to the people attribute
+            result_name = sc.dcp(rk)
+            na = len(rdict.bins)
+            ng = sim['n_genotypes']
+
+            # Clean up the name
+            if 'genotype' in result_name: # Results by genotype
+                result_name = result_name.replace('_by_genotype','') # remove "by_genotype" from result name
+                rdict.size = (na, ng)
+                rdict.by_genotype = True
+            else: # Total results
+                rdict.size = na
+                rdict.by_genotype = False
+            rdict.by_hiv = False
+            if '_with_hiv' in result_name:
+                result_name = result_name.replace('_with_hiv', '')  # remove "_with_hiv" from result name
+                rdict.by_hiv = True
+                rdict.hiv_attr = 'hiv'
+            elif '_no_hiv' in result_name:
+                result_name = result_name.replace('_no_hiv', '')  # remove "_no_hiv" from result name
+                rdict.by_hiv = True
+                # attr3 = ~ppl['hiv']
+
+            # Figure out if it's a flow or incidence
+            if result_name in hpd.flow_keys or 'incidence' in result_name or 'mortality' in result_name:
+                date_attr, attr = self.convert_rname_flows(result_name)
+                rdict.result_type = 'flow'
+            elif result_name[:2] == 'n_' or 'prevalence' in result_name:
+                attr = self.convert_rname_stocks(result_name)  # Convert to a people attribute
+                date_attr = None
+                rdict.result_type = 'stock'
+
+            rdict.attr = attr
+            rdict.date_attr = date_attr
+
+            # Initialize results
+            for year in rdict.years:
+                self.results[rk][year] = np.zeros(rdict.size)
+
+            # For flows, we calculate results on all the timepoints throughout the year, not just the last one
+            if rdict.result_type == 'flow':
+                rdict.calcpoints = []
+                rdict.calcpointyears = []
+                for tpi, tp in enumerate(rdict.timepoints):
+                    rdict.calcpoints += [tp+i+1 for i in range(-int(1/self.dt),0)]
+                    rdict.calcpointyears += [sim.yearvec[tp-(int(1/sim['dt'])-1)]]*int(1/self.dt)
+            else:
+                rdict.calcpoints = sc.dcp(rdict.timepoints)
+                rdict.calcpointyears = [sim.yearvec[tp-(int(1/sim['dt'])-1)] for tp in rdict.calcpoints]
 
             if 'compute_fit' in rdict.keys() and rdict.compute_fit:
                 if rdict.data is None:
                     errormsg = 'Cannot compute fit without data'
                     raise ValueError(errormsg)
                 else:
                     if 'weights' in rdict.data.columns:
@@ -714,146 +757,110 @@
         ng = self.ng
         ppl = sim.people
 
         def bin_ages(inds=None, bins=None):
             return np.histogram(ppl.age[inds], bins=bins, weights=ppl.scale[inds])[0] # Bin the people
 
         # Go through each result key and determine if this is a timepoint where age results are requested
-        for result, result_dict in self.result_args.items():
+        for rkey, rdict in self.result_args.items():
 
             # Establish initial quantities
-            bins = result_dict.edges
-            na = len(result_dict.bins)
-            if 'genotype' in result: # Results by genotype
-                result_name = result.replace('_by_genotype','') # remove "by_genotype" from result name
-                size = (na, ng)
-                by_genotype = True
-            else: # Total results
-                result_name = result[:]
-                size = na
-                by_genotype = False
-
-            # This section is completed for stocks
-            if sim.t in result_dict.timepoints:
-
-                ind = sc.findinds(result_dict.timepoints, sim.t)[0]  # Get the index
-                date = result_dict.dates[ind]  # Create the date which will be used to key the results
-                self.results[result][date] = np.zeros(size)
+            bins = rdict.edges
+            na = len(rdict.bins)
+
+            # Calculate flows and stocks over all calcpoints
+            if sim.t in rdict.calcpoints:
 
-                if 'compute_fit' in result_dict.keys():
-                    thisdatadf = result_dict.data[(result_dict.data.year == float(date)) & (result_dict.data.name == result)]
+                date_ind = sc.findinds(rdict.calcpoints, sim.t)[0]  # Get the index
+                date = rdict.calcpointyears[date_ind]  # Create the date which will be used to key the results
+
+                if 'compute_fit' in rdict.keys():
+                    thisdatadf = rdict.data[(rdict.data.year == float(date)) & (rdict.data.name == rkey)]
                     unique_genotypes = thisdatadf.genotype.unique()
-                    ng = len(unique_genotypes)
+                    ng = len(unique_genotypes)  # CAREFUL, THIS IS OVERWRITING
 
-                # Both annual stocks and prevalence require us to calculate the current stocks.
-                # Unlike incidence, these don't have to be aggregated over multiple timepoints.
-                if result_name[0] == 'n' or 'prevalence' in result_name:
-                    by_hiv = False
-                    if '_with_hiv' in result_name:
-                        result_name = result_name.replace('_with_hiv', '')  # remove "_with_hiv" from result name
-                        by_hiv = True
-                        attr2 = ppl['hiv']
-                    elif '_no_hiv' in result_name:
-                        result_name = result_name.replace('_no_hiv', '')  # remove "_no_hiv" from result name
-                        by_hiv = True
-                        attr2 = ~ppl['hiv']
-
-                    attr = self.convert_rname_stocks(result_name) # Convert to a people attribute
-                    if attr in ppl.keys():
-                        if not by_genotype:
-                            if by_hiv:
-                                inds = (ppl[attr].any(axis=0) * attr2).nonzero()[-1]  # Pull out people for which this state is true
-                            else:
-                                inds = ppl[attr].any(axis=0).nonzero()[-1]  # Pull out people for which this state is true
-                            self.results[result][date] = bin_ages(inds, bins)
-                        else:
-                            for g in range(ng):
-                                inds = ppl[attr][g, :].nonzero()[-1]
-                                self.results[result][date][g, :] = bin_ages(inds, bins)  # Bin the people
-
-                        if 'prevalence' in result:
-                            # Need to divide by the right denominator
-                            if 'hpv' in result:  # Denominator is whole population
-                                if by_hiv:
-                                    inds = sc.findinds(attr2)
-                                    denom = bin_ages(inds=inds, bins=bins)
-                                else:
-                                    denom = bin_ages(inds=None, bins=bins)
-                            else:  # Denominator is females
-                                denom = bin_ages(inds=ppl.f_inds, bins=bins)
-                            if by_genotype: denom = denom[None, :]
-                            self.results[result][date] = self.results[result][date] / denom
-
-                self.date = date # Need to store the date for subsequent calcpoints
-                self.timepoint = sim.t # Need to store the timepoints for subsequent calcpoints
-
-            # Both annual new cases and incidence require us to calculate the new cases over all
-            # the timepoints that belong to the requested year.
-            if sim.t in result_dict.calcpoints:
-                by_hiv = False
-                if '_with_hiv' in result_name:
-                    result_name = result_name.replace('_with_hiv','') # remove "_with_hiv" from result name
-                    by_hiv = True
-                    attr3 = ppl['hiv']
-                elif '_no_hiv' in result_name:
-                    result_name = result_name.replace('_no_hiv', '')  # remove "_no_hiv" from result name
-                    by_hiv = True
-                    attr3 = ~ppl['hiv']
-                # Figure out if it's a flow or incidence
-                if result_name in hpd.flow_keys or 'incidence' in result_name or 'mortality' in result_name:
-
-                    date = self.date  # Stored just above for use here
-                    attr1, attr2 = self.convert_rname_flows(result_name)
-
-                    if not by_genotype:  # Results across all genotypes
-                        if result_name == 'detected_cancer_deaths':
-                            inds = ((ppl[attr1] == sim.t) * (ppl[attr2]) * (ppl['detected_cancer'])).nonzero()[-1]
+                # Figure out if it's a flow
+                if rdict.result_type == 'flow':
+
+                    if not rdict.by_genotype:  # Results across all genotypes
+                        if rkey == 'detected_cancer_deaths':
+                            inds = ((ppl[rdict.date_attr] == sim.t) * (ppl[rdict.attr]) * (ppl['detected_cancer'])).nonzero()[-1]
                         else:
-                            if by_hiv:
-                                inds = ((ppl[attr1] == sim.t) * (ppl[attr2]) * (attr3)).nonzero()[-1]
+                            if rdict.by_hiv:
+                                inds = ((ppl[rdict.date_attr] == sim.t) * (ppl[rdict.attr]) * (ppl[rdict.hiv_attr])).nonzero()[-1]
                             else:
-                                inds = ((ppl[attr1] == sim.t) * (ppl[attr2])).nonzero()[-1]
-                        self.results[result][date] += bin_ages(inds, bins)  # Bin the people
+                                inds = ((ppl[rdict.date_attr] == sim.t) * (ppl[rdict.attr])).nonzero()[-1]
+                        self.results[rkey][date] += bin_ages(inds, bins)  # Bin the people
                     else:  # Results by genotype
                         for g in range(ng):  # Loop over genotypes
-                            inds = ((ppl[attr1][g, :] == sim.t) * (ppl[attr2][g, :])).nonzero()[-1]
-                            self.results[result][date][:, g] += bin_ages(inds, bins)  # Bin the people
+                            inds = ((ppl[rdict.date_attr][g, :] == sim.t) * (ppl[rdict.attr][g, :])).nonzero()[-1]
+                            self.results[rkey][date][:, g] += bin_ages(inds, bins)  # Bin the people
 
-                    # Figure out if this is the last timepoint in the year we're calculating results for
-                    if sim.t == self.timepoint+self.resfreq-1:
-                        if 'incidence' in result:
-                            # Need to divide by the right denominator
-                            if 'hpv' in result:  # Denominator is susceptible population
-                                denom = bin_ages(inds=hpu.true(ppl.sus_pool), bins=bins)
-                            else:  # Denominator is females at risk for cancer
-                                if by_hiv:
-                                    inds = sc.findinds(ppl.is_female_alive & attr3 * ~ppl.cancerous.any(axis=0))
-                                else:
-                                    inds = sc.findinds(ppl.is_female_alive & ~ppl.cancerous.any(axis=0))
-                                denom = bin_ages(inds, bins) / 1e5  # CIN and cancer are per 100,000 women
-                            if 'total' not in result and 'cancer' not in result: denom = denom[None, :]
-                            self.results[result][date] = self.results[result][date] / denom
-
-                        if 'mortality' in result:
-                            # Need to divide by the right denominator
-                            # first need to find people who died of other causes today and add them back into denom
-                            denom = bin_ages(inds=ppl.is_female_alive, bins=bins)
-                            scale_factor =  1e5  # per 100,000 women
-                            denom /= scale_factor
-                            self.results[result][date] = self.results[result][date] / denom
+                # This section is completed for stocks
+                elif rdict.result_type == 'stock':
+
+                    if not rdict.by_genotype:
+                        if rdict.by_hiv:
+                            inds = (ppl[rdict.attr].any(axis=0) * ppl[rdict.hiv_attr]).nonzero()[-1]
+                        else:
+                            inds = ppl[rdict.attr].any(axis=0).nonzero()[-1]
+                        self.results[rkey][date] = bin_ages(inds, bins)
+                    else:
+                        for g in range(ng):
+                            inds = ppl[rdict.attr][g, :].nonzero()[-1]
+                            self.results[rkey][date][g, :] = bin_ages(inds, bins)  # Bin the people
+
+            # On the final timepoint in the year, normalize
+            if sim.t in rdict.timepoints:
+
+                if 'prevalence' in rkey:
+                    if 'hpv' in rkey:  # Denominator is whole population
+                        if rdict.by_hiv:
+                            inds = sc.findinds(ppl[rdict.hiv_attr])
+                            denom = bin_ages(inds=inds, bins=bins)
+                        else:
+                            denom = bin_ages(inds=ppl.alive, bins=bins)
+                    else:  # Denominator is females
+                        denom = bin_ages(inds=ppl.f_inds, bins=bins)
+                    if rdict.by_genotype: denom = denom[None, :]
+                    self.results[rkey][date] = self.results[rkey][date] / (denom)
+
+                if 'incidence' in rkey:
+                    if 'hpv' in rkey:  # Denominator is susceptible population
+                        denom = bin_ages(inds=hpu.true(ppl.sus_pool), bins=bins)
+                    else:  # Denominator is females at risk for cancer
+                        if rdict.by_hiv:
+                            inds = sc.findinds(ppl.is_female_alive & ppl[rdict.hiv_attr] * ~ppl.cancerous.any(axis=0))
+                        else:
+                            inds = sc.findinds(ppl.is_female_alive & ~ppl.cancerous.any(axis=0))
+                        denom = bin_ages(inds, bins) / 1e5  # CIN and cancer are per 100,000 women
+                    # if 'total' not in result and 'cancer' not in result: denom = denom[None, :] # THIS IS IT!!!!
+                    self.results[rkey][date] = self.results[rkey][date] / denom
+
+                if 'mortality' in rkey:
+                    # first need to find people who died of other causes today and add them back into denom
+                    denom = bin_ages(inds=ppl.is_female_alive, bins=bins)
+                    scale_factor =  1e5  # per 100,000 women
+                    denom /= scale_factor
+                    self.results[rkey][date] = self.results[rkey][date] / denom
+
+        return
 
 
     def finalize(self, sim):
         super().finalize()
         for rkey, rdict in self.result_args.items():
-            validate_recorded_dates(sim, requested_dates=rdict.dates, recorded_dates=self.results[rkey].keys()[1:], die=self.die)
+            recorded_dates = [k for k in self.results[rkey].keys()][1:]
+            validate_recorded_dates(sim, requested_dates=rdict.years, recorded_dates=recorded_dates, die=self.die)
             if 'compute_fit' in rdict.keys():
-                self.mismatch += self.compute(rkey)
+                self.mismatch += self.compute_mismatch(rkey)
 
-        sim.fit = self.mismatch
+        # Add to sim.fit
+        if hasattr(sim,'fit'): sim.fit += self.mismatch
+        else: sim.fit = self.mismatch
 
         return
 
 
     @staticmethod
     def reduce(analyzers, use_mean=False, bounds=None, quantiles=None):
         ''' Create an averaged age result from a list of age result analyzers '''
@@ -901,50 +908,52 @@
         reduced_analyzer = sc.dcp(base_analyzer)
         reduced_analyzer.results = sc.objdict() # Remove the age results so we can rebuild them
 
         # Aggregate the list of analyzers
         raw = {}
         for reskey in base_analyzer.results.keys():
             raw[reskey] = {}
-            reduced_analyzer.results[reskey] = sc.objdict()
+            reduced_analyzer.results[reskey] = dict()
             reduced_analyzer.results[reskey]['bins'] = base_analyzer.results[reskey]['bins']
-            for date,tp in zip(base_analyzer.result_args[reskey].dates, base_analyzer.result_args[reskey].timepoints):
-                ashape = analyzer.results[reskey][date].shape # Figure out dimensions
+            for year,tp in zip(base_analyzer.result_args[reskey].years, base_analyzer.result_args[reskey].timepoints):
+                ashape = analyzer.results[reskey][year].shape # Figure out dimensions
                 new_ashape = ashape + (len(analyzers),)
-                raw[reskey][date] = np.zeros(new_ashape)
+                raw[reskey][year] = np.zeros(new_ashape)
                 for a, analyzer in enumerate(analyzers):
-                    vals = analyzer.results[reskey][date]
+                    vals = analyzer.results[reskey][year]
                     if len(ashape) == 1:
-                        raw[reskey][date][:, a] = vals
+                        raw[reskey][year][:, a] = vals
                     elif len(ashape) == 2:
-                        raw[reskey][date][:, :, a] = vals
+                        raw[reskey][year][:, :, a] = vals
 
                 # Summarizing the aggregated list
-                reduced_analyzer.results[reskey][date] = sc.objdict()
+                reduced_analyzer.results[reskey][year] = sc.objdict()
                 if use_mean:
-                    r_mean = np.mean(raw[reskey][date], axis=-1)
-                    r_std = np.std(raw[reskey][date], axis=-1)
-                    reduced_analyzer.results[reskey][date].best = r_mean
-                    reduced_analyzer.results[reskey][date].low  = r_mean - bounds * r_std
-                    reduced_analyzer.results[reskey][date].high = r_mean + bounds * r_std
+                    r_mean = np.mean(raw[reskey][year], axis=-1)
+                    r_std = np.std(raw[reskey][year], axis=-1)
+                    reduced_analyzer.results[reskey][year].best = r_mean
+                    reduced_analyzer.results[reskey][year].low  = r_mean - bounds * r_std
+                    reduced_analyzer.results[reskey][year].high = r_mean + bounds * r_std
                 else:
-                    reduced_analyzer.results[reskey][date].best = np.quantile(raw[reskey][date], q=0.5, axis=-1)
-                    reduced_analyzer.results[reskey][date].low  = np.quantile(raw[reskey][date], q=quantiles['low'], axis=-1)
-                    reduced_analyzer.results[reskey][date].high = np.quantile(raw[reskey][date], q=quantiles['high'], axis=-1)
+                    reduced_analyzer.results[reskey][year].best = np.quantile(raw[reskey][year], q=0.5, axis=-1)
+                    reduced_analyzer.results[reskey][year].low  = np.quantile(raw[reskey][year], q=quantiles['low'], axis=-1)
+                    reduced_analyzer.results[reskey][year].high = np.quantile(raw[reskey][year], q=quantiles['high'], axis=-1)
 
         return reduced_analyzer
 
 
-    def compute(self, key):
+    def compute_mismatch(self, key):
+        ''' Compute mismatch between analyzer results and datafile'''
+
         res = []
         resargs = self.result_args[key]
         results = self.results[key]
         for name, group in resargs.data.groupby(['genotype', 'year']):
             genotype = name[0]
-            year = str(name[1]) + '.0'
+            year = name[1]
             if 'genotype' in key:
                 sim_res = list(results[year][self.glabels.index(genotype)])
                 res.extend(sim_res)
             else:
                 sim_res = list(results[year])
                 res.extend(sim_res)
 
@@ -959,20 +968,20 @@
     def get_to_plot(self):
         ''' Get number of plots to make '''
 
         if len(self.results) == 0:
             errormsg = 'Cannot plot since no age results were recorded)'
             raise ValueError(errormsg)
         else:
-            dates_per_result = [len(rk['dates']) for rk in self.result_args.values()]
-            n_plots = sum(dates_per_result)
+            years_per_result = [len(rk['years']) for rk in self.result_args.values()]
+            n_plots = sum(years_per_result)
             to_plot_args = []
             for rkey in self.result_keys:
-                for date in self.result_args[rkey]['dates']:
-                    to_plot_args.append([rkey,date])
+                for year in self.result_args[rkey]['years']:
+                    to_plot_args.append([rkey,year])
         return n_plots, to_plot_args
 
 
     def plot_single(self, ax, rkey, date, by_genotype, plot_args=None, scatter_args=None):
         '''
         Function to plot a single age result for a single date. Requires an axis as
         input and will generally be called by a helper function rather than directly.
@@ -1010,15 +1019,15 @@
             ax.plot(x, resdict[date].T, color=resargs.color, **args.plot, label='Model')
             if ('data' in resargs.keys()) and (len(thisdatadf) > 0):
                 ydata = np.array(thisdatadf.value)
                 ax.scatter(x, ydata,  color=resargs.color, **args.scatter, label='Data')
 
         # Labels and legends
         ax.set_xlabel('Age')
-        ax.set_title(resargs.name+' - '+date.split('.')[0])
+        ax.set_title(f'{resargs.name} - {date}')
         ax.legend()
         pl.xticks(x, resargs.age_labels)
 
         return ax
 
 
 
@@ -1050,17 +1059,17 @@
 
         # Make the figure(s)
         with hpo.with_style(**kwargs):
             plot_count=1
             for rkey,resdict in self.results.items():
                 pl.subplots_adjust(**axis_args)
                 by_genotype=True if 'genotype' in rkey else False
-                for date in self.result_args[rkey]['dates']:
+                for year in self.result_args[rkey]['years']:
                     ax = pl.subplot(n_rows, n_cols, plot_count)
-                    ax = self.plot_single(ax, rkey, date, by_genotype, plot_args=plot_args, scatter_args=scatter_args)
+                    ax = self.plot_single(ax, rkey, year, by_genotype, plot_args=plot_args, scatter_args=scatter_args)
                     plot_count+=1
 
         return hppl.tidy_up(fig, do_save=do_save, fig_path=fig_path, do_show=do_show, args=all_args)
 
 
 class age_causal_infection(Analyzer):
     '''
```

### Comparing `hpvsim-1.1.1/hpvsim/base.py` & `hpvsim-1.2.0/hpvsim/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,18 +289,17 @@
         # Merge everything together
         pars = sc.mergedicts(pars, kwargs)
         if pars:
 
             # Handle other special parameters
             if pars.get('network'):
                 hppar.reset_layer_pars(pars, force=False)
-            location = 'nigeria'
             if pars.get('location'):
                 location = pars['location']
-            pars['birth_rates'], pars['death_rates'] = hppar.get_births_deaths(location=location) # Set birth and death rates
+                pars['birth_rates'], pars['death_rates'] = hppar.get_births_deaths(location=location) # Set birth and death rates
 
             # Call update_pars() for ParsObj
             super().update_pars(pars=pars, create=create)
 
         return
 
 
@@ -1377,55 +1376,46 @@
         people have inactive infection and no cancer.
         '''
         return (self.inactive * ~self.cancerous.any(axis=0)).astype(bool)
 
     @property
     def precin(self):
         '''
-        Boolean array of everyone with whose disease severity level does not meet the threshold for detectable cell changes
+        Boolean array of females with HPV whose disease severity level does not meet the threshold for detectable cell changes
         '''
-        return (self.sev < self.pars['clinical_cutoffs']['precin']).astype(bool)
+        return ((self.sex == 0) & self.infectious & (np.isnan(self.sev) | (self.sev==0))).astype(bool)
 
     @property
     def cin1(self):
         '''
-        Boolean array of everyone with whose disease severity level lies within the thresholds for CIN1-level cell changes
+        Boolean array of females with HPV whose disease severity level lies within the thresholds for CIN1-level cell changes
         '''
-        return ((self.sev >= self.pars['clinical_cutoffs']['precin']) * (
-                 self.sev < self.pars['clinical_cutoffs']['cin1'])).astype(bool)
+        return ((self.sex == 0) * (self.sev > 0) * (self.sev < self.pars['clinical_cutoffs']['cin1'])).astype(bool)
 
     @property
     def cin2(self):
         '''
-        Boolean array of everyone with whose disease severity level lies within the thresholds for CIN2-level cell changes
+        Boolean array of females with HPV whose disease severity level lies within the thresholds for CIN2-level cell changes
         '''
-        return ((self.sev >= self.pars['clinical_cutoffs']['cin1']) * (
+        return ((self.sex == 0) * (self.sev >= self.pars['clinical_cutoffs']['cin1']) * (
                  self.sev < self.pars['clinical_cutoffs']['cin2'])).astype(bool)
 
     @property
     def cin3(self):
         '''
-        Boolean array of everyone with whose disease severity level lies within the thresholds for CIN3-level cell changes
+        Boolean array of females with HPV whose disease severity level lies within the thresholds for CIN3-level cell changes
         '''
-        return ((self.sev >= self.pars['clinical_cutoffs']['cin2']) * (
-                 self.sev < self.pars['clinical_cutoffs']['cin3'])).astype(bool)
-
-    @property
-    def carcinoma(self):
-        '''
-        Boolean array of everyone with whose disease severity level lies within the thresholds for carcinoma in situ
-        '''
-        return (self.sev >= self.pars['clinical_cutoffs']['cin3']).astype(bool)
+        return ((self.sex == 0) * (self.sev >= self.pars['clinical_cutoffs']['cin2'])).astype(bool)
 
     @property
     def cin(self):
         '''
-        Boolean array of everyone with whose disease severity level meets the threshold for detectable cell changes
+        Boolean array of females with HPV whose disease severity level meets the threshold for detectable cell changes
         '''
-        return (self.sev >= self.pars['clinical_cutoffs']['precin']).astype(bool)
+        return (self.sev>0).astype(bool)
 
     def true(self, key):
         ''' Return indices matching the condition '''
         return self[key].nonzero()[-1]
 
     def true_by_genotype(self, key, genotype):
         ''' Return indices matching genotype-condition'''
```

### Comparing `hpvsim-1.1.1/hpvsim/calibration.py` & `hpvsim-1.2.0/hpvsim/calibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                                            'test_data/south_africa_cancer_data.xlsx'],
                                 total_trials=10, n_workers=4)
         calib.calibrate()
         calib.plot()
 
     '''
 
-    def __init__(self, sim, datafiles, calib_pars=None, genotype_pars=None, hiv_pars=None, fit_args=None, extra_sim_results=None,
+    def __init__(self, sim, datafiles, calib_pars=None, genotype_pars=None, hiv_pars=None, fit_args=None, extra_sim_result_keys=None,
                  par_samplers=None, n_trials=None, n_workers=None, total_trials=None, name=None, db_name=None,
                  keep_db=None, storage=None, rand_seed=None, label=None, die=False, verbose=True):
 
         import multiprocessing as mp # Import here since it's also slow
 
         # Handle run arguments
         if n_trials  is None: n_trials  = 20
@@ -93,37 +93,28 @@
 
         # Handle other inputs
         self.label          = label
         self.sim            = sim
         self.calib_pars     = calib_pars
         self.genotype_pars  = genotype_pars
         self.hiv_pars       = hiv_pars
-        self.extra_sim_results = extra_sim_results
+        self.extra_sim_result_keys = extra_sim_result_keys
         self.fit_args       = sc.mergedicts(fit_args)
         self.par_samplers   = sc.mergedicts(par_samplers)
         self.die            = die
         self.verbose        = verbose
         self.calibrated     = False
 
         # Create age_results intervention
         self.target_data = []
         for datafile in datafiles:
             self.target_data.append(hpm.load_data(datafile))
 
         sim_results = sc.objdict()
-
         age_result_args = sc.objdict()
-        extra_sim_results = sc.objdict()
-
-        if self.extra_sim_results:
-            for extra_result in self.extra_sim_results:
-                extra_sim_results[extra_result] = sc.objdict()
-            self.extra_sim_results_keys = extra_sim_results.keys()
-        else:
-            self.extra_sim_results_keys = None
 
         # Go through each of the target keys and determine how we are going to get the results from sim
         for targ in self.target_data:
             targ_keys = targ.name.unique()
             if len(targ_keys) > 1:
                 errormsg = f'Only support one set of targets per datafile, {len(targ_keys)} provided'
                 raise ValueError(errormsg)
@@ -156,32 +147,33 @@
             if 'hiv' in rkey:
                 self.result_args[rkey].name = self.sim.hivsim.results[rkey].name
                 self.result_args[rkey].color = self.sim.hivsim.results[rkey].color
             else:
                 self.result_args[rkey].name = self.sim.results[rkey].name
                 self.result_args[rkey].color = self.sim.results[rkey].color
 
-        if self.extra_sim_results:
-            for rkey in self.extra_sim_results_keys:
+        if self.extra_sim_result_keys:
+            for rkey in self.extra_sim_result_keys:
                 self.result_args[rkey] = sc.objdict()
                 self.result_args[rkey].name = self.sim.results[rkey].name
                 self.result_args[rkey].color = self.sim.results[rkey].color
         # Temporarily store a filename
         self.tmp_filename = 'tmp_calibration_%05i.obj'
 
         return
 
 
     def run_sim(self, calib_pars=None, genotype_pars=None, hiv_pars=None, label=None, return_sim=False):
         ''' Create and run a simulation '''
-        sim = self.sim.copy()
+        sim = sc.dcp(self.sim)
         if label: sim.label = label
 
         new_pars = self.get_full_pars(sim=sim, calib_pars=calib_pars, genotype_pars=genotype_pars, hiv_pars=hiv_pars)
         sim.update_pars(new_pars)
+        sim.initialize(reset=True, init_analyzers=False) # Necessary to reinitialize the sim here so that the initial infections get the right parameters
 
         # Run the sim
         try:
             sim.run()
             if return_sim:
                 return sim
             else:
@@ -390,39 +382,53 @@
         '''
         Take in an optuna trial and sample from pars, after extracting them from the structure they're provided in
         '''
         pars = {}
         for key, val in pardict.items():
             if isinstance(val, list):
                 low, high = val[1], val[2]
+                if (len(val)>3):
+                    step = val[3]
+                else:
+                    step=None
                 if key in self.par_samplers:  # If a custom sampler is used, get it now
                     try:
                         sampler_fn = getattr(trial, self.par_samplers[key])
                     except Exception as E:
                         errormsg = 'The requested sampler function is not found: ensure it is a valid attribute of an Optuna Trial object'
                         raise AttributeError(errormsg) from E
                 else:
                     sampler_fn = trial.suggest_float
                 if gname is not None:
                     sampler_key = gname + '_' + key
                 else:
                     sampler_key = key
-                pars[key] = sampler_fn(sampler_key, low, high)  # Sample from values within this range
+                pars[key] = sampler_fn(sampler_key, low, high, step=step)  # Sample from values within this range
 
             elif isinstance(val, dict):
                 sampler_fn = trial.suggest_float
                 pars[key] = dict()
                 for parkey, par_highlowlist in val.items():
                     if gname is not None:
                         sampler_key = gname + '_' + key + '_' + parkey
                     else:
                         sampler_key = key + '_' + parkey
                     if isinstance(par_highlowlist, dict):
                         par_highlowlist = par_highlowlist['value']
-                    pars[key][parkey] = sampler_fn(sampler_key, par_highlowlist[1], par_highlowlist[2])
+                        low, high = par_highlowlist[1], par_highlowlist[2]
+                        if (len(par_highlowlist) > 3):
+                            step = par_highlowlist[3]
+                        else: step = None
+                    elif isinstance(par_highlowlist, list):
+                        low, high = par_highlowlist[1], par_highlowlist[2]
+                        if (len(par_highlowlist) > 3):
+                            step = par_highlowlist[3]
+                        else:
+                            step = None
+                    pars[key][parkey] = sampler_fn(sampler_key, low, high, step=step)
 
         return pars
 
 
     def run_trial(self, trial, save=True):
         ''' Define the objective for Optuna '''
 
@@ -439,28 +445,31 @@
         if self.calib_pars is not None:
             calib_pars = self.trial_to_sim_pars(self.calib_pars, trial)
         else:
             calib_pars = None
 
         sim = self.run_sim(calib_pars, genotype_pars, hiv_pars, return_sim=True)
 
-        # Compute fit for sim results and save sim results (TODO: THIS IS BY GENOTYPE FOR A SINGLE TIMEPOINT. GENERALIZE THIS)
+        # Compute fit for sim results and save sim results (TODO: THIS IS FOR A SINGLE TIMEPOINT. GENERALIZE THIS)
         sim_results = sc.objdict()
         for rkey in self.sim_results:
-            model_output = sim.results[rkey][:,self.sim_results[rkey].timepoints[0]]
+            if sim.results[rkey][:].ndim==1:
+                model_output = sim.results[rkey][self.sim_results[rkey].timepoints[0]]
+            else:
+                model_output = sim.results[rkey][:,self.sim_results[rkey].timepoints[0]]
             diffs = self.sim_results[rkey].data.value - model_output
             gofs = hpm.compute_gof(self.sim_results[rkey].data.value, model_output)
             losses = gofs * self.sim_results[rkey].weights
             mismatch = losses.sum()
             sim.fit += mismatch
             sim_results[rkey] = model_output
 
         extra_sim_results = sc.objdict()
-        if self.extra_sim_results:
-            for rkey in self.extra_sim_results_keys:
+        if self.extra_sim_result_keys:
+            for rkey in self.extra_sim_result_keys:
                 model_output = sim.results[rkey]
                 extra_sim_results[rkey] = model_output
 
         # Store results in temporary files (TODO: consider alternatives)
         if save:
             results = dict(sim=sim_results, analyzer=sim.get_analyzer().results, extra_sim_results=extra_sim_results)
             filename = self.tmp_filename % trial.number
@@ -560,14 +569,15 @@
         sim = self.sim # TODO: make sure this is OK #sc.jsonpickle(self.study.trials[0].user_attrs['jsonpickle_sim'])
         self.ng = sim['n_genotypes']
         self.glabels = [g.upper() for g in sim['genotype_map'].values()]
 
         # Replace with something else, this is fragile
         self.analyzer_results = []
         self.sim_results = []
+        self.extra_sim_results = []
         if load:
             print('Loading saved results...')
             for trial in study.trials:
                 n = trial.number
                 try:
                     filename = self.tmp_filename % trial.number
                     results = sc.load(filename)
@@ -699,17 +709,18 @@
             dates_per_result = [len(date_list) for date_list in all_dates]
             other_results = len(sim_results[0].keys())
             n_plots = sum(dates_per_result) + other_results
             n_rows, n_cols = sc.get_rows_cols(n_plots)
 
         # Initialize
         fig, axes = pl.subplots(n_rows, n_cols, **fig_args)
-        for ax in axes.flat[n_plots:]:
-            ax.set_visible(False)
-        axes = axes.flatten()
+        if n_plots>1:
+            for ax in axes.flat[n_plots:]:
+                ax.set_visible(False)
+            axes = axes.flatten()
         pl.subplots_adjust(**axis_args)
 
         # Pull out attributes that don't vary by run
         age_labels = sc.objdict()
         for resname,resdict in zip(self.age_results_keys, analyzer_results[0].values()):
             age_labels[resname] = [str(int(resdict['bins'][i])) + '-' + str(int(resdict['bins'][i + 1])) for i in range(len(resdict['bins']) - 1)]
             age_labels[resname].append(str(int(resdict['bins'][-1])) + '+')
@@ -726,15 +737,18 @@
             plot_count = 0
             for rn, resname in enumerate(self.age_results_keys):
                 x = np.arange(len(age_labels[resname]))  # the label locations
 
                 for date in all_dates[rn]:
 
                     # Initialize axis and data storage structures
-                    ax = axes[plot_count]
+                    if n_plots>1:
+                        ax = axes[plot_count]
+                    else:
+                        ax = axes
                     bins = []
                     genotypes = []
                     values = []
 
                     # Pull out data
                     thisdatadf = self.target_data[rn][(self.target_data[rn].year == float(date)) & (self.target_data[rn].name == resname)]
                     unique_genotypes = thisdatadf.genotype.unique()
@@ -770,39 +784,45 @@
 
                         # Plot model
                         modeldf = pd.DataFrame({'bins':bins, 'values':values})
                         ax = plot_func(ax=ax, x='bins', y='values', data=modeldf, color=self.result_args[resname].color, **extra_args)
 
                     # Set title and labels
                     ax.set_xlabel('Age group')
-                    ax.set_title(self.result_args[resname].name+', '+ date.replace('.0', ''))
+                    ax.set_title(f'{self.result_args[resname].name}, {date}')
                     ax.legend()
                     ax.set_xticks(x, age_labels[resname])
                     plot_count += 1
 
             for rn, resname in enumerate(self.sim_results_keys):
-                x = np.arange(len(self.glabels))
-                ax = axes[plot_count]
-                bins = []
-                values = []
+                if n_plots > 1:
+                    ax = axes[plot_count]
+                else:
+                    ax = axes
+                bins = sc.autolist()
+                values = sc.autolist()
                 thisdatadf = self.target_data[rn+sum(dates_per_result)][self.target_data[rn + sum(dates_per_result)].name == resname]
                 ydata = np.array(thisdatadf.value)
+                x = np.arange(len(ydata))
                 ax.scatter(x, ydata, color=pl.cm.Reds(0.95), marker='s', label='Data')
 
-
                 # Construct a dataframe with things in the most logical order for plotting
                 for run_num, run in enumerate(sim_results):
                     bins += x.tolist()
-                    values += list(run[resname])
+                    if sc.isnumber(run[resname]):
+                        values += sc.promotetolist(run[resname])
+                    else:
+                        values += run[resname].tolist()
+
                 # Plot model
                 modeldf = pd.DataFrame({'bins': bins, 'values': values})
                 ax = plot_func(ax=ax, x='bins', y='values', data=modeldf, **extra_args)
 
                 # Set title and labels
                 date = thisdatadf.year[0]
-                ax.set_xlabel('Genotype')
+                # ax.set_xlabel('Genotype')
                 ax.set_title(self.result_args[resname].name + ', ' + str(date))
                 ax.legend()
-                ax.set_xticks(x, self.glabels)
+                # ax.set_xticks(x, self.glabels)
                 plot_count += 1
 
         return hppl.tidy_up(fig, do_save=do_save, fig_path=fig_path, do_show=do_show, args=all_args)
```

### Comparing `hpvsim-1.1.1/hpvsim/data/get_data.py` & `hpvsim-1.2.0/hpvsim/data/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     ''' Download pre-processed data files '''
     if verbose:
         sc.heading('Downloading preprocessed HPVsim data')
         if init:
             print('Note: this automatic download only happens once, when HPVsim is first run.\n\n')
     filepath = sc.makefilepath(filesdir / f'tmp_{data_file}.zip')
     sc.download(url=quick_url, filename=filepath, convert=False, verbose=verbose)
-    sc.loadzip(filepath, outfolder=filesdir)
+    sc.unzip(filepath, outfolder=filesdir)
     sc.rmpath(filepath)
     if verbose:
         print('\nData downloaded.')
     return
 
 
 def check_downloaded(verbose=1, check_version=True):
```

### Comparing `hpvsim-1.1.1/hpvsim/data/loaders.py` & `hpvsim-1.2.0/hpvsim/data/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,19 @@
     ''' Define aliases for countries with odd names in the data '''
     country_mappings = {
        'Bolivia':        'Bolivia (Plurinational State of)',
        'Burkina':        'Burkina Faso',
        'Cape Verde':     'Cabo Verdeo',
        'Hong Kong':      'China, Hong Kong Special Administrative Region',
        'Macao':          'China, Macao Special Administrative Region',
-       "Cote d'Ivoire":  'Côte d’Ivoire',
-       "Ivory Coast":    'Côte d’Ivoire',
+       "Cote d'Ivoire":  "Côte d'Ivoire",
+       "Cote dIvoire":   "Côte d'Ivoire",
+       "Ivory Coast":    "Côte d'Ivoire",
        'DRC':            'Democratic Republic of the Congo',
+       'Congo':          'Congo, Rep.',
        'Iran':           'Iran (Islamic Republic of)',
        'Laos':           "Lao People's Democratic Republic",
        'Micronesia':     'Micronesia (Federated States of)',
        'Korea':          'Republic of Korea',
        'South Korea':    'Republic of Korea',
        'Moldova':        'Republic of Moldova',
        'Russia':         'Russian Federation',
@@ -86,14 +88,16 @@
         }
 
     # Slightly different aliases for WB data
     if wb:
         for key,val in country_mappings.items():
             if val == 'Democratic Republic of the Congo':
                 country_mappings[key] = 'Congo, Dem. Rep.'
+            if val in ["Cote d'Ivoire", "Cote dIvoire", "Côte d'Ivoire"]:
+                country_mappings[key] = "Cote d'Ivoire"
 
     return country_mappings # Convert to lowercase
 
 
 def map_entries(json, location, df=None, wb=False):
     '''
     Find a match between the JSON file and the provided location(s).
```

### Comparing `hpvsim-1.1.1/hpvsim/defaults.py` & `hpvsim-1.2.0/hpvsim/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,17 @@
             State('uid',            default_int),           # Int
             State('scale',          default_float,  1.0), # Float
             State('level0',         bool,  True), # "Normal" people
             State('level1',         bool,  False), # "High-resolution" people: e.g. cancer agents
             State('age',            default_float,  np.nan), # Float
             State('sex',            default_float,  np.nan), # Float
             State('debut',          default_float,  np.nan), # Float
+            State('ever_partnered', bool,  False), # Whether this person has ever been partnered
             State('sev',            default_float, np.nan, shape='n_genotypes'), # Severity of infection, taking values between 0-1
-            State('rel_sev',        default_float, 1.0), # Individual relative risk for rate severe disease growth (does not vary by genotype)
+            State('rel_sev',        default_float, 1.0), # Individual relative risk for rate severe disease growth
             State('rel_sus',        default_float, 1.0), # Individual relative risk for acquiring infection (does not vary by genotype)
             State('rel_imm',        default_float, 1.0), # Individual relative level of immunity acquired from infection clearance/vaccination
             State('doses',          default_int,    0),  # Number of doses of the prophylactic vaccine given per person
             State('txvx_doses',     default_int,    0),  # Number of doses of the therapeutic vaccine given per person
             State('vaccine_source', default_int,    -1), # Index of the prophylactic vaccine that individual received
             State('screens',        default_int,    0),  # Number of screens given per person
             State('cin_treatments', default_int,    0),  # Number of CIN treatments given per person
@@ -124,16 +125,15 @@
             State('infected',   bool, False, 'n_genotypes', label='Number infected', color='#c78f65'), # Union of infectious and inactive. Includes people with cancer, people with latent infections, and people with active infections
             State('abnormal',   bool, False, 'n_genotypes', label='Number with abnormal cells', color='#9e1149'),  # Union of episomal, transformed, and cancerous. Allowable viral states: infectious
             State('latent',     bool, False, 'n_genotypes', label='Number with latent infection', color='#5f5cd2'), # Intersection of normal and inactive.
             State('precin',     bool, False, 'n_genotypes', label='Number with precin', color='#9e1149'), # Defined as those with sev < clinical_cuttoff[0]
             State('cin1',       bool, False, 'n_genotypes', label='Number with cin1', color='#9e1149'), # Defined as those with clinical_cuttoff[0] < sev < clinical_cuttoff[1]
             State('cin2',       bool, False, 'n_genotypes', label='Number with cin2', color='#9e1149'), # Defined as those with clinical_cuttoff[1] < sev < clinical_cuttoff[2]
             State('cin3',       bool, False, 'n_genotypes', label='Number with cin3', color='#5f5cd2'), # Defined as those with clinical_cuttoff[2] < sev < clinical_cuttoff[3]
-            State('carcinoma',  bool, False, 'n_genotypes', label='Number with carcinoma in situ', color='#5f5cd2'), # Defined as those with clinical_cuttoff[3] < sev < clinical_cuttoff[4]
-            State('cin',        bool, False, 'n_genotypes', label='Number with detectable dysplasia', color='#5f5cd2'), # Union of CIN1, CIN3, CIN3, and carcinoma in situ
+            State('cin',        bool, False, 'n_genotypes', label='Number with detectable dysplasia', color='#5f5cd2'), # Union of CIN1, CIN3, and CIN3
         ]
 
         # Additional intervention states
         self.intv_states = [
             State('detected_cancer',    bool,   False, label='Number with detected cancer'), # Whether the person's cancer has been detected
             State('screened',           bool,   False, label='Number screened'), # Whether the person has been screened (how does this change over time?)
             State('cin_treated',        bool,   False, label='Number treated for precancerous lesions'), # Whether the person has been treated for CINs
@@ -144,14 +144,15 @@
 
         # Any other stock states - add a placeholder here to be populated later
         self.other_stock_states = []
 
         # Immune states, by genotype/vaccine
         self.imm_states = [
             State('sus_imm',        default_float,  0,'n_imm_sources'),  # Float, by genotype
+            State('sev_imm',        default_float,  0, 'n_imm_sources'),  # Float, by genotype
             State('peak_imm',       default_float,  0,'n_imm_sources'),  # Float, peak level of immunity
             State('nab_imm',        default_float,  0,'n_imm_sources'),  # Float, current immunity level
             State('t_imm_event',    default_int,    0,'n_imm_sources'),  # Int, time since immunity event
             State('cell_imm',       default_float,  0,'n_imm_sources'),
         ]
 
         # Relationship states
@@ -192,14 +193,15 @@
     @property
     def dates(self):
         ''' Dates are stored for all states except susceptible, and alive, and normal (which are True by default) '''
         dates = [State(f'date_{state.name}', default_float, np.nan, shape=state.shape) for state in self.date_states]
         dates += [
             State('date_clearance', default_float, np.nan, shape='n_genotypes'),
             State('date_exposed', default_float, np.nan, shape='n_genotypes'),
+            State('date_reactivated', default_float, np.nan, shape='n_genotypes'),
         ]
         return dates
 
     # All states
     @property
     def all_states(self):
         return self.person + self.alive_states + self.viral_states + self.cell_states + self.derived_states + self.intv_states + self.other_stock_states + self.imm_states + self.rship_states + self.durs
```

### Comparing `hpvsim-1.1.1/hpvsim/hiv.py` & `hpvsim-1.2.0/hpvsim/hiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             output = hpb.Result(*args, **kwargs, npts=sim.res_npts)
             return output
 
         self.resfreq = sim.resfreq
         # Initialize storage
         results = sc.objdict()
 
-        na = len(sim['age_bins']) - 1  # Number of age bins
+        na = len(sim['age_bin_edges']) - 1  # Number of age bins
 
         stock_colors = [i for i in set(sim.people.meta.stock_colors) if i is not None]
 
         results['hiv_infections'] = init_res('New HIV infections')
         results['hiv_infections_by_age'] = init_res('New HIV infections by age', n_rows=na, color=stock_colors[0])
         results['n_hiv'] = init_res('Number living with HIV', color=stock_colors[0])
         results['n_hiv_by_age'] = init_res('Number living with HIV by age', n_rows=na, color=stock_colors[0])
@@ -200,15 +200,15 @@
         filter_inds = people.true('hiv')
         inds = people.check_inds(people.dead_hiv, people.date_dead_hiv, filter_inds=filter_inds)
 
         # Remove people and update flows
         people.remove_people(inds, cause='hiv')
         idx = int(people.t / self.resfreq)
         if len(inds):
-            deaths_by_age = np.histogram(people.age[inds], bins=people.age_bins, weights=people.scale[inds])[0]
+            deaths_by_age = np.histogram(people.age[inds], bins=people.age_bin_edges, weights=people.scale[inds])[0]
             self.results['hiv_deaths'][idx] += people.scale_flows(inds)
             self.results['hiv_deaths_by_age'][:, idx] += deaths_by_age
 
         return
 
 
     def update_cd4(self, people):
@@ -322,55 +322,55 @@
         ''' Update the HIV results '''
 
         idx = int(people.t / self.resfreq)
 
         #### Calculate flows
         # Flows get accumulated *every* time step
         self.results['hiv_infections'][idx] += people.scale_flows(hiv_inds)
-        self.results['hiv_infections_by_age'][:, idx] += np.histogram(people.age[hiv_inds], bins=people.age_bins, weights=people.scale[hiv_inds])[0]
+        self.results['hiv_infections_by_age'][:, idx] += np.histogram(people.age[hiv_inds], bins=people.age_bin_edges, weights=people.scale[hiv_inds])[0]
 
         # Pull out those with cancer and HIV+
         cancer_today_inds = hpu.true(people.date_cancerous == people.t)
         if len(cancer_today_inds):
             hiv_bools = people.hiv[cancer_today_inds]
             cancer_today_hiv_pos_inds = cancer_today_inds[hiv_bools]
             cancer_today_hiv_neg_inds = cancer_today_inds[~hiv_bools]
             self.results['cancers_with_hiv'][idx] = people.scale_flows(cancer_today_hiv_pos_inds)
             self.results['cancers_no_hiv'][idx] = people.scale_flows(cancer_today_hiv_neg_inds)
             self.results['cancers_by_age_with_hiv'][:, idx] = \
-            np.histogram(people.age[cancer_today_hiv_pos_inds], bins=people.age_bins,
+            np.histogram(people.age[cancer_today_hiv_pos_inds], bins=people.age_bin_edges,
                          weights=people.scale[cancer_today_hiv_pos_inds])[0]
             self.results['cancers_by_age_no_hiv'][:, idx] = \
-            np.histogram(people.age[cancer_today_hiv_neg_inds], bins=people.age_bins,
+            np.histogram(people.age[cancer_today_hiv_neg_inds], bins=people.age_bin_edges,
                          weights=people.scale[cancer_today_hiv_neg_inds])[0]
 
         #### Calculate stocks
         # Stocks only get accumulated every nth time step, where n is the result frequency
         if people.t % self.resfreq == self.resfreq - 1:
 
             self.results['n_hiv'][idx] = people.count('hiv')
             hivinds = hpu.true(people['hiv'])
-            self.results['n_hiv_by_age'][:, idx] = np.histogram(people.age[hivinds], bins=people.age_bins, weights=people.scale[hivinds])[0]
+            self.results['n_hiv_by_age'][:, idx] = np.histogram(people.age[hivinds], bins=people.age_bin_edges, weights=people.scale[hivinds])[0]
             self.results['n_art'][idx] = people.count('art')
 
             # Pull out those with HPV and HIV+
             hpvhivinds = hpu.true((people['hiv']) & people['infectious'])
-            self.results['n_hpv_by_age_with_hiv'][:, idx] = np.histogram(people.age[hpvhivinds], bins=people.age_bins, weights=people.scale[hpvhivinds])[0]
+            self.results['n_hpv_by_age_with_hiv'][:, idx] = np.histogram(people.age[hpvhivinds], bins=people.age_bin_edges, weights=people.scale[hpvhivinds])[0]
 
             # Pull out those with HPV and HIV-
             hpvnohivinds = hpu.true(~(people['hiv']) & people['infectious'])
-            self.results['n_hpv_by_age_no_hiv'][:, idx] = np.histogram(people.age[hpvnohivinds], bins=people.age_bins, weights=people.scale[hpvnohivinds])[0]
+            self.results['n_hpv_by_age_no_hiv'][:, idx] = np.histogram(people.age[hpvnohivinds], bins=people.age_bin_edges, weights=people.scale[hpvnohivinds])[0]
 
             alive_female_hiv_inds = hpu.true(people.alive*people.is_female*people.hiv)
             self.results['n_females_with_hiv_alive'][idx] = people.scale_flows(alive_female_hiv_inds)
-            self.results['n_females_with_hiv_alive_by_age'][:, idx] = np.histogram(people.age[alive_female_hiv_inds], bins=people.age_bins,
+            self.results['n_females_with_hiv_alive_by_age'][:, idx] = np.histogram(people.age[alive_female_hiv_inds], bins=people.age_bin_edges,
                  weights=people.scale[alive_female_hiv_inds])[0]
             alive_female_no_hiv_inds = hpu.true(people.alive * people.is_female * ~people.hiv)
             self.results['n_females_no_hiv_alive'][idx] = people.scale_flows(alive_female_no_hiv_inds)
-            self.results['n_females_no_hiv_alive_by_age'][:, idx] = np.histogram(people.age[alive_female_no_hiv_inds], bins=people.age_bins,
+            self.results['n_females_no_hiv_alive_by_age'][:, idx] = np.histogram(people.age[alive_female_no_hiv_inds], bins=people.age_bin_edges,
                  weights=people.scale[alive_female_no_hiv_inds])[0]
         return
 
 
     def get_hiv_data(self, hiv_datafile=None, art_datafile=None):
         '''
         Load HIV incidence and art coverage data, if provided
```

### Comparing `hpvsim-1.1.1/hpvsim/immunity.py` & `hpvsim-1.2.0/hpvsim/immunity.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,69 +15,133 @@
 
 def init_immunity(sim, create=True):
     ''' Initialize immunity matrices with all genotypes and vaccines in the sim'''
 
     # Pull out all of the circulating genotypes for cross-immunity
     ng = sim['n_genotypes']
 
-    # Pull out all the vaccination interventions
+    # Pull out all the unique vaccine products
     vx_intvs = [x for x in sim['interventions'] if isinstance(x, hpi.BaseVaccination)]
-    nv = len(vx_intvs)
+    vx_intv_prods = [x.product.genotype_pars['name'].values[0] for x in vx_intvs]
+    unique_vx_prods, unique_vx_prod_inds = np.unique(vx_intv_prods, return_index=True)
+    unique_vx_prod_dict = dict()
+    for unique_vx_prod, unique_vx_prod_ind in zip(unique_vx_prods, unique_vx_prod_inds):
+        unique_vx_prod_dict[unique_vx_prod] = unique_vx_prod_ind
+    nv = len(unique_vx_prods) if len(vx_intvs) else 0
+
+    unique_vx_intvs = sc.autolist()
+    for ind in unique_vx_prod_inds:
+        unique_vx_intvs += vx_intvs[ind]
+
+    for iv, vx_intv in enumerate(vx_intvs):
+        vx_intv.product.imm_source = unique_vx_prod_dict[vx_intv_prods[iv]]+ng
+
+    txv_intvs = [x for x in sim['interventions'] if isinstance(x, hpi.BaseTxVx)]
+    txv_intv_prods = [x.product.name.replace('2', '1') for x in txv_intvs]
+    unique_txv_prods, unique_txv_prod_inds = np.unique(txv_intv_prods, return_index=True)
+    unique_txv_prod_dict = dict()
+    for unique_txv_prod, unique_txv_prod_ind in zip(unique_txv_prods, unique_txv_prod_inds):
+        unique_txv_prod_dict[unique_txv_prod] = unique_txv_prod_ind
+    ntxv = len(unique_txv_prods) if len(txv_intvs) else 0
+
+    unique_txv_intvs = sc.autolist()
+    for ind in unique_txv_prod_inds:
+        unique_txv_intvs += txv_intvs[ind]
+
+    for itxv, txv_intv in enumerate(txv_intvs):
+        txv_intv.product.imm_source = unique_txv_prod_dict[txv_intv_prods[itxv]] + ng + nv
+
+    all_vx_intvs = unique_vx_intvs + unique_txv_intvs
 
     # Dimension for immunity matrix
-    ndim = ng + nv
+    ndim = ng + nv + ntxv
+
+    # If cross-immunity values have been provided, process them
+    if sim['cross_immunity_sus'] is None or create:
+
+        # Precompute waning - same for all genotypes
+        if sim['use_waning']:
+            imm_decay = sc.dcp(sim['imm_decay'])
+            if 'half_life' in imm_decay.keys():
+                imm_decay['half_life'] /= sim['dt']
+            sim['imm_kin'] = precompute_waning(t=sim.tvec, pars=imm_decay)
+
+        sim['immunity_map'] = dict()
+        # Firstly, initialize immunity matrix with defaults. These are then overwitten with specific values below
+        immunity = np.ones((ng, ng), dtype=hpd.default_float)  # Fill with defaults
+
+        # Next, overwrite these defaults with any known immunity values about specific genotypes
+        default_cross_immunity = hppar.get_cross_immunity(cross_imm_med=sim['cross_imm_sus_med'], cross_imm_high=sim['cross_imm_sus_high'],
+                                                          own_imm_hr=sim['own_imm_hr'])
+        for i in range(ng):
+            sim['immunity_map'][i] = 'infection'
+            label_i = sim['genotype_map'][i]
+            for j in range(ng):
+                label_j = sim['genotype_map'][j]
+                if label_i in default_cross_immunity and label_j in default_cross_immunity:
+                    immunity[j][i] = default_cross_immunity[label_j][label_i]
+
+        for vi,vx_intv in enumerate(all_vx_intvs):
+            genotype_pars_df = vx_intv.product.genotype_pars[vx_intv.product.genotype_pars.genotype.isin(sim['genotype_map'].values())] # TODO fix this
+            vacc_mapping = [genotype_pars_df[genotype_pars_df.genotype==gtype].rel_imm.values[0] for gtype in sim['genotype_map'].values()]
+            vacc_mapping += [1]*(vi+1) # Add on some ones to pad out the matrix
+            vacc_mapping = np.reshape(vacc_mapping, (len(immunity)+1, 1)).astype(hpd.default_float) # Reshape
+            immunity = np.hstack((immunity, vacc_mapping[0:len(immunity),]))
+            immunity = np.vstack((immunity, np.transpose(vacc_mapping)))
+
+        sim['cross_immunity_sus'] = immunity
+
 
-    # If immunity values have been provided, process them
-    if sim['immunity'] is None or create:
+    # If cross-immunity values have been provided, process them
+    if sim['cross_immunity_sev'] is None or create:
 
         # Precompute waning - same for all genotypes
         if sim['use_waning']:
             imm_decay = sc.dcp(sim['imm_decay'])
             if 'half_life' in imm_decay.keys():
                 imm_decay['half_life'] /= sim['dt']
             sim['imm_kin'] = precompute_waning(t=sim.tvec, pars=imm_decay)
 
         sim['immunity_map'] = dict()
         # Firstly, initialize immunity matrix with defaults. These are then overwitten with specific values below
         immunity = np.ones((ng, ng), dtype=hpd.default_float)  # Fill with defaults
 
         # Next, overwrite these defaults with any known immunity values about specific genotypes
-        default_cross_immunity = hppar.get_cross_immunity(cross_imm_med=sim['cross_imm_med'], cross_imm_high=sim['cross_imm_high'])
+        default_cross_immunity = hppar.get_cross_immunity(cross_imm_med=sim['cross_imm_sev_med'], cross_imm_high=sim['cross_imm_sev_high'],
+                                                          own_imm_hr=sim['own_imm_hr'])
         for i in range(ng):
             sim['immunity_map'][i] = 'infection'
             label_i = sim['genotype_map'][i]
             for j in range(ng):
                 label_j = sim['genotype_map'][j]
                 if label_i in default_cross_immunity and label_j in default_cross_immunity:
                     immunity[j][i] = default_cross_immunity[label_j][label_i]
 
-        imm_source = ng
-        for vi,vx_intv in enumerate(vx_intvs):
+        for vi,vx_intv in enumerate(all_vx_intvs):
             genotype_pars_df = vx_intv.product.genotype_pars[vx_intv.product.genotype_pars.genotype.isin(sim['genotype_map'].values())] # TODO fix this
             vacc_mapping = [genotype_pars_df[genotype_pars_df.genotype==gtype].rel_imm.values[0] for gtype in sim['genotype_map'].values()]
             vacc_mapping += [1]*(vi+1) # Add on some ones to pad out the matrix
             vacc_mapping = np.reshape(vacc_mapping, (len(immunity)+1, 1)).astype(hpd.default_float) # Reshape
             immunity = np.hstack((immunity, vacc_mapping[0:len(immunity),]))
             immunity = np.vstack((immunity, np.transpose(vacc_mapping)))
-            vx_intv.product.imm_source = imm_source
-            imm_source += 1
 
-        sim['immunity'] = immunity
+        sim['cross_immunity_sev'] = immunity
 
-    sim['immunity'] = sim['immunity'].astype('float32')
+    sim['cross_immunity_sus'] = sim['cross_immunity_sus'].astype('float32')
+    sim['cross_immunity_sev'] = sim['cross_immunity_sev'].astype('float32')
     sim['n_imm_sources'] = ndim
 
     return
 
 
 def update_peak_immunity(people, inds, imm_pars, imm_source, offset=None, infection=True):
     '''
         Update immunity level
 
-        This function updates the immunity for individuals when an infection or vaccination occurs.
+        This function updates the immunity for individuals when an infection is cleared or vaccination occurs.
             - individuals that are infected and already have immunity from a previous vaccination/infection have their immunity level;
             - individuals without prior immunity are assigned an initial level drawn from a distribution. This level
                 depends on whether the immunity is from a natural infection or from a vaccination (and if so, on the type of vaccine).
 
         Args:
             people: A people object
             inds: Array of people indices
@@ -105,15 +169,15 @@
             people.peak_imm[imm_source, prior_imm_inds] = np.maximum(new_peak, people.peak_imm[imm_source, prior_imm_inds])
 
             new_cell_imm = hpu.sample(**imm_pars['cell_imm_init'], size=len(prior_imm_inds))
             people.cell_imm[imm_source, prior_imm_inds] = np.maximum(new_cell_imm, people.cell_imm[imm_source, prior_imm_inds])
 
         if len(no_prior_imm_inds):
             people.peak_imm[imm_source, no_prior_imm_inds] = is_seroconvert[~has_imm] * hpu.sample(**imm_pars['imm_init'], size=len(no_prior_imm_inds)) * people.rel_imm[no_prior_imm_inds]
-            people.cell_imm[imm_source, no_prior_imm_inds] = is_seroconvert[~has_imm] * hpu.sample(**imm_pars['cell_imm_init'], size=len(no_prior_imm_inds))
+            people.cell_imm[imm_source, no_prior_imm_inds] = hpu.sample(**imm_pars['cell_imm_init'], size=len(no_prior_imm_inds)) * people.rel_imm[no_prior_imm_inds]
     else:
         # Vaccination by dose
         dose1_inds = inds[people.doses[inds]==1] # First doses
         dose2_inds = inds[people.doses[inds]==2] # Second doses
         dose3_inds = inds[people.doses[inds]>=3] # Third doses or beyond
         if imm_pars['doses']>1:
             imm_pars['imm_boost'] = sc.promotetolist(imm_pars['imm_boost'])
@@ -158,17 +222,20 @@
         people.sus_imm = np.array([[0.9 , 0.35, 0.  ],
                                    [0.27, 0.7 , 0.  ]])
 
     This indicates that the person 1 has high protection against reinfection with HPV16, and
     some (30% of 90%) protection against infection with HPV18, and so on.
 
     '''
-    immunity = people.pars['immunity'] # cross-immunity/own-immunity scalars to be applied to immunity level
-    sus_imm = np.dot(immunity,people.nab_imm) # Dot product gives immunity to all genotypes
-    people.sus_imm[:] = np.minimum(sus_imm, np.ones_like(sus_imm)) # Don't let this be above 1
+    cross_immunity_sus = people.pars['cross_immunity_sus'] # cross-immunity/own-immunity scalars to be applied to sus immunity level
+    cross_immunity_sev = people.pars['cross_immunity_sev'] # cross-immunity/own-immunity scalars to be applied to sev immunity level
+    sus_imm = np.dot(cross_immunity_sus, people.nab_imm) # Dot product gives immunity to all genotypes
+    sev_imm = np.dot(cross_immunity_sev, people.cell_imm)  # Dot product gives immunity to all genotypes
+    people.sus_imm[:] = np.minimum(sus_imm, np.ones_like(sus_imm))  # Don't let this be above 1
+    people.sev_imm[:] = np.minimum(sev_imm, np.ones_like(sev_imm))  # Don't let this be above 1
     return
 
 
 
 
 #%% Methods for computing waning
```

### Comparing `hpvsim-1.1.1/hpvsim/interventions.py` & `hpvsim-1.2.0/hpvsim/interventions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from . import utils as hpu
 from . import immunity as hpi
 from . import base as hpb
 from collections import defaultdict
 
 #%% Define data files
 datafiles = sc.objdict()
-for key in ['dx', 'tx', 'vx']:
+for key in ['dx', 'tx', 'vx', 'txvx']:
     datafiles[key] = hpd.datadir / f'products_{key}.csv'
 
 
 #%% Helper functions
 
 def find_timepoint(arr, t=None, interv=None, sim=None, which='first'):
     '''
@@ -574,15 +574,26 @@
         self.label = label
         self.eligibility = eligibility
         self._parse_product(product)
 
         # Deal with sex
         if sc.checktype(sex,'listlike'):
             if sc.checktype(sex[0],'str'): # If provided as ['f','m'], convert to [0,1]
-                self.sex = np.array([0,1])
+                sex_list = sc.autolist()
+                for isex in sex:
+                    if isex=='f':
+                        sex_list += 0
+                    elif isex=='m':
+                        sex_list += 1
+                    else:
+                        errormsg = f'Sex "{isex}" not understood.'
+                        raise ValueError(errormsg)
+                self.sex = sc.promotetoarray(sex_list)
+            else:
+                self.sex=sc.promotetoarray(sex)
         elif sc.checktype(sex, 'str'):  # If provided as 'f' or 'm', convert to 0 or 1
             if sex=='f':
                 self.sex = np.array([0])
             elif sex=='m':
                 self.sex = np.array([1])
             else:
                 errormsg = f'Sex "{sex}" not understood.'
@@ -1205,15 +1216,15 @@
     '''
     Campaign delivery of therapeutic vaccine - an instance of treat_num combined
     with campaign delivery. See base classes for a description of input arguments.
     '''
 
     def __init__(self, product=None, prob=None, age_range=None, eligibility=None,
                  years=None, interpolate=True, annual_prob=None, **kwargs):
-        BaseScreening.__init__(self, product=product, age_range=age_range, eligibility=eligibility, **kwargs)
+        BaseTxVx.__init__(self, product=product, age_range=age_range, eligibility=eligibility, **kwargs)
         CampaignDelivery.__init__(self, prob=prob, years=years, interpolate=interpolate, annual_prob=annual_prob)
 
     def initialize(self, sim):
         CampaignDelivery.initialize(self, sim) # Initialize this first, as it ensures that prob is interpolated properly
         BaseTxVx.initialize(self, sim) # Initialize this next - this actually calls BaseTreatment.initialize() and ensures products will be counted
 
     def apply(self, sim):
@@ -1303,18 +1314,22 @@
 
 
 class tx(Product):
     '''
     Treatment products include anything used to treat cancer or precancer, as well as therapeutic vaccination.
     They change fundamental properties about People, including their prognoses and infectiousness.
     '''
-    def __init__(self, df, clearance=0.8, name=None):
+    def __init__(self, df, clearance=0.8, genotype_pars=None, imm_init=None, imm_boost=None):
         self.df = df
         self.clearance = clearance
         self.name = df.name.unique()[0]
+        self.genotype_pars=genotype_pars
+        self.imm_init = imm_init
+        self.imm_boost = imm_boost
+        self.imm_source = None
         self.states = df.state.unique()
         self.genotypes = df.genotype.unique()
         self.ng = len(self.genotypes)
 
     def get_people_in_state(self, state, g, sim):
         '''
         Find people within a given state/genotype. Returns indices
@@ -1330,15 +1345,15 @@
 
         tx_successful = [] # Initialize list of successfully treated individuals
         people = sim.people
 
         for state in self.states: # Loop over states
             for g,genotype in sim['genotype_map'].items(): # Loop over genotypes in the sim
 
-                theseinds = inds[hpu.true(people[state][g, inds])] # Extract people for whom this state is true for this genotype]
+                theseinds = inds[hpu.true(people[state][g, inds])] # Extract people for whom this state is true for this genotype
 
                 if len(theseinds):
 
                     df_filter = (self.df.state == state)  # Filter by state
                     if self.ng>1: df_filter = df_filter & (self.df.genotype == genotype)
                     thisdf = self.df[df_filter] # apply filter to get the results for this state & genotype
 
@@ -1369,14 +1384,20 @@
         tx_successful = np.array(list(set(tx_successful)))
         tx_unsuccessful = np.setdiff1d(inds, tx_successful)
         if return_format=='dict':
             output = {'successful':tx_successful, 'unsuccessful': tx_unsuccessful}
         elif return_format=='array':
             output = tx_successful
 
+        if self.imm_init is not None:
+            people.cell_imm[self.imm_source, inds] = hpu.sample(**self.imm_init, size=len(inds))
+            people.t_imm_event[self.imm_source, inds] = people.t
+        elif self.imm_boost is not None:
+            people.cell_imm[self.imm_source, inds] *= self.imm_boost
+            people.t_imm_event[self.imm_source, inds] = people.t
         return output
 
 
 class vx(Product):
     ''' Vaccine product '''
     def __init__(self, genotype_pars=None, imm_init=None, imm_boost=None):
         self.genotype_pars = genotype_pars
@@ -1450,17 +1471,27 @@
 
 
 def default_tx(prod_name=None):
     '''
     Create default treatment products
     '''
     dftx = pd.read_csv(datafiles.tx) # Read in dataframe with parameters
+    dftxvx = pd.read_csv(datafiles.txvx)
     txprods = dict()
     for name in dftx.name.unique():
-        txprods[name] = tx(dftx[dftx.name==name])
+        if name =='txvx1':
+            txprods[name] = tx(dftx[dftx.name==name],
+                               genotype_pars=dftxvx[dftxvx.name==name],
+                               imm_init=dict(dist='beta_mean', par1=0.35, par2=0.025))
+        elif name == 'txvx2':
+            txprods[name] = tx(dftx[dftx.name==name],
+                               genotype_pars=dftxvx[dftxvx.name==name],
+                               imm_boost=1.5)
+        else:
+            txprods[name] = tx(dftx[dftx.name == name])
     if prod_name is not None:   return txprods[prod_name]
     else:                       return txprods
 
 
 def default_vx(prod_name=None):
     '''
     Create default vaccine products
```

### Comparing `hpvsim-1.1.1/hpvsim/misc.py` & `hpvsim-1.2.0/hpvsim/misc.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/parameters.py` & `hpvsim-1.2.0/hpvsim/parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,61 +71,66 @@
     pars['condoms']         = None  # The proportion of acts in which condoms are used for each partnership type
     pars['layer_probs']     = None  # Proportion of the population in each partnership type
     pars['dur_pship']       = None  # Duration of partnerships in each partnership type
     pars['mixing']          = None  # Mixing matrices for storing age differences in partnerships
     pars['n_partner_types'] = 1  # Number of partnership types - reset below
 
     # Basic disease transmission parameters
-    pars['beta']                = 0.21   # Per-act transmission probability; absolute value, calibrated
+    pars['beta']                = 0.2   # Per-act transmission probability; absolute value, calibrated
     pars['transf2m']            = 1.0   # Relative transmissibility of receptive partners in penile-vaginal intercourse; baseline value
     pars['transm2f']            = 3.69  # Relative transmissibility of insertive partners in penile-vaginal intercourse; based on https://doi.org/10.1038/srep10986: "For vaccination types, the risk of male-to-female transmission was higher than that of female-to-male transmission"
     pars['eff_condoms']         = 0.7   # The efficacy of condoms; https://www.nejm.org/doi/10.1056/NEJMoa053284?url_ver=Z39.88-2003&rfr_id=ori:rid:crossref.org&rfr_dat=cr_pub%20%200www.ncbi.nlm.nih.gov
 
     # Parameters for disease progression
     pars['hpv_control_prob']    = 0.0 # Probability that HPV is controlled latently vs. cleared
     pars['hpv_reactivation']    = 0.025 # Placeholder; unused unless hpv_control_prob>0
-    pars['dur_cancer']          = dict(dist='lognormal', par1=12.0, par2=3.0)  # Duration of untreated invasive cerival cancer before death (years)
-    pars['dur_transformed']     = dict(dist='normal_pos', par1=5.77, par2=5)  # Duration of transformed infection prior to onset of invasive cervical cancer (years)
+    pars['dur_cancer']          = dict(dist='lognormal', par1=8.0, par2=3.0)  # Duration of untreated invasive cerival cancer before death (years)
     pars['dur_infection_male']  = dict(dist='lognormal', par1=1, par2=1) # Duration of infection for men
-    pars['clinical_cutoffs']    = dict(precin=0.03, cin1=0.353, cin2=0.676, cin3=0.99) # Parameters used to map disease severity onto cytological grades
-    pars['sev_dist']            = dict(dist='normal_pos', par1=1.0, par2=0.05) # Distribution to draw individual level severity scale factors
+    pars['clinical_cutoffs']    = dict(cin1=0.33, cin2=0.676, cin3=0.8) # Parameters used to map disease severity onto cytological grades
+    pars['sev_dist']            = dict(dist='normal_pos', par1=1.0, par2=0.25) # Distribution to draw individual level severity scale factors
+    pars['age_risk']            = dict(age=30, risk=1)
 
     # Parameters used to calculate immunity
     pars['imm_init']        = dict(dist='beta_mean', par1=0.35, par2=0.025)  # beta distribution for initial level of immunity following infection clearance. Parameters are mean and variance from https://doi.org/10.1093/infdis/jiv753
     pars['imm_decay']       = dict(form=None)  # decay rate, with half life in years
     pars['cell_imm_init']   = dict(dist='beta_mean', par1=0.25, par2=0.025) # beta distribution for level of immunity against persistence/progression of infection following infection clearance and seroconversion
     pars['imm_boost']       = []  # Multiplicative factor applied to a person's immunity levels if they get reinfected. No data on this, assumption.
-    pars['immunity']        = None  # Matrix of immunity and cross-immunity factors, set by init_immunity() in immunity.py
-    pars['cross_imm_med']   = 0.3
-    pars['cross_imm_high']  = 0.5
+    pars['cross_immunity_sus'] = None  # Matrix of susceptibility cross-immunity factors, set by init_immunity() in immunity.py
+    pars['cross_immunity_sev'] = None  # Matrix of severity cross-immunity factors, set by init_immunity() in immunity.py
+    pars['cross_imm_sus_med']   = 0.3
+    pars['cross_imm_sus_high']  = 0.5
+    pars['cross_imm_sev_med']   = 0.5
+    pars['cross_imm_sev_high']  = 0.7
+    pars['own_imm_hr'] = 0.9
 
     # Genotype parameters
-    pars['genotypes']       = [16, 18, 'hrhpv']  # Genotypes to model
+    pars['genotypes']       = [16, 18, 'hi5']  # Genotypes to model
     pars['genotype_pars']   = sc.objdict()  # Can be directly modified by passing in arguments listed in get_genotype_pars
 
     # Events and interventions
     pars['interventions']   = sc.autolist() # The interventions present in this simulation; populated by the user
     pars['analyzers']       = sc.autolist() # The functions present in this simulation; populated by the user
     pars['timelimit']       = None # Time limit for the simulation (seconds)
     pars['stopping_func']   = None # A function to call to stop the sim partway through
 
     # Population distribution of the World Standard Population, used to calculate age-standardised rates (ASR) of incidence
-    pars['age_bins']        = np.array( [  0,   5,  10,  15,  20,  25,  30,  35,  40,  45,  50,  55,  60,  65,  70,  75,    80,    85, 100])
-    pars['standard_pop']    = np.array([pars['age_bins'],
+    pars['age_bin_edges']        = np.array( [  0,   5,  10,  15,  20,  25,  30,  35,  40,  45,  50,  55,  60,  65,  70,  75,    80,    85, 100])
+    pars['standard_pop']    = np.array([pars['age_bin_edges'],
                                         [.12, .10, .09, .09, .08, .08, .06, .06, .06, .06, .05, .04, .04, .03, .02, .01, 0.005, 0.005,   0]])
 
     # The following variables are stored within the pars dict for ease of access, but should not be directly specified.
-    # Rather, they are automaticall constructed during sim initialization.
+    # Rather, they are automatically constructed during sim initialization.
     pars['immunity_map']    = None  # dictionary mapping the index of immune source to the type of immunity (vaccine vs natural)
     pars['imm_kin']         = None  # Constructed during sim initialization using the nab_decay parameters
     pars['genotype_map']    = dict()  # Reverse mapping from number to genotype key
     pars['n_genotypes']     = 1 # The number of genotypes circulating in the population
     pars['n_imm_sources']   = 1 # The number of immunity sources circulating in the population
     pars['vaccine_pars']    = dict()  # Vaccines that are being used; populated during initialization
     pars['vaccine_map']     = dict()  # Reverse mapping from number to vaccine key
+    pars['cumdysp']         = dict()
 
     # Update with any supplied parameter values and generate things that need to be generated
     pars.update(kwargs)
     reset_layer_pars(pars)
 
     return pars
 
@@ -149,33 +154,33 @@
     '''
 
     layer_defaults = {}
     # Specify defaults for random -- layer 'a' for 'all'
     layer_defaults['random'] = dict(
         partners    = dict(a=dict(dist='poisson', par1=0.01)), # Everyone in this layer has one partner; this captures *additional* partners. If using a poisson distribution, par1 is roughly equal to the proportion of people with >1 partner
         acts        = dict(a=dict(dist='neg_binomial', par1=100,par2=50)),  # Default number of sexual acts per year for people at sexual peak
-        age_act_pars = dict(a=dict(peak=35, retirement=60, debut_ratio=0.5, retirement_ratio=0.1)), # Parameters describing changes in coital frequency over agent lifespans
+        age_act_pars = dict(a=dict(peak=35, retirement=100, debut_ratio=0.5, retirement_ratio=0.1)), # Parameters describing changes in coital frequency over agent lifespans
         layer_probs = dict(a=1.0),  # Default proportion of the population in each layer
         dur_pship   = dict(a=dict(dist='normal_pos', par1=5,par2=3)),    # Default duration of partnerships
         condoms     = dict(a=0.25),  # Default proportion of acts in which condoms are used
     )
     layer_defaults['random']['mixing'], layer_defaults['random']['layer_probs'] = get_mixing('random')
 
     # Specify defaults for basic sexual network with marital, casual, and one-off partners
     layer_defaults['default'] = dict(
         partners    = dict(m=dict(dist='poisson', par1=0.01), # Everyone in this layer has one marital partner; this captures *additional* marital partners. If using a poisson distribution, par1 is roughly equal to the proportion of people with >1 spouse
                            c=dict(dist='poisson', par1=0.2), # If using a poisson distribution, par1 is roughly equal to the proportion of people with >1 casual partner at a time
                            o=dict(dist='poisson', par1=0.0),), # If using a poisson distribution, par1 is roughly equal to the proportion of people with >1 one-off partner at a time. Can be set to zero since these relationships only last a single timestep
         acts         = dict(m=dict(dist='neg_binomial', par1=80, par2=40), # Default number of acts per year for people at sexual peak
                             c=dict(dist='neg_binomial', par1=10, par2=5), # Default number of acts per year for people at sexual peak
                             o=dict(dist='neg_binomial', par1=1,  par2=.01)),  # Default number of acts per year for people at sexual peak
-        age_act_pars = dict(m=dict(peak=30, retirement=60, debut_ratio=0.5, retirement_ratio=0.1), # Parameters describing changes in coital frequency over agent lifespans
-                            c=dict(peak=25, retirement=60, debut_ratio=0.5, retirement_ratio=0.1),
-                            o=dict(peak=25, retirement=50, debut_ratio=0.5, retirement_ratio=0.1)),
-        dur_pship   = dict(m=dict(dist='normal_pos', par1=20, par2=3),
+        age_act_pars = dict(m=dict(peak=30, retirement=100, debut_ratio=0.5, retirement_ratio=0.1), # Parameters describing changes in coital frequency over agent lifespans
+                            c=dict(peak=25, retirement=100, debut_ratio=0.5, retirement_ratio=0.1),
+                            o=dict(peak=25, retirement=100, debut_ratio=0.5, retirement_ratio=0.1)),
+        dur_pship   = dict(m=dict(dist='normal_pos', par1=12, par2=3),
                            c=dict(dist='normal_pos', par1=1, par2=1),
                            o=dict(dist='normal_pos', par1=0.1, par2=0.05)),
         condoms     = dict(m=0.01, c=0.2, o=0.1),  # Default proportion of acts in which condoms are used
     )
     layer_defaults['default']['mixing'], layer_defaults['default']['layer_probs'] = get_mixing('default')
 
     # Choose the parameter defaults based on the population type, and get the layer keys
@@ -244,17 +249,20 @@
 
 def get_genotype_choices():
     '''
     Define valid genotype names
     '''
     # List of choices available
     choices = {
-        'hpv16':  ['hpv16', '16'],
-        'hpv18': ['hpv18', '18'],
-        'hrhpv': ['hrhpv', 'ohrhpv', 'hr', 'ohr'],
+        'hpv16':    ['hpv16', '16'],
+        'hpv18':    ['hpv18', '18'],
+        'hi5':      ['hi5hpv', 'hi5hpv', 'cross-protective'],
+        'ohr':      ['ohrhpv', 'non-cross-protective'],
+        'hr':       ['allhr', 'allhrhpv', 'hrhpv', 'oncogenic', 'hr10', 'hi10'],
+        'lo':       ['lohpv'],
     }
     mapping = {name:key for key,synonyms in choices.items() for name in synonyms} # Flip from key:value to value:key
     return choices, mapping
 
 def get_vaccine_choices():
     '''
     Define valid pre-defined vaccine names
@@ -280,30 +288,14 @@
     choices['nonavalent_3dose'] = [f'{x}_{dose}' for x in choices['nonavalent'] for dose in dose_3_options]
     choices['nonavalent'] = ['nonavalent']+[f'{x}_{dose}' for x in choices['nonavalent'] for dose in dose_1_options]
 
     mapping = {name:key for key,synonyms in choices.items() for name in synonyms} # Flip from key:value to value:key
     return choices, mapping
 
 
-
-def get_treatment_choices():
-    '''
-    Define valid pre-defined treatment names
-    '''
-    # List of choices currently available: new ones can be added to the list along with their aliases
-    choices = {
-        'default': ['default', None],
-        'ablative':  ['ablative', 'thermal_ablation', 'TA'],
-        'excisional': ['excisional', 'leep'],
-        'radiation': ['radiation']
-    }
-    mapping = {name:key for key,synonyms in choices.items() for name in synonyms} # Flip from key:value to value:key
-    return choices, mapping
-
-
 def _get_from_pars(pars, default=False, key=None, defaultkey='default'):
     ''' Helper function to get the right output from genotype functions '''
 
     # If a string was provided, interpret it as a key and swap
     if isinstance(default, str):
         key, default = default, key
 
@@ -324,59 +316,124 @@
     '''
     Define the default parameters for the different genotypes
     '''
 
     pars = sc.objdict()
 
     pars.hpv16 = sc.objdict()
-    pars.hpv16.dur_episomal     = dict(dist='lognormal', par1=4.5, par2=9) # Duration of episomal infection prior to cancer
-    pars.hpv16.sev_fn           = dict(form='logf3', k=0.3, x_infl=13, s=1) # Function mapping duration of infection to severity
+    pars.hpv16.dur_precin       = dict(dist='normal_pos', par1=0.5, par2=0.25)  # Duration of infection prior to precancer
+    pars.hpv16.dur_episomal     = dict(dist='lognormal', par1=2, par2=5) # Duration of episomal infection prior to cancer
+    pars.hpv16.sev_fn           = dict(form='logf2', k=0.175, x_infl=0, ttc=30) # Function mapping duration of infection to severity
     pars.hpv16.rel_beta         = 1.0  # Baseline relative transmissibility, other genotypes are relative to this
-    pars.hpv16.transform_prob   = 0.00025 # Annual rate of transformed cell invading
+    pars.hpv16.transform_prob   = 1.3e-9 # Annual rate of transformed cell invading
+    pars.hpv16.sev_integral     = 'analytic' # Type of integral used for translating severity to transformation probability. Accepts numeric, analytic, or None
     pars.hpv16.sero_prob        = 0.75 # https://www.sciencedirect.com/science/article/pii/S2666679022000027#fig1
 
     pars.hpv18 = sc.objdict()
-    pars.hpv18.dur_episomal     = dict(dist='lognormal', par1=3.5, par2=9) # Duration of infection prior to cancer
-    pars.hpv18.sev_fn           = dict(form='logf3', k=0.238, x_infl=14, s=1) # Function mapping duration of infection to severity
+    pars.hpv18.dur_precin       = dict(dist='normal_pos', par1=0.5, par2=0.25)  # Duration of infection prior to precancer
+    pars.hpv18.dur_episomal     = dict(dist='lognormal', par1=2, par2=5) # Duration of infection prior to cancer
+    pars.hpv18.sev_fn           = dict(form='logf2', k=0.15, x_infl=0, ttc=30) # Function mapping duration of infection to severity
     pars.hpv18.rel_beta         = 0.75  # Relative transmissibility, current estimate from Harvard model calibration of m2f tx
-    pars.hpv18.transform_prob   = 0.00015 # Annual rate of transformed cell invading
+    pars.hpv18.transform_prob   = 1.0e-9 # Annual rate of transformed cell invading
+    pars.hpv18.sev_integral     = 'analytic' # Type of integral used for translating severity to transformation probability. Accepts numeric, analytic, or None
     pars.hpv18.sero_prob        = 0.56 # https://www.sciencedirect.com/science/article/pii/S2666679022000027#fig1
 
-    pars.hrhpv = sc.objdict()
-    pars.hrhpv.dur_episomal     = dict(dist='lognormal', par1=5, par2=10) # Duration of infection prior to cancer
-    pars.hrhpv.sev_fn           = dict(form='logf3', k=0.35, x_infl=15, s=1) # Function mapping duration of infection to severity
-    pars.hrhpv.rel_beta         = 0.9 # placeholder
-    pars.hrhpv.transform_prob   = 0.00015
-    pars.hrhpv.sero_prob        = 0.60 # placeholder
+    # High-risk oncogenic types included in 9valent vaccine: 31, 33, 45, 52, 58
+    pars.hi5 = sc.objdict()
+    pars.hi5.dur_precin         = dict(dist='normal_pos', par1=0.5, par2=0.25)  # Duration of infection prior to precancer
+    pars.hi5.dur_episomal       = dict(dist='lognormal', par1=2, par2=4) # Duration of infection prior to cancer
+    pars.hi5.sev_fn             = dict(form='logf2', k=0.125, x_infl=0, ttc=30) # Function mapping duration of infection to severity
+    pars.hi5.rel_beta           = 0.9 # placeholder
+    pars.hi5.transform_prob     = 3e-10 # Annual rate of transformed cell invading
+    pars.hi5.sev_integral       = 'analytic' # Type of integral used for translating severity to transformation probability. Accepts numeric, analytic, or None
+    pars.hi5.sero_prob          = 0.60 # placeholder
+
+    # Other high-risk: oncogenic but not covered in 9valent vaccine: 35, 39, 51, 56, 59
+    pars.ohr = sc.objdict()
+    pars.ohr.dur_precin         = dict(dist='normal_pos', par1=0.5, par2=0.25)  # Duration of infection prior to precancer
+    pars.ohr.dur_episomal       = dict(dist='lognormal', par1=2, par2=6) # Duration of infection prior to cancer
+    pars.ohr.sev_fn             = dict(form='logf2', k=0.125, x_infl=0, ttc=30) # Function mapping duration of infection to severity
+    pars.ohr.rel_beta           = 0.9 # placeholder
+    pars.ohr.transform_prob     = 3e-10 # Annual rate of transformed cell invading
+    pars.ohr.sev_integral       = 'analytic' # Type of integral used for translating severity to transformation probability. Accepts numeric, analytic, or None
+    pars.ohr.sero_prob          = 0.60 # placeholder
+
+    # All other high-risk types: 31, 33, 35, 39, 45, 51, 52, 56, 58, 59
+    # Warning: this should not be used in conjuction with hi5 or ohr
+    pars.hr = sc.objdict()
+    pars.hr.dur_precin       = dict(dist='normal_pos', par1=0.5, par2=0.25)  # Duration of infection prior to precancer
+    pars.hr.dur_episomal     = dict(dist='lognormal', par1=2, par2=4) # Duration of infection prior to cancer
+    pars.hr.sev_fn           = dict(form='logf2', k=0.125, x_infl=0, ttc=30) # Function mapping duration of infection to severity
+    pars.hr.rel_beta         = 0.9 # placeholder
+    pars.hr.transform_prob   = 3e-10 # Annual rate of transformed cell invading
+    pars.hr.sev_integral     = 'analytic' # Type of integral used for translating severity to transformation probability. Accepts numeric, analytic, or None
+    pars.hr.sero_prob        = 0.60 # placeholder
+
+    # Low-risk
+    pars.lr = sc.objdict()
+    pars.lr.dur_precin          = dict(dist='normal_pos', par1=0.5, par2=0.25)  # Duration of infection prior to precancer
+    pars.lr.dur_episomal        = dict(dist='lognormal', par1=2, par2=4) # Duration of infection prior to cancer
+    pars.lr.sev_fn              = dict(form='logf2', k=0.0, x_infl=0, ttc=30) # Function mapping duration of infection to severity
+    pars.lr.rel_beta            = 0.9 # placeholder
+    pars.lr.transform_prob      = 0 # Annual rate of transformed cell invading
+    pars.lr.sev_integral        = 'analytic' # Type of integral used for translating severity to transformation probability. Accepts numeric, analytic, or None
+    pars.lr.sero_prob           = 0.60 # placeholder
 
     return _get_from_pars(pars, default, key=genotype, defaultkey='hpv16')
 
 
-def get_cross_immunity(cross_imm_med=None, cross_imm_high=None, default=False, genotype=None):
+def get_cross_immunity(cross_imm_med=None, cross_imm_high=None, own_imm_hr=None, default=False, genotype=None):
     '''
     Get the cross immunity between each genotype in a sim
     '''
     pars = dict(
         # All values based roughly on https://academic.oup.com/jnci/article/112/10/1030/5753954 or assumptions
         hpv16 = dict(
             hpv16=1.0, # Default for own-immunity
             hpv18=cross_imm_high,
-            hrhpv=cross_imm_med,
+            hi5=cross_imm_med,
+            ohr=cross_imm_med,
+            hr=cross_imm_med,
+            lr=cross_imm_med,
         ),
 
         hpv18 = dict(
             hpv16=cross_imm_high,
             hpv18=1.0,  # Default for own-immunity
-            hrhpv=cross_imm_med,
+            hi5=cross_imm_med,
+            ohr=cross_imm_med,
+            hr=cross_imm_med,
+            lr=cross_imm_med,
         ),
 
-        hrhpv=dict(
+        hi5=dict(
             hpv16=cross_imm_med,
             hpv18=cross_imm_med,
-            hrhpv=cross_imm_med,
+            hi5=own_imm_hr,
+            ohr=cross_imm_med,
+            hr=cross_imm_med,
+            lr=cross_imm_med,
+        ),
+
+        ohr=dict(
+            hpv16=cross_imm_med,
+            hpv18=cross_imm_med,
+            hi5=cross_imm_med,
+            ohr=own_imm_hr,
+            hr=cross_imm_med,
+            lr=cross_imm_med,
+        ),
+
+        lr=dict(
+            hpv16=cross_imm_med,
+            hpv18=cross_imm_med,
+            hi5=cross_imm_med,
+            ohr=cross_imm_med,
+            hr=cross_imm_med,
+            lr=own_imm_hr,
         ),
 
     )
 
     return _get_from_pars(pars, default, key=genotype, defaultkey='hpv16')
 
 
@@ -638,7 +695,42 @@
         raise NotImplementedError(errormsg)
 
     # Scale by relative severity
     if rel_sev is not None:
         output = output / rel_sev
 
     return output
+
+
+def compute_severity_integral(t, rel_sev=None, pars=None):
+    '''
+    Process functional form and parameters into values:
+    '''
+
+    pars = sc.dcp(pars)
+    form = pars.pop('form')
+    choices = [
+        'logf2',
+        'logf3 with s=1',
+    ]
+
+    # Scale t
+    if rel_sev is not None:
+        t = rel_sev * t
+
+    # Process inputs
+    if form is None or form == 'logf2':
+        output = hpu.intlogf2(t, **pars)
+
+    elif form=='logf3':
+        s = pars.pop('s')
+        if s==1:
+            output = hpu.intlogf2(t, **pars)
+        else:
+            errormsg = f'Analytic integral for logf3 only implemented for s=1. Select integral=numeric.'
+
+    else:
+        errormsg = f'Analytic integral for the selected functional form "{form}" is not implemented; choices are: {sc.strjoin(choices)}, or select integral=numeric.'
+        raise NotImplementedError(errormsg)
+
+    return output
+
```

### Comparing `hpvsim-1.1.1/hpvsim/people.py` & `hpvsim-1.2.0/hpvsim/people.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,23 +55,23 @@
         # Handle pars and settings
 
         # Other initialization
         self.pop_trend = pop_trend
         self.pop_age_trend = pop_age_trend
         self.init_contacts() # Initialize the contacts
         self.ng = self.pars['n_genotypes']
-        self.na = len(self.pars['age_bins'])-1
+        self.na = len(self.pars['age_bin_edges'])-1
 
         self.lag_bins = np.linspace(0,50,51)
         self.rship_lags = dict()
         for lkey in self.layer_keys():
             self.rship_lags[lkey] = np.zeros(len(self.lag_bins)-1, dtype=hpd.default_float)
 
         # Store age bins
-        self.age_bins = self.pars['age_bins'] # Age bins for age results
+        self.age_bin_edges = self.pars['age_bin_edges'] # Age bins for age results
 
         if strict:
             self.lock() # If strict is true, stop further keys from being set (does not affect attributes)
 
         # Store flows to be computed during simulation
         self.init_flows()
 
@@ -108,42 +108,45 @@
         self.age[self.alive] += self.dt
         return
 
 
     def initialize(self, sim_pars=None):
         ''' Perform initializations '''
         super().initialize() # Initialize states
-        
+
         # Handle partners and contacts
         kwargs = self.kwargs
         if 'partners' in kwargs:
             self.partners[:] = kwargs.pop('partners') # Store the desired concurrency
         if 'current_partners' in kwargs:
             self.current_partners[:] = kwargs.pop('current_partners') # Store current actual number - updated each step though
             for ln,lkey in enumerate(self.layer_keys()):
                 self.rship_start_dates[ln,self.current_partners[ln]>0] = 0
         if 'contacts' in kwargs:
             self.add_contacts(kwargs.pop('contacts')) # Also updated each step
 
+        self.n_rships[:] = self.current_partners
+        self.ever_partnered[:] = self.current_partners.sum(axis=0)>0
+
         # Handle all other values, e.g. age
         for key,value in kwargs.items():
             if self._lock:
                 self.set(key, value)
             elif key in self._data:
                 self[key][:] = value
             else:
                 self[key] = value
         
         # Set the scale factor
         self.scale[:] = sim_pars['pop_scale']
 
         # Additional validation
         self.validate(sim_pars=sim_pars) # First, check that essential-to-match parameters match
-
         self.initialized = True
+
         return
 
 
     def update_states_pre(self, t, year=None):
         ''' Perform all state updates at the current timestep '''
 
         # Initialize
@@ -171,61 +174,97 @@
             # Check migration
             migration = self.check_migration(year=year)
             self.demographic_flows['migration'] = migration
 
         # Perform updates that are genotype-specific
         ng = self.pars['n_genotypes']
         for g in range(ng):
-            self.check_transformation(g) # check for new transformations, persistence, or clearance
+            self.check_clearance(g) # check for clearance (need to do this first)
             self.update_severity(g) # update severity values
-            self.check_clearance(g) # check for clearance
+            self.check_transformation(g)  # check for new transformations
 
             for key in ['cin1s','cin2s','cin3s','cancers']:  # update flows
                 cases_by_age, cases = self.check_progress(key, g)
                 self.flows[key] += cases  # Increment flows (summed over all genotypes)
                 self.genotype_flows[key][g] = cases # Store flows by genotype
                 self.age_flows[key] += cases_by_age # Increment flows by age (summed over all genotypes)
             self.flows['cins'] += self.flows['cin1s']+self.flows['cin2s']+self.flows['cin3s']
             self.genotype_flows['cins'][g] = self.genotype_flows['cin1s'][g]+self.genotype_flows['cin2s'][g]+self.genotype_flows['cin3s'][g]
             self.age_flows['cins'] += self.age_flows['cin1s']+self.age_flows['cin2s']+self.age_flows['cin3s']
 
         # Perform updates that are not genotype specific
-        self.flows['cancer_deaths'] = self.check_cancer_deaths()
+        deaths_by_age, deaths = self.check_cancer_deaths()
+        self.flows['cancer_deaths'] = deaths
+        self.age_flows['cancer_deaths'] = deaths_by_age
 
         # Before applying interventions or new infections, calculate the pool of susceptibles
         self.sus_pool = self.susceptible.all(axis=0) # True for people with no infection at the start of the timestep
 
         return
 
     
     #%% Disease progression methods
     def set_prognoses(self, inds, g, gpars, dt):
         '''
         Assigns prognoses for all infected women on day of infection.
         '''
 
         # Set length of infection, which is moderated by any prior cell-level immunity
-        cell_imm = self.cell_imm[g, inds]
-        self.dur_episomal[g, inds]  = hpu.sample(**gpars['dur_episomal'], size=len(inds))*(1-cell_imm)
+        sev_imm = self.sev_imm[g, inds]
+        age_mod = np.ones(len(inds))
+        age_mod[self.age[inds]>= self.pars['age_risk']['age']] = self.pars['age_risk']['risk']
+        self.dur_episomal[g, inds]  = hpu.sample(**gpars['dur_episomal'], size=len(inds))*(1-sev_imm)*age_mod
+        self.dur_infection[g, inds]  = self.dur_episomal[g, inds]
+
+        # Determine how long before precancerous cell changes
+        dur_precin = hpu.sample(**gpars['dur_precin'], size=len(inds)) # Sample from distribution
+        cin_bools = self.dur_episomal[g, inds] > dur_precin # Pull out those whose infection is long enough for precancer
+        cin_inds = inds[cin_bools]
+        nocin_inds = inds[~cin_bools]
+        self.dur_precin[g, inds] = np.minimum(self.dur_episomal[g, inds], dur_precin)
+        self.dur_cin[g, cin_inds] = self.dur_episomal[g, cin_inds] - self.dur_precin[g, cin_inds]
+
+        # Set date of clearance for those who don't develop precancer
+        self.date_clearance[g, nocin_inds] = self.t + sc.randround(self.dur_precin[g, nocin_inds]/dt)
+
+        # Set date of onset of precancer and eventual severity outcomes for those who develop precancer
+        self.date_cin1[g, cin_inds] = self.t + sc.randround(self.dur_precin[g, cin_inds]/dt)
 
         # Set infection severity and outcomes
-        self.set_severity(inds, g, gpars, dt)
+        self.set_severity(inds[cin_bools], g, gpars, dt)
 
         return
 
 
     def set_severity(self, inds, g, gpars, dt, set_sev=True):
         '''
         Set severity levels for individual women
+        Args:
+            inds: indices of women to set severity for
+            g: genotype index
+            dt: timestep
+            set_sev: whether or not to set initial severity
         '''
 
-        # Firstly, calculate the overall maximal severity that each woman will have
+        # Pull out useful variables
+        ccdict = self.pars['clinical_cutoffs']
+        if set_sev: self.sev[g, inds] = 0 # For those who develop dysplasia, sev begins at 0 on their first day of infection
+
+        # Calculate the integral of severity for each woman
         dur_episomal = self.dur_episomal[g, inds]
-        if set_sev: self.sev[g, inds] = 0 # Severity starts at 0 on day 1 of infection
-        sevs = hppar.compute_severity(dur_episomal, rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])  # Calculate maximal severity
+        dur_cin = self.dur_cin[g, inds]
+        if gpars['sev_integral']=='analytic':
+            sevs = hppar.compute_severity_integral(dur_cin, rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])  # Calculate analytic integral of cumulative severity
+        elif gpars['sev_integral']=='numeric':
+            cumdysp = self.pars['cumdysp'][self.pars['genotype_map'][g]]
+            t = np.around(dur_cin/dt).astype(int) # Round
+            t[t > len(cumdysp) - 1] = len(cumdysp) - 1
+            sevs = cumdysp[t]
+        elif gpars['sev_integral'] is None:
+            sevs = hppar.compute_severity(dur_cin, rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])
 
         # Now figure out probabilities of cellular transformations preceding cancer, based on this severity level
         transform_prob_par = gpars['transform_prob'] # Pull out the genotype-specific parameter governing the probability of transformation
         n_extra = self.pars['ms_agent_ratio']
         cancer_scale = self.pars['pop_scale'] / n_extra
 
         # Non-multiscale version
@@ -240,16 +279,27 @@
             is_transform = hpu.binomial_arr(transform_probs) # Select who transforms - NB, this array gets extended later
             transform_inds = inds[is_transform] # Indices of those who transform
             self.scale[transform_inds] = cancer_scale  # Shrink the weight of the original agents, but otherwise leave them the same
 
             # Create extra disease severity values for the extra agents
             full_size = (len(inds), n_extra)  # Main axis is indices, but include columns for multiscale agents
             extra_dur_episomal = hpu.sample(**gpars['dur_episomal'], size=full_size)
-            extra_rel_sevs = hpu.sample(**self.pars['sev_dist'], size=full_size)
-            extra_sev = hppar.compute_severity(extra_dur_episomal, rel_sev=extra_rel_sevs, pars=gpars['sev_fn'])  # Calculate maximal severity
+            extra_dur_precin = hpu.sample(**gpars['dur_precin'], size=full_size)
+            extra_dur_cin = np.maximum(extra_dur_episomal - extra_dur_precin, 0)
+            extra_rel_sevs = np.ones(full_size)*self.rel_sev[inds][:,None]
+
+            if gpars['sev_integral'] == 'analytic':
+                extra_sev = hppar.compute_severity_integral(extra_dur_cin, rel_sev=extra_rel_sevs, pars=gpars['sev_fn'])  # Calculate analytic integral of cumulative severity
+            elif gpars['sev_integral'] == 'numeric':
+                cumdysp = self.pars['cumdysp'][self.pars['genotype_map'][g]]
+                t = np.around(extra_dur_cin/dt*extra_rel_sevs).astype(int)  # Round
+                t[t > len(cumdysp) - 1] = len(cumdysp) - 1
+                extra_sev = cumdysp[t]
+            elif gpars['sev_integral'] is None:
+                extra_sev = hppar.compute_severity(extra_dur_cin, rel_sev=extra_rel_sevs, pars=gpars['sev_fn'])  # Calculate analytic integral of cumulative severity
 
             # Based on the extra severity values, determine additional transformation probabilities
             extra_transform_probs = hpu.transform_prob(transform_prob_par, extra_sev[:, 1:])
             extra_transform_bools = hpu.binomial_arr(extra_transform_probs)
             extra_transform_bools *= self.level0[inds, None]  # Don't allow existing cancer agents to make more cancer agents
             extra_transform_counts = extra_transform_bools.sum(axis=1)  # Find out how many new cancer cases we have
             n_new_agents = extra_transform_counts.sum()  # Total number of new agents
@@ -275,84 +325,103 @@
                 self.level1[new_inds] = True
                 self.scale[new_inds] = cancer_scale
 
                 # Add the new indices onto the existing vectors
                 inds = np.append(inds, new_inds)
                 is_transform = np.append(is_transform, np.full(len(new_inds), fill_value=True))
                 new_dur_episomal = extra_dur_episomal[:,1:][extra_transform_bools]
+                new_dur_precin = extra_dur_precin[:, 1:][extra_transform_bools]
+                new_dur_cin = extra_dur_cin[:, 1:][extra_transform_bools]
                 self.dur_episomal[g, new_inds] = new_dur_episomal
+                self.dur_precin[g, new_inds] = new_dur_precin
+                self.dur_cin[g, new_inds] = new_dur_cin
                 self.dur_infection[g, new_inds] = new_dur_episomal
                 self.date_infectious[g, new_inds] = self.t
-                self.date_exposed[g, new_inds] = self.t
                 dur_episomal = np.append(dur_episomal, new_dur_episomal)
 
             # Finally, create an array for storing the transformation probabilities.
             # We've already figured out who's going to transform, so we fill the array with 1s for those who do.
             transform_prob_arr = np.zeros(len(inds))
             transform_prob_arr[is_transform] = 1  # Make sure inds that got assigned cancer above dont get stochastically missed
 
         # Set dates of cin1, 2, 3 for all women who get infected
-        ccdict = self.pars['clinical_cutoffs']
-        rel_sev_vals = self.rel_sev[inds]
-        self.date_cin1[g, inds]         = self.t + sc.randround(hppar.compute_inv_severity(ccdict['precin'],    rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])/dt)
-        self.date_cin2[g, inds]         = self.t + sc.randround(hppar.compute_inv_severity(ccdict['cin1'],      rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])/dt)
-        self.date_cin3[g, inds]         = self.t + sc.randround(hppar.compute_inv_severity(ccdict['cin2'],      rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])/dt)
-        self.date_carcinoma[g, inds]    = self.t + sc.randround(hppar.compute_inv_severity(ccdict['cin3'],      rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])/dt)
+        self.date_cin2[g, inds]         = self.date_cin1[g,inds] + sc.randround(hppar.compute_inv_severity(ccdict['cin1'],      rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])/dt)
+        self.date_cin3[g, inds]         = self.date_cin1[g,inds] + sc.randround(hppar.compute_inv_severity(ccdict['cin2'],      rel_sev=self.rel_sev[inds], pars=gpars['sev_fn'])/dt)
 
-        # Now handle women who transform - need to adjust their length of infection and set more dates
+        # Determine who goes to cancer
         is_transform = hpu.binomial_arr(transform_prob_arr)
         transform_inds = inds[is_transform]
         no_cancer_inds = inds[~is_transform]  # Indices of those who eventually heal lesion/clear infection
+
+        # Set date of clearance for those who don't go to cancer
         time_to_clear = dur_episomal[~is_transform]
         self.date_clearance[g, no_cancer_inds] = np.fmax(self.date_clearance[g, no_cancer_inds],
                                                          self.date_exposed[g, no_cancer_inds] +
                                                          sc.randround(time_to_clear / dt))
 
-        self.date_transformed[g, transform_inds] = self.t + sc.randround(dur_episomal[is_transform] / dt)
-        dur_transformed = hpu.sample(**self.pars['dur_transformed'], size=len(transform_inds))
-        self.date_cancerous[g, transform_inds] = self.date_transformed[g, transform_inds] + sc.randround(dur_transformed / dt)
-        self.dur_infection[g, transform_inds] = self.dur_infection[g, transform_inds] + dur_transformed
-
+        # Set dates for those who go to cancer. Transformation is assumed to occur at
+        # the end of episomal infection, while cancer is assumed to begin once severity
+        # exceeds the cancer cutoff, which may mean that it begins as soon as transformation
+        # happens, if severity is already above the threshold.
+        dur_episomal_transformed = dur_episomal[is_transform] # Duration of episomal infection for those who transform
+        self.date_transformed[g, transform_inds] = self.t + sc.randround(dur_episomal_transformed/dt)
+        time_to_cancer = hppar.compute_inv_severity(ccdict['cin3'], rel_sev=self.rel_sev[transform_inds], pars=gpars['sev_fn'])
+
+        # Calculate duration of transformed infection. The minimum ensures that anyone who
+        # transforms after they've already exceeded the severity cutoff goes straight to cancer
+        self.dur_transformed[g, transform_inds] = np.maximum(time_to_cancer - dur_episomal_transformed, 0)
+        self.date_cancerous[g, transform_inds] = self.date_transformed[g, transform_inds] + sc.randround(self.dur_transformed[g, transform_inds]/dt)
+        self.dur_infection[g, transform_inds] = self.dur_infection[g, transform_inds] + self.dur_transformed[g, transform_inds]
         dur_cancer = hpu.sample(**self.pars['dur_cancer'], size=len(transform_inds))
         self.date_dead_cancer[transform_inds] = self.date_cancerous[g, transform_inds] + sc.randround(dur_cancer / dt)
         self.dur_cancer[g, transform_inds] = dur_cancer
 
         return
 
     def update_severity(self, genotype):
         '''
-        Update disease severity for women with infection and calculate their CIN status
+        Update disease severity for women with infection and update their current severity
         '''
         gpars = self.pars['genotype_pars'][genotype]
+
+        # Only need to update severity for people who with dysplasia underway
         fg_inds = hpu.true(self.is_female & self.infectious[genotype,:]) # Indices of women infected with this genotype
-        time_with_infection = (self.t - self.date_exposed[genotype, fg_inds]) * self.dt
-        rel_sevs = self.rel_sev[fg_inds]
-        if (time_with_infection<0).any():
-            errormsg = 'Time with infection cannot be less than zero.'
+        fg_cin_inds = hpu.true(self.is_female & ~np.isnan(self.sev[genotype,:]) & self.infectious[genotype,:]) # Indices of women infected with this genotype who will develop CIN1
+        fg_cin_underway_inds = fg_cin_inds[(self.t >= self.date_cin1[genotype, fg_cin_inds])] # Indices of women for whom dysplasia is underway
+
+        time_with_dysplasia = (self.t - self.date_cin1[genotype, fg_cin_underway_inds]) * self.dt
+        rel_sevs = self.rel_sev[fg_cin_underway_inds]
+        if (time_with_dysplasia<0).any() or (np.isnan(time_with_dysplasia)).any():
+            errormsg = 'Time with dysplasia cannot be less than zero or NaN.'
+            raise ValueError(errormsg)
+        if (np.isnan(self.date_exposed[genotype, fg_cin_inds])).any():
+            errormsg = f'No date of exposure defined for {hpu.iundefined(self.date_exposed[genotype, fg_cin_inds],fg_cin_inds)} on timestep {self.t}'
             raise ValueError(errormsg)
-        if (np.isnan(self.date_exposed[genotype, fg_inds])).any():
-            errormsg = f'No date of exposure defined for {hpu.iundefined(self.date_exposed[genotype, fg_inds],fg_inds)} on timestep {self.t}'
+        if (np.isnan(self.date_cin1[genotype, fg_cin_inds])).any():
+            errormsg = f'No date of dysplasia onset defined for {hpu.iundefined(self.date_cin1[genotype, fg_cin_inds],fg_cin_inds)} on timestep {self.t}'
             raise ValueError(errormsg)
 
-        self.sev[genotype, fg_inds] = hppar.compute_severity(time_with_infection, rel_sev=rel_sevs, pars=gpars['sev_fn'])
-        if (np.isnan(self.sev[genotype, fg_inds])).any():
+        self.sev[genotype, fg_cin_underway_inds] = hppar.compute_severity(time_with_dysplasia, rel_sev=rel_sevs, pars=gpars['sev_fn'])
+
+        if (np.isnan(self.sev[genotype, fg_cin_underway_inds])).any():
             errormsg = 'Invalid severity values.'
             raise ValueError(errormsg)
 
         return
 
 
     #%% Methods for updating partnerships
     def dissolve_partnerships(self, t=None):
         ''' Dissolve partnerships '''
 
         n_dissolved = dict()
 
         for lno,lkey in enumerate(self.layer_keys()):
             layer = self.contacts[lkey]
+
             to_dissolve = (~self['alive'][layer['m']]) + (~self['alive'][layer['f']]) + ( (self.t*self.pars['dt']) > layer['end']).astype(bool)
             dissolved = layer.pop_inds(to_dissolve) # Remove them from the contacts list
 
             # Update current number of partners
             unique, counts = hpu.unique(np.concatenate([dissolved['f'],dissolved['m']]))
             self.current_partners[lno,unique] -= counts
             self.rship_end_dates[lno, unique] = self.t
@@ -367,31 +436,36 @@
         which in turn relies on hpu.create_edgelist for creating the edgelist. This method is just a light wrapper
         that passes in the arguments in the right format and the updates relationship info stored in the People class.
         '''
         # Initialize
         new_pships = dict()
 
         # Loop over layers
-        for lno, lkey in enumerate(self.layer_keys()):
+        lno=0
+        for lkey in self.layer_keys():
             pship_args = dict(
                 lno=lno, tind=tind, partners=self.partners[lno], current_partners=self.current_partners,
                 sexes=self.sex, ages=self.age, debuts=self.debut, is_female=self.is_female, is_active=self.is_active,
                 mixing=mixing[lkey], layer_probs=layer_probs[lkey], cross_layer=cross_layer,
                 pref_weight=pref_weight, durations=dur_pship[lkey], acts=acts[lkey], age_act_pars=age_act_pars[lkey]
             )
             new_pships[lkey], current_partners, new_pship_inds, new_pship_counts = hppop.make_contacts(**pship_args)
 
             # Update relationship info
+            if len(new_pship_inds)>0:
+                self.ever_partnered[new_pship_inds] = True
             self.current_partners[:] = current_partners
             if len(new_pship_inds):
                 self.rship_start_dates[lno, new_pship_inds] = self.t
                 self.n_rships[lno, new_pship_inds] += new_pship_counts
                 lags = self.rship_start_dates[lno, new_pship_inds] - self.rship_end_dates[lno, new_pship_inds]
                 self.rship_lags[lkey] += np.histogram(lags, self.lag_bins)[0]
 
+            lno += 1
+
         self.add_contacts(new_pships)
 
         return
 
 
 
     #%% Methods for updating state
@@ -413,15 +487,15 @@
         else:
             current_inds = hpu.itruei(current, filter_inds)
         has_date = hpu.idefinedi(date, current_inds)
         inds     = hpu.itrue(self.t >= date[has_date], has_date)
         return inds
 
     def check_transformation(self, genotype):
-        ''' Check for new transformations, clearance or persistence '''
+        ''' Check for new transformations '''
         # Only include infectious, episomal females who haven't already cleared infection
         filter_inds = self.true_by_genotype('episomal', genotype)
         inds = self.check_inds(self.transformed[genotype,:], self.date_transformed[genotype,:], filter_inds=filter_inds)
         self.transformed[genotype, inds] = True  # Now transformed, cannot clear
         self.date_clearance[genotype, inds] = np.nan  # Remove their clearance dates
         return
 
@@ -439,37 +513,37 @@
         ''' Check for new progressions to CIN1 '''
         # Only include infectious females who haven't already cleared CIN1 or progressed to CIN2
         filters = self.infectious[genotype,:]*self.is_female*~(self.date_clearance[genotype,:]<=self.t)*(self.date_cin2[genotype,:]>=self.t)
         filter_inds = filters.nonzero()[0]
         inds = self.check_inds(self.cin1[genotype,:], self.date_cin1[genotype,:], filter_inds=filter_inds)
         self.cin1[genotype, inds] = True
         # Age calculations
-        cases_by_age = np.histogram(self.age[inds], bins=self.age_bins, weights=self.scale[inds])[0]
+        cases_by_age = np.histogram(self.age[inds], bins=self.age_bin_edges, weights=self.scale[inds])[0]
         return cases_by_age, self.scale_flows(inds)
 
 
     def check_cin2(self, genotype):
         ''' Check for new progressions to CIN2 '''
         filter_inds = self.true_by_genotype('cin1', genotype)
         inds = self.check_inds(self.cin2[genotype,:], self.date_cin2[genotype,:], filter_inds=filter_inds)
         self.cin2[genotype, inds] = True
         self.cin1[genotype, inds] = False # No longer counted as CIN1
         # Age calculations
-        cases_by_age = np.histogram(self.age[inds], bins=self.age_bins, weights=self.scale[inds])[0]
+        cases_by_age = np.histogram(self.age[inds], bins=self.age_bin_edges, weights=self.scale[inds])[0]
         return cases_by_age, self.scale_flows(inds)
 
 
     def check_cin3(self, genotype):
         ''' Check for new progressions to CIN3 '''
         filter_inds = self.true_by_genotype('cin2', genotype)
         inds = self.check_inds(self.cin3[genotype,:], self.date_cin3[genotype,:], filter_inds=filter_inds)
         self.cin3[genotype, inds] = True
         self.cin2[genotype, inds] = False # No longer counted as CIN2
         # Age calculations
-        cases_by_age = np.histogram(self.age[inds], bins=self.age_bins, weights=self.scale[inds])[0]
+        cases_by_age = np.histogram(self.age[inds], bins=self.age_bin_edges, weights=self.scale[inds])[0]
         return cases_by_age, self.scale_flows(inds)
 
 
     def check_cancer(self, genotype):
         ''' Check for new progressions to cancer '''
         filter_inds = self.true('transformed')
         inds = self.check_inds(self.cancerous[genotype,:], self.date_cancerous[genotype,:], filter_inds=filter_inds)
@@ -484,87 +558,90 @@
         # Deal with dysplasia states and dates
         for g in range(self.ng):
             if g != genotype:
                 self.date_cancerous[g, inds] = np.nan  # Remove their date of cancer for all genotypes but the one currently causing cancer
                 self.date_cin1[g, inds] = np.nan
                 self.date_cin2[g, inds] = np.nan
                 self.date_cin3[g, inds] = np.nan
-            else:
-                date_cin2 = self.date_cin2[g,inds]
-                change_inds = hpu.true(date_cin2 > self.t)
-                self.date_cin2[g,inds[change_inds]] = np.nan
-
-                date_cin3 = self.date_cin3[g,inds]
-                change_inds = hpu.true(date_cin3 > self.t)
-                self.date_cin3[g,inds[change_inds]] = np.nan
 
         # Set the properties related to cell changes and disease severity markers
         self.cancerous[genotype, inds] = True
         self.episomal[:, inds] = False  # No longer counted as episomal with any genotype
         self.transformed[:, inds] = False  # No longer counted as transformed with any genotype
         self.sev[:, inds] = np.nan # NOTE: setting this to nan means this people no longer counts as CIN1/2/3, since those categories are based on this value
 
         # Age results
-        cases_by_age = np.histogram(self.age[inds], bins=self.age_bins, weights=self.scale[inds])[0]
+        cases_by_age = np.histogram(self.age[inds], bins=self.age_bin_edges, weights=self.scale[inds])[0]
+
 
         return cases_by_age, self.scale_flows(inds)
 
 
     def check_cancer_deaths(self):
         '''
         Check for new deaths from cancer
         '''
         filter_inds = self.true('cancerous')
         inds = self.check_inds(self.dead_cancer, self.date_dead_cancer, filter_inds=filter_inds)
         self.remove_people(inds, cause='cancer')
-        if len(inds):
-            cases_by_age = np.histogram(self.age[inds], bins=self.age_bins, weights=self.scale[inds])[0]
+        cases_by_age = np.histogram(self.age[inds], bins=self.age_bin_edges, weights=self.scale[inds])[0]
 
         # check which of these were detected by symptom or screening
         self.flows['detected_cancer_deaths'] += self.scale_flows(hpu.true(self.detected_cancer[inds]))
 
-        return self.scale_flows(inds)
+        return cases_by_age, self.scale_flows(inds)
 
 
     def check_clearance(self, genotype):
         '''
         Check for HPV clearance.
         '''
-        filter_inds = self.true_by_genotype('infectious', genotype)
-        inds = self.check_inds_true(self.infectious[genotype,:], self.date_clearance[genotype,:], filter_inds=filter_inds)
+        f_filter_inds = (self.is_female_alive & self.infectious[genotype,:]).nonzero()[-1]
+        m_filter_inds = (self.is_male_alive   & self.infectious[genotype,:]).nonzero()[-1]
+        f_inds = self.check_inds_true(self.infectious[genotype,:], self.date_clearance[genotype,:], filter_inds=f_filter_inds)
+        m_inds = self.check_inds_true(self.infectious[genotype,:], self.date_clearance[genotype,:], filter_inds=m_filter_inds)
+        m_cleared_inds = m_inds # All males clear
+
+        # For females, determine who clears and who controls
+        if self.pars['hpv_control_prob']>0:
+            latent_probs = np.full(len(f_inds), self.pars['hpv_control_prob'], dtype=hpd.default_float)
+            latent_bools = hpu.binomial_arr(latent_probs)
+            latent_inds = f_inds[latent_bools]
+
+            if len(latent_inds):
+                self.susceptible[genotype, latent_inds] = False  # should already be false
+                self.infectious[genotype, latent_inds] = False
+                self.inactive[genotype, latent_inds] = True
+                self.date_clearance[genotype, latent_inds] = np.nan
+
+            f_cleared_inds = f_inds[~latent_bools]
 
-        # Determine who clears and who controls
-        latent_probs = np.full(len(inds), self.pars['hpv_control_prob'], dtype=hpd.default_float)
-        latent_bools = hpu.binomial_arr(latent_probs)
+        else:
+            f_cleared_inds = f_inds
 
-        latent_inds = inds[latent_bools]
-        cleared_inds = inds[~latent_bools]
+        cleared_inds = np.array(m_cleared_inds.tolist()+f_cleared_inds.tolist())
 
         # Now reset disease states
         if len(cleared_inds):
             self.susceptible[genotype, cleared_inds] = True
             self.infectious[genotype, cleared_inds] = False
             self.inactive[genotype, cleared_inds] = False # should already be false
-            female_cleared_inds = np.intersect1d(cleared_inds, self.f_inds) # Only give natural immunity to females
-            hpimm.update_peak_immunity(self, female_cleared_inds, imm_pars=self.pars, imm_source=genotype) # update immunity
 
-        if len(latent_inds):
-            self.susceptible[genotype, latent_inds] = False # should already be false
-            self.infectious[genotype, latent_inds] = False
-            self.inactive[genotype, latent_inds] = True
-            self.date_clearance[genotype, latent_inds] = np.nan
+        if len(f_cleared_inds):
+            # female_cleared_inds = np.intersect1d(cleared_inds, self.f_inds) # Only give natural immunity to females
+            hpimm.update_peak_immunity(self, f_cleared_inds, imm_pars=self.pars, imm_source=genotype) # update immunity
+            self.date_reactivated[genotype, f_cleared_inds] = np.nan
 
         # Whether infection is controlled on not, clear all cell changes and severity markeres
-        self.episomal[genotype, inds] = False
-        self.transformed[genotype, inds] = False
-        self.sev[genotype, inds] = np.nan
-        self.date_cin1[genotype, inds] = np.nan
-        self.date_cin2[genotype, inds] = np.nan
-        self.date_cin3[genotype, inds] = np.nan
-        self.date_carcinoma[genotype, inds] = np.nan
+        self.episomal[genotype, f_inds] = False
+        self.transformed[genotype, f_inds] = False
+        self.sev[genotype, f_inds] = np.nan
+        self.date_cin1[genotype, f_inds] = np.nan
+        self.date_cin2[genotype, f_inds] = np.nan
+        self.date_cin3[genotype, f_inds] = np.nan
 
         return
 
 
     def apply_death_rates(self, year=None):
         '''
         Apply death rates to remove people from the population
@@ -614,15 +691,15 @@
             this_birth_rate = self.pars['rel_birth']*np.interp(year, years, rates)*self.pars['dt_demog']/1e3
             new_births = sc.randround(this_birth_rate*self.n_alive_level0) # Crude births per 1000
 
         if new_births>0:
             # Generate other characteristics of the new people
             uids, sexes, debuts, rel_sev, partners = hppop.set_static(new_n=new_births, existing_n=len(self), pars=self.pars)
             
-            # Grow the arrays
+            # Grow the arrays`
             new_inds = self._grow(new_births)
             self.uid[new_inds]          = uids
             self.age[new_inds]          = ages
             self.scale[new_inds]        = self.pars['pop_scale']
             self.sex[new_inds]          = sexes
             self.debut[new_inds]        = debuts
             self.rel_sev[new_inds]      = rel_sev
@@ -661,32 +738,35 @@
                 errormsg = 'Starting the sim earlier than the data is not hard, but has not been done yet'
                 raise NotImplementedError(errormsg)
 
             # Do basic calculations
             data_pop0 = np.interp(sim_start, data_years, data_pop)
             scale = sim_pop0 / data_pop0 # Scale factor
             alive_inds = hpu.true(self.alive_level0)
-            ages = self.age[alive_inds].astype(int) # Return ages for everyone level 0 and alive
-            count_ages = np.bincount(ages, minlength=age_dist_data.shape[0]) # Bin and count them
+            alive_ages = self.age[alive_inds].astype(int) # Return ages for everyone level 0 and alive
+            count_ages = np.bincount(alive_ages, minlength=age_dist_data.shape[0]) # Bin and count them
             expected = age_dist_data['PopTotal'].values*scale # Compute how many of each age we would expect in population
-            difference = np.array([int(i) for i in (expected - count_ages)]) # Compute difference between expected and simulated for each age
+            difference = (expected-count_ages).astype(int) # Compute difference between expected and simulated for each age
             n_migrate = np.sum(difference) # Compute total migrations (in and out)
             ages_to_remove = hpu.true(difference<0) # Ages where we have too many, need to apply emigration
-            n_to_remove = [int(i) for i in difference[ages_to_remove]] # Determine number of agents to remove for each age
+            n_to_remove = difference[ages_to_remove] # Determine number of agents to remove for each age
             ages_to_add = hpu.true(difference>0) # Ages where we have too few, need to apply imigration
-            n_to_add = [int(i) for i in difference[ages_to_add]] # Determine number of agents to add for each age
+            n_to_add = difference[ages_to_add] # Determine number of agents to add for each age
             ages_to_add_list = np.repeat(ages_to_add, n_to_add)
             self.add_births(new_births=len(ages_to_add_list), ages=np.array(ages_to_add_list))
 
-            for ind, diff in enumerate(n_to_remove): #TODO: is there a faster way to do this than in a for loop?
+            # Remove people
+            remove_frac = n_to_remove / count_ages[ages_to_remove]
+            remove_probs = np.zeros(len(self))
+            for ind,rf in enumerate(remove_frac):
                 age = ages_to_remove[ind]
-                alive_this_age_inds = np.where(ages==age)[0]
-                inds = hpu.choose(len(alive_this_age_inds), -diff)
-                migrate_inds = alive_inds[alive_this_age_inds[inds]]
-                self.remove_people(migrate_inds, cause='emigration')  # Remove people
+                inds_this_age = hpu.true((self.age>=age) * (self.age<age+1) * self.alive_level0)
+                remove_probs[inds_this_age] = -rf
+            migrate_inds = hpu.choose_w(remove_probs, -n_to_remove.sum())
+            self.remove_people(migrate_inds, cause='emigration')  # Remove people
 
         else:
             n_migrate = 0
 
         return n_migrate*self.pars['pop_scale'] # These are not indices, so they scale differently
 
 
@@ -756,44 +836,45 @@
         for key in ['date_clearance', 'date_transformed']:
             self[key][g, inds] = np.nan
 
         # Count reactivations and adjust latency status
         if layer == 'reactivation':
             self.genotype_flows['reactivations'][g] += self.scale_flows(inds)
             self.flows['reactivations']             += self.scale_flows(inds)
-            self.age_flows['reactivations']         += np.histogram(self.age[inds], bins=self.age_bins, weights=self.scale[inds])[0]
+            self.age_flows['reactivations']         += np.histogram(self.age[inds], bins=self.age_bin_edges, weights=self.scale[inds])[0]
             self.latent[g, inds] = False # Adjust states -- no longer latent
+            self.date_reactivated[g,inds]           = base_t
 
         # Update states, genotype info, and flows
         self.susceptible[g, inds]   = False # no longer susceptible
         self.infectious[g, inds]    = True  # now infectious
         self.episomal[g, inds]      = True  # now episomal
         self.inactive[g, inds]      = False  # no longer inactive
 
         # Add to flow results. Note, we only count these infectious in the results if they happened at this timestep
         if layer != 'seed_infection':
             # Create overall flows
             self.flows['infections']                += self.scale_flows(inds) # Add the total count to the total flow data
             self.genotype_flows['infections'][g]    += self.scale_flows(inds) # Add the count by genotype to the flow data
-            self.age_flows['infections'][:]         += np.histogram(self.age[inds], bins=self.age_bins, weights=self.scale[inds])[0]
+            self.age_flows['infections'][:]         += np.histogram(self.age[inds], bins=self.age_bin_edges, weights=self.scale[inds])[0]
 
             # Create by-sex flows
             infs_female = self.scale_flows(hpu.true(self.is_female[inds]))
             infs_male = self.scale_flows(hpu.true(self.is_male[inds]))
             self.sex_flows['infections_by_sex'][0] += infs_female
             self.sex_flows['infections_by_sex'][1] += infs_male
 
         # Now use genotype-specific prognosis probabilities to determine what happens.
         # Only women can progress beyond infection.
         f_inds = hpu.itruei(self.is_female,inds)
         m_inds = hpu.itruei(self.is_male,inds)
 
         # Compute disease progression for females
         if len(f_inds)>0:
-            gpars = self.pars['genotype_pars'][self.pars['genotype_map'][g]]
+            gpars = self.pars['genotype_pars'][g]
             self.set_prognoses(f_inds, g, gpars, dt)
 
         # Compute infection clearance for males
         if len(m_inds)>0:
             dur_infection = hpu.sample(**self.pars['dur_infection_male'], size=len(m_inds))
             self.date_clearance[g, m_inds] = self.date_infectious[g, m_inds] + np.ceil(dur_infection/dt)  # Date they clear HPV infection (interpreted as the timestep on which they recover)
```

### Comparing `hpvsim-1.1.1/hpvsim/plotting.py` & `hpvsim-1.2.0/hpvsim/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,15 +502,15 @@
     '''
     Function to plot a single age result for a single date. Requires an axis as
     input and will generally be called by a helper function rather than directly.
     '''
     idx = sc.findinds(sim.res_yearvec, date)[0]
     res = sim.results[reskey]
     label = res.name.replace('by age', '')
-    x = sim['age_bins'][:-1]
+    x = sim['age_bin_edges'][:-1]
     ax.plot(x, res.values[:,idx], color=res.color, **args.plot, label=label)
     ax.set_xlabel('Age')
     ax.set_ylabel('Value')
     return ax
```

### Comparing `hpvsim-1.1.1/hpvsim/population.py` & `hpvsim-1.2.0/hpvsim/population.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,21 +103,23 @@
         is_female = sexes == 0
 
         # Create the contacts
         lkeys = sim['partners'].keys() # TODO: consider a more robust way to do this
         if microstructure in ['random', 'default']:
             contacts = dict()
             current_partners = np.zeros((len(lkeys),n_agents))
-            for lno,lkey in enumerate(lkeys):
+            lno=0
+            for lkey in lkeys:
                 contacts[lkey], current_partners,_,_ = make_contacts(
                     lno=lno, tind=0, partners=partners[lno,:], current_partners=current_partners,
                     sexes=sexes, ages=ages, debuts=debuts, is_female=is_female, is_active=is_active,
                     mixing=sim['mixing'][lkey], layer_probs=sim['layer_probs'][lkey], cross_layer=sim['cross_layer'],
                     pref_weight=100, durations=sim['dur_pship'][lkey], acts=sim['acts'][lkey], age_act_pars=sim['age_act_pars'][lkey], **kwargs
                 )
+                lno += 1
 
         else:
             errormsg = f'Microstructure type "{microstructure}" not found; choices are random or TBC'
             raise NotImplementedError(errormsg)
 
         popdict['contacts'] = contacts
         popdict['current_partners'] = current_partners
```

### Comparing `hpvsim-1.1.1/hpvsim/regression/pars_v0.2.6.json` & `hpvsim-1.2.0/hpvsim/regression/pars_v0.2.6.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/regression/pars_v0.2.9.json` & `hpvsim-1.2.0/hpvsim/regression/pars_v0.2.9.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/regression/pars_v0.3.0.json` & `hpvsim-1.2.0/hpvsim/regression/pars_v0.3.0.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/regression/pars_v0.3.1.json` & `hpvsim-1.2.0/hpvsim/regression/pars_v0.3.1.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/run.py` & `hpvsim-1.2.0/hpvsim/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         raw = {}
 
         totalkeys = reduced_sim.result_keys('total')
         genotypekeys = reduced_sim.result_keys('genotype')
         sexkeys = reduced_sim.result_keys('sex')
         agekeys = reduced_sim.result_keys('age')
         type_dist_keys = reduced_sim.result_keys('type_dist')
-        n_age_bins = len(reduced_sim['age_bins'])-1
+        n_age_bins = len(reduced_sim['age_bin_edges'])-1
 
         for reskey in totalkeys:
             raw[reskey] = np.zeros((reduced_sim.res_npts, len(self.sims)))
             for s,sim in enumerate(self.sims):
                 vals = sim.results[reskey].values
                 raw[reskey][:, s] = vals
         for reskey in genotypekeys:
@@ -1064,15 +1064,15 @@
                 scen_sims = [single_run(scen_sim, **run_args, **kwargs)]*self['n_runs'] # Ensure it has correct length -- WARNING, kludgy
             else:
                 scen_sims = multi_run(scen_sim, **run_args, **kwargs) # This is where the sims actually get run
 
             # Process the simulations
             print_heading(f'Processing {scenkey}')
             ng = scen_sims[0]['n_genotypes'] # Get number of genotypes
-            na = len(scen_sims[0]['age_bins'])-1 # Get number of age bins
+            na = len(scen_sims[0]['age_bin_edges'])-1 # Get number of age bins
             scenraw = {}
             for reskey in totalkeys:
                 scenraw[reskey] = np.zeros((self.res_npts, len(scen_sims)))
                 for s,sim in enumerate(scen_sims):
                     scenraw[reskey][:,s] = sim.results[reskey].values
             for reskey in genotypekeys+type_dist_keys:
                 scenraw[reskey] = np.zeros((ng, self.res_npts, len(scen_sims)))
```

### Comparing `hpvsim-1.1.1/hpvsim/settings.py` & `hpvsim-1.2.0/hpvsim/settings.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.1.1/hpvsim/sim.py` & `hpvsim-1.2.0/hpvsim/sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,3948 +136,4071 @@
 00000870: 696e 6720 7661 6c75 6573 2066 726f 6d20  ing values from 
 00000880: 7061 7261 6d65 7465 7273 2e70 7929 0a20  parameters.py). 
 00000890: 2020 2020 2020 2064 6566 6175 6c74 5f70         default_p
 000008a0: 6172 7320 3d20 6870 7061 722e 6d61 6b65  ars = hppar.make
 000008b0: 5f70 6172 7328 7665 7273 696f 6e3d 7665  _pars(version=ve
 000008c0: 7273 696f 6e29 2023 2053 7461 7274 2077  rsion) # Start w
 000008d0: 6974 6820 6465 6661 756c 7420 7061 7273  ith default pars
-000008e0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-000008f0: 2e5f 5f69 6e69 745f 5f28 6465 6661 756c  .__init__(defaul
-00000900: 745f 7061 7273 2920 2320 496e 6974 6961  t_pars) # Initia
-00000910: 6c69 7a65 2061 6e64 2073 6574 2074 6865  lize and set the
-00000920: 2070 6172 616d 6574 6572 7320 6173 2061   parameters as a
-00000930: 7474 7269 6275 7465 730a 0a20 2020 2020  ttributes..     
-00000940: 2020 2023 204c 6f61 6420 6461 7461 2c20     # Load data, 
-00000950: 696e 636c 7564 696e 6720 6461 7461 6669  including datafi
-00000960: 6c65 2074 6861 7420 6172 6520 7573 6564  le that are used
-00000970: 2074 6f20 6372 6561 7465 2061 6464 6974   to create addit
-00000980: 696f 6e61 6c20 6f70 7469 6f6e 616c 2070  ional optional p
-00000990: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-000009a0: 2020 7365 6c66 2e6c 6f61 645f 6461 7461    self.load_data
-000009b0: 2864 6174 6166 696c 6529 2023 204c 6f61  (datafile) # Loa
-000009c0: 6420 7468 6520 6461 7461 2c20 6966 2070  d the data, if p
-000009d0: 726f 7669 6465 640a 0a20 2020 2020 2020  rovided..       
-000009e0: 2023 2055 7064 6174 6520 7061 7261 6d65   # Update parame
-000009f0: 7465 7273 0a20 2020 2020 2020 2073 656c  ters.        sel
-00000a00: 662e 7570 6461 7465 5f70 6172 7328 7061  f.update_pars(pa
-00000a10: 7273 2c20 2a2a 6b77 6172 6773 2920 2020  rs, **kwargs)   
-00000a20: 2320 5570 6461 7465 2074 6865 2070 6172  # Update the par
-00000a30: 616d 6574 6572 730a 0a20 2020 2020 2020  ameters..       
-00000a40: 2072 6574 7572 6e0a 0a0a 2020 2020 6465   return...    de
-00000a50: 6620 6c6f 6164 5f64 6174 6128 7365 6c66  f load_data(self
-00000a60: 2c20 6461 7461 6669 6c65 3d4e 6f6e 652c  , datafile=None,
-00000a70: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00000a80: 2020 2020 2727 2720 4c6f 6164 2074 6865      ''' Load the
-00000a90: 2064 6174 6120 746f 2063 616c 6962 7261   data to calibra
-00000aa0: 7465 2061 6761 696e 7374 2c20 6966 2070  te against, if p
-00000ab0: 726f 7669 6465 6420 2727 270a 2020 2020  rovided '''.    
-00000ac0: 2020 2020 6966 2064 6174 6166 696c 6520      if datafile 
-00000ad0: 6973 206e 6f74 204e 6f6e 653a 2023 2049  is not None: # I
-00000ae0: 6620 6120 6461 7461 2066 696c 6520 6973  f a data file is
-00000af0: 2070 726f 7669 6465 642c 206c 6f61 6420   provided, load 
-00000b00: 6974 0a20 2020 2020 2020 2020 2020 2073  it.            s
-00000b10: 656c 662e 6461 7461 203d 2068 706d 2e6c  elf.data = hpm.l
-00000b20: 6f61 645f 6461 7461 2864 6174 6166 696c  oad_data(datafil
-00000b30: 653d 6461 7461 6669 6c65 2c20 6368 6563  e=datafile, chec
-00000b40: 6b5f 6461 7465 3d54 7275 652c 202a 2a6b  k_date=True, **k
-00000b50: 7761 7267 7329 0a20 2020 2020 2020 2072  wargs).        r
-00000b60: 6574 7572 6e0a 0a0a 2020 2020 6465 6620  eturn...    def 
-00000b70: 696e 6974 6961 6c69 7a65 2873 656c 662c  initialize(self,
-00000b80: 2072 6573 6574 3d46 616c 7365 2c20 696e   reset=False, in
-00000b90: 6974 5f73 7461 7465 733d 5472 7565 2c20  it_states=True, 
-00000ba0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-00000bb0: 2020 2027 2727 0a20 2020 2020 2020 2050     '''.        P
-00000bc0: 6572 666f 726d 2061 6c6c 2069 6e69 7469  erform all initi
-00000bd0: 616c 697a 6174 696f 6e73 206f 6e20 7468  alizations on th
-00000be0: 6520 7369 6d2e 0a20 2020 2020 2020 2027  e sim..        '
-00000bf0: 2727 0a20 2020 2020 2020 2073 656c 662e  ''.        self.
-00000c00: 7420 3d20 3020 2023 2054 6865 2063 7572  t = 0  # The cur
-00000c10: 7265 6e74 2074 696d 6520 696e 6465 780a  rent time index.
-00000c20: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00000c30: 6964 6174 655f 7061 7273 2829 2023 2045  idate_pars() # E
-00000c40: 6e73 7572 6520 7061 7261 6d65 7465 7273  nsure parameters
-00000c50: 2068 6176 6520 7661 6c69 6420 7661 6c75   have valid valu
-00000c60: 6573 0a20 2020 2020 2020 2068 7075 2e73  es.        hpu.s
-00000c70: 6574 5f73 6565 6428 7365 6c66 5b27 7261  et_seed(self['ra
-00000c80: 6e64 5f73 6565 6427 5d29 2023 2052 6573  nd_seed']) # Res
-00000c90: 6574 2074 6865 2072 616e 646f 6d20 7365  et the random se
-00000ca0: 6564 2062 6566 6f72 6520 7468 6520 706f  ed before the po
-00000cb0: 7075 6c61 7469 6f6e 2069 7320 6372 6561  pulation is crea
-00000cc0: 7465 640a 2020 2020 2020 2020 7365 6c66  ted.        self
-00000cd0: 2e69 6e69 745f 6765 6e6f 7479 7065 7328  .init_genotypes(
-00000ce0: 2920 2320 496e 6974 6961 6c69 7a65 2074  ) # Initialize t
-00000cf0: 6865 2067 656e 6f74 7970 6573 0a20 2020  he genotypes.   
-00000d00: 2020 2020 2073 656c 662e 696e 6974 5f72       self.init_r
-00000d10: 6573 756c 7473 2829 2023 2041 6674 6572  esults() # After
-00000d20: 2069 6e69 7469 616c 697a 696e 6720 7468   initializing th
-00000d30: 6520 6765 6e6f 7479 7065 7320 616e 6420  e genotypes and 
-00000d40: 7065 6f70 6c65 2c20 6372 6561 7465 2074  people, create t
-00000d50: 6865 2072 6573 756c 7473 2073 7472 7563  he results struc
-00000d60: 7475 7265 0a20 2020 2020 2020 2073 656c  ture.        sel
-00000d70: 662e 696e 6974 5f69 6e74 6572 7665 6e74  f.init_intervent
-00000d80: 696f 6e73 2829 2020 2320 496e 6974 6961  ions()  # Initia
-00000d90: 6c69 7a65 2074 6865 2069 6e74 6572 7665  lize the interve
-00000da0: 6e74 696f 6e73 2042 4546 4f52 4520 7468  ntions BEFORE th
-00000db0: 6520 7065 6f70 6c65 2c20 6265 6361 7573  e people, becaus
-00000dc0: 6520 7468 656e 2076 6163 6369 6e61 7469  e then vaccinati
-00000dd0: 6f6e 2069 6e74 6572 7665 6e74 696f 6e73  on interventions
-00000de0: 2067 6574 2063 6f75 6e74 6564 2069 6e20   get counted in 
-00000df0: 696d 6d75 6e69 7479 2073 7472 7563 7475  immunity structu
-00000e00: 7265 730a 2020 2020 2020 2020 7365 6c66  res.        self
-00000e10: 2e69 6e69 745f 696d 6d75 6e69 7479 2829  .init_immunity()
-00000e20: 2023 2069 6e69 7469 616c 697a 6520 696e   # initialize in
-00000e30: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-00000e40: 696d 6d75 6e69 7479 0a20 2020 2020 2020  immunity.       
-00000e50: 2073 656c 662e 696e 6974 5f70 656f 706c   self.init_peopl
-00000e60: 6528 7265 7365 743d 7265 7365 742c 2069  e(reset=reset, i
-00000e70: 6e69 745f 7374 6174 6573 3d69 6e69 745f  nit_states=init_
-00000e80: 7374 6174 6573 2c20 2a2a 6b77 6172 6773  states, **kwargs
-00000e90: 2920 2320 4372 6561 7465 2061 6c6c 2074  ) # Create all t
-00000ea0: 6865 2070 656f 706c 6520 2874 6865 2068  he people (the h
-00000eb0: 6561 7669 6573 7420 7374 6570 290a 2020  eaviest step).  
-00000ec0: 2020 2020 2020 7365 6c66 2e69 6e69 745f        self.init_
-00000ed0: 616e 616c 797a 6572 7328 2920 2023 202e  analyzers()  # .
-00000ee0: 2e2e 616e 6420 7468 6520 616e 616c 797a  ..and the analyz
-00000ef0: 6572 732e 2e2e 0a20 2020 2020 2020 2068  ers....        h
-00000f00: 7075 2e73 6574 5f73 6565 6428 7365 6c66  pu.set_seed(self
-00000f10: 5b27 7261 6e64 5f73 6565 6427 5d2b 3129  ['rand_seed']+1)
-00000f20: 2020 2320 5265 7365 7420 7468 6520 7261    # Reset the ra
-00000f30: 6e64 6f6d 2073 6565 6420 746f 2074 6865  ndom seed to the
-00000f40: 2064 6566 6175 6c74 2072 756e 2073 6565   default run see
-00000f50: 642c 2073 6f20 7468 6174 2069 6620 7468  d, so that if th
-00000f60: 6520 7369 6d75 6c61 7469 6f6e 2069 7320  e simulation is 
-00000f70: 7275 6e20 7769 7468 2072 6573 6574 5f73  run with reset_s
-00000f80: 6565 643d 4661 6c73 6520 7269 6768 7420  eed=False right 
-00000f90: 6166 7465 7220 696e 6974 6961 6c69 7a61  after initializa
-00000fa0: 7469 6f6e 2c20 6974 2077 696c 6c20 7374  tion, it will st
-00000fb0: 696c 6c20 7072 6f64 7563 6520 7468 6520  ill produce the 
-00000fc0: 7361 6d65 206f 7574 7075 740a 2020 2020  same output.    
-00000fd0: 2020 2020 7365 6c66 2e69 6e69 7469 616c      self.initial
-00000fe0: 697a 6564 2020 203d 2054 7275 650a 2020  ized   = True.  
-00000ff0: 2020 2020 2020 7365 6c66 2e63 6f6d 706c        self.compl
-00001000: 6574 6520 2020 2020 203d 2046 616c 7365  ete      = False
-00001010: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00001020: 7375 6c74 735f 7265 6164 7920 3d20 4661  sults_ready = Fa
-00001030: 6c73 650a 0a20 2020 2020 2020 2072 6574  lse..        ret
-00001040: 7572 6e20 7365 6c66 0a0a 0a20 2020 2064  urn self...    d
-00001050: 6566 206c 6179 6572 5f6b 6579 7328 7365  ef layer_keys(se
-00001060: 6c66 293a 0a20 2020 2020 2020 2027 2727  lf):.        '''
-00001070: 0a20 2020 2020 2020 2041 7474 656d 7074  .        Attempt
-00001080: 2074 6f20 7265 7472 6965 7665 2074 6865   to retrieve the
-00001090: 2063 7572 7265 6e74 206c 6179 6572 206b   current layer k
-000010a0: 6579 732e 0a20 2020 2020 2020 2027 2727  eys..        '''
-000010b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-000010c0: 2020 2020 2020 2020 2020 6b65 7973 203d            keys =
-000010d0: 206c 6973 7428 7365 6c66 5b27 6163 7473   list(self['acts
-000010e0: 275d 2e6b 6579 7328 2929 2023 2047 6574  '].keys()) # Get
-000010f0: 206b 6579 7320 6672 6f6d 2061 6374 730a   keys from acts.
-00001100: 2020 2020 2020 2020 6578 6365 7074 3a20          except: 
-00001110: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-00001120: 6572 0a20 2020 2020 2020 2020 2020 206b  er.            k
-00001130: 6579 7320 3d20 5b5d 0a20 2020 2020 2020  eys = [].       
-00001140: 2072 6574 7572 6e20 6b65 7973 0a0a 0a20   return keys... 
-00001150: 2020 2064 6566 2072 6573 6574 5f6c 6179     def reset_lay
-00001160: 6572 5f70 6172 7328 7365 6c66 2c20 6c61  er_pars(self, la
-00001170: 7965 725f 6b65 7973 3d4e 6f6e 652c 2066  yer_keys=None, f
-00001180: 6f72 6365 3d46 616c 7365 293a 0a20 2020  orce=False):.   
-00001190: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000011a0: 2052 6573 6574 2074 6865 2070 6172 616d   Reset the param
-000011b0: 6574 6572 7320 746f 206d 6174 6368 2074  eters to match t
-000011c0: 6865 2070 6f70 756c 6174 696f 6e2e 0a0a  he population...
-000011d0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000011e0: 2020 2020 2020 2020 2020 6c61 7965 725f            layer_
-000011f0: 6b65 7973 2028 6c69 7374 293a 206f 7665  keys (list): ove
-00001200: 7272 6964 6520 7468 6520 6465 6661 756c  rride the defaul
-00001210: 7420 6c61 7965 7220 6b65 7973 2028 7573  t layer keys (us
-00001220: 6520 7374 6f72 6564 206b 6579 7320 6279  e stored keys by
-00001230: 2064 6566 6175 6c74 290a 2020 2020 2020   default).      
-00001240: 2020 2020 2020 666f 7263 6520 2862 6f6f        force (boo
-00001250: 6c29 3a20 7265 7365 7420 7468 6520 7061  l): reset the pa
-00001260: 7261 6d65 7465 7273 2065 7665 6e20 6966  rameters even if
-00001270: 2074 6865 7920 616c 7265 6164 7920 6578   they already ex
-00001280: 6973 740a 2020 2020 2020 2020 2727 270a  ist.        '''.
-00001290: 2020 2020 2020 2020 6966 206c 6179 6572          if layer
-000012a0: 5f6b 6579 7320 6973 204e 6f6e 653a 0a20  _keys is None:. 
-000012b0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000012c0: 6c66 2e70 656f 706c 6520 6973 206e 6f74  lf.people is not
-000012d0: 204e 6f6e 653a 2023 2049 6620 7065 6f70   None: # If peop
-000012e0: 6c65 2065 7869 7374 0a20 2020 2020 2020  le exist.       
-000012f0: 2020 2020 2020 2020 206c 6179 6572 5f6b           layer_k
-00001300: 6579 7320 3d20 7365 6c66 2e70 656f 706c  eys = self.peopl
-00001310: 652e 636f 6e74 6163 7473 2e6b 6579 7328  e.contacts.keys(
-00001320: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00001330: 6966 2073 656c 662e 706f 7064 6963 7420  if self.popdict 
-00001340: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00001350: 2020 2020 2020 2020 2020 2020 206c 6179               lay
-00001360: 6572 5f6b 6579 7320 3d20 7365 6c66 2e70  er_keys = self.p
-00001370: 6f70 6469 6374 5b27 6c61 7965 725f 6b65  opdict['layer_ke
-00001380: 7973 275d 0a20 2020 2020 2020 2068 7070  ys'].        hpp
-00001390: 6172 2e72 6573 6574 5f6c 6179 6572 5f70  ar.reset_layer_p
-000013a0: 6172 7328 7365 6c66 2e70 6172 732c 206c  ars(self.pars, l
-000013b0: 6179 6572 5f6b 6579 733d 6c61 7965 725f  ayer_keys=layer_
-000013c0: 6b65 7973 2c20 666f 7263 653d 666f 7263  keys, force=forc
-000013d0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-000013e0: 6e0a 0a0a 2020 2020 6465 6620 7661 6c69  n...    def vali
-000013f0: 6461 7465 5f6c 6179 6572 5f70 6172 7328  date_layer_pars(
-00001400: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
-00001410: 2727 0a20 2020 2020 2020 2048 616e 646c  ''.        Handl
-00001420: 6520 6c61 7965 7220 7061 7261 6d65 7465  e layer paramete
-00001430: 7273 2c20 7369 6e63 6520 7468 6579 206e  rs, since they n
-00001440: 6565 6420 746f 2062 6520 7661 6c69 6461  eed to be valida
-00001450: 7465 6420 6166 7465 7220 7468 6520 706f  ted after the po
-00001460: 7075 6c61 7469 6f6e 0a20 2020 2020 2020  pulation.       
-00001470: 2063 7265 6174 696f 6e2c 2072 6174 6865   creation, rathe
-00001480: 7220 7468 616e 2062 6566 6f72 652e 0a20  r than before.. 
-00001490: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
-000014a0: 2020 2020 2320 4669 7273 742c 2074 7279      # First, try
-000014b0: 2074 6f20 6669 6775 7265 206f 7574 2077   to figure out w
-000014c0: 6861 7420 7468 6520 6c61 7965 7220 6b65  hat the layer ke
-000014d0: 7973 2073 686f 756c 6420 6265 2061 6e64  ys should be and
-000014e0: 2070 6572 666f 726d 2062 6173 6963 2074   perform basic t
-000014f0: 7970 6520 6368 6563 6b69 6e67 0a20 2020  ype checking.   
-00001500: 2020 2020 206c 6179 6572 5f6b 6579 7320       layer_keys 
-00001510: 3d20 7365 6c66 2e6c 6179 6572 5f6b 6579  = self.layer_key
-00001520: 7328 290a 2020 2020 2020 2020 6c61 7965  s().        laye
-00001530: 725f 7061 7273 203d 2068 7070 6172 2e6c  r_pars = hppar.l
-00001540: 6179 6572 5f70 6172 7320 2320 5468 6520  ayer_pars # The 
-00001550: 6e61 6d65 7320 6f66 2074 6865 2070 6172  names of the par
-00001560: 616d 6574 6572 7320 7468 6174 2061 7265  ameters that are
-00001570: 2073 7065 6369 6669 6564 2062 7920 6c61   specified by la
-00001580: 7965 720a 2020 2020 2020 2020 666f 7220  yer.        for 
-00001590: 6c70 2069 6e20 6c61 7965 725f 7061 7273  lp in layer_pars
-000015a0: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
-000015b0: 6c20 3d20 7365 6c66 5b6c 705d 0a20 2020  l = self[lp].   
-000015c0: 2020 2020 2020 2020 2069 6620 7363 2e69           if sc.i
-000015d0: 736e 756d 6265 7228 7661 6c29 3a20 2320  snumber(val): # 
-000015e0: 4974 2773 2061 2073 6361 6c61 7220 696e  It's a scalar in
-000015f0: 7374 6561 6420 6f66 2061 2064 6963 742c  stead of a dict,
-00001600: 2061 7373 756d 6520 6974 2773 2061 6c6c   assume it's all
-00001610: 2063 6f6e 7461 6374 730a 2020 2020 2020   contacts.      
-00001620: 2020 2020 2020 2020 2020 7365 6c66 5b6c            self[l
-00001630: 705d 203d 207b 6b3a 7661 6c20 666f 7220  p] = {k:val for 
-00001640: 6b20 696e 206c 6179 6572 5f6b 6579 737d  k in layer_keys}
-00001650: 0a0a 2020 2020 2020 2020 2320 4861 6e64  ..        # Hand
-00001660: 6c65 206b 6579 206d 6973 6d61 7463 6865  le key mismatche
-00001670: 730a 2020 2020 2020 2020 666f 7220 6c70  s.        for lp
-00001680: 2069 6e20 6c61 7965 725f 7061 7273 3a0a   in layer_pars:.
-00001690: 2020 2020 2020 2020 2020 2020 6c70 5f6b              lp_k
-000016a0: 6579 7320 3d20 7365 7428 7365 6c66 2e70  eys = set(self.p
-000016b0: 6172 735b 6c70 5d2e 6b65 7973 2829 290a  ars[lp].keys()).
-000016c0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000016d0: 7020 213d 2027 6c61 7965 725f 7072 6f62  p != 'layer_prob
-000016e0: 7327 3a0a 2020 2020 2020 2020 2020 2020  s':.            
-000016f0: 2020 2020 6966 206e 6f74 206c 705f 6b65      if not lp_ke
-00001700: 7973 203d 3d20 7365 7428 6c61 7965 725f  ys == set(layer_
-00001710: 6b65 7973 293a 0a20 2020 2020 2020 2020  keys):.         
-00001720: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00001730: 6d73 6720 3d20 2741 7420 6c65 6173 7420  msg = 'At least 
-00001740: 6f6e 6520 6c61 7965 7220 7061 7261 6d65  one layer parame
-00001750: 7465 7220 6973 2069 6e63 6f6e 7369 7374  ter is inconsist
-00001760: 656e 7420 7769 7468 2074 6865 206c 6179  ent with the lay
-00001770: 6572 206b 6579 733b 2061 6c6c 2070 6172  er keys; all par
-00001780: 616d 6574 6572 7320 6d75 7374 2068 6176  ameters must hav
-00001790: 6520 7468 6520 7361 6d65 206b 6579 733a  e the same keys:
-000017a0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000017b0: 2020 2020 2020 6572 726f 726d 7367 202b        errormsg +
-000017c0: 3d20 6627 5c6e 7369 6d2e 6c61 7965 725f  = f'\nsim.layer_
-000017d0: 6b65 7973 2829 203d 207b 6c61 7965 725f  keys() = {layer_
-000017e0: 6b65 7973 7d27 0a20 2020 2020 2020 2020  keys}'.         
-000017f0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-00001800: 7032 2069 6e20 6c61 7965 725f 7061 7273  p2 in layer_pars
-00001810: 3a20 2320 4661 696c 206f 6e20 6669 7273  : # Fail on firs
-00001820: 7420 6572 726f 722c 2062 7574 2072 652d  t error, but re-
-00001830: 6c6f 6f70 2074 6f20 6c69 7374 2061 6c6c  loop to list all
-00001840: 206f 6620 7468 656d 0a20 2020 2020 2020   of them.       
-00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001860: 2065 7272 6f72 6d73 6720 2b3d 2066 275c   errormsg += f'\
-00001870: 6e7b 6c70 327d 203d 2027 202b 2027 2c20  n{lp2} = ' + ', 
-00001880: 272e 6a6f 696e 2873 656c 662e 7061 7273  '.join(self.pars
-00001890: 5b6c 7032 5d2e 6b65 7973 2829 290a 2020  [lp2].keys()).  
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018b0: 2020 7261 6973 6520 7363 2e4b 6579 4e6f    raise sc.KeyNo
-000018c0: 7446 6f75 6e64 4572 726f 7228 6572 726f  tFoundError(erro
-000018d0: 726d 7367 290a 0a20 2020 2020 2020 2020  rmsg)..         
-000018e0: 2020 2023 2054 4f44 4f3a 2061 6464 2076     # TODO: add v
-000018f0: 616c 6964 6174 696f 6e20 6865 7265 2066  alidation here f
-00001900: 6f72 206c 6179 6572 5f70 726f 6273 0a0a  or layer_probs..
-00001910: 2020 2020 2020 2020 2320 4861 6e64 6c65          # Handle
-00001920: 206d 6973 6d61 7463 6865 7320 7769 7468   mismatches with
-00001930: 2074 6865 2070 6f70 756c 6174 696f 6e0a   the population.
-00001940: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001950: 7065 6f70 6c65 2069 7320 6e6f 7420 4e6f  people is not No
-00001960: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00001970: 706f 705f 6b65 7973 203d 2073 6574 2873  pop_keys = set(s
-00001980: 656c 662e 7065 6f70 6c65 2e63 6f6e 7461  elf.people.conta
-00001990: 6374 732e 6b65 7973 2829 290a 2020 2020  cts.keys()).    
-000019a0: 2020 2020 2020 2020 6966 2070 6f70 5f6b          if pop_k
-000019b0: 6579 7320 213d 2073 6574 286c 6179 6572  eys != set(layer
-000019c0: 5f6b 6579 7329 3a20 2320 7072 6167 6d61  _keys): # pragma
-000019d0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
-000019e0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000019f0: 7420 6c65 6e28 706f 705f 6b65 7973 293a  t len(pop_keys):
-00001a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a10: 2020 2020 2065 7272 6f72 6d73 6720 3d20       errormsg = 
-00001a20: 6627 596f 7572 2070 6f70 756c 6174 696f  f'Your populatio
-00001a30: 6e20 646f 6573 206e 6f74 2068 6176 6520  n does not have 
-00001a40: 616e 7920 6c61 7965 7220 6b65 7973 2c20  any layer keys, 
-00001a50: 6275 7420 796f 7572 2073 696d 756c 6174  but your simulat
-00001a60: 696f 6e20 646f 6573 207b 6c61 7965 725f  ion does {layer_
-00001a70: 6b65 7973 7d2e 2049 6620 796f 7520 6361  keys}. If you ca
-00001a80: 6c6c 6564 2068 7076 2e50 656f 706c 6528  lled hpv.People(
-00001a90: 2920 6469 7265 6374 6c79 2c20 796f 7520  ) directly, you 
-00001aa0: 7072 6f62 6162 6c79 206e 6565 6420 6870  probably need hp
-00001ab0: 762e 6d61 6b65 5f70 656f 706c 6528 2920  v.make_people() 
-00001ac0: 696e 7374 6561 642e 270a 2020 2020 2020  instead.'.      
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00001ae0: 6973 6520 7363 2e4b 6579 4e6f 7446 6f75  ise sc.KeyNotFou
-00001af0: 6e64 4572 726f 7228 6572 726f 726d 7367  ndError(errormsg
-00001b00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001b10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001b20: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00001b30: 726d 7367 203d 2066 2750 6c65 6173 6520  rmsg = f'Please 
-00001b40: 7570 6461 7465 2079 6f75 7220 7061 7261  update your para
-00001b50: 6d65 7465 7220 6b65 7973 207b 6c61 7965  meter keys {laye
-00001b60: 725f 6b65 7973 7d20 746f 206d 6174 6368  r_keys} to match
-00001b70: 2070 6f70 756c 6174 696f 6e20 6b65 7973   population keys
-00001b80: 207b 706f 705f 6b65 7973 7d2e 2059 6f75   {pop_keys}. You
-00001b90: 206d 6179 2066 696e 6420 7369 6d2e 7265   may find sim.re
-00001ba0: 7365 745f 6c61 7965 725f 7061 7273 2829  set_layer_pars()
-00001bb0: 2068 656c 7066 756c 2e27 0a20 2020 2020   helpful.'.     
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001bd0: 6169 7365 2073 632e 4b65 794e 6f74 466f  aise sc.KeyNotFo
-00001be0: 756e 6445 7272 6f72 2865 7272 6f72 6d73  undError(errorms
-00001bf0: 6729 0a0a 2020 2020 2020 2020 7265 7475  g)..        retu
-00001c00: 726e 0a0a 0a20 2020 2064 6566 2076 616c  rn...    def val
-00001c10: 6964 6174 655f 7061 7273 2873 656c 662c  idate_pars(self,
-00001c20: 2076 616c 6964 6174 655f 6c61 7965 7273   validate_layers
-00001c30: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-00001c40: 2727 270a 2020 2020 2020 2020 536f 6d65  '''.        Some
-00001c50: 2070 6172 616d 6574 6572 7320 6361 6e20   parameters can 
-00001c60: 7461 6b65 206d 756c 7469 706c 6520 7479  take multiple ty
-00001c70: 7065 733b 2074 6869 7320 6d61 6b65 7320  pes; this makes 
-00001c80: 7468 656d 2063 6f6e 7369 7374 656e 742e  them consistent.
-00001c90: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00001ca0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
-00001cb0: 6461 7465 5f6c 6179 6572 7320 2862 6f6f  date_layers (boo
-00001cc0: 6c29 3a20 7768 6574 6865 7220 746f 2076  l): whether to v
-00001cd0: 616c 6964 6174 6520 6c61 7965 7220 7061  alidate layer pa
-00001ce0: 7261 6d65 7465 7273 2061 7320 7765 6c6c  rameters as well
-00001cf0: 2076 6961 2076 616c 6964 6174 655f 6c61   via validate_la
-00001d00: 7965 725f 7061 7273 2829 202d 2d20 7573  yer_pars() -- us
-00001d10: 7561 6c6c 7920 7965 732c 2065 7863 6570  ually yes, excep
-00001d20: 7420 6475 7269 6e67 2069 6e69 7469 616c  t during initial
-00001d30: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
-00001d40: 2727 270a 0a20 2020 2020 2020 2023 2048  '''..        # H
-00001d50: 616e 646c 6520 7479 7065 730a 2020 2020  andle types.    
-00001d60: 2020 2020 666f 7220 6b65 7920 696e 205b      for key in [
-00001d70: 276e 5f61 6765 6e74 7327 5d3a 0a20 2020  'n_agents']:.   
-00001d80: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00001d90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001da0: 6c66 5b6b 6579 5d20 3d20 696e 7428 7365  lf[key] = int(se
-00001db0: 6c66 5b6b 6579 5d29 0a20 2020 2020 2020  lf[key]).       
-00001dc0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00001dd0: 7074 696f 6e20 6173 2045 3a0a 2020 2020  ption as E:.    
-00001de0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00001df0: 726d 7367 203d 2066 2743 6f75 6c64 206e  rmsg = f'Could n
-00001e00: 6f74 2063 6f6e 7665 7274 207b 6b65 797d  ot convert {key}
-00001e10: 3d7b 7365 6c66 5b6b 6579 5d7d 206f 6620  ={self[key]} of 
-00001e20: 7b74 7970 6528 7365 6c66 5b6b 6579 5d29  {type(self[key])
-00001e30: 7d20 746f 2069 6e74 6567 6572 270a 2020  } to integer'.  
-00001e40: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00001e50: 6973 6520 5661 6c75 6545 7272 6f72 2865  ise ValueError(e
-00001e60: 7272 6f72 6d73 6729 2066 726f 6d20 450a  rrormsg) from E.
-00001e70: 0a20 2020 2020 2020 2023 2048 616e 646c  .        # Handl
-00001e80: 6520 7374 6172 740a 2020 2020 2020 2020  e start.        
-00001e90: 6966 2073 656c 665b 2773 7461 7274 275d  if self['start']
-00001ea0: 2069 6e20 5b4e 6f6e 652c 2030 5d3a 2023   in [None, 0]: #
-00001eb0: 2055 7365 2064 6566 6175 6c74 2073 7461   Use default sta
-00001ec0: 7274 0a20 2020 2020 2020 2020 2020 2073  rt.            s
-00001ed0: 656c 665b 2773 7461 7274 275d 203d 2032  elf['start'] = 2
-00001ee0: 3031 350a 0a20 2020 2020 2020 2023 2048  015..        # H
-00001ef0: 616e 646c 6520 656e 6420 616e 6420 6e5f  andle end and n_
-00001f00: 7965 6172 730a 2020 2020 2020 2020 6966  years.        if
-00001f10: 2073 656c 665b 2765 6e64 275d 3a0a 2020   self['end']:.  
-00001f20: 2020 2020 2020 2020 2020 7365 6c66 5b27            self['
-00001f30: 6e5f 7965 6172 7327 5d20 3d20 696e 7428  n_years'] = int(
-00001f40: 7365 6c66 5b27 656e 6427 5d20 2d20 7365  self['end'] - se
-00001f50: 6c66 5b27 7374 6172 7427 5d29 0a20 2020  lf['start']).   
-00001f60: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00001f70: 5b27 6e5f 7965 6172 7327 5d20 3c3d 2030  ['n_years'] <= 0
-00001f80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001f90: 2020 6572 726f 726d 7367 203d 2066 224e    errormsg = f"N
-00001fa0: 756d 6265 7220 6f66 2079 6561 7273 206d  umber of years m
-00001fb0: 7573 7420 6265 203e 302c 2062 7574 2079  ust be >0, but y
-00001fc0: 6f75 2073 7570 706c 6965 6420 7374 6172  ou supplied star
-00001fd0: 743d 7b73 7472 2873 656c 665b 2773 7461  t={str(self['sta
-00001fe0: 7274 275d 297d 2061 6e64 2065 6e64 3d7b  rt'])} and end={
-00001ff0: 7374 7228 7365 6c66 5b27 656e 6427 5d29  str(self['end'])
-00002000: 7d2c 2077 6869 6368 2067 6976 6573 206e  }, which gives n
-00002010: 5f79 6561 7273 3d7b 7365 6c66 5b27 6e5f  _years={self['n_
-00002020: 7965 6172 7327 5d7d 220a 2020 2020 2020  years']}".      
-00002030: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00002040: 5661 6c75 6545 7272 6f72 2865 7272 6f72  ValueError(error
-00002050: 6d73 6729 0a20 2020 2020 2020 2065 6c73  msg).        els
-00002060: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00002070: 6620 7365 6c66 5b27 6e5f 7965 6172 7327  f self['n_years'
-00002080: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00002090: 2020 2073 656c 665b 2765 6e64 275d 203d     self['end'] =
-000020a0: 2073 656c 665b 2773 7461 7274 275d 202b   self['start'] +
-000020b0: 2073 656c 665b 276e 5f79 6561 7273 275d   self['n_years']
-000020c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000020d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000020e0: 2020 2065 7272 6f72 6d73 6720 3d20 2759     errormsg = 'Y
-000020f0: 6f75 206d 7573 7420 7375 7070 6c79 206f  ou must supply o
-00002100: 6e65 206f 6620 6e5f 7965 6172 7320 616e  ne of n_years an
-00002110: 6420 656e 642e 2227 0a20 2020 2020 2020  d end."'.       
-00002120: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00002130: 616c 7565 4572 726f 7228 6572 726f 726d  alueError(errorm
-00002140: 7367 290a 0a20 2020 2020 2020 2023 2043  sg)..        # C
-00002150: 6f6e 7374 7275 6374 206f 7468 6572 2074  onstruct other t
-00002160: 6869 6e67 7320 7468 6174 206b 6565 7020  hings that keep 
-00002170: 7472 6163 6b20 6f66 2074 696d 650a 2020  track of time.  
-00002180: 2020 2020 2020 7365 6c66 2e79 6561 7273        self.years
-00002190: 2020 2020 2020 3d20 7363 2e69 6e63 6c75        = sc.inclu
-000021a0: 7369 7665 7261 6e67 6528 7365 6c66 5b27  siverange(self['
-000021b0: 7374 6172 7427 5d2c 7365 6c66 5b27 656e  start'],self['en
-000021c0: 6427 5d29 0a20 2020 2020 2020 2073 656c  d']).        sel
-000021d0: 662e 7965 6172 7665 6320 2020 203d 2073  f.yearvec    = s
-000021e0: 632e 696e 636c 7573 6976 6572 616e 6765  c.inclusiverange
-000021f0: 2873 7461 7274 3d73 656c 665b 2773 7461  (start=self['sta
-00002200: 7274 275d 2c20 7374 6f70 3d73 656c 665b  rt'], stop=self[
-00002210: 2765 6e64 275d 2b31 2d73 656c 665b 2764  'end']+1-self['d
-00002220: 7427 5d2c 2073 7465 703d 7365 6c66 5b27  t'], step=self['
-00002230: 6474 275d 2920 2320 496e 636c 7564 6573  dt']) # Includes
-00002240: 2061 6c6c 2074 6865 2074 696d 6570 6f69   all the timepoi
-00002250: 6e74 7320 696e 2074 6865 206c 6173 7420  nts in the last 
-00002260: 7965 6172 0a20 2020 2020 2020 2073 656c  year.        sel
-00002270: 662e 6e70 7473 2020 2020 2020 203d 206c  f.npts       = l
-00002280: 656e 2873 656c 662e 7965 6172 7665 6329  en(self.yearvec)
-00002290: 0a20 2020 2020 2020 2073 656c 662e 7476  .        self.tv
-000022a0: 6563 2020 2020 2020 203d 206e 702e 6172  ec       = np.ar
-000022b0: 616e 6765 2873 656c 662e 6e70 7473 290a  ange(self.npts).
-000022c0: 0a20 2020 2020 2020 2023 2048 616e 646c  .        # Handl
-000022d0: 6520 706f 7075 6c61 7469 6f6e 206e 6574  e population net
-000022e0: 776f 726b 2064 6174 610a 2020 2020 2020  work data.      
-000022f0: 2020 6e65 7477 6f72 6b5f 6368 6f69 6365    network_choice
-00002300: 7320 3d20 5b27 7261 6e64 6f6d 272c 2027  s = ['random', '
-00002310: 6465 6661 756c 7427 5d0a 2020 2020 2020  default'].      
-00002320: 2020 6368 6f69 6365 203d 2073 656c 665b    choice = self[
-00002330: 276e 6574 776f 726b 275d 0a20 2020 2020  'network'].     
-00002340: 2020 2069 6620 6368 6f69 6365 2061 6e64     if choice and
-00002350: 2063 686f 6963 6520 6e6f 7420 696e 206e   choice not in n
-00002360: 6574 776f 726b 5f63 686f 6963 6573 3a20  etwork_choices: 
-00002370: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-00002380: 6572 0a20 2020 2020 2020 2020 2020 2063  er.            c
-00002390: 686f 6963 6573 7472 203d 2027 2c20 272e  hoicestr = ', '.
-000023a0: 6a6f 696e 286e 6574 776f 726b 5f63 686f  join(network_cho
-000023b0: 6963 6573 290a 2020 2020 2020 2020 2020  ices).          
-000023c0: 2020 6572 726f 726d 7367 203d 2066 2750    errormsg = f'P
-000023d0: 6f70 756c 6174 696f 6e20 7479 7065 2022  opulation type "
-000023e0: 7b63 686f 6963 657d 2220 6e6f 7420 6176  {choice}" not av
-000023f0: 6169 6c61 626c 653b 2063 686f 6963 6573  ailable; choices
-00002400: 2061 7265 3a20 7b63 686f 6963 6573 7472   are: {choicestr
-00002410: 7d27 0a20 2020 2020 2020 2020 2020 2072  }'.            r
-00002420: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00002430: 6572 726f 726d 7367 290a 0a20 2020 2020  errormsg)..     
-00002440: 2020 2023 2048 616e 646c 6520 616e 616c     # Handle anal
-00002450: 797a 6572 7320 616e 6420 696e 7465 7276  yzers and interv
-00002460: 656e 7469 6f6e 730a 2020 2020 2020 2020  entions.        
-00002470: 666f 7220 6b65 7920 696e 205b 2769 6e74  for key in ['int
-00002480: 6572 7665 6e74 696f 6e73 272c 2027 616e  erventions', 'an
-00002490: 616c 797a 6572 7327 5d3a 2023 2045 6e73  alyzers']: # Ens
-000024a0: 7572 6520 616c 6c20 6f66 2074 6865 6d20  ure all of them 
-000024b0: 6172 6520 6c69 7374 730a 2020 2020 2020  are lists.      
-000024c0: 2020 2020 2020 7365 6c66 5b6b 6579 5d20        self[key] 
-000024d0: 3d20 7363 2e64 6370 2873 632e 746f 6c69  = sc.dcp(sc.toli
-000024e0: 7374 2873 656c 665b 6b65 795d 2c20 6b65  st(self[key], ke
-000024f0: 6570 6e6f 6e65 3d46 616c 7365 2929 2023  epnone=False)) #
-00002500: 2041 6c6c 206f 6620 7468 6573 6520 6861   All of these ha
-00002510: 7665 2069 6e69 7469 616c 697a 6520 6675  ve initialize fu
-00002520: 6e63 7469 6f6e 7320 7468 6174 2072 756e  nctions that run
-00002530: 2069 6e74 6f20 6973 7375 6573 2069 6620   into issues if 
-00002540: 7468 6579 2772 6520 7265 7573 6564 0a20  they're reused. 
-00002550: 2020 2020 2020 2066 6f72 2069 2c69 6e74         for i,int
-00002560: 6572 7620 696e 2065 6e75 6d65 7261 7465  erv in enumerate
-00002570: 2873 656c 665b 2769 6e74 6572 7665 6e74  (self['intervent
-00002580: 696f 6e73 275d 293a 0a20 2020 2020 2020  ions']):.       
-00002590: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000025a0: 6365 2869 6e74 6572 762c 2064 6963 7429  ce(interv, dict)
-000025b0: 3a20 2320 4974 2773 2061 2064 6963 7469  : # It's a dicti
-000025c0: 6f6e 6172 7920 7265 7072 6573 656e 7461  onary representa
-000025d0: 7469 6f6e 206f 6620 616e 2069 6e74 6572  tion of an inter
-000025e0: 7665 6e74 696f 6e0a 2020 2020 2020 2020  vention.        
-000025f0: 2020 2020 2020 2020 7365 6c66 5b27 696e          self['in
-00002600: 7465 7276 656e 7469 6f6e 7327 5d5b 695d  terventions'][i]
-00002610: 203d 2068 7069 2e49 6e74 6572 7665 6e74   = hpi.Intervent
-00002620: 696f 6e44 6963 7428 2a2a 696e 7465 7276  ionDict(**interv
-00002630: 290a 0a20 2020 2020 2020 2023 204f 7074  )..        # Opt
-00002640: 696f 6e61 6c6c 7920 6861 6e64 6c65 206c  ionally handle l
-00002650: 6179 6572 2070 6172 616d 6574 6572 730a  ayer parameters.
-00002660: 2020 2020 2020 2020 6966 2076 616c 6964          if valid
-00002670: 6174 655f 6c61 7965 7273 3a0a 2020 2020  ate_layers:.    
-00002680: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00002690: 6964 6174 655f 6c61 7965 725f 7061 7273  idate_layer_pars
-000026a0: 2829 0a0a 2020 2020 2020 2020 2320 4861  ()..        # Ha
-000026b0: 6e64 6c65 2076 6572 626f 7365 0a20 2020  ndle verbose.   
-000026c0: 2020 2020 2069 6620 7365 6c66 5b27 7665       if self['ve
-000026d0: 7262 6f73 6527 5d20 3d3d 2027 6272 6965  rbose'] == 'brie
-000026e0: 6627 3a0a 2020 2020 2020 2020 2020 2020  f':.            
-000026f0: 7365 6c66 5b27 7665 7262 6f73 6527 5d20  self['verbose'] 
-00002700: 3d20 2d31 0a20 2020 2020 2020 2069 6620  = -1.        if 
-00002710: 6e6f 7420 7363 2e69 736e 756d 6265 7228  not sc.isnumber(
-00002720: 7365 6c66 5b27 7665 7262 6f73 6527 5d29  self['verbose'])
-00002730: 3a20 2320 7072 6167 6d61 3a20 6e6f 2063  : # pragma: no c
-00002740: 6f76 6572 0a20 2020 2020 2020 2020 2020  over.           
-00002750: 2065 7272 6f72 6d73 6720 3d20 6627 5665   errormsg = f'Ve
-00002760: 7262 6f73 6520 6172 6775 6d65 6e74 2073  rbose argument s
-00002770: 686f 756c 6420 6265 2065 6974 6865 7220  hould be either 
-00002780: 2262 7269 6566 222c 202d 312c 206f 7220  "brief", -1, or 
-00002790: 6120 666c 6f61 742c 206e 6f74 207b 7479  a float, not {ty
-000027a0: 7065 2873 656c 665b 2276 6572 626f 7365  pe(self["verbose
-000027b0: 225d 297d 2022 7b73 656c 665b 2276 6572  "])} "{self["ver
-000027c0: 626f 7365 225d 7d22 270a 2020 2020 2020  bose"]}"'.      
-000027d0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000027e0: 6545 7272 6f72 2865 7272 6f72 6d73 6729  eError(errormsg)
-000027f0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002800: 0a0a 0a20 2020 2064 6566 2076 616c 6964  ...    def valid
-00002810: 6174 655f 696e 6974 5f63 6f6e 6469 7469  ate_init_conditi
-00002820: 6f6e 7328 7365 6c66 2c20 696e 6974 5f68  ons(self, init_h
-00002830: 7076 5f70 7265 7629 3a0a 2020 2020 2020  pv_prev):.      
-00002840: 2020 2727 270a 2020 2020 2020 2020 496e    '''.        In
-00002850: 6974 6961 6c20 7072 6576 616c 656e 6365  itial prevalence
-00002860: 2076 616c 7565 7320 6361 6e20 6265 2073   values can be s
-00002870: 7570 706c 6965 6420 7769 7468 2064 6966  upplied with dif
-00002880: 6665 7265 6e74 2061 6d6f 756e 7473 206f  ferent amounts o
-00002890: 6620 6465 7461 696c 2e0a 2020 2020 2020  f detail..      
-000028a0: 2020 4865 7265 2077 6520 666c 6573 6820    Here we flesh 
-000028b0: 6f75 7420 616e 7920 6d69 7373 696e 6720  out any missing 
-000028c0: 6465 7461 696c 7320 736f 2074 6861 7420  details so that 
-000028d0: 7468 6520 696e 6974 6961 6c20 7072 6576  the initial prev
-000028e0: 2076 616c 7565 7320 6172 650a 2020 2020   values are.    
-000028f0: 2020 2020 6279 2061 6765 2061 6e64 2067      by age and g
-00002900: 656e 6f74 7970 652e 2057 6520 616c 736f  enotype. We also
-00002910: 2063 6865 636b 2074 6865 2070 7265 7661   check the preva
-00002920: 6c65 6e63 6520 7661 6c75 6573 2061 7265  lence values are
-00002930: 206f 6b2e 0a20 2020 2020 2020 2027 2727   ok..        '''
-00002940: 0a0a 2020 2020 2020 2020 6465 6620 7661  ..        def va
-00002950: 6c69 6461 7465 5f61 7272 6179 7328 7661  lidate_arrays(va
-00002960: 6c73 2c20 6e5f 6167 655f 6272 6163 6b65  ls, n_age_bracke
-00002970: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
-00002980: 2020 2020 2020 2727 2720 4c69 7474 6c65        ''' Little
-00002990: 2068 656c 7065 7220 6675 6e63 7469 6f6e   helper function
-000029a0: 2074 6f20 6368 6563 6b20 7072 6576 616c   to check preval
-000029b0: 656e 6365 2076 616c 7565 7320 2727 270a  ence values '''.
-000029c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000029d0: 5f61 6765 5f62 7261 636b 6574 7320 6973  _age_brackets is
-000029e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000029f0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00002a00: 6e28 7661 6c73 2920 213d 206e 5f61 6765  n(vals) != n_age
-00002a10: 5f62 7261 636b 6574 733a 0a20 2020 2020  _brackets:.     
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002a30: 7272 6f72 6d73 6720 3d20 6627 5468 6520  rrormsg = f'The 
-00002a40: 696e 6974 6961 6c20 7072 6576 616c 656e  initial prevalen
-00002a50: 6365 2076 616c 7565 7320 6d75 7374 2065  ce values must e
-00002a60: 6974 6865 7220 6265 2074 6865 2073 616d  ither be the sam
-00002a70: 6520 6c65 6e67 7468 2061 7320 7468 6520  e length as the 
-00002a80: 6167 6520 6272 6163 6b65 7473 3a20 7b6c  age brackets: {l
-00002a90: 656e 2876 616c 7329 7d20 7673 207b 6e5f  en(vals)} vs {n_
-00002aa0: 6167 655f 6272 6163 6b65 7473 7d2e 270a  age_brackets}.'.
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ac0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00002ad0: 7272 6f72 2865 7272 6f72 6d73 6729 0a20  rror(errormsg). 
-00002ae0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00002af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b00: 2069 6620 6c65 6e28 7661 6c73 2920 213d   if len(vals) !=
-00002b10: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00002b20: 2020 2020 2020 2020 6572 726f 726d 7367          errormsg
-00002b30: 203d 2066 274e 6f20 6167 6520 6272 6163   = f'No age brac
-00002b40: 6b65 7473 2077 6572 6520 7375 7070 6c69  kets were suppli
-00002b50: 6564 2c20 6275 7420 6d6f 7265 2074 6861  ed, but more tha
-00002b60: 6e20 6f6e 6520 7072 6576 616c 656e 6365  n one prevalence
-00002b70: 2076 616c 7565 2077 6173 2073 7570 706c   value was suppl
-00002b80: 6965 6420 287b 6c65 6e28 7661 6c73 297d  ied ({len(vals)}
-00002b90: 292e 2041 6e20 6172 7261 7920 6f66 2070  ). An array of p
-00002ba0: 7265 7661 6c65 6e63 6520 7661 6c75 6573  revalence values
-00002bb0: 2063 616e 206f 6e6c 7920 6265 2073 7570   can only be sup
-00002bc0: 706c 6965 6420 616c 6f6e 6720 7769 7468  plied along with
-00002bd0: 2061 6e20 6172 7261 7920 6f66 2063 6f72   an array of cor
-00002be0: 7265 7370 6f6e 6469 6e67 2061 6765 2062  responding age b
-00002bf0: 7261 636b 6574 732e 270a 2020 2020 2020  rackets.'.      
-00002c00: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00002c10: 6973 6520 5661 6c75 6545 7272 6f72 2865  ise ValueError(e
-00002c20: 7272 6f72 6d73 6729 0a20 2020 2020 2020  rrormsg).       
-00002c30: 2020 2020 2069 6620 7661 6c73 2e61 6e79       if vals.any
-00002c40: 2829 203c 2030 206f 7220 7661 6c73 2e61  () < 0 or vals.a
-00002c50: 6e79 2829 203e 2031 3a0a 2020 2020 2020  ny() > 1:.      
-00002c60: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
-00002c70: 7367 203d 2066 2754 6865 2069 6e69 7469  sg = f'The initi
-00002c80: 616c 2070 7265 7661 6c65 6e63 6520 7661  al prevalence va
-00002c90: 6c75 6573 206d 7573 7420 6569 7468 6572  lues must either
-00002ca0: 2062 6574 7765 656e 2030 2061 6e64 2031   between 0 and 1
-00002cb0: 2c20 6e6f 7420 7b76 616c 737d 2e27 0a20  , not {vals}.'. 
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002cd0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00002ce0: 6572 726f 726d 7367 290a 0a20 2020 2020  errormsg)..     
-00002cf0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-00002d00: 2020 2020 2020 2023 2049 6620 7661 6c75         # If valu
-00002d10: 6573 2068 6176 6520 6265 656e 2070 726f  es have been pro
-00002d20: 7669 6465 642c 2076 616c 6964 6174 6520  vided, validate 
-00002d30: 7468 656d 0a20 2020 2020 2020 2073 6578  them.        sex
-00002d40: 5f6b 6579 7320 3d20 7b27 6d27 2c20 2766  _keys = {'m', 'f
-00002d50: 277d 0a20 2020 2020 2020 2074 6f74 5f6b  '}.        tot_k
-00002d60: 6579 7320 3d20 5b27 616c 6c27 2c20 2774  eys = ['all', 't
-00002d70: 6f74 616c 272c 2027 746f 7427 2c20 2761  otal', 'tot', 'a
-00002d80: 7665 7261 6765 272c 2027 6176 6727 5d0a  verage', 'avg'].
-00002d90: 2020 2020 2020 2020 6e5f 6167 655f 6272          n_age_br
-00002da0: 6163 6b65 7473 203d 204e 6f6e 650a 0a20  ackets = None.. 
-00002db0: 2020 2020 2020 2069 6620 696e 6974 5f68         if init_h
-00002dc0: 7076 5f70 7265 7620 6973 206e 6f74 204e  pv_prev is not N
-00002dd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002de0: 2069 6620 7363 2e63 6865 636b 7479 7065   if sc.checktype
-00002df0: 2869 6e69 745f 6870 765f 7072 6576 2c20  (init_hpv_prev, 
-00002e00: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-00002e10: 2020 2020 2020 2023 2047 6574 2061 6765         # Get age
-00002e20: 2062 7261 636b 6574 7320 6966 2073 7570   brackets if sup
-00002e30: 706c 6965 640a 2020 2020 2020 2020 2020  plied.          
-00002e40: 2020 2020 2020 6966 2027 6167 655f 6272        if 'age_br
-00002e50: 6163 6b65 7473 2720 696e 2069 6e69 745f  ackets' in init_
-00002e60: 6870 765f 7072 6576 2e6b 6579 7328 293a  hpv_prev.keys():
-00002e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e80: 2020 2020 2061 6765 5f62 7261 636b 6574       age_bracket
-00002e90: 7320 3d20 696e 6974 5f68 7076 5f70 7265  s = init_hpv_pre
-00002ea0: 762e 706f 7028 2761 6765 5f62 7261 636b  v.pop('age_brack
-00002eb0: 6574 7327 290a 2020 2020 2020 2020 2020  ets').          
-00002ec0: 2020 2020 2020 2020 2020 6e5f 6167 655f            n_age_
-00002ed0: 6272 6163 6b65 7473 203d 206c 656e 2861  brackets = len(a
-00002ee0: 6765 5f62 7261 636b 6574 7329 0a20 2020  ge_brackets).   
-00002ef0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00002f00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002f10: 2020 2020 2020 2061 6765 5f62 7261 636b         age_brack
-00002f20: 6574 7320 3d20 6e70 2e61 7272 6179 285b  ets = np.array([
-00002f30: 3135 305d 290a 0a20 2020 2020 2020 2020  150])..         
-00002f40: 2020 2020 2020 2023 2048 616e 646c 6520         # Handle 
-00002f50: 7468 6520 7265 7374 206f 6620 7468 6520  the rest of the 
-00002f60: 6b65 7973 0a20 2020 2020 2020 2020 2020  keys.           
-00002f70: 2020 2020 2076 6172 5f6b 6579 7320 3d20       var_keys = 
-00002f80: 6c69 7374 2869 6e69 745f 6870 765f 7072  list(init_hpv_pr
-00002f90: 6576 2e6b 6579 7328 2929 0a20 2020 2020  ev.keys()).     
-00002fa0: 2020 2020 2020 2020 2020 2069 6620 286c             if (l
-00002fb0: 656e 2876 6172 5f6b 6579 7329 3d3d 3120  en(var_keys)==1 
-00002fc0: 616e 6420 7661 725f 6b65 7973 5b30 5d20  and var_keys[0] 
-00002fd0: 6e6f 7420 696e 2074 6f74 5f6b 6579 7329  not in tot_keys)
-00002fe0: 206f 7220 286c 656e 2876 6172 5f6b 6579   or (len(var_key
-00002ff0: 7329 3e31 2061 6e64 2073 6574 2876 6172  s)>1 and set(var
-00003000: 5f6b 6579 7329 2021 3d20 7365 785f 6b65  _keys) != sex_ke
-00003010: 7973 293a 0a20 2020 2020 2020 2020 2020  ys):.           
-00003020: 2020 2020 2020 2020 2065 7272 6f72 6d73           errorms
-00003030: 6720 3d20 6627 436f 756c 6420 6e6f 7420  g = f'Could not 
-00003040: 756e 6465 7273 7461 6e64 2074 6865 2069  understand the i
-00003050: 6e69 7469 616c 2070 7265 7661 6c65 6e63  nitial prevalenc
-00003060: 6520 7072 6f76 6964 6564 3a20 7b69 6e69  e provided: {ini
-00003070: 745f 6870 765f 7072 6576 7d2e 2049 6620  t_hpv_prev}. If 
-00003080: 7375 7070 6c79 696e 6720 6120 6469 6374  supplying a dict
-00003090: 696f 6e61 7279 2c20 706c 6561 7365 2075  ionary, please u
-000030a0: 7365 2022 6d22 2061 6e64 2022 6622 206b  se "m" and "f" k
-000030b0: 6579 7320 6f72 2022 746f 7422 2e20 270a  eys or "tot". '.
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-000030e0: 7272 6f72 2865 7272 6f72 6d73 6729 0a20  rror(errormsg). 
-000030f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003100: 6620 6c65 6e28 7661 725f 6b65 7973 2920  f len(var_keys) 
-00003110: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00003120: 2020 2020 2020 2020 2020 6b20 3d20 7661            k = va
-00003130: 725f 6b65 7973 5b30 5d0a 2020 2020 2020  r_keys[0].      
-00003140: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00003150: 6974 5f68 7076 5f70 7265 7620 3d20 7b73  it_hpv_prev = {s
-00003160: 6b3a 2073 632e 7072 6f6d 6f74 6574 6f61  k: sc.promotetoa
-00003170: 7272 6179 2869 6e69 745f 6870 765f 7072  rray(init_hpv_pr
-00003180: 6576 5b6b 5d29 2066 6f72 2073 6b20 696e  ev[k]) for sk in
-00003190: 2073 6578 5f6b 6579 737d 0a0a 2020 2020   sex_keys}..    
-000031a0: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
-000031b0: 7720 7365 7420 7468 6520 7661 6c75 6573  w set the values
-000031c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000031d0: 2066 6f72 206b 2c20 7661 6c73 2069 6e20   for k, vals in 
-000031e0: 696e 6974 5f68 7076 5f70 7265 762e 6974  init_hpv_prev.it
-000031f0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00003200: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
-00003210: 6870 765f 7072 6576 5b6b 5d20 3d20 7363  hpv_prev[k] = sc
-00003220: 2e70 726f 6d6f 7465 746f 6172 7261 7928  .promotetoarray(
-00003230: 7661 6c73 290a 0a20 2020 2020 2020 2020  vals)..         
-00003240: 2020 2065 6c69 6620 7363 2e63 6865 636b     elif sc.check
-00003250: 7479 7065 2869 6e69 745f 6870 765f 7072  type(init_hpv_pr
-00003260: 6576 2c20 2761 7272 6179 6c69 6b65 2729  ev, 'arraylike')
-00003270: 206f 7220 7363 2e69 736e 756d 6265 7228   or sc.isnumber(
-00003280: 696e 6974 5f68 7076 5f70 7265 7629 3a0a  init_hpv_prev):.
-00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032a0: 2320 4966 2069 7427 7320 616e 2061 7272  # If it's an arr
-000032b0: 6179 2c20 6173 7375 6d65 2074 6865 7365  ay, assume these
-000032c0: 2076 616c 7565 7320 6170 706c 7920 746f   values apply to
-000032d0: 206d 616c 6573 2061 6e64 2066 656d 616c   males and femal
-000032e0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-000032f0: 2020 2069 6e69 745f 6870 765f 7072 6576     init_hpv_prev
-00003300: 203d 207b 736b 3a20 7363 2e70 726f 6d6f   = {sk: sc.promo
-00003310: 7465 746f 6172 7261 7928 696e 6974 5f68  tetoarray(init_h
-00003320: 7076 5f70 7265 7629 2066 6f72 2073 6b20  pv_prev) for sk 
-00003330: 696e 2073 6578 5f6b 6579 737d 0a20 2020  in sex_keys}.   
-00003340: 2020 2020 2020 2020 2020 2020 2061 6765               age
-00003350: 5f62 7261 636b 6574 7320 3d20 6e70 2e61  _brackets = np.a
-00003360: 7272 6179 285b 3135 305d 290a 0a20 2020  rray([150])..   
-00003370: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00003380: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003390: 7272 6f72 6d73 6720 3d20 6627 496e 6974  rrormsg = f'Init
-000033a0: 6961 6c20 7072 6576 616c 656e 6365 2076  ial prevalence v
-000033b0: 616c 7565 7320 6f66 2074 7970 6520 7b74  alues of type {t
-000033c0: 7970 6528 696e 6974 5f68 7076 5f70 7265  ype(init_hpv_pre
-000033d0: 7629 7d20 6e6f 7420 7265 636f 676e 697a  v)} not recogniz
-000033e0: 6564 2c20 6d75 7374 2062 6520 6120 6469  ed, must be a di
-000033f0: 6374 2c20 616e 2061 7272 6179 2c20 6f72  ct, an array, or
-00003400: 2061 2066 6c6f 6174 2e27 0a20 2020 2020   a float.'.     
-00003410: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003420: 2056 616c 7565 4572 726f 7228 6572 726f   ValueError(erro
-00003430: 726d 7367 290a 0a20 2020 2020 2020 2020  rmsg)..         
-00003440: 2020 2023 204e 6f77 2076 616c 6964 6174     # Now validat
-00003450: 6520 7468 6520 6172 7261 7973 0a20 2020  e the arrays.   
-00003460: 2020 2020 2020 2020 2066 6f72 2073 6b2c           for sk,
-00003470: 2076 616c 7320 696e 2069 6e69 745f 6870   vals in init_hp
-00003480: 765f 7072 6576 2e69 7465 6d73 2829 3a0a  v_prev.items():.
-00003490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034a0: 7661 6c69 6461 7465 5f61 7272 6179 7328  validate_arrays(
-000034b0: 7661 6c73 2c20 6e5f 6167 655f 6272 6163  vals, n_age_brac
-000034c0: 6b65 7473 290a 0a20 2020 2020 2020 2023  kets)..        #
-000034d0: 2049 6620 7661 6c75 6573 2068 6176 656e   If values haven
-000034e0: 2774 2062 6565 6e20 7375 7070 6c69 6564  't been supplied
-000034f0: 2c20 6173 7375 6d65 207a 6572 6f0a 2020  , assume zero.  
-00003500: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00003510: 2020 2020 2020 2020 696e 6974 5f68 7076          init_hpv
-00003520: 5f70 7265 7620 3d20 7b27 6627 3a20 6e70  _prev = {'f': np
-00003530: 2e61 7272 6179 285b 305d 292c 2027 6d27  .array([0]), 'm'
-00003540: 3a20 6e70 2e61 7272 6179 285b 305d 297d  : np.array([0])}
-00003550: 0a20 2020 2020 2020 2020 2020 2061 6765  .            age
-00003560: 5f62 7261 636b 6574 7320 3d20 6e70 2e61  _brackets = np.a
-00003570: 7272 6179 285b 3135 305d 290a 0a20 2020  rray([150])..   
-00003580: 2020 2020 2072 6574 7572 6e20 696e 6974       return init
-00003590: 5f68 7076 5f70 7265 762c 2061 6765 5f62  _hpv_prev, age_b
-000035a0: 7261 636b 6574 730a 0a0a 2020 2020 6465  rackets...    de
-000035b0: 6620 696e 6974 5f67 656e 6f74 7970 6573  f init_genotypes
-000035c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000035d0: 2727 2720 496e 6974 6961 6c69 7a65 2074  ''' Initialize t
-000035e0: 6865 2067 656e 6f74 7970 6520 7061 7261  he genotype para
-000035f0: 6d65 7465 7273 2027 2727 0a20 2020 2020  meters '''.     
-00003600: 2020 2069 6620 7365 6c66 2e5f 6f72 6967     if self._orig
-00003610: 5f70 6172 7320 616e 6420 2767 656e 6f74  _pars and 'genot
-00003620: 7970 6573 2720 696e 2073 656c 662e 5f6f  ypes' in self._o
-00003630: 7269 675f 7061 7273 3a0a 2020 2020 2020  rig_pars:.      
-00003640: 2020 2020 2020 7365 6c66 5b27 6765 6e6f        self['geno
-00003650: 7479 7065 7327 5d20 3d20 7365 6c66 2e5f  types'] = self._
-00003660: 6f72 6967 5f70 6172 732e 706f 7028 2767  orig_pars.pop('g
-00003670: 656e 6f74 7970 6573 2729 2020 2320 5265  enotypes')  # Re
-00003680: 7374 6f72 650a 0a20 2020 2020 2020 2064  store..        d
-00003690: 6566 6175 6c74 5f67 7061 7273 2020 203d  efault_gpars   =
-000036a0: 2068 7070 6172 2e67 6574 5f67 656e 6f74   hppar.get_genot
-000036b0: 7970 655f 7061 7273 2829 0a20 2020 2020  ype_pars().     
-000036c0: 2020 2075 7365 725f 6770 6172 7320 2020     user_gpars   
-000036d0: 2020 203d 2073 632e 6463 7028 7365 6c66     = sc.dcp(self
-000036e0: 5b27 6765 6e6f 7479 7065 5f70 6172 7327  ['genotype_pars'
-000036f0: 5d29 0a20 2020 2020 2020 2073 656c 665b  ]).        self[
-00003700: 2767 656e 6f74 7970 655f 7061 7273 275d  'genotype_pars']
-00003710: 203d 2073 632e 6f62 6a64 6963 7428 290a   = sc.objdict().
-00003720: 0a20 2020 2020 2020 2023 2048 616e 646c  .        # Handl
-00003730: 6520 7370 6563 6961 6c20 696e 7075 7420  e special input 
-00003740: 6361 7365 730a 2020 2020 2020 2020 6966  cases.        if
-00003750: 2073 656c 665b 2767 656e 6f74 7970 6573   self['genotypes
-00003760: 275d 203d 3d20 2761 6c6c 273a 0a20 2020  '] == 'all':.   
-00003770: 2020 2020 2020 2020 2073 656c 665b 2767           self['g
-00003780: 656e 6f74 7970 6573 275d 203d 2064 6566  enotypes'] = def
-00003790: 6175 6c74 5f67 7061 7273 2e6b 6579 7328  ault_gpars.keys(
-000037a0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-000037b0: 206c 656e 2873 656c 665b 2767 656e 6f74   len(self['genot
-000037c0: 7970 6573 275d 293a 0a20 2020 2020 2020  ypes']):.       
-000037d0: 2020 2020 2070 7269 6e74 2827 4e6f 2067       print('No g
-000037e0: 656e 6f74 7970 6573 2070 726f 7669 6465  enotypes provide
-000037f0: 642c 2077 696c 6c20 7369 6d75 6c61 7465  d, will simulate
-00003800: 2031 362c 2031 382c 2061 6e64 206f 7468   16, 18, and oth
-00003810: 6572 2048 5220 7479 7065 7320 6279 2064  er HR types by d
-00003820: 6566 6175 6c74 2729 0a20 2020 2020 2020  efault').       
-00003830: 2020 2020 2073 656c 665b 2767 656e 6f74       self['genot
-00003840: 7970 6573 275d 203d 205b 3136 2c31 382c  ypes'] = [16,18,
-00003850: 2768 7268 7076 275d 0a0a 2020 2020 2020  'hrhpv']..      
-00003860: 2020 2320 4c6f 6f70 206f 7665 7220 6765    # Loop over ge
-00003870: 6e6f 7479 7065 730a 2020 2020 2020 2020  notypes.        
-00003880: 666f 7220 692c 2067 2069 6e20 656e 756d  for i, g in enum
-00003890: 6572 6174 6528 7365 6c66 5b27 6765 6e6f  erate(self['geno
-000038a0: 7479 7065 7327 5d29 3a0a 0a20 2020 2020  types']):..     
-000038b0: 2020 2020 2020 2023 2053 7461 6e64 6172         # Standar
-000038c0: 6469 7a65 2066 6f72 6d61 7420 6f66 2067  dize format of g
-000038d0: 656e 6f74 7970 6520 696e 7075 7473 0a20  enotype inputs. 
-000038e0: 2020 2020 2020 2020 2020 2069 6620 7363             if sc
-000038f0: 2e69 736e 756d 6265 7228 6729 3a20 6720  .isnumber(g): g 
-00003900: 3d20 6627 6870 767b 677d 2720 2320 436f  = f'hpv{g}' # Co
-00003910: 6e76 6572 7420 652e 672e 2031 3620 746f  nvert e.g. 16 to
-00003920: 2068 7076 3136 0a20 2020 2020 2020 2020   hpv16.         
-00003930: 2020 2069 6620 7363 2e63 6865 636b 7479     if sc.checkty
-00003940: 7065 2867 2c73 7472 293a 0a20 2020 2020  pe(g,str):.     
-00003950: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00003960: 7420 6720 696e 2064 6566 6175 6c74 5f67  t g in default_g
-00003970: 7061 7273 2e6b 6579 7328 293a 0a20 2020  pars.keys():.   
-00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003990: 2065 7272 6f72 6d73 6720 3d20 6627 4765   errormsg = f'Ge
-000039a0: 6e6f 7479 7065 207b 697d 2028 7b67 7d29  notype {i} ({g})
-000039b0: 2069 7320 6e6f 7420 6f6e 6520 6f66 2074   is not one of t
-000039c0: 6865 2069 6e62 7569 6c74 206f 7074 696f  he inbuilt optio
-000039d0: 6e73 2e27 0a20 2020 2020 2020 2020 2020  ns.'.           
-000039e0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000039f0: 616c 7565 4572 726f 7228 6572 726f 726d  alueError(errorm
-00003a00: 7367 290a 2020 2020 2020 2020 2020 2020  sg).            
-00003a10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003a20: 2020 2020 2020 6572 726f 726d 7367 203d        errormsg =
-00003a30: 2066 2746 6f72 6d61 7420 7b74 7970 6528   f'Format {type(
-00003a40: 6729 7d20 6973 206e 6f74 2075 6e64 6572  g)} is not under
-00003a50: 7374 6f6f 642e 270a 2020 2020 2020 2020  stood.'.        
-00003a60: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00003a70: 6c75 6545 7272 6f72 2865 7272 6f72 6d73  lueError(errorms
-00003a80: 6729 0a0a 2020 2020 2020 2020 2020 2020  g)..            
-00003a90: 2320 4164 6420 746f 2067 656e 6f74 7970  # Add to genotyp
-00003aa0: 655f 7061 7220 6469 6374 0a20 2020 2020  e_par dict.     
-00003ab0: 2020 2020 2020 2073 656c 665b 2767 656e         self['gen
-00003ac0: 6f74 7970 655f 7061 7273 275d 5b67 5d20  otype_pars'][g] 
-00003ad0: 3d20 6465 6661 756c 745f 6770 6172 735b  = default_gpars[
-00003ae0: 675d 0a20 2020 2020 2020 2020 2020 2073  g].            s
-00003af0: 656c 665b 2767 656e 6f74 7970 655f 6d61  elf['genotype_ma
-00003b00: 7027 5d5b 695d 203d 2067 0a0a 2020 2020  p'][i] = g..    
-00003b10: 2020 2020 2320 4c6f 6f70 206f 7665 7220      # Loop over 
-00003b20: 7573 6572 2d73 7570 706c 6965 6420 6765  user-supplied ge
-00003b30: 6e6f 7479 7065 2070 6172 616d 6574 6572  notype parameter
-00003b40: 7320 7468 6174 2063 616e 206f 7665 7277  s that can overw
-00003b50: 7269 7465 2076 616c 7565 730a 2020 2020  rite values.    
-00003b60: 2020 2020 6966 206c 656e 2875 7365 725f      if len(user_
-00003b70: 6770 6172 7329 3a0a 2020 2020 2020 2020  gpars):.        
-00003b80: 2020 2020 666f 7220 672c 6770 6172 7320      for g,gpars 
-00003b90: 696e 2075 7365 725f 6770 6172 732e 6974  in user_gpars.it
-00003ba0: 656d 7328 293a 0a0a 2020 2020 2020 2020  ems():..        
-00003bb0: 2020 2020 2020 2020 2320 5374 616e 6461          # Standa
-00003bc0: 7264 697a 6520 666f 726d 6174 206f 6620  rdize format of 
-00003bd0: 6765 6e6f 7479 7065 2069 6e70 7574 730a  genotype inputs.
-00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bf0: 6966 2073 632e 6973 6e75 6d62 6572 2867  if sc.isnumber(g
-00003c00: 293a 2067 203d 2066 2768 7076 7b67 7d27  ): g = f'hpv{g}'
-00003c10: 2020 2320 436f 6e76 6572 7420 652e 672e    # Convert e.g.
-00003c20: 2031 3620 746f 2068 7076 3136 0a20 2020   16 to hpv16.   
-00003c30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003c40: 7363 2e63 6865 636b 7479 7065 2867 2c20  sc.checktype(g, 
-00003c50: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00003c60: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00003c70: 2067 2069 6e20 7365 6c66 5b27 6765 6e6f   g in self['geno
-00003c80: 7479 7065 5f70 6172 7327 5d2e 6b65 7973  type_pars'].keys
-00003c90: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00003ca0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00003cb0: 726d 7367 203d 2066 2750 6172 616d 6574  rmsg = f'Paramet
-00003cc0: 6572 7320 7072 6f76 6964 6564 2066 6f72  ers provided for
-00003cd0: 2067 656e 6f74 7970 6520 7b67 7d2c 2062   genotype {g}, b
-00003ce0: 7574 2069 7420 6973 206e 6f74 2069 6e20  ut it is not in 
-00003cf0: 7468 6520 7369 6d2e 270a 2020 2020 2020  the sim.'.      
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00003d20: 6f72 2865 7272 6f72 6d73 6729 0a20 2020  or(errormsg).   
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003d50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00003d60: 6f72 2067 7061 726e 616d 652c 6770 6172  or gparname,gpar
-00003d70: 7661 6c20 696e 2067 7061 7273 2e69 7465  val in gpars.ite
-00003d80: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2020 6966 2067 7061 726e 616d 6520 696e    if gparname in
-00003db0: 2073 656c 665b 2767 656e 6f74 7970 655f   self['genotype_
-00003dc0: 7061 7273 275d 5b67 5d2e 6b65 7973 2829  pars'][g].keys()
-00003dd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003df0: 2020 7072 696e 746d 7367 203d 2066 2252    printmsg = f"R
-00003e00: 6573 6574 7469 6e67 2070 6172 616d 6574  esetting paramet
-00003e10: 6572 2027 7b67 7061 726e 616d 657d 2720  er '{gparname}' 
-00003e20: 6672 6f6d 207b 7365 6c66 5b27 6765 6e6f  from {self['geno
-00003e30: 7479 7065 5f70 6172 7327 5d5b 675d 5b67  type_pars'][g][g
-00003e40: 7061 726e 616d 655d 7d20 746f 207b 6770  parname]} to {gp
-00003e50: 6172 7661 6c7d 2066 6f72 2067 656e 6f74  arval} for genot
-00003e60: 7970 6520 7b67 7d22 0a20 2020 2020 2020  ype {g}".       
-00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e80: 2020 2020 2020 2020 2073 632e 7072 696e           sc.prin
-00003e90: 7476 2870 7269 6e74 6d73 672c 2031 2c20  tv(printmsg, 1, 
-00003ea0: 7365 6c66 5b27 7665 7262 6f73 6527 5d29  self['verbose'])
-00003eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ed0: 2073 656c 665b 2767 656e 6f74 7970 655f   self['genotype_
-00003ee0: 7061 7273 275d 5b67 5d5b 6770 6172 6e61  pars'][g][gparna
-00003ef0: 6d65 5d20 3d20 6770 6172 7661 6c0a 2020  me] = gparval.  
-00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 0a20 2020 2020 2020 2064 6566 6175 6c74  .        default
+000008f0: 5f6c 6f63 6174 696f 6e20 3d20 7363 2e64  _location = sc.d
+00000900: 6370 2864 6566 6175 6c74 5f70 6172 735b  cp(default_pars[
+00000910: 276c 6f63 6174 696f 6e27 5d29 2023 2050  'location']) # P
+00000920: 756c 6c20 6f75 7420 7468 6520 6465 6661  ull out the defa
+00000930: 756c 7420 6c6f 6361 7469 6f6e 2068 6572  ult location her
+00000940: 650a 2020 2020 2020 2020 6465 6661 756c  e.        defaul
+00000950: 745f 7061 7273 5b27 6c6f 6361 7469 6f6e  t_pars['location
+00000960: 275d 203d 204e 6f6e 6520 2320 446f 6e27  '] = None # Don'
+00000970: 7420 6c6f 6164 2074 6865 2064 6566 6175  t load the defau
+00000980: 6c74 206c 6f63 6174 696f 6e20 6865 7265  lt location here
+00000990: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+000009a0: 2e5f 5f69 6e69 745f 5f28 6465 6661 756c  .__init__(defaul
+000009b0: 745f 7061 7273 2920 2320 496e 6974 6961  t_pars) # Initia
+000009c0: 6c69 7a65 2061 6e64 2073 6574 2074 6865  lize and set the
+000009d0: 2070 6172 616d 6574 6572 7320 6173 2061   parameters as a
+000009e0: 7474 7269 6275 7465 730a 0a20 2020 2020  ttributes..     
+000009f0: 2020 2023 204c 6f61 6420 6461 7461 2c20     # Load data, 
+00000a00: 696e 636c 7564 696e 6720 6461 7461 6669  including datafi
+00000a10: 6c65 2074 6861 7420 6172 6520 7573 6564  le that are used
+00000a20: 2074 6f20 6372 6561 7465 2061 6464 6974   to create addit
+00000a30: 696f 6e61 6c20 6f70 7469 6f6e 616c 2070  ional optional p
+00000a40: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00000a50: 2020 7365 6c66 2e6c 6f61 645f 6461 7461    self.load_data
+00000a60: 2864 6174 6166 696c 6529 2023 204c 6f61  (datafile) # Loa
+00000a70: 6420 7468 6520 6461 7461 2c20 6966 2070  d the data, if p
+00000a80: 726f 7669 6465 640a 0a20 2020 2020 2020  rovided..       
+00000a90: 2023 2055 7064 6174 6520 7061 7261 6d65   # Update parame
+00000aa0: 7465 7273 0a20 2020 2020 2020 2069 6620  ters.        if 
+00000ab0: 7061 7273 2069 7320 4e6f 6e65 3a0a 2020  pars is None:.  
+00000ac0: 2020 2020 2020 2020 2020 7061 7273 203d            pars =
+00000ad0: 2064 6963 7428 6c6f 6361 7469 6f6e 3d64   dict(location=d
+00000ae0: 6566 6175 6c74 5f6c 6f63 6174 696f 6e29  efault_location)
+00000af0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00000b00: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00000b10: 7420 7061 7273 2e67 6574 2827 6c6f 6361  t pars.get('loca
+00000b20: 7469 6f6e 2729 206f 7220 7061 7273 5b27  tion') or pars['
+00000b30: 6c6f 6361 7469 6f6e 275d 2069 7320 4e6f  location'] is No
+00000b40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00000b50: 2020 2020 7061 7273 5b27 6c6f 6361 7469      pars['locati
+00000b60: 6f6e 275d 203d 2064 6566 6175 6c74 5f6c  on'] = default_l
+00000b70: 6f63 6174 696f 6e0a 0a20 2020 2020 2020  ocation..       
+00000b80: 2073 656c 662e 7570 6461 7465 5f70 6172   self.update_par
+00000b90: 7328 7061 7273 2c20 2a2a 6b77 6172 6773  s(pars, **kwargs
+00000ba0: 2920 2020 2320 5570 6461 7465 2074 6865  )   # Update the
+00000bb0: 2070 6172 616d 6574 6572 730a 0a20 2020   parameters..   
+00000bc0: 2020 2020 2072 6574 7572 6e0a 0a0a 2020       return...  
+00000bd0: 2020 6465 6620 6c6f 6164 5f64 6174 6128    def load_data(
+00000be0: 7365 6c66 2c20 6461 7461 6669 6c65 3d4e  self, datafile=N
+00000bf0: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0a  one, **kwargs):.
+00000c00: 2020 2020 2020 2020 2727 2720 4c6f 6164          ''' Load
+00000c10: 2074 6865 2064 6174 6120 746f 2063 616c   the data to cal
+00000c20: 6962 7261 7465 2061 6761 696e 7374 2c20  ibrate against, 
+00000c30: 6966 2070 726f 7669 6465 6420 2727 270a  if provided '''.
+00000c40: 2020 2020 2020 2020 6966 2064 6174 6166          if dataf
+00000c50: 696c 6520 6973 206e 6f74 204e 6f6e 653a  ile is not None:
+00000c60: 2023 2049 6620 6120 6461 7461 2066 696c   # If a data fil
+00000c70: 6520 6973 2070 726f 7669 6465 642c 206c  e is provided, l
+00000c80: 6f61 6420 6974 0a20 2020 2020 2020 2020  oad it.         
+00000c90: 2020 2073 656c 662e 6461 7461 203d 2068     self.data = h
+00000ca0: 706d 2e6c 6f61 645f 6461 7461 2864 6174  pm.load_data(dat
+00000cb0: 6166 696c 653d 6461 7461 6669 6c65 2c20  afile=datafile, 
+00000cc0: 6368 6563 6b5f 6461 7465 3d54 7275 652c  check_date=True,
+00000cd0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+00000ce0: 2020 2072 6574 7572 6e0a 0a0a 2020 2020     return...    
+00000cf0: 6465 6620 696e 6974 6961 6c69 7a65 2873  def initialize(s
+00000d00: 656c 662c 2072 6573 6574 3d46 616c 7365  elf, reset=False
+00000d10: 2c20 696e 6974 5f73 7461 7465 733d 5472  , init_states=Tr
+00000d20: 7565 2c20 696e 6974 5f61 6e61 6c79 7a65  ue, init_analyze
+00000d30: 7273 3d54 7275 652c 202a 2a6b 7761 7267  rs=True, **kwarg
+00000d40: 7329 3a0a 2020 2020 2020 2020 2727 270a  s):.        '''.
+00000d50: 2020 2020 2020 2020 5065 7266 6f72 6d20          Perform 
+00000d60: 616c 6c20 696e 6974 6961 6c69 7a61 7469  all initializati
+00000d70: 6f6e 7320 6f6e 2074 6865 2073 696d 2e0a  ons on the sim..
+00000d80: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00000d90: 2020 2020 7365 6c66 2e74 203d 2030 2020      self.t = 0  
+00000da0: 2320 5468 6520 6375 7272 656e 7420 7469  # The current ti
+00000db0: 6d65 2069 6e64 6578 0a20 2020 2020 2020  me index.       
+00000dc0: 2073 656c 662e 7661 6c69 6461 7465 5f70   self.validate_p
+00000dd0: 6172 7328 2920 2320 456e 7375 7265 2070  ars() # Ensure p
+00000de0: 6172 616d 6574 6572 7320 6861 7665 2076  arameters have v
+00000df0: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
+00000e00: 2020 2020 6870 752e 7365 745f 7365 6564      hpu.set_seed
+00000e10: 2873 656c 665b 2772 616e 645f 7365 6564  (self['rand_seed
+00000e20: 275d 2920 2320 5265 7365 7420 7468 6520  ']) # Reset the 
+00000e30: 7261 6e64 6f6d 2073 6565 6420 6265 666f  random seed befo
+00000e40: 7265 2074 6865 2070 6f70 756c 6174 696f  re the populatio
+00000e50: 6e20 6973 2063 7265 6174 6564 0a20 2020  n is created.   
+00000e60: 2020 2020 2073 656c 662e 696e 6974 5f67       self.init_g
+00000e70: 656e 6f74 7970 6573 2829 2023 2049 6e69  enotypes() # Ini
+00000e80: 7469 616c 697a 6520 7468 6520 6765 6e6f  tialize the geno
+00000e90: 7479 7065 730a 2020 2020 2020 2020 7365  types.        se
+00000ea0: 6c66 2e69 6e69 745f 7265 7375 6c74 7328  lf.init_results(
+00000eb0: 2920 2320 4166 7465 7220 696e 6974 6961  ) # After initia
+00000ec0: 6c69 7a69 6e67 2074 6865 2067 656e 6f74  lizing the genot
+00000ed0: 7970 6573 2061 6e64 2070 656f 706c 652c  ypes and people,
+00000ee0: 2063 7265 6174 6520 7468 6520 7265 7375   create the resu
+00000ef0: 6c74 7320 7374 7275 6374 7572 650a 2020  lts structure.  
+00000f00: 2020 2020 2020 7365 6c66 2e69 6e69 745f        self.init_
+00000f10: 696e 7465 7276 656e 7469 6f6e 7328 2920  interventions() 
+00000f20: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
+00000f30: 6520 696e 7465 7276 656e 7469 6f6e 7320  e interventions 
+00000f40: 4245 464f 5245 2074 6865 2070 656f 706c  BEFORE the peopl
+00000f50: 652c 2062 6563 6175 7365 2074 6865 6e20  e, because then 
+00000f60: 7661 6363 696e 6174 696f 6e20 696e 7465  vaccination inte
+00000f70: 7276 656e 7469 6f6e 7320 6765 7420 636f  rventions get co
+00000f80: 756e 7465 6420 696e 2069 6d6d 756e 6974  unted in immunit
+00000f90: 7920 7374 7275 6374 7572 6573 0a20 2020  y structures.   
+00000fa0: 2020 2020 2073 656c 662e 696e 6974 5f69       self.init_i
+00000fb0: 6d6d 756e 6974 7928 2920 2320 496e 636c  mmunity() # Incl
+00000fc0: 7564 6573 2069 6d6d 756e 6974 7920 6d61  udes immunity ma
+00000fd0: 7472 6963 6573 2061 6e64 2063 756d 756c  trices and cumul
+00000fe0: 6174 6976 6520 6479 7370 6c61 7369 6120  ative dysplasia 
+00000ff0: 6172 7261 7973 0a20 2020 2020 2020 2073  arrays.        s
+00001000: 656c 662e 696e 6974 5f70 656f 706c 6528  elf.init_people(
+00001010: 7265 7365 743d 7265 7365 742c 2069 6e69  reset=reset, ini
+00001020: 745f 7374 6174 6573 3d69 6e69 745f 7374  t_states=init_st
+00001030: 6174 6573 2c20 2a2a 6b77 6172 6773 2920  ates, **kwargs) 
+00001040: 2320 4372 6561 7465 2061 6c6c 2074 6865  # Create all the
+00001050: 2070 656f 706c 6520 2874 6865 2068 6561   people (the hea
+00001060: 7669 6573 7420 7374 6570 290a 2020 2020  viest step).    
+00001070: 2020 2020 6966 2069 6e69 745f 616e 616c      if init_anal
+00001080: 797a 6572 733a 2073 656c 662e 696e 6974  yzers: self.init
+00001090: 5f61 6e61 6c79 7a65 7273 2829 2020 2320  _analyzers()  # 
+000010a0: 2e2e 2e61 6e64 2074 6865 2061 6e61 6c79  ...and the analy
+000010b0: 7a65 7273 2e2e 2e0a 2020 2020 2020 2020  zers....        
+000010c0: 6870 752e 7365 745f 7365 6564 2873 656c  hpu.set_seed(sel
+000010d0: 665b 2772 616e 645f 7365 6564 275d 2b31  f['rand_seed']+1
+000010e0: 2920 2023 2052 6573 6574 2074 6865 2072  )  # Reset the r
+000010f0: 616e 646f 6d20 7365 6564 2074 6f20 7468  andom seed to th
+00001100: 6520 6465 6661 756c 7420 7275 6e20 7365  e default run se
+00001110: 6564 2c20 736f 2074 6861 7420 6966 2074  ed, so that if t
+00001120: 6865 2073 696d 756c 6174 696f 6e20 6973  he simulation is
+00001130: 2072 756e 2077 6974 6820 7265 7365 745f   run with reset_
+00001140: 7365 6564 3d46 616c 7365 2072 6967 6874  seed=False right
+00001150: 2061 6674 6572 2069 6e69 7469 616c 697a   after initializ
+00001160: 6174 696f 6e2c 2069 7420 7769 6c6c 2073  ation, it will s
+00001170: 7469 6c6c 2070 726f 6475 6365 2074 6865  till produce the
+00001180: 2073 616d 6520 6f75 7470 7574 0a20 2020   same output.   
+00001190: 2020 2020 2073 656c 662e 696e 6974 6961       self.initia
+000011a0: 6c69 7a65 6420 2020 3d20 5472 7565 0a20  lized   = True. 
+000011b0: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
+000011c0: 6c65 7465 2020 2020 2020 3d20 4661 6c73  lete      = Fals
+000011d0: 650a 2020 2020 2020 2020 7365 6c66 2e72  e.        self.r
+000011e0: 6573 756c 7473 5f72 6561 6479 203d 2046  esults_ready = F
+000011f0: 616c 7365 0a0a 2020 2020 2020 2020 7265  alse..        re
+00001200: 7475 726e 2073 656c 660a 0a0a 2020 2020  turn self...    
+00001210: 6465 6620 6c61 7965 725f 6b65 7973 2873  def layer_keys(s
+00001220: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
+00001230: 270a 2020 2020 2020 2020 4174 7465 6d70  '.        Attemp
+00001240: 7420 746f 2072 6574 7269 6576 6520 7468  t to retrieve th
+00001250: 6520 6375 7272 656e 7420 6c61 7965 7220  e current layer 
+00001260: 6b65 7973 2e0a 2020 2020 2020 2020 2727  keys..        ''
+00001270: 270a 2020 2020 2020 2020 7472 793a 0a20  '.        try:. 
+00001280: 2020 2020 2020 2020 2020 206b 6579 7320             keys 
+00001290: 3d20 6c69 7374 2873 656c 665b 2761 6374  = list(self['act
+000012a0: 7327 5d2e 6b65 7973 2829 2920 2320 4765  s'].keys()) # Ge
+000012b0: 7420 6b65 7973 2066 726f 6d20 6163 7473  t keys from acts
+000012c0: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
+000012d0: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+000012e0: 7665 720a 2020 2020 2020 2020 2020 2020  ver.            
+000012f0: 6b65 7973 203d 205b 5d0a 2020 2020 2020  keys = [].      
+00001300: 2020 7265 7475 726e 206b 6579 730a 0a0a    return keys...
+00001310: 2020 2020 6465 6620 7265 7365 745f 6c61      def reset_la
+00001320: 7965 725f 7061 7273 2873 656c 662c 206c  yer_pars(self, l
+00001330: 6179 6572 5f6b 6579 733d 4e6f 6e65 2c20  ayer_keys=None, 
+00001340: 666f 7263 653d 4661 6c73 6529 3a0a 2020  force=False):.  
+00001350: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00001360: 2020 5265 7365 7420 7468 6520 7061 7261    Reset the para
+00001370: 6d65 7465 7273 2074 6f20 6d61 7463 6820  meters to match 
+00001380: 7468 6520 706f 7075 6c61 7469 6f6e 2e0a  the population..
+00001390: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+000013a0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+000013b0: 5f6b 6579 7320 286c 6973 7429 3a20 6f76  _keys (list): ov
+000013c0: 6572 7269 6465 2074 6865 2064 6566 6175  erride the defau
+000013d0: 6c74 206c 6179 6572 206b 6579 7320 2875  lt layer keys (u
+000013e0: 7365 2073 746f 7265 6420 6b65 7973 2062  se stored keys b
+000013f0: 7920 6465 6661 756c 7429 0a20 2020 2020  y default).     
+00001400: 2020 2020 2020 2066 6f72 6365 2028 626f         force (bo
+00001410: 6f6c 293a 2072 6573 6574 2074 6865 2070  ol): reset the p
+00001420: 6172 616d 6574 6572 7320 6576 656e 2069  arameters even i
+00001430: 6620 7468 6579 2061 6c72 6561 6479 2065  f they already e
+00001440: 7869 7374 0a20 2020 2020 2020 2027 2727  xist.        '''
+00001450: 0a20 2020 2020 2020 2069 6620 6c61 7965  .        if laye
+00001460: 725f 6b65 7973 2069 7320 4e6f 6e65 3a0a  r_keys is None:.
+00001470: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00001480: 656c 662e 7065 6f70 6c65 2069 7320 6e6f  elf.people is no
+00001490: 7420 4e6f 6e65 3a20 2320 4966 2070 656f  t None: # If peo
+000014a0: 706c 6520 6578 6973 740a 2020 2020 2020  ple exist.      
+000014b0: 2020 2020 2020 2020 2020 6c61 7965 725f            layer_
+000014c0: 6b65 7973 203d 2073 656c 662e 7065 6f70  keys = self.peop
+000014d0: 6c65 2e63 6f6e 7461 6374 732e 6b65 7973  le.contacts.keys
+000014e0: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
+000014f0: 6c69 6620 7365 6c66 2e70 6f70 6469 6374  lif self.popdict
+00001500: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00001510: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00001520: 7965 725f 6b65 7973 203d 2073 656c 662e  yer_keys = self.
+00001530: 706f 7064 6963 745b 276c 6179 6572 5f6b  popdict['layer_k
+00001540: 6579 7327 5d0a 2020 2020 2020 2020 6870  eys'].        hp
+00001550: 7061 722e 7265 7365 745f 6c61 7965 725f  par.reset_layer_
+00001560: 7061 7273 2873 656c 662e 7061 7273 2c20  pars(self.pars, 
+00001570: 6c61 7965 725f 6b65 7973 3d6c 6179 6572  layer_keys=layer
+00001580: 5f6b 6579 732c 2066 6f72 6365 3d66 6f72  _keys, force=for
+00001590: 6365 290a 2020 2020 2020 2020 7265 7475  ce).        retu
+000015a0: 726e 0a0a 0a20 2020 2064 6566 2076 616c  rn...    def val
+000015b0: 6964 6174 655f 6c61 7965 725f 7061 7273  idate_layer_pars
+000015c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000015d0: 2727 270a 2020 2020 2020 2020 4861 6e64  '''.        Hand
+000015e0: 6c65 206c 6179 6572 2070 6172 616d 6574  le layer paramet
+000015f0: 6572 732c 2073 696e 6365 2074 6865 7920  ers, since they 
+00001600: 6e65 6564 2074 6f20 6265 2076 616c 6964  need to be valid
+00001610: 6174 6564 2061 6674 6572 2074 6865 2070  ated after the p
+00001620: 6f70 756c 6174 696f 6e0a 2020 2020 2020  opulation.      
+00001630: 2020 6372 6561 7469 6f6e 2c20 7261 7468    creation, rath
+00001640: 6572 2074 6861 6e20 6265 666f 7265 2e0a  er than before..
+00001650: 2020 2020 2020 2020 2727 270a 0a20 2020          '''..   
+00001660: 2020 2020 2023 2046 6972 7374 2c20 7472       # First, tr
+00001670: 7920 746f 2066 6967 7572 6520 6f75 7420  y to figure out 
+00001680: 7768 6174 2074 6865 206c 6179 6572 206b  what the layer k
+00001690: 6579 7320 7368 6f75 6c64 2062 6520 616e  eys should be an
+000016a0: 6420 7065 7266 6f72 6d20 6261 7369 6320  d perform basic 
+000016b0: 7479 7065 2063 6865 636b 696e 670a 2020  type checking.  
+000016c0: 2020 2020 2020 6c61 7965 725f 6b65 7973        layer_keys
+000016d0: 203d 2073 656c 662e 6c61 7965 725f 6b65   = self.layer_ke
+000016e0: 7973 2829 0a20 2020 2020 2020 206c 6179  ys().        lay
+000016f0: 6572 5f70 6172 7320 3d20 6870 7061 722e  er_pars = hppar.
+00001700: 6c61 7965 725f 7061 7273 2023 2054 6865  layer_pars # The
+00001710: 206e 616d 6573 206f 6620 7468 6520 7061   names of the pa
+00001720: 7261 6d65 7465 7273 2074 6861 7420 6172  rameters that ar
+00001730: 6520 7370 6563 6966 6965 6420 6279 206c  e specified by l
+00001740: 6179 6572 0a20 2020 2020 2020 2066 6f72  ayer.        for
+00001750: 206c 7020 696e 206c 6179 6572 5f70 6172   lp in layer_par
+00001760: 733a 0a20 2020 2020 2020 2020 2020 2076  s:.            v
+00001770: 616c 203d 2073 656c 665b 6c70 5d0a 2020  al = self[lp].  
+00001780: 2020 2020 2020 2020 2020 6966 2073 632e            if sc.
+00001790: 6973 6e75 6d62 6572 2876 616c 293a 2023  isnumber(val): #
+000017a0: 2049 7427 7320 6120 7363 616c 6172 2069   It's a scalar i
+000017b0: 6e73 7465 6164 206f 6620 6120 6469 6374  nstead of a dict
+000017c0: 2c20 6173 7375 6d65 2069 7427 7320 616c  , assume it's al
+000017d0: 6c20 636f 6e74 6163 7473 0a20 2020 2020  l contacts.     
+000017e0: 2020 2020 2020 2020 2020 2073 656c 665b             self[
+000017f0: 6c70 5d20 3d20 7b6b 3a76 616c 2066 6f72  lp] = {k:val for
+00001800: 206b 2069 6e20 6c61 7965 725f 6b65 7973   k in layer_keys
+00001810: 7d0a 0a20 2020 2020 2020 2023 2048 616e  }..        # Han
+00001820: 646c 6520 6b65 7920 6d69 736d 6174 6368  dle key mismatch
+00001830: 6573 0a20 2020 2020 2020 2066 6f72 206c  es.        for l
+00001840: 7020 696e 206c 6179 6572 5f70 6172 733a  p in layer_pars:
+00001850: 0a20 2020 2020 2020 2020 2020 206c 705f  .            lp_
+00001860: 6b65 7973 203d 2073 6574 2873 656c 662e  keys = set(self.
+00001870: 7061 7273 5b6c 705d 2e6b 6579 7328 2929  pars[lp].keys())
+00001880: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001890: 6c70 2021 3d20 276c 6179 6572 5f70 726f  lp != 'layer_pro
+000018a0: 6273 273a 0a20 2020 2020 2020 2020 2020  bs':.           
+000018b0: 2020 2020 2069 6620 6e6f 7420 6c70 5f6b       if not lp_k
+000018c0: 6579 7320 3d3d 2073 6574 286c 6179 6572  eys == set(layer
+000018d0: 5f6b 6579 7329 3a0a 2020 2020 2020 2020  _keys):.        
+000018e0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+000018f0: 726d 7367 203d 2027 4174 206c 6561 7374  rmsg = 'At least
+00001900: 206f 6e65 206c 6179 6572 2070 6172 616d   one layer param
+00001910: 6574 6572 2069 7320 696e 636f 6e73 6973  eter is inconsis
+00001920: 7465 6e74 2077 6974 6820 7468 6520 6c61  tent with the la
+00001930: 7965 7220 6b65 7973 3b20 616c 6c20 7061  yer keys; all pa
+00001940: 7261 6d65 7465 7273 206d 7573 7420 6861  rameters must ha
+00001950: 7665 2074 6865 2073 616d 6520 6b65 7973  ve the same keys
+00001960: 3a27 0a20 2020 2020 2020 2020 2020 2020  :'.             
+00001970: 2020 2020 2020 2065 7272 6f72 6d73 6720         errormsg 
+00001980: 2b3d 2066 275c 6e73 696d 2e6c 6179 6572  += f'\nsim.layer
+00001990: 5f6b 6579 7328 2920 3d20 7b6c 6179 6572  _keys() = {layer
+000019a0: 5f6b 6579 737d 270a 2020 2020 2020 2020  _keys}'.        
+000019b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000019c0: 6c70 3220 696e 206c 6179 6572 5f70 6172  lp2 in layer_par
+000019d0: 733a 2023 2046 6169 6c20 6f6e 2066 6972  s: # Fail on fir
+000019e0: 7374 2065 7272 6f72 2c20 6275 7420 7265  st error, but re
+000019f0: 2d6c 6f6f 7020 746f 206c 6973 7420 616c  -loop to list al
+00001a00: 6c20 6f66 2074 6865 6d0a 2020 2020 2020  l of them.      
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 6572 726f 726d 7367 202b 3d20 6627    errormsg += f'
+00001a30: 5c6e 7b6c 7032 7d20 3d20 2720 2b20 272c  \n{lp2} = ' + ',
+00001a40: 2027 2e6a 6f69 6e28 7365 6c66 2e70 6172   '.join(self.par
+00001a50: 735b 6c70 325d 2e6b 6579 7328 2929 0a20  s[lp2].keys()). 
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2072 6169 7365 2073 632e 4b65 794e     raise sc.KeyN
+00001a80: 6f74 466f 756e 6445 7272 6f72 2865 7272  otFoundError(err
+00001a90: 6f72 6d73 6729 0a0a 2020 2020 2020 2020  ormsg)..        
+00001aa0: 2020 2020 2320 544f 444f 3a20 6164 6420      # TODO: add 
+00001ab0: 7661 6c69 6461 7469 6f6e 2068 6572 6520  validation here 
+00001ac0: 666f 7220 6c61 7965 725f 7072 6f62 730a  for layer_probs.
+00001ad0: 0a20 2020 2020 2020 2023 2048 616e 646c  .        # Handl
+00001ae0: 6520 6d69 736d 6174 6368 6573 2077 6974  e mismatches wit
+00001af0: 6820 7468 6520 706f 7075 6c61 7469 6f6e  h the population
+00001b00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00001b10: 2e70 656f 706c 6520 6973 206e 6f74 204e  .people is not N
+00001b20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00001b30: 2070 6f70 5f6b 6579 7320 3d20 7365 7428   pop_keys = set(
+00001b40: 7365 6c66 2e70 656f 706c 652e 636f 6e74  self.people.cont
+00001b50: 6163 7473 2e6b 6579 7328 2929 0a20 2020  acts.keys()).   
+00001b60: 2020 2020 2020 2020 2069 6620 706f 705f           if pop_
+00001b70: 6b65 7973 2021 3d20 7365 7428 6c61 7965  keys != set(laye
+00001b80: 725f 6b65 7973 293a 2023 2070 7261 676d  r_keys): # pragm
+00001b90: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+00001ba0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00001bb0: 6f74 206c 656e 2870 6f70 5f6b 6579 7329  ot len(pop_keys)
+00001bc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001bd0: 2020 2020 2020 6572 726f 726d 7367 203d        errormsg =
+00001be0: 2066 2759 6f75 7220 706f 7075 6c61 7469   f'Your populati
+00001bf0: 6f6e 2064 6f65 7320 6e6f 7420 6861 7665  on does not have
+00001c00: 2061 6e79 206c 6179 6572 206b 6579 732c   any layer keys,
+00001c10: 2062 7574 2079 6f75 7220 7369 6d75 6c61   but your simula
+00001c20: 7469 6f6e 2064 6f65 7320 7b6c 6179 6572  tion does {layer
+00001c30: 5f6b 6579 737d 2e20 4966 2079 6f75 2063  _keys}. If you c
+00001c40: 616c 6c65 6420 6870 762e 5065 6f70 6c65  alled hpv.People
+00001c50: 2829 2064 6972 6563 746c 792c 2079 6f75  () directly, you
+00001c60: 2070 726f 6261 626c 7920 6e65 6564 2068   probably need h
+00001c70: 7076 2e6d 616b 655f 7065 6f70 6c65 2829  pv.make_people()
+00001c80: 2069 6e73 7465 6164 2e27 0a20 2020 2020   instead.'.     
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001ca0: 6169 7365 2073 632e 4b65 794e 6f74 466f  aise sc.KeyNotFo
+00001cb0: 756e 6445 7272 6f72 2865 7272 6f72 6d73  undError(errorms
+00001cc0: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00001cd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00001ce0: 2020 2020 2020 2020 2020 2020 2065 7272               err
+00001cf0: 6f72 6d73 6720 3d20 6627 506c 6561 7365  ormsg = f'Please
+00001d00: 2075 7064 6174 6520 796f 7572 2070 6172   update your par
+00001d10: 616d 6574 6572 206b 6579 7320 7b6c 6179  ameter keys {lay
+00001d20: 6572 5f6b 6579 737d 2074 6f20 6d61 7463  er_keys} to matc
+00001d30: 6820 706f 7075 6c61 7469 6f6e 206b 6579  h population key
+00001d40: 7320 7b70 6f70 5f6b 6579 737d 2e20 596f  s {pop_keys}. Yo
+00001d50: 7520 6d61 7920 6669 6e64 2073 696d 2e72  u may find sim.r
+00001d60: 6573 6574 5f6c 6179 6572 5f70 6172 7328  eset_layer_pars(
+00001d70: 2920 6865 6c70 6675 6c2e 270a 2020 2020  ) helpful.'.    
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 7261 6973 6520 7363 2e4b 6579 4e6f 7446  raise sc.KeyNotF
+00001da0: 6f75 6e64 4572 726f 7228 6572 726f 726d  oundError(errorm
+00001db0: 7367 290a 0a20 2020 2020 2020 2072 6574  sg)..        ret
+00001dc0: 7572 6e0a 0a0a 2020 2020 6465 6620 7661  urn...    def va
+00001dd0: 6c69 6461 7465 5f70 6172 7328 7365 6c66  lidate_pars(self
+00001de0: 2c20 7661 6c69 6461 7465 5f6c 6179 6572  , validate_layer
+00001df0: 733d 5472 7565 293a 0a20 2020 2020 2020  s=True):.       
+00001e00: 2027 2727 0a20 2020 2020 2020 2053 6f6d   '''.        Som
+00001e10: 6520 7061 7261 6d65 7465 7273 2063 616e  e parameters can
+00001e20: 2074 616b 6520 6d75 6c74 6970 6c65 2074   take multiple t
+00001e30: 7970 6573 3b20 7468 6973 206d 616b 6573  ypes; this makes
+00001e40: 2074 6865 6d20 636f 6e73 6973 7465 6e74   them consistent
+00001e50: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00001e60: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00001e70: 6964 6174 655f 6c61 7965 7273 2028 626f  idate_layers (bo
+00001e80: 6f6c 293a 2077 6865 7468 6572 2074 6f20  ol): whether to 
+00001e90: 7661 6c69 6461 7465 206c 6179 6572 2070  validate layer p
+00001ea0: 6172 616d 6574 6572 7320 6173 2077 656c  arameters as wel
+00001eb0: 6c20 7669 6120 7661 6c69 6461 7465 5f6c  l via validate_l
+00001ec0: 6179 6572 5f70 6172 7328 2920 2d2d 2075  ayer_pars() -- u
+00001ed0: 7375 616c 6c79 2079 6573 2c20 6578 6365  sually yes, exce
+00001ee0: 7074 2064 7572 696e 6720 696e 6974 6961  pt during initia
+00001ef0: 6c69 7a61 7469 6f6e 0a20 2020 2020 2020  lization.       
+00001f00: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
+00001f10: 4861 6e64 6c65 2074 7970 6573 0a20 2020  Handle types.   
+00001f20: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
+00001f30: 5b27 6e5f 6167 656e 7473 275d 3a0a 2020  ['n_agents']:.  
+00001f40: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001f60: 656c 665b 6b65 795d 203d 2069 6e74 2873  elf[key] = int(s
+00001f70: 656c 665b 6b65 795d 290a 2020 2020 2020  elf[key]).      
+00001f80: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00001f90: 6570 7469 6f6e 2061 7320 453a 0a20 2020  eption as E:.   
+00001fa0: 2020 2020 2020 2020 2020 2020 2065 7272               err
+00001fb0: 6f72 6d73 6720 3d20 6627 436f 756c 6420  ormsg = f'Could 
+00001fc0: 6e6f 7420 636f 6e76 6572 7420 7b6b 6579  not convert {key
+00001fd0: 7d3d 7b73 656c 665b 6b65 795d 7d20 6f66  }={self[key]} of
+00001fe0: 207b 7479 7065 2873 656c 665b 6b65 795d   {type(self[key]
+00001ff0: 297d 2074 6f20 696e 7465 6765 7227 0a20  )} to integer'. 
+00002000: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002010: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00002020: 6572 726f 726d 7367 2920 6672 6f6d 2045  errormsg) from E
+00002030: 0a0a 2020 2020 2020 2020 2320 4861 6e64  ..        # Hand
+00002040: 6c65 2073 7461 7274 0a20 2020 2020 2020  le start.       
+00002050: 2069 6620 7365 6c66 5b27 7374 6172 7427   if self['start'
+00002060: 5d20 696e 205b 4e6f 6e65 2c20 305d 3a20  ] in [None, 0]: 
+00002070: 2320 5573 6520 6465 6661 756c 7420 7374  # Use default st
+00002080: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
+00002090: 7365 6c66 5b27 7374 6172 7427 5d20 3d20  self['start'] = 
+000020a0: 3230 3135 0a0a 2020 2020 2020 2020 2320  2015..        # 
+000020b0: 4861 6e64 6c65 2065 6e64 2061 6e64 206e  Handle end and n
+000020c0: 5f79 6561 7273 0a20 2020 2020 2020 2069  _years.        i
+000020d0: 6620 7365 6c66 5b27 656e 6427 5d3a 0a20  f self['end']:. 
+000020e0: 2020 2020 2020 2020 2020 2073 656c 665b             self[
+000020f0: 276e 5f79 6561 7273 275d 203d 2069 6e74  'n_years'] = int
+00002100: 2873 656c 665b 2765 6e64 275d 202d 2073  (self['end'] - s
+00002110: 656c 665b 2773 7461 7274 275d 290a 2020  elf['start']).  
+00002120: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00002130: 665b 276e 5f79 6561 7273 275d 203c 3d20  f['n_years'] <= 
+00002140: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00002150: 2020 2065 7272 6f72 6d73 6720 3d20 6622     errormsg = f"
+00002160: 4e75 6d62 6572 206f 6620 7965 6172 7320  Number of years 
+00002170: 6d75 7374 2062 6520 3e30 2c20 6275 7420  must be >0, but 
+00002180: 796f 7520 7375 7070 6c69 6564 2073 7461  you supplied sta
+00002190: 7274 3d7b 7374 7228 7365 6c66 5b27 7374  rt={str(self['st
+000021a0: 6172 7427 5d29 7d20 616e 6420 656e 643d  art'])} and end=
+000021b0: 7b73 7472 2873 656c 665b 2765 6e64 275d  {str(self['end']
+000021c0: 297d 2c20 7768 6963 6820 6769 7665 7320  )}, which gives 
+000021d0: 6e5f 7965 6172 733d 7b73 656c 665b 276e  n_years={self['n
+000021e0: 5f79 6561 7273 275d 7d22 0a20 2020 2020  _years']}".     
+000021f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002200: 2056 616c 7565 4572 726f 7228 6572 726f   ValueError(erro
+00002210: 726d 7367 290a 2020 2020 2020 2020 656c  rmsg).        el
+00002220: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00002230: 6966 2073 656c 665b 276e 5f79 6561 7273  if self['n_years
+00002240: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00002250: 2020 2020 7365 6c66 5b27 656e 6427 5d20      self['end'] 
+00002260: 3d20 7365 6c66 5b27 7374 6172 7427 5d20  = self['start'] 
+00002270: 2b20 7365 6c66 5b27 6e5f 7965 6172 7327  + self['n_years'
+00002280: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+00002290: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000022a0: 2020 2020 6572 726f 726d 7367 203d 2027      errormsg = '
+000022b0: 596f 7520 6d75 7374 2073 7570 706c 7920  You must supply 
+000022c0: 6f6e 6520 6f66 206e 5f79 6561 7273 2061  one of n_years a
+000022d0: 6e64 2065 6e64 2e22 270a 2020 2020 2020  nd end."'.      
+000022e0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000022f0: 5661 6c75 6545 7272 6f72 2865 7272 6f72  ValueError(error
+00002300: 6d73 6729 0a0a 2020 2020 2020 2020 2320  msg)..        # 
+00002310: 436f 6e73 7472 7563 7420 6f74 6865 7220  Construct other 
+00002320: 7468 696e 6773 2074 6861 7420 6b65 6570  things that keep
+00002330: 2074 7261 636b 206f 6620 7469 6d65 0a20   track of time. 
+00002340: 2020 2020 2020 2073 656c 662e 7965 6172         self.year
+00002350: 7320 2020 2020 203d 2073 632e 696e 636c  s      = sc.incl
+00002360: 7573 6976 6572 616e 6765 2873 656c 665b  usiverange(self[
+00002370: 2773 7461 7274 275d 2c73 656c 665b 2765  'start'],self['e
+00002380: 6e64 275d 290a 2020 2020 2020 2020 7365  nd']).        se
+00002390: 6c66 2e79 6561 7276 6563 2020 2020 3d20  lf.yearvec    = 
+000023a0: 7363 2e69 6e63 6c75 7369 7665 7261 6e67  sc.inclusiverang
+000023b0: 6528 7374 6172 743d 7365 6c66 5b27 7374  e(start=self['st
+000023c0: 6172 7427 5d2c 2073 746f 703d 7365 6c66  art'], stop=self
+000023d0: 5b27 656e 6427 5d2b 312d 7365 6c66 5b27  ['end']+1-self['
+000023e0: 6474 275d 2c20 7374 6570 3d73 656c 665b  dt'], step=self[
+000023f0: 2764 7427 5d29 2023 2049 6e63 6c75 6465  'dt']) # Include
+00002400: 7320 616c 6c20 7468 6520 7469 6d65 706f  s all the timepo
+00002410: 696e 7473 2069 6e20 7468 6520 6c61 7374  ints in the last
+00002420: 2079 6561 720a 2020 2020 2020 2020 7365   year.        se
+00002430: 6c66 2e6e 7074 7320 2020 2020 2020 3d20  lf.npts       = 
+00002440: 6c65 6e28 7365 6c66 2e79 6561 7276 6563  len(self.yearvec
+00002450: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00002460: 7665 6320 2020 2020 2020 3d20 6e70 2e61  vec       = np.a
+00002470: 7261 6e67 6528 7365 6c66 2e6e 7074 7329  range(self.npts)
+00002480: 0a0a 2020 2020 2020 2020 2320 4861 6e64  ..        # Hand
+00002490: 6c65 2070 6f70 756c 6174 696f 6e20 6e65  le population ne
+000024a0: 7477 6f72 6b20 6461 7461 0a20 2020 2020  twork data.     
+000024b0: 2020 206e 6574 776f 726b 5f63 686f 6963     network_choic
+000024c0: 6573 203d 205b 2772 616e 646f 6d27 2c20  es = ['random', 
+000024d0: 2764 6566 6175 6c74 275d 0a20 2020 2020  'default'].     
+000024e0: 2020 2063 686f 6963 6520 3d20 7365 6c66     choice = self
+000024f0: 5b27 6e65 7477 6f72 6b27 5d0a 2020 2020  ['network'].    
+00002500: 2020 2020 6966 2063 686f 6963 6520 616e      if choice an
+00002510: 6420 6368 6f69 6365 206e 6f74 2069 6e20  d choice not in 
+00002520: 6e65 7477 6f72 6b5f 6368 6f69 6365 733a  network_choices:
+00002530: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+00002540: 7665 720a 2020 2020 2020 2020 2020 2020  ver.            
+00002550: 6368 6f69 6365 7374 7220 3d20 272c 2027  choicestr = ', '
+00002560: 2e6a 6f69 6e28 6e65 7477 6f72 6b5f 6368  .join(network_ch
+00002570: 6f69 6365 7329 0a20 2020 2020 2020 2020  oices).         
+00002580: 2020 2065 7272 6f72 6d73 6720 3d20 6627     errormsg = f'
+00002590: 506f 7075 6c61 7469 6f6e 2074 7970 6520  Population type 
+000025a0: 227b 6368 6f69 6365 7d22 206e 6f74 2061  "{choice}" not a
+000025b0: 7661 696c 6162 6c65 3b20 6368 6f69 6365  vailable; choice
+000025c0: 7320 6172 653a 207b 6368 6f69 6365 7374  s are: {choicest
+000025d0: 727d 270a 2020 2020 2020 2020 2020 2020  r}'.            
+000025e0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000025f0: 2865 7272 6f72 6d73 6729 0a0a 2020 2020  (errormsg)..    
+00002600: 2020 2020 2320 4861 6e64 6c65 2061 6e61      # Handle ana
+00002610: 6c79 7a65 7273 2061 6e64 2069 6e74 6572  lyzers and inter
+00002620: 7665 6e74 696f 6e73 0a20 2020 2020 2020  ventions.       
+00002630: 2066 6f72 206b 6579 2069 6e20 5b27 696e   for key in ['in
+00002640: 7465 7276 656e 7469 6f6e 7327 2c20 2761  terventions', 'a
+00002650: 6e61 6c79 7a65 7273 275d 3a20 2320 456e  nalyzers']: # En
+00002660: 7375 7265 2061 6c6c 206f 6620 7468 656d  sure all of them
+00002670: 2061 7265 206c 6973 7473 0a20 2020 2020   are lists.     
+00002680: 2020 2020 2020 2073 656c 665b 6b65 795d         self[key]
+00002690: 203d 2073 632e 6463 7028 7363 2e74 6f6c   = sc.dcp(sc.tol
+000026a0: 6973 7428 7365 6c66 5b6b 6579 5d2c 206b  ist(self[key], k
+000026b0: 6565 706e 6f6e 653d 4661 6c73 6529 2920  eepnone=False)) 
+000026c0: 2320 416c 6c20 6f66 2074 6865 7365 2068  # All of these h
+000026d0: 6176 6520 696e 6974 6961 6c69 7a65 2066  ave initialize f
+000026e0: 756e 6374 696f 6e73 2074 6861 7420 7275  unctions that ru
+000026f0: 6e20 696e 746f 2069 7373 7565 7320 6966  n into issues if
+00002700: 2074 6865 7927 7265 2072 6575 7365 640a   they're reused.
+00002710: 2020 2020 2020 2020 666f 7220 692c 696e          for i,in
+00002720: 7465 7276 2069 6e20 656e 756d 6572 6174  terv in enumerat
+00002730: 6528 7365 6c66 5b27 696e 7465 7276 656e  e(self['interven
+00002740: 7469 6f6e 7327 5d29 3a0a 2020 2020 2020  tions']):.      
+00002750: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00002760: 6e63 6528 696e 7465 7276 2c20 6469 6374  nce(interv, dict
+00002770: 293a 2023 2049 7427 7320 6120 6469 6374  ): # It's a dict
+00002780: 696f 6e61 7279 2072 6570 7265 7365 6e74  ionary represent
+00002790: 6174 696f 6e20 6f66 2061 6e20 696e 7465  ation of an inte
+000027a0: 7276 656e 7469 6f6e 0a20 2020 2020 2020  rvention.       
+000027b0: 2020 2020 2020 2020 2073 656c 665b 2769           self['i
+000027c0: 6e74 6572 7665 6e74 696f 6e73 275d 5b69  nterventions'][i
+000027d0: 5d20 3d20 6870 692e 496e 7465 7276 656e  ] = hpi.Interven
+000027e0: 7469 6f6e 4469 6374 282a 2a69 6e74 6572  tionDict(**inter
+000027f0: 7629 0a0a 2020 2020 2020 2020 2320 4f70  v)..        # Op
+00002800: 7469 6f6e 616c 6c79 2068 616e 646c 6520  tionally handle 
+00002810: 6c61 7965 7220 7061 7261 6d65 7465 7273  layer parameters
+00002820: 0a20 2020 2020 2020 2069 6620 7661 6c69  .        if vali
+00002830: 6461 7465 5f6c 6179 6572 733a 0a20 2020  date_layers:.   
+00002840: 2020 2020 2020 2020 2073 656c 662e 7661           self.va
+00002850: 6c69 6461 7465 5f6c 6179 6572 5f70 6172  lidate_layer_par
+00002860: 7328 290a 0a20 2020 2020 2020 2023 2048  s()..        # H
+00002870: 616e 646c 6520 7665 7262 6f73 650a 2020  andle verbose.  
+00002880: 2020 2020 2020 6966 2073 656c 665b 2776        if self['v
+00002890: 6572 626f 7365 275d 203d 3d20 2762 7269  erbose'] == 'bri
+000028a0: 6566 273a 0a20 2020 2020 2020 2020 2020  ef':.           
+000028b0: 2073 656c 665b 2776 6572 626f 7365 275d   self['verbose']
+000028c0: 203d 202d 310a 2020 2020 2020 2020 6966   = -1.        if
+000028d0: 206e 6f74 2073 632e 6973 6e75 6d62 6572   not sc.isnumber
+000028e0: 2873 656c 665b 2776 6572 626f 7365 275d  (self['verbose']
+000028f0: 293a 2023 2070 7261 676d 613a 206e 6f20  ): # pragma: no 
+00002900: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+00002910: 2020 6572 726f 726d 7367 203d 2066 2756    errormsg = f'V
+00002920: 6572 626f 7365 2061 7267 756d 656e 7420  erbose argument 
+00002930: 7368 6f75 6c64 2062 6520 6569 7468 6572  should be either
+00002940: 2022 6272 6965 6622 2c20 2d31 2c20 6f72   "brief", -1, or
+00002950: 2061 2066 6c6f 6174 2c20 6e6f 7420 7b74   a float, not {t
+00002960: 7970 6528 7365 6c66 5b22 7665 7262 6f73  ype(self["verbos
+00002970: 6522 5d29 7d20 227b 7365 6c66 5b22 7665  e"])} "{self["ve
+00002980: 7262 6f73 6522 5d7d 2227 0a20 2020 2020  rbose"]}"'.     
+00002990: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000029a0: 7565 4572 726f 7228 6572 726f 726d 7367  ueError(errormsg
+000029b0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000029c0: 6e0a 0a0a 2020 2020 6465 6620 7661 6c69  n...    def vali
+000029d0: 6461 7465 5f69 6e69 745f 636f 6e64 6974  date_init_condit
+000029e0: 696f 6e73 2873 656c 662c 2069 6e69 745f  ions(self, init_
+000029f0: 6870 765f 7072 6576 293a 0a20 2020 2020  hpv_prev):.     
+00002a00: 2020 2027 2727 0a20 2020 2020 2020 2049     '''.        I
+00002a10: 6e69 7469 616c 2070 7265 7661 6c65 6e63  nitial prevalenc
+00002a20: 6520 7661 6c75 6573 2063 616e 2062 6520  e values can be 
+00002a30: 7375 7070 6c69 6564 2077 6974 6820 6469  supplied with di
+00002a40: 6666 6572 656e 7420 616d 6f75 6e74 7320  fferent amounts 
+00002a50: 6f66 2064 6574 6169 6c2e 0a20 2020 2020  of detail..     
+00002a60: 2020 2048 6572 6520 7765 2066 6c65 7368     Here we flesh
+00002a70: 206f 7574 2061 6e79 206d 6973 7369 6e67   out any missing
+00002a80: 2064 6574 6169 6c73 2073 6f20 7468 6174   details so that
+00002a90: 2074 6865 2069 6e69 7469 616c 2070 7265   the initial pre
+00002aa0: 7620 7661 6c75 6573 2061 7265 0a20 2020  v values are.   
+00002ab0: 2020 2020 2062 7920 6167 6520 616e 6420       by age and 
+00002ac0: 6765 6e6f 7479 7065 2e20 5765 2061 6c73  genotype. We als
+00002ad0: 6f20 6368 6563 6b20 7468 6520 7072 6576  o check the prev
+00002ae0: 616c 656e 6365 2076 616c 7565 7320 6172  alence values ar
+00002af0: 6520 6f6b 2e0a 2020 2020 2020 2020 2727  e ok..        ''
+00002b00: 270a 0a20 2020 2020 2020 2064 6566 2076  '..        def v
+00002b10: 616c 6964 6174 655f 6172 7261 7973 2876  alidate_arrays(v
+00002b20: 616c 732c 206e 5f61 6765 5f62 7261 636b  als, n_age_brack
+00002b30: 6574 733d 4e6f 6e65 293a 0a20 2020 2020  ets=None):.     
+00002b40: 2020 2020 2020 2027 2727 204c 6974 746c         ''' Littl
+00002b50: 6520 6865 6c70 6572 2066 756e 6374 696f  e helper functio
+00002b60: 6e20 746f 2063 6865 636b 2070 7265 7661  n to check preva
+00002b70: 6c65 6e63 6520 7661 6c75 6573 2027 2727  lence values '''
+00002b80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002b90: 6e5f 6167 655f 6272 6163 6b65 7473 2069  n_age_brackets i
+00002ba0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00002bb0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00002bc0: 656e 2876 616c 7329 2021 3d20 6e5f 6167  en(vals) != n_ag
+00002bd0: 655f 6272 6163 6b65 7473 3a0a 2020 2020  e_brackets:.    
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 6572 726f 726d 7367 203d 2066 2754 6865  errormsg = f'The
+00002c00: 2069 6e69 7469 616c 2070 7265 7661 6c65   initial prevale
+00002c10: 6e63 6520 7661 6c75 6573 206d 7573 7420  nce values must 
+00002c20: 6569 7468 6572 2062 6520 7468 6520 7361  either be the sa
+00002c30: 6d65 206c 656e 6774 6820 6173 2074 6865  me length as the
+00002c40: 2061 6765 2062 7261 636b 6574 733a 207b   age brackets: {
+00002c50: 6c65 6e28 7661 6c73 297d 2076 7320 7b6e  len(vals)} vs {n
+00002c60: 5f61 6765 5f62 7261 636b 6574 737d 2e27  _age_brackets}.'
+00002c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c80: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00002c90: 4572 726f 7228 6572 726f 726d 7367 290a  Error(errormsg).
+00002ca0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002cb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002cc0: 2020 6966 206c 656e 2876 616c 7329 2021    if len(vals) !
+00002cd0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00002ce0: 2020 2020 2020 2020 2065 7272 6f72 6d73           errorms
+00002cf0: 6720 3d20 6627 4e6f 2061 6765 2062 7261  g = f'No age bra
+00002d00: 636b 6574 7320 7765 7265 2073 7570 706c  ckets were suppl
+00002d10: 6965 642c 2062 7574 206d 6f72 6520 7468  ied, but more th
+00002d20: 616e 206f 6e65 2070 7265 7661 6c65 6e63  an one prevalenc
+00002d30: 6520 7661 6c75 6520 7761 7320 7375 7070  e value was supp
+00002d40: 6c69 6564 2028 7b6c 656e 2876 616c 7329  lied ({len(vals)
+00002d50: 7d29 2e20 416e 2061 7272 6179 206f 6620  }). An array of 
+00002d60: 7072 6576 616c 656e 6365 2076 616c 7565  prevalence value
+00002d70: 7320 6361 6e20 6f6e 6c79 2062 6520 7375  s can only be su
+00002d80: 7070 6c69 6564 2061 6c6f 6e67 2077 6974  pplied along wit
+00002d90: 6820 616e 2061 7272 6179 206f 6620 636f  h an array of co
+00002da0: 7272 6573 706f 6e64 696e 6720 6167 6520  rresponding age 
+00002db0: 6272 6163 6b65 7473 2e27 0a20 2020 2020  brackets.'.     
+00002dc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002dd0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00002de0: 6572 726f 726d 7367 290a 2020 2020 2020  errormsg).      
+00002df0: 2020 2020 2020 6966 2076 616c 732e 616e        if vals.an
+00002e00: 7928 2920 3c20 3020 6f72 2076 616c 732e  y() < 0 or vals.
+00002e10: 616e 7928 2920 3e20 313a 0a20 2020 2020  any() > 1:.     
+00002e20: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00002e30: 6d73 6720 3d20 6627 5468 6520 696e 6974  msg = f'The init
+00002e40: 6961 6c20 7072 6576 616c 656e 6365 2076  ial prevalence v
+00002e50: 616c 7565 7320 6d75 7374 2065 6974 6865  alues must eithe
+00002e60: 7220 6265 7477 6565 6e20 3020 616e 6420  r between 0 and 
+00002e70: 312c 206e 6f74 207b 7661 6c73 7d2e 270a  1, not {vals}.'.
+00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e90: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00002ea0: 2865 7272 6f72 6d73 6729 0a0a 2020 2020  (errormsg)..    
+00002eb0: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00002ec0: 2020 2020 2020 2020 2320 4966 2076 616c          # If val
+00002ed0: 7565 7320 6861 7665 2062 6565 6e20 7072  ues have been pr
+00002ee0: 6f76 6964 6564 2c20 7661 6c69 6461 7465  ovided, validate
+00002ef0: 2074 6865 6d0a 2020 2020 2020 2020 7365   them.        se
+00002f00: 785f 6b65 7973 203d 207b 276d 272c 2027  x_keys = {'m', '
+00002f10: 6627 7d0a 2020 2020 2020 2020 746f 745f  f'}.        tot_
+00002f20: 6b65 7973 203d 205b 2761 6c6c 272c 2027  keys = ['all', '
+00002f30: 746f 7461 6c27 2c20 2774 6f74 272c 2027  total', 'tot', '
+00002f40: 6176 6572 6167 6527 2c20 2761 7667 275d  average', 'avg']
+00002f50: 0a20 2020 2020 2020 206e 5f61 6765 5f62  .        n_age_b
+00002f60: 7261 636b 6574 7320 3d20 4e6f 6e65 0a0a  rackets = None..
+00002f70: 2020 2020 2020 2020 6966 2069 6e69 745f          if init_
+00002f80: 6870 765f 7072 6576 2069 7320 6e6f 7420  hpv_prev is not 
+00002f90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00002fa0: 2020 6966 2073 632e 6368 6563 6b74 7970    if sc.checktyp
+00002fb0: 6528 696e 6974 5f68 7076 5f70 7265 762c  e(init_hpv_prev,
+00002fc0: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00002fd0: 2020 2020 2020 2020 2320 4765 7420 6167          # Get ag
+00002fe0: 6520 6272 6163 6b65 7473 2069 6620 7375  e brackets if su
+00002ff0: 7070 6c69 6564 0a20 2020 2020 2020 2020  pplied.         
+00003000: 2020 2020 2020 2069 6620 2761 6765 5f62         if 'age_b
+00003010: 7261 636b 6574 7327 2069 6e20 696e 6974  rackets' in init
+00003020: 5f68 7076 5f70 7265 762e 6b65 7973 2829  _hpv_prev.keys()
+00003030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003040: 2020 2020 2020 6167 655f 6272 6163 6b65        age_bracke
+00003050: 7473 203d 2069 6e69 745f 6870 765f 7072  ts = init_hpv_pr
+00003060: 6576 2e70 6f70 2827 6167 655f 6272 6163  ev.pop('age_brac
+00003070: 6b65 7473 2729 0a20 2020 2020 2020 2020  kets').         
+00003080: 2020 2020 2020 2020 2020 206e 5f61 6765             n_age
+00003090: 5f62 7261 636b 6574 7320 3d20 6c65 6e28  _brackets = len(
+000030a0: 6167 655f 6272 6163 6b65 7473 290a 2020  age_brackets).  
+000030b0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000030c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000030d0: 2020 2020 2020 2020 6167 655f 6272 6163          age_brac
+000030e0: 6b65 7473 203d 206e 702e 6172 7261 7928  kets = np.array(
+000030f0: 5b31 3530 5d29 0a0a 2020 2020 2020 2020  [150])..        
+00003100: 2020 2020 2020 2020 2320 4861 6e64 6c65          # Handle
+00003110: 2074 6865 2072 6573 7420 6f66 2074 6865   the rest of the
+00003120: 206b 6579 730a 2020 2020 2020 2020 2020   keys.          
+00003130: 2020 2020 2020 7661 725f 6b65 7973 203d        var_keys =
+00003140: 206c 6973 7428 696e 6974 5f68 7076 5f70   list(init_hpv_p
+00003150: 7265 762e 6b65 7973 2829 290a 2020 2020  rev.keys()).    
+00003160: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00003170: 6c65 6e28 7661 725f 6b65 7973 293d 3d31  len(var_keys)==1
+00003180: 2061 6e64 2076 6172 5f6b 6579 735b 305d   and var_keys[0]
+00003190: 206e 6f74 2069 6e20 746f 745f 6b65 7973   not in tot_keys
+000031a0: 2920 6f72 2028 6c65 6e28 7661 725f 6b65  ) or (len(var_ke
+000031b0: 7973 293e 3120 616e 6420 7365 7428 7661  ys)>1 and set(va
+000031c0: 725f 6b65 7973 2920 213d 2073 6578 5f6b  r_keys) != sex_k
+000031d0: 6579 7329 3a0a 2020 2020 2020 2020 2020  eys):.          
+000031e0: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
+000031f0: 7367 203d 2066 2743 6f75 6c64 206e 6f74  sg = f'Could not
+00003200: 2075 6e64 6572 7374 616e 6420 7468 6520   understand the 
+00003210: 696e 6974 6961 6c20 7072 6576 616c 656e  initial prevalen
+00003220: 6365 2070 726f 7669 6465 643a 207b 696e  ce provided: {in
+00003230: 6974 5f68 7076 5f70 7265 767d 2e20 4966  it_hpv_prev}. If
+00003240: 2073 7570 706c 7969 6e67 2061 2064 6963   supplying a dic
+00003250: 7469 6f6e 6172 792c 2070 6c65 6173 6520  tionary, please 
+00003260: 7573 6520 226d 2220 616e 6420 2266 2220  use "m" and "f" 
+00003270: 6b65 7973 206f 7220 2274 6f74 222e 2027  keys or "tot". '
+00003280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003290: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000032a0: 4572 726f 7228 6572 726f 726d 7367 290a  Error(errormsg).
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032c0: 6966 206c 656e 2876 6172 5f6b 6579 7329  if len(var_keys)
+000032d0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+000032e0: 2020 2020 2020 2020 2020 206b 203d 2076             k = v
+000032f0: 6172 5f6b 6579 735b 305d 0a20 2020 2020  ar_keys[0].     
+00003300: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003310: 6e69 745f 6870 765f 7072 6576 203d 207b  nit_hpv_prev = {
+00003320: 736b 3a20 7363 2e70 726f 6d6f 7465 746f  sk: sc.promoteto
+00003330: 6172 7261 7928 696e 6974 5f68 7076 5f70  array(init_hpv_p
+00003340: 7265 765b 6b5d 2920 666f 7220 736b 2069  rev[k]) for sk i
+00003350: 6e20 7365 785f 6b65 7973 7d0a 0a20 2020  n sex_keys}..   
+00003360: 2020 2020 2020 2020 2020 2020 2023 204e               # N
+00003370: 6f77 2073 6574 2074 6865 2076 616c 7565  ow set the value
+00003380: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00003390: 2020 666f 7220 6b2c 2076 616c 7320 696e    for k, vals in
+000033a0: 2069 6e69 745f 6870 765f 7072 6576 2e69   init_hpv_prev.i
+000033b0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+000033c0: 2020 2020 2020 2020 2020 2020 696e 6974              init
+000033d0: 5f68 7076 5f70 7265 765b 6b5d 203d 2073  _hpv_prev[k] = s
+000033e0: 632e 7072 6f6d 6f74 6574 6f61 7272 6179  c.promotetoarray
+000033f0: 2876 616c 7329 0a0a 2020 2020 2020 2020  (vals)..        
+00003400: 2020 2020 656c 6966 2073 632e 6368 6563      elif sc.chec
+00003410: 6b74 7970 6528 696e 6974 5f68 7076 5f70  ktype(init_hpv_p
+00003420: 7265 762c 2027 6172 7261 796c 696b 6527  rev, 'arraylike'
+00003430: 2920 6f72 2073 632e 6973 6e75 6d62 6572  ) or sc.isnumber
+00003440: 2869 6e69 745f 6870 765f 7072 6576 293a  (init_hpv_prev):
+00003450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003460: 2023 2049 6620 6974 2773 2061 6e20 6172   # If it's an ar
+00003470: 7261 792c 2061 7373 756d 6520 7468 6573  ray, assume thes
+00003480: 6520 7661 6c75 6573 2061 7070 6c79 2074  e values apply t
+00003490: 6f20 6d61 6c65 7320 616e 6420 6665 6d61  o males and fema
+000034a0: 6c65 730a 2020 2020 2020 2020 2020 2020  les.            
+000034b0: 2020 2020 696e 6974 5f68 7076 5f70 7265      init_hpv_pre
+000034c0: 7620 3d20 7b73 6b3a 2073 632e 7072 6f6d  v = {sk: sc.prom
+000034d0: 6f74 6574 6f61 7272 6179 2869 6e69 745f  otetoarray(init_
+000034e0: 6870 765f 7072 6576 2920 666f 7220 736b  hpv_prev) for sk
+000034f0: 2069 6e20 7365 785f 6b65 7973 7d0a 2020   in sex_keys}.  
+00003500: 2020 2020 2020 2020 2020 2020 2020 6167                ag
+00003510: 655f 6272 6163 6b65 7473 203d 206e 702e  e_brackets = np.
+00003520: 6172 7261 7928 5b31 3530 5d29 0a0a 2020  array([150])..  
+00003530: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003550: 6572 726f 726d 7367 203d 2066 2749 6e69  errormsg = f'Ini
+00003560: 7469 616c 2070 7265 7661 6c65 6e63 6520  tial prevalence 
+00003570: 7661 6c75 6573 206f 6620 7479 7065 207b  values of type {
+00003580: 7479 7065 2869 6e69 745f 6870 765f 7072  type(init_hpv_pr
+00003590: 6576 297d 206e 6f74 2072 6563 6f67 6e69  ev)} not recogni
+000035a0: 7a65 642c 206d 7573 7420 6265 2061 2064  zed, must be a d
+000035b0: 6963 742c 2061 6e20 6172 7261 792c 206f  ict, an array, o
+000035c0: 7220 6120 666c 6f61 742e 270a 2020 2020  r a float.'.    
+000035d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000035e0: 6520 5661 6c75 6545 7272 6f72 2865 7272  e ValueError(err
+000035f0: 6f72 6d73 6729 0a0a 2020 2020 2020 2020  ormsg)..        
+00003600: 2020 2020 2320 4e6f 7720 7661 6c69 6461      # Now valida
+00003610: 7465 2074 6865 2061 7272 6179 730a 2020  te the arrays.  
+00003620: 2020 2020 2020 2020 2020 666f 7220 736b            for sk
+00003630: 2c20 7661 6c73 2069 6e20 696e 6974 5f68  , vals in init_h
+00003640: 7076 5f70 7265 762e 6974 656d 7328 293a  pv_prev.items():
+00003650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003660: 2076 616c 6964 6174 655f 6172 7261 7973   validate_arrays
+00003670: 2876 616c 732c 206e 5f61 6765 5f62 7261  (vals, n_age_bra
+00003680: 636b 6574 7329 0a0a 2020 2020 2020 2020  ckets)..        
+00003690: 2320 4966 2076 616c 7565 7320 6861 7665  # If values have
+000036a0: 6e27 7420 6265 656e 2073 7570 706c 6965  n't been supplie
+000036b0: 642c 2061 7373 756d 6520 7a65 726f 0a20  d, assume zero. 
+000036c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000036d0: 2020 2020 2020 2020 2069 6e69 745f 6870           init_hp
+000036e0: 765f 7072 6576 203d 207b 2766 273a 206e  v_prev = {'f': n
+000036f0: 702e 6172 7261 7928 5b30 5d29 2c20 276d  p.array([0]), 'm
+00003700: 273a 206e 702e 6172 7261 7928 5b30 5d29  ': np.array([0])
+00003710: 7d0a 2020 2020 2020 2020 2020 2020 6167  }.            ag
+00003720: 655f 6272 6163 6b65 7473 203d 206e 702e  e_brackets = np.
+00003730: 6172 7261 7928 5b31 3530 5d29 0a0a 2020  array([150])..  
+00003740: 2020 2020 2020 7265 7475 726e 2069 6e69        return ini
+00003750: 745f 6870 765f 7072 6576 2c20 6167 655f  t_hpv_prev, age_
+00003760: 6272 6163 6b65 7473 0a0a 0a20 2020 2064  brackets...    d
+00003770: 6566 2069 6e69 745f 6765 6e6f 7479 7065  ef init_genotype
+00003780: 7328 7365 6c66 2c20 7570 7065 725f 6479  s(self, upper_dy
+00003790: 7370 5f6c 696d 3d32 3030 293a 0a20 2020  sp_lim=200):.   
+000037a0: 2020 2020 2027 2727 2049 6e69 7469 616c       ''' Initial
+000037b0: 697a 6520 7468 6520 6765 6e6f 7479 7065  ize the genotype
+000037c0: 2070 6172 616d 6574 6572 7320 2727 270a   parameters '''.
+000037d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000037e0: 5f6f 7269 675f 7061 7273 2061 6e64 2027  _orig_pars and '
+000037f0: 6765 6e6f 7479 7065 7327 2069 6e20 7365  genotypes' in se
+00003800: 6c66 2e5f 6f72 6967 5f70 6172 733a 0a20  lf._orig_pars:. 
+00003810: 2020 2020 2020 2020 2020 2073 656c 665b             self[
+00003820: 2767 656e 6f74 7970 6573 275d 203d 2073  'genotypes'] = s
+00003830: 656c 662e 5f6f 7269 675f 7061 7273 2e70  elf._orig_pars.p
+00003840: 6f70 2827 6765 6e6f 7479 7065 7327 2920  op('genotypes') 
+00003850: 2023 2052 6573 746f 7265 0a0a 2020 2020   # Restore..    
+00003860: 2020 2020 6465 6661 756c 745f 6770 6172      default_gpar
+00003870: 7320 2020 3d20 6870 7061 722e 6765 745f  s   = hppar.get_
+00003880: 6765 6e6f 7479 7065 5f70 6172 7328 290a  genotype_pars().
+00003890: 2020 2020 2020 2020 7573 6572 5f67 7061          user_gpa
+000038a0: 7273 2020 2020 2020 3d20 7363 2e64 6370  rs      = sc.dcp
+000038b0: 2873 656c 665b 2767 656e 6f74 7970 655f  (self['genotype_
+000038c0: 7061 7273 275d 290a 2020 2020 2020 2020  pars']).        
+000038d0: 7365 6c66 5b27 6765 6e6f 7479 7065 5f70  self['genotype_p
+000038e0: 6172 7327 5d20 3d20 7363 2e6f 626a 6469  ars'] = sc.objdi
+000038f0: 6374 2829 0a0a 2020 2020 2020 2020 2320  ct()..        # 
+00003900: 4861 6e64 6c65 2073 7065 6369 616c 2069  Handle special i
+00003910: 6e70 7574 2063 6173 6573 0a20 2020 2020  nput cases.     
+00003920: 2020 2069 6620 7365 6c66 5b27 6765 6e6f     if self['geno
+00003930: 7479 7065 7327 5d20 3d3d 2027 616c 6c27  types'] == 'all'
+00003940: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00003950: 6c66 5b27 6765 6e6f 7479 7065 7327 5d20  lf['genotypes'] 
+00003960: 3d20 6465 6661 756c 745f 6770 6172 732e  = default_gpars.
+00003970: 6b65 7973 2829 0a20 2020 2020 2020 2069  keys().        i
+00003980: 6620 6e6f 7420 6c65 6e28 7365 6c66 5b27  f not len(self['
+00003990: 6765 6e6f 7479 7065 7327 5d29 3a0a 2020  genotypes']):.  
+000039a0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000039b0: 274e 6f20 6765 6e6f 7479 7065 7320 7072  'No genotypes pr
+000039c0: 6f76 6964 6564 3a20 7369 6d75 6c61 7469  ovided: simulati
+000039d0: 6e67 2031 362c 2031 382c 2061 6e64 2035  ng 16, 18, and 5
+000039e0: 206f 7468 6572 2070 6f6f 6c65 6420 4852   other pooled HR
+000039f0: 2074 7970 6573 2028 3331 2c20 3333 2c20   types (31, 33, 
+00003a00: 3435 2c20 3532 2c20 3538 292e 2729 0a20  45, 52, 58).'). 
+00003a10: 2020 2020 2020 2020 2020 2073 656c 665b             self[
+00003a20: 2767 656e 6f74 7970 6573 275d 203d 205b  'genotypes'] = [
+00003a30: 3136 2c31 382c 2768 6935 275d 0a0a 2020  16,18,'hi5']..  
+00003a40: 2020 2020 2020 2320 4c6f 6f70 206f 7665        # Loop ove
+00003a50: 7220 6765 6e6f 7479 7065 730a 2020 2020  r genotypes.    
+00003a60: 2020 2020 666f 7220 692c 2067 2069 6e20      for i, g in 
+00003a70: 656e 756d 6572 6174 6528 7365 6c66 5b27  enumerate(self['
+00003a80: 6765 6e6f 7479 7065 7327 5d29 3a0a 0a20  genotypes']):.. 
+00003a90: 2020 2020 2020 2020 2020 2023 2053 7461             # Sta
+00003aa0: 6e64 6172 6469 7a65 2066 6f72 6d61 7420  ndardize format 
+00003ab0: 6f66 2067 656e 6f74 7970 6520 696e 7075  of genotype inpu
+00003ac0: 7473 0a20 2020 2020 2020 2020 2020 2069  ts.            i
+00003ad0: 6620 7363 2e69 736e 756d 6265 7228 6729  f sc.isnumber(g)
+00003ae0: 3a20 6720 3d20 6627 6870 767b 677d 2720  : g = f'hpv{g}' 
+00003af0: 2320 436f 6e76 6572 7420 652e 672e 2031  # Convert e.g. 1
+00003b00: 3620 746f 2068 7076 3136 0a20 2020 2020  6 to hpv16.     
+00003b10: 2020 2020 2020 2069 6620 7363 2e63 6865         if sc.che
+00003b20: 636b 7479 7065 2867 2c73 7472 293a 0a20  cktype(g,str):. 
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003b40: 6620 6e6f 7420 6720 696e 2064 6566 6175  f not g in defau
+00003b50: 6c74 5f67 7061 7273 2e6b 6579 7328 293a  lt_gpars.keys():
+00003b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b70: 2020 2020 2065 7272 6f72 6d73 6720 3d20       errormsg = 
+00003b80: 6627 4765 6e6f 7479 7065 207b 697d 2028  f'Genotype {i} (
+00003b90: 7b67 7d29 2069 7320 6e6f 7420 6f6e 6520  {g}) is not one 
+00003ba0: 6f66 2074 6865 2069 6e62 7569 6c74 206f  of the inbuilt o
+00003bb0: 7074 696f 6e73 2e27 0a20 2020 2020 2020  ptions.'.       
+00003bc0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00003bd0: 7365 2056 616c 7565 4572 726f 7228 6572  se ValueError(er
+00003be0: 726f 726d 7367 290a 2020 2020 2020 2020  rormsg).        
+00003bf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00003c00: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
+00003c10: 7367 203d 2066 2746 6f72 6d61 7420 7b74  sg = f'Format {t
+00003c20: 7970 6528 6729 7d20 6973 206e 6f74 2075  ype(g)} is not u
+00003c30: 6e64 6572 7374 6f6f 642e 270a 2020 2020  nderstood.'.    
+00003c40: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00003c50: 6520 5661 6c75 6545 7272 6f72 2865 7272  e ValueError(err
+00003c60: 6f72 6d73 6729 0a0a 2020 2020 2020 2020  ormsg)..        
+00003c70: 2020 2020 2320 4164 6420 746f 2067 656e      # Add to gen
+00003c80: 6f74 7970 655f 7061 7220 6469 6374 0a20  otype_par dict. 
+00003c90: 2020 2020 2020 2020 2020 2073 656c 665b             self[
+00003ca0: 2767 656e 6f74 7970 655f 7061 7273 275d  'genotype_pars']
+00003cb0: 5b67 5d20 3d20 6465 6661 756c 745f 6770  [g] = default_gp
+00003cc0: 6172 735b 675d 0a20 2020 2020 2020 2020  ars[g].         
+00003cd0: 2020 2073 656c 665b 2767 656e 6f74 7970     self['genotyp
+00003ce0: 655f 6d61 7027 5d5b 695d 203d 2067 0a0a  e_map'][i] = g..
+00003cf0: 2020 2020 2020 2020 2320 4c6f 6f70 206f          # Loop o
+00003d00: 7665 7220 7573 6572 2d73 7570 706c 6965  ver user-supplie
+00003d10: 6420 6765 6e6f 7479 7065 2070 6172 616d  d genotype param
+00003d20: 6574 6572 7320 7468 6174 2063 616e 206f  eters that can o
+00003d30: 7665 7277 7269 7465 2076 616c 7565 730a  verwrite values.
+00003d40: 2020 2020 2020 2020 6966 206c 656e 2875          if len(u
+00003d50: 7365 725f 6770 6172 7329 3a0a 2020 2020  ser_gpars):.    
+00003d60: 2020 2020 2020 2020 666f 7220 672c 6770          for g,gp
+00003d70: 6172 7320 696e 2075 7365 725f 6770 6172  ars in user_gpar
+00003d80: 732e 6974 656d 7328 293a 0a0a 2020 2020  s.items():..    
+00003d90: 2020 2020 2020 2020 2020 2020 2320 5374              # St
+00003da0: 616e 6461 7264 697a 6520 666f 726d 6174  andardize format
+00003db0: 206f 6620 6765 6e6f 7479 7065 2069 6e70   of genotype inp
+00003dc0: 7574 730a 2020 2020 2020 2020 2020 2020  uts.            
+00003dd0: 2020 2020 6966 2073 632e 6973 6e75 6d62      if sc.isnumb
+00003de0: 6572 2867 293a 2067 203d 2066 2768 7076  er(g): g = f'hpv
+00003df0: 7b67 7d27 2020 2320 436f 6e76 6572 7420  {g}'  # Convert 
+00003e00: 652e 672e 2031 3620 746f 2068 7076 3136  e.g. 16 to hpv16
+00003e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e20: 2069 6620 7363 2e63 6865 636b 7479 7065   if sc.checktype
+00003e30: 2867 2c20 7374 7229 3a0a 2020 2020 2020  (g, str):.      
+00003e40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003e50: 206e 6f74 2067 2069 6e20 7365 6c66 5b27   not g in self['
+00003e60: 6765 6e6f 7479 7065 5f70 6172 7327 5d2e  genotype_pars'].
+00003e70: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
+00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e90: 6572 726f 726d 7367 203d 2066 2750 6172  errormsg = f'Par
+00003ea0: 616d 6574 6572 7320 7072 6f76 6964 6564  ameters provided
+00003eb0: 2066 6f72 2067 656e 6f74 7970 6520 7b67   for genotype {g
+00003ec0: 7d2c 2062 7574 2069 7420 6973 206e 6f74  }, but it is not
+00003ed0: 2069 6e20 7468 6520 7369 6d2e 270a 2020   in the sim.'.  
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ef0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00003f00: 6545 7272 6f72 2865 7272 6f72 6d73 6729  eError(errormsg)
+00003f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003f20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
 00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f40: 6572 726f 726d 7367 203d 2066 2250 6172  errormsg = f"Par
-00003f50: 616d 6574 6572 207b 6770 6172 6e61 6d65  ameter {gparname
-00003f60: 7d20 646f 6573 206e 6f74 2065 7869 7374  } does not exist
-00003f70: 2066 6f72 2067 656e 6f74 7970 6520 7b67   for genotype {g
-00003f80: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fa0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00003fb0: 726f 7228 6572 726f 726d 7367 290a 0a20  ror(errormsg).. 
-00003fc0: 2020 2020 2020 206c 656e 5f70 6172 7320         len_pars 
-00003fd0: 3d20 6c65 6e28 7365 6c66 5b27 6765 6e6f  = len(self['geno
-00003fe0: 7479 7065 5f70 6172 7327 5d29 0a20 2020  type_pars']).   
-00003ff0: 2020 2020 2073 656c 665b 276e 5f67 656e       self['n_gen
-00004000: 6f74 7970 6573 275d 203d 206c 656e 5f70  otypes'] = len_p
-00004010: 6172 7320 2023 2045 6163 6820 6765 6e6f  ars  # Each geno
-00004020: 7479 7065 2068 6173 2061 6e20 656e 7472  type has an entr
-00004030: 7920 696e 2067 656e 6f74 7970 655f 7061  y in genotype_pa
-00004040: 7273 0a0a 2020 2020 2020 2020 2320 5365  rs..        # Se
-00004050: 7420 7468 6520 6e75 6d62 6572 206f 6620  t the number of 
-00004060: 696d 6d75 6e69 7479 2073 6f75 7263 6573  immunity sources
-00004070: 0a20 2020 2020 2020 2073 656c 665b 276e  .        self['n
-00004080: 5f69 6d6d 5f73 6f75 7263 6573 275d 203d  _imm_sources'] =
-00004090: 206c 656e 2873 656c 665b 2767 656e 6f74   len(self['genot
-000040a0: 7970 6573 275d 290a 0a20 2020 2020 2020  ypes'])..       
-000040b0: 2072 6574 7572 6e0a 0a20 2020 2064 6566   return..    def
-000040c0: 2069 6e69 745f 696d 6d75 6e69 7479 2873   init_immunity(s
-000040d0: 656c 662c 2063 7265 6174 653d 5472 7565  elf, create=True
-000040e0: 293a 0a20 2020 2020 2020 2027 2727 2049  ):.        ''' I
-000040f0: 6e69 7469 616c 697a 6520 696d 6d75 6e69  nitialize immuni
-00004100: 7479 206d 6174 7269 6365 7320 2727 270a  ty matrices '''.
-00004110: 2020 2020 2020 2020 6870 696d 6d2e 696e          hpimm.in
-00004120: 6974 5f69 6d6d 756e 6974 7928 7365 6c66  it_immunity(self
-00004130: 2c20 6372 6561 7465 3d63 7265 6174 6529  , create=create)
-00004140: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
-00004150: 0a0a 2020 2020 6465 6620 696e 6974 5f72  ..    def init_r
-00004160: 6573 756c 7473 2873 656c 662c 2066 7265  esults(self, fre
-00004170: 7175 656e 6379 3d27 616e 6e75 616c 272c  quency='annual',
-00004180: 2061 6464 5f64 6174 613d 5472 7565 293a   add_data=True):
-00004190: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000041a0: 2020 2020 2043 7265 6174 6520 7468 6520       Create the 
-000041b0: 6d61 696e 2072 6573 756c 7473 2073 7472  main results str
-000041c0: 7563 7475 7265 2e0a 2020 2020 2020 2020  ucture..        
-000041d0: 5468 6520 7072 6566 6978 2022 6e22 2069  The prefix "n" i
-000041e0: 7320 7573 6564 2066 6f72 2073 746f 636b  s used for stock
-000041f0: 2076 6172 6961 626c 6573 2c20 692e 652e   variables, i.e.
-00004200: 2063 6f75 6e74 696e 6720 7468 6520 746f   counting the to
-00004210: 7461 6c20 6e75 6d62 6572 2069 6e20 616e  tal number in an
-00004220: 7920 6769 7665 6e20 7374 6174 6520 2873  y given state (s
-00004230: 7573 2f69 6e66 2f65 7463 2920 6f6e 2061  us/inf/etc) on a
-00004240: 6e79 2070 6172 7469 6375 6c61 7220 7469  ny particular ti
-00004250: 6d65 7374 6570 0a0a 2020 2020 2020 2020  mestep..        
-00004260: 4172 6775 6d65 6e74 733a 0a20 2020 2020  Arguments:.     
-00004270: 2020 2020 2020 2073 696d 2020 2020 2020         sim      
-00004280: 2020 2028 6870 762e 5369 6d29 2020 2020     (hpv.Sim)    
-00004290: 2020 203a 2061 2073 696d 0a20 2020 2020     : a sim.     
-000042a0: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-000042b0: 2020 2028 7374 7220 6f72 2066 6c6f 6174     (str or float
-000042c0: 2920 203a 2074 6865 2066 7265 7175 656e  )  : the frequen
-000042d0: 6379 2077 6974 6820 7768 6963 6820 746f  cy with which to
-000042e0: 2073 6176 6520 7265 7375 6c74 733a 2061   save results: a
-000042f0: 6363 6570 7473 2027 616e 6e75 616c 272c  ccepts 'annual',
-00004300: 2027 6474 272c 206f 7220 6120 666c 6f61   'dt', or a floa
-00004310: 7420 7768 6963 6820 6973 2069 6e74 6572  t which is inter
-00004320: 7072 6574 6564 2061 7320 6120 6672 6163  preted as a frac
-00004330: 7469 6f6e 206f 6620 6120 7965 6172 2c20  tion of a year, 
-00004340: 652e 672e 2030 2e32 2077 696c 6c20 7361  e.g. 0.2 will sa
-00004350: 7665 2072 6573 756c 7473 2065 7665 7279  ve results every
-00004360: 2030 2e32 2079 6561 7273 0a20 2020 2020   0.2 years.     
-00004370: 2020 2020 2020 2061 6464 5f64 6174 6120         add_data 
-00004380: 2020 2028 626f 6f6c 2920 2020 2020 2020     (bool)       
-00004390: 2020 203a 2077 6865 7468 6572 206f 7220     : whether or 
-000043a0: 6e6f 7420 746f 2061 6464 2064 6174 6120  not to add data 
-000043b0: 746f 2074 6865 2072 6573 756c 7420 7374  to the result st
-000043c0: 7275 6374 7572 6573 0a20 2020 2020 2020  ructures.       
-000043d0: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
-000043e0: 4861 6e64 6c65 2066 7265 7175 656e 6379  Handle frequency
-000043f0: 0a20 2020 2020 2020 2069 6620 7479 7065  .        if type
-00004400: 2866 7265 7175 656e 6379 2920 3d3d 2073  (frequency) == s
-00004410: 7472 3a0a 2020 2020 2020 2020 2020 2020  tr:.            
-00004420: 6966 2066 7265 7175 656e 6379 203d 3d20  if frequency == 
-00004430: 2761 6e6e 7561 6c27 3a0a 2020 2020 2020  'annual':.      
-00004440: 2020 2020 2020 2020 2020 7265 7366 7265            resfre
-00004450: 7120 3d20 696e 7428 3120 2f20 7365 6c66  q = int(1 / self
-00004460: 5b27 6474 275d 290a 2020 2020 2020 2020  ['dt']).        
-00004470: 2020 2020 656c 6966 2066 7265 7175 656e      elif frequen
-00004480: 6379 203d 3d20 2764 7427 3a0a 2020 2020  cy == 'dt':.    
-00004490: 2020 2020 2020 2020 2020 2020 7265 7366              resf
-000044a0: 7265 7120 3d20 310a 2020 2020 2020 2020  req = 1.        
-000044b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000044c0: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
-000044d0: 7367 203d 2066 2752 6573 756c 7420 6672  sg = f'Result fr
-000044e0: 6571 7565 6e63 7920 6e6f 7420 756e 6465  equency not unde
-000044f0: 7273 746f 6f64 3a20 6d75 7374 2062 6520  rstood: must be 
-00004500: 2261 6e6e 7561 6c22 2c20 2264 7422 206f  "annual", "dt" o
-00004510: 7220 6120 666c 6f61 742c 2062 7574 2079  r a float, but y
-00004520: 6f75 2070 726f 7669 6465 6420 7b66 7265  ou provided {fre
-00004530: 7175 656e 6379 7d2e 270a 2020 2020 2020  quency}.'.      
-00004540: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00004550: 5661 6c75 6545 7272 6f72 2865 7272 6f72  ValueError(error
-00004560: 6d73 6729 0a20 2020 2020 2020 2065 6c69  msg).        eli
-00004570: 6620 7479 7065 2866 7265 7175 656e 6379  f type(frequency
-00004580: 2920 3d3d 2066 6c6f 6174 3a0a 2020 2020  ) == float:.    
-00004590: 2020 2020 2020 2020 6966 2066 7265 7175          if frequ
-000045a0: 656e 6379 203c 2073 656c 665b 2764 7427  ency < self['dt'
-000045b0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-000045c0: 2020 2065 7272 6f72 6d73 6720 3d20 6627     errormsg = f'
-000045d0: 596f 7520 7265 7175 6573 7465 6420 7265  You requested re
-000045e0: 7375 6c74 7320 7769 7468 2066 7265 7175  sults with frequ
-000045f0: 656e 6379 207b 6672 6571 7565 6e63 797d  ency {frequency}
-00004600: 2c20 6275 7420 7468 6973 2069 7320 736d  , but this is sm
-00004610: 616c 6c65 7220 7468 616e 2074 6865 2073  aller than the s
-00004620: 696d 756c 6174 696f 6e20 7469 6d65 7374  imulation timest
-00004630: 6570 207b 7365 6c66 5b22 6474 225d 7d2e  ep {self["dt"]}.
-00004640: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00004650: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00004660: 6f72 2865 7272 6f72 6d73 6729 0a20 2020  or(errormsg).   
-00004670: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00004680: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004690: 6573 6672 6571 203d 2069 6e74 2866 7265  esfreq = int(fre
-000046a0: 7175 656e 6379 202f 2073 656c 665b 2764  quency / self['d
-000046b0: 7427 5d29 0a20 2020 2020 2020 2073 656c  t']).        sel
-000046c0: 662e 7265 7366 7265 7120 3d20 7265 7366  f.resfreq = resf
-000046d0: 7265 710a 2020 2020 2020 2020 6966 206e  req.        if n
-000046e0: 6f74 2073 656c 662e 7265 7366 7265 7120  ot self.resfreq 
-000046f0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-00004700: 2065 7272 6f72 6d73 6720 3d20 6627 5468   errormsg = f'Th
-00004710: 6520 7265 7375 6c74 7320 6672 6571 7565  e results freque
-00004720: 6e63 6520 7368 6f75 6c64 2062 6520 6120  nce should be a 
-00004730: 706f 7369 7469 7665 2069 6e74 6567 6572  positive integer
-00004740: 2c20 6e6f 7420 7b73 656c 662e 7265 7366  , not {self.resf
-00004750: 7265 717d 3a20 6474 206d 6179 2062 6520  req}: dt may be 
-00004760: 746f 6f20 6c61 7267 6527 0a20 2020 2020  too large'.     
-00004770: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00004780: 7565 4572 726f 7228 6572 726f 726d 7367  ueError(errormsg
-00004790: 290a 0a20 2020 2020 2020 2023 2043 6f6e  )..        # Con
-000047a0: 7374 7275 6374 2074 6865 2074 7665 6320  struct the tvec 
-000047b0: 7468 6174 2077 696c 6c20 6265 2075 7365  that will be use
-000047c0: 6420 7769 7468 2074 6865 2072 6573 756c  d with the resul
-000047d0: 7473 0a20 2020 2020 2020 2070 6f69 6e74  ts.        point
-000047e0: 735f 746f 5f75 7365 203d 206e 702e 6172  s_to_use = np.ar
-000047f0: 616e 6765 2830 2c20 7365 6c66 2e6e 7074  ange(0, self.npt
-00004800: 732c 2073 656c 662e 7265 7366 7265 7129  s, self.resfreq)
-00004810: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00004820: 735f 7965 6172 7665 6320 3d20 7365 6c66  s_yearvec = self
-00004830: 2e79 6561 7276 6563 5b70 6f69 6e74 735f  .yearvec[points_
-00004840: 746f 5f75 7365 5d0a 2020 2020 2020 2020  to_use].        
-00004850: 7365 6c66 2e72 6573 5f6e 7074 7320 3d20  self.res_npts = 
-00004860: 6c65 6e28 7365 6c66 2e72 6573 5f79 6561  len(self.res_yea
-00004870: 7276 6563 290a 2020 2020 2020 2020 7365  rvec).        se
-00004880: 6c66 2e72 6573 5f74 7665 6320 3d20 6e70  lf.res_tvec = np
-00004890: 2e61 7261 6e67 6528 7365 6c66 2e72 6573  .arange(self.res
-000048a0: 5f6e 7074 7329 0a0a 2020 2020 2020 2020  _npts)..        
-000048b0: 2320 4675 6e63 7469 6f6e 2074 6f20 6372  # Function to cr
-000048c0: 6561 7465 2072 6573 756c 7473 0a20 2020  eate results.   
-000048d0: 2020 2020 2064 6566 2069 6e69 745f 7265       def init_re
-000048e0: 7328 2a61 7267 732c 202a 2a6b 7761 7267  s(*args, **kwarg
-000048f0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00004900: 2727 2720 496e 6974 6961 6c69 7a65 2061  ''' Initialize a
-00004910: 2073 696e 676c 6520 7265 7375 6c74 206f   single result o
-00004920: 626a 6563 7420 2727 270a 2020 2020 2020  bject '''.      
-00004930: 2020 2020 2020 6f75 7470 7574 203d 2068        output = h
-00004940: 7062 2e52 6573 756c 7428 2a61 7267 732c  pb.Result(*args,
-00004950: 202a 2a6b 7761 7267 732c 206e 7074 733d   **kwargs, npts=
-00004960: 7365 6c66 2e72 6573 5f6e 7074 7329 0a20  self.res_npts). 
-00004970: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004980: 6e20 6f75 7470 7574 0a0a 2020 2020 2020  n output..      
-00004990: 2020 2320 496e 6974 6961 6c69 7a65 2073    # Initialize s
-000049a0: 746f 7261 6765 0a20 2020 2020 2020 2072  torage.        r
-000049b0: 6573 756c 7473 203d 2073 632e 6f62 6a64  esults = sc.objd
-000049c0: 6963 7428 290a 0a20 2020 2020 2020 206e  ict()..        n
-000049d0: 6720 3d20 7365 6c66 5b27 6e5f 6765 6e6f  g = self['n_geno
-000049e0: 7479 7065 7327 5d20 2320 4e75 6d62 6572  types'] # Number
-000049f0: 206f 6620 6765 6e6f 7479 7065 730a 2020   of genotypes.  
-00004a00: 2020 2020 2020 6e61 203d 206c 656e 2873        na = len(s
-00004a10: 656c 665b 2761 6765 5f62 696e 7327 5d29  elf['age_bins'])
-00004a20: 202d 2031 2023 204e 756d 6265 7220 6f66   - 1 # Number of
-00004a30: 2061 6765 2062 696e 730a 0a20 2020 2020   age bins..     
-00004a40: 2020 2023 2043 7265 6174 6520 666c 6f77     # Create flow
-00004a50: 730a 2020 2020 2020 2020 666f 7220 666c  s.        for fl
-00004a60: 6f77 2069 6e20 6870 642e 666c 6f77 733a  ow in hpd.flows:
-00004a70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00004a80: 756c 7473 5b66 6c6f 772e 6e61 6d65 5d20  ults[flow.name] 
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 203d 2069 6e69 745f 7265 7328 666c 6f77   = init_res(flow
-00004ab0: 2e6c 6162 656c 2c20 636f 6c6f 723d 666c  .label, color=fl
-00004ac0: 6f77 2e63 6f6c 6f72 290a 2020 2020 2020  ow.color).      
-00004ad0: 2020 2020 2020 7265 7375 6c74 735b 666c        results[fl
-00004ae0: 6f77 2e6e 616d 652b 275f 6279 5f67 656e  ow.name+'_by_gen
-00004af0: 6f74 7970 6527 5d20 2020 3d20 696e 6974  otype']   = init
-00004b00: 5f72 6573 2866 6c6f 772e 6c61 6265 6c2b  _res(flow.label+
-00004b10: 2720 6279 2067 656e 6f74 7970 6527 2c20  ' by genotype', 
-00004b20: 6e5f 726f 7773 3d6e 6729 0a20 2020 2020  n_rows=ng).     
-00004b30: 2020 2020 2020 2072 6573 756c 7473 5b66         results[f
-00004b40: 6c6f 772e 6e61 6d65 2b27 5f62 795f 6167  low.name+'_by_ag
-00004b50: 6527 5d20 2020 2020 2020 203d 2069 6e69  e']        = ini
-00004b60: 745f 7265 7328 666c 6f77 2e6c 6162 656c  t_res(flow.label
-00004b70: 2b27 2062 7920 6167 6527 2c20 6e5f 726f  +' by age', n_ro
-00004b80: 7773 3d6e 612c 2063 6f6c 6f72 3d66 6c6f  ws=na, color=flo
-00004b90: 772e 636f 6c6f 7229 0a0a 2020 2020 2020  w.color)..      
-00004ba0: 2020 2320 4372 6561 7465 2073 746f 636b    # Create stock
-00004bb0: 730a 2020 2020 2020 2020 666f 7220 7374  s.        for st
-00004bc0: 6f63 6b20 696e 2068 7064 2e50 656f 706c  ock in hpd.Peopl
-00004bd0: 654d 6574 6128 292e 7374 6f63 6b5f 7374  eMeta().stock_st
-00004be0: 6174 6573 3a0a 2020 2020 2020 2020 2020  ates:.          
-00004bf0: 2020 7265 7375 6c74 735b 6627 6e5f 7b73    results[f'n_{s
-00004c00: 746f 636b 2e6e 616d 657d 275d 2020 2020  tock.name}']    
-00004c10: 2020 2020 2020 2020 2020 3d20 696e 6974            = init
-00004c20: 5f72 6573 2873 746f 636b 2e6c 6162 656c  _res(stock.label
-00004c30: 2c20 636f 6c6f 723d 7374 6f63 6b2e 636f  , color=stock.co
-00004c40: 6c6f 7229 0a20 2020 2020 2020 2020 2020  lor).           
-00004c50: 2072 6573 756c 7473 5b66 276e 5f7b 7374   results[f'n_{st
-00004c60: 6f63 6b2e 6e61 6d65 7d5f 6279 5f67 656e  ock.name}_by_gen
-00004c70: 6f74 7970 6527 5d20 203d 2069 6e69 745f  otype']  = init_
-00004c80: 7265 7328 7374 6f63 6b2e 6c61 6265 6c2b  res(stock.label+
-00004c90: 2720 6279 2067 656e 6f74 7970 6527 2c20  ' by genotype', 
-00004ca0: 6e5f 726f 7773 3d6e 6729 0a0a 2020 2020  n_rows=ng)..    
-00004cb0: 2020 2020 2320 4f6e 6c79 2062 792d 6167      # Only by-ag
-00004cc0: 6520 7374 6f63 6b20 7265 7375 6c74 2077  e stock result w
-00004cd0: 6520 7769 6c6c 206e 6565 6420 6973 206e  e will need is n
-00004ce0: 756d 6265 7220 696e 6665 6374 696f 7573  umber infectious
-00004cf0: 2c20 7375 7363 6570 7469 626c 652c 2061  , susceptible, a
-00004d00: 6e64 2077 6974 6820 6369 6e2c 2066 6f72  nd with cin, for
-00004d10: 2048 5056 2061 6e64 2043 494e 2070 7265   HPV and CIN pre
-00004d20: 7661 6c65 6e63 652f 696e 6369 6465 6e63  valence/incidenc
-00004d30: 6520 6361 6c63 756c 6174 696f 6e73 0a20  e calculations. 
-00004d40: 2020 2020 2020 2072 6573 756c 7473 5b66         results[f
-00004d50: 276e 5f69 6e66 6563 7469 6f75 735f 6279  'n_infectious_by
-00004d60: 5f61 6765 275d 2020 2020 2020 2020 2020  _age']          
-00004d70: 2020 203d 2069 6e69 745f 7265 7328 274e     = init_res('N
-00004d80: 756d 6265 7220 696e 6665 6374 696f 7573  umber infectious
-00004d90: 2062 7920 6167 6527 2c20 6e5f 726f 7773   by age', n_rows
-00004da0: 3d6e 612c 2063 6f6c 6f72 3d73 746f 636b  =na, color=stock
-00004db0: 2e63 6f6c 6f72 290a 2020 2020 2020 2020  .color).        
-00004dc0: 7265 7375 6c74 735b 6627 6e5f 7375 7363  results[f'n_susc
-00004dd0: 6570 7469 626c 655f 6279 5f61 6765 275d  eptible_by_age']
-00004de0: 2020 2020 2020 2020 2020 2020 3d20 696e              = in
-00004df0: 6974 5f72 6573 2827 4e75 6d62 6572 2073  it_res('Number s
-00004e00: 7573 6365 7074 6962 6c65 2062 7920 6167  usceptible by ag
-00004e10: 6527 2c20 6e5f 726f 7773 3d6e 612c 2063  e', n_rows=na, c
-00004e20: 6f6c 6f72 3d73 746f 636b 2e63 6f6c 6f72  olor=stock.color
-00004e30: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-00004e40: 735b 6627 6e5f 7472 616e 7366 6f72 6d65  s[f'n_transforme
-00004e50: 645f 6279 5f61 6765 275d 2020 2020 2020  d_by_age']      
-00004e60: 2020 2020 2020 3d20 696e 6974 5f72 6573        = init_res
-00004e70: 2827 4e75 6d62 6572 2074 7261 6e73 666f  ('Number transfo
-00004e80: 726d 6564 2062 7920 6167 6527 2c20 6e5f  rmed by age', n_
-00004e90: 726f 7773 3d6e 612c 2063 6f6c 6f72 3d73  rows=na, color=s
-00004ea0: 746f 636b 2e63 6f6c 6f72 290a 2020 2020  tock.color).    
-00004eb0: 2020 2020 7265 7375 6c74 735b 6627 6e5f      results[f'n_
-00004ec0: 7072 6563 696e 5f62 795f 6167 6527 5d20  precin_by_age'] 
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ee0: 3d20 696e 6974 5f72 6573 2827 4e75 6d62  = init_res('Numb
-00004ef0: 6572 2050 7265 2d43 494e 2062 7920 6167  er Pre-CIN by ag
-00004f00: 6527 2c20 6e5f 726f 7773 3d6e 612c 2063  e', n_rows=na, c
-00004f10: 6f6c 6f72 3d73 746f 636b 2e63 6f6c 6f72  olor=stock.color
-00004f20: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-00004f30: 735b 6627 6e5f 6369 6e31 5f62 795f 6167  s[f'n_cin1_by_ag
-00004f40: 6527 5d20 2020 2020 2020 2020 2020 2020  e']             
-00004f50: 2020 2020 2020 3d20 696e 6974 5f72 6573        = init_res
-00004f60: 2827 4e75 6d62 6572 2043 494e 3120 6279  ('Number CIN1 by
-00004f70: 2061 6765 272c 206e 5f72 6f77 733d 6e61   age', n_rows=na
-00004f80: 2c20 636f 6c6f 723d 7374 6f63 6b2e 636f  , color=stock.co
-00004f90: 6c6f 7229 0a20 2020 2020 2020 2072 6573  lor).        res
-00004fa0: 756c 7473 5b66 276e 5f63 696e 325f 6279  ults[f'n_cin2_by
-00004fb0: 5f61 6765 275d 2020 2020 2020 2020 2020  _age']          
-00004fc0: 2020 2020 2020 2020 203d 2069 6e69 745f           = init_
-00004fd0: 7265 7328 274e 756d 6265 7220 4349 4e32  res('Number CIN2
-00004fe0: 2062 7920 6167 6527 2c20 6e5f 726f 7773   by age', n_rows
-00004ff0: 3d6e 612c 2063 6f6c 6f72 3d73 746f 636b  =na, color=stock
-00005000: 2e63 6f6c 6f72 290a 2020 2020 2020 2020  .color).        
-00005010: 7265 7375 6c74 735b 6627 6e5f 6369 6e33  results[f'n_cin3
-00005020: 5f62 795f 6167 6527 5d20 2020 2020 2020  _by_age']       
-00005030: 2020 2020 2020 2020 2020 2020 3d20 696e              = in
-00005040: 6974 5f72 6573 2827 4e75 6d62 6572 2043  it_res('Number C
-00005050: 494e 3320 6279 2061 6765 272c 206e 5f72  IN3 by age', n_r
-00005060: 6f77 733d 6e61 2c20 636f 6c6f 723d 7374  ows=na, color=st
-00005070: 6f63 6b2e 636f 6c6f 7229 0a0a 2020 2020  ock.color)..    
-00005080: 2020 2020 2320 4372 6561 7465 2069 6e63      # Create inc
-00005090: 6964 656e 6365 2061 6e64 2070 7265 7661  idence and preva
-000050a0: 6c65 6e63 6520 7265 7375 6c74 730a 2020  lence results.  
-000050b0: 2020 2020 2020 666f 7220 7661 722c 6e61        for var,na
-000050c0: 6d65 2c63 6f6c 6f72 2069 6e20 7a69 7028  me,color in zip(
-000050d0: 6870 642e 696e 6369 5f6b 6579 732c 2068  hpd.inci_keys, h
-000050e0: 7064 2e69 6e63 695f 6e61 6d65 732c 2068  pd.inci_names, h
-000050f0: 7064 2e69 6e63 695f 636f 6c6f 7273 293a  pd.inci_colors):
-00005100: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00005110: 756c 7473 5b66 277b 7661 727d 5f69 6e63  ults[f'{var}_inc
-00005120: 6964 656e 6365 275d 2020 2020 2020 2020  idence']        
-00005130: 2020 2020 203d 2069 6e69 745f 7265 7328       = init_res(
-00005140: 6e61 6d65 2b27 2069 6e63 6964 656e 6365  name+' incidence
-00005150: 272c 2063 6f6c 6f72 3d63 6f6c 6f72 290a  ', color=color).
-00005160: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00005170: 6c74 735b 6627 7b76 6172 7d5f 696e 6369  lts[f'{var}_inci
-00005180: 6465 6e63 655f 6279 5f67 656e 6f74 7970  dence_by_genotyp
-00005190: 6527 5d20 3d20 696e 6974 5f72 6573 286e  e'] = init_res(n
-000051a0: 616d 652b 2720 696e 6369 6465 6e63 6520  ame+' incidence 
-000051b0: 6279 2067 656e 6f74 7970 6527 2c20 6e5f  by genotype', n_
-000051c0: 726f 7773 3d6e 6729 0a20 2020 2020 2020  rows=ng).       
-000051d0: 2020 2020 2072 6573 756c 7473 5b66 277b       results[f'{
-000051e0: 7661 727d 5f69 6e63 6964 656e 6365 5f62  var}_incidence_b
-000051f0: 795f 6167 6527 5d20 2020 2020 203d 2069  y_age']      = i
-00005200: 6e69 745f 7265 7328 6e61 6d65 2b27 2069  nit_res(name+' i
-00005210: 6e63 6964 656e 6365 2062 7920 6167 6527  ncidence by age'
-00005220: 2c20 6e5f 726f 7773 3d6e 612c 2063 6f6c  , n_rows=na, col
-00005230: 6f72 3d63 6f6c 6f72 290a 0a20 2020 2020  or=color)..     
-00005240: 2020 2023 2043 7265 6174 6520 6465 6d6f     # Create demo
-00005250: 6772 6170 6869 6320 666c 6f77 730a 2020  graphic flows.  
-00005260: 2020 2020 2020 666f 7220 7661 722c 206e        for var, n
-00005270: 616d 652c 2063 6f6c 6f72 2069 6e20 7a69  ame, color in zi
-00005280: 7028 6870 642e 6465 6d5f 6b65 7973 2c20  p(hpd.dem_keys, 
-00005290: 6870 642e 6465 6d5f 6e61 6d65 732c 2068  hpd.dem_names, h
-000052a0: 7064 2e64 656d 5f63 6f6c 6f72 7329 3a0a  pd.dem_colors):.
-000052b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000052c0: 6c74 735b 7661 725d 203d 2069 6e69 745f  lts[var] = init_
-000052d0: 7265 7328 6e61 6d65 2c20 636f 6c6f 723d  res(name, color=
-000052e0: 636f 6c6f 7229 0a0a 2020 2020 2020 2020  color)..        
-000052f0: 2320 4372 6561 7465 2072 6573 756c 7473  # Create results
-00005300: 2062 7920 7365 780a 2020 2020 2020 2020   by sex.        
-00005310: 666f 7220 7661 722c 206e 616d 652c 2063  for var, name, c
-00005320: 6f6c 6f72 2069 6e20 7a69 7028 6870 642e  olor in zip(hpd.
-00005330: 6279 5f73 6578 5f6b 6579 732c 2068 7064  by_sex_keys, hpd
-00005340: 2e62 795f 7365 785f 636f 6c6f 7273 2c20  .by_sex_colors, 
-00005350: 6870 642e 6279 5f73 6578 5f63 6f6c 6f72  hpd.by_sex_color
-00005360: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00005370: 7265 7375 6c74 735b 7661 725d 203d 2069  results[var] = i
-00005380: 6e69 745f 7265 7328 6e61 6d65 2c20 636f  nit_res(name, co
-00005390: 6c6f 723d 636f 6c6f 722c 206e 5f72 6f77  lor=color, n_row
-000053a0: 733d 3229 0a0a 2020 2020 2020 2020 2320  s=2)..        # 
-000053b0: 4372 6561 7465 2041 5352 2072 6573 756c  Create ASR resul
-000053c0: 7473 2075 7369 6e67 2073 7461 6e64 6172  ts using standar
-000053d0: 6420 706f 7075 6c61 7469 6f6e 730a 2020  d populations.  
-000053e0: 2020 2020 2020 7265 7375 6c74 735b 2761        results['a
-000053f0: 7372 5f63 616e 6365 725f 696e 6369 6465  sr_cancer_incide
-00005400: 6e63 6527 5d20 3d20 696e 6974 5f72 6573  nce'] = init_res
-00005410: 2827 4167 652d 6164 6a75 7374 6564 2063  ('Age-adjusted c
-00005420: 6572 7669 6361 6c20 6361 6e63 6572 2069  ervical cancer i
-00005430: 6e63 6964 656e 6365 272c 2073 6361 6c65  ncidence', scale
-00005440: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00005450: 7265 7375 6c74 735b 2761 7372 5f63 616e  results['asr_can
-00005460: 6365 725f 6d6f 7274 616c 6974 7927 5d20  cer_mortality'] 
-00005470: 3d20 696e 6974 5f72 6573 2827 4167 652d  = init_res('Age-
-00005480: 6164 6a75 7374 6564 2063 6572 7669 6361  adjusted cervica
-00005490: 6c20 6361 6e63 6572 206d 6f72 7461 6c69  l cancer mortali
-000054a0: 7479 272c 2073 6361 6c65 3d46 616c 7365  ty', scale=False
-000054b0: 290a 0a20 2020 2020 2020 2073 746f 636b  )..        stock
-000054c0: 5f63 6f6c 6f72 7320 3d20 5b69 2066 6f72  _colors = [i for
-000054d0: 2069 2069 6e20 7365 7428 6870 642e 5065   i in set(hpd.Pe
-000054e0: 6f70 6c65 4d65 7461 2829 2e73 746f 636b  opleMeta().stock
-000054f0: 5f63 6f6c 6f72 7329 2069 6620 6920 6973  _colors) if i is
-00005500: 206e 6f74 204e 6f6e 655d 0a0a 2020 2020   not None]..    
-00005510: 2020 2020 2320 5479 7065 2064 6973 7472      # Type distr
-00005520: 6962 7574 696f 6e73 2062 7920 6379 746f  ibutions by cyto
-00005530: 6c6f 6779 0a20 2020 2020 2020 2066 6f72  logy.        for
-00005540: 2076 6172 2c20 6e61 6d65 2069 6e20 7a69   var, name in zi
-00005550: 7028 6870 642e 7479 7065 5f64 6973 745f  p(hpd.type_dist_
-00005560: 6b65 7973 2c20 6870 642e 7479 7065 5f64  keys, hpd.type_d
-00005570: 6973 745f 6e61 6d65 7329 3a0a 2020 2020  ist_names):.    
-00005580: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
-00005590: 7661 722b 275f 6765 6e6f 7479 7065 5f64  var+'_genotype_d
-000055a0: 6973 7427 5d20 3d20 696e 6974 5f72 6573  ist'] = init_res
-000055b0: 286e 616d 652c 206e 5f72 6f77 733d 6e67  (name, n_rows=ng
-000055c0: 2c20 636f 6c6f 723d 7374 6f63 6b5f 636f  , color=stock_co
-000055d0: 6c6f 7273 5b30 5d29 0a0a 2020 2020 2020  lors[0])..      
-000055e0: 2020 2320 5661 6363 696e 6174 696f 6e20    # Vaccination 
-000055f0: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
-00005600: 7265 7375 6c74 735b 276e 6577 5f76 6163  results['new_vac
-00005610: 6369 6e61 7465 6427 5d20 3d20 696e 6974  cinated'] = init
-00005620: 5f72 6573 2827 4e65 776c 7920 7661 6363  _res('Newly vacc
-00005630: 696e 6174 6564 2062 7920 6765 6e6f 7479  inated by genoty
-00005640: 7065 272c 206e 5f72 6f77 733d 6e67 290a  pe', n_rows=ng).
-00005650: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
-00005660: 276e 6577 5f74 6f74 616c 5f76 6163 6369  'new_total_vacci
-00005670: 6e61 7465 6427 5d20 3d20 696e 6974 5f72  nated'] = init_r
-00005680: 6573 2827 4e65 776c 7920 7661 6363 696e  es('Newly vaccin
-00005690: 6174 6564 2729 0a20 2020 2020 2020 2072  ated').        r
-000056a0: 6573 756c 7473 5b27 6375 6d5f 7661 6363  esults['cum_vacc
-000056b0: 696e 6174 6564 275d 203d 2069 6e69 745f  inated'] = init_
-000056c0: 7265 7328 2743 756d 756c 6174 6976 6520  res('Cumulative 
-000056d0: 6e75 6d62 6572 2076 6163 6369 6e61 7465  number vaccinate
-000056e0: 6420 6279 2067 656e 6f74 7970 6527 2c20  d by genotype', 
-000056f0: 6e5f 726f 7773 3d6e 6729 0a20 2020 2020  n_rows=ng).     
-00005700: 2020 2072 6573 756c 7473 5b27 6375 6d5f     results['cum_
-00005710: 746f 7461 6c5f 7661 6363 696e 6174 6564  total_vaccinated
-00005720: 275d 203d 2069 6e69 745f 7265 7328 2743  '] = init_res('C
-00005730: 756d 756c 6174 6976 6520 6e75 6d62 6572  umulative number
-00005740: 2076 6163 6369 6e61 7465 6427 290a 2020   vaccinated').  
-00005750: 2020 2020 2020 7265 7375 6c74 735b 276e        results['n
-00005760: 6577 5f64 6f73 6573 275d 203d 2069 6e69  ew_doses'] = ini
-00005770: 745f 7265 7328 274e 6577 2064 6f73 6573  t_res('New doses
-00005780: 2729 0a20 2020 2020 2020 2072 6573 756c  ').        resul
-00005790: 7473 5b27 6375 6d5f 646f 7365 7327 5d20  ts['cum_doses'] 
-000057a0: 3d20 696e 6974 5f72 6573 2827 4375 6d75  = init_res('Cumu
-000057b0: 6c61 7469 7665 2064 6f73 6573 2729 0a0a  lative doses')..
-000057c0: 2020 2020 2020 2020 2320 5468 6572 6170          # Therap
-000057d0: 6575 7469 6320 7661 6363 696e 6520 7265  eutic vaccine re
-000057e0: 7375 6c74 730a 2020 2020 2020 2020 7265  sults.        re
-000057f0: 7375 6c74 735b 276e 6577 5f74 7876 785f  sults['new_txvx_
-00005800: 646f 7365 7327 5d20 3d20 696e 6974 5f72  doses'] = init_r
-00005810: 6573 2827 4e65 7720 7468 6572 6170 6575  es('New therapeu
-00005820: 7469 6320 7661 6363 696e 6520 646f 7365  tic vaccine dose
-00005830: 7327 290a 2020 2020 2020 2020 7265 7375  s').        resu
-00005840: 6c74 735b 276e 6577 5f74 785f 7661 6363  lts['new_tx_vacc
-00005850: 696e 6174 6564 275d 203d 2069 6e69 745f  inated'] = init_
-00005860: 7265 7328 274e 6577 6c79 2072 6563 6569  res('Newly recei
-00005870: 7665 6420 7468 6572 6170 6575 7469 6320  ved therapeutic 
-00005880: 7661 6363 696e 6527 290a 2020 2020 2020  vaccine').      
-00005890: 2020 7265 7375 6c74 735b 2763 756d 5f74    results['cum_t
-000058a0: 7876 785f 646f 7365 7327 5d20 3d20 696e  xvx_doses'] = in
-000058b0: 6974 5f72 6573 2827 4375 6d75 6c61 7469  it_res('Cumulati
-000058c0: 7665 2074 6865 7261 7065 7574 6963 2076  ve therapeutic v
-000058d0: 6163 6369 6e65 2064 6f73 6573 2729 0a20  accine doses'). 
-000058e0: 2020 2020 2020 2072 6573 756c 7473 5b27         results['
-000058f0: 6375 6d5f 7478 5f76 6163 6369 6e61 7465  cum_tx_vaccinate
-00005900: 6427 5d20 3d20 696e 6974 5f72 6573 2827  d'] = init_res('
-00005910: 546f 7461 6c20 7265 6365 6976 6564 2074  Total received t
-00005920: 6865 7261 7065 7574 6963 2076 6163 6369  herapeutic vacci
-00005930: 6e65 2729 0a0a 2020 2020 2020 2020 2320  ne')..        # 
-00005940: 5363 7265 656e 2026 2074 7265 6174 2072  Screen & treat r
-00005950: 6573 756c 7473 0a20 2020 2020 2020 2072  esults.        r
-00005960: 6573 756c 7473 5b27 6e65 775f 7363 7265  esults['new_scre
-00005970: 656e 7327 5d20 3d20 696e 6974 5f72 6573  ens'] = init_res
-00005980: 2827 4e65 7720 7363 7265 656e 7327 290a  ('New screens').
-00005990: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
-000059a0: 276e 6577 5f73 6372 6565 6e65 6427 5d20  'new_screened'] 
-000059b0: 3d20 696e 6974 5f72 6573 2827 4e65 776c  = init_res('Newl
-000059c0: 7920 7363 7265 656e 6564 2729 0a20 2020  y screened').   
-000059d0: 2020 2020 2072 6573 756c 7473 5b27 6e65       results['ne
-000059e0: 775f 6369 6e5f 7472 6561 746d 656e 7473  w_cin_treatments
-000059f0: 275d 203d 2069 6e69 745f 7265 7328 274e  '] = init_res('N
-00005a00: 6577 2043 494e 2074 7265 6174 6d65 6e74  ew CIN treatment
-00005a10: 7327 290a 2020 2020 2020 2020 7265 7375  s').        resu
-00005a20: 6c74 735b 276e 6577 5f63 696e 5f74 7265  lts['new_cin_tre
-00005a30: 6174 6564 275d 203d 2069 6e69 745f 7265  ated'] = init_re
-00005a40: 7328 274e 6577 6c79 2074 7265 6174 6564  s('Newly treated
-00005a50: 2066 6f72 2043 494e 7327 290a 2020 2020   for CINs').    
-00005a60: 2020 2020 7265 7375 6c74 735b 276e 6577      results['new
-00005a70: 5f63 616e 6365 725f 7472 6561 746d 656e  _cancer_treatmen
-00005a80: 7473 275d 203d 2069 6e69 745f 7265 7328  ts'] = init_res(
-00005a90: 274e 6577 2063 616e 6365 7220 7472 6561  'New cancer trea
-00005aa0: 746d 656e 7473 2729 0a20 2020 2020 2020  tments').       
-00005ab0: 2072 6573 756c 7473 5b27 6e65 775f 6361   results['new_ca
-00005ac0: 6e63 6572 5f74 7265 6174 6564 275d 203d  ncer_treated'] =
-00005ad0: 2069 6e69 745f 7265 7328 274e 6577 6c79   init_res('Newly
-00005ae0: 2074 7265 6174 6564 2066 6f72 2063 616e   treated for can
-00005af0: 6365 7227 290a 2020 2020 2020 2020 7265  cer').        re
-00005b00: 7375 6c74 735b 2763 756d 5f73 6372 6565  sults['cum_scree
-00005b10: 6e73 275d 203d 2069 6e69 745f 7265 7328  ns'] = init_res(
-00005b20: 2743 756d 756c 6174 6976 6520 7363 7265  'Cumulative scre
-00005b30: 656e 7327 290a 2020 2020 2020 2020 7265  ens').        re
-00005b40: 7375 6c74 735b 2763 756d 5f73 6372 6565  sults['cum_scree
-00005b50: 6e65 6427 5d20 3d20 696e 6974 5f72 6573  ned'] = init_res
-00005b60: 2827 4375 6d75 6c61 7469 7665 206e 756d  ('Cumulative num
-00005b70: 6265 7220 7363 7265 656e 6564 2729 0a20  ber screened'). 
-00005b80: 2020 2020 2020 2072 6573 756c 7473 5b27         results['
-00005b90: 6375 6d5f 6369 6e5f 7472 6561 746d 656e  cum_cin_treatmen
-00005ba0: 7473 275d 203d 2069 6e69 745f 7265 7328  ts'] = init_res(
-00005bb0: 2743 756d 756c 6174 6976 6520 4349 4e20  'Cumulative CIN 
-00005bc0: 7472 6561 746d 656e 7473 2729 0a20 2020  treatments').   
-00005bd0: 2020 2020 2072 6573 756c 7473 5b27 6375       results['cu
-00005be0: 6d5f 6369 6e5f 7472 6561 7465 6427 5d20  m_cin_treated'] 
-00005bf0: 3d20 696e 6974 5f72 6573 2827 4375 6d75  = init_res('Cumu
-00005c00: 6c61 7469 7665 206e 756d 6265 7220 7472  lative number tr
-00005c10: 6561 7465 6420 666f 7220 4349 4e73 2729  eated for CINs')
-00005c20: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
-00005c30: 5b27 6375 6d5f 6361 6e63 6572 5f74 7265  ['cum_cancer_tre
-00005c40: 6174 6d65 6e74 7327 5d20 3d20 696e 6974  atments'] = init
-00005c50: 5f72 6573 2827 4375 6d75 6c61 7469 7665  _res('Cumulative
-00005c60: 2063 616e 6365 7220 7472 6561 746d 656e   cancer treatmen
-00005c70: 7473 2729 0a20 2020 2020 2020 2072 6573  ts').        res
-00005c80: 756c 7473 5b27 6375 6d5f 6361 6e63 6572  ults['cum_cancer
-00005c90: 5f74 7265 6174 6564 275d 203d 2069 6e69  _treated'] = ini
-00005ca0: 745f 7265 7328 2743 756d 756c 6174 6976  t_res('Cumulativ
-00005cb0: 6520 6e75 6d62 6572 2074 7265 6174 6564  e number treated
-00005cc0: 2066 6f72 2063 616e 6365 7227 290a 0a20   for cancer').. 
-00005cd0: 2020 2020 2020 2023 2041 6464 6974 696f         # Additio
-00005ce0: 6e61 6c20 6361 6e63 6572 2072 6573 756c  nal cancer resul
-00005cf0: 7473 0a20 2020 2020 2020 2072 6573 756c  ts.        resul
-00005d00: 7473 5b27 6465 7465 6374 6564 5f63 616e  ts['detected_can
-00005d10: 6365 725f 696e 6369 6465 6e63 6527 5d20  cer_incidence'] 
-00005d20: 3d20 696e 6974 5f72 6573 2827 4465 7465  = init_res('Dete
-00005d30: 6374 6564 2063 616e 6365 7220 696e 6369  cted cancer inci
-00005d40: 6465 6e63 6527 2c20 636f 6c6f 723d 2723  dence', color='#
-00005d50: 6663 6261 3033 2729 0a20 2020 2020 2020  fcba03').       
-00005d60: 2072 6573 756c 7473 5b27 6361 6e63 6572   results['cancer
-00005d70: 5f6d 6f72 7461 6c69 7479 275d 203d 2069  _mortality'] = i
-00005d80: 6e69 745f 7265 7328 2743 616e 6365 7220  nit_res('Cancer 
-00005d90: 6d6f 7274 616c 6974 7927 290a 0a20 2020  mortality')..   
-00005da0: 2020 2020 2023 204f 7468 6572 2072 6573       # Other res
-00005db0: 756c 7473 0a20 2020 2020 2020 2072 6573  ults.        res
-00005dc0: 756c 7473 5b27 6e5f 616c 6976 6527 5d20  ults['n_alive'] 
-00005dd0: 3d20 696e 6974 5f72 6573 2827 4e75 6d62  = init_res('Numb
-00005de0: 6572 2061 6c69 7665 2729 0a20 2020 2020  er alive').     
-00005df0: 2020 2072 6573 756c 7473 5b27 6e5f 616c     results['n_al
-00005e00: 6976 655f 6279 5f73 6578 275d 203d 2069  ive_by_sex'] = i
-00005e10: 6e69 745f 7265 7328 274e 756d 6265 7220  nit_res('Number 
-00005e20: 616c 6976 6520 6279 2073 6578 272c 206e  alive by sex', n
-00005e30: 5f72 6f77 733d 3229 0a20 2020 2020 2020  _rows=2).       
-00005e40: 2072 6573 756c 7473 5b27 6e5f 616c 6976   results['n_aliv
-00005e50: 655f 6279 5f61 6765 275d 203d 2069 6e69  e_by_age'] = ini
-00005e60: 745f 7265 7328 274e 756d 6265 7220 616c  t_res('Number al
-00005e70: 6976 6520 6279 2061 6765 272c 206e 5f72  ive by age', n_r
-00005e80: 6f77 733d 6e61 290a 2020 2020 2020 2020  ows=na).        
-00005e90: 7265 7375 6c74 735b 276e 5f66 656d 616c  results['n_femal
-00005ea0: 6573 5f61 6c69 7665 5f62 795f 6167 6527  es_alive_by_age'
-00005eb0: 5d20 3d20 696e 6974 5f72 6573 2827 4e75  ] = init_res('Nu
-00005ec0: 6d62 6572 2066 656d 616c 6573 2061 6c69  mber females ali
-00005ed0: 7665 2062 7920 6167 6527 2c20 6e5f 726f  ve by age', n_ro
-00005ee0: 7773 3d6e 6129 0a20 2020 2020 2020 2072  ws=na).        r
-00005ef0: 6573 756c 7473 5b27 6364 7227 5d20 3d20  esults['cdr'] = 
-00005f00: 696e 6974 5f72 6573 2827 4372 7564 6520  init_res('Crude 
-00005f10: 6465 6174 6820 7261 7465 272c 2073 6361  death rate', sca
-00005f20: 6c65 3d46 616c 7365 290a 2020 2020 2020  le=False).      
-00005f30: 2020 7265 7375 6c74 735b 2763 6272 275d    results['cbr']
-00005f40: 203d 2069 6e69 745f 7265 7328 2743 7275   = init_res('Cru
-00005f50: 6465 2062 6972 7468 2072 6174 6527 2c20  de birth rate', 
-00005f60: 7363 616c 653d 4661 6c73 652c 2063 6f6c  scale=False, col
-00005f70: 6f72 3d27 2366 6362 6130 3327 290a 2020  or='#fcba03').  
-00005f80: 2020 2020 2020 7265 7375 6c74 735b 2768        results['h
-00005f90: 7076 5f70 7265 7661 6c65 6e63 6527 5d20  pv_prevalence'] 
-00005fa0: 3d20 696e 6974 5f72 6573 2827 4850 5620  = init_res('HPV 
-00005fb0: 7072 6576 616c 656e 6365 272c 2063 6f6c  prevalence', col
-00005fc0: 6f72 3d73 746f 636b 5f63 6f6c 6f72 735b  or=stock_colors[
-00005fd0: 305d 290a 2020 2020 2020 2020 7265 7375  0]).        resu
-00005fe0: 6c74 735b 2768 7076 5f70 7265 7661 6c65  lts['hpv_prevale
-00005ff0: 6e63 655f 6279 5f67 656e 6f74 7970 6527  nce_by_genotype'
-00006000: 5d20 3d20 696e 6974 5f72 6573 2827 4850  ] = init_res('HP
-00006010: 5620 7072 6576 616c 656e 6365 272c 206e  V prevalence', n
-00006020: 5f72 6f77 733d 6e67 2c20 636f 6c6f 723d  _rows=ng, color=
-00006030: 7374 6f63 6b5f 636f 6c6f 7273 5b30 5d29  stock_colors[0])
-00006040: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
-00006050: 5b27 6870 765f 7072 6576 616c 656e 6365  ['hpv_prevalence
-00006060: 5f62 795f 6167 6527 5d20 3d20 696e 6974  _by_age'] = init
-00006070: 5f72 6573 2827 4850 5620 7072 6576 616c  _res('HPV preval
-00006080: 656e 6365 2062 7920 6167 6527 2c20 6e5f  ence by age', n_
-00006090: 726f 7773 3d6e 612c 2063 6f6c 6f72 3d73  rows=na, color=s
-000060a0: 746f 636b 5f63 6f6c 6f72 735b 305d 290a  tock_colors[0]).
-000060b0: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
-000060c0: 2770 7265 6369 6e5f 7072 6576 616c 656e  'precin_prevalen
-000060d0: 6365 275d 203d 2069 6e69 745f 7265 7328  ce'] = init_res(
-000060e0: 2750 7265 2d43 494e 2070 7265 7661 6c65  'Pre-CIN prevale
-000060f0: 6e63 6527 2c20 636f 6c6f 723d 7374 6f63  nce', color=stoc
-00006100: 6b5f 636f 6c6f 7273 5b30 5d29 0a20 2020  k_colors[0]).   
-00006110: 2020 2020 2072 6573 756c 7473 5b27 7072       results['pr
-00006120: 6563 696e 5f70 7265 7661 6c65 6e63 655f  ecin_prevalence_
-00006130: 6279 5f67 656e 6f74 7970 6527 5d20 3d20  by_genotype'] = 
-00006140: 696e 6974 5f72 6573 2827 5072 652d 4349  init_res('Pre-CI
-00006150: 4e20 7072 6576 616c 656e 6365 2062 7920  N prevalence by 
-00006160: 6765 6e6f 7479 7065 272c 206e 5f72 6f77  genotype', n_row
-00006170: 733d 6e67 2c20 636f 6c6f 723d 7374 6f63  s=ng, color=stoc
-00006180: 6b5f 636f 6c6f 7273 5b30 5d29 0a20 2020  k_colors[0]).   
-00006190: 2020 2020 2072 6573 756c 7473 5b27 7072       results['pr
-000061a0: 6563 696e 5f70 7265 7661 6c65 6e63 655f  ecin_prevalence_
-000061b0: 6279 5f61 6765 275d 203d 2069 6e69 745f  by_age'] = init_
-000061c0: 7265 7328 2750 7265 2d43 494e 2070 7265  res('Pre-CIN pre
-000061d0: 7661 6c65 6e63 6520 6279 2061 6765 272c  valence by age',
-000061e0: 206e 5f72 6f77 733d 6e61 2c20 636f 6c6f   n_rows=na, colo
-000061f0: 723d 7374 6f63 6b5f 636f 6c6f 7273 5b30  r=stock_colors[0
-00006200: 5d29 0a20 2020 2020 2020 2072 6573 756c  ]).        resul
-00006210: 7473 5b27 6369 6e31 5f70 7265 7661 6c65  ts['cin1_prevale
-00006220: 6e63 6527 5d20 3d20 696e 6974 5f72 6573  nce'] = init_res
-00006230: 2827 4349 4e31 2070 7265 7661 6c65 6e63  ('CIN1 prevalenc
-00006240: 6527 2c20 636f 6c6f 723d 7374 6f63 6b5f  e', color=stock_
-00006250: 636f 6c6f 7273 5b31 5d29 0a20 2020 2020  colors[1]).     
-00006260: 2020 2072 6573 756c 7473 5b27 6369 6e31     results['cin1
-00006270: 5f70 7265 7661 6c65 6e63 655f 6279 5f67  _prevalence_by_g
-00006280: 656e 6f74 7970 6527 5d20 3d20 696e 6974  enotype'] = init
-00006290: 5f72 6573 2827 4349 4e31 2070 7265 7661  _res('CIN1 preva
-000062a0: 6c65 6e63 6520 6279 2067 656e 6f74 7970  lence by genotyp
-000062b0: 6527 2c20 6e5f 726f 7773 3d6e 672c 2063  e', n_rows=ng, c
-000062c0: 6f6c 6f72 3d73 746f 636b 5f63 6f6c 6f72  olor=stock_color
-000062d0: 735b 315d 290a 2020 2020 2020 2020 7265  s[1]).        re
-000062e0: 7375 6c74 735b 2763 696e 315f 7072 6576  sults['cin1_prev
-000062f0: 616c 656e 6365 5f62 795f 6167 6527 5d20  alence_by_age'] 
-00006300: 3d20 696e 6974 5f72 6573 2827 4349 4e31  = init_res('CIN1
-00006310: 2070 7265 7661 6c65 6e63 6520 6279 2061   prevalence by a
-00006320: 6765 272c 206e 5f72 6f77 733d 6e61 2c20  ge', n_rows=na, 
-00006330: 636f 6c6f 723d 7374 6f63 6b5f 636f 6c6f  color=stock_colo
-00006340: 7273 5b31 5d29 0a20 2020 2020 2020 2072  rs[1]).        r
-00006350: 6573 756c 7473 5b27 6369 6e32 5f70 7265  esults['cin2_pre
-00006360: 7661 6c65 6e63 6527 5d20 3d20 696e 6974  valence'] = init
-00006370: 5f72 6573 2827 4349 4e32 2070 7265 7661  _res('CIN2 preva
-00006380: 6c65 6e63 6527 2c20 636f 6c6f 723d 7374  lence', color=st
-00006390: 6f63 6b5f 636f 6c6f 7273 5b32 5d29 0a20  ock_colors[2]). 
-000063a0: 2020 2020 2020 2072 6573 756c 7473 5b27         results['
-000063b0: 6369 6e32 5f70 7265 7661 6c65 6e63 655f  cin2_prevalence_
-000063c0: 6279 5f67 656e 6f74 7970 6527 5d20 3d20  by_genotype'] = 
-000063d0: 696e 6974 5f72 6573 2827 4349 4e32 2070  init_res('CIN2 p
-000063e0: 7265 7661 6c65 6e63 6520 6279 2067 656e  revalence by gen
-000063f0: 6f74 7970 6527 2c20 6e5f 726f 7773 3d6e  otype', n_rows=n
-00006400: 672c 2063 6f6c 6f72 3d73 746f 636b 5f63  g, color=stock_c
-00006410: 6f6c 6f72 735b 325d 290a 2020 2020 2020  olors[2]).      
-00006420: 2020 7265 7375 6c74 735b 2763 696e 325f    results['cin2_
-00006430: 7072 6576 616c 656e 6365 5f62 795f 6167  prevalence_by_ag
-00006440: 6527 5d20 3d20 696e 6974 5f72 6573 2827  e'] = init_res('
-00006450: 4349 4e32 2070 7265 7661 6c65 6e63 6520  CIN2 prevalence 
-00006460: 6279 2061 6765 272c 206e 5f72 6f77 733d  by age', n_rows=
-00006470: 6e61 2c20 636f 6c6f 723d 7374 6f63 6b5f  na, color=stock_
-00006480: 636f 6c6f 7273 5b32 5d29 0a20 2020 2020  colors[2]).     
-00006490: 2020 2072 6573 756c 7473 5b27 6369 6e33     results['cin3
-000064a0: 5f70 7265 7661 6c65 6e63 6527 5d20 3d20  _prevalence'] = 
-000064b0: 696e 6974 5f72 6573 2827 4349 4e33 2070  init_res('CIN3 p
-000064c0: 7265 7661 6c65 6e63 6527 2c20 636f 6c6f  revalence', colo
-000064d0: 723d 7374 6f63 6b5f 636f 6c6f 7273 5b33  r=stock_colors[3
-000064e0: 5d29 0a20 2020 2020 2020 2072 6573 756c  ]).        resul
-000064f0: 7473 5b27 6369 6e33 5f70 7265 7661 6c65  ts['cin3_prevale
-00006500: 6e63 655f 6279 5f67 656e 6f74 7970 6527  nce_by_genotype'
-00006510: 5d20 3d20 696e 6974 5f72 6573 2827 4349  ] = init_res('CI
-00006520: 4e33 2070 7265 7661 6c65 6e63 6527 2c20  N3 prevalence', 
-00006530: 6e5f 726f 7773 3d6e 672c 2063 6f6c 6f72  n_rows=ng, color
-00006540: 3d73 746f 636b 5f63 6f6c 6f72 735b 335d  =stock_colors[3]
-00006550: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-00006560: 735b 2763 696e 335f 7072 6576 616c 656e  s['cin3_prevalen
-00006570: 6365 5f62 795f 6167 6527 5d20 3d20 696e  ce_by_age'] = in
-00006580: 6974 5f72 6573 2827 4349 4e33 2070 7265  it_res('CIN3 pre
-00006590: 7661 6c65 6e63 6520 6279 2061 6765 272c  valence by age',
-000065a0: 206e 5f72 6f77 733d 6e61 2c20 636f 6c6f   n_rows=na, colo
-000065b0: 723d 7374 6f63 6b5f 636f 6c6f 7273 5b33  r=stock_colors[3
-000065c0: 5d29 0a0a 2020 2020 2020 2020 2320 5469  ])..        # Ti
-000065d0: 6d65 2076 6563 746f 720a 2020 2020 2020  me vector.      
-000065e0: 2020 7265 7375 6c74 735b 2779 6561 7227    results['year'
-000065f0: 5d20 3d20 7365 6c66 2e72 6573 5f79 6561  ] = self.res_yea
-00006600: 7276 6563 0a20 2020 2020 2020 2072 6573  rvec.        res
-00006610: 756c 7473 5b27 7427 5d20 3d20 7365 6c66  ults['t'] = self
-00006620: 2e72 6573 5f74 7665 630a 0a20 2020 2020  .res_tvec..     
-00006630: 2020 2023 2046 696e 616c 2069 7465 6d73     # Final items
-00006640: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00006650: 7375 6c74 7320 3d20 7265 7375 6c74 730a  sults = results.
-00006660: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00006670: 756c 7473 5f72 6561 6479 203d 2046 616c  ults_ready = Fal
-00006680: 7365 0a0a 2020 2020 2020 2020 7265 7475  se..        retu
-00006690: 726e 0a0a 0a20 2020 2064 6566 2069 6e69  rn...    def ini
-000066a0: 745f 7065 6f70 6c65 2873 656c 662c 2070  t_people(self, p
-000066b0: 6f70 6469 6374 3d4e 6f6e 652c 2069 6e69  opdict=None, ini
-000066c0: 745f 7374 6174 6573 3d46 616c 7365 2c20  t_states=False, 
-000066d0: 7265 7365 743d 4661 6c73 652c 2076 6572  reset=False, ver
-000066e0: 626f 7365 3d4e 6f6e 652c 202a 2a6b 7761  bose=None, **kwa
-000066f0: 7267 7329 3a0a 2020 2020 2020 2020 2727  rgs):.        ''
-00006700: 270a 2020 2020 2020 2020 4372 6561 7465  '.        Create
-00006710: 2074 6865 2070 656f 706c 6520 616e 6420   the people and 
-00006720: 7468 6520 6e65 7477 6f72 6b2e 0a0a 2020  the network...  
-00006730: 2020 2020 2020 5573 6520 6060 696e 6974        Use ``init
-00006740: 5f73 7461 7465 733d 4661 6c73 6560 6020  _states=False`` 
-00006750: 666f 7220 6372 6561 7469 6e67 2061 2066  for creating a f
-00006760: 7265 7368 2050 656f 706c 6520 6f62 6a65  resh People obje
-00006770: 6374 2066 6f72 2075 7365 0a20 2020 2020  ct for use.     
-00006780: 2020 2069 6e20 6675 7475 7265 2073 696d     in future sim
-00006790: 756c 6174 696f 6e73 0a0a 2020 2020 2020  ulations..      
-000067a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000067b0: 2020 2020 706f 7064 6963 7420 2020 2020      popdict     
-000067c0: 2020 2020 2861 6e79 293a 2020 7072 652d      (any):  pre-
-000067d0: 6765 6e65 7261 7465 6420 7065 6f70 6c65  generated people
-000067e0: 206f 6620 7661 7269 6f75 7320 666f 726d   of various form
-000067f0: 6174 732e 0a20 2020 2020 2020 2020 2020  ats..           
-00006800: 2069 6e69 745f 7374 6174 6573 2020 2020   init_states    
-00006810: 2028 626f 6f6c 293a 2077 6865 7468 6572   (bool): whether
-00006820: 2074 6f20 696e 6974 6961 6c69 7a65 2073   to initialize s
-00006830: 7461 7465 7320 2864 6566 6175 6c74 2066  tates (default f
-00006840: 616c 7365 2077 6865 6e20 6361 6c6c 6564  alse when called
-00006850: 2064 6972 6563 746c 7929 0a20 2020 2020   directly).     
-00006860: 2020 2020 2020 2072 6573 6574 2020 2020         reset    
-00006870: 2020 2020 2020 2028 626f 6f6c 293a 2077         (bool): w
-00006880: 6865 7468 6572 2074 6f20 7265 6765 6e65  hether to regene
-00006890: 7261 7465 2074 6865 2070 656f 706c 6520  rate the people 
-000068a0: 6576 656e 2069 6620 7468 6579 2061 6c72  even if they alr
-000068b0: 6561 6479 2065 7869 7374 0a20 2020 2020  eady exist.     
-000068c0: 2020 2020 2020 2076 6572 626f 7365 2020         verbose  
-000068d0: 2020 2020 2020 2028 696e 7429 3a20 2064         (int):  d
-000068e0: 6574 6169 6c20 746f 2070 7269 6e74 0a20  etail to print. 
-000068f0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00006900: 7320 2020 2020 2020 2020 2028 6469 6374  s          (dict
-00006910: 293a 2070 6173 7365 6420 746f 2068 7076  ): passed to hpv
-00006920: 2e6d 616b 655f 7065 6f70 6c65 2829 0a20  .make_people(). 
-00006930: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
-00006940: 2020 2020 2320 4861 6e64 6c65 2069 6e70      # Handle inp
-00006950: 7574 730a 2020 2020 2020 2020 6966 2076  uts.        if v
-00006960: 6572 626f 7365 2069 7320 4e6f 6e65 3a0a  erbose is None:.
-00006970: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-00006980: 6f73 6520 3d20 7365 6c66 5b27 7665 7262  ose = self['verb
-00006990: 6f73 6527 5d0a 2020 2020 2020 2020 6966  ose'].        if
-000069a0: 2070 6f70 6469 6374 2069 7320 6e6f 7420   popdict is not 
-000069b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000069c0: 2020 7365 6c66 2e70 6f70 6469 6374 203d    self.popdict =
-000069d0: 2070 6f70 6469 6374 0a20 2020 2020 2020   popdict.       
-000069e0: 2069 6620 7665 7262 6f73 6520 3e20 303a   if verbose > 0:
-000069f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00006a00: 6574 7374 723d 2027 270a 2020 2020 2020  etstr= ''.      
-00006a10: 2020 2020 2020 6966 2073 656c 662e 7065        if self.pe
-00006a20: 6f70 6c65 3a0a 2020 2020 2020 2020 2020  ople:.          
-00006a30: 2020 2020 2020 7265 7365 7473 7472 203d        resetstr =
-00006a40: 2027 2028 7265 7365 7474 696e 6720 7065   ' (resetting pe
-00006a50: 6f70 6c65 2927 2069 6620 7265 7365 7420  ople)' if reset 
-00006a60: 656c 7365 2027 2028 7761 726e 696e 673a  else ' (warning:
-00006a70: 206e 6f74 2072 6573 6574 7469 6e67 2073   not resetting s
-00006a80: 696d 2e70 656f 706c 6529 270a 2020 2020  im.people)'.    
-00006a90: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00006aa0: 496e 6974 6961 6c69 7a69 6e67 2073 696d  Initializing sim
-00006ab0: 7b72 6573 6574 7374 727d 2077 6974 6820  {resetstr} with 
-00006ac0: 7b73 656c 665b 226e 5f61 6765 6e74 7322  {self["n_agents"
-00006ad0: 5d3a 306e 7d20 6167 656e 7473 2729 0a20  ]:0n} agents'). 
-00006ae0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00006af0: 6f70 6669 6c65 2061 6e64 2073 656c 662e  opfile and self.
-00006b00: 706f 7064 6963 7420 6973 204e 6f6e 653a  popdict is None:
-00006b10: 2023 2049 6620 7468 6572 6527 7320 6120   # If there's a 
-00006b20: 706f 7064 6963 742c 2077 6520 696e 6974  popdict, we init
-00006b30: 6961 6c69 7a65 2069 740a 2020 2020 2020  ialize it.      
-00006b40: 2020 2020 2020 7365 6c66 2e6c 6f61 645f        self.load_
-00006b50: 706f 7075 6c61 7469 6f6e 2869 6e69 745f  population(init_
-00006b60: 7065 6f70 6c65 3d46 616c 7365 290a 0a20  people=False).. 
-00006b70: 2020 2020 2020 2023 204d 616b 6520 7468         # Make th
-00006b80: 6520 7065 6f70 6c65 0a20 2020 2020 2020  e people.       
-00006b90: 2073 656c 662e 7065 6f70 6c65 2c20 746f   self.people, to
-00006ba0: 7461 6c5f 706f 7020 3d20 6870 706f 702e  tal_pop = hppop.
-00006bb0: 6d61 6b65 5f70 656f 706c 6528 7365 6c66  make_people(self
-00006bc0: 2c20 7265 7365 743d 7265 7365 742c 2076  , reset=reset, v
-00006bd0: 6572 626f 7365 3d76 6572 626f 7365 2c20  erbose=verbose, 
-00006be0: 6d69 6372 6f73 7472 7563 7475 7265 3d73  microstructure=s
-00006bf0: 656c 665b 276e 6574 776f 726b 275d 2c20  elf['network'], 
-00006c00: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-00006c10: 2020 0a20 2020 2020 2020 2023 2046 6967    .        # Fig
-00006c20: 7572 6520 6f75 7420 7468 6520 7363 616c  ure out the scal
-00006c30: 6520 6661 6374 6f72 730a 2020 2020 2020  e factors.      
-00006c40: 2020 6966 2073 656c 665b 2774 6f74 616c    if self['total
-00006c50: 5f70 6f70 275d 2069 7320 6e6f 7420 4e6f  _pop'] is not No
-00006c60: 6e65 2061 6e64 2074 6f74 616c 5f70 6f70  ne and total_pop
-00006c70: 2069 7320 6e6f 7420 4e6f 6e65 3a20 2320   is not None: # 
-00006c80: 4966 206e 6f20 706f 705f 7363 616c 6520  If no pop_scale 
-00006c90: 6861 7320 6265 656e 2070 726f 7669 6465  has been provide
-00006ca0: 642c 2074 7279 2074 6f20 6765 7420 6974  d, try to get it
-00006cb0: 2066 726f 6d20 7468 6520 6c6f 6361 7469   from the locati
-00006cc0: 6f6e 0a20 2020 2020 2020 2020 2020 2065  on.            e
-00006cd0: 7272 6f72 6d73 6720 3d20 2759 6f75 2063  rrormsg = 'You c
-00006ce0: 616e 2065 6974 6865 7220 6465 6669 6e65  an either define
-00006cf0: 2074 6f74 616c 5f70 6f70 2065 7870 6c69   total_pop expli
-00006d00: 6369 746c 7920 6f72 2076 6961 2074 6865  citly or via the
-00006d10: 206c 6f63 6174 696f 6e2c 2062 7574 206e   location, but n
-00006d20: 6f74 2062 6f74 6827 0a20 2020 2020 2020  ot both'.       
-00006d30: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00006d40: 4572 726f 7228 6572 726f 726d 7367 290a  Error(errormsg).
-00006d50: 2020 2020 2020 2020 656c 6966 2074 6f74          elif tot
-00006d60: 616c 5f70 6f70 2069 7320 4e6f 6e65 2061  al_pop is None a
-00006d70: 6e64 2073 656c 665b 2774 6f74 616c 5f70  nd self['total_p
-00006d80: 6f70 275d 2069 7320 6e6f 7420 4e6f 6e65  op'] is not None
-00006d90: 3a0a 2020 2020 2020 2020 2020 2020 746f  :.            to
-00006da0: 7461 6c5f 706f 7020 3d20 7365 6c66 5b27  tal_pop = self['
-00006db0: 746f 7461 6c5f 706f 7027 5d0a 2020 2020  total_pop'].    
-00006dc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006dd0: 2069 6620 7365 6c66 5b27 706f 705f 7363   if self['pop_sc
-00006de0: 616c 6527 5d20 6973 204e 6f6e 653a 0a20  ale'] is None:. 
-00006df0: 2020 2020 2020 2020 2020 2069 6620 746f             if to
-00006e00: 7461 6c5f 706f 7020 6973 204e 6f6e 653a  tal_pop is None:
-00006e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006e20: 2073 656c 665b 2770 6f70 5f73 6361 6c65   self['pop_scale
-00006e30: 275d 203d 2031 2e30 0a20 2020 2020 2020  '] = 1.0.       
-00006e40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00006e50: 2020 2020 2020 2020 2020 2073 656c 665b             self[
-00006e60: 2770 6f70 5f73 6361 6c65 275d 203d 2074  'pop_scale'] = t
-00006e70: 6f74 616c 5f70 6f70 2f73 656c 665b 276e  otal_pop/self['n
-00006e80: 5f61 6765 6e74 7327 5d0a 2020 2020 2020  _agents'].      
-00006e90: 2020 7365 6c66 5b27 6d73 5f61 6765 6e74    self['ms_agent
-00006ea0: 5f72 6174 696f 275d 203d 2069 6e74 2873  _ratio'] = int(s
-00006eb0: 656c 665b 276d 735f 6167 656e 745f 7261  elf['ms_agent_ra
-00006ec0: 7469 6f27 5d29 0a0a 2020 2020 2020 2020  tio'])..        
-00006ed0: 2320 4465 616c 2077 6974 6820 4849 560a  # Deal with HIV.
-00006ee0: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
-00006ef0: 745f 6869 7628 2920 2320 4372 6561 7465  t_hiv() # Create
-00006f00: 7320 7468 6520 6869 7673 696d 206f 626a  s the hivsim obj
-00006f10: 6563 742c 2077 6869 6368 2069 7320 7374  ect, which is st
-00006f20: 6f72 6564 2069 6e20 7468 6520 7369 6d0a  ored in the sim.
-00006f30: 2020 2020 2020 2020 7365 6c66 2e68 6976          self.hiv
-00006f40: 7369 6d2e 696e 6974 5f73 7461 7465 7328  sim.init_states(
-00006f50: 7365 6c66 2e70 656f 706c 6529 2023 2041  self.people) # A
-00006f60: 6464 7320 736f 6d65 2073 7461 7465 7320  dds some states 
-00006f70: 746f 2074 6865 2070 656f 706c 650a 0a20  to the people.. 
-00006f80: 2020 2020 2020 2023 2046 696e 6973 6820         # Finish 
-00006f90: 696e 6974 6961 6c69 7a61 7469 6f6e 0a20  initialization. 
-00006fa0: 2020 2020 2020 2073 656c 662e 7065 6f70         self.peop
-00006fb0: 6c65 2e69 6e69 7469 616c 697a 6528 7369  le.initialize(si
-00006fc0: 6d5f 7061 7273 3d73 656c 662e 7061 7273  m_pars=self.pars
-00006fd0: 2920 2320 4675 6c6c 7920 696e 6974 6961  ) # Fully initia
-00006fe0: 6c69 7a65 2074 6865 2070 656f 706c 650a  lize the people.
-00006ff0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00007000: 6574 5f6c 6179 6572 5f70 6172 7328 666f  et_layer_pars(fo
-00007010: 7263 653d 4661 6c73 6529 2023 2045 6e73  rce=False) # Ens
-00007020: 7572 6520 7468 6174 206c 6179 6572 206b  ure that layer k
-00007030: 6579 7320 6d61 7463 6820 7468 6520 6c6f  eys match the lo
-00007040: 6164 6564 2070 6f70 756c 6174 696f 6e0a  aded population.
-00007050: 2020 2020 2020 2020 6966 2069 6e69 745f          if init_
-00007060: 7374 6174 6573 3a0a 2020 2020 2020 2020  states:.        
-00007070: 2020 2020 696e 6974 5f68 7076 5f70 7265      init_hpv_pre
-00007080: 7620 3d20 7363 2e64 6370 2873 656c 665b  v = sc.dcp(self[
-00007090: 2769 6e69 745f 6870 765f 7072 6576 275d  'init_hpv_prev']
-000070a0: 290a 2020 2020 2020 2020 2020 2020 696e  ).            in
-000070b0: 6974 5f68 7076 5f70 7265 762c 2061 6765  it_hpv_prev, age
-000070c0: 5f62 7261 636b 6574 7320 3d20 7365 6c66  _brackets = self
-000070d0: 2e76 616c 6964 6174 655f 696e 6974 5f63  .validate_init_c
-000070e0: 6f6e 6469 7469 6f6e 7328 696e 6974 5f68  onditions(init_h
-000070f0: 7076 5f70 7265 7629 0a20 2020 2020 2020  pv_prev).       
-00007100: 2020 2020 2073 656c 662e 696e 6974 5f73       self.init_s
-00007110: 7461 7465 7328 6167 655f 6272 6163 6b65  tates(age_bracke
-00007120: 7473 3d61 6765 5f62 7261 636b 6574 732c  ts=age_brackets,
-00007130: 2069 6e69 745f 6870 765f 7072 6576 3d69   init_hpv_prev=i
-00007140: 6e69 745f 6870 765f 7072 6576 290a 0a20  nit_hpv_prev).. 
-00007150: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00007160: 6c66 0a0a 2020 2020 6465 6620 696e 6974  lf..    def init
-00007170: 5f68 6976 2873 656c 6629 3a0a 2020 2020  _hiv(self):.    
-00007180: 2020 2020 2727 2720 496e 6974 6961 6c69      ''' Initiali
-00007190: 7a65 2073 7461 7465 732c 2061 7474 7269  ze states, attri
-000071a0: 6275 7465 732c 2061 6e64 2070 6172 616d  butes, and param
-000071b0: 6574 6572 7320 7265 6c61 7469 6e67 2074  eters relating t
-000071c0: 6f20 4849 5620 2727 270a 2020 2020 2020  o HIV '''.      
-000071d0: 2020 6966 2073 656c 662e 7061 7273 5b27    if self.pars['
-000071e0: 6d6f 6465 6c5f 6869 7627 5d3a 0a20 2020  model_hiv']:.   
-000071f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00007200: 2e68 6976 5f64 6174 6166 696c 6520 6973  .hiv_datafile is
-00007210: 204e 6f6e 6520 6f72 2073 656c 662e 6172   None or self.ar
-00007220: 745f 6461 7461 6669 6c65 2069 7320 4e6f  t_datafile is No
-00007230: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007240: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00007250: 7272 6f72 2827 4d75 7374 2073 7570 706c  rror('Must suppl
-00007260: 7920 4849 5620 616e 6420 4152 5420 6461  y HIV and ART da
-00007270: 7461 6669 6c65 7320 746f 206d 6f64 656c  tafiles to model
-00007280: 2048 4956 2e27 290a 2020 2020 2020 2020   HIV.').        
-00007290: 7365 6c66 2e68 6976 7369 6d20 3d20 6870  self.hivsim = hp
-000072a0: 6869 762e 4849 5673 696d 2873 656c 662c  hiv.HIVsim(self,
-000072b0: 2068 6976 5f64 6174 6166 696c 653d 7365   hiv_datafile=se
-000072c0: 6c66 2e68 6976 5f64 6174 6166 696c 652c  lf.hiv_datafile,
-000072d0: 2061 7274 5f64 6174 6166 696c 653d 7365   art_datafile=se
-000072e0: 6c66 2e61 7274 5f64 6174 6166 696c 652c  lf.art_datafile,
-000072f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 2020 2020 6869 765f 7061 7273 3d73 656c      hiv_pars=sel
-00007320: 665b 2768 6976 5f70 6172 7327 5d29 0a20  f['hiv_pars']). 
-00007330: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-00007340: 2020 2064 6566 2069 6e69 745f 696e 7465     def init_inte
-00007350: 7276 656e 7469 6f6e 7328 7365 6c66 293a  rventions(self):
-00007360: 0a20 2020 2020 2020 2027 2727 2049 6e69  .        ''' Ini
-00007370: 7469 616c 697a 6520 616e 6420 7661 6c69  tialize and vali
-00007380: 6461 7465 2074 6865 2069 6e74 6572 7665  date the interve
-00007390: 6e74 696f 6e73 2027 2727 0a0a 2020 2020  ntions '''..    
-000073a0: 2020 2020 2320 496e 6974 6961 6c69 7a61      # Initializa
-000073b0: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
-000073c0: 662e 696e 7465 7276 656e 7469 6f6e 7320  f.interventions 
-000073d0: 3d20 7363 2e61 7574 6f6c 6973 7428 290a  = sc.autolist().
-000073e0: 0a20 2020 2020 2020 2023 2054 7261 6e73  .        # Trans
-000073f0: 6c61 7465 2074 6865 2069 6e74 6572 7665  late the interve
-00007400: 6e74 696f 6e20 7370 6563 7320 696e 746f  ntion specs into
-00007410: 2061 6374 7561 6c20 696e 7465 7276 656e   actual interven
-00007420: 7469 6f6e 730a 2020 2020 2020 2020 666f  tions.        fo
-00007430: 7220 692c 696e 7465 7276 656e 7469 6f6e  r i,intervention
-00007440: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
-00007450: 6c66 5b27 696e 7465 7276 656e 7469 6f6e  lf['intervention
-00007460: 7327 5d29 3a0a 2020 2020 2020 2020 2020  s']):.          
-00007470: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00007480: 696e 7465 7276 656e 7469 6f6e 2c20 7479  intervention, ty
-00007490: 7065 2920 616e 6420 6973 7375 6263 6c61  pe) and issubcla
-000074a0: 7373 2869 6e74 6572 7665 6e74 696f 6e2c  ss(intervention,
-000074b0: 2068 7069 2e49 6e74 6572 7665 6e74 696f   hpi.Interventio
-000074c0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-000074d0: 2020 2020 696e 7465 7276 656e 7469 6f6e      intervention
-000074e0: 203d 2069 6e74 6572 7665 6e74 696f 6e28   = intervention(
-000074f0: 2920 2320 436f 6e76 6572 7420 6672 6f6d  ) # Convert from
-00007500: 2061 2063 6c61 7373 2074 6f20 616e 2069   a class to an i
-00007510: 6e73 7461 6e63 6520 6f66 2061 2063 6c61  nstance of a cla
-00007520: 7373 0a20 2020 2020 2020 2020 2020 2069  ss.            i
-00007530: 6620 6973 696e 7374 616e 6365 2869 6e74  f isinstance(int
-00007540: 6572 7665 6e74 696f 6e2c 2068 7069 2e49  ervention, hpi.I
-00007550: 6e74 6572 7665 6e74 696f 6e29 3a0a 2020  ntervention):.  
-00007560: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00007570: 7465 7276 656e 7469 6f6e 2e69 6e69 7469  tervention.initi
-00007580: 616c 697a 6528 7365 6c66 290a 2020 2020  alize(self).    
-00007590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000075a0: 2e69 6e74 6572 7665 6e74 696f 6e73 202b  .interventions +
-000075b0: 3d20 696e 7465 7276 656e 7469 6f6e 0a20  = intervention. 
-000075c0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000075d0: 6361 6c6c 6162 6c65 2869 6e74 6572 7665  callable(interve
-000075e0: 6e74 696f 6e29 3a0a 2020 2020 2020 2020  ntion):.        
-000075f0: 2020 2020 2020 2020 7365 6c66 2e69 6e74          self.int
-00007600: 6572 7665 6e74 696f 6e73 202b 3d20 696e  erventions += in
-00007610: 7465 7276 656e 7469 6f6e 0a20 2020 2020  tervention.     
-00007620: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007630: 2020 2020 2020 2020 2020 2020 2065 7272               err
-00007640: 6f72 6d73 6720 3d20 6627 496e 7465 7276  ormsg = f'Interv
-00007650: 656e 7469 6f6e 207b 696e 7465 7276 656e  ention {interven
-00007660: 7469 6f6e 7d20 646f 6573 206e 6f74 2073  tion} does not s
-00007670: 6565 6d20 746f 2062 6520 6120 7661 6c69  eem to be a vali
-00007680: 6420 696e 7465 7276 656e 7469 6f6e 3a20  d intervention: 
-00007690: 6d75 7374 2062 6520 6120 6675 6e63 7469  must be a functi
-000076a0: 6f6e 206f 7220 6870 762e 496e 7465 7276  on or hpv.Interv
-000076b0: 656e 7469 6f6e 2073 7562 636c 6173 7327  ention subclass'
-000076c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000076d0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000076e0: 2865 7272 6f72 6d73 6729 0a0a 2020 2020  (errormsg)..    
-000076f0: 2020 2020 7265 7475 726e 0a0a 0a20 2020      return...   
-00007700: 2064 6566 2069 6e69 745f 616e 616c 797a   def init_analyz
-00007710: 6572 7328 7365 6c66 293a 0a20 2020 2020  ers(self):.     
-00007720: 2020 2027 2727 2049 6e69 7469 616c 697a     ''' Initializ
-00007730: 6520 7468 6520 616e 616c 797a 6572 7320  e the analyzers 
-00007740: 2727 270a 0a20 2020 2020 2020 2073 656c  '''..        sel
-00007750: 662e 616e 616c 797a 6572 7320 3d20 7363  f.analyzers = sc
-00007760: 2e61 7574 6f6c 6973 7428 290a 0a20 2020  .autolist()..   
-00007770: 2020 2020 2064 6566 2063 6f6e 7665 7274       def convert
-00007780: 5f61 6e61 6c79 7a65 7228 616e 616c 797a  _analyzer(analyz
-00007790: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
-000077a0: 2027 2727 2048 656c 7065 7220 6675 6e63   ''' Helper func
-000077b0: 7469 6f6e 2074 6f20 7475 726e 2073 7472  tion to turn str
-000077c0: 696e 6773 2069 6e74 6f20 616e 616c 797a  ings into analyz
-000077d0: 6572 7320 2727 270a 2020 2020 2020 2020  ers '''.        
-000077e0: 2020 2020 6368 6f69 6365 7320 3d20 6870      choices = hp
-000077f0: 612e 616e 616c 797a 6572 5f6d 6170 2e6b  a.analyzer_map.k
-00007800: 6579 7328 290a 2020 2020 2020 2020 2020  eys().          
-00007810: 2020 6966 206e 6f74 2061 6e61 6c79 7a65    if not analyze
-00007820: 7220 696e 2063 686f 6963 6573 3a0a 2020  r in choices:.  
-00007830: 2020 2020 2020 2020 2020 2020 2020 6572                er
-00007840: 726f 726d 7367 203d 2066 2741 6e61 6c79  rormsg = f'Analy
-00007850: 7a65 7220 7b61 6e61 6c79 7a65 727d 206e  zer {analyzer} n
-00007860: 6f74 2075 6e64 6572 7374 6f6f 643a 2063  ot understood: c
-00007870: 686f 6963 6573 2061 7265 207b 6368 6f69  hoices are {choi
-00007880: 6365 737d 2e27 0a20 2020 2020 2020 2020  ces}.'.         
-00007890: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000078a0: 7565 4572 726f 7228 6572 726f 726d 7367  ueError(errormsg
-000078b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000078c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000078d0: 2020 2020 616e 616c 797a 6572 203d 2068      analyzer = h
-000078e0: 7061 2e61 6e61 6c79 7a65 725f 6d61 705b  pa.analyzer_map[
-000078f0: 616e 616c 797a 6572 5d0a 2020 2020 2020  analyzer].      
-00007900: 2020 2020 2020 7265 7475 726e 2061 6e61        return ana
-00007910: 6c79 7a65 720a 0a20 2020 2020 2020 2023  lyzer..        #
-00007920: 2049 6e74 6572 7072 6574 2061 6e61 6c79   Interpret analy
-00007930: 7a65 7273 0a20 2020 2020 2020 2066 6f72  zers.        for
-00007940: 2061 692c 616e 616c 797a 6572 2069 6e20   ai,analyzer in 
-00007950: 656e 756d 6572 6174 6528 7365 6c66 5b27  enumerate(self['
-00007960: 616e 616c 797a 6572 7327 5d29 3a0a 2020  analyzers']):.  
-00007970: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00007980: 6e73 7461 6e63 6528 616e 616c 797a 6572  nstance(analyzer
-00007990: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-000079a0: 2020 2020 2020 2020 616e 616c 797a 6572          analyzer
-000079b0: 5f6c 6973 7420 3d20 7363 2e74 6f6c 6973  _list = sc.tolis
-000079c0: 7428 636f 6e76 6572 745f 616e 616c 797a  t(convert_analyz
-000079d0: 6572 2861 6e61 6c79 7a65 7229 2920 2320  er(analyzer)) # 
-000079e0: 4966 206e 6f74 2061 206c 6973 742c 2074  If not a list, t
-000079f0: 7572 6e20 6974 2069 6e74 6f20 6f6e 6520  urn it into one 
-00007a00: 2d20 666f 7220 636f 6e73 6973 7465 6e63  - for consistenc
-00007a10: 7920 6f66 2070 726f 6365 7373 696e 670a  y of processing.
-00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a30: 666f 7220 617a 2069 6e20 616e 616c 797a  for az in analyz
-00007a40: 6572 5f6c 6973 743a 0a20 2020 2020 2020  er_list:.       
-00007a50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007a60: 6973 696e 7374 616e 6365 2861 7a2c 2073  isinstance(az, s
-00007a70: 7472 293a 2061 7a20 3d20 636f 6e76 6572  tr): az = conver
-00007a80: 745f 616e 616c 797a 6572 2861 7a29 2023  t_analyzer(az) #
-00007a90: 2049 7420 6d69 6768 7420 7374 696c 6c20   It might still 
-00007aa0: 6265 2061 2073 7472 696e 670a 2020 2020  be a string.    
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 7365 6c66 2e61 6e61 6c79 7a65 7273 202b  self.analyzers +
-00007ad0: 3d20 617a 2829 2023 2055 6e70 6163 6b20  = az() # Unpack 
-00007ae0: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
-00007af0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00007b00: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00007b10: 616e 6365 2861 6e61 6c79 7a65 722c 2074  ance(analyzer, t
-00007b20: 7970 6529 2061 6e64 2069 7373 7562 636c  ype) and issubcl
-00007b30: 6173 7328 616e 616c 797a 6572 2c20 6870  ass(analyzer, hp
-00007b40: 612e 416e 616c 797a 6572 293a 0a20 2020  a.Analyzer):.   
-00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 2061 6e61 6c79 7a65 7220 3d20 616e 616c   analyzer = anal
-00007b70: 797a 6572 2829 2023 2043 6f6e 7665 7274  yzer() # Convert
-00007b80: 2066 726f 6d20 6120 636c 6173 7320 746f   from a class to
-00007b90: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
-00007ba0: 6120 636c 6173 730a 2020 2020 2020 2020  a class.        
-00007bb0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-00007bc0: 6973 696e 7374 616e 6365 2861 6e61 6c79  isinstance(analy
-00007bd0: 7a65 722c 2068 7061 2e41 6e61 6c79 7a65  zer, hpa.Analyze
-00007be0: 7229 206f 7220 6361 6c6c 6162 6c65 2861  r) or callable(a
-00007bf0: 6e61 6c79 7a65 7229 293a 0a20 2020 2020  nalyzer)):.     
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00007c10: 7272 6f72 6d73 6720 3d20 6627 416e 616c  rrormsg = f'Anal
-00007c20: 797a 6572 207b 616e 616c 797a 6572 7d20  yzer {analyzer} 
-00007c30: 646f 6573 206e 6f74 2073 6565 6d20 746f  does not seem to
-00007c40: 2062 6520 6120 7661 6c69 6420 616e 616c   be a valid anal
-00007c50: 797a 6572 3a20 6d75 7374 2062 6520 6120  yzer: must be a 
-00007c60: 6675 6e63 7469 6f6e 206f 7220 6870 762e  function or hpv.
-00007c70: 416e 616c 797a 6572 2073 7562 636c 6173  Analyzer subclas
-00007c80: 7327 0a20 2020 2020 2020 2020 2020 2020  s'.             
-00007c90: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-00007ca0: 6545 7272 6f72 2865 7272 6f72 6d73 6729  eError(errormsg)
-00007cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007cc0: 2073 656c 662e 616e 616c 797a 6572 7320   self.analyzers 
-00007cd0: 2b3d 2061 6e61 6c79 7a65 7220 2320 4164  += analyzer # Ad
-00007ce0: 6420 6974 2069 6e0a 0a20 2020 2020 2020  d it in..       
-00007cf0: 2066 6f72 2061 6e61 6c79 7a65 7220 696e   for analyzer in
-00007d00: 2073 656c 662e 616e 616c 797a 6572 733a   self.analyzers:
-00007d10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007d20: 6973 696e 7374 616e 6365 2861 6e61 6c79  isinstance(analy
-00007d30: 7a65 722c 2068 7061 2e41 6e61 6c79 7a65  zer, hpa.Analyze
-00007d40: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00007d50: 2020 2020 616e 616c 797a 6572 2e69 6e69      analyzer.ini
-00007d60: 7469 616c 697a 6528 7365 6c66 290a 2020  tialize(self).  
-00007d70: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00007d80: 2020 2020 2020 2072 6574 7572 6e0a 0a0a         return...
-00007d90: 2020 2020 6465 6620 6669 6e61 6c69 7a65      def finalize
-00007da0: 5f61 6e61 6c79 7a65 7273 2873 656c 6629  _analyzers(self)
-00007db0: 3a0a 2020 2020 2020 2020 666f 7220 616e  :.        for an
-00007dc0: 616c 797a 6572 2069 6e20 7365 6c66 2e61  alyzer in self.a
-00007dd0: 6e61 6c79 7a65 7273 3a0a 2020 2020 2020  nalyzers:.      
-00007de0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00007df0: 6e63 6528 616e 616c 797a 6572 2c20 6870  nce(analyzer, hp
-00007e00: 612e 416e 616c 797a 6572 293a 0a20 2020  a.Analyzer):.   
-00007e10: 2020 2020 2020 2020 2020 2020 2061 6e61               ana
-00007e20: 6c79 7a65 722e 6669 6e61 6c69 7a65 2873  lyzer.finalize(s
-00007e30: 656c 6629 0a0a 0a20 2020 2064 6566 2069  elf)...    def i
-00007e40: 6e69 745f 7374 6174 6573 2873 656c 662c  nit_states(self,
-00007e50: 2061 6765 5f62 7261 636b 6574 733d 4e6f   age_brackets=No
-00007e60: 6e65 2c20 696e 6974 5f68 7076 5f70 7265  ne, init_hpv_pre
-00007e70: 763d 4e6f 6e65 2c20 696e 6974 5f63 696e  v=None, init_cin
-00007e80: 5f70 7265 763d 4e6f 6e65 2c20 696e 6974  _prev=None, init
-00007e90: 5f63 616e 6365 725f 7072 6576 3d4e 6f6e  _cancer_prev=Non
-00007ea0: 6529 3a0a 2020 2020 2020 2020 2727 270a  e):.        '''.
-00007eb0: 2020 2020 2020 2020 496e 6974 6961 6c69          Initiali
-00007ec0: 7a65 2070 7269 6f72 2069 6d6d 756e 6974  ze prior immunit
-00007ed0: 7920 616e 6420 7365 6564 2069 6e66 6563  y and seed infec
-00007ee0: 7469 6f6e 730a 2020 2020 2020 2020 2727  tions.        ''
-00007ef0: 270a 0a20 2020 2020 2020 2023 2053 686f  '..        # Sho
-00007f00: 7274 656e 206b 6579 2076 6172 6961 626c  rten key variabl
-00007f10: 6573 0a20 2020 2020 2020 206e 6720 3d20  es.        ng = 
-00007f20: 7365 6c66 5b27 6e5f 6765 6e6f 7479 7065  self['n_genotype
-00007f30: 7327 5d0a 0a20 2020 2020 2020 2023 2041  s']..        # A
-00007f40: 7373 6967 6e20 7065 6f70 6c65 2074 6f20  ssign people to 
-00007f50: 6167 6520 6275 636b 6574 730a 2020 2020  age buckets.    
-00007f60: 2020 2020 6167 655f 696e 6473 203d 206e      age_inds = n
-00007f70: 702e 6469 6769 7469 7a65 2873 656c 662e  p.digitize(self.
-00007f80: 7065 6f70 6c65 2e61 6765 2c20 6167 655f  people.age, age_
-00007f90: 6272 6163 6b65 7473 290a 0a20 2020 2020  brackets)..     
-00007fa0: 2020 2023 2041 7373 6967 6e20 7072 6f62     # Assign prob
-00007fb0: 6162 696c 6974 6965 7320 6f66 2068 6176  abilities of hav
-00007fc0: 696e 6720 4850 5620 746f 2065 6163 6820  ing HPV to each 
-00007fd0: 6167 652f 7365 7820 6772 6f75 700a 2020  age/sex group.  
-00007fe0: 2020 2020 2020 6870 765f 7072 6f62 7320        hpv_probs 
-00007ff0: 3d20 6e70 2e66 756c 6c28 6c65 6e28 7365  = np.full(len(se
-00008000: 6c66 2e70 656f 706c 6529 2c20 6e70 2e6e  lf.people), np.n
-00008010: 616e 2c20 6474 7970 653d 6870 642e 6465  an, dtype=hpd.de
-00008020: 6661 756c 745f 666c 6f61 7429 0a20 2020  fault_float).   
-00008030: 2020 2020 2068 7076 5f70 726f 6273 5b73       hpv_probs[s
-00008040: 656c 662e 7065 6f70 6c65 2e66 5f69 6e64  elf.people.f_ind
-00008050: 735d 203d 2069 6e69 745f 6870 765f 7072  s] = init_hpv_pr
-00008060: 6576 5b27 6627 5d5b 6167 655f 696e 6473  ev['f'][age_inds
-00008070: 5b73 656c 662e 7065 6f70 6c65 2e66 5f69  [self.people.f_i
-00008080: 6e64 735d 5d2a 7365 6c66 2e70 6172 735b  nds]]*self.pars[
-00008090: 2772 656c 5f69 6e69 745f 7072 6576 275d  'rel_init_prev']
-000080a0: 0a20 2020 2020 2020 2068 7076 5f70 726f  .        hpv_pro
-000080b0: 6273 5b73 656c 662e 7065 6f70 6c65 2e6d  bs[self.people.m
-000080c0: 5f69 6e64 735d 203d 2069 6e69 745f 6870  _inds] = init_hp
-000080d0: 765f 7072 6576 5b27 6d27 5d5b 6167 655f  v_prev['m'][age_
-000080e0: 696e 6473 5b73 656c 662e 7065 6f70 6c65  inds[self.people
-000080f0: 2e6d 5f69 6e64 735d 5d2a 7365 6c66 2e70  .m_inds]]*self.p
-00008100: 6172 735b 2772 656c 5f69 6e69 745f 7072  ars['rel_init_pr
-00008110: 6576 275d 0a20 2020 2020 2020 2068 7076  ev'].        hpv
-00008120: 5f70 726f 6273 5b7e 7365 6c66 2e70 656f  _probs[~self.peo
-00008130: 706c 652e 6973 5f61 6374 6976 655d 203d  ple.is_active] =
-00008140: 2030 2023 2042 6c61 6e6b 206f 7574 2070   0 # Blank out p
-00008150: 656f 706c 6520 7768 6f20 6172 6520 6e6f  eople who are no
-00008160: 7420 7965 7420 7365 7875 616c 6c79 2061  t yet sexually a
-00008170: 6374 6976 650a 0a20 2020 2020 2020 2023  ctive..        #
-00008180: 2047 6574 2069 6e64 6963 6573 206f 6620   Get indices of 
-00008190: 7065 6f70 6c65 2077 686f 2068 6176 6520  people who have 
-000081a0: 4850 560a 2020 2020 2020 2020 6870 765f  HPV.        hpv_
-000081b0: 696e 6473 203d 2068 7075 2e74 7275 6528  inds = hpu.true(
-000081c0: 6870 752e 6269 6e6f 6d69 616c 5f61 7272  hpu.binomial_arr
-000081d0: 2868 7076 5f70 726f 6273 2929 0a0a 2020  (hpv_probs))..  
-000081e0: 2020 2020 2020 2320 4465 7465 726d 696e        # Determin
-000081f0: 6520 7768 6963 6820 6765 6e6f 7479 7065  e which genotype
-00008200: 2070 656f 706c 6520 6172 6520 696e 6665   people are infe
-00008210: 6374 6564 2077 6974 680a 2020 2020 2020  cted with.      
-00008220: 2020 6966 2073 656c 665b 2769 6e69 745f    if self['init_
-00008230: 6870 765f 6469 7374 275d 2069 7320 4e6f  hpv_dist'] is No
-00008240: 6e65 3a20 2320 4e6f 2074 7970 6520 6469  ne: # No type di
-00008250: 7374 7269 6275 7469 6f6e 2070 726f 7669  stribution provi
-00008260: 6465 642c 2061 7373 756d 6520 6576 656e  ded, assume even
-00008270: 2073 706c 6974 0a20 2020 2020 2020 2020   split.         
-00008280: 2020 2067 656e 6f74 7970 6573 203d 206e     genotypes = n
-00008290: 702e 7261 6e64 6f6d 2e72 616e 6469 6e74  p.random.randint
-000082a0: 2830 2c20 6e67 2c20 6c65 6e28 6870 765f  (0, ng, len(hpv_
-000082b0: 696e 6473 2929 0a20 2020 2020 2020 2065  inds)).        e
-000082c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000082d0: 2023 2045 7272 6f72 2063 6865 636b 696e   # Error checkin
-000082e0: 670a 2020 2020 2020 2020 2020 2020 6966  g.            if
-000082f0: 206e 6f74 2073 632e 6368 6563 6b74 7970   not sc.checktyp
-00008300: 6528 7365 6c66 5b27 696e 6974 5f68 7076  e(self['init_hpv
-00008310: 5f64 6973 7427 5d2c 2064 6963 7429 3a0a  _dist'], dict):.
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 6572 726f 726d 7367 203d 2066 2750 6c65  errormsg = f'Ple
-00008340: 6173 6520 7072 6f76 6964 6520 696e 6974  ase provide init
-00008350: 6961 6c20 4850 5620 7479 7065 2064 6973  ial HPV type dis
-00008360: 7472 6962 7574 696f 6e20 6173 2061 2064  tribution as a d
-00008370: 6963 7469 6f6e 6172 7920 6b65 7965 6420  ictionary keyed 
-00008380: 6279 2067 656e 6f74 7970 652c 206e 6f74  by genotype, not
-00008390: 207b 7365 6c66 5b22 696e 6974 5f68 7076   {self["init_hpv
-000083a0: 5f64 6973 7422 5d7d 270a 2020 2020 2020  _dist"]}'.      
-000083b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000083c0: 5661 6c75 6545 7272 6f72 2865 7272 6f72  ValueError(error
-000083d0: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
-000083e0: 2069 6620 7365 7428 7365 6c66 5b27 696e   if set(self['in
-000083f0: 6974 5f68 7076 5f64 6973 7427 5d2e 6b65  it_hpv_dist'].ke
-00008400: 7973 2829 2921 3d73 6574 2873 656c 665b  ys())!=set(self[
-00008410: 2767 656e 6f74 7970 655f 6d61 7027 5d2e  'genotype_map'].
-00008420: 7661 6c75 6573 2829 293a 0a20 2020 2020  values()):.     
-00008430: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00008440: 6d73 6720 3d20 6627 5468 6520 4850 5620  msg = f'The HPV 
-00008450: 7479 7065 7320 7072 6f76 6964 6564 2069  types provided i
-00008460: 6e20 7468 6520 696e 6974 6961 6c20 4850  n the initial HP
-00008470: 5620 7479 7065 2064 6973 7472 6962 7574  V type distribut
-00008480: 696f 6e20 6172 6520 6e6f 7420 7468 6520  ion are not the 
-00008490: 7361 6d65 2061 7320 7468 6520 4850 5620  same as the HPV 
-000084a0: 7479 7065 7320 6265 696e 6720 7369 6d75  types being simu
-000084b0: 6c61 7465 643a 207b 7365 6c66 5b22 696e  lated: {self["in
-000084c0: 6974 5f68 7076 5f64 6973 7422 5d2e 6b65  it_hpv_dist"].ke
-000084d0: 7973 2829 7d20 7673 207b 7365 6c66 5b22  ys()} vs {self["
-000084e0: 6765 6e6f 7479 7065 5f6d 6170 225d 2e76  genotype_map"].v
-000084f0: 616c 7565 7328 297d 2e27 0a20 2020 2020  alues()}.'.     
-00008500: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00008510: 2056 616c 7565 4572 726f 7228 6572 726f   ValueError(erro
-00008520: 726d 7367 290a 0a20 2020 2020 2020 2020  rmsg)..         
-00008530: 2020 2074 7970 655f 6469 7374 203d 206e     type_dist = n
-00008540: 702e 6172 7261 7928 6c69 7374 2873 656c  p.array(list(sel
-00008550: 665b 2769 6e69 745f 6870 765f 6469 7374  f['init_hpv_dist
-00008560: 275d 2e76 616c 7565 7328 2929 290a 2020  '].values())).  
-00008570: 2020 2020 2020 2020 2020 6765 6e6f 7479            genoty
-00008580: 7065 7320 3d20 6870 752e 6368 6f6f 7365  pes = hpu.choose
-00008590: 5f77 2874 7970 655f 6469 7374 2c20 6c65  _w(type_dist, le
-000085a0: 6e28 6870 765f 696e 6473 292c 2075 6e69  n(hpv_inds), uni
-000085b0: 7175 653d 4661 6c73 6529 0a0a 2020 2020  que=False)..    
-000085c0: 2020 2020 666f 7220 6720 696e 2072 616e      for g in ran
-000085d0: 6765 286e 6729 3a0a 2020 2020 2020 2020  ge(ng):.        
-000085e0: 2020 2020 7365 6c66 2e70 656f 706c 652e      self.people.
-000085f0: 696e 6665 6374 2869 6e64 733d 6870 765f  infect(inds=hpv_
-00008600: 696e 6473 5b67 656e 6f74 7970 6573 3d3d  inds[genotypes==
-00008610: 675d 2c20 673d 672c 206c 6179 6572 3d27  g], g=g, layer='
-00008620: 7365 6564 5f69 6e66 6563 7469 6f6e 2729  seed_infection')
-00008630: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00008640: 0a0a 0a20 2020 2064 6566 2073 7465 7028  ...    def step(
-00008650: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
-00008660: 2727 2053 7465 7020 7468 726f 7567 6820  '' Step through 
-00008670: 7469 6d65 2061 6e64 2075 7064 6174 6520  time and update 
-00008680: 7661 6c75 6573 2027 2727 0a0a 2020 2020  values '''..    
-00008690: 2020 2020 2320 5365 7420 7468 6520 7469      # Set the ti
-000086a0: 6d65 2061 6e64 2069 6620 7765 2068 6176  me and if we hav
-000086b0: 6520 7265 6163 6865 6420 7468 6520 656e  e reached the en
-000086c0: 6420 6f66 2074 6865 2073 696d 756c 6174  d of the simulat
-000086d0: 696f 6e2c 2074 6865 6e20 646f 206e 6f74  ion, then do not
-000086e0: 6869 6e67 0a20 2020 2020 2020 2069 6620  hing.        if 
-000086f0: 7365 6c66 2e63 6f6d 706c 6574 653a 0a20  self.complete:. 
-00008700: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00008710: 2041 6c72 6561 6479 5275 6e45 7272 6f72   AlreadyRunError
-00008720: 2827 5369 6d75 6c61 7469 6f6e 2061 6c72  ('Simulation alr
-00008730: 6561 6479 2063 6f6d 706c 6574 6520 2863  eady complete (c
-00008740: 616c 6c20 7369 6d2e 696e 6974 6961 6c69  all sim.initiali
-00008750: 7a65 2829 2074 6f20 7265 2d72 756e 2927  ze() to re-run)'
-00008760: 290a 0a20 2020 2020 2020 2023 2053 686f  )..        # Sho
-00008770: 7274 656e 206b 6579 2076 6172 6961 626c  rten key variabl
-00008780: 6573 0a20 2020 2020 2020 2064 7420 3d20  es.        dt = 
-00008790: 7365 6c66 5b27 6474 275d 2023 2054 696d  self['dt'] # Tim
-000087a0: 6573 7465 700a 2020 2020 2020 2020 7420  estep.        t 
-000087b0: 3d20 7365 6c66 2e74 0a20 2020 2020 2020  = self.t.       
-000087c0: 206e 6720 3d20 7365 6c66 5b27 6e5f 6765   ng = self['n_ge
-000087d0: 6e6f 7479 7065 7327 5d0a 2020 2020 2020  notypes'].      
-000087e0: 2020 6e61 203d 206c 656e 2873 656c 662e    na = len(self.
-000087f0: 7061 7273 5b27 6167 655f 6269 6e73 275d  pars['age_bins']
-00008800: 2920 2d20 3120 2320 4e75 6d62 6572 206f  ) - 1 # Number o
-00008810: 6620 6167 6520 6269 6e73 0a20 2020 2020  f age bins.     
-00008820: 2020 2063 6f6e 646f 6d73 203d 2073 656c     condoms = sel
-00008830: 665b 2763 6f6e 646f 6d73 275d 0a20 2020  f['condoms'].   
-00008840: 2020 2020 2065 6666 5f63 6f6e 646f 6d73       eff_condoms
-00008850: 203d 2073 656c 665b 2765 6666 5f63 6f6e   = self['eff_con
-00008860: 646f 6d73 275d 0a20 2020 2020 2020 2062  doms'].        b
-00008870: 6574 6120 3d20 7365 6c66 5b27 6265 7461  eta = self['beta
-00008880: 275d 0a20 2020 2020 2020 2067 656e 5f70  '].        gen_p
-00008890: 6172 7320 3d20 7365 6c66 5b27 6765 6e6f  ars = self['geno
-000088a0: 7479 7065 5f70 6172 7327 5d0a 2020 2020  type_pars'].    
-000088b0: 2020 2020 696d 6d5f 6b69 6e5f 7061 7273      imm_kin_pars
-000088c0: 203d 2073 656c 665b 2769 6d6d 5f6b 696e   = self['imm_kin
-000088d0: 275d 0a20 2020 2020 2020 206d 6978 696e  '].        mixin
-000088e0: 6720 3d20 7365 6c66 5b27 6d69 7869 6e67  g = self['mixing
-000088f0: 275d 0a20 2020 2020 2020 206c 6179 6572  '].        layer
-00008900: 5f70 726f 6273 203d 2073 656c 665b 276c  _probs = self['l
-00008910: 6179 6572 5f70 726f 6273 275d 0a20 2020  ayer_probs'].   
-00008920: 2020 2020 2063 726f 7373 5f6c 6179 6572       cross_layer
-00008930: 203d 2073 656c 665b 2763 726f 7373 5f6c   = self['cross_l
-00008940: 6179 6572 275d 0a20 2020 2020 2020 2061  ayer'].        a
-00008950: 6374 7320 3d20 7365 6c66 5b27 6163 7473  cts = self['acts
-00008960: 275d 0a20 2020 2020 2020 2064 7572 5f70  '].        dur_p
-00008970: 7368 6970 203d 2073 656c 665b 2764 7572  ship = self['dur
-00008980: 5f70 7368 6970 275d 0a20 2020 2020 2020  _pship'].       
-00008990: 2061 6765 5f61 6374 5f70 6172 7320 3d20   age_act_pars = 
-000089a0: 7365 6c66 5b27 6167 655f 6163 745f 7061  self['age_act_pa
-000089b0: 7273 275d 0a20 2020 2020 2020 2074 7261  rs'].        tra
-000089c0: 6e73 203d 206e 702e 6172 7261 7928 5b73  ns = np.array([s
-000089d0: 656c 665b 2774 7261 6e73 6632 6d27 5d2c  elf['transf2m'],
-000089e0: 7365 6c66 5b27 7472 616e 736d 3266 275d  self['transm2f']
-000089f0: 5d29 2023 2046 324d 2066 6972 7374 2073  ]) # F2M first s
-00008a00: 696e 6365 2074 6861 7427 7320 7468 6520  ince that's the 
-00008a10: 6f72 6465 7220 7468 696e 6773 2061 7265  order things are
-00008a20: 2064 6f6e 6520 6c61 7465 720a 2020 2020   done later.    
-00008a30: 2020 2020 7965 6172 203d 2073 656c 662e      year = self.
-00008a40: 7965 6172 7665 635b 745d 0a0a 2020 2020  yearvec[t]..    
-00008a50: 2020 2020 2320 4d61 6b65 2048 4956 2d72      # Make HIV-r
-00008a60: 656c 6174 6564 2075 7064 6174 6573 0a20  elated updates. 
-00008a70: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00008a80: 6172 735b 276d 6f64 656c 5f68 6976 275d  ars['model_hiv']
-00008a90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008aa0: 6c66 2e68 6976 7369 6d2e 7374 6570 2870  lf.hivsim.step(p
-00008ab0: 656f 706c 653d 7365 6c66 2e70 656f 706c  eople=self.peopl
-00008ac0: 652c 2079 6561 723d 7965 6172 290a 0a20  e, year=year).. 
-00008ad0: 2020 2020 2020 2023 2055 7064 6174 6520         # Update 
-00008ae0: 6465 6d6f 6772 6170 6869 6373 2c20 7374  demographics, st
-00008af0: 6174 6573 2c20 616e 6420 7061 7274 6e65  ates, and partne
-00008b00: 7273 6869 7073 0a20 2020 2020 2020 2073  rships.        s
-00008b10: 656c 662e 7065 6f70 6c65 2e75 7064 6174  elf.people.updat
-00008b20: 655f 7374 6174 6573 5f70 7265 2874 3d74  e_states_pre(t=t
-00008b30: 2c20 7965 6172 3d79 6561 7229 2023 2054  , year=year) # T
-00008b40: 6869 7320 616c 736f 2061 6765 7320 7065  his also ages pe
-00008b50: 6f70 6c65 2c20 6170 706c 6965 7320 6465  ople, applies de
-00008b60: 6174 6873 2c20 616e 6420 6765 6e65 7261  aths, and genera
-00008b70: 7465 7320 6e65 7720 6269 7274 6873 0a20  tes new births. 
-00008b80: 2020 2020 2020 2070 656f 706c 6520 3d20         people = 
-00008b90: 7365 6c66 2e70 656f 706c 6520 2320 5368  self.people # Sh
-00008ba0: 6f72 7465 6e0a 2020 2020 2020 2020 7065  orten.        pe
-00008bb0: 6f70 6c65 2e64 6973 736f 6c76 655f 7061  ople.dissolve_pa
-00008bc0: 7274 6e65 7273 6869 7073 2874 3d74 2920  rtnerships(t=t) 
-00008bd0: 2320 4469 7373 6f6c 7665 2070 6172 746e  # Dissolve partn
-00008be0: 6572 7368 6970 730a 2020 2020 2020 2020  erships.        
-00008bf0: 7469 6e64 203d 2073 656c 662e 7965 6172  tind = self.year
-00008c00: 7665 635b 745d 202d 2073 656c 665b 2773  vec[t] - self['s
-00008c10: 7461 7274 275d 0a20 2020 2020 2020 2070  tart'].        p
-00008c20: 656f 706c 652e 6372 6561 7465 5f70 6172  eople.create_par
-00008c30: 746e 6572 7368 6970 7328 7469 6e64 2c20  tnerships(tind, 
-00008c40: 6d69 7869 6e67 2c20 6c61 7965 725f 7072  mixing, layer_pr
-00008c50: 6f62 732c 2063 726f 7373 5f6c 6179 6572  obs, cross_layer
-00008c60: 2c20 6475 725f 7073 6869 702c 2061 6374  , dur_pship, act
-00008c70: 732c 2061 6765 5f61 6374 5f70 6172 7329  s, age_act_pars)
-00008c80: 0a0a 2020 2020 2020 2020 2320 4170 706c  ..        # Appl
-00008c90: 7920 696e 7465 7276 656e 7469 6f6e 730a  y interventions.
-00008ca0: 2020 2020 2020 2020 666f 7220 692c 696e          for i,in
-00008cb0: 7465 7276 656e 7469 6f6e 2069 6e20 656e  tervention in en
-00008cc0: 756d 6572 6174 6528 7365 6c66 2e69 6e74  umerate(self.int
-00008cd0: 6572 7665 6e74 696f 6e73 293a 0a20 2020  erventions):.   
-00008ce0: 2020 2020 2020 2020 2069 6e74 6572 7665           interve
-00008cf0: 6e74 696f 6e28 7365 6c66 2920 2320 4966  ntion(self) # If
-00008d00: 2069 7427 7320 6120 6675 6e63 7469 6f6e   it's a function
-00008d10: 2c20 6361 6c6c 2069 7420 6469 7265 6374  , call it direct
-00008d20: 6c79 0a0a 2020 2020 2020 2020 2320 4173  ly..        # As
-00008d30: 7369 676e 2073 7573 5f69 6d6d 2076 616c  sign sus_imm val
-00008d40: 7565 732c 2069 2e65 2e20 7468 6520 7072  ues, i.e. the pr
-00008d50: 6f74 6563 7469 6f6e 2061 6761 696e 7374  otection against
-00008d60: 2069 6e66 6563 7469 6f6e 2062 6173 6564   infection based
-00008d70: 206f 6e20 7072 696f 7220 696d 6d75 6e65   on prior immune
-00008d80: 2068 6973 746f 7279 0a20 2020 2020 2020   history.       
-00008d90: 2069 6620 7365 6c66 5b27 7573 655f 7761   if self['use_wa
-00008da0: 6e69 6e67 275d 3a0a 2020 2020 2020 2020  ning']:.        
-00008db0: 2020 2020 696e 6473 203d 2068 7075 2e74      inds = hpu.t
-00008dc0: 7275 6528 7065 6f70 6c65 2e70 6561 6b5f  rue(people.peak_
-00008dd0: 696d 6d2e 7375 6d28 6178 6973 3d30 2929  imm.sum(axis=0))
-00008de0: 2e61 7374 7970 6528 6870 642e 6465 6661  .astype(hpd.defa
-00008df0: 756c 745f 696e 7429 0a20 2020 2020 2020  ult_int).       
-00008e00: 2020 2020 2069 6620 6c65 6e28 696e 6473       if len(inds
-00008e10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008e20: 2020 2073 7320 3d20 7065 6f70 6c65 2e74     ss = people.t
-00008e30: 5f69 6d6d 5f65 7665 6e74 5b3a 2c20 696e  _imm_event[:, in
-00008e40: 6473 5d2e 7368 6170 650a 2020 2020 2020  ds].shape.      
-00008e50: 2020 2020 2020 2020 2020 745f 7369 6e63            t_sinc
-00008e60: 655f 626f 6f73 7420 3d20 2874 202d 2070  e_boost = (t - p
-00008e70: 656f 706c 652e 745f 696d 6d5f 6576 656e  eople.t_imm_even
-00008e80: 745b 3a2c 696e 6473 5d29 2e72 6176 656c  t[:,inds]).ravel
-00008e90: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00008ea0: 2020 2063 7572 7265 6e74 5f69 6d6d 203d     current_imm =
-00008eb0: 2069 6d6d 5f6b 696e 5f70 6172 735b 745f   imm_kin_pars[t_
-00008ec0: 7369 6e63 655f 626f 6f73 745d 2e72 6573  since_boost].res
-00008ed0: 6861 7065 2873 7329 2023 2047 6574 2070  hape(ss) # Get p
-00008ee0: 656f 706c 6527 7320 6375 7272 656e 7420  eople's current 
-00008ef0: 6c65 7665 6c20 6f66 2069 6d6d 756e 6974  level of immunit
-00008f00: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00008f10: 2020 7065 6f70 6c65 2e6e 6162 5f69 6d6d    people.nab_imm
-00008f20: 5b3a 2c69 6e64 735d 203d 2063 7572 7265  [:,inds] = curre
-00008f30: 6e74 5f69 6d6d 2a70 656f 706c 652e 7065  nt_imm*people.pe
-00008f40: 616b 5f69 6d6d 5b3a 2c69 6e64 735d 2023  ak_imm[:,inds] #
-00008f50: 2053 6574 2069 6d6d 756e 6974 7920 7265   Set immunity re
-00008f60: 6c61 7469 7665 2074 6f20 7065 616b 0a20  lative to peak. 
-00008f70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008f80: 2020 2020 2020 2020 2070 656f 706c 652e           people.
-00008f90: 6e61 625f 696d 6d5b 3a5d 203d 2070 656f  nab_imm[:] = peo
-00008fa0: 706c 652e 7065 616b 5f69 6d6d 0a20 2020  ple.peak_imm.   
-00008fb0: 2020 2020 2068 7069 6d6d 2e63 6865 636b       hpimm.check
-00008fc0: 5f69 6d6d 756e 6974 7928 7065 6f70 6c65  _immunity(people
-00008fd0: 290a 0a20 2020 2020 2020 2023 2053 686f  )..        # Sho
-00008fe0: 7274 656e 206d 6f72 6520 7661 7269 6162  rten more variab
-00008ff0: 6c65 730a 2020 2020 2020 2020 6765 6e5f  les.        gen_
-00009000: 6265 7461 7320 3d20 6e70 2e61 7272 6179  betas = np.array
-00009010: 285b 675b 2772 656c 5f62 6574 6127 5d20  ([g['rel_beta'] 
-00009020: 2a20 6265 7461 2066 6f72 2067 2069 6e20  * beta for g in 
-00009030: 6765 6e5f 7061 7273 2e76 616c 7565 7328  gen_pars.values(
-00009040: 295d 2c20 6474 7970 653d 6870 642e 6465  )], dtype=hpd.de
-00009050: 6661 756c 745f 666c 6f61 7429 0a20 2020  fault_float).   
-00009060: 2020 2020 2073 7573 5f69 6d6d 203d 2070       sus_imm = p
-00009070: 656f 706c 652e 7375 735f 696d 6d0a 2020  eople.sus_imm.  
-00009080: 2020 2020 2020 7265 6c5f 7375 7320 3d20        rel_sus = 
-00009090: 7065 6f70 6c65 2e72 656c 5f73 7573 0a0a  people.rel_sus..
-000090a0: 2020 2020 2020 2020 696e 6620 3d20 7065          inf = pe
-000090b0: 6f70 6c65 2e69 6e66 6563 7469 6f75 732e  ople.infectious.
-000090c0: 636f 7079 2829 2023 2063 616c 6375 6c61  copy() # calcula
-000090d0: 7465 2074 7261 6e73 6d69 7373 696f 6e20  te transmission 
-000090e0: 6261 7365 6420 6f6e 2069 6e66 6563 7469  based on infecti
-000090f0: 6f75 736e 6573 7320 6174 2073 7461 7274  ousness at start
-00009100: 206f 6620 7469 6d65 7374 6570 2069 2e65   of timestep i.e
-00009110: 2e20 736f 6d65 6f6e 6520 696e 6665 6374  . someone infect
-00009120: 6564 2069 6e20 6f6e 6520 6c61 7965 7220  ed in one layer 
-00009130: 6361 6e6e 6f74 2074 7261 6e73 6d69 7420  cannot transmit 
-00009140: 7468 6520 696e 6665 6374 696f 6e20 7669  the infection vi
-00009150: 6120 6120 6469 6666 6572 656e 7420 6c61  a a different la
-00009160: 7965 7220 696e 2074 6865 2073 616d 6520  yer in the same 
-00009170: 7469 6d65 7374 6570 0a0a 2020 2020 2020  timestep..      
-00009180: 2020 2320 4c6f 6f70 206f 7665 7220 6c61    # Loop over la
-00009190: 7965 7273 0a20 2020 2020 2020 2066 6f72  yers.        for
-000091a0: 206c 6b65 792c 206c 6179 6572 2069 6e20   lkey, layer in 
-000091b0: 7065 6f70 6c65 2e63 6f6e 7461 6374 732e  people.contacts.
-000091c0: 6974 656d 7328 293a 0a0a 2020 2020 2020  items():..      
-000091d0: 2020 2020 2020 7375 7320 3d20 7065 6f70        sus = peop
-000091e0: 6c65 2e73 7573 6365 7074 6962 6c65 2e63  le.susceptible.c
-000091f0: 6f70 7928 2920 2320 666f 7220 6561 6368  opy() # for each
-00009200: 206c 6179 6572 2c20 7570 6461 7465 2077   layer, update w
-00009210: 686f 2773 2073 7469 6c6c 2073 7573 6365  ho's still susce
-00009220: 7074 6962 6c65 0a0a 2020 2020 2020 2020  ptible..        
-00009230: 2020 2020 2320 5368 6f72 7465 6e20 7661      # Shorten va
-00009240: 7269 6162 6c65 730a 2020 2020 2020 2020  riables.        
-00009250: 2020 2020 6620 3d20 6c61 7965 725b 2766      f = layer['f
-00009260: 275d 0a20 2020 2020 2020 2020 2020 206d  '].            m
-00009270: 203d 206c 6179 6572 5b27 6d27 5d0a 2020   = layer['m'].  
-00009280: 2020 2020 2020 2020 2020 6163 7473 203d            acts =
-00009290: 206c 6179 6572 5b27 6163 7473 275d 202a   layer['acts'] *
-000092a0: 2064 740a 2020 2020 2020 2020 2020 2020   dt.            
-000092b0: 6672 6163 5f61 6374 732c 2077 686f 6c65  frac_acts, whole
-000092c0: 5f61 6374 7320 3d20 6e70 2e6d 6f64 6628  _acts = np.modf(
-000092d0: 6163 7473 290a 2020 2020 2020 2020 2020  acts).          
-000092e0: 2020 7768 6f6c 655f 6163 7473 203d 2077    whole_acts = w
-000092f0: 686f 6c65 5f61 6374 732e 6173 7479 7065  hole_acts.astype
-00009300: 2868 7064 2e64 6566 6175 6c74 5f69 6e74  (hpd.default_int
-00009310: 290a 2020 2020 2020 2020 2020 2020 6566  ).            ef
-00009320: 6665 6374 6976 655f 636f 6e64 6f6d 7320  fective_condoms 
-00009330: 3d20 6870 642e 6465 6661 756c 745f 666c  = hpd.default_fl
-00009340: 6f61 7428 636f 6e64 6f6d 735b 6c6b 6579  oat(condoms[lkey
-00009350: 5d20 2a20 6566 665f 636f 6e64 6f6d 7329  ] * eff_condoms)
-00009360: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00009370: 436f 6d70 7574 6520 7472 616e 736d 6973  Compute transmis
-00009380: 7369 6f6e 7320 6279 2067 656e 6f74 7970  sions by genotyp
-00009390: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-000093a0: 7220 6720 696e 2072 616e 6765 286e 6729  r g in range(ng)
-000093b0: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-000093c0: 2020 2066 5f73 6f75 7263 655f 696e 6473     f_source_inds
-000093d0: 203d 2028 696e 665b 675d 5b66 5d20 2620   = (inf[g][f] & 
-000093e0: 7375 735b 675d 5b6d 5d29 2e6e 6f6e 7a65  sus[g][m]).nonze
-000093f0: 726f 2829 5b30 5d20 2023 2067 6574 2066  ro()[0]  # get f
-00009400: 656d 616c 6520 736f 7572 6365 7320 7768  emale sources wh
-00009410: 6572 6520 6665 6d61 6c65 2070 6172 746e  ere female partn
-00009420: 6572 2069 7320 696e 6665 6374 696f 7573  er is infectious
-00009430: 2077 6974 6820 6765 6e6f 7479 7065 2061   with genotype a
-00009440: 6e64 206d 616c 6520 7061 7274 6e65 7220  nd male partner 
-00009450: 6973 2073 7573 6365 7074 6962 6c65 2074  is susceptible t
-00009460: 6f20 7468 6174 2067 656e 6f74 7970 650a  o that genotype.
-00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009480: 6d5f 736f 7572 6365 5f69 6e64 7320 3d20  m_source_inds = 
-00009490: 2869 6e66 5b67 5d5b 6d5d 2026 2073 7573  (inf[g][m] & sus
-000094a0: 5b67 5d5b 665d 292e 6e6f 6e7a 6572 6f28  [g][f]).nonzero(
-000094b0: 295b 305d 2020 2320 6765 7420 6d61 6c65  )[0]  # get male
-000094c0: 2073 6f75 7263 6573 2077 6865 7265 2074   sources where t
-000094d0: 6865 206d 616c 6520 7061 7274 6e65 7220  he male partner 
-000094e0: 6973 2069 6e66 6563 7469 6f75 7320 7769  is infectious wi
-000094f0: 7468 2067 656e 6f74 7970 6520 616e 6420  th genotype and 
-00009500: 7468 6520 6665 6d61 6c65 2070 6172 746e  the female partn
-00009510: 6572 2069 7320 7375 7363 6570 7469 626c  er is susceptibl
-00009520: 6520 746f 2074 6861 7420 6765 6e6f 7479  e to that genoty
-00009530: 7065 0a0a 2020 2020 2020 2020 2020 2020  pe..            
-00009540: 2020 2020 666f 695f 6672 6163 203d 2031      foi_frac = 1
-00009550: 202d 2066 7261 635f 6163 7473 202a 2067   - frac_acts * g
-00009560: 656e 5f62 6574 6173 5b67 5d20 2a20 7472  en_betas[g] * tr
-00009570: 616e 735b 3a2c 204e 6f6e 655d 202a 2028  ans[:, None] * (
-00009580: 3120 2d20 6566 6665 6374 6976 655f 636f  1 - effective_co
-00009590: 6e64 6f6d 7329 2020 2320 5072 6f62 6162  ndoms)  # Probab
-000095a0: 696c 6974 7920 6f66 206e 6f74 2067 6574  ility of not get
-000095b0: 7469 6e67 2069 6e66 6563 7465 6420 6672  ting infected fr
-000095c0: 6f6d 2061 6e79 2066 7261 6374 696f 6e61  om any fractiona
-000095d0: 6c20 6163 7473 0a20 2020 2020 2020 2020  l acts.         
-000095e0: 2020 2020 2020 2066 6f69 5f77 686f 6c65         foi_whole
-000095f0: 203d 2028 3120 2d20 6765 6e5f 6265 7461   = (1 - gen_beta
-00009600: 735b 675d 202a 2074 7261 6e73 5b3a 2c20  s[g] * trans[:, 
-00009610: 4e6f 6e65 5d20 2a20 2831 202d 2065 6666  None] * (1 - eff
-00009620: 6563 7469 7665 5f63 6f6e 646f 6d73 2929  ective_condoms))
-00009630: 202a 2a20 7768 6f6c 655f 6163 7473 2020   ** whole_acts  
-00009640: 2320 5072 6f62 6162 696c 6974 7920 6f66  # Probability of
-00009650: 206e 6f74 2067 6574 7469 6e67 2069 6e66   not getting inf
-00009660: 6563 7465 6420 6672 6f6d 2077 686f 6c65  ected from whole
-00009670: 2061 6374 730a 2020 2020 2020 2020 2020   acts.          
-00009680: 2020 2020 2020 666f 6920 3d20 2831 202d        foi = (1 -
-00009690: 2028 666f 695f 7768 6f6c 6520 2a20 666f   (foi_whole * fo
-000096a0: 695f 6672 6163 2929 2e61 7374 7970 6528  i_frac)).astype(
-000096b0: 6870 642e 6465 6661 756c 745f 666c 6f61  hpd.default_floa
-000096c0: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
-000096d0: 2020 2020 6469 7363 6f72 6461 6e74 5f70      discordant_p
-000096e0: 6169 7273 203d 205b 5b66 5f73 6f75 7263  airs = [[f_sourc
-000096f0: 655f 696e 6473 2c20 665b 665f 736f 7572  e_inds, f[f_sour
-00009700: 6365 5f69 6e64 735d 2c20 6d5b 665f 736f  ce_inds], m[f_so
-00009710: 7572 6365 5f69 6e64 735d 2c20 666f 695b  urce_inds], foi[
-00009720: 302c 3a5d 5d2c 0a20 2020 2020 2020 2020  0,:]],.         
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2020 2020 205b 6d5f 736f             [m_so
-00009750: 7572 6365 5f69 6e64 732c 206d 5b6d 5f73  urce_inds, m[m_s
-00009760: 6f75 7263 655f 696e 6473 5d2c 2066 5b6d  ource_inds], f[m
-00009770: 5f73 6f75 7263 655f 696e 6473 5d2c 2066  _source_inds], f
-00009780: 6f69 5b31 2c3a 5d5d 5d0a 0a20 2020 2020  oi[1,:]]]..     
-00009790: 2020 2020 2020 2020 2020 2023 2043 6f6d             # Com
-000097a0: 7075 7465 2074 7261 6e73 6d69 7373 6962  pute transmissib
-000097b0: 696c 6974 7920 666f 7220 6561 6368 2070  ility for each p
-000097c0: 6172 746e 6572 7368 6970 0a20 2020 2020  artnership.     
-000097d0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-000097e0: 7368 6970 5f69 6e64 732c 2073 6f75 7263  ship_inds, sourc
-000097f0: 6573 2c20 7461 7267 6574 732c 2074 6869  es, targets, thi
-00009800: 735f 666f 6920 696e 2064 6973 636f 7264  s_foi in discord
-00009810: 616e 745f 7061 6972 733a 0a20 2020 2020  ant_pairs:.     
-00009820: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00009830: 6574 6173 203d 2074 6869 735f 666f 695b  etas = this_foi[
-00009840: 7073 6869 705f 696e 6473 5d20 2a20 2831  pship_inds] * (1
-00009850: 2e20 2d20 7375 735f 696d 6d5b 672c 7461  . - sus_imm[g,ta
-00009860: 7267 6574 735d 2920 2a20 7265 6c5f 7375  rgets]) * rel_su
-00009870: 735b 7461 7267 6574 735d 2023 2050 756c  s[targets] # Pul
-00009880: 6c20 6f75 7420 7468 6520 7472 616e 736d  l out the transm
-00009890: 6973 7369 6269 6c69 7479 2061 7373 6f63  issibility assoc
-000098a0: 6961 7465 6420 7769 7468 2074 6869 7320  iated with this 
-000098b0: 7061 7274 6e65 7273 6869 700a 2020 2020  partnership.    
-000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098d0: 7472 616e 736d 6973 7369 6f6e 7320 3d20  transmissions = 
-000098e0: 286e 702e 7261 6e64 6f6d 2e72 616e 646f  (np.random.rando
-000098f0: 6d28 6c65 6e28 6265 7461 7329 2920 3c20  m(len(betas)) < 
-00009900: 6265 7461 7329 2e6e 6f6e 7a65 726f 2829  betas).nonzero()
-00009910: 5b30 5d20 2320 4170 706c 7920 7072 6f62  [0] # Apply prob
-00009920: 6162 696c 6974 6965 7320 746f 2064 6574  abilities to det
-00009930: 6572 6d69 6e65 2070 6172 746e 6572 7368  ermine partnersh
-00009940: 6970 7320 696e 2077 6869 6368 2074 7261  ips in which tra
-00009950: 6e73 6d69 7373 696f 6e20 6f63 6375 7272  nsmission occurr
-00009960: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
-00009970: 2020 2020 2020 2074 6172 6765 745f 696e         target_in
-00009980: 6473 2020 203d 2074 6172 6765 7473 5b74  ds   = targets[t
-00009990: 7261 6e73 6d69 7373 696f 6e73 5d20 2320  ransmissions] # 
-000099a0: 4578 7472 6163 7420 696e 6469 6365 7320  Extract indices 
-000099b0: 6f66 2074 686f 7365 2077 686f 2067 6f74  of those who got
-000099c0: 2069 6e66 6563 7465 640a 2020 2020 2020   infected.      
-000099d0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-000099e0: 7267 6574 5f69 6e64 732c 2075 6e69 7175  rget_inds, uniqu
-000099f0: 655f 696e 6473 203d 206e 702e 756e 6971  e_inds = np.uniq
-00009a00: 7565 2874 6172 6765 745f 696e 6473 2c20  ue(target_inds, 
-00009a10: 7265 7475 726e 5f69 6e64 6578 3d54 7275  return_index=Tru
-00009a20: 6529 2020 2320 4475 6520 746f 206d 756c  e)  # Due to mul
-00009a30: 7469 706c 6520 7061 7274 6e65 7273 6869  tiple partnershi
-00009a40: 7073 2c20 736f 6d65 2070 656f 706c 6520  ps, some people 
-00009a50: 7769 6c6c 2062 6520 636f 756e 7465 6420  will be counted 
-00009a60: 7477 6963 653b 2072 656d 6f76 6520 7468  twice; remove th
-00009a70: 656d 0a20 2020 2020 2020 2020 2020 2020  em.             
-00009a80: 2020 2020 2020 2070 656f 706c 652e 696e         people.in
-00009a90: 6665 6374 2869 6e64 733d 7461 7267 6574  fect(inds=target
-00009aa0: 5f69 6e64 732c 2067 3d67 2c20 6c61 7965  _inds, g=g, laye
-00009ab0: 723d 6c6b 6579 2920 2023 2049 6e66 6563  r=lkey)  # Infec
-00009ac0: 7420 7065 6f70 6c65 0a0a 2020 2020 2020  t people..      
-00009ad0: 2020 2320 4465 7465 726d 696e 6520 6966    # Determine if
-00009ae0: 2074 6865 7265 2061 7265 2061 6e79 2072   there are any r
-00009af0: 6561 6374 6976 6174 6564 2069 6e66 6563  eactivated infec
-00009b00: 7469 6f6e 7320 6f6e 2074 6869 7320 7469  tions on this ti
-00009b10: 6d65 7374 6570 0a20 2020 2020 2020 2066  mestep.        f
-00009b20: 6f72 2067 2069 6e20 7261 6e67 6528 6e67  or g in range(ng
-00009b30: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
-00009b40: 6174 656e 745f 696e 6473 203d 2068 7075  atent_inds = hpu
-00009b50: 2e74 7275 6528 7065 6f70 6c65 2e6c 6174  .true(people.lat
-00009b60: 656e 745b 672c 3a5d 290a 2020 2020 2020  ent[g,:]).      
-00009b70: 2020 2020 2020 6966 206c 656e 286c 6174        if len(lat
-00009b80: 656e 745f 696e 6473 293a 0a20 2020 2020  ent_inds):.     
-00009b90: 2020 2020 2020 2020 2020 2072 6561 6374             react
-00009ba0: 6976 6174 696f 6e5f 7072 6f62 7320 3d20  ivation_probs = 
-00009bb0: 6e70 2e66 756c 6c5f 6c69 6b65 286c 6174  np.full_like(lat
-00009bc0: 656e 745f 696e 6473 2c20 7365 6c66 5b27  ent_inds, self['
-00009bd0: 6870 765f 7265 6163 7469 7661 7469 6f6e  hpv_reactivation
-00009be0: 275d 202a 2064 742c 2064 7479 7065 3d68  '] * dt, dtype=h
-00009bf0: 7064 2e64 6566 6175 6c74 5f66 6c6f 6174  pd.default_float
-00009c00: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009c10: 2020 2023 2069 6620 7365 6c66 5b27 6d6f     # if self['mo
-00009c20: 6465 6c5f 6869 7627 5d3a 0a20 2020 2020  del_hiv']:.     
-00009c30: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00009c40: 2023 2064 6574 6572 6d69 6e65 2069 6620   # determine if 
-00009c50: 616e 7920 6f66 2074 6865 7365 2069 6e64  any of these ind
-00009c60: 7320 6861 7665 2048 4956 2061 6e64 2061  s have HIV and a
-00009c70: 646a 7573 7420 7468 6569 7220 7072 6f62  djust their prob
-00009c80: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00009c90: 2020 2320 2020 2020 6869 765f 6c61 7465    #     hiv_late
-00009ca0: 6e74 5f69 6e64 7320 3d20 6c61 7465 6e74  nt_inds = latent
-00009cb0: 5f69 6e64 735b 6870 752e 7472 7565 2870  _inds[hpu.true(p
-00009cc0: 656f 706c 652e 6869 765b 6c61 7465 6e74  eople.hiv[latent
-00009cd0: 5f69 6e64 735d 295d 0a20 2020 2020 2020  _inds])].       
-00009ce0: 2020 2020 2020 2020 2023 2020 2020 2069           #     i
-00009cf0: 6620 6c65 6e28 6869 765f 6c61 7465 6e74  f len(hiv_latent
-00009d00: 5f69 6e64 7329 3a0a 2020 2020 2020 2020  _inds):.        
-00009d10: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00009d20: 2020 696d 6d75 6e65 5f63 6f6d 7072 6f6d    immune_comprom
-00009d30: 6973 6520 3d20 3120 2d20 7065 6f70 6c65  ise = 1 - people
-00009d40: 2e61 7274 5f61 6468 6572 656e 6365 5b68  .art_adherence[h
-00009d50: 6976 5f6c 6174 656e 745f 696e 6473 5d0a  iv_latent_inds].
-00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d70: 2320 2020 2020 2020 2020 6d6f 6420 3d20  #         mod = 
-00009d80: 696d 6d75 6e65 5f63 6f6d 7072 6f6d 6973  immune_compromis
-00009d90: 6520 2a20 7365 6c66 5b27 6869 765f 7061  e * self['hiv_pa
-00009da0: 7273 275d 5b27 7265 6163 7469 7661 7469  rs']['reactivati
-00009db0: 6f6e 5f70 726f 6227 5d0a 2020 2020 2020  on_prob'].      
-00009dc0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00009dd0: 2020 2020 6d6f 645b 6d6f 6420 3c20 315d      mod[mod < 1]
-00009de0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
-00009df0: 2020 2020 2023 2020 2020 2020 2020 2072       #         r
-00009e00: 6561 6374 6976 6174 696f 6e5f 7072 6f62  eactivation_prob
-00009e10: 735b 6870 752e 7472 7565 2870 656f 706c  s[hpu.true(peopl
-00009e20: 652e 6869 765b 6c61 7465 6e74 5f69 6e64  e.hiv[latent_ind
-00009e30: 735d 295d 202a 3d20 6d6f 640a 2020 2020  s])] *= mod.    
-00009e40: 2020 2020 2020 2020 2020 2020 6973 5f72              is_r
-00009e50: 6561 6374 6976 6174 6564 203d 2068 7075  eactivated = hpu
-00009e60: 2e62 696e 6f6d 6961 6c5f 6172 7228 7265  .binomial_arr(re
-00009e70: 6163 7469 7661 7469 6f6e 5f70 726f 6273  activation_probs
-00009e80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009e90: 2020 7265 6163 7469 7661 7465 645f 696e    reactivated_in
-00009ea0: 6473 203d 206c 6174 656e 745f 696e 6473  ds = latent_inds
-00009eb0: 5b69 735f 7265 6163 7469 7661 7465 645d  [is_reactivated]
-00009ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ed0: 2070 656f 706c 652e 696e 6665 6374 2869   people.infect(i
-00009ee0: 6e64 733d 7265 6163 7469 7661 7465 645f  nds=reactivated_
-00009ef0: 696e 6473 2c20 673d 672c 206c 6179 6572  inds, g=g, layer
-00009f00: 3d27 7265 6163 7469 7661 7469 6f6e 2729  ='reactivation')
-00009f10: 0a0a 2020 2020 2020 2020 2320 496e 6465  ..        # Inde
-00009f20: 7820 666f 7220 7265 7375 6c74 730a 2020  x for results.  
-00009f30: 2020 2020 2020 6964 7820 3d20 696e 7428        idx = int(
-00009f40: 7420 2f20 7365 6c66 2e72 6573 6672 6571  t / self.resfreq
-00009f50: 290a 0a20 2020 2020 2020 2023 2055 7064  )..        # Upd
-00009f60: 6174 6520 636f 756e 7473 2066 6f72 2074  ate counts for t
-00009f70: 6869 7320 7469 6d65 2073 7465 703a 2066  his time step: f
-00009f80: 6c6f 7773 0a20 2020 2020 2020 2066 6f72  lows.        for
-00009f90: 206b 6579 2c63 6f75 6e74 2069 6e20 7065   key,count in pe
-00009fa0: 6f70 6c65 2e66 6c6f 7773 2e69 7465 6d73  ople.flows.items
-00009fb0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00009fc0: 7365 6c66 2e72 6573 756c 7473 5b6b 6579  self.results[key
-00009fd0: 5d5b 6964 785d 202b 3d20 636f 756e 740a  ][idx] += count.
-00009fe0: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-00009ff0: 636f 756e 7420 696e 2070 656f 706c 652e  count in people.
-0000a000: 6465 6d6f 6772 6170 6869 635f 666c 6f77  demographic_flow
-0000a010: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
-0000a020: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-0000a030: 6c74 735b 6b65 795d 5b69 6478 5d20 2b3d  lts[key][idx] +=
-0000a040: 2063 6f75 6e74 0a20 2020 2020 2020 2066   count.        f
-0000a050: 6f72 206b 6579 2c63 6f75 6e74 2069 6e20  or key,count in 
-0000a060: 7065 6f70 6c65 2e67 656e 6f74 7970 655f  people.genotype_
-0000a070: 666c 6f77 732e 6974 656d 7328 293a 0a20  flows.items():. 
-0000a080: 2020 2020 2020 2020 2020 2066 6c6f 775f             flow_
-0000a090: 696e 6420 3d20 5b66 6c6f 772e 6e61 6d65  ind = [flow.name
-0000a0a0: 2066 6f72 2066 6c6f 7720 696e 2068 7064   for flow in hpd
-0000a0b0: 2e66 6c6f 7773 5d2e 696e 6465 7828 6b65  .flows].index(ke
-0000a0c0: 7929 0a20 2020 2020 2020 2020 2020 2069  y).            i
-0000a0d0: 6620 6870 642e 666c 6f77 735b 666c 6f77  f hpd.flows[flow
-0000a0e0: 5f69 6e64 5d2e 6279 5f67 656e 6f74 7970  _ind].by_genotyp
-0000a0f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000a100: 2020 2066 6f72 2067 656e 6f74 7970 6520     for genotype 
-0000a110: 696e 2072 616e 6765 286e 6729 3a0a 2020  in range(ng):.  
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 2020 7365 6c66 2e72 6573 756c 7473 5b6b    self.results[k
-0000a140: 6579 2b27 5f62 795f 6765 6e6f 7479 7065  ey+'_by_genotype
-0000a150: 275d 5b67 656e 6f74 7970 655d 5b69 6478  '][genotype][idx
-0000a160: 5d20 2b3d 2063 6f75 6e74 5b67 656e 6f74  ] += count[genot
-0000a170: 7970 655d 0a20 2020 2020 2020 2066 6f72  ype].        for
-0000a180: 206b 6579 2c63 6f75 6e74 2069 6e20 7065   key,count in pe
-0000a190: 6f70 6c65 2e73 6578 5f66 6c6f 7773 2e69  ople.sex_flows.i
-0000a1a0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0000a1b0: 2020 2020 666f 7220 7365 7820 696e 2072      for sex in r
-0000a1c0: 616e 6765 2832 293a 0a20 2020 2020 2020  ange(2):.       
-0000a1d0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000a1e0: 7375 6c74 735b 6b65 795d 5b73 6578 5d5b  sults[key][sex][
-0000a1f0: 6964 785d 202b 3d20 636f 756e 745b 7365  idx] += count[se
-0000a200: 785d 0a20 2020 2020 2020 2066 6f72 206b  x].        for k
-0000a210: 6579 2c63 6f75 6e74 2069 6e20 7065 6f70  ey,count in peop
-0000a220: 6c65 2e61 6765 5f66 6c6f 7773 2e69 7465  le.age_flows.ite
-0000a230: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000a240: 2020 7365 6c66 2e72 6573 756c 7473 5b6b    self.results[k
-0000a250: 6579 2b27 5f62 795f 6167 6527 5d5b 3a2c  ey+'_by_age'][:,
-0000a260: 6964 785d 202b 3d20 636f 756e 740a 0a20  idx] += count.. 
-0000a270: 2020 2020 2020 2023 204d 616b 6520 7374         # Make st
-0000a280: 6f63 6b20 7570 6461 7465 7320 6576 6572  ock updates ever
-0000a290: 7920 6e74 6820 7374 6570 2c20 7768 6572  y nth step, wher
-0000a2a0: 6520 6e20 6973 2074 6865 2066 7265 7175  e n is the frequ
-0000a2b0: 656e 6379 206f 6620 7265 7375 6c74 206f  ency of result o
-0000a2c0: 7574 7075 740a 2020 2020 2020 2020 6966  utput.        if
-0000a2d0: 2074 2025 2073 656c 662e 7265 7366 7265   t % self.resfre
-0000a2e0: 7120 3d3d 2073 656c 662e 7265 7366 7265  q == self.resfre
-0000a2f0: 712d 313a 0a0a 2020 2020 2020 2020 2020  q-1:..          
-0000a300: 2020 2320 4e75 6d62 6572 2069 6e66 6563    # Number infec
-0000a310: 7469 6f75 732f 7375 7363 6570 7469 626c  tious/susceptibl
-0000a320: 6520 6279 2061 6765 2c20 666f 7220 7072  e by age, for pr
-0000a330: 6576 616c 656e 6365 2063 616c 6375 6c61  evalence calcula
-0000a340: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
-0000a350: 2020 696e 6669 6e64 7320 3d20 6870 752e    infinds = hpu.
-0000a360: 7472 7565 2870 656f 706c 655b 2769 6e66  true(people['inf
-0000a370: 6563 7469 6f75 7327 5d29 0a20 2020 2020  ectious']).     
-0000a380: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-0000a390: 6c74 735b 6627 6e5f 696e 6665 6374 696f  lts[f'n_infectio
-0000a3a0: 7573 5f62 795f 6167 6527 5d5b 3a2c 2069  us_by_age'][:, i
-0000a3b0: 6478 5d20 3d20 6e70 2e68 6973 746f 6772  dx] = np.histogr
-0000a3c0: 616d 2870 656f 706c 652e 6167 655b 696e  am(people.age[in
-0000a3d0: 6669 6e64 735d 2c20 6269 6e73 3d70 656f  finds], bins=peo
-0000a3e0: 706c 652e 6167 655f 6269 6e73 2c20 7765  ple.age_bins, we
-0000a3f0: 6967 6874 733d 7065 6f70 6c65 2e73 6361  ights=people.sca
-0000a400: 6c65 5b69 6e66 696e 6473 5d29 5b30 5d0a  le[infinds])[0].
-0000a410: 2020 2020 2020 2020 2020 2020 7375 7369              susi
-0000a420: 6e64 7320 3d20 6870 752e 7472 7565 2870  nds = hpu.true(p
-0000a430: 656f 706c 655b 2773 7573 6365 7074 6962  eople['susceptib
-0000a440: 6c65 275d 290a 2020 2020 2020 2020 2020  le']).          
-0000a450: 2020 7365 6c66 2e72 6573 756c 7473 5b66    self.results[f
-0000a460: 276e 5f73 7573 6365 7074 6962 6c65 5f62  'n_susceptible_b
-0000a470: 795f 6167 6527 5d5b 3a2c 2069 6478 5d20  y_age'][:, idx] 
-0000a480: 3d20 6e70 2e68 6973 746f 6772 616d 2870  = np.histogram(p
-0000a490: 656f 706c 652e 6167 655b 7375 7369 6e64  eople.age[susind
-0000a4a0: 735d 2c20 6269 6e73 3d70 656f 706c 652e  s], bins=people.
-0000a4b0: 6167 655f 6269 6e73 2c20 7765 6967 6874  age_bins, weight
-0000a4c0: 733d 7065 6f70 6c65 2e73 6361 6c65 5b73  s=people.scale[s
-0000a4d0: 7573 696e 6473 5d29 5b30 5d0a 2020 2020  usinds])[0].    
-0000a4e0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-0000a4f0: 6d65 6469 6e64 7320 3d20 6870 752e 7472  medinds = hpu.tr
-0000a500: 7565 2870 656f 706c 655b 2774 7261 6e73  ue(people['trans
-0000a510: 666f 726d 6564 275d 290a 2020 2020 2020  formed']).      
-0000a520: 2020 2020 2020 7365 6c66 2e72 6573 756c        self.resul
-0000a530: 7473 5b66 276e 5f74 7261 6e73 666f 726d  ts[f'n_transform
-0000a540: 6564 5f62 795f 6167 6527 5d5b 3a2c 2069  ed_by_age'][:, i
-0000a550: 6478 5d20 3d20 6e70 2e68 6973 746f 6772  dx] = np.histogr
-0000a560: 616d 2870 656f 706c 652e 6167 655b 7472  am(people.age[tr
-0000a570: 616e 7366 6f72 6d65 6469 6e64 735d 2c20  ansformedinds], 
-0000a580: 6269 6e73 3d70 656f 706c 652e 6167 655f  bins=people.age_
-0000a590: 6269 6e73 2c20 7765 6967 6874 733d 7065  bins, weights=pe
-0000a5a0: 6f70 6c65 2e73 6361 6c65 5b74 7261 6e73  ople.scale[trans
-0000a5b0: 666f 726d 6564 696e 6473 5d29 5b30 5d0a  formedinds])[0].
-0000a5c0: 2020 2020 2020 2020 2020 2020 7072 6563              prec
-0000a5d0: 696e 696e 6473 203d 2068 7075 2e74 7275  ininds = hpu.tru
-0000a5e0: 6528 7065 6f70 6c65 5b27 7072 6563 696e  e(people['precin
-0000a5f0: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
-0000a600: 7365 6c66 2e72 6573 756c 7473 5b66 276e  self.results[f'n
-0000a610: 5f70 7265 6369 6e5f 6279 5f61 6765 275d  _precin_by_age']
-0000a620: 5b3a 2c20 6964 785d 203d 206e 702e 6869  [:, idx] = np.hi
-0000a630: 7374 6f67 7261 6d28 7065 6f70 6c65 2e61  stogram(people.a
-0000a640: 6765 5b70 7265 6369 6e69 6e64 735d 2c20  ge[precininds], 
-0000a650: 6269 6e73 3d70 656f 706c 652e 6167 655f  bins=people.age_
-0000a660: 6269 6e73 2c20 7765 6967 6874 733d 7065  bins, weights=pe
-0000a670: 6f70 6c65 2e73 6361 6c65 5b70 7265 6369  ople.scale[preci
-0000a680: 6e69 6e64 735d 295b 305d 0a20 2020 2020  ninds])[0].     
-0000a690: 2020 2020 2020 2063 696e 3169 6e64 7320         cin1inds 
-0000a6a0: 3d20 6870 752e 7472 7565 2870 656f 706c  = hpu.true(peopl
-0000a6b0: 655b 2763 696e 3127 5d29 0a20 2020 2020  e['cin1']).     
-0000a6c0: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-0000a6d0: 6c74 735b 6627 6e5f 6369 6e31 5f62 795f  lts[f'n_cin1_by_
-0000a6e0: 6167 6527 5d5b 3a2c 2069 6478 5d20 3d20  age'][:, idx] = 
-0000a6f0: 6e70 2e68 6973 746f 6772 616d 2870 656f  np.histogram(peo
-0000a700: 706c 652e 6167 655b 6369 6e31 696e 6473  ple.age[cin1inds
-0000a710: 5d2c 2062 696e 733d 7065 6f70 6c65 2e61  ], bins=people.a
-0000a720: 6765 5f62 696e 732c 2077 6569 6768 7473  ge_bins, weights
-0000a730: 3d70 656f 706c 652e 7363 616c 655b 6369  =people.scale[ci
-0000a740: 6e31 696e 6473 5d29 5b30 5d0a 2020 2020  n1inds])[0].    
-0000a750: 2020 2020 2020 2020 6369 6e32 696e 6473          cin2inds
-0000a760: 203d 2068 7075 2e74 7275 6528 7065 6f70   = hpu.true(peop
-0000a770: 6c65 5b27 6369 6e32 275d 290a 2020 2020  le['cin2']).    
-0000a780: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-0000a790: 756c 7473 5b66 276e 5f63 696e 325f 6279  ults[f'n_cin2_by
-0000a7a0: 5f61 6765 275d 5b3a 2c20 6964 785d 203d  _age'][:, idx] =
-0000a7b0: 206e 702e 6869 7374 6f67 7261 6d28 7065   np.histogram(pe
-0000a7c0: 6f70 6c65 2e61 6765 5b63 696e 3269 6e64  ople.age[cin2ind
-0000a7d0: 735d 2c20 6269 6e73 3d70 656f 706c 652e  s], bins=people.
-0000a7e0: 6167 655f 6269 6e73 2c20 7765 6967 6874  age_bins, weight
-0000a7f0: 733d 7065 6f70 6c65 2e73 6361 6c65 5b63  s=people.scale[c
-0000a800: 696e 3269 6e64 735d 295b 305d 0a20 2020  in2inds])[0].   
-0000a810: 2020 2020 2020 2020 2063 696e 3369 6e64           cin3ind
-0000a820: 7320 3d20 6870 752e 7472 7565 2870 656f  s = hpu.true(peo
-0000a830: 706c 655b 2763 696e 3327 5d29 0a20 2020  ple['cin3']).   
-0000a840: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000a850: 7375 6c74 735b 6627 6e5f 6369 6e33 5f62  sults[f'n_cin3_b
-0000a860: 795f 6167 6527 5d5b 3a2c 2069 6478 5d20  y_age'][:, idx] 
-0000a870: 3d20 6e70 2e68 6973 746f 6772 616d 2870  = np.histogram(p
-0000a880: 656f 706c 652e 6167 655b 6369 6e33 696e  eople.age[cin3in
-0000a890: 6473 5d2c 2062 696e 733d 7065 6f70 6c65  ds], bins=people
-0000a8a0: 2e61 6765 5f62 696e 732c 2077 6569 6768  .age_bins, weigh
-0000a8b0: 7473 3d70 656f 706c 652e 7363 616c 655b  ts=people.scale[
-0000a8c0: 6369 6e33 696e 6473 5d29 5b30 5d0a 0a20  cin3inds])[0].. 
-0000a8d0: 2020 2020 2020 2020 2020 2023 2043 7265             # Cre
-0000a8e0: 6174 6520 746f 7461 6c20 7374 6f63 6b73  ate total stocks
-0000a8f0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000a900: 206b 6579 2069 6e20 7365 6c66 2e70 656f   key in self.peo
-0000a910: 706c 652e 6d65 7461 2e67 656e 6f74 7970  ple.meta.genotyp
-0000a920: 655f 7374 6f63 6b5f 6b65 7973 3a0a 0a20  e_stock_keys:.. 
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000a940: 2053 746f 636b 7320 6279 2067 656e 6f74   Stocks by genot
-0000a950: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
-0000a960: 2020 2020 666f 7220 6720 696e 2072 616e      for g in ran
-0000a970: 6765 286e 6729 3a0a 2020 2020 2020 2020  ge(ng):.        
-0000a980: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a990: 2e72 6573 756c 7473 5b66 276e 5f7b 6b65  .results[f'n_{ke
-0000a9a0: 797d 5f62 795f 6765 6e6f 7479 7065 275d  y}_by_genotype']
-0000a9b0: 5b67 2c20 6964 785d 203d 2070 656f 706c  [g, idx] = peopl
-0000a9c0: 652e 636f 756e 745f 6279 5f67 656e 6f74  e.count_by_genot
-0000a9d0: 7970 6528 6b65 792c 2067 290a 0a20 2020  ype(key, g)..   
-0000a9e0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-0000a9f0: 6f74 616c 2073 746f 636b 730a 2020 2020  otal stocks.    
-0000aa00: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-0000aa10: 6579 206e 6f74 2069 6e20 5b27 7375 7363  ey not in ['susc
-0000aa20: 6570 7469 626c 6527 5d3a 0a20 2020 2020  eptible']:.     
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000aa40: 2046 6f72 206e 5f69 6e66 6563 7469 6f75   For n_infectiou
-0000aa50: 7320 6574 632c 2077 6520 6765 7420 7468  s etc, we get th
-0000aa60: 6520 746f 7461 6c20 6e75 6d62 6572 2077  e total number w
-0000aa70: 6865 7265 2074 6869 7320 7374 6174 6520  here this state 
-0000aa80: 6973 2074 7275 6520 666f 7220 6174 206c  is true for at l
-0000aa90: 6561 7374 206f 6e65 2067 656e 6f74 7970  east one genotyp
-0000aaa0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000aab0: 2020 2020 2020 7365 6c66 2e72 6573 756c        self.resul
-0000aac0: 7473 5b66 276e 5f7b 6b65 797d 275d 5b69  ts[f'n_{key}'][i
-0000aad0: 6478 5d20 3d20 7065 6f70 6c65 2e63 6f75  dx] = people.cou
-0000aae0: 6e74 5f61 6e79 286b 6579 290a 2020 2020  nt_any(key).    
-0000aaf0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000ab00: 206b 6579 203d 3d20 2773 7573 6365 7074   key == 'suscept
-0000ab10: 6962 6c65 273a 0a20 2020 2020 2020 2020  ible':.         
-0000ab20: 2020 2020 2020 2020 2020 2023 2046 6f72             # For
-0000ab30: 206e 5f74 6f74 616c 5f73 7573 6365 7074   n_total_suscept
-0000ab40: 6962 6c65 2c20 7765 2067 6574 2074 6865  ible, we get the
-0000ab50: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
-0000ab60: 2069 6e66 6563 7469 6f6e 7320 7468 6174   infections that
-0000ab70: 2063 6f75 6c64 2074 6865 6f72 6574 6963   could theoretic
-0000ab80: 616c 6c79 2068 6170 7065 6e20 696e 2074  ally happen in t
-0000ab90: 6865 2070 6f70 756c 6174 696f 6e2c 2077  he population, w
-0000aba0: 6869 6368 2063 616e 2062 6520 6772 6561  hich can be grea
-0000abb0: 7465 7220 7468 616e 2074 6865 2070 6f70  ter than the pop
-0000abc0: 756c 6174 696f 6e20 7369 7a65 0a20 2020  ulation size.   
-0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abe0: 2073 656c 662e 7265 7375 6c74 735b 6627   self.results[f'
-0000abf0: 6e5f 7b6b 6579 7d27 5d5b 6964 785d 203d  n_{key}'][idx] =
-0000ac00: 2070 656f 706c 652e 636f 756e 7428 6b65   people.count(ke
-0000ac10: 7929 0a0a 2020 2020 2020 2020 2020 2020  y)..            
-0000ac20: 2320 4372 6561 7465 2073 746f 636b 7320  # Create stocks 
-0000ac30: 6f66 2069 6e74 6572 7665 6e74 696f 6e73  of interventions
-0000ac40: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000ac50: 206b 6579 2069 6e20 7365 6c66 2e70 656f   key in self.peo
-0000ac60: 706c 652e 6d65 7461 2e69 6e74 765f 7374  ple.meta.intv_st
-0000ac70: 6f63 6b5f 6b65 7973 3a0a 2020 2020 2020  ock_keys:.      
-0000ac80: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000ac90: 6573 756c 7473 5b66 276e 5f7b 6b65 797d  esults[f'n_{key}
-0000aca0: 275d 5b69 6478 5d20 3d20 7065 6f70 6c65  '][idx] = people
-0000acb0: 2e63 6f75 6e74 286b 6579 290a 0a20 2020  .count(key)..   
-0000acc0: 2020 2020 2020 2020 2023 2055 7064 6174           # Updat
-0000acd0: 6520 6361 6e63 6572 7320 616e 6420 6361  e cancers and ca
-0000ace0: 6e63 6572 7320 6279 2061 6765 0a20 2020  ncers by age.   
-0000acf0: 2020 2020 2020 2020 2063 6173 6573 5f62           cases_b
-0000ad00: 795f 6167 6520 3d20 7365 6c66 2e72 6573  y_age = self.res
-0000ad10: 756c 7473 5b27 6361 6e63 6572 735f 6279  ults['cancers_by
-0000ad20: 5f61 6765 275d 5b3a 2c20 6964 785d 0a20  _age'][:, idx]. 
-0000ad30: 2020 2020 2020 2020 2020 2069 6e64 7320             inds 
-0000ad40: 3d20 7065 6f70 6c65 2e61 6c69 7665 202a  = people.alive *
-0000ad50: 2028 7365 6c66 2e70 656f 706c 652e 7365   (self.people.se
-0000ad60: 783d 3d30 2920 2a20 7e70 656f 706c 652e  x==0) * ~people.
-0000ad70: 6361 6e63 6572 6f75 732e 616e 7928 6178  cancerous.any(ax
-0000ad80: 6973 3d30 290a 2020 2020 2020 2020 2020  is=0).          
-0000ad90: 2020 7661 6c73 203d 2073 656c 662e 7065    vals = self.pe
-0000ada0: 6f70 6c65 2e61 6765 5b69 6e64 735d 0a20  ople.age[inds]. 
-0000adb0: 2020 2020 2020 2020 2020 2062 696e 7320             bins 
-0000adc0: 3d20 7365 6c66 2e70 6172 735b 2773 7461  = self.pars['sta
-0000add0: 6e64 6172 645f 706f 7027 5d5b 302c 5d0a  ndard_pop'][0,].
-0000ade0: 2020 2020 2020 2020 2020 2020 7765 6967              weig
-0000adf0: 6874 7320 3d20 7065 6f70 6c65 2e73 6361  hts = people.sca
-0000ae00: 6c65 5b69 6e64 735d 0a20 2020 2020 2020  le[inds].       
-0000ae10: 2020 2020 2064 656e 6f6d 203d 206e 702e       denom = np.
-0000ae20: 6869 7374 6f67 7261 6d28 7661 6c73 2c20  histogram(vals, 
-0000ae30: 6269 6e73 2c20 7765 6967 6874 733d 7765  bins, weights=we
-0000ae40: 6967 6874 7329 5b30 5d0a 2020 2020 2020  ights)[0].      
-0000ae50: 2020 2020 2020 6167 655f 7370 6563 6966        age_specif
-0000ae60: 6963 5f69 6e63 6964 656e 6365 203d 2073  ic_incidence = s
-0000ae70: 632e 7361 6665 6469 7669 6465 2863 6173  c.safedivide(cas
-0000ae80: 6573 5f62 795f 6167 652c 2064 656e 6f6d  es_by_age, denom
-0000ae90: 292a 3130 3065 330a 2020 2020 2020 2020  )*100e3.        
-0000aea0: 2020 2020 7374 616e 6461 7264 5f70 6f70      standard_pop
-0000aeb0: 203d 2073 656c 662e 7061 7273 5b27 7374   = self.pars['st
-0000aec0: 616e 6461 7264 5f70 6f70 275d 5b31 2c20  andard_pop'][1, 
-0000aed0: 3a2d 315d 0a20 2020 2020 2020 2020 2020  :-1].           
-0000aee0: 2073 656c 662e 7265 7375 6c74 735b 2761   self.results['a
-0000aef0: 7372 5f63 616e 6365 725f 696e 6369 6465  sr_cancer_incide
-0000af00: 6e63 6527 5d5b 6964 785d 203d 206e 702e  nce'][idx] = np.
-0000af10: 646f 7428 6167 655f 7370 6563 6966 6963  dot(age_specific
-0000af20: 5f69 6e63 6964 656e 6365 2c73 7461 6e64  _incidence,stand
-0000af30: 6172 645f 706f 7029 0a0a 2020 2020 2020  ard_pop)..      
-0000af40: 2020 2020 2020 2320 5361 7665 206e 756d        # Save num
-0000af50: 6265 7220 616c 6976 650a 2020 2020 2020  ber alive.      
-0000af60: 2020 2020 2020 616c 6976 655f 696e 6473        alive_inds
-0000af70: 203d 2068 7075 2e74 7275 6528 7065 6f70   = hpu.true(peop
-0000af80: 6c65 2e61 6c69 7665 290a 2020 2020 2020  le.alive).      
-0000af90: 2020 2020 2020 616c 6976 655f 6665 6d61        alive_fema
-0000afa0: 6c65 5f69 6e64 7320 3d20 6870 752e 7472  le_inds = hpu.tr
-0000afb0: 7565 2870 656f 706c 652e 616c 6976 652a  ue(people.alive*
-0000afc0: 7065 6f70 6c65 2e69 735f 6665 6d61 6c65  people.is_female
-0000afd0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000afe0: 6c66 2e72 6573 756c 7473 5b27 6e5f 616c  lf.results['n_al
-0000aff0: 6976 6527 5d5b 6964 785d 203d 2070 656f  ive'][idx] = peo
-0000b000: 706c 652e 7363 616c 655f 666c 6f77 7328  ple.scale_flows(
-0000b010: 616c 6976 655f 696e 6473 290a 2020 2020  alive_inds).    
-0000b020: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-0000b030: 756c 7473 5b27 6e5f 616c 6976 655f 6279  ults['n_alive_by
-0000b040: 5f73 6578 275d 5b30 2c69 6478 5d20 3d20  _sex'][0,idx] = 
-0000b050: 7065 6f70 6c65 2e73 6361 6c65 5f66 6c6f  people.scale_flo
-0000b060: 7773 2828 7065 6f70 6c65 2e61 6c69 7665  ws((people.alive
-0000b070: 2a70 656f 706c 652e 6973 5f66 656d 616c  *people.is_femal
-0000b080: 6529 2e6e 6f6e 7a65 726f 2829 5b30 5d29  e).nonzero()[0])
-0000b090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b0a0: 662e 7265 7375 6c74 735b 276e 5f61 6c69  f.results['n_ali
-0000b0b0: 7665 5f62 795f 7365 7827 5d5b 312c 6964  ve_by_sex'][1,id
-0000b0c0: 785d 203d 2070 656f 706c 652e 7363 616c  x] = people.scal
-0000b0d0: 655f 666c 6f77 7328 2870 656f 706c 652e  e_flows((people.
-0000b0e0: 616c 6976 652a 7065 6f70 6c65 2e69 735f  alive*people.is_
-0000b0f0: 6d61 6c65 292e 6e6f 6e7a 6572 6f28 295b  male).nonzero()[
-0000b100: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0000b110: 7365 6c66 2e72 6573 756c 7473 5b27 6e5f  self.results['n_
-0000b120: 616c 6976 655f 6279 5f61 6765 275d 5b3a  alive_by_age'][:
-0000b130: 2c69 6478 5d20 3d20 6e70 2e68 6973 746f  ,idx] = np.histo
-0000b140: 6772 616d 2870 656f 706c 652e 6167 655b  gram(people.age[
-0000b150: 616c 6976 655f 696e 6473 5d2c 2062 696e  alive_inds], bin
-0000b160: 733d 7065 6f70 6c65 2e61 6765 5f62 696e  s=people.age_bin
-0000b170: 732c 2077 6569 6768 7473 3d70 656f 706c  s, weights=peopl
-0000b180: 652e 7363 616c 655b 616c 6976 655f 696e  e.scale[alive_in
-0000b190: 6473 5d29 5b30 5d0a 2020 2020 2020 2020  ds])[0].        
-0000b1a0: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
-0000b1b0: 5b27 6e5f 6665 6d61 6c65 735f 616c 6976  ['n_females_aliv
-0000b1c0: 655f 6279 5f61 6765 275d 5b3a 2c69 6478  e_by_age'][:,idx
-0000b1d0: 5d20 3d20 6e70 2e68 6973 746f 6772 616d  ] = np.histogram
-0000b1e0: 2870 656f 706c 652e 6167 655b 616c 6976  (people.age[aliv
-0000b1f0: 655f 6665 6d61 6c65 5f69 6e64 735d 2c20  e_female_inds], 
-0000b200: 6269 6e73 3d70 656f 706c 652e 6167 655f  bins=people.age_
-0000b210: 6269 6e73 2c20 7765 6967 6874 733d 7065  bins, weights=pe
-0000b220: 6f70 6c65 2e73 6361 6c65 5b61 6c69 7665  ople.scale[alive
-0000b230: 5f66 656d 616c 655f 696e 6473 5d29 5b30  _female_inds])[0
-0000b240: 5d0a 0a20 2020 2020 2020 2023 2041 7070  ]..        # App
-0000b250: 6c79 2061 6e61 6c79 7a65 7273 0a20 2020  ly analyzers.   
-0000b260: 2020 2020 2066 6f72 2069 2c61 6e61 6c79       for i,analy
-0000b270: 7a65 7220 696e 2065 6e75 6d65 7261 7465  zer in enumerate
-0000b280: 2873 656c 662e 616e 616c 797a 6572 7329  (self.analyzers)
-0000b290: 3a0a 2020 2020 2020 2020 2020 2020 616e  :.            an
-0000b2a0: 616c 797a 6572 2873 656c 6629 0a0a 2020  alyzer(self)..  
-0000b2b0: 2020 2020 2020 2320 5469 6479 2075 700a        # Tidy up.
-0000b2c0: 2020 2020 2020 2020 7365 6c66 2e74 202b          self.t +
-0000b2d0: 3d20 310a 2020 2020 2020 2020 6966 2073  = 1.        if s
-0000b2e0: 656c 662e 7420 3d3d 2073 656c 662e 6e70  elf.t == self.np
-0000b2f0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-0000b300: 7365 6c66 2e63 6f6d 706c 6574 6520 3d20  self.complete = 
-0000b310: 5472 7565 0a0a 2020 2020 2020 2020 7265  True..        re
-0000b320: 7475 726e 0a0a 0a20 2020 2064 6566 2072  turn...    def r
-0000b330: 756e 2873 656c 662c 2064 6f5f 706c 6f74  un(self, do_plot
-0000b340: 3d46 616c 7365 2c20 756e 7469 6c3d 4e6f  =False, until=No
-0000b350: 6e65 2c20 7265 7374 6f72 655f 7061 7273  ne, restore_pars
-0000b360: 3d54 7275 652c 2072 6573 6574 5f73 6565  =True, reset_see
-0000b370: 643d 5472 7565 2c20 7665 7262 6f73 653d  d=True, verbose=
-0000b380: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
-0000b390: 2727 2052 756e 2074 6865 206d 6f64 656c  '' Run the model
-0000b3a0: 206f 6e63 6520 2727 270a 2020 2020 2020   once '''.      
-0000b3b0: 2020 2320 496e 6974 6961 6c69 7a61 7469    # Initializati
-0000b3c0: 6f6e 2073 7465 7073 202d 2d20 7374 6172  on steps -- star
-0000b3d0: 7420 7468 6520 7469 6d65 722c 2069 6e69  t the timer, ini
-0000b3e0: 7469 616c 697a 6520 7468 6520 7369 6d20  tialize the sim 
-0000b3f0: 616e 6420 7468 6520 7365 6564 2c20 616e  and the seed, an
-0000b400: 6420 6368 6563 6b20 7468 6174 2074 6865  d check that the
-0000b410: 2073 696d 2068 6173 6e27 7420 6265 656e   sim hasn't been
-0000b420: 2072 756e 0a20 2020 2020 2020 2054 203d   run.        T =
-0000b430: 2073 632e 7469 6d65 7228 290a 0a20 2020   sc.timer()..   
-0000b440: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0000b450: 2e69 6e69 7469 616c 697a 6564 3a0a 2020  .initialized:.  
-0000b460: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-0000b470: 6e69 7469 616c 697a 6528 290a 2020 2020  nitialize().    
-0000b480: 2020 2020 2020 2020 7365 6c66 2e5f 6f72          self._or
-0000b490: 6967 5f70 6172 7320 3d20 7363 2e64 6370  ig_pars = sc.dcp
-0000b4a0: 2873 656c 662e 7061 7273 2920 2320 4372  (self.pars) # Cr
-0000b4b0: 6561 7465 2061 2063 6f70 7920 6f66 2074  eate a copy of t
-0000b4c0: 6865 2070 6172 616d 6574 6572 732c 2074  he parameters, t
-0000b4d0: 6f20 7265 7374 6f72 6520 6166 7465 7220  o restore after 
-0000b4e0: 7468 6520 7275 6e2c 2069 6e20 6361 7365  the run, in case
-0000b4f0: 2074 6865 7920 6172 6520 6479 6e61 6d69   they are dynami
-0000b500: 6361 6c6c 7920 6d6f 6469 6669 6564 0a0a  cally modified..
-0000b510: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-0000b520: 7365 2069 7320 4e6f 6e65 3a0a 2020 2020  se is None:.    
-0000b530: 2020 2020 2020 2020 7665 7262 6f73 6520          verbose 
-0000b540: 3d20 7365 6c66 5b27 7665 7262 6f73 6527  = self['verbose'
-0000b550: 5d0a 0a20 2020 2020 2020 2069 6620 7265  ]..        if re
-0000b560: 7365 745f 7365 6564 3a0a 2020 2020 2020  set_seed:.      
-0000b570: 2020 2020 2020 2320 5265 7365 7420 7468        # Reset th
-0000b580: 6520 524e 472e 2054 6865 2070 7269 6d61  e RNG. The prima
-0000b590: 7279 2075 7365 2063 6173 6520 2861 6e64  ry use case (and
-0000b5a0: 2077 6879 2069 7420 6465 6661 756c 7473   why it defaults
-0000b5b0: 2074 6f20 5472 7565 2920 6973 2074 6f20   to True) is to 
-0000b5c0: 656e 7375 7265 2074 6861 740a 2020 2020  ensure that.    
-0000b5d0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-0000b5e0: 2020 2020 2020 2320 3e3e 3e20 7369 6d30        # >>> sim0
-0000b5f0: 2e69 6e69 7469 616c 697a 6528 290a 2020  .initialize().  
-0000b600: 2020 2020 2020 2020 2020 2320 3e3e 3e20            # >>> 
-0000b610: 7369 6d30 2e72 756e 2829 0a20 2020 2020  sim0.run().     
-0000b620: 2020 2020 2020 2023 203e 3e3e 2073 696d         # >>> sim
-0000b630: 312e 696e 6974 6961 6c69 7a65 2829 0a20  1.initialize(). 
-0000b640: 2020 2020 2020 2020 2020 2023 203e 3e3e             # >>>
-0000b650: 2073 696d 312e 7275 6e28 290a 2020 2020   sim1.run().    
-0000b660: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-0000b670: 2020 2020 2020 2320 7072 6f64 7563 6573        # produces
-0000b680: 2074 6865 2073 616d 6520 6f75 7470 7574   the same output
-0000b690: 2061 730a 2020 2020 2020 2020 2020 2020   as.            
-0000b6a0: 230a 2020 2020 2020 2020 2020 2020 2320  #.            # 
-0000b6b0: 3e3e 3e20 7369 6d30 2e69 6e69 7469 616c  >>> sim0.initial
-0000b6c0: 697a 6528 290a 2020 2020 2020 2020 2020  ize().          
-0000b6d0: 2020 2320 3e3e 3e20 7369 6d31 2e69 6e69    # >>> sim1.ini
-0000b6e0: 7469 616c 697a 6528 290a 2020 2020 2020  tialize().      
-0000b6f0: 2020 2020 2020 2320 3e3e 3e20 7369 6d30        # >>> sim0
-0000b700: 2e72 756e 2829 0a20 2020 2020 2020 2020  .run().         
-0000b710: 2020 2023 203e 3e3e 2073 696d 312e 7275     # >>> sim1.ru
-0000b720: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-0000b730: 230a 2020 2020 2020 2020 2020 2020 2320  #.            # 
-0000b740: 5468 6520 7365 6564 2069 7320 6f66 6673  The seed is offs
-0000b750: 6574 2062 7920 3120 746f 2061 766f 6964  et by 1 to avoid
-0000b760: 2064 7261 7769 6e67 2074 6865 2073 616d   drawing the sam
-0000b770: 6520 7261 6e64 6f6d 206e 756d 6265 7273  e random numbers
-0000b780: 2061 7320 7468 6f73 6520 7573 6564 2066   as those used f
-0000b790: 6f72 2070 6f70 756c 6174 696f 6e20 6765  or population ge
-0000b7a0: 6e65 7261 7469 6f6e 2c20 6f74 6865 7277  neration, otherw
-0000b7b0: 6973 650a 2020 2020 2020 2020 2020 2020  ise.            
-0000b7c0: 2320 7468 6520 6669 7273 7420 7365 7420  # the first set 
-0000b7d0: 6f66 2072 616e 646f 6d20 6e75 6d62 6572  of random number
-0000b7e0: 7320 696e 2074 6865 206d 6f64 656c 2028  s in the model (
-0000b7f0: 652e 672e 2c20 6465 6174 6873 2920 7769  e.g., deaths) wi
-0000b800: 6c6c 2062 6520 636f 7272 656c 6174 6564  ll be correlated
-0000b810: 2077 6974 6820 7468 6520 6669 7273 7420   with the first 
-0000b820: 7365 7420 6f66 2072 616e 646f 6d20 6e75  set of random nu
-0000b830: 6d62 6572 730a 2020 2020 2020 2020 2020  mbers.          
-0000b840: 2020 2320 6472 6177 6e20 696e 2070 6f70    # drawn in pop
-0000b850: 756c 6174 696f 6e20 6765 6e65 7261 7469  ulation generati
-0000b860: 6f6e 2028 652e 672e 2c20 7365 7829 0a20  on (e.g., sex). 
-0000b870: 2020 2020 2020 2020 2020 2068 7075 2e73             hpu.s
-0000b880: 6574 5f73 6565 6428 7365 6c66 5b27 7261  et_seed(self['ra
-0000b890: 6e64 5f73 6565 6427 5d2b 3129 0a0a 2020  nd_seed']+1)..  
-0000b8a0: 2020 2020 2020 2320 4368 6563 6b20 666f        # Check fo
-0000b8b0: 7220 416c 7265 6164 7952 756e 2065 7272  r AlreadyRun err
-0000b8c0: 6f72 730a 2020 2020 2020 2020 6572 726f  ors.        erro
-0000b8d0: 726d 7367 203d 204e 6f6e 650a 2020 2020  rmsg = None.    
-0000b8e0: 2020 2020 756e 7469 6c20 3d20 7365 6c66      until = self
-0000b8f0: 2e6e 7074 7320 6966 2075 6e74 696c 2069  .npts if until i
-0000b900: 7320 4e6f 6e65 2065 6c73 6520 7365 6c66  s None else self
-0000b910: 2e67 6574 5f74 2875 6e74 696c 290a 2020  .get_t(until).  
-0000b920: 2020 2020 2020 6966 2075 6e74 696c 203e        if until >
-0000b930: 2073 656c 662e 6e70 7473 3a0a 2020 2020   self.npts:.    
-0000b940: 2020 2020 2020 2020 6572 726f 726d 7367          errormsg
-0000b950: 203d 2066 2752 6571 7565 7374 6564 2074   = f'Requested t
-0000b960: 6f20 7275 6e20 756e 7469 6c20 743d 7b75  o run until t={u
-0000b970: 6e74 696c 7d20 6275 7420 7468 6520 7369  ntil} but the si
-0000b980: 6d75 6c61 7469 6f6e 2065 6e64 2069 7320  mulation end is 
-0000b990: 743d 7b73 656c 662e 6e70 7473 7d27 0a20  t={self.npts}'. 
-0000b9a0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-0000b9b0: 203e 3d20 756e 7469 6c3a 2023 204e 422e   >= until: # NB.
-0000b9c0: 2041 7420 7468 6520 7374 6172 742c 2073   At the start, s
-0000b9d0: 656c 662e 7420 6973 204e 6f6e 6520 736f  elf.t is None so
-0000b9e0: 2074 6869 7320 6368 6563 6b20 6d75 7374   this check must
-0000b9f0: 206f 6363 7572 2061 6674 6572 2069 6e69   occur after ini
-0000ba00: 7469 616c 697a 6174 696f 6e0a 2020 2020  tialization.    
-0000ba10: 2020 2020 2020 2020 6572 726f 726d 7367          errormsg
-0000ba20: 203d 2066 2753 696d 756c 6174 696f 6e20   = f'Simulation 
-0000ba30: 6973 2063 7572 7265 6e74 6c79 2061 7420  is currently at 
-0000ba40: 743d 7b73 656c 662e 747d 2c20 7265 7175  t={self.t}, requ
-0000ba50: 6573 7465 6420 746f 2072 756e 2075 6e74  ested to run unt
-0000ba60: 696c 2074 3d7b 756e 7469 6c7d 2077 6869  il t={until} whi
-0000ba70: 6368 2068 6173 2061 6c72 6561 6479 2062  ch has already b
-0000ba80: 6565 6e20 7265 6163 6865 6427 0a20 2020  een reached'.   
-0000ba90: 2020 2020 2069 6620 7365 6c66 2e63 6f6d       if self.com
-0000baa0: 706c 6574 653a 0a20 2020 2020 2020 2020  plete:.         
-0000bab0: 2020 2065 7272 6f72 6d73 6720 3d20 2753     errormsg = 'S
-0000bac0: 696d 756c 6174 696f 6e20 6973 2061 6c72  imulation is alr
-0000bad0: 6561 6479 2063 6f6d 706c 6574 6520 2863  eady complete (c
-0000bae0: 616c 6c20 7369 6d2e 696e 6974 6961 6c69  all sim.initiali
-0000baf0: 7a65 2829 2074 6f20 7265 2d72 756e 2927  ze() to re-run)'
-0000bb00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000bb10: 2e70 656f 706c 652e 7420 6e6f 7420 696e  .people.t not in
-0000bb20: 205b 7365 6c66 2e74 2c20 7365 6c66 2e74   [self.t, self.t
-0000bb30: 2d31 5d3a 2023 2044 6570 656e 6469 6e67  -1]: # Depending
-0000bb40: 206f 6e20 686f 7720 7468 6520 7369 6d20   on how the sim 
-0000bb50: 7374 6f70 7065 642c 2065 6974 6865 7220  stopped, either 
-0000bb60: 6f66 2074 6865 7365 2073 7461 7465 7320  of these states 
-0000bb70: 6172 6520 706f 7373 6962 6c65 0a20 2020  are possible.   
-0000bb80: 2020 2020 2020 2020 2065 7272 6f72 6d73           errorms
-0000bb90: 6720 3d20 6627 5468 6520 7369 6d75 6c61  g = f'The simula
-0000bba0: 7469 6f6e 2068 6173 2062 6565 6e20 7275  tion has been ru
-0000bbb0: 6e20 696e 6465 7065 6e64 656e 746c 7920  n independently 
-0000bbc0: 6672 6f6d 2074 6865 2070 656f 706c 6520  from the people 
-0000bbd0: 2874 3d7b 7365 6c66 2e74 7d2c 2070 656f  (t={self.t}, peo
-0000bbe0: 706c 652e 743d 7b73 656c 662e 7065 6f70  ple.t={self.peop
-0000bbf0: 6c65 2e74 7d29 3a20 6966 2074 6869 7320  le.t}): if this 
-0000bc00: 6973 2069 6e74 656e 7469 6f6e 616c 2c20  is intentional, 
-0000bc10: 6d61 6e75 616c 6c79 2073 6574 2073 696d  manually set sim
-0000bc20: 2e70 656f 706c 652e 7420 3d20 7369 6d2e  .people.t = sim.
-0000bc30: 742e 2052 656d 656d 6265 7220 746f 2073  t. Remember to s
-0000bc40: 6176 6520 7468 6520 7065 6f70 6c65 206f  ave the people o
-0000bc50: 626a 6563 7420 6265 666f 7265 2072 756e  bject before run
-0000bc60: 6e69 6e67 2074 6865 2073 696d 2e27 0a20  ning the sim.'. 
-0000bc70: 2020 2020 2020 2069 6620 6572 726f 726d         if errorm
-0000bc80: 7367 3a0a 2020 2020 2020 2020 2020 2020  sg:.            
-0000bc90: 7261 6973 6520 416c 7265 6164 7952 756e  raise AlreadyRun
-0000bca0: 4572 726f 7228 6572 726f 726d 7367 290a  Error(errormsg).
-0000bcb0: 0a20 2020 2020 2020 2023 204d 6169 6e20  .        # Main 
-0000bcc0: 7369 6d75 6c61 7469 6f6e 206c 6f6f 700a  simulation loop.
-0000bcd0: 2020 2020 2020 2020 7768 696c 6520 7365          while se
-0000bce0: 6c66 2e74 203c 2075 6e74 696c 3a0a 0a20  lf.t < until:.. 
-0000bcf0: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
-0000bd00: 636b 2069 6620 7765 2077 6572 6520 6173  ck if we were as
-0000bd10: 6b65 6420 746f 2073 746f 700a 2020 2020  ked to stop.    
-0000bd20: 2020 2020 2020 2020 656c 6170 7365 6420          elapsed 
-0000bd30: 3d20 542e 746f 6328 6f75 7470 7574 3d54  = T.toc(output=T
-0000bd40: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0000bd50: 2069 6620 7365 6c66 5b27 7469 6d65 6c69   if self['timeli
-0000bd60: 6d69 7427 5d20 616e 6420 656c 6170 7365  mit'] and elapse
-0000bd70: 6420 3e20 7365 6c66 5b27 7469 6d65 6c69  d > self['timeli
-0000bd80: 6d69 7427 5d3a 0a20 2020 2020 2020 2020  mit']:.         
-0000bd90: 2020 2020 2020 2073 632e 7072 696e 7476         sc.printv
-0000bda0: 2866 2254 696d 6520 6c69 6d69 7420 287b  (f"Time limit ({
-0000bdb0: 7365 6c66 5b27 7469 6d65 6c69 6d69 7427  self['timelimit'
-0000bdc0: 5d7d 2073 2920 6578 6365 6564 6564 3b20  ]} s) exceeded; 
-0000bdd0: 6361 6c6c 2073 696d 2e66 696e 616c 697a  call sim.finaliz
-0000bde0: 6528 2920 746f 2063 6f6d 7075 7465 2072  e() to compute r
-0000bdf0: 6573 756c 7473 2069 6620 6465 7369 7265  esults if desire
-0000be00: 6422 2c20 312c 2076 6572 626f 7365 290a  d", 1, verbose).
-0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-0000be30: 2020 2065 6c69 6620 7365 6c66 5b27 7374     elif self['st
-0000be40: 6f70 7069 6e67 5f66 756e 6327 5d20 616e  opping_func'] an
-0000be50: 6420 7365 6c66 5b27 7374 6f70 7069 6e67  d self['stopping
-0000be60: 5f66 756e 6327 5d28 7365 6c66 293a 0a20  _func'](self):. 
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000be80: 632e 7072 696e 7476 2822 5374 6f70 7069  c.printv("Stoppi
-0000be90: 6e67 2066 756e 6374 696f 6e20 7465 726d  ng function term
-0000bea0: 696e 6174 6564 2074 6865 2073 696d 756c  inated the simul
-0000beb0: 6174 696f 6e3b 2063 616c 6c20 7369 6d2e  ation; call sim.
-0000bec0: 6669 6e61 6c69 7a65 2829 2074 6f20 636f  finalize() to co
-0000bed0: 6d70 7574 6520 7265 7375 6c74 7320 6966  mpute results if
-0000bee0: 2064 6573 6972 6564 222c 2031 2c20 7665   desired", 1, ve
-0000bef0: 7262 6f73 6529 0a20 2020 2020 2020 2020  rbose).         
-0000bf00: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-0000bf10: 2020 2020 2020 2020 2020 2023 2050 7269             # Pri
-0000bf20: 6e74 2070 726f 6772 6573 730a 2020 2020  nt progress.    
-0000bf30: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-0000bf40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000bf50: 2020 2020 7369 6d6c 6162 656c 203d 2066      simlabel = f
-0000bf60: 2722 7b73 656c 662e 6c61 6265 6c7d 223a  '"{self.label}":
-0000bf70: 2027 2069 6620 7365 6c66 2e6c 6162 656c   ' if self.label
-0000bf80: 2065 6c73 6520 2727 0a20 2020 2020 2020   else ''.       
-0000bf90: 2020 2020 2020 2020 2073 7472 696e 6720           string 
-0000bfa0: 3d20 6627 2020 5275 6e6e 696e 6720 7b73  = f'  Running {s
-0000bfb0: 696d 6c61 6265 6c7d 7b73 656c 662e 7965  imlabel}{self.ye
-0000bfc0: 6172 7665 635b 7365 6c66 2e74 5d3a 302e  arvec[self.t]:0.
-0000bfd0: 3166 7d20 287b 7365 6c66 2e74 3a32 2e30  1f} ({self.t:2.0
-0000bfe0: 667d 2f7b 7365 6c66 2e6e 7074 737d 2920  f}/{self.npts}) 
-0000bff0: 287b 656c 6170 7365 643a 302e 3266 7d20  ({elapsed:0.2f} 
-0000c000: 7329 2027 0a20 2020 2020 2020 2020 2020  s) '.           
-0000c010: 2020 2020 2069 6620 7665 7262 6f73 6520       if verbose 
-0000c020: 3e3d 2032 3a0a 2020 2020 2020 2020 2020  >= 2:.          
-0000c030: 2020 2020 2020 2020 2020 7363 2e68 6561            sc.hea
-0000c040: 6469 6e67 2873 7472 696e 6729 0a20 2020  ding(string).   
-0000c050: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-0000c060: 6620 7665 7262 6f73 653e 303a 0a20 2020  f verbose>0:.   
-0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c080: 2069 6620 6e6f 7420 2873 656c 662e 7420   if not (self.t 
-0000c090: 2520 696e 7428 312e 302f 7665 7262 6f73  % int(1.0/verbos
-0000c0a0: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
-0000c0b0: 2020 2020 2020 2020 2020 2020 2073 632e               sc.
-0000c0c0: 7072 6f67 7265 7373 6261 7228 7365 6c66  progressbar(self
-0000c0d0: 2e74 2b31 2c20 7365 6c66 2e6e 7074 732c  .t+1, self.npts,
-0000c0e0: 206c 6162 656c 3d73 7472 696e 672c 206c   label=string, l
-0000c0f0: 656e 6774 683d 3230 2c20 6e65 776c 696e  ength=20, newlin
-0000c100: 653d 5472 7565 290a 0a20 2020 2020 2020  e=True)..       
-0000c110: 2020 2020 2023 2044 6f20 7468 6520 6865       # Do the he
-0000c120: 6176 7920 6c69 6674 696e 6720 2d2d 2061  avy lifting -- a
-0000c130: 6374 7561 6c6c 7920 7275 6e20 7468 6520  ctually run the 
-0000c140: 6d6f 6465 6c21 0a20 2020 2020 2020 2020  model!.         
-0000c150: 2020 2073 656c 662e 7374 6570 2829 0a0a     self.step()..
-0000c160: 2020 2020 2020 2020 2320 4966 2073 696d          # If sim
-0000c170: 756c 6174 696f 6e20 7265 6163 6865 6420  ulation reached 
-0000c180: 7468 6520 656e 642c 2066 696e 616c 697a  the end, finaliz
-0000c190: 6520 7468 6520 7265 7375 6c74 730a 2020  e the results.  
-0000c1a0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-0000c1b0: 6d70 6c65 7465 3a0a 2020 2020 2020 2020  mplete:.        
-0000c1c0: 2020 2020 7365 6c66 2e66 696e 616c 697a      self.finaliz
-0000c1d0: 6528 7665 7262 6f73 653d 7665 7262 6f73  e(verbose=verbos
-0000c1e0: 652c 2072 6573 746f 7265 5f70 6172 733d  e, restore_pars=
-0000c1f0: 7265 7374 6f72 655f 7061 7273 290a 2020  restore_pars).  
-0000c200: 2020 2020 2020 2020 2020 7363 2e70 7269            sc.pri
-0000c210: 6e74 7628 6627 5275 6e20 6669 6e69 7368  ntv(f'Run finish
-0000c220: 6564 2061 6674 6572 207b 656c 6170 7365  ed after {elapse
-0000c230: 643a 302e 3266 7d20 732e 5c6e 272c 2031  d:0.2f} s.\n', 1
-0000c240: 2c20 7665 7262 6f73 6529 0a0a 2020 2020  , verbose)..    
-0000c250: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0000c260: 0a0a 2020 2020 6465 6620 6669 6e61 6c69  ..    def finali
-0000c270: 7a65 2873 656c 662c 2076 6572 626f 7365  ze(self, verbose
-0000c280: 3d4e 6f6e 652c 2072 6573 746f 7265 5f70  =None, restore_p
-0000c290: 6172 733d 5472 7565 293a 0a20 2020 2020  ars=True):.     
-0000c2a0: 2020 2027 2727 2043 6f6d 7075 7465 2066     ''' Compute f
-0000c2b0: 696e 616c 2072 6573 756c 7473 2027 2727  inal results '''
-0000c2c0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-0000c2d0: 662e 7265 7375 6c74 735f 7265 6164 793a  f.results_ready:
-0000c2e0: 0a20 2020 2020 2020 2020 2020 2023 2042  .            # B
-0000c2f0: 6563 6175 7365 2074 6865 2072 6573 756c  ecause the resul
-0000c300: 7473 2061 7265 2072 6573 6361 6c65 6420  ts are rescaled 
-0000c310: 696e 2d70 6c61 6365 2c20 6669 6e61 6c69  in-place, finali
-0000c320: 7a69 6e67 2074 6865 2073 696d 2063 616e  zing the sim can
-0000c330: 6e6f 7420 6265 2072 756e 206d 6f72 6520  not be run more 
-0000c340: 7468 616e 206f 6e63 6520 6f72 0a20 2020  than once or.   
-0000c350: 2020 2020 2020 2020 2023 206f 7468 6572           # other
-0000c360: 7769 7365 2074 6865 2073 6361 6c65 2066  wise the scale f
-0000c370: 6163 746f 7220 7769 6c6c 2062 6520 6170  actor will be ap
-0000c380: 706c 6965 6420 6d75 6c74 6970 6c65 2074  plied multiple t
-0000c390: 696d 6573 0a20 2020 2020 2020 2020 2020  imes.           
-0000c3a0: 2072 6169 7365 2041 6c72 6561 6479 5275   raise AlreadyRu
-0000c3b0: 6e45 7272 6f72 2827 5369 6d75 6c61 7469  nError('Simulati
-0000c3c0: 6f6e 2068 6173 2061 6c72 6561 6479 2062  on has already b
-0000c3d0: 6565 6e20 6669 6e61 6c69 7a65 6427 290a  een finalized').
-0000c3e0: 0a20 2020 2020 2020 2023 2046 696e 616c  .        # Final
-0000c3f0: 697a 6520 616e 616c 797a 6572 7320 616e  ize analyzers an
-0000c400: 6420 696e 7465 7276 656e 7469 6f6e 730a  d interventions.
-0000c410: 2020 2020 2020 2020 7365 6c66 2e66 696e          self.fin
-0000c420: 616c 697a 655f 616e 616c 797a 6572 7328  alize_analyzers(
-0000c430: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
-0000c440: 2e66 696e 616c 697a 655f 696e 7465 7276  .finalize_interv
-0000c450: 656e 7469 6f6e 7328 2920 2354 4f44 4f3a  entions() #TODO:
-0000c460: 2077 6879 2069 7320 7468 6973 2063 6f6d   why is this com
-0000c470: 6d65 6e74 6564 206f 7574 3f0a 0a20 2020  mented out?..   
-0000c480: 2020 2020 2069 6620 7365 6c66 5b27 6d6f       if self['mo
-0000c490: 6465 6c5f 6869 7627 5d3a 0a20 2020 2020  del_hiv']:.     
-0000c4a0: 2020 2020 2020 2073 656c 662e 6869 7673         self.hivs
-0000c4b0: 696d 2e66 696e 616c 697a 6528 7365 6c66  im.finalize(self
-0000c4c0: 290a 0a20 2020 2020 2020 2023 2046 696e  )..        # Fin
-0000c4d0: 616c 2073 6574 7469 6e67 730a 2020 2020  al settings.    
-0000c4e0: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
-0000c4f0: 5f72 6561 6479 203d 2054 7275 6520 2320  _ready = True # 
-0000c500: 5365 7420 7468 6973 2066 6972 7374 2073  Set this first s
-0000c510: 6f20 7365 6c66 2e73 756d 6d61 7279 2829  o self.summary()
-0000c520: 206b 6e6f 7773 2074 6f20 7072 696e 7420   knows to print 
-0000c530: 7468 6520 7265 7375 6c74 730a 2020 2020  the results.    
-0000c540: 2020 2020 7365 6c66 2e74 202d 3d20 3120      self.t -= 1 
-0000c550: 2320 4475 7269 6e67 2074 6865 2072 756e  # During the run
-0000c560: 2c20 7468 6973 206b 6565 7073 2074 7261  , this keeps tra
-0000c570: 636b 206f 6620 7468 6520 6e65 7874 2073  ck of the next s
-0000c580: 7465 703b 2072 6573 746f 7265 2074 6869  tep; restore thi
-0000c590: 7320 6265 2074 6865 2066 696e 616c 2064  s be the final d
-0000c5a0: 6179 206f 6620 7468 6520 7369 6d0a 0a20  ay of the sim.. 
-0000c5b0: 2020 2020 2020 2023 2050 6572 666f 726d         # Perform
-0000c5c0: 2063 616c 6375 6c61 7469 6f6e 7320 6f6e   calculations on
-0000c5d0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
-0000c5e0: 2073 656c 662e 636f 6d70 7574 655f 7265   self.compute_re
-0000c5f0: 7375 6c74 7328 7665 7262 6f73 653d 7665  sults(verbose=ve
-0000c600: 7262 6f73 6529 2023 2043 616c 6375 6c61  rbose) # Calcula
-0000c610: 7465 2074 6865 2072 6573 7420 6f66 2074  te the rest of t
-0000c620: 6865 2072 6573 756c 7473 0a20 2020 2020  he results.     
-0000c630: 2020 2073 656c 662e 7265 7375 6c74 7320     self.results 
-0000c640: 3d20 7363 2e6f 626a 6469 6374 2873 656c  = sc.objdict(sel
-0000c650: 662e 7265 7375 6c74 7329 2023 2043 6f6e  f.results) # Con
-0000c660: 7665 7274 2072 6573 756c 7473 2074 6f20  vert results to 
-0000c670: 6120 6f64 6963 7473 2f6f 626a 6469 6374  a odicts/objdict
-0000c680: 2074 6f20 616c 6c6f 7720 652e 672e 2073   to allow e.g. s
-0000c690: 696d 2e72 6573 756c 7473 2e64 6961 676e  im.results.diagn
-0000c6a0: 6f73 6573 0a0a 2020 2020 2020 2020 2320  oses..        # 
-0000c6b0: 4f70 7469 6f6e 616c 6c79 2070 7269 6e74  Optionally print
-0000c6c0: 2073 756d 6d61 7279 206f 7574 7075 740a   summary output.
-0000c6d0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-0000c6e0: 7365 3a20 2320 5665 7262 6f73 6520 6973  se: # Verbose is
-0000c6f0: 2061 6e79 206e 6f6e 2d7a 6572 6f20 7661   any non-zero va
-0000c700: 6c75 650a 2020 2020 2020 2020 2020 2020  lue.            
-0000c710: 6966 2076 6572 626f 7365 3e30 3a20 2320  if verbose>0: # 
-0000c720: 5665 7262 6f73 6520 6973 2061 6e79 2070  Verbose is any p
-0000c730: 6f73 6974 6976 6520 6e75 6d62 6572 0a20  ositive number. 
-0000c740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c750: 656c 662e 7375 6d6d 6172 697a 6528 2920  elf.summarize() 
-0000c760: 2320 5072 696e 7420 6d65 6469 756d 2d6c  # Print medium-l
-0000c770: 656e 6774 6820 7375 6d6d 6172 7920 6f66  ength summary of
-0000c780: 2074 6865 2073 696d 0a20 2020 2020 2020   the sim.       
-0000c790: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000c7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c7b0: 6272 6965 6628 2920 2320 5072 696e 7420  brief() # Print 
-0000c7c0: 6272 6965 6620 7375 6d6d 6172 7920 6f66  brief summary of
-0000c7d0: 2074 6865 2073 696d 0a0a 2020 2020 2020   the sim..      
-0000c7e0: 2020 7265 7475 726e 0a0a 0a20 2020 2064    return...    d
-0000c7f0: 6566 2063 6f6d 7075 7465 5f72 6573 756c  ef compute_resul
-0000c800: 7473 2873 656c 662c 2076 6572 626f 7365  ts(self, verbose
-0000c810: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0000c820: 2727 2720 5065 7266 6f72 6d20 6669 6e61  ''' Perform fina
-0000c830: 6c20 6361 6c63 756c 6174 696f 6e73 206f  l calculations o
-0000c840: 6e20 7468 6520 7265 7375 6c74 7320 2727  n the results ''
-0000c850: 270a 2020 2020 2020 2020 7365 6c66 2e63  '.        self.c
-0000c860: 6f6d 7075 7465 5f73 7461 7465 7328 290a  ompute_states().
-0000c870: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-0000c880: 7075 7465 5f73 756d 6d61 7279 2829 0a20  pute_summary(). 
-0000c890: 2020 2020 2020 2072 6574 7572 6e0a 0a0a         return...
-0000c8a0: 2020 2020 6465 6620 636f 6d70 7574 655f      def compute_
-0000c8b0: 7374 6174 6573 2873 656c 6629 3a0a 2020  states(self):.  
-0000c8c0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000c8d0: 2020 436f 6d70 7574 6520 7072 6576 616c    Compute preval
-0000c8e0: 656e 6365 2c20 696e 6369 6465 6e63 652c  ence, incidence,
-0000c8f0: 2061 6e64 206f 7468 6572 2073 7461 7465   and other state
-0000c900: 732e 0a20 2020 2020 2020 2027 2727 0a20  s..        '''. 
-0000c910: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-0000c920: 662e 7265 7375 6c74 730a 0a20 2020 2020  f.results..     
-0000c930: 2020 2023 2043 6f6d 7075 7465 2048 5056     # Compute HPV
-0000c940: 2069 6e63 6964 656e 6365 2061 6e64 2070   incidence and p
-0000c950: 7265 7661 6c65 6e63 650a 2020 2020 2020  revalence.      
-0000c960: 2020 6465 6620 7361 6665 6469 7669 6465    def safedivide
-0000c970: 286e 756d 2c64 656e 6f6d 293a 0a20 2020  (num,denom):.   
-0000c980: 2020 2020 2020 2020 2027 2727 2044 6566           ''' Def
-0000c990: 696e 6520 6120 7661 7269 6174 696f 6e20  ine a variation 
-0000c9a0: 6f6e 2073 632e 7361 6665 6469 7669 6465  on sc.safedivide
-0000c9b0: 2074 6861 7420 7265 7370 6563 7473 2073   that respects s
-0000c9c0: 6861 7065 206f 6620 6e75 6d65 7261 746f  hape of numerato
-0000c9d0: 7220 2727 270a 2020 2020 2020 2020 2020  r '''.          
-0000c9e0: 2020 616e 7377 6572 203d 206e 702e 7a65    answer = np.ze
-0000c9f0: 726f 735f 6c69 6b65 286e 756d 290a 2020  ros_like(num).  
-0000ca00: 2020 2020 2020 2020 2020 6669 6c6c 5f69            fill_i
-0000ca10: 6e64 7320 3d20 2864 656e 6f6d 213d 3029  nds = (denom!=0)
-0000ca20: 2e6e 6f6e 7a65 726f 2829 0a20 2020 2020  .nonzero().     
-0000ca30: 2020 2020 2020 2069 6620 6c65 6e28 6e75         if len(nu
-0000ca40: 6d2e 7368 6170 6529 3d3d 6c65 6e28 6465  m.shape)==len(de
-0000ca50: 6e6f 6d2e 7368 6170 6529 3a0a 2020 2020  nom.shape):.    
-0000ca60: 2020 2020 2020 2020 2020 2020 616e 7377              answ
-0000ca70: 6572 5b66 696c 6c5f 696e 6473 5d20 3d20  er[fill_inds] = 
-0000ca80: 6e75 6d5b 6669 6c6c 5f69 6e64 735d 202f  num[fill_inds] /
-0000ca90: 2064 656e 6f6d 5b66 696c 6c5f 696e 6473   denom[fill_inds
-0000caa0: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-0000cab0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000cac0: 2020 2020 616e 7377 6572 5b3a 2c20 6669      answer[:, fi
-0000cad0: 6c6c 5f69 6e64 735d 203d 206e 756d 5b3a  ll_inds] = num[:
-0000cae0: 2c20 6669 6c6c 5f69 6e64 735d 202f 2064  , fill_inds] / d
-0000caf0: 656e 6f6d 5b66 696c 6c5f 696e 6473 5d0a  enom[fill_inds].
-0000cb00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000cb10: 726e 2061 6e73 7765 720a 2020 2020 2020  rn answer.      
-0000cb20: 2020 6e67 203d 2073 656c 662e 7061 7273    ng = self.pars
-0000cb30: 5b27 6e5f 6765 6e6f 7479 7065 7327 5d0a  ['n_genotypes'].
-0000cb40: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-0000cb50: 756c 7473 5b27 6870 765f 696e 6369 6465  ults['hpv_incide
-0000cb60: 6e63 6527 5d5b 3a5d 2020 2020 2020 2020  nce'][:]        
-0000cb70: 2020 2020 2020 2020 3d20 7363 2e73 6166          = sc.saf
-0000cb80: 6564 6976 6964 6528 7265 735b 2769 6e66  edivide(res['inf
-0000cb90: 6563 7469 6f6e 7327 5d5b 3a5d 2c20 6e67  ections'][:], ng
-0000cba0: 2a72 6573 5b27 6e5f 7375 7363 6570 7469  *res['n_suscepti
-0000cbb0: 626c 6527 5d5b 3a5d 290a 2020 2020 2020  ble'][:]).      
-0000cbc0: 2020 7365 6c66 2e72 6573 756c 7473 5b27    self.results['
-0000cbd0: 6870 765f 696e 6369 6465 6e63 655f 6279  hpv_incidence_by
-0000cbe0: 5f67 656e 6f74 7970 6527 5d5b 3a5d 2020  _genotype'][:]  
-0000cbf0: 2020 3d20 7361 6665 6469 7669 6465 2872    = safedivide(r
-0000cc00: 6573 5b27 696e 6665 6374 696f 6e73 5f62  es['infections_b
-0000cc10: 795f 6765 6e6f 7479 7065 275d 5b3a 5d2c  y_genotype'][:],
-0000cc20: 2072 6573 5b27 6e5f 7375 7363 6570 7469   res['n_suscepti
-0000cc30: 626c 655f 6279 5f67 656e 6f74 7970 6527  ble_by_genotype'
-0000cc40: 5d5b 3a5d 290a 2020 2020 2020 2020 7365  ][:]).        se
-0000cc50: 6c66 2e72 6573 756c 7473 5b27 6870 765f  lf.results['hpv_
-0000cc60: 696e 6369 6465 6e63 655f 6279 5f61 6765  incidence_by_age
-0000cc70: 275d 5b3a 5d20 2020 2020 2020 2020 3d20  '][:]         = 
-0000cc80: 7361 6665 6469 7669 6465 2872 6573 5b27  safedivide(res['
-0000cc90: 696e 6665 6374 696f 6e73 5f62 795f 6167  infections_by_ag
-0000cca0: 6527 5d5b 3a5d 2c20 6e67 2a72 6573 5b27  e'][:], ng*res['
-0000ccb0: 6e5f 7375 7363 6570 7469 626c 655f 6279  n_susceptible_by
-0000ccc0: 5f61 6765 275d 5b3a 5d29 0a20 2020 2020  _age'][:]).     
-0000ccd0: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
-0000cce0: 2768 7076 5f70 7265 7661 6c65 6e63 6527  'hpv_prevalence'
-0000ccf0: 5d5b 3a5d 2020 2020 2020 2020 2020 2020  ][:]            
-0000cd00: 2020 203d 2073 632e 7361 6665 6469 7669     = sc.safedivi
-0000cd10: 6465 2872 6573 5b27 6e5f 696e 6665 6374  de(res['n_infect
-0000cd20: 696f 7573 275d 5b3a 5d2c 206e 672a 7265  ious'][:], ng*re
-0000cd30: 735b 276e 5f61 6c69 7665 275d 5b3a 5d29  s['n_alive'][:])
-0000cd40: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000cd50: 7375 6c74 735b 2768 7076 5f70 7265 7661  sults['hpv_preva
-0000cd60: 6c65 6e63 655f 6279 5f67 656e 6f74 7970  lence_by_genotyp
-0000cd70: 6527 5d5b 3a5d 2020 203d 2073 6166 6564  e'][:]   = safed
-0000cd80: 6976 6964 6528 7265 735b 276e 5f69 6e66  ivide(res['n_inf
-0000cd90: 6563 7469 6f75 735f 6279 5f67 656e 6f74  ectious_by_genot
-0000cda0: 7970 6527 5d5b 3a5d 2c20 7265 735b 276e  ype'][:], res['n
-0000cdb0: 5f61 6c69 7665 275d 5b3a 5d29 0a20 2020  _alive'][:]).   
-0000cdc0: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
-0000cdd0: 735b 2768 7076 5f70 7265 7661 6c65 6e63  s['hpv_prevalenc
-0000cde0: 655f 6279 5f61 6765 275d 5b3a 5d20 2020  e_by_age'][:]   
-0000cdf0: 2020 2020 203d 2073 6166 6564 6976 6964       = safedivid
-0000ce00: 6528 7265 735b 276e 5f69 6e66 6563 7469  e(res['n_infecti
-0000ce10: 6f75 735f 6279 5f61 6765 275d 5b3a 5d2c  ous_by_age'][:],
-0000ce20: 206e 672a 7265 735b 276e 5f61 6c69 7665   ng*res['n_alive
-0000ce30: 5f62 795f 6167 6527 5d5b 3a5d 290a 0a20  _by_age'][:]).. 
-0000ce40: 2020 2020 2020 2061 6c69 7665 5f66 656d         alive_fem
-0000ce50: 616c 6573 203d 2072 6573 5b27 6e5f 616c  ales = res['n_al
-0000ce60: 6976 655f 6279 5f73 6578 275d 5b30 2c3a  ive_by_sex'][0,:
-0000ce70: 5d0a 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-0000ce80: 7265 7375 6c74 735b 2770 7265 6369 6e5f  results['precin_
-0000ce90: 7072 6576 616c 656e 6365 275d 5b3a 5d20  prevalence'][:] 
-0000cea0: 3d20 7363 2e73 6166 6564 6976 6964 6528  = sc.safedivide(
-0000ceb0: 7265 735b 276e 5f70 7265 6369 6e27 5d5b  res['n_precin'][
-0000cec0: 3a5d 2c20 6e67 202a 2061 6c69 7665 5f66  :], ng * alive_f
-0000ced0: 656d 616c 6573 290a 2020 2020 2020 2020  emales).        
-0000cee0: 7365 6c66 2e72 6573 756c 7473 5b27 7072  self.results['pr
-0000cef0: 6563 696e 5f70 7265 7661 6c65 6e63 655f  ecin_prevalence_
-0000cf00: 6279 5f67 656e 6f74 7970 6527 5d5b 3a5d  by_genotype'][:]
-0000cf10: 203d 2073 6166 6564 6976 6964 6528 7265   = safedivide(re
-0000cf20: 735b 276e 5f70 7265 6369 6e5f 6279 5f67  s['n_precin_by_g
-0000cf30: 656e 6f74 7970 6527 5d5b 3a5d 2c20 616c  enotype'][:], al
-0000cf40: 6976 655f 6665 6d61 6c65 7329 0a20 2020  ive_females).   
-0000cf50: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
-0000cf60: 735b 2770 7265 6369 6e5f 7072 6576 616c  s['precin_preval
-0000cf70: 656e 6365 5f62 795f 6167 6527 5d5b 3a5d  ence_by_age'][:]
-0000cf80: 203d 2073 6166 6564 6976 6964 6528 7265   = safedivide(re
-0000cf90: 735b 276e 5f70 7265 6369 6e5f 6279 5f61  s['n_precin_by_a
-0000cfa0: 6765 275d 5b3a 5d2c 0a20 2020 2020 2020  ge'][:],.       
-0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfe0: 2020 2020 2020 2020 6e67 202a 2072 6573          ng * res
-0000cff0: 5b27 6e5f 6665 6d61 6c65 735f 616c 6976  ['n_females_aliv
-0000d000: 655f 6279 5f61 6765 275d 5b3a 5d29 0a20  e_by_age'][:]). 
-0000d010: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-0000d020: 6c74 735b 2763 696e 315f 7072 6576 616c  lts['cin1_preval
-0000d030: 656e 6365 275d 5b3a 5d20 3d20 7363 2e73  ence'][:] = sc.s
-0000d040: 6166 6564 6976 6964 6528 7265 735b 276e  afedivide(res['n
-0000d050: 5f63 696e 3127 5d5b 3a5d 2c20 6e67 2a61  _cin1'][:], ng*a
-0000d060: 6c69 7665 5f66 656d 616c 6573 290a 2020  live_females).  
-0000d070: 2020 2020 2020 7365 6c66 2e72 6573 756c        self.resul
-0000d080: 7473 5b27 6369 6e31 5f70 7265 7661 6c65  ts['cin1_prevale
-0000d090: 6e63 655f 6279 5f67 656e 6f74 7970 6527  nce_by_genotype'
-0000d0a0: 5d5b 3a5d 203d 2073 6166 6564 6976 6964  ][:] = safedivid
-0000d0b0: 6528 7265 735b 276e 5f63 696e 315f 6279  e(res['n_cin1_by
-0000d0c0: 5f67 656e 6f74 7970 6527 5d5b 3a5d 2c20  _genotype'][:], 
-0000d0d0: 616c 6976 655f 6665 6d61 6c65 7329 0a20  alive_females). 
-0000d0e0: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-0000d0f0: 6c74 735b 2763 696e 315f 7072 6576 616c  lts['cin1_preval
-0000d100: 656e 6365 5f62 795f 6167 6527 5d5b 3a5d  ence_by_age'][:]
-0000d110: 203d 2073 6166 6564 6976 6964 6528 7265   = safedivide(re
-0000d120: 735b 276e 5f63 696e 315f 6279 5f61 6765  s['n_cin1_by_age
-0000d130: 275d 5b3a 5d2c 0a20 2020 2020 2020 2020  '][:],.         
-0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d170: 2020 2020 2020 6e67 2a72 6573 5b27 6e5f        ng*res['n_
-0000d180: 6665 6d61 6c65 735f 616c 6976 655f 6279  females_alive_by
-0000d190: 5f61 6765 275d 5b3a 5d29 0a20 2020 2020  _age'][:]).     
-0000d1a0: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
-0000d1b0: 2763 696e 325f 7072 6576 616c 656e 6365  'cin2_prevalence
-0000d1c0: 275d 5b3a 5d20 3d20 7363 2e73 6166 6564  '][:] = sc.safed
-0000d1d0: 6976 6964 6528 7265 735b 276e 5f63 696e  ivide(res['n_cin
-0000d1e0: 3227 5d5b 3a5d 2c20 6e67 2a61 6c69 7665  2'][:], ng*alive
-0000d1f0: 5f66 656d 616c 6573 290a 2020 2020 2020  _females).      
-0000d200: 2020 7365 6c66 2e72 6573 756c 7473 5b27    self.results['
-0000d210: 6369 6e32 5f70 7265 7661 6c65 6e63 655f  cin2_prevalence_
-0000d220: 6279 5f67 656e 6f74 7970 6527 5d5b 3a5d  by_genotype'][:]
-0000d230: 203d 2073 6166 6564 6976 6964 6528 7265   = safedivide(re
-0000d240: 735b 276e 5f63 696e 325f 6279 5f67 656e  s['n_cin2_by_gen
-0000d250: 6f74 7970 6527 5d5b 3a5d 2c20 616c 6976  otype'][:], aliv
-0000d260: 655f 6665 6d61 6c65 7329 0a20 2020 2020  e_females).     
-0000d270: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
-0000d280: 2763 696e 325f 7072 6576 616c 656e 6365  'cin2_prevalence
-0000d290: 5f62 795f 6167 6527 5d5b 3a5d 203d 2073  _by_age'][:] = s
-0000d2a0: 6166 6564 6976 6964 6528 7265 735b 276e  afedivide(res['n
-0000d2b0: 5f63 696e 325f 6279 5f61 6765 275d 5b3a  _cin2_by_age'][:
-0000d2c0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d300: 2020 6e67 2a72 6573 5b27 6e5f 6665 6d61    ng*res['n_fema
-0000d310: 6c65 735f 616c 6976 655f 6279 5f61 6765  les_alive_by_age
-0000d320: 275d 5b3a 5d29 0a20 2020 2020 2020 2073  '][:]).        s
-0000d330: 656c 662e 7265 7375 6c74 735b 2763 696e  elf.results['cin
-0000d340: 335f 7072 6576 616c 656e 6365 275d 5b3a  3_prevalence'][:
-0000d350: 5d20 3d20 7363 2e73 6166 6564 6976 6964  ] = sc.safedivid
-0000d360: 6528 7265 735b 276e 5f63 696e 3327 5d5b  e(res['n_cin3'][
-0000d370: 3a5d 2c20 6e67 2a61 6c69 7665 5f66 656d  :], ng*alive_fem
-0000d380: 616c 6573 290a 2020 2020 2020 2020 7365  ales).        se
-0000d390: 6c66 2e72 6573 756c 7473 5b27 6369 6e33  lf.results['cin3
-0000d3a0: 5f70 7265 7661 6c65 6e63 655f 6279 5f67  _prevalence_by_g
-0000d3b0: 656e 6f74 7970 6527 5d5b 3a5d 203d 2073  enotype'][:] = s
-0000d3c0: 6166 6564 6976 6964 6528 7265 735b 276e  afedivide(res['n
-0000d3d0: 5f63 696e 335f 6279 5f67 656e 6f74 7970  _cin3_by_genotyp
-0000d3e0: 6527 5d5b 3a5d 2c20 616c 6976 655f 6665  e'][:], alive_fe
-0000d3f0: 6d61 6c65 7329 0a20 2020 2020 2020 2073  males).        s
-0000d400: 656c 662e 7265 7375 6c74 735b 2763 696e  elf.results['cin
-0000d410: 335f 7072 6576 616c 656e 6365 5f62 795f  3_prevalence_by_
-0000d420: 6167 6527 5d5b 3a5d 203d 2073 6166 6564  age'][:] = safed
-0000d430: 6976 6964 6528 7265 735b 276e 5f63 696e  ivide(res['n_cin
-0000d440: 335f 6279 5f61 6765 275d 5b3a 5d2c 0a20  3_by_age'][:],. 
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d480: 2020 2020 2020 2020 2020 2020 2020 6e67                ng
-0000d490: 2a72 6573 5b27 6e5f 6665 6d61 6c65 735f  *res['n_females_
-0000d4a0: 616c 6976 655f 6279 5f61 6765 275d 5b3a  alive_by_age'][:
-0000d4b0: 5d29 0a20 2020 2020 2020 2023 2043 6f6d  ]).        # Com
-0000d4c0: 7075 7465 2063 616e 6365 7220 696e 6369  pute cancer inci
-0000d4d0: 6465 6e63 652e 0a20 2020 2020 2020 2061  dence..        a
-0000d4e0: 745f 7269 736b 5f66 656d 616c 6573 203d  t_risk_females =
-0000d4f0: 2061 6c69 7665 5f66 656d 616c 6573 202d   alive_females -
-0000d500: 2072 6573 5b27 6e5f 6361 6e63 6572 6f75   res['n_cancerou
-0000d510: 7327 5d5b 3a5d 0a20 2020 2020 2020 2073  s'][:].        s
-0000d520: 6361 6c65 5f66 6163 746f 7220 3d20 3165  cale_factor = 1e
-0000d530: 3520 2023 2043 616e 6365 7220 696e 6369  5  # Cancer inci
-0000d540: 6465 6e63 6520 6172 6520 6469 7370 6c61  dence are displa
-0000d550: 7965 6420 6173 2072 6174 6573 2070 6572  yed as rates per
-0000d560: 2031 3030 6b20 776f 6d65 6e0a 2020 2020   100k women.    
-0000d570: 2020 2020 6465 6d6f 6e69 6e61 746f 7220      demoninator 
-0000d580: 3d20 6174 5f72 6973 6b5f 6665 6d61 6c65  = at_risk_female
-0000d590: 7320 2f20 7363 616c 655f 6661 6374 6f72  s / scale_factor
-0000d5a0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000d5b0: 7375 6c74 735b 2763 616e 6365 725f 696e  sults['cancer_in
-0000d5c0: 6369 6465 6e63 6527 5d5b 3a5d 2020 2020  cidence'][:]    
-0000d5d0: 2020 2020 2020 2020 203d 2072 6573 5b27           = res['
-0000d5e0: 6361 6e63 6572 7327 5d5b 3a5d 202f 2064  cancers'][:] / d
-0000d5f0: 656d 6f6e 696e 6174 6f72 0a20 2020 2020  emoninator.     
-0000d600: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
-0000d610: 2763 616e 6365 725f 696e 6369 6465 6e63  'cancer_incidenc
-0000d620: 655f 6279 5f67 656e 6f74 7970 6527 5d5b  e_by_genotype'][
-0000d630: 3a5d 203d 2072 6573 5b27 6361 6e63 6572  :] = res['cancer
-0000d640: 735f 6279 5f67 656e 6f74 7970 6527 5d5b  s_by_genotype'][
-0000d650: 3a5d 202f 2064 656d 6f6e 696e 6174 6f72  :] / demoninator
-0000d660: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000d670: 7375 6c74 735b 2763 616e 6365 725f 696e  sults['cancer_in
-0000d680: 6369 6465 6e63 655f 6279 5f61 6765 275d  cidence_by_age']
-0000d690: 5b3a 5d20 2020 2020 203d 2073 632e 7361  [:]      = sc.sa
-0000d6a0: 6665 6469 7669 6465 2872 6573 5b27 6361  fedivide(res['ca
-0000d6b0: 6e63 6572 735f 6279 5f61 6765 275d 5b3a  ncers_by_age'][:
-0000d6c0: 5d2c 2072 6573 5b27 6e5f 6665 6d61 6c65  ], res['n_female
-0000d6d0: 735f 616c 6976 655f 6279 5f61 6765 275d  s_alive_by_age']
-0000d6e0: 5b3a 5d2f 7363 616c 655f 6661 6374 6f72  [:]/scale_factor
-0000d6f0: 290a 0a20 2020 2020 2020 2023 2043 6f6d  )..        # Com
-0000d700: 7075 7465 2063 616e 6365 7220 6d6f 7274  pute cancer mort
-0000d710: 616c 6974 792e 2044 656e 6f6d 696e 6174  ality. Denominat
-0000d720: 6f72 2069 7320 616c 6c20 776f 6d65 6e20  or is all women 
-0000d730: 616c 6976 650a 2020 2020 2020 2020 6465  alive.        de
-0000d740: 6e6f 6d69 6e61 746f 7220 3d20 616c 6976  nominator = aliv
-0000d750: 655f 6665 6d61 6c65 732f 7363 616c 655f  e_females/scale_
-0000d760: 6661 6374 6f72 0a20 2020 2020 2020 2073  factor.        s
-0000d770: 656c 662e 7265 7375 6c74 735b 2763 616e  elf.results['can
-0000d780: 6365 725f 6d6f 7274 616c 6974 7927 5d5b  cer_mortality'][
-0000d790: 3a5d 2020 2020 2020 2020 203d 2072 6573  :]         = res
-0000d7a0: 5b27 6361 6e63 6572 5f64 6561 7468 7327  ['cancer_deaths'
-0000d7b0: 5d5b 3a5d 2f64 656e 6f6d 696e 6174 6f72  ][:]/denominator
-0000d7c0: 0a0a 2020 2020 2020 2020 2320 436f 6d70  ..        # Comp
-0000d7d0: 7574 6520 4850 5620 7479 7065 2064 6973  ute HPV type dis
-0000d7e0: 7472 6962 7574 696f 6e20 6279 2063 7974  tribution by cyt
-0000d7f0: 6f6c 6f67 790a 2020 2020 2020 2020 666f  ology.        fo
-0000d800: 7220 7768 6963 6820 696e 2068 7064 2e74  r which in hpd.t
-0000d810: 7970 655f 6469 7374 5f6b 6579 733a 0a20  ype_dist_keys:. 
-0000d820: 2020 2020 2020 2020 2020 2062 795f 7479             by_ty
-0000d830: 7065 203d 2072 6573 5b66 276e 5f7b 7768  pe = res[f'n_{wh
-0000d840: 6963 687d 5f62 795f 6765 6e6f 7479 7065  ich}_by_genotype
-0000d850: 275d 5b3a 5d0a 2020 2020 2020 2020 2020  '][:].          
-0000d860: 2020 746f 7461 6c73 203d 2062 795f 7479    totals = by_ty
-0000d870: 7065 2e73 756d 2861 7869 733d 3029 0a20  pe.sum(axis=0). 
-0000d880: 2020 2020 2020 2020 2020 2069 6e64 735f             inds_
-0000d890: 746f 5f66 696c 6c20 3d20 746f 7461 6c73  to_fill = totals
-0000d8a0: 203e 2030 0a20 2020 2020 2020 2020 2020   > 0.           
-0000d8b0: 2072 6573 5b77 6869 6368 202b 2027 5f67   res[which + '_g
-0000d8c0: 656e 6f74 7970 655f 6469 7374 275d 5b3a  enotype_dist'][:
-0000d8d0: 2c20 696e 6473 5f74 6f5f 6669 6c6c 5d20  , inds_to_fill] 
-0000d8e0: 3d20 6279 5f74 7970 655b 3a2c 2069 6e64  = by_type[:, ind
-0000d8f0: 735f 746f 5f66 696c 6c5d 202f 2074 6f74  s_to_fill] / tot
-0000d900: 616c 735b 696e 6473 5f74 6f5f 6669 6c6c  als[inds_to_fill
-0000d910: 5d0a 0a20 2020 2020 2020 2023 2044 656d  ]..        # Dem
-0000d920: 6f67 7261 7068 6963 2072 6573 756c 7473  ographic results
-0000d930: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000d940: 7375 6c74 735b 2763 6472 275d 5b3a 5d20  sults['cdr'][:] 
-0000d950: 203d 2073 656c 662e 7265 7375 6c74 735b   = self.results[
-0000d960: 276f 7468 6572 5f64 6561 7468 7327 5d5b  'other_deaths'][
-0000d970: 3a5d 202f 2028 7365 6c66 2e72 6573 756c  :] / (self.resul
-0000d980: 7473 5b27 6e5f 616c 6976 6527 5d5b 3a5d  ts['n_alive'][:]
-0000d990: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-0000d9a0: 6573 756c 7473 5b27 6362 7227 5d5b 3a5d  esults['cbr'][:]
-0000d9b0: 2020 3d20 7365 6c66 2e72 6573 756c 7473    = self.results
-0000d9c0: 5b27 6269 7274 6873 275d 5b3a 5d20 2f20  ['births'][:] / 
-0000d9d0: 2873 656c 662e 7265 7375 6c74 735b 276e  (self.results['n
-0000d9e0: 5f61 6c69 7665 275d 5b3a 5d29 0a0a 2020  _alive'][:])..  
-0000d9f0: 2020 2020 2020 2320 5661 6363 696e 6174        # Vaccinat
-0000da00: 696f 6e20 7265 7375 6c74 730a 2020 2020  ion results.    
-0000da10: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
-0000da20: 5b27 6375 6d5f 7661 6363 696e 6174 6564  ['cum_vaccinated
-0000da30: 275d 5b3a 5d20 3d20 6e70 2e63 756d 7375  '][:] = np.cumsu
-0000da40: 6d28 7365 6c66 2e72 6573 756c 7473 5b27  m(self.results['
-0000da50: 6e65 775f 7661 6363 696e 6174 6564 275d  new_vaccinated']
-0000da60: 5b3a 5d2c 2061 7869 733d 3029 0a20 2020  [:], axis=0).   
-0000da70: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
-0000da80: 735b 2763 756d 5f74 6f74 616c 5f76 6163  s['cum_total_vac
-0000da90: 6369 6e61 7465 6427 5d5b 3a5d 203d 206e  cinated'][:] = n
-0000daa0: 702e 6375 6d73 756d 2873 656c 662e 7265  p.cumsum(self.re
-0000dab0: 7375 6c74 735b 276e 6577 5f74 6f74 616c  sults['new_total
-0000dac0: 5f76 6163 6369 6e61 7465 6427 5d5b 3a5d  _vaccinated'][:]
-0000dad0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-0000dae0: 6573 756c 7473 5b27 6375 6d5f 646f 7365  esults['cum_dose
-0000daf0: 7327 5d5b 3a5d 203d 206e 702e 6375 6d73  s'][:] = np.cums
-0000db00: 756d 2873 656c 662e 7265 7375 6c74 735b  um(self.results[
-0000db10: 276e 6577 5f64 6f73 6573 275d 5b3a 5d29  'new_doses'][:])
-0000db20: 0a0a 2020 2020 2020 2020 2320 5468 6572  ..        # Ther
-0000db30: 6170 6575 7469 6320 7661 6363 696e 6174  apeutic vaccinat
-0000db40: 696f 6e20 7265 7375 6c74 730a 2020 2020  ion results.    
-0000db50: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
-0000db60: 5b27 6375 6d5f 7478 5f76 6163 6369 6e61  ['cum_tx_vaccina
-0000db70: 7465 6427 5d5b 3a5d 203d 206e 702e 6375  ted'][:] = np.cu
-0000db80: 6d73 756d 2873 656c 662e 7265 7375 6c74  msum(self.result
-0000db90: 735b 276e 6577 5f74 785f 7661 6363 696e  s['new_tx_vaccin
-0000dba0: 6174 6564 275d 5b3a 5d2c 2061 7869 733d  ated'][:], axis=
-0000dbb0: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
-0000dbc0: 7265 7375 6c74 735b 2763 756d 5f74 7876  results['cum_txv
-0000dbd0: 785f 646f 7365 7327 5d5b 3a5d 203d 206e  x_doses'][:] = n
-0000dbe0: 702e 6375 6d73 756d 2873 656c 662e 7265  p.cumsum(self.re
-0000dbf0: 7375 6c74 735b 276e 6577 5f74 7876 785f  sults['new_txvx_
-0000dc00: 646f 7365 7327 5d5b 3a5d 290a 0a20 2020  doses'][:])..   
-0000dc10: 2020 2020 2023 2053 6372 6565 6e20 2620       # Screen & 
-0000dc20: 7472 6561 7420 7265 7375 6c74 730a 2020  treat results.  
-0000dc30: 2020 2020 2020 7365 6c66 2e72 6573 756c        self.resul
-0000dc40: 7473 5b27 6375 6d5f 7363 7265 656e 7327  ts['cum_screens'
-0000dc50: 5d5b 3a5d 203d 206e 702e 6375 6d73 756d  ][:] = np.cumsum
-0000dc60: 2873 656c 662e 7265 7375 6c74 735b 276e  (self.results['n
-0000dc70: 6577 5f73 6372 6565 6e73 275d 5b3a 5d2c  ew_screens'][:],
-0000dc80: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-0000dc90: 2073 656c 662e 7265 7375 6c74 735b 2763   self.results['c
-0000dca0: 756d 5f73 6372 6565 6e65 6427 5d5b 3a5d  um_screened'][:]
-0000dcb0: 203d 206e 702e 6375 6d73 756d 2873 656c   = np.cumsum(sel
-0000dcc0: 662e 7265 7375 6c74 735b 276e 6577 5f73  f.results['new_s
-0000dcd0: 6372 6565 6e65 6427 5d5b 3a5d 2c20 6178  creened'][:], ax
-0000dce0: 6973 3d30 290a 2020 2020 2020 2020 7365  is=0).        se
-0000dcf0: 6c66 2e72 6573 756c 7473 5b27 6375 6d5f  lf.results['cum_
-0000dd00: 6369 6e5f 7472 6561 746d 656e 7473 275d  cin_treatments']
-0000dd10: 5b3a 5d20 3d20 6e70 2e63 756d 7375 6d28  [:] = np.cumsum(
-0000dd20: 7365 6c66 2e72 6573 756c 7473 5b27 6e65  self.results['ne
-0000dd30: 775f 6369 6e5f 7472 6561 746d 656e 7473  w_cin_treatments
-0000dd40: 275d 5b3a 5d2c 2061 7869 733d 3029 0a20  '][:], axis=0). 
+00003f40: 2020 2066 6f72 2067 7061 726e 616d 652c     for gparname,
+00003f50: 6770 6172 7661 6c20 696e 2067 7061 7273  gparval in gpars
+00003f60: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f80: 2020 2020 2020 6966 2067 7061 726e 616d        if gparnam
+00003f90: 6520 696e 2073 656c 665b 2767 656e 6f74  e in self['genot
+00003fa0: 7970 655f 7061 7273 275d 5b67 5d2e 6b65  ype_pars'][g].ke
+00003fb0: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fd0: 2020 2020 2020 7072 696e 746d 7367 203d        printmsg =
+00003fe0: 2066 2252 6573 6574 7469 6e67 2070 6172   f"Resetting par
+00003ff0: 616d 6574 6572 2027 7b67 7061 726e 616d  ameter '{gparnam
+00004000: 657d 2720 6672 6f6d 207b 7365 6c66 5b27  e}' from {self['
+00004010: 6765 6e6f 7479 7065 5f70 6172 7327 5d5b  genotype_pars'][
+00004020: 675d 5b67 7061 726e 616d 655d 7d20 746f  g][gparname]} to
+00004030: 207b 6770 6172 7661 6c7d 2066 6f72 2067   {gparval} for g
+00004040: 656e 6f74 7970 6520 7b67 7d22 0a20 2020  enotype {g}".   
+00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004060: 2020 2020 2020 2020 2020 2020 2073 632e               sc.
+00004070: 7072 696e 7476 2870 7269 6e74 6d73 672c  printv(printmsg,
+00004080: 2031 2c20 7365 6c66 5b27 7665 7262 6f73   1, self['verbos
+00004090: 6527 5d29 0a20 2020 2020 2020 2020 2020  e']).           
+000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040b0: 2020 2020 2073 656c 665b 2767 656e 6f74       self['genot
+000040c0: 7970 655f 7061 7273 275d 5b67 5d5b 6770  ype_pars'][g][gp
+000040d0: 6172 6e61 6d65 5d20 3d20 6770 6172 7661  arname] = gparva
+000040e0: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+000040f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00004100: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004120: 2020 2020 6572 726f 726d 7367 203d 2066      errormsg = f
+00004130: 2250 6172 616d 6574 6572 207b 6770 6172  "Parameter {gpar
+00004140: 6e61 6d65 7d20 646f 6573 206e 6f74 2065  name} does not e
+00004150: 7869 7374 2066 6f72 2067 656e 6f74 7970  xist for genotyp
+00004160: 6520 7b67 7d22 0a20 2020 2020 2020 2020  e {g}".         
+00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004180: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00004190: 7565 4572 726f 7228 6572 726f 726d 7367  ueError(errormsg
+000041a0: 290a 0a20 2020 2020 2020 2073 656c 665b  )..        self[
+000041b0: 276e 5f67 656e 6f74 7970 6573 275d 203d  'n_genotypes'] =
+000041c0: 206c 656e 2873 656c 665b 2767 656e 6f74   len(self['genot
+000041d0: 7970 655f 7061 7273 275d 2920 2023 2045  ype_pars'])  # E
+000041e0: 6163 6820 6765 6e6f 7479 7065 2068 6173  ach genotype has
+000041f0: 2061 6e20 656e 7472 7920 696e 2067 656e   an entry in gen
+00004200: 6f74 7970 655f 7061 7273 0a0a 2020 2020  otype_pars..    
+00004210: 2020 2020 2320 5365 7420 7468 6520 6e75      # Set the nu
+00004220: 6d62 6572 206f 6620 696d 6d75 6e69 7479  mber of immunity
+00004230: 2073 6f75 7263 6573 0a20 2020 2020 2020   sources.       
+00004240: 2073 656c 665b 276e 5f69 6d6d 5f73 6f75   self['n_imm_sou
+00004250: 7263 6573 275d 203d 206c 656e 2873 656c  rces'] = len(sel
+00004260: 665b 2767 656e 6f74 7970 6573 275d 290a  f['genotypes']).
+00004270: 0a20 2020 2020 2020 2023 2044 6f20 616e  .        # Do an
+00004280: 7920 7072 6563 6f6d 7075 7461 7469 6f6e  y precomputation
+00004290: 7320 666f 7220 7468 6520 6765 6e6f 7479  s for the genoty
+000042a0: 7065 2074 7261 6e73 666f 726d 6174 696f  pe transformatio
+000042b0: 6e20 6675 6e63 7469 6f6e 730a 2020 2020  n functions.    
+000042c0: 2020 2020 745f 7374 6570 203d 2073 656c      t_step = sel
+000042d0: 665b 2764 7427 5d0a 2020 2020 2020 2020  f['dt'].        
+000042e0: 745f 7365 7175 656e 6365 203d 206e 702e  t_sequence = np.
+000042f0: 6172 616e 6765 2830 2c20 7570 7065 725f  arange(0, upper_
+00004300: 6479 7370 5f6c 696d 2c20 745f 7374 6570  dysp_lim, t_step
+00004310: 290a 2020 2020 2020 2020 7469 6d65 7374  ).        timest
+00004320: 6570 7320 3d20 745f 7365 7175 656e 6365  eps = t_sequence
+00004330: 202f 2074 5f73 7465 700a 2020 2020 2020   / t_step.      
+00004340: 2020 6375 6d64 7973 7020 3d20 6469 6374    cumdysp = dict
+00004350: 2829 0a20 2020 2020 2020 2066 6f72 2067  ().        for g
+00004360: 2069 6e20 7261 6e67 6528 7365 6c66 5b27   in range(self['
+00004370: 6e5f 6765 6e6f 7479 7065 7327 5d29 3a0a  n_genotypes']):.
+00004380: 2020 2020 2020 2020 2020 2020 7365 765f              sev_
+00004390: 666e 203d 2073 656c 665b 2767 656e 6f74  fn = self['genot
+000043a0: 7970 655f 7061 7273 275d 5b67 5d5b 2773  ype_pars'][g]['s
+000043b0: 6576 5f66 6e27 5d0a 2020 2020 2020 2020  ev_fn'].        
+000043c0: 2020 2020 7365 765f 696e 7465 6772 616c      sev_integral
+000043d0: 203d 2073 656c 665b 2767 656e 6f74 7970   = self['genotyp
+000043e0: 655f 7061 7273 275d 5b67 5d5b 2773 6576  e_pars'][g]['sev
+000043f0: 5f69 6e74 6567 7261 6c27 5d0a 2020 2020  _integral'].    
+00004400: 2020 2020 2020 2020 6966 2073 6576 5f69          if sev_i
+00004410: 6e74 6567 7261 6c3d 3d27 6e75 6d65 7269  ntegral=='numeri
+00004420: 6327 3a0a 2020 2020 2020 2020 2020 2020  c':.            
+00004430: 2020 2020 676c 6162 656c 203d 2073 656c      glabel = sel
+00004440: 665b 2767 656e 6f74 7970 655f 6d61 7027  f['genotype_map'
+00004450: 5d5b 675d 0a20 2020 2020 2020 2020 2020  ][g].           
+00004460: 2020 2020 2064 7973 705f 6172 7220 3d20       dysp_arr = 
+00004470: 6870 7061 722e 636f 6d70 7574 655f 7365  hppar.compute_se
+00004480: 7665 7269 7479 2874 5f73 6571 7565 6e63  verity(t_sequenc
+00004490: 652c 2072 656c 5f73 6576 3d4e 6f6e 652c  e, rel_sev=None,
+000044a0: 2070 6172 733d 7365 765f 666e 290a 2020   pars=sev_fn).  
+000044b0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000044c0: 6d64 7973 705b 676c 6162 656c 5d20 3d20  mdysp[glabel] = 
+000044d0: 6e70 2e63 756d 7375 6d28 6479 7370 5f61  np.cumsum(dysp_a
+000044e0: 7272 2920 2a20 745f 7374 6570 0a0a 2020  rr) * t_step..  
+000044f0: 2020 2020 2020 7365 6c66 5b27 6375 6d64        self['cumd
+00004500: 7973 7027 5d20 3d20 6375 6d64 7973 7020  ysp'] = cumdysp 
+00004510: 2023 2053 746f 7265 0a0a 2020 2020 2020   # Store..      
+00004520: 2020 7265 7475 726e 0a0a 0a20 2020 2064    return...    d
+00004530: 6566 2069 6e69 745f 7265 7375 6c74 7328  ef init_results(
+00004540: 7365 6c66 2c20 6672 6571 7565 6e63 793d  self, frequency=
+00004550: 2761 6e6e 7561 6c27 2c20 6164 645f 6461  'annual', add_da
+00004560: 7461 3d54 7275 6529 3a0a 2020 2020 2020  ta=True):.      
+00004570: 2020 2727 270a 2020 2020 2020 2020 4372    '''.        Cr
+00004580: 6561 7465 2074 6865 206d 6169 6e20 7265  eate the main re
+00004590: 7375 6c74 7320 7374 7275 6374 7572 652e  sults structure.
+000045a0: 0a20 2020 2020 2020 2054 6865 2070 7265  .        The pre
+000045b0: 6669 7820 226e 2220 6973 2075 7365 6420  fix "n" is used 
+000045c0: 666f 7220 7374 6f63 6b20 7661 7269 6162  for stock variab
+000045d0: 6c65 732c 2069 2e65 2e20 636f 756e 7469  les, i.e. counti
+000045e0: 6e67 2074 6865 2074 6f74 616c 206e 756d  ng the total num
+000045f0: 6265 7220 696e 2061 6e79 2067 6976 656e  ber in any given
+00004600: 2073 7461 7465 2028 7375 732f 696e 662f   state (sus/inf/
+00004610: 6574 6329 206f 6e20 616e 7920 7061 7274  etc) on any part
+00004620: 6963 756c 6172 2074 696d 6573 7465 700a  icular timestep.
+00004630: 0a20 2020 2020 2020 2041 7267 756d 656e  .        Argumen
+00004640: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00004650: 7369 6d20 2020 2020 2020 2020 2868 7076  sim         (hpv
+00004660: 2e53 696d 2920 2020 2020 2020 3a20 6120  .Sim)       : a 
+00004670: 7369 6d0a 2020 2020 2020 2020 2020 2020  sim.            
+00004680: 6672 6571 7565 6e63 7920 2020 2873 7472  frequency   (str
+00004690: 206f 7220 666c 6f61 7429 2020 3a20 7468   or float)  : th
+000046a0: 6520 6672 6571 7565 6e63 7920 7769 7468  e frequency with
+000046b0: 2077 6869 6368 2074 6f20 7361 7665 2072   which to save r
+000046c0: 6573 756c 7473 3a20 6163 6365 7074 7320  esults: accepts 
+000046d0: 2761 6e6e 7561 6c27 2c20 2764 7427 2c20  'annual', 'dt', 
+000046e0: 6f72 2061 2066 6c6f 6174 2077 6869 6368  or a float which
+000046f0: 2069 7320 696e 7465 7270 7265 7465 6420   is interpreted 
+00004700: 6173 2061 2066 7261 6374 696f 6e20 6f66  as a fraction of
+00004710: 2061 2079 6561 722c 2065 2e67 2e20 302e   a year, e.g. 0.
+00004720: 3220 7769 6c6c 2073 6176 6520 7265 7375  2 will save resu
+00004730: 6c74 7320 6576 6572 7920 302e 3220 7965  lts every 0.2 ye
+00004740: 6172 730a 2020 2020 2020 2020 2020 2020  ars.            
+00004750: 6164 645f 6461 7461 2020 2020 2862 6f6f  add_data    (boo
+00004760: 6c29 2020 2020 2020 2020 2020 3a20 7768  l)          : wh
+00004770: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
+00004780: 6164 6420 6461 7461 2074 6f20 7468 6520  add data to the 
+00004790: 7265 7375 6c74 2073 7472 7563 7475 7265  result structure
+000047a0: 730a 2020 2020 2020 2020 2727 270a 0a20  s.        '''.. 
+000047b0: 2020 2020 2020 2023 2048 616e 646c 6520         # Handle 
+000047c0: 6672 6571 7565 6e63 790a 2020 2020 2020  frequency.      
+000047d0: 2020 6966 2074 7970 6528 6672 6571 7565    if type(freque
+000047e0: 6e63 7929 203d 3d20 7374 723a 0a20 2020  ncy) == str:.   
+000047f0: 2020 2020 2020 2020 2069 6620 6672 6571           if freq
+00004800: 7565 6e63 7920 3d3d 2027 616e 6e75 616c  uency == 'annual
+00004810: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00004820: 2020 2072 6573 6672 6571 203d 2069 6e74     resfreq = int
+00004830: 2831 202f 2073 656c 665b 2764 7427 5d29  (1 / self['dt'])
+00004840: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00004850: 6620 6672 6571 7565 6e63 7920 3d3d 2027  f frequency == '
+00004860: 6474 273a 0a20 2020 2020 2020 2020 2020  dt':.           
+00004870: 2020 2020 2072 6573 6672 6571 203d 2031       resfreq = 1
+00004880: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00004890: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000048a0: 2020 2065 7272 6f72 6d73 6720 3d20 6627     errormsg = f'
+000048b0: 5265 7375 6c74 2066 7265 7175 656e 6379  Result frequency
+000048c0: 206e 6f74 2075 6e64 6572 7374 6f6f 643a   not understood:
+000048d0: 206d 7573 7420 6265 2022 616e 6e75 616c   must be "annual
+000048e0: 222c 2022 6474 2220 6f72 2061 2066 6c6f  ", "dt" or a flo
+000048f0: 6174 2c20 6275 7420 796f 7520 7072 6f76  at, but you prov
+00004900: 6964 6564 207b 6672 6571 7565 6e63 797d  ided {frequency}
+00004910: 2e27 0a20 2020 2020 2020 2020 2020 2020  .'.             
+00004920: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00004930: 726f 7228 6572 726f 726d 7367 290a 2020  ror(errormsg).  
+00004940: 2020 2020 2020 656c 6966 2074 7970 6528        elif type(
+00004950: 6672 6571 7565 6e63 7929 203d 3d20 666c  frequency) == fl
+00004960: 6f61 743a 0a20 2020 2020 2020 2020 2020  oat:.           
+00004970: 2069 6620 6672 6571 7565 6e63 7920 3c20   if frequency < 
+00004980: 7365 6c66 5b27 6474 275d 3a0a 2020 2020  self['dt']:.    
+00004990: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+000049a0: 726d 7367 203d 2066 2759 6f75 2072 6571  rmsg = f'You req
+000049b0: 7565 7374 6564 2072 6573 756c 7473 2077  uested results w
+000049c0: 6974 6820 6672 6571 7565 6e63 7920 7b66  ith frequency {f
+000049d0: 7265 7175 656e 6379 7d2c 2062 7574 2074  requency}, but t
+000049e0: 6869 7320 6973 2073 6d61 6c6c 6572 2074  his is smaller t
+000049f0: 6861 6e20 7468 6520 7369 6d75 6c61 7469  han the simulati
+00004a00: 6f6e 2074 696d 6573 7465 7020 7b73 656c  on timestep {sel
+00004a10: 665b 2264 7422 5d7d 2e27 0a20 2020 2020  f["dt"]}.'.     
+00004a20: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00004a30: 2056 616c 7565 4572 726f 7228 6572 726f   ValueError(erro
+00004a40: 726d 7367 290a 2020 2020 2020 2020 2020  rmsg).          
+00004a50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004a60: 2020 2020 2020 2020 7265 7366 7265 7120          resfreq 
+00004a70: 3d20 696e 7428 6672 6571 7565 6e63 7920  = int(frequency 
+00004a80: 2f20 7365 6c66 5b27 6474 275d 290a 2020  / self['dt']).  
+00004a90: 2020 2020 2020 7365 6c66 2e72 6573 6672        self.resfr
+00004aa0: 6571 203d 2072 6573 6672 6571 0a20 2020  eq = resfreq.   
+00004ab0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00004ac0: 2e72 6573 6672 6571 203e 2030 3a0a 2020  .resfreq > 0:.  
+00004ad0: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
+00004ae0: 7367 203d 2066 2754 6865 2072 6573 756c  sg = f'The resul
+00004af0: 7473 2066 7265 7175 656e 6365 2073 686f  ts frequence sho
+00004b00: 756c 6420 6265 2061 2070 6f73 6974 6976  uld be a positiv
+00004b10: 6520 696e 7465 6765 722c 206e 6f74 207b  e integer, not {
+00004b20: 7365 6c66 2e72 6573 6672 6571 7d3a 2064  self.resfreq}: d
+00004b30: 7420 6d61 7920 6265 2074 6f6f 206c 6172  t may be too lar
+00004b40: 6765 270a 2020 2020 2020 2020 2020 2020  ge'.            
+00004b50: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00004b60: 2865 7272 6f72 6d73 6729 0a0a 2020 2020  (errormsg)..    
+00004b70: 2020 2020 2320 436f 6e73 7472 7563 7420      # Construct 
+00004b80: 7468 6520 7476 6563 2074 6861 7420 7769  the tvec that wi
+00004b90: 6c6c 2062 6520 7573 6564 2077 6974 6820  ll be used with 
+00004ba0: 7468 6520 7265 7375 6c74 730a 2020 2020  the results.    
+00004bb0: 2020 2020 706f 696e 7473 5f74 6f5f 7573      points_to_us
+00004bc0: 6520 3d20 6e70 2e61 7261 6e67 6528 302c  e = np.arange(0,
+00004bd0: 2073 656c 662e 6e70 7473 2c20 7365 6c66   self.npts, self
+00004be0: 2e72 6573 6672 6571 290a 2020 2020 2020  .resfreq).      
+00004bf0: 2020 7365 6c66 2e72 6573 5f79 6561 7276    self.res_yearv
+00004c00: 6563 203d 2073 656c 662e 7965 6172 7665  ec = self.yearve
+00004c10: 635b 706f 696e 7473 5f74 6f5f 7573 655d  c[points_to_use]
+00004c20: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00004c30: 735f 6e70 7473 203d 206c 656e 2873 656c  s_npts = len(sel
+00004c40: 662e 7265 735f 7965 6172 7665 6329 0a20  f.res_yearvec). 
+00004c50: 2020 2020 2020 2073 656c 662e 7265 735f         self.res_
+00004c60: 7476 6563 203d 206e 702e 6172 616e 6765  tvec = np.arange
+00004c70: 2873 656c 662e 7265 735f 6e70 7473 290a  (self.res_npts).
+00004c80: 0a20 2020 2020 2020 2023 2046 756e 6374  .        # Funct
+00004c90: 696f 6e20 746f 2063 7265 6174 6520 7265  ion to create re
+00004ca0: 7375 6c74 730a 2020 2020 2020 2020 6465  sults.        de
+00004cb0: 6620 696e 6974 5f72 6573 282a 6172 6773  f init_res(*args
+00004cc0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00004cd0: 2020 2020 2020 2020 2027 2727 2049 6e69           ''' Ini
+00004ce0: 7469 616c 697a 6520 6120 7369 6e67 6c65  tialize a single
+00004cf0: 2072 6573 756c 7420 6f62 6a65 6374 2027   result object '
+00004d00: 2727 0a20 2020 2020 2020 2020 2020 206f  ''.            o
+00004d10: 7574 7075 7420 3d20 6870 622e 5265 7375  utput = hpb.Resu
+00004d20: 6c74 282a 6172 6773 2c20 2a2a 6b77 6172  lt(*args, **kwar
+00004d30: 6773 2c20 6e70 7473 3d73 656c 662e 7265  gs, npts=self.re
+00004d40: 735f 6e70 7473 290a 2020 2020 2020 2020  s_npts).        
+00004d50: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
+00004d60: 740a 0a20 2020 2020 2020 2023 2049 6e69  t..        # Ini
+00004d70: 7469 616c 697a 6520 7374 6f72 6167 650a  tialize storage.
+00004d80: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
+00004d90: 3d20 7363 2e6f 626a 6469 6374 2829 0a0a  = sc.objdict()..
+00004da0: 2020 2020 2020 2020 6e67 203d 2073 656c          ng = sel
+00004db0: 665b 276e 5f67 656e 6f74 7970 6573 275d  f['n_genotypes']
+00004dc0: 2023 204e 756d 6265 7220 6f66 2067 656e   # Number of gen
+00004dd0: 6f74 7970 6573 0a20 2020 2020 2020 206e  otypes.        n
+00004de0: 6120 3d20 6c65 6e28 7365 6c66 5b27 6167  a = len(self['ag
+00004df0: 655f 6269 6e5f 6564 6765 7327 5d29 202d  e_bin_edges']) -
+00004e00: 2031 2023 204e 756d 6265 7220 6f66 2061   1 # Number of a
+00004e10: 6765 2062 696e 730a 0a20 2020 2020 2020  ge bins..       
+00004e20: 2023 2043 7265 6174 6520 666c 6f77 730a   # Create flows.
+00004e30: 2020 2020 2020 2020 666f 7220 666c 6f77          for flow
+00004e40: 2069 6e20 6870 642e 666c 6f77 733a 0a20   in hpd.flows:. 
+00004e50: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00004e60: 7473 5b66 6c6f 772e 6e61 6d65 5d20 2020  ts[flow.name]   
+00004e70: 2020 2020 2020 2020 2020 2020 2020 203d                 =
+00004e80: 2069 6e69 745f 7265 7328 666c 6f77 2e6c   init_res(flow.l
+00004e90: 6162 656c 2c20 636f 6c6f 723d 666c 6f77  abel, color=flow
+00004ea0: 2e63 6f6c 6f72 290a 2020 2020 2020 2020  .color).        
+00004eb0: 2020 2020 7265 7375 6c74 735b 666c 6f77      results[flow
+00004ec0: 2e6e 616d 652b 275f 6279 5f67 656e 6f74  .name+'_by_genot
+00004ed0: 7970 6527 5d20 2020 3d20 696e 6974 5f72  ype']   = init_r
+00004ee0: 6573 2866 6c6f 772e 6c61 6265 6c2b 2720  es(flow.label+' 
+00004ef0: 6279 2067 656e 6f74 7970 6527 2c20 6e5f  by genotype', n_
+00004f00: 726f 7773 3d6e 6729 0a20 2020 2020 2020  rows=ng).       
+00004f10: 2020 2020 2072 6573 756c 7473 5b66 6c6f       results[flo
+00004f20: 772e 6e61 6d65 2b27 5f62 795f 6167 6527  w.name+'_by_age'
+00004f30: 5d20 2020 2020 2020 203d 2069 6e69 745f  ]        = init_
+00004f40: 7265 7328 666c 6f77 2e6c 6162 656c 2b27  res(flow.label+'
+00004f50: 2062 7920 6167 6527 2c20 6e5f 726f 7773   by age', n_rows
+00004f60: 3d6e 612c 2063 6f6c 6f72 3d66 6c6f 772e  =na, color=flow.
+00004f70: 636f 6c6f 7229 0a0a 2020 2020 2020 2020  color)..        
+00004f80: 2320 4372 6561 7465 2073 746f 636b 730a  # Create stocks.
+00004f90: 2020 2020 2020 2020 666f 7220 7374 6f63          for stoc
+00004fa0: 6b20 696e 2068 7064 2e50 656f 706c 654d  k in hpd.PeopleM
+00004fb0: 6574 6128 292e 7374 6f63 6b5f 7374 6174  eta().stock_stat
+00004fc0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00004fd0: 7265 7375 6c74 735b 6627 6e5f 7b73 746f  results[f'n_{sto
+00004fe0: 636b 2e6e 616d 657d 275d 2020 2020 2020  ck.name}']      
+00004ff0: 2020 2020 2020 2020 3d20 696e 6974 5f72          = init_r
+00005000: 6573 2873 746f 636b 2e6c 6162 656c 2c20  es(stock.label, 
+00005010: 636f 6c6f 723d 7374 6f63 6b2e 636f 6c6f  color=stock.colo
+00005020: 7229 0a20 2020 2020 2020 2020 2020 2072  r).            r
+00005030: 6573 756c 7473 5b66 276e 5f7b 7374 6f63  esults[f'n_{stoc
+00005040: 6b2e 6e61 6d65 7d5f 6279 5f67 656e 6f74  k.name}_by_genot
+00005050: 7970 6527 5d20 203d 2069 6e69 745f 7265  ype']  = init_re
+00005060: 7328 7374 6f63 6b2e 6c61 6265 6c2b 2720  s(stock.label+' 
+00005070: 6279 2067 656e 6f74 7970 6527 2c20 6e5f  by genotype', n_
+00005080: 726f 7773 3d6e 6729 0a0a 2020 2020 2020  rows=ng)..      
+00005090: 2020 2320 4f6e 6c79 2062 792d 6167 6520    # Only by-age 
+000050a0: 7374 6f63 6b20 7265 7375 6c74 2077 6520  stock result we 
+000050b0: 7769 6c6c 206e 6565 6420 6973 206e 756d  will need is num
+000050c0: 6265 7220 696e 6665 6374 696f 7573 2c20  ber infectious, 
+000050d0: 7375 7363 6570 7469 626c 652c 2061 6e64  susceptible, and
+000050e0: 2077 6974 6820 6369 6e2c 2066 6f72 2048   with cin, for H
+000050f0: 5056 2061 6e64 2043 494e 2070 7265 7661  PV and CIN preva
+00005100: 6c65 6e63 652f 696e 6369 6465 6e63 6520  lence/incidence 
+00005110: 6361 6c63 756c 6174 696f 6e73 0a20 2020  calculations.   
+00005120: 2020 2020 2072 6573 756c 7473 5b66 276e       results[f'n
+00005130: 5f69 6e66 6563 7469 6f75 735f 6279 5f61  _infectious_by_a
+00005140: 6765 275d 2020 2020 2020 2020 2020 2020  ge']            
+00005150: 203d 2069 6e69 745f 7265 7328 274e 756d   = init_res('Num
+00005160: 6265 7220 696e 6665 6374 696f 7573 2062  ber infectious b
+00005170: 7920 6167 6527 2c20 6e5f 726f 7773 3d6e  y age', n_rows=n
+00005180: 612c 2063 6f6c 6f72 3d73 746f 636b 2e63  a, color=stock.c
+00005190: 6f6c 6f72 290a 2020 2020 2020 2020 7265  olor).        re
+000051a0: 7375 6c74 735b 6627 6e5f 6665 6d61 6c65  sults[f'n_female
+000051b0: 735f 696e 6665 6374 696f 7573 5f62 795f  s_infectious_by_
+000051c0: 6167 6527 5d20 2020 2020 3d20 696e 6974  age']     = init
+000051d0: 5f72 6573 2827 4e75 6d62 6572 206f 6620  _res('Number of 
+000051e0: 6665 6d61 6c65 7320 696e 6665 6374 696f  females infectio
+000051f0: 7573 2062 7920 6167 6527 2c20 6e5f 726f  us by age', n_ro
+00005200: 7773 3d6e 612c 2063 6f6c 6f72 3d73 746f  ws=na, color=sto
+00005210: 636b 2e63 6f6c 6f72 290a 2020 2020 2020  ck.color).      
+00005220: 2020 7265 7375 6c74 735b 6627 6e5f 7375    results[f'n_su
+00005230: 7363 6570 7469 626c 655f 6279 5f61 6765  sceptible_by_age
+00005240: 275d 2020 2020 2020 2020 2020 2020 3d20  ']            = 
+00005250: 696e 6974 5f72 6573 2827 4e75 6d62 6572  init_res('Number
+00005260: 2073 7573 6365 7074 6962 6c65 2062 7920   susceptible by 
+00005270: 6167 6527 2c20 6e5f 726f 7773 3d6e 612c  age', n_rows=na,
+00005280: 2063 6f6c 6f72 3d73 746f 636b 2e63 6f6c   color=stock.col
+00005290: 6f72 290a 2020 2020 2020 2020 7265 7375  or).        resu
+000052a0: 6c74 735b 6627 6e5f 7472 616e 7366 6f72  lts[f'n_transfor
+000052b0: 6d65 645f 6279 5f61 6765 275d 2020 2020  med_by_age']    
+000052c0: 2020 2020 2020 2020 3d20 696e 6974 5f72          = init_r
+000052d0: 6573 2827 4e75 6d62 6572 2074 7261 6e73  es('Number trans
+000052e0: 666f 726d 6564 2062 7920 6167 6527 2c20  formed by age', 
+000052f0: 6e5f 726f 7773 3d6e 612c 2063 6f6c 6f72  n_rows=na, color
+00005300: 3d73 746f 636b 2e63 6f6c 6f72 290a 2020  =stock.color).  
+00005310: 2020 2020 2020 7265 7375 6c74 735b 6627        results[f'
+00005320: 6e5f 7072 6563 696e 5f62 795f 6167 6527  n_precin_by_age'
+00005330: 5d20 2020 2020 2020 2020 2020 2020 2020  ]               
+00005340: 2020 3d20 696e 6974 5f72 6573 2827 4e75    = init_res('Nu
+00005350: 6d62 6572 2050 7265 2d43 494e 2062 7920  mber Pre-CIN by 
+00005360: 6167 6527 2c20 6e5f 726f 7773 3d6e 612c  age', n_rows=na,
+00005370: 2063 6f6c 6f72 3d73 746f 636b 2e63 6f6c   color=stock.col
+00005380: 6f72 290a 2020 2020 2020 2020 7265 7375  or).        resu
+00005390: 6c74 735b 6627 6e5f 6369 6e31 5f62 795f  lts[f'n_cin1_by_
+000053a0: 6167 6527 5d20 2020 2020 2020 2020 2020  age']           
+000053b0: 2020 2020 2020 2020 3d20 696e 6974 5f72          = init_r
+000053c0: 6573 2827 4e75 6d62 6572 2043 494e 3120  es('Number CIN1 
+000053d0: 6279 2061 6765 272c 206e 5f72 6f77 733d  by age', n_rows=
+000053e0: 6e61 2c20 636f 6c6f 723d 7374 6f63 6b2e  na, color=stock.
+000053f0: 636f 6c6f 7229 0a20 2020 2020 2020 2072  color).        r
+00005400: 6573 756c 7473 5b66 276e 5f63 696e 325f  esults[f'n_cin2_
+00005410: 6279 5f61 6765 275d 2020 2020 2020 2020  by_age']        
+00005420: 2020 2020 2020 2020 2020 203d 2069 6e69             = ini
+00005430: 745f 7265 7328 274e 756d 6265 7220 4349  t_res('Number CI
+00005440: 4e32 2062 7920 6167 6527 2c20 6e5f 726f  N2 by age', n_ro
+00005450: 7773 3d6e 612c 2063 6f6c 6f72 3d73 746f  ws=na, color=sto
+00005460: 636b 2e63 6f6c 6f72 290a 2020 2020 2020  ck.color).      
+00005470: 2020 7265 7375 6c74 735b 6627 6e5f 6369    results[f'n_ci
+00005480: 6e33 5f62 795f 6167 6527 5d20 2020 2020  n3_by_age']     
+00005490: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+000054a0: 696e 6974 5f72 6573 2827 4e75 6d62 6572  init_res('Number
+000054b0: 2043 494e 3320 6279 2061 6765 272c 206e   CIN3 by age', n
+000054c0: 5f72 6f77 733d 6e61 2c20 636f 6c6f 723d  _rows=na, color=
+000054d0: 7374 6f63 6b2e 636f 6c6f 7229 0a0a 2020  stock.color)..  
+000054e0: 2020 2020 2020 2320 4372 6561 7465 2069        # Create i
+000054f0: 6e63 6964 656e 6365 2061 6e64 2070 7265  ncidence and pre
+00005500: 7661 6c65 6e63 6520 7265 7375 6c74 730a  valence results.
+00005510: 2020 2020 2020 2020 666f 7220 7661 722c          for var,
+00005520: 6e61 6d65 2c63 6f6c 6f72 2069 6e20 7a69  name,color in zi
+00005530: 7028 6870 642e 696e 6369 5f6b 6579 732c  p(hpd.inci_keys,
+00005540: 2068 7064 2e69 6e63 695f 6e61 6d65 732c   hpd.inci_names,
+00005550: 2068 7064 2e69 6e63 695f 636f 6c6f 7273   hpd.inci_colors
+00005560: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00005570: 6573 756c 7473 5b66 277b 7661 727d 5f69  esults[f'{var}_i
+00005580: 6e63 6964 656e 6365 275d 2020 2020 2020  ncidence']      
+00005590: 2020 2020 2020 203d 2069 6e69 745f 7265         = init_re
+000055a0: 7328 6e61 6d65 2b27 2069 6e63 6964 656e  s(name+' inciden
+000055b0: 6365 272c 2063 6f6c 6f72 3d63 6f6c 6f72  ce', color=color
+000055c0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000055d0: 7375 6c74 735b 6627 7b76 6172 7d5f 696e  sults[f'{var}_in
+000055e0: 6369 6465 6e63 655f 6279 5f67 656e 6f74  cidence_by_genot
+000055f0: 7970 6527 5d20 3d20 696e 6974 5f72 6573  ype'] = init_res
+00005600: 286e 616d 652b 2720 696e 6369 6465 6e63  (name+' incidenc
+00005610: 6520 6279 2067 656e 6f74 7970 6527 2c20  e by genotype', 
+00005620: 6e5f 726f 7773 3d6e 6729 0a20 2020 2020  n_rows=ng).     
+00005630: 2020 2020 2020 2072 6573 756c 7473 5b66         results[f
+00005640: 277b 7661 727d 5f69 6e63 6964 656e 6365  '{var}_incidence
+00005650: 5f62 795f 6167 6527 5d20 2020 2020 203d  _by_age']      =
+00005660: 2069 6e69 745f 7265 7328 6e61 6d65 2b27   init_res(name+'
+00005670: 2069 6e63 6964 656e 6365 2062 7920 6167   incidence by ag
+00005680: 6527 2c20 6e5f 726f 7773 3d6e 612c 2063  e', n_rows=na, c
+00005690: 6f6c 6f72 3d63 6f6c 6f72 290a 0a20 2020  olor=color)..   
+000056a0: 2020 2020 2023 2043 7265 6174 6520 6465       # Create de
+000056b0: 6d6f 6772 6170 6869 6320 666c 6f77 730a  mographic flows.
+000056c0: 2020 2020 2020 2020 666f 7220 7661 722c          for var,
+000056d0: 206e 616d 652c 2063 6f6c 6f72 2069 6e20   name, color in 
+000056e0: 7a69 7028 6870 642e 6465 6d5f 6b65 7973  zip(hpd.dem_keys
+000056f0: 2c20 6870 642e 6465 6d5f 6e61 6d65 732c  , hpd.dem_names,
+00005700: 2068 7064 2e64 656d 5f63 6f6c 6f72 7329   hpd.dem_colors)
+00005710: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00005720: 7375 6c74 735b 7661 725d 203d 2069 6e69  sults[var] = ini
+00005730: 745f 7265 7328 6e61 6d65 2c20 636f 6c6f  t_res(name, colo
+00005740: 723d 636f 6c6f 7229 0a0a 2020 2020 2020  r=color)..      
+00005750: 2020 2320 4372 6561 7465 2072 6573 756c    # Create resul
+00005760: 7473 2062 7920 7365 780a 2020 2020 2020  ts by sex.      
+00005770: 2020 666f 7220 7661 722c 206e 616d 652c    for var, name,
+00005780: 2063 6f6c 6f72 2069 6e20 7a69 7028 6870   color in zip(hp
+00005790: 642e 6279 5f73 6578 5f6b 6579 732c 2068  d.by_sex_keys, h
+000057a0: 7064 2e62 795f 7365 785f 636f 6c6f 7273  pd.by_sex_colors
+000057b0: 2c20 6870 642e 6279 5f73 6578 5f63 6f6c  , hpd.by_sex_col
+000057c0: 6f72 7329 3a0a 2020 2020 2020 2020 2020  ors):.          
+000057d0: 2020 7265 7375 6c74 735b 7661 725d 203d    results[var] =
+000057e0: 2069 6e69 745f 7265 7328 6e61 6d65 2c20   init_res(name, 
+000057f0: 636f 6c6f 723d 636f 6c6f 722c 206e 5f72  color=color, n_r
+00005800: 6f77 733d 3229 0a0a 2020 2020 2020 2020  ows=2)..        
+00005810: 2320 4372 6561 7465 2041 5352 2072 6573  # Create ASR res
+00005820: 756c 7473 2075 7369 6e67 2073 7461 6e64  ults using stand
+00005830: 6172 6420 706f 7075 6c61 7469 6f6e 730a  ard populations.
+00005840: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
+00005850: 2761 7372 5f63 616e 6365 725f 696e 6369  'asr_cancer_inci
+00005860: 6465 6e63 6527 5d20 3d20 696e 6974 5f72  dence'] = init_r
+00005870: 6573 2827 4167 652d 6164 6a75 7374 6564  es('Age-adjusted
+00005880: 2063 6572 7669 6361 6c20 6361 6e63 6572   cervical cancer
+00005890: 2069 6e63 6964 656e 6365 272c 2073 6361   incidence', sca
+000058a0: 6c65 3d46 616c 7365 290a 2020 2020 2020  le=False).      
+000058b0: 2020 7265 7375 6c74 735b 2761 7372 5f63    results['asr_c
+000058c0: 616e 6365 725f 6d6f 7274 616c 6974 7927  ancer_mortality'
+000058d0: 5d20 3d20 696e 6974 5f72 6573 2827 4167  ] = init_res('Ag
+000058e0: 652d 6164 6a75 7374 6564 2063 6572 7669  e-adjusted cervi
+000058f0: 6361 6c20 6361 6e63 6572 206d 6f72 7461  cal cancer morta
+00005900: 6c69 7479 272c 2073 6361 6c65 3d46 616c  lity', scale=Fal
+00005910: 7365 290a 0a20 2020 2020 2020 2073 746f  se)..        sto
+00005920: 636b 5f63 6f6c 6f72 7320 3d20 5b69 2066  ck_colors = [i f
+00005930: 6f72 2069 2069 6e20 7365 7428 6870 642e  or i in set(hpd.
+00005940: 5065 6f70 6c65 4d65 7461 2829 2e73 746f  PeopleMeta().sto
+00005950: 636b 5f63 6f6c 6f72 7329 2069 6620 6920  ck_colors) if i 
+00005960: 6973 206e 6f74 204e 6f6e 655d 0a0a 2020  is not None]..  
+00005970: 2020 2020 2020 2320 5479 7065 2064 6973        # Type dis
+00005980: 7472 6962 7574 696f 6e73 2062 7920 6379  tributions by cy
+00005990: 746f 6c6f 6779 0a20 2020 2020 2020 2066  tology.        f
+000059a0: 6f72 2076 6172 2c20 6e61 6d65 2069 6e20  or var, name in 
+000059b0: 7a69 7028 6870 642e 7479 7065 5f64 6973  zip(hpd.type_dis
+000059c0: 745f 6b65 7973 2c20 6870 642e 7479 7065  t_keys, hpd.type
+000059d0: 5f64 6973 745f 6e61 6d65 7329 3a0a 2020  _dist_names):.  
+000059e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000059f0: 735b 7661 722b 275f 6765 6e6f 7479 7065  s[var+'_genotype
+00005a00: 5f64 6973 7427 5d20 3d20 696e 6974 5f72  _dist'] = init_r
+00005a10: 6573 286e 616d 652c 206e 5f72 6f77 733d  es(name, n_rows=
+00005a20: 6e67 2c20 636f 6c6f 723d 7374 6f63 6b5f  ng, color=stock_
+00005a30: 636f 6c6f 7273 5b30 5d29 0a0a 2020 2020  colors[0])..    
+00005a40: 2020 2020 2320 5661 6363 696e 6174 696f      # Vaccinatio
+00005a50: 6e20 7265 7375 6c74 730a 2020 2020 2020  n results.      
+00005a60: 2020 7265 7375 6c74 735b 276e 6577 5f76    results['new_v
+00005a70: 6163 6369 6e61 7465 6427 5d20 3d20 696e  accinated'] = in
+00005a80: 6974 5f72 6573 2827 4e65 776c 7920 7661  it_res('Newly va
+00005a90: 6363 696e 6174 6564 2062 7920 6765 6e6f  ccinated by geno
+00005aa0: 7479 7065 272c 206e 5f72 6f77 733d 6e67  type', n_rows=ng
+00005ab0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+00005ac0: 735b 276e 6577 5f74 6f74 616c 5f76 6163  s['new_total_vac
+00005ad0: 6369 6e61 7465 6427 5d20 3d20 696e 6974  cinated'] = init
+00005ae0: 5f72 6573 2827 4e65 776c 7920 7661 6363  _res('Newly vacc
+00005af0: 696e 6174 6564 2729 0a20 2020 2020 2020  inated').       
+00005b00: 2072 6573 756c 7473 5b27 6375 6d5f 7661   results['cum_va
+00005b10: 6363 696e 6174 6564 275d 203d 2069 6e69  ccinated'] = ini
+00005b20: 745f 7265 7328 2743 756d 756c 6174 6976  t_res('Cumulativ
+00005b30: 6520 6e75 6d62 6572 2076 6163 6369 6e61  e number vaccina
+00005b40: 7465 6420 6279 2067 656e 6f74 7970 6527  ted by genotype'
+00005b50: 2c20 6e5f 726f 7773 3d6e 6729 0a20 2020  , n_rows=ng).   
+00005b60: 2020 2020 2072 6573 756c 7473 5b27 6375       results['cu
+00005b70: 6d5f 746f 7461 6c5f 7661 6363 696e 6174  m_total_vaccinat
+00005b80: 6564 275d 203d 2069 6e69 745f 7265 7328  ed'] = init_res(
+00005b90: 2743 756d 756c 6174 6976 6520 6e75 6d62  'Cumulative numb
+00005ba0: 6572 2076 6163 6369 6e61 7465 6427 290a  er vaccinated').
+00005bb0: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
+00005bc0: 276e 6577 5f64 6f73 6573 275d 203d 2069  'new_doses'] = i
+00005bd0: 6e69 745f 7265 7328 274e 6577 2064 6f73  nit_res('New dos
+00005be0: 6573 2729 0a20 2020 2020 2020 2072 6573  es').        res
+00005bf0: 756c 7473 5b27 6375 6d5f 646f 7365 7327  ults['cum_doses'
+00005c00: 5d20 3d20 696e 6974 5f72 6573 2827 4375  ] = init_res('Cu
+00005c10: 6d75 6c61 7469 7665 2064 6f73 6573 2729  mulative doses')
+00005c20: 0a0a 2020 2020 2020 2020 2320 5468 6572  ..        # Ther
+00005c30: 6170 6575 7469 6320 7661 6363 696e 6520  apeutic vaccine 
+00005c40: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
+00005c50: 7265 7375 6c74 735b 276e 6577 5f74 7876  results['new_txv
+00005c60: 785f 646f 7365 7327 5d20 3d20 696e 6974  x_doses'] = init
+00005c70: 5f72 6573 2827 4e65 7720 7468 6572 6170  _res('New therap
+00005c80: 6575 7469 6320 7661 6363 696e 6520 646f  eutic vaccine do
+00005c90: 7365 7327 290a 2020 2020 2020 2020 7265  ses').        re
+00005ca0: 7375 6c74 735b 276e 6577 5f74 785f 7661  sults['new_tx_va
+00005cb0: 6363 696e 6174 6564 275d 203d 2069 6e69  ccinated'] = ini
+00005cc0: 745f 7265 7328 274e 6577 6c79 2072 6563  t_res('Newly rec
+00005cd0: 6569 7665 6420 7468 6572 6170 6575 7469  eived therapeuti
+00005ce0: 6320 7661 6363 696e 6527 290a 2020 2020  c vaccine').    
+00005cf0: 2020 2020 7265 7375 6c74 735b 2763 756d      results['cum
+00005d00: 5f74 7876 785f 646f 7365 7327 5d20 3d20  _txvx_doses'] = 
+00005d10: 696e 6974 5f72 6573 2827 4375 6d75 6c61  init_res('Cumula
+00005d20: 7469 7665 2074 6865 7261 7065 7574 6963  tive therapeutic
+00005d30: 2076 6163 6369 6e65 2064 6f73 6573 2729   vaccine doses')
+00005d40: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00005d50: 5b27 6375 6d5f 7478 5f76 6163 6369 6e61  ['cum_tx_vaccina
+00005d60: 7465 6427 5d20 3d20 696e 6974 5f72 6573  ted'] = init_res
+00005d70: 2827 546f 7461 6c20 7265 6365 6976 6564  ('Total received
+00005d80: 2074 6865 7261 7065 7574 6963 2076 6163   therapeutic vac
+00005d90: 6369 6e65 2729 0a0a 2020 2020 2020 2020  cine')..        
+00005da0: 2320 5363 7265 656e 2026 2074 7265 6174  # Screen & treat
+00005db0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+00005dc0: 2072 6573 756c 7473 5b27 6e65 775f 7363   results['new_sc
+00005dd0: 7265 656e 7327 5d20 3d20 696e 6974 5f72  reens'] = init_r
+00005de0: 6573 2827 4e65 7720 7363 7265 656e 7327  es('New screens'
+00005df0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+00005e00: 735b 276e 6577 5f73 6372 6565 6e65 6427  s['new_screened'
+00005e10: 5d20 3d20 696e 6974 5f72 6573 2827 4e65  ] = init_res('Ne
+00005e20: 776c 7920 7363 7265 656e 6564 2729 0a20  wly screened'). 
+00005e30: 2020 2020 2020 2072 6573 756c 7473 5b27         results['
+00005e40: 6e65 775f 6369 6e5f 7472 6561 746d 656e  new_cin_treatmen
+00005e50: 7473 275d 203d 2069 6e69 745f 7265 7328  ts'] = init_res(
+00005e60: 274e 6577 2043 494e 2074 7265 6174 6d65  'New CIN treatme
+00005e70: 6e74 7327 290a 2020 2020 2020 2020 7265  nts').        re
+00005e80: 7375 6c74 735b 276e 6577 5f63 696e 5f74  sults['new_cin_t
+00005e90: 7265 6174 6564 275d 203d 2069 6e69 745f  reated'] = init_
+00005ea0: 7265 7328 274e 6577 6c79 2074 7265 6174  res('Newly treat
+00005eb0: 6564 2066 6f72 2043 494e 7327 290a 2020  ed for CINs').  
+00005ec0: 2020 2020 2020 7265 7375 6c74 735b 276e        results['n
+00005ed0: 6577 5f63 616e 6365 725f 7472 6561 746d  ew_cancer_treatm
+00005ee0: 656e 7473 275d 203d 2069 6e69 745f 7265  ents'] = init_re
+00005ef0: 7328 274e 6577 2063 616e 6365 7220 7472  s('New cancer tr
+00005f00: 6561 746d 656e 7473 2729 0a20 2020 2020  eatments').     
+00005f10: 2020 2072 6573 756c 7473 5b27 6e65 775f     results['new_
+00005f20: 6361 6e63 6572 5f74 7265 6174 6564 275d  cancer_treated']
+00005f30: 203d 2069 6e69 745f 7265 7328 274e 6577   = init_res('New
+00005f40: 6c79 2074 7265 6174 6564 2066 6f72 2063  ly treated for c
+00005f50: 616e 6365 7227 290a 2020 2020 2020 2020  ancer').        
+00005f60: 7265 7375 6c74 735b 2763 756d 5f73 6372  results['cum_scr
+00005f70: 6565 6e73 275d 203d 2069 6e69 745f 7265  eens'] = init_re
+00005f80: 7328 2743 756d 756c 6174 6976 6520 7363  s('Cumulative sc
+00005f90: 7265 656e 7327 290a 2020 2020 2020 2020  reens').        
+00005fa0: 7265 7375 6c74 735b 2763 756d 5f73 6372  results['cum_scr
+00005fb0: 6565 6e65 6427 5d20 3d20 696e 6974 5f72  eened'] = init_r
+00005fc0: 6573 2827 4375 6d75 6c61 7469 7665 206e  es('Cumulative n
+00005fd0: 756d 6265 7220 7363 7265 656e 6564 2729  umber screened')
+00005fe0: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00005ff0: 5b27 6375 6d5f 6369 6e5f 7472 6561 746d  ['cum_cin_treatm
+00006000: 656e 7473 275d 203d 2069 6e69 745f 7265  ents'] = init_re
+00006010: 7328 2743 756d 756c 6174 6976 6520 4349  s('Cumulative CI
+00006020: 4e20 7472 6561 746d 656e 7473 2729 0a20  N treatments'). 
+00006030: 2020 2020 2020 2072 6573 756c 7473 5b27         results['
+00006040: 6375 6d5f 6369 6e5f 7472 6561 7465 6427  cum_cin_treated'
+00006050: 5d20 3d20 696e 6974 5f72 6573 2827 4375  ] = init_res('Cu
+00006060: 6d75 6c61 7469 7665 206e 756d 6265 7220  mulative number 
+00006070: 7472 6561 7465 6420 666f 7220 4349 4e73  treated for CINs
+00006080: 2729 0a20 2020 2020 2020 2072 6573 756c  ').        resul
+00006090: 7473 5b27 6375 6d5f 6361 6e63 6572 5f74  ts['cum_cancer_t
+000060a0: 7265 6174 6d65 6e74 7327 5d20 3d20 696e  reatments'] = in
+000060b0: 6974 5f72 6573 2827 4375 6d75 6c61 7469  it_res('Cumulati
+000060c0: 7665 2063 616e 6365 7220 7472 6561 746d  ve cancer treatm
+000060d0: 656e 7473 2729 0a20 2020 2020 2020 2072  ents').        r
+000060e0: 6573 756c 7473 5b27 6375 6d5f 6361 6e63  esults['cum_canc
+000060f0: 6572 5f74 7265 6174 6564 275d 203d 2069  er_treated'] = i
+00006100: 6e69 745f 7265 7328 2743 756d 756c 6174  nit_res('Cumulat
+00006110: 6976 6520 6e75 6d62 6572 2074 7265 6174  ive number treat
+00006120: 6564 2066 6f72 2063 616e 6365 7227 290a  ed for cancer').
+00006130: 0a20 2020 2020 2020 2023 2041 6464 6974  .        # Addit
+00006140: 696f 6e61 6c20 6361 6e63 6572 2072 6573  ional cancer res
+00006150: 756c 7473 0a20 2020 2020 2020 2072 6573  ults.        res
+00006160: 756c 7473 5b27 6465 7465 6374 6564 5f63  ults['detected_c
+00006170: 616e 6365 725f 696e 6369 6465 6e63 6527  ancer_incidence'
+00006180: 5d20 3d20 696e 6974 5f72 6573 2827 4465  ] = init_res('De
+00006190: 7465 6374 6564 2063 616e 6365 7220 696e  tected cancer in
+000061a0: 6369 6465 6e63 6527 2c20 636f 6c6f 723d  cidence', color=
+000061b0: 2723 6663 6261 3033 2729 0a20 2020 2020  '#fcba03').     
+000061c0: 2020 2072 6573 756c 7473 5b27 6361 6e63     results['canc
+000061d0: 6572 5f6d 6f72 7461 6c69 7479 275d 203d  er_mortality'] =
+000061e0: 2069 6e69 745f 7265 7328 2743 616e 6365   init_res('Cance
+000061f0: 7220 6d6f 7274 616c 6974 7927 290a 0a20  r mortality').. 
+00006200: 2020 2020 2020 2023 204f 7468 6572 2072         # Other r
+00006210: 6573 756c 7473 0a20 2020 2020 2020 2072  esults.        r
+00006220: 6573 756c 7473 5b27 6e5f 616c 6976 6527  esults['n_alive'
+00006230: 5d20 3d20 696e 6974 5f72 6573 2827 4e75  ] = init_res('Nu
+00006240: 6d62 6572 2061 6c69 7665 2729 0a20 2020  mber alive').   
+00006250: 2020 2020 2072 6573 756c 7473 5b27 6e5f       results['n_
+00006260: 616c 6976 655f 6279 5f73 6578 275d 203d  alive_by_sex'] =
+00006270: 2069 6e69 745f 7265 7328 274e 756d 6265   init_res('Numbe
+00006280: 7220 616c 6976 6520 6279 2073 6578 272c  r alive by sex',
+00006290: 206e 5f72 6f77 733d 3229 0a20 2020 2020   n_rows=2).     
+000062a0: 2020 2072 6573 756c 7473 5b27 6e5f 616c     results['n_al
+000062b0: 6976 655f 6279 5f61 6765 275d 203d 2069  ive_by_age'] = i
+000062c0: 6e69 745f 7265 7328 274e 756d 6265 7220  nit_res('Number 
+000062d0: 616c 6976 6520 6279 2061 6765 272c 206e  alive by age', n
+000062e0: 5f72 6f77 733d 6e61 290a 2020 2020 2020  _rows=na).      
+000062f0: 2020 7265 7375 6c74 735b 276e 5f66 656d    results['n_fem
+00006300: 616c 6573 5f61 6c69 7665 5f62 795f 6167  ales_alive_by_ag
+00006310: 6527 5d20 3d20 696e 6974 5f72 6573 2827  e'] = init_res('
+00006320: 4e75 6d62 6572 2066 656d 616c 6573 2061  Number females a
+00006330: 6c69 7665 2062 7920 6167 6527 2c20 6e5f  live by age', n_
+00006340: 726f 7773 3d6e 6129 0a20 2020 2020 2020  rows=na).       
+00006350: 2072 6573 756c 7473 5b27 6364 7227 5d20   results['cdr'] 
+00006360: 3d20 696e 6974 5f72 6573 2827 4372 7564  = init_res('Crud
+00006370: 6520 6465 6174 6820 7261 7465 272c 2073  e death rate', s
+00006380: 6361 6c65 3d46 616c 7365 290a 2020 2020  cale=False).    
+00006390: 2020 2020 7265 7375 6c74 735b 2763 6272      results['cbr
+000063a0: 275d 203d 2069 6e69 745f 7265 7328 2743  '] = init_res('C
+000063b0: 7275 6465 2062 6972 7468 2072 6174 6527  rude birth rate'
+000063c0: 2c20 7363 616c 653d 4661 6c73 652c 2063  , scale=False, c
+000063d0: 6f6c 6f72 3d27 2366 6362 6130 3327 290a  olor='#fcba03').
+000063e0: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
+000063f0: 2768 7076 5f70 7265 7661 6c65 6e63 6527  'hpv_prevalence'
+00006400: 5d20 3d20 696e 6974 5f72 6573 2827 4850  ] = init_res('HP
+00006410: 5620 7072 6576 616c 656e 6365 272c 2063  V prevalence', c
+00006420: 6f6c 6f72 3d73 746f 636b 5f63 6f6c 6f72  olor=stock_color
+00006430: 735b 305d 290a 2020 2020 2020 2020 7265  s[0]).        re
+00006440: 7375 6c74 735b 2768 7076 5f70 7265 7661  sults['hpv_preva
+00006450: 6c65 6e63 655f 6279 5f67 656e 6f74 7970  lence_by_genotyp
+00006460: 6527 5d20 3d20 696e 6974 5f72 6573 2827  e'] = init_res('
+00006470: 4850 5620 7072 6576 616c 656e 6365 272c  HPV prevalence',
+00006480: 206e 5f72 6f77 733d 6e67 2c20 636f 6c6f   n_rows=ng, colo
+00006490: 723d 7374 6f63 6b5f 636f 6c6f 7273 5b30  r=stock_colors[0
+000064a0: 5d29 0a20 2020 2020 2020 2072 6573 756c  ]).        resul
+000064b0: 7473 5b27 6870 765f 7072 6576 616c 656e  ts['hpv_prevalen
+000064c0: 6365 5f62 795f 6167 6527 5d20 3d20 696e  ce_by_age'] = in
+000064d0: 6974 5f72 6573 2827 4850 5620 7072 6576  it_res('HPV prev
+000064e0: 616c 656e 6365 2062 7920 6167 6527 2c20  alence by age', 
+000064f0: 6e5f 726f 7773 3d6e 612c 2063 6f6c 6f72  n_rows=na, color
+00006500: 3d73 746f 636b 5f63 6f6c 6f72 735b 305d  =stock_colors[0]
+00006510: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+00006520: 735b 2770 7265 6369 6e5f 7072 6576 616c  s['precin_preval
+00006530: 656e 6365 275d 203d 2069 6e69 745f 7265  ence'] = init_re
+00006540: 7328 2750 7265 2d43 494e 2070 7265 7661  s('Pre-CIN preva
+00006550: 6c65 6e63 6527 2c20 636f 6c6f 723d 7374  lence', color=st
+00006560: 6f63 6b5f 636f 6c6f 7273 5b30 5d29 0a20  ock_colors[0]). 
+00006570: 2020 2020 2020 2072 6573 756c 7473 5b27         results['
+00006580: 7072 6563 696e 5f70 7265 7661 6c65 6e63  precin_prevalenc
+00006590: 655f 6279 5f67 656e 6f74 7970 6527 5d20  e_by_genotype'] 
+000065a0: 3d20 696e 6974 5f72 6573 2827 5072 652d  = init_res('Pre-
+000065b0: 4349 4e20 7072 6576 616c 656e 6365 2062  CIN prevalence b
+000065c0: 7920 6765 6e6f 7479 7065 272c 206e 5f72  y genotype', n_r
+000065d0: 6f77 733d 6e67 2c20 636f 6c6f 723d 7374  ows=ng, color=st
+000065e0: 6f63 6b5f 636f 6c6f 7273 5b30 5d29 0a20  ock_colors[0]). 
+000065f0: 2020 2020 2020 2072 6573 756c 7473 5b27         results['
+00006600: 7072 6563 696e 5f70 7265 7661 6c65 6e63  precin_prevalenc
+00006610: 655f 6279 5f61 6765 275d 203d 2069 6e69  e_by_age'] = ini
+00006620: 745f 7265 7328 2750 7265 2d43 494e 2070  t_res('Pre-CIN p
+00006630: 7265 7661 6c65 6e63 6520 6279 2061 6765  revalence by age
+00006640: 272c 206e 5f72 6f77 733d 6e61 2c20 636f  ', n_rows=na, co
+00006650: 6c6f 723d 7374 6f63 6b5f 636f 6c6f 7273  lor=stock_colors
+00006660: 5b30 5d29 0a20 2020 2020 2020 2072 6573  [0]).        res
+00006670: 756c 7473 5b27 6369 6e31 5f70 7265 7661  ults['cin1_preva
+00006680: 6c65 6e63 6527 5d20 3d20 696e 6974 5f72  lence'] = init_r
+00006690: 6573 2827 4349 4e31 2070 7265 7661 6c65  es('CIN1 prevale
+000066a0: 6e63 6527 2c20 636f 6c6f 723d 7374 6f63  nce', color=stoc
+000066b0: 6b5f 636f 6c6f 7273 5b31 5d29 0a20 2020  k_colors[1]).   
+000066c0: 2020 2020 2072 6573 756c 7473 5b27 6369       results['ci
+000066d0: 6e31 5f70 7265 7661 6c65 6e63 655f 6279  n1_prevalence_by
+000066e0: 5f67 656e 6f74 7970 6527 5d20 3d20 696e  _genotype'] = in
+000066f0: 6974 5f72 6573 2827 4349 4e31 2070 7265  it_res('CIN1 pre
+00006700: 7661 6c65 6e63 6520 6279 2067 656e 6f74  valence by genot
+00006710: 7970 6527 2c20 6e5f 726f 7773 3d6e 672c  ype', n_rows=ng,
+00006720: 2063 6f6c 6f72 3d73 746f 636b 5f63 6f6c   color=stock_col
+00006730: 6f72 735b 315d 290a 2020 2020 2020 2020  ors[1]).        
+00006740: 7265 7375 6c74 735b 2763 696e 315f 7072  results['cin1_pr
+00006750: 6576 616c 656e 6365 5f62 795f 6167 6527  evalence_by_age'
+00006760: 5d20 3d20 696e 6974 5f72 6573 2827 4349  ] = init_res('CI
+00006770: 4e31 2070 7265 7661 6c65 6e63 6520 6279  N1 prevalence by
+00006780: 2061 6765 272c 206e 5f72 6f77 733d 6e61   age', n_rows=na
+00006790: 2c20 636f 6c6f 723d 7374 6f63 6b5f 636f  , color=stock_co
+000067a0: 6c6f 7273 5b31 5d29 0a20 2020 2020 2020  lors[1]).       
+000067b0: 2072 6573 756c 7473 5b27 6369 6e32 5f70   results['cin2_p
+000067c0: 7265 7661 6c65 6e63 6527 5d20 3d20 696e  revalence'] = in
+000067d0: 6974 5f72 6573 2827 4349 4e32 2070 7265  it_res('CIN2 pre
+000067e0: 7661 6c65 6e63 6527 2c20 636f 6c6f 723d  valence', color=
+000067f0: 7374 6f63 6b5f 636f 6c6f 7273 5b32 5d29  stock_colors[2])
+00006800: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00006810: 5b27 6369 6e32 5f70 7265 7661 6c65 6e63  ['cin2_prevalenc
+00006820: 655f 6279 5f67 656e 6f74 7970 6527 5d20  e_by_genotype'] 
+00006830: 3d20 696e 6974 5f72 6573 2827 4349 4e32  = init_res('CIN2
+00006840: 2070 7265 7661 6c65 6e63 6520 6279 2067   prevalence by g
+00006850: 656e 6f74 7970 6527 2c20 6e5f 726f 7773  enotype', n_rows
+00006860: 3d6e 672c 2063 6f6c 6f72 3d73 746f 636b  =ng, color=stock
+00006870: 5f63 6f6c 6f72 735b 325d 290a 2020 2020  _colors[2]).    
+00006880: 2020 2020 7265 7375 6c74 735b 2763 696e      results['cin
+00006890: 325f 7072 6576 616c 656e 6365 5f62 795f  2_prevalence_by_
+000068a0: 6167 6527 5d20 3d20 696e 6974 5f72 6573  age'] = init_res
+000068b0: 2827 4349 4e32 2070 7265 7661 6c65 6e63  ('CIN2 prevalenc
+000068c0: 6520 6279 2061 6765 272c 206e 5f72 6f77  e by age', n_row
+000068d0: 733d 6e61 2c20 636f 6c6f 723d 7374 6f63  s=na, color=stoc
+000068e0: 6b5f 636f 6c6f 7273 5b32 5d29 0a20 2020  k_colors[2]).   
+000068f0: 2020 2020 2072 6573 756c 7473 5b27 6369       results['ci
+00006900: 6e33 5f70 7265 7661 6c65 6e63 6527 5d20  n3_prevalence'] 
+00006910: 3d20 696e 6974 5f72 6573 2827 4349 4e33  = init_res('CIN3
+00006920: 2070 7265 7661 6c65 6e63 6527 2c20 636f   prevalence', co
+00006930: 6c6f 723d 7374 6f63 6b5f 636f 6c6f 7273  lor=stock_colors
+00006940: 5b33 5d29 0a20 2020 2020 2020 2072 6573  [3]).        res
+00006950: 756c 7473 5b27 6369 6e33 5f70 7265 7661  ults['cin3_preva
+00006960: 6c65 6e63 655f 6279 5f67 656e 6f74 7970  lence_by_genotyp
+00006970: 6527 5d20 3d20 696e 6974 5f72 6573 2827  e'] = init_res('
+00006980: 4349 4e33 2070 7265 7661 6c65 6e63 6527  CIN3 prevalence'
+00006990: 2c20 6e5f 726f 7773 3d6e 672c 2063 6f6c  , n_rows=ng, col
+000069a0: 6f72 3d73 746f 636b 5f63 6f6c 6f72 735b  or=stock_colors[
+000069b0: 335d 290a 2020 2020 2020 2020 7265 7375  3]).        resu
+000069c0: 6c74 735b 2763 696e 335f 7072 6576 616c  lts['cin3_preval
+000069d0: 656e 6365 5f62 795f 6167 6527 5d20 3d20  ence_by_age'] = 
+000069e0: 696e 6974 5f72 6573 2827 4349 4e33 2070  init_res('CIN3 p
+000069f0: 7265 7661 6c65 6e63 6520 6279 2061 6765  revalence by age
+00006a00: 272c 206e 5f72 6f77 733d 6e61 2c20 636f  ', n_rows=na, co
+00006a10: 6c6f 723d 7374 6f63 6b5f 636f 6c6f 7273  lor=stock_colors
+00006a20: 5b33 5d29 0a20 2020 2020 2020 2072 6573  [3]).        res
+00006a30: 756c 7473 5b27 6665 6d61 6c65 5f68 7076  ults['female_hpv
+00006a40: 5f70 7265 7661 6c65 6e63 655f 6279 5f61  _prevalence_by_a
+00006a50: 6765 275d 203d 2069 6e69 745f 7265 7328  ge'] = init_res(
+00006a60: 2746 656d 616c 6520 4850 5620 7072 6576  'Female HPV prev
+00006a70: 616c 656e 6365 2062 7920 6167 6527 2c20  alence by age', 
+00006a80: 6e5f 726f 7773 3d6e 612c 2063 6f6c 6f72  n_rows=na, color
+00006a90: 3d73 746f 636b 5f63 6f6c 6f72 735b 335d  =stock_colors[3]
+00006aa0: 290a 0a20 2020 2020 2020 2023 2054 696d  )..        # Tim
+00006ab0: 6520 7665 6374 6f72 0a20 2020 2020 2020  e vector.       
+00006ac0: 2072 6573 756c 7473 5b27 7965 6172 275d   results['year']
+00006ad0: 203d 2073 656c 662e 7265 735f 7965 6172   = self.res_year
+00006ae0: 7665 630a 2020 2020 2020 2020 7265 7375  vec.        resu
+00006af0: 6c74 735b 2774 275d 203d 2073 656c 662e  lts['t'] = self.
+00006b00: 7265 735f 7476 6563 0a0a 2020 2020 2020  res_tvec..      
+00006b10: 2020 2320 4669 6e61 6c20 6974 656d 730a    # Final items.
+00006b20: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+00006b30: 756c 7473 203d 2072 6573 756c 7473 0a20  ults = results. 
+00006b40: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
+00006b50: 6c74 735f 7265 6164 7920 3d20 4661 6c73  lts_ready = Fals
+00006b60: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+00006b70: 6e0a 0a0a 2020 2020 6465 6620 696e 6974  n...    def init
+00006b80: 5f69 6e74 6572 7665 6e74 696f 6e73 2873  _interventions(s
+00006b90: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
+00006ba0: 2720 496e 6974 6961 6c69 7a65 2061 6e64  ' Initialize and
+00006bb0: 2076 616c 6964 6174 6520 7468 6520 696e   validate the in
+00006bc0: 7465 7276 656e 7469 6f6e 7320 2727 270a  terventions '''.
+00006bd0: 0a20 2020 2020 2020 2023 2049 6e69 7469  .        # Initi
+00006be0: 616c 697a 6174 696f 6e0a 2020 2020 2020  alization.      
+00006bf0: 2020 7365 6c66 2e69 6e74 6572 7665 6e74    self.intervent
+00006c00: 696f 6e73 203d 2073 632e 6175 746f 6c69  ions = sc.autoli
+00006c10: 7374 2829 0a0a 2020 2020 2020 2020 2320  st()..        # 
+00006c20: 5472 616e 736c 6174 6520 7468 6520 696e  Translate the in
+00006c30: 7465 7276 656e 7469 6f6e 2073 7065 6373  tervention specs
+00006c40: 2069 6e74 6f20 6163 7475 616c 2069 6e74   into actual int
+00006c50: 6572 7665 6e74 696f 6e73 0a20 2020 2020  erventions.     
+00006c60: 2020 2066 6f72 2069 2c69 6e74 6572 7665     for i,interve
+00006c70: 6e74 696f 6e20 696e 2065 6e75 6d65 7261  ntion in enumera
+00006c80: 7465 2873 656c 665b 2769 6e74 6572 7665  te(self['interve
+00006c90: 6e74 696f 6e73 275d 293a 0a20 2020 2020  ntions']):.     
+00006ca0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00006cb0: 616e 6365 2869 6e74 6572 7665 6e74 696f  ance(interventio
+00006cc0: 6e2c 2074 7970 6529 2061 6e64 2069 7373  n, type) and iss
+00006cd0: 7562 636c 6173 7328 696e 7465 7276 656e  ubclass(interven
+00006ce0: 7469 6f6e 2c20 6870 692e 496e 7465 7276  tion, hpi.Interv
+00006cf0: 656e 7469 6f6e 293a 0a20 2020 2020 2020  ention):.       
+00006d00: 2020 2020 2020 2020 2069 6e74 6572 7665           interve
+00006d10: 6e74 696f 6e20 3d20 696e 7465 7276 656e  ntion = interven
+00006d20: 7469 6f6e 2829 2023 2043 6f6e 7665 7274  tion() # Convert
+00006d30: 2066 726f 6d20 6120 636c 6173 7320 746f   from a class to
+00006d40: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
+00006d50: 6120 636c 6173 730a 2020 2020 2020 2020  a class.        
+00006d60: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00006d70: 6528 696e 7465 7276 656e 7469 6f6e 2c20  e(intervention, 
+00006d80: 6870 692e 496e 7465 7276 656e 7469 6f6e  hpi.Intervention
+00006d90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00006da0: 2020 2069 6e74 6572 7665 6e74 696f 6e2e     intervention.
+00006db0: 696e 6974 6961 6c69 7a65 2873 656c 6629  initialize(self)
+00006dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006dd0: 2073 656c 662e 696e 7465 7276 656e 7469   self.interventi
+00006de0: 6f6e 7320 2b3d 2069 6e74 6572 7665 6e74  ons += intervent
+00006df0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00006e00: 656c 6966 2063 616c 6c61 626c 6528 696e  elif callable(in
+00006e10: 7465 7276 656e 7469 6f6e 293a 0a20 2020  tervention):.   
+00006e20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006e30: 662e 696e 7465 7276 656e 7469 6f6e 7320  f.interventions 
+00006e40: 2b3d 2069 6e74 6572 7665 6e74 696f 6e0a  += intervention.
+00006e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00006e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006e70: 2020 6572 726f 726d 7367 203d 2066 2749    errormsg = f'I
+00006e80: 6e74 6572 7665 6e74 696f 6e20 7b69 6e74  ntervention {int
+00006e90: 6572 7665 6e74 696f 6e7d 2064 6f65 7320  ervention} does 
+00006ea0: 6e6f 7420 7365 656d 2074 6f20 6265 2061  not seem to be a
+00006eb0: 2076 616c 6964 2069 6e74 6572 7665 6e74   valid intervent
+00006ec0: 696f 6e3a 206d 7573 7420 6265 2061 2066  ion: must be a f
+00006ed0: 756e 6374 696f 6e20 6f72 2068 7076 2e49  unction or hpv.I
+00006ee0: 6e74 6572 7665 6e74 696f 6e20 7375 6263  ntervention subc
+00006ef0: 6c61 7373 270a 2020 2020 2020 2020 2020  lass'.          
+00006f00: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+00006f10: 4572 726f 7228 6572 726f 726d 7367 290a  Error(errormsg).
+00006f20: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
+00006f30: 0a0a 2020 2020 6465 6620 696e 6974 5f70  ..    def init_p
+00006f40: 656f 706c 6528 7365 6c66 2c20 706f 7064  eople(self, popd
+00006f50: 6963 743d 4e6f 6e65 2c20 696e 6974 5f73  ict=None, init_s
+00006f60: 7461 7465 733d 4661 6c73 652c 2072 6573  tates=False, res
+00006f70: 6574 3d46 616c 7365 2c20 7665 7262 6f73  et=False, verbos
+00006f80: 653d 4e6f 6e65 2c20 2a2a 6b77 6172 6773  e=None, **kwargs
+00006f90: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
+00006fa0: 2020 2020 2020 2043 7265 6174 6520 7468         Create th
+00006fb0: 6520 7065 6f70 6c65 2061 6e64 2074 6865  e people and the
+00006fc0: 206e 6574 776f 726b 2e0a 0a20 2020 2020   network...     
+00006fd0: 2020 2055 7365 2060 6069 6e69 745f 7374     Use ``init_st
+00006fe0: 6174 6573 3d46 616c 7365 6060 2066 6f72  ates=False`` for
+00006ff0: 2063 7265 6174 696e 6720 6120 6672 6573   creating a fres
+00007000: 6820 5065 6f70 6c65 206f 626a 6563 7420  h People object 
+00007010: 666f 7220 7573 650a 2020 2020 2020 2020  for use.        
+00007020: 696e 2066 7574 7572 6520 7369 6d75 6c61  in future simula
+00007030: 7469 6f6e 730a 0a20 2020 2020 2020 2041  tions..        A
+00007040: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00007050: 2070 6f70 6469 6374 2020 2020 2020 2020   popdict        
+00007060: 2028 616e 7929 3a20 2070 7265 2d67 656e   (any):  pre-gen
+00007070: 6572 6174 6564 2070 656f 706c 6520 6f66  erated people of
+00007080: 2076 6172 696f 7573 2066 6f72 6d61 7473   various formats
+00007090: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+000070a0: 6974 5f73 7461 7465 7320 2020 2020 2862  it_states     (b
+000070b0: 6f6f 6c29 3a20 7768 6574 6865 7220 746f  ool): whether to
+000070c0: 2069 6e69 7469 616c 697a 6520 7374 6174   initialize stat
+000070d0: 6573 2028 6465 6661 756c 7420 6661 6c73  es (default fals
+000070e0: 6520 7768 656e 2063 616c 6c65 6420 6469  e when called di
+000070f0: 7265 6374 6c79 290a 2020 2020 2020 2020  rectly).        
+00007100: 2020 2020 7265 7365 7420 2020 2020 2020      reset       
+00007110: 2020 2020 2862 6f6f 6c29 3a20 7768 6574      (bool): whet
+00007120: 6865 7220 746f 2072 6567 656e 6572 6174  her to regenerat
+00007130: 6520 7468 6520 7065 6f70 6c65 2065 7665  e the people eve
+00007140: 6e20 6966 2074 6865 7920 616c 7265 6164  n if they alread
+00007150: 7920 6578 6973 740a 2020 2020 2020 2020  y exist.        
+00007160: 2020 2020 7665 7262 6f73 6520 2020 2020      verbose     
+00007170: 2020 2020 2869 6e74 293a 2020 6465 7461      (int):  deta
+00007180: 696c 2074 6f20 7072 696e 740a 2020 2020  il to print.    
+00007190: 2020 2020 2020 2020 6b77 6172 6773 2020          kwargs  
+000071a0: 2020 2020 2020 2020 2864 6963 7429 3a20          (dict): 
+000071b0: 7061 7373 6564 2074 6f20 6870 762e 6d61  passed to hpv.ma
+000071c0: 6b65 5f70 656f 706c 6528 290a 2020 2020  ke_people().    
+000071d0: 2020 2020 2727 270a 0a20 2020 2020 2020      '''..       
+000071e0: 2023 2048 616e 646c 6520 696e 7075 7473   # Handle inputs
+000071f0: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+00007200: 6f73 6520 6973 204e 6f6e 653a 0a20 2020  ose is None:.   
+00007210: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
+00007220: 203d 2073 656c 665b 2776 6572 626f 7365   = self['verbose
+00007230: 275d 0a20 2020 2020 2020 2069 6620 706f  '].        if po
+00007240: 7064 6963 7420 6973 206e 6f74 204e 6f6e  pdict is not Non
+00007250: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00007260: 656c 662e 706f 7064 6963 7420 3d20 706f  elf.popdict = po
+00007270: 7064 6963 740a 2020 2020 2020 2020 6966  pdict.        if
+00007280: 2076 6572 626f 7365 203e 2030 3a0a 2020   verbose > 0:.  
+00007290: 2020 2020 2020 2020 2020 7265 7365 7473            resets
+000072a0: 7472 3d20 2727 0a20 2020 2020 2020 2020  tr= ''.         
+000072b0: 2020 2069 6620 7365 6c66 2e70 656f 706c     if self.peopl
+000072c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000072d0: 2020 2072 6573 6574 7374 7220 3d20 2720     resetstr = ' 
+000072e0: 2872 6573 6574 7469 6e67 2070 656f 706c  (resetting peopl
+000072f0: 6529 2720 6966 2072 6573 6574 2065 6c73  e)' if reset els
+00007300: 6520 2720 2877 6172 6e69 6e67 3a20 6e6f  e ' (warning: no
+00007310: 7420 7265 7365 7474 696e 6720 7369 6d2e  t resetting sim.
+00007320: 7065 6f70 6c65 2927 0a20 2020 2020 2020  people)'.       
+00007330: 2020 2020 2070 7269 6e74 2866 2749 6e69       print(f'Ini
+00007340: 7469 616c 697a 696e 6720 7369 6d7b 7265  tializing sim{re
+00007350: 7365 7473 7472 7d20 7769 7468 207b 7365  setstr} with {se
+00007360: 6c66 5b22 6e5f 6167 656e 7473 225d 3a30  lf["n_agents"]:0
+00007370: 6e7d 2061 6765 6e74 7327 290a 2020 2020  n} agents').    
+00007380: 2020 2020 6966 2073 656c 662e 706f 7066      if self.popf
+00007390: 696c 6520 616e 6420 7365 6c66 2e70 6f70  ile and self.pop
+000073a0: 6469 6374 2069 7320 4e6f 6e65 3a20 2320  dict is None: # 
+000073b0: 4966 2074 6865 7265 2773 2061 2070 6f70  If there's a pop
+000073c0: 6469 6374 2c20 7765 2069 6e69 7469 616c  dict, we initial
+000073d0: 697a 6520 6974 0a20 2020 2020 2020 2020  ize it.         
+000073e0: 2020 2073 656c 662e 6c6f 6164 5f70 6f70     self.load_pop
+000073f0: 756c 6174 696f 6e28 696e 6974 5f70 656f  ulation(init_peo
+00007400: 706c 653d 4661 6c73 6529 0a0a 2020 2020  ple=False)..    
+00007410: 2020 2020 2320 4d61 6b65 2074 6865 2070      # Make the p
+00007420: 656f 706c 650a 2020 2020 2020 2020 7365  eople.        se
+00007430: 6c66 2e70 656f 706c 652c 2074 6f74 616c  lf.people, total
+00007440: 5f70 6f70 203d 2068 7070 6f70 2e6d 616b  _pop = hppop.mak
+00007450: 655f 7065 6f70 6c65 2873 656c 662c 2072  e_people(self, r
+00007460: 6573 6574 3d72 6573 6574 2c20 7665 7262  eset=reset, verb
+00007470: 6f73 653d 7665 7262 6f73 652c 206d 6963  ose=verbose, mic
+00007480: 726f 7374 7275 6374 7572 653d 7365 6c66  rostructure=self
+00007490: 5b27 6e65 7477 6f72 6b27 5d2c 202a 2a6b  ['network'], **k
+000074a0: 7761 7267 7329 0a0a 2020 2020 2020 2020  wargs)..        
+000074b0: 2320 4669 6775 7265 206f 7574 2074 6865  # Figure out the
+000074c0: 2073 6361 6c65 2066 6163 746f 7273 0a20   scale factors. 
+000074d0: 2020 2020 2020 2069 6620 7365 6c66 5b27         if self['
+000074e0: 746f 7461 6c5f 706f 7027 5d20 6973 206e  total_pop'] is n
+000074f0: 6f74 204e 6f6e 6520 616e 6420 746f 7461  ot None and tota
+00007500: 6c5f 706f 7020 6973 206e 6f74 204e 6f6e  l_pop is not Non
+00007510: 653a 2023 2049 6620 6e6f 2070 6f70 5f73  e: # If no pop_s
+00007520: 6361 6c65 2068 6173 2062 6565 6e20 7072  cale has been pr
+00007530: 6f76 6964 6564 2c20 7472 7920 746f 2067  ovided, try to g
+00007540: 6574 2069 7420 6672 6f6d 2074 6865 206c  et it from the l
+00007550: 6f63 6174 696f 6e0a 2020 2020 2020 2020  ocation.        
+00007560: 2020 2020 6572 726f 726d 7367 203d 2027      errormsg = '
+00007570: 596f 7520 6361 6e20 6569 7468 6572 2064  You can either d
+00007580: 6566 696e 6520 746f 7461 6c5f 706f 7020  efine total_pop 
+00007590: 6578 706c 6963 6974 6c79 206f 7220 7669  explicitly or vi
+000075a0: 6120 7468 6520 6c6f 6361 7469 6f6e 2c20  a the location, 
+000075b0: 6275 7420 6e6f 7420 626f 7468 270a 2020  but not both'.  
+000075c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000075d0: 5661 6c75 6545 7272 6f72 2865 7272 6f72  ValueError(error
+000075e0: 6d73 6729 0a20 2020 2020 2020 2065 6c69  msg).        eli
+000075f0: 6620 746f 7461 6c5f 706f 7020 6973 204e  f total_pop is N
+00007600: 6f6e 6520 616e 6420 7365 6c66 5b27 746f  one and self['to
+00007610: 7461 6c5f 706f 7027 5d20 6973 206e 6f74  tal_pop'] is not
+00007620: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00007630: 2020 2074 6f74 616c 5f70 6f70 203d 2073     total_pop = s
+00007640: 656c 665b 2774 6f74 616c 5f70 6f70 275d  elf['total_pop']
+00007650: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00007660: 2020 2020 2020 6966 2073 656c 665b 2770        if self['p
+00007670: 6f70 5f73 6361 6c65 275d 2069 7320 4e6f  op_scale'] is No
+00007680: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007690: 6966 2074 6f74 616c 5f70 6f70 2069 7320  if total_pop is 
+000076a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000076b0: 2020 2020 2020 7365 6c66 5b27 706f 705f        self['pop_
+000076c0: 7363 616c 6527 5d20 3d20 312e 300a 2020  scale'] = 1.0.  
+000076d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 7365 6c66 5b27 706f 705f 7363 616c 6527  self['pop_scale'
+00007700: 5d20 3d20 746f 7461 6c5f 706f 702f 7365  ] = total_pop/se
+00007710: 6c66 5b27 6e5f 6167 656e 7473 275d 0a20  lf['n_agents']. 
+00007720: 2020 2020 2020 2073 656c 665b 276d 735f         self['ms_
+00007730: 6167 656e 745f 7261 7469 6f27 5d20 3d20  agent_ratio'] = 
+00007740: 696e 7428 7365 6c66 5b27 6d73 5f61 6765  int(self['ms_age
+00007750: 6e74 5f72 6174 696f 275d 290a 0a20 2020  nt_ratio'])..   
+00007760: 2020 2020 2023 2044 6561 6c20 7769 7468       # Deal with
+00007770: 2048 4956 0a20 2020 2020 2020 2073 656c   HIV.        sel
+00007780: 662e 696e 6974 5f68 6976 2829 2023 2043  f.init_hiv() # C
+00007790: 7265 6174 6573 2074 6865 2068 6976 7369  reates the hivsi
+000077a0: 6d20 6f62 6a65 6374 2c20 7768 6963 6820  m object, which 
+000077b0: 6973 2073 746f 7265 6420 696e 2074 6865  is stored in the
+000077c0: 2073 696d 0a20 2020 2020 2020 2073 656c   sim.        sel
+000077d0: 662e 6869 7673 696d 2e69 6e69 745f 7374  f.hivsim.init_st
+000077e0: 6174 6573 2873 656c 662e 7065 6f70 6c65  ates(self.people
+000077f0: 2920 2320 4164 6473 2073 6f6d 6520 7374  ) # Adds some st
+00007800: 6174 6573 2074 6f20 7468 6520 7065 6f70  ates to the peop
+00007810: 6c65 0a0a 2020 2020 2020 2020 2320 4669  le..        # Fi
+00007820: 6e69 7368 2069 6e69 7469 616c 697a 6174  nish initializat
+00007830: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
+00007840: 2e70 656f 706c 652e 696e 6974 6961 6c69  .people.initiali
+00007850: 7a65 2873 696d 5f70 6172 733d 7365 6c66  ze(sim_pars=self
+00007860: 2e70 6172 7329 2023 2046 756c 6c79 2069  .pars) # Fully i
+00007870: 6e69 7469 616c 697a 6520 7468 6520 7065  nitialize the pe
+00007880: 6f70 6c65 0a20 2020 2020 2020 2073 656c  ople.        sel
+00007890: 662e 7265 7365 745f 6c61 7965 725f 7061  f.reset_layer_pa
+000078a0: 7273 2866 6f72 6365 3d46 616c 7365 2920  rs(force=False) 
+000078b0: 2320 456e 7375 7265 2074 6861 7420 6c61  # Ensure that la
+000078c0: 7965 7220 6b65 7973 206d 6174 6368 2074  yer keys match t
+000078d0: 6865 206c 6f61 6465 6420 706f 7075 6c61  he loaded popula
+000078e0: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
+000078f0: 696e 6974 5f73 7461 7465 733a 0a20 2020  init_states:.   
+00007900: 2020 2020 2020 2020 2069 6e69 745f 6870           init_hp
+00007910: 765f 7072 6576 203d 2073 632e 6463 7028  v_prev = sc.dcp(
+00007920: 7365 6c66 5b27 696e 6974 5f68 7076 5f70  self['init_hpv_p
+00007930: 7265 7627 5d29 0a20 2020 2020 2020 2020  rev']).         
+00007940: 2020 2069 6e69 745f 6870 765f 7072 6576     init_hpv_prev
+00007950: 2c20 6167 655f 6272 6163 6b65 7473 203d  , age_brackets =
+00007960: 2073 656c 662e 7661 6c69 6461 7465 5f69   self.validate_i
+00007970: 6e69 745f 636f 6e64 6974 696f 6e73 2869  nit_conditions(i
+00007980: 6e69 745f 6870 765f 7072 6576 290a 2020  nit_hpv_prev).  
+00007990: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+000079a0: 6e69 745f 7374 6174 6573 2861 6765 5f62  nit_states(age_b
+000079b0: 7261 636b 6574 733d 6167 655f 6272 6163  rackets=age_brac
+000079c0: 6b65 7473 2c20 696e 6974 5f68 7076 5f70  kets, init_hpv_p
+000079d0: 7265 763d 696e 6974 5f68 7076 5f70 7265  rev=init_hpv_pre
+000079e0: 7629 0a0a 2020 2020 2020 2020 7265 7475  v)..        retu
+000079f0: 726e 2073 656c 660a 0a20 2020 2064 6566  rn self..    def
+00007a00: 2069 6e69 745f 616e 616c 797a 6572 7328   init_analyzers(
+00007a10: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
+00007a20: 2727 2049 6e69 7469 616c 697a 6520 7468  '' Initialize th
+00007a30: 6520 616e 616c 797a 6572 7320 2727 270a  e analyzers '''.
+00007a40: 0a20 2020 2020 2020 2073 656c 662e 616e  .        self.an
+00007a50: 616c 797a 6572 7320 3d20 7363 2e61 7574  alyzers = sc.aut
+00007a60: 6f6c 6973 7428 290a 0a20 2020 2020 2020  olist()..       
+00007a70: 2064 6566 2063 6f6e 7665 7274 5f61 6e61   def convert_ana
+00007a80: 6c79 7a65 7228 616e 616c 797a 6572 293a  lyzer(analyzer):
+00007a90: 0a20 2020 2020 2020 2020 2020 2027 2727  .            '''
+00007aa0: 2048 656c 7065 7220 6675 6e63 7469 6f6e   Helper function
+00007ab0: 2074 6f20 7475 726e 2073 7472 696e 6773   to turn strings
+00007ac0: 2069 6e74 6f20 616e 616c 797a 6572 7320   into analyzers 
+00007ad0: 2727 270a 2020 2020 2020 2020 2020 2020  '''.            
+00007ae0: 6368 6f69 6365 7320 3d20 6870 612e 616e  choices = hpa.an
+00007af0: 616c 797a 6572 5f6d 6170 2e6b 6579 7328  alyzer_map.keys(
+00007b00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00007b10: 206e 6f74 2061 6e61 6c79 7a65 7220 696e   not analyzer in
+00007b20: 2063 686f 6963 6573 3a0a 2020 2020 2020   choices:.      
+00007b30: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
+00007b40: 7367 203d 2066 2741 6e61 6c79 7a65 7220  sg = f'Analyzer 
+00007b50: 7b61 6e61 6c79 7a65 727d 206e 6f74 2075  {analyzer} not u
+00007b60: 6e64 6572 7374 6f6f 643a 2063 686f 6963  nderstood: choic
+00007b70: 6573 2061 7265 207b 6368 6f69 6365 737d  es are {choices}
+00007b80: 2e27 0a20 2020 2020 2020 2020 2020 2020  .'.             
+00007b90: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00007ba0: 726f 7228 6572 726f 726d 7367 290a 2020  ror(errormsg).  
+00007bb0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 616e 616c 797a 6572 203d 2068 7061 2e61  analyzer = hpa.a
+00007be0: 6e61 6c79 7a65 725f 6d61 705b 616e 616c  nalyzer_map[anal
+00007bf0: 797a 6572 5d0a 2020 2020 2020 2020 2020  yzer].          
+00007c00: 2020 7265 7475 726e 2061 6e61 6c79 7a65    return analyze
+00007c10: 720a 0a20 2020 2020 2020 2023 2049 6e74  r..        # Int
+00007c20: 6572 7072 6574 2061 6e61 6c79 7a65 7273  erpret analyzers
+00007c30: 0a20 2020 2020 2020 2066 6f72 2061 692c  .        for ai,
+00007c40: 2061 6e61 6c79 7a65 7220 696e 2065 6e75   analyzer in enu
+00007c50: 6d65 7261 7465 2873 656c 665b 2761 6e61  merate(self['ana
+00007c60: 6c79 7a65 7273 275d 293a 0a20 2020 2020  lyzers']):.     
+00007c70: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00007c80: 616e 6365 2861 6e61 6c79 7a65 722c 2073  ance(analyzer, s
+00007c90: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00007ca0: 2020 2020 2061 6e61 6c79 7a65 725f 6c69       analyzer_li
+00007cb0: 7374 203d 2073 632e 746f 6c69 7374 280a  st = sc.tolist(.
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cd0: 2020 2020 636f 6e76 6572 745f 616e 616c      convert_anal
+00007ce0: 797a 6572 2861 6e61 6c79 7a65 7229 2920  yzer(analyzer)) 
+00007cf0: 2023 2049 6620 6e6f 7420 6120 6c69 7374   # If not a list
+00007d00: 2c20 7475 726e 2069 7420 696e 746f 206f  , turn it into o
+00007d10: 6e65 202d 2066 6f72 2063 6f6e 7369 7374  ne - for consist
+00007d20: 656e 6379 206f 6620 7072 6f63 6573 7369  ency of processi
+00007d30: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00007d40: 2020 2066 6f72 2061 7a20 696e 2061 6e61     for az in ana
+00007d50: 6c79 7a65 725f 6c69 7374 3a0a 2020 2020  lyzer_list:.    
+00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d70: 6966 2069 7369 6e73 7461 6e63 6528 617a  if isinstance(az
+00007d80: 2c20 7374 7229 3a20 617a 203d 2063 6f6e  , str): az = con
+00007d90: 7665 7274 5f61 6e61 6c79 7a65 7228 617a  vert_analyzer(az
+00007da0: 2920 2023 2049 7420 6d69 6768 7420 7374  )  # It might st
+00007db0: 696c 6c20 6265 2061 2073 7472 696e 670a  ill be a string.
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dd0: 2020 2020 7365 6c66 2e61 6e61 6c79 7a65      self.analyze
+00007de0: 7273 202b 3d20 617a 2829 2020 2320 556e  rs += az()  # Un
+00007df0: 7061 636b 206c 6973 740a 2020 2020 2020  pack list.      
+00007e00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00007e10: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00007e20: 7369 6e73 7461 6e63 6528 616e 616c 797a  sinstance(analyz
+00007e30: 6572 2c20 7479 7065 2920 616e 6420 6973  er, type) and is
+00007e40: 7375 6263 6c61 7373 2861 6e61 6c79 7a65  subclass(analyze
+00007e50: 722c 2068 7061 2e41 6e61 6c79 7a65 7229  r, hpa.Analyzer)
+00007e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007e70: 2020 2020 2020 616e 616c 797a 6572 203d        analyzer =
+00007e80: 2061 6e61 6c79 7a65 7228 2920 2023 2043   analyzer()  # C
+00007e90: 6f6e 7665 7274 2066 726f 6d20 6120 636c  onvert from a cl
+00007ea0: 6173 7320 746f 2061 6e20 696e 7374 616e  ass to an instan
+00007eb0: 6365 206f 6620 6120 636c 6173 730a 2020  ce of a class.  
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007ed0: 206e 6f74 2028 6973 696e 7374 616e 6365   not (isinstance
+00007ee0: 2861 6e61 6c79 7a65 722c 2068 7061 2e41  (analyzer, hpa.A
+00007ef0: 6e61 6c79 7a65 7229 206f 7220 6361 6c6c  nalyzer) or call
+00007f00: 6162 6c65 2861 6e61 6c79 7a65 7229 293a  able(analyzer)):
+00007f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007f20: 2020 2020 2065 7272 6f72 6d73 6720 3d20       errormsg = 
+00007f30: 6627 416e 616c 797a 6572 207b 616e 616c  f'Analyzer {anal
+00007f40: 797a 6572 7d20 646f 6573 206e 6f74 2073  yzer} does not s
+00007f50: 6565 6d20 746f 2062 6520 6120 7661 6c69  eem to be a vali
+00007f60: 6420 616e 616c 797a 6572 3a20 6d75 7374  d analyzer: must
+00007f70: 2062 6520 6120 6675 6e63 7469 6f6e 206f   be a function o
+00007f80: 7220 6870 762e 416e 616c 797a 6572 2073  r hpv.Analyzer s
+00007f90: 7562 636c 6173 7327 0a20 2020 2020 2020  ubclass'.       
+00007fa0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00007fb0: 7365 2054 7970 6545 7272 6f72 2865 7272  se TypeError(err
+00007fc0: 6f72 6d73 6729 0a20 2020 2020 2020 2020  ormsg).         
+00007fd0: 2020 2020 2020 2073 656c 662e 616e 616c         self.anal
+00007fe0: 797a 6572 7320 2b3d 2061 6e61 6c79 7a65  yzers += analyze
+00007ff0: 7220 2023 2041 6464 2069 7420 696e 0a0a  r  # Add it in..
+00008000: 2020 2020 2020 2020 666f 7220 616e 616c          for anal
+00008010: 797a 6572 2069 6e20 7365 6c66 2e61 6e61  yzer in self.ana
+00008020: 6c79 7a65 7273 3a0a 2020 2020 2020 2020  lyzers:.        
+00008030: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00008040: 6528 616e 616c 797a 6572 2c20 6870 612e  e(analyzer, hpa.
+00008050: 416e 616c 797a 6572 293a 0a20 2020 2020  Analyzer):.     
+00008060: 2020 2020 2020 2020 2020 2061 6e61 6c79             analy
+00008070: 7a65 722e 696e 6974 6961 6c69 7a65 2873  zer.initialize(s
+00008080: 656c 6629 0a0a 2020 2020 2020 2020 7265  elf)..        re
+00008090: 7475 726e 0a0a 0a20 2020 2064 6566 2069  turn...    def i
+000080a0: 6e69 745f 696d 6d75 6e69 7479 2873 656c  nit_immunity(sel
+000080b0: 662c 2063 7265 6174 653d 5472 7565 293a  f, create=True):
+000080c0: 0a20 2020 2020 2020 2027 2727 2049 6e69  .        ''' Ini
+000080d0: 7469 616c 697a 6520 696d 6d75 6e69 7479  tialize immunity
+000080e0: 206d 6174 7269 6365 7320 616e 6420 6375   matrices and cu
+000080f0: 6d75 6c61 7469 7665 2064 7973 706c 6173  mulative dysplas
+00008100: 6961 2027 2727 0a0a 2020 2020 2020 2020  ia '''..        
+00008110: 2320 496e 6974 6961 6c69 7a65 2069 6d6d  # Initialize imm
+00008120: 756e 6974 7920 6172 7261 7973 0a20 2020  unity arrays.   
+00008130: 2020 2020 2068 7069 6d6d 2e69 6e69 745f       hpimm.init_
+00008140: 696d 6d75 6e69 7479 2873 656c 662c 2063  immunity(self, c
+00008150: 7265 6174 653d 6372 6561 7465 290a 2020  reate=create).  
+00008160: 2020 2020 2020 7265 7475 726e 0a0a 0a20        return... 
+00008170: 2020 2064 6566 2069 6e69 745f 6869 7628     def init_hiv(
+00008180: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
+00008190: 2727 2049 6e69 7469 616c 697a 6520 7374  '' Initialize st
+000081a0: 6174 6573 2c20 6174 7472 6962 7574 6573  ates, attributes
+000081b0: 2c20 616e 6420 7061 7261 6d65 7465 7273  , and parameters
+000081c0: 2072 656c 6174 696e 6720 746f 2048 4956   relating to HIV
+000081d0: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
+000081e0: 7365 6c66 2e70 6172 735b 276d 6f64 656c  self.pars['model
+000081f0: 5f68 6976 275d 3a0a 2020 2020 2020 2020  _hiv']:.        
+00008200: 2020 2020 6966 2073 656c 662e 6869 765f      if self.hiv_
+00008210: 6461 7461 6669 6c65 2069 7320 4e6f 6e65  datafile is None
+00008220: 206f 7220 7365 6c66 2e61 7274 5f64 6174   or self.art_dat
+00008230: 6166 696c 6520 6973 204e 6f6e 653a 0a20  afile is None:. 
+00008240: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008250: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00008260: 274d 7573 7420 7375 7070 6c79 2048 4956  'Must supply HIV
+00008270: 2061 6e64 2041 5254 2064 6174 6166 696c   and ART datafil
+00008280: 6573 2074 6f20 6d6f 6465 6c20 4849 562e  es to model HIV.
+00008290: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+000082a0: 6869 7673 696d 203d 2068 7068 6976 2e48  hivsim = hphiv.H
+000082b0: 4956 7369 6d28 7365 6c66 2c20 6869 765f  IVsim(self, hiv_
+000082c0: 6461 7461 6669 6c65 3d73 656c 662e 6869  datafile=self.hi
+000082d0: 765f 6461 7461 6669 6c65 2c20 6172 745f  v_datafile, art_
+000082e0: 6461 7461 6669 6c65 3d73 656c 662e 6172  datafile=self.ar
+000082f0: 745f 6461 7461 6669 6c65 2c0a 2020 2020  t_datafile,.    
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00008320: 6976 5f70 6172 733d 7365 6c66 5b27 6869  iv_pars=self['hi
+00008330: 765f 7061 7273 275d 290a 2020 2020 2020  v_pars']).      
+00008340: 2020 7265 7475 726e 0a0a 0a20 2020 2064    return...    d
+00008350: 6566 2066 696e 616c 697a 655f 616e 616c  ef finalize_anal
+00008360: 797a 6572 7328 7365 6c66 293a 0a20 2020  yzers(self):.   
+00008370: 2020 2020 2066 6f72 2061 6e61 6c79 7a65       for analyze
+00008380: 7220 696e 2073 656c 662e 616e 616c 797a  r in self.analyz
+00008390: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+000083a0: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+000083b0: 6e61 6c79 7a65 722c 2068 7061 2e41 6e61  nalyzer, hpa.Ana
+000083c0: 6c79 7a65 7229 3a0a 2020 2020 2020 2020  lyzer):.        
+000083d0: 2020 2020 2020 2020 616e 616c 797a 6572          analyzer
+000083e0: 2e66 696e 616c 697a 6528 7365 6c66 290a  .finalize(self).
+000083f0: 0a0a 2020 2020 6465 6620 696e 6974 5f73  ..    def init_s
+00008400: 7461 7465 7328 7365 6c66 2c20 6167 655f  tates(self, age_
+00008410: 6272 6163 6b65 7473 3d4e 6f6e 652c 2069  brackets=None, i
+00008420: 6e69 745f 6870 765f 7072 6576 3d4e 6f6e  nit_hpv_prev=Non
+00008430: 652c 2069 6e69 745f 6369 6e5f 7072 6576  e, init_cin_prev
+00008440: 3d4e 6f6e 652c 2069 6e69 745f 6361 6e63  =None, init_canc
+00008450: 6572 5f70 7265 763d 4e6f 6e65 293a 0a20  er_prev=None):. 
+00008460: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00008470: 2020 2049 6e69 7469 616c 697a 6520 7072     Initialize pr
+00008480: 696f 7220 696d 6d75 6e69 7479 2061 6e64  ior immunity and
+00008490: 2073 6565 6420 696e 6665 6374 696f 6e73   seed infections
+000084a0: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
+000084b0: 2020 2020 2020 2320 5368 6f72 7465 6e20        # Shorten 
+000084c0: 6b65 7920 7661 7269 6162 6c65 730a 2020  key variables.  
+000084d0: 2020 2020 2020 6e67 203d 2073 656c 665b        ng = self[
+000084e0: 276e 5f67 656e 6f74 7970 6573 275d 0a0a  'n_genotypes']..
+000084f0: 2020 2020 2020 2020 2320 4173 7369 676e          # Assign
+00008500: 2070 656f 706c 6520 746f 2061 6765 2062   people to age b
+00008510: 7563 6b65 7473 0a20 2020 2020 2020 2061  uckets.        a
+00008520: 6765 5f69 6e64 7320 3d20 6e70 2e64 6967  ge_inds = np.dig
+00008530: 6974 697a 6528 7365 6c66 2e70 656f 706c  itize(self.peopl
+00008540: 652e 6167 652c 2061 6765 5f62 7261 636b  e.age, age_brack
+00008550: 6574 7329 0a0a 2020 2020 2020 2020 2320  ets)..        # 
+00008560: 4173 7369 676e 2070 726f 6261 6269 6c69  Assign probabili
+00008570: 7469 6573 206f 6620 6861 7669 6e67 2048  ties of having H
+00008580: 5056 2074 6f20 6561 6368 2061 6765 2f73  PV to each age/s
+00008590: 6578 2067 726f 7570 0a20 2020 2020 2020  ex group.       
+000085a0: 2068 7076 5f70 726f 6273 203d 206e 702e   hpv_probs = np.
+000085b0: 6675 6c6c 286c 656e 2873 656c 662e 7065  full(len(self.pe
+000085c0: 6f70 6c65 292c 206e 702e 6e61 6e2c 2064  ople), np.nan, d
+000085d0: 7479 7065 3d68 7064 2e64 6566 6175 6c74  type=hpd.default
+000085e0: 5f66 6c6f 6174 290a 2020 2020 2020 2020  _float).        
+000085f0: 6870 765f 7072 6f62 735b 7365 6c66 2e70  hpv_probs[self.p
+00008600: 656f 706c 652e 665f 696e 6473 5d20 3d20  eople.f_inds] = 
+00008610: 696e 6974 5f68 7076 5f70 7265 765b 2766  init_hpv_prev['f
+00008620: 275d 5b61 6765 5f69 6e64 735b 7365 6c66  '][age_inds[self
+00008630: 2e70 656f 706c 652e 665f 696e 6473 5d5d  .people.f_inds]]
+00008640: 2a73 656c 662e 7061 7273 5b27 7265 6c5f  *self.pars['rel_
+00008650: 696e 6974 5f70 7265 7627 5d0a 2020 2020  init_prev'].    
+00008660: 2020 2020 6870 765f 7072 6f62 735b 7365      hpv_probs[se
+00008670: 6c66 2e70 656f 706c 652e 6d5f 696e 6473  lf.people.m_inds
+00008680: 5d20 3d20 696e 6974 5f68 7076 5f70 7265  ] = init_hpv_pre
+00008690: 765b 276d 275d 5b61 6765 5f69 6e64 735b  v['m'][age_inds[
+000086a0: 7365 6c66 2e70 656f 706c 652e 6d5f 696e  self.people.m_in
+000086b0: 6473 5d5d 2a73 656c 662e 7061 7273 5b27  ds]]*self.pars['
+000086c0: 7265 6c5f 696e 6974 5f70 7265 7627 5d0a  rel_init_prev'].
+000086d0: 2020 2020 2020 2020 6870 765f 7072 6f62          hpv_prob
+000086e0: 735b 7e73 656c 662e 7065 6f70 6c65 2e69  s[~self.people.i
+000086f0: 735f 6163 7469 7665 5d20 3d20 3020 2320  s_active] = 0 # 
+00008700: 426c 616e 6b20 6f75 7420 7065 6f70 6c65  Blank out people
+00008710: 2077 686f 2061 7265 206e 6f74 2079 6574   who are not yet
+00008720: 2073 6578 7561 6c6c 7920 6163 7469 7665   sexually active
+00008730: 0a0a 2020 2020 2020 2020 2320 4765 7420  ..        # Get 
+00008740: 696e 6469 6365 7320 6f66 2070 656f 706c  indices of peopl
+00008750: 6520 7768 6f20 6861 7665 2048 5056 0a20  e who have HPV. 
+00008760: 2020 2020 2020 2068 7076 5f69 6e64 7320         hpv_inds 
+00008770: 3d20 6870 752e 7472 7565 2868 7075 2e62  = hpu.true(hpu.b
+00008780: 696e 6f6d 6961 6c5f 6172 7228 6870 765f  inomial_arr(hpv_
+00008790: 7072 6f62 7329 290a 0a20 2020 2020 2020  probs))..       
+000087a0: 2023 2044 6574 6572 6d69 6e65 2077 6869   # Determine whi
+000087b0: 6368 2067 656e 6f74 7970 6520 7065 6f70  ch genotype peop
+000087c0: 6c65 2061 7265 2069 6e66 6563 7465 6420  le are infected 
+000087d0: 7769 7468 0a20 2020 2020 2020 2069 6620  with.        if 
+000087e0: 7365 6c66 5b27 696e 6974 5f68 7076 5f64  self['init_hpv_d
+000087f0: 6973 7427 5d20 6973 204e 6f6e 653a 2023  ist'] is None: #
+00008800: 204e 6f20 7479 7065 2064 6973 7472 6962   No type distrib
+00008810: 7574 696f 6e20 7072 6f76 6964 6564 2c20  ution provided, 
+00008820: 6173 7375 6d65 2065 7665 6e20 7370 6c69  assume even spli
+00008830: 740a 2020 2020 2020 2020 2020 2020 6765  t.            ge
+00008840: 6e6f 7479 7065 7320 3d20 6e70 2e72 616e  notypes = np.ran
+00008850: 646f 6d2e 7261 6e64 696e 7428 302c 206e  dom.randint(0, n
+00008860: 672c 206c 656e 2868 7076 5f69 6e64 7329  g, len(hpv_inds)
+00008870: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00008880: 2020 2020 2020 2020 2020 2020 2320 4572              # Er
+00008890: 726f 7220 6368 6563 6b69 6e67 0a20 2020  ror checking.   
+000088a0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000088b0: 7363 2e63 6865 636b 7479 7065 2873 656c  sc.checktype(sel
+000088c0: 665b 2769 6e69 745f 6870 765f 6469 7374  f['init_hpv_dist
+000088d0: 275d 2c20 6469 6374 293a 0a20 2020 2020  '], dict):.     
+000088e0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+000088f0: 6d73 6720 3d20 6627 506c 6561 7365 2070  msg = f'Please p
+00008900: 726f 7669 6465 2069 6e69 7469 616c 2048  rovide initial H
+00008910: 5056 2074 7970 6520 6469 7374 7269 6275  PV type distribu
+00008920: 7469 6f6e 2061 7320 6120 6469 6374 696f  tion as a dictio
+00008930: 6e61 7279 206b 6579 6564 2062 7920 6765  nary keyed by ge
+00008940: 6e6f 7479 7065 2c20 6e6f 7420 7b73 656c  notype, not {sel
+00008950: 665b 2269 6e69 745f 6870 765f 6469 7374  f["init_hpv_dist
+00008960: 225d 7d27 0a20 2020 2020 2020 2020 2020  "]}'.           
+00008970: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00008980: 4572 726f 7228 6572 726f 726d 7367 290a  Error(errormsg).
+00008990: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000089a0: 6574 2873 656c 665b 2769 6e69 745f 6870  et(self['init_hp
+000089b0: 765f 6469 7374 275d 2e6b 6579 7328 2929  v_dist'].keys())
+000089c0: 213d 7365 7428 7365 6c66 5b27 6765 6e6f  !=set(self['geno
+000089d0: 7479 7065 5f6d 6170 275d 2e76 616c 7565  type_map'].value
+000089e0: 7328 2929 3a0a 2020 2020 2020 2020 2020  s()):.          
+000089f0: 2020 2020 2020 6572 726f 726d 7367 203d        errormsg =
+00008a00: 2066 2754 6865 2048 5056 2074 7970 6573   f'The HPV types
+00008a10: 2070 726f 7669 6465 6420 696e 2074 6865   provided in the
+00008a20: 2069 6e69 7469 616c 2048 5056 2074 7970   initial HPV typ
+00008a30: 6520 6469 7374 7269 6275 7469 6f6e 2061  e distribution a
+00008a40: 7265 206e 6f74 2074 6865 2073 616d 6520  re not the same 
+00008a50: 6173 2074 6865 2048 5056 2074 7970 6573  as the HPV types
+00008a60: 2062 6569 6e67 2073 696d 756c 6174 6564   being simulated
+00008a70: 3a20 7b73 656c 665b 2269 6e69 745f 6870  : {self["init_hp
+00008a80: 765f 6469 7374 225d 2e6b 6579 7328 297d  v_dist"].keys()}
+00008a90: 2076 7320 7b73 656c 665b 2267 656e 6f74   vs {self["genot
+00008aa0: 7970 655f 6d61 7022 5d2e 7661 6c75 6573  ype_map"].values
+00008ab0: 2829 7d2e 270a 2020 2020 2020 2020 2020  ()}.'.          
+00008ac0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00008ad0: 6545 7272 6f72 2865 7272 6f72 6d73 6729  eError(errormsg)
+00008ae0: 0a0a 2020 2020 2020 2020 2020 2020 7479  ..            ty
+00008af0: 7065 5f64 6973 7420 3d20 6e70 2e61 7272  pe_dist = np.arr
+00008b00: 6179 286c 6973 7428 7365 6c66 5b27 696e  ay(list(self['in
+00008b10: 6974 5f68 7076 5f64 6973 7427 5d2e 7661  it_hpv_dist'].va
+00008b20: 6c75 6573 2829 2929 0a20 2020 2020 2020  lues())).       
+00008b30: 2020 2020 2067 656e 6f74 7970 6573 203d       genotypes =
+00008b40: 2068 7075 2e63 686f 6f73 655f 7728 7479   hpu.choose_w(ty
+00008b50: 7065 5f64 6973 742c 206c 656e 2868 7076  pe_dist, len(hpv
+00008b60: 5f69 6e64 7329 2c20 756e 6971 7565 3d46  _inds), unique=F
+00008b70: 616c 7365 290a 0a20 2020 2020 2020 2066  alse)..        f
+00008b80: 6f72 2067 2069 6e20 7261 6e67 6528 6e67  or g in range(ng
+00008b90: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00008ba0: 656c 662e 7065 6f70 6c65 2e69 6e66 6563  elf.people.infec
+00008bb0: 7428 696e 6473 3d68 7076 5f69 6e64 735b  t(inds=hpv_inds[
+00008bc0: 6765 6e6f 7479 7065 733d 3d67 5d2c 2067  genotypes==g], g
+00008bd0: 3d67 2c20 6c61 7965 723d 2773 6565 645f  =g, layer='seed_
+00008be0: 696e 6665 6374 696f 6e27 290a 0a20 2020  infection')..   
+00008bf0: 2020 2020 2072 6574 7572 6e0a 0a0a 2020       return...  
+00008c00: 2020 6465 6620 7374 6570 2873 656c 6629    def step(self)
+00008c10: 3a0a 2020 2020 2020 2020 2727 2720 5374  :.        ''' St
+00008c20: 6570 2074 6872 6f75 6768 2074 696d 6520  ep through time 
+00008c30: 616e 6420 7570 6461 7465 2076 616c 7565  and update value
+00008c40: 7320 2727 270a 0a20 2020 2020 2020 2023  s '''..        #
+00008c50: 2053 6574 2074 6865 2074 696d 6520 616e   Set the time an
+00008c60: 6420 6966 2077 6520 6861 7665 2072 6561  d if we have rea
+00008c70: 6368 6564 2074 6865 2065 6e64 206f 6620  ched the end of 
+00008c80: 7468 6520 7369 6d75 6c61 7469 6f6e 2c20  the simulation, 
+00008c90: 7468 656e 2064 6f20 6e6f 7468 696e 670a  then do nothing.
+00008ca0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00008cb0: 636f 6d70 6c65 7465 3a0a 2020 2020 2020  complete:.      
+00008cc0: 2020 2020 2020 7261 6973 6520 416c 7265        raise Alre
+00008cd0: 6164 7952 756e 4572 726f 7228 2753 696d  adyRunError('Sim
+00008ce0: 756c 6174 696f 6e20 616c 7265 6164 7920  ulation already 
+00008cf0: 636f 6d70 6c65 7465 2028 6361 6c6c 2073  complete (call s
+00008d00: 696d 2e69 6e69 7469 616c 697a 6528 2920  im.initialize() 
+00008d10: 746f 2072 652d 7275 6e29 2729 0a0a 2020  to re-run)')..  
+00008d20: 2020 2020 2020 2320 5368 6f72 7465 6e20        # Shorten 
+00008d30: 6b65 7920 7661 7269 6162 6c65 730a 2020  key variables.  
+00008d40: 2020 2020 2020 6474 203d 2073 656c 665b        dt = self[
+00008d50: 2764 7427 5d20 2320 5469 6d65 7374 6570  'dt'] # Timestep
+00008d60: 0a20 2020 2020 2020 2074 203d 2073 656c  .        t = sel
+00008d70: 662e 740a 2020 2020 2020 2020 6e67 203d  f.t.        ng =
+00008d80: 2073 656c 665b 276e 5f67 656e 6f74 7970   self['n_genotyp
+00008d90: 6573 275d 0a20 2020 2020 2020 206e 6120  es'].        na 
+00008da0: 3d20 6c65 6e28 7365 6c66 2e70 6172 735b  = len(self.pars[
+00008db0: 2761 6765 5f62 696e 5f65 6467 6573 275d  'age_bin_edges']
+00008dc0: 2920 2d20 3120 2320 4e75 6d62 6572 206f  ) - 1 # Number o
+00008dd0: 6620 6167 6520 6269 6e73 0a20 2020 2020  f age bins.     
+00008de0: 2020 2063 6f6e 646f 6d73 203d 2073 656c     condoms = sel
+00008df0: 665b 2763 6f6e 646f 6d73 275d 0a20 2020  f['condoms'].   
+00008e00: 2020 2020 2065 6666 5f63 6f6e 646f 6d73       eff_condoms
+00008e10: 203d 2073 656c 665b 2765 6666 5f63 6f6e   = self['eff_con
+00008e20: 646f 6d73 275d 0a20 2020 2020 2020 2062  doms'].        b
+00008e30: 6574 6120 3d20 7365 6c66 5b27 6265 7461  eta = self['beta
+00008e40: 275d 0a20 2020 2020 2020 2067 656e 5f70  '].        gen_p
+00008e50: 6172 7320 3d20 7365 6c66 5b27 6765 6e6f  ars = self['geno
+00008e60: 7479 7065 5f70 6172 7327 5d0a 2020 2020  type_pars'].    
+00008e70: 2020 2020 696d 6d5f 6b69 6e5f 7061 7273      imm_kin_pars
+00008e80: 203d 2073 656c 665b 2769 6d6d 5f6b 696e   = self['imm_kin
+00008e90: 275d 0a20 2020 2020 2020 206d 6978 696e  '].        mixin
+00008ea0: 6720 3d20 7365 6c66 5b27 6d69 7869 6e67  g = self['mixing
+00008eb0: 275d 0a20 2020 2020 2020 206c 6179 6572  '].        layer
+00008ec0: 5f70 726f 6273 203d 2073 656c 665b 276c  _probs = self['l
+00008ed0: 6179 6572 5f70 726f 6273 275d 0a20 2020  ayer_probs'].   
+00008ee0: 2020 2020 2063 726f 7373 5f6c 6179 6572       cross_layer
+00008ef0: 203d 2073 656c 665b 2763 726f 7373 5f6c   = self['cross_l
+00008f00: 6179 6572 275d 0a20 2020 2020 2020 2061  ayer'].        a
+00008f10: 6374 7320 3d20 7365 6c66 5b27 6163 7473  cts = self['acts
+00008f20: 275d 0a20 2020 2020 2020 2064 7572 5f70  '].        dur_p
+00008f30: 7368 6970 203d 2073 656c 665b 2764 7572  ship = self['dur
+00008f40: 5f70 7368 6970 275d 0a20 2020 2020 2020  _pship'].       
+00008f50: 2061 6765 5f61 6374 5f70 6172 7320 3d20   age_act_pars = 
+00008f60: 7365 6c66 5b27 6167 655f 6163 745f 7061  self['age_act_pa
+00008f70: 7273 275d 0a20 2020 2020 2020 2074 7261  rs'].        tra
+00008f80: 6e73 203d 206e 702e 6172 7261 7928 5b73  ns = np.array([s
+00008f90: 656c 665b 2774 7261 6e73 6632 6d27 5d2c  elf['transf2m'],
+00008fa0: 7365 6c66 5b27 7472 616e 736d 3266 275d  self['transm2f']
+00008fb0: 5d29 2023 2046 324d 2066 6972 7374 2073  ]) # F2M first s
+00008fc0: 696e 6365 2074 6861 7427 7320 7468 6520  ince that's the 
+00008fd0: 6f72 6465 7220 7468 696e 6773 2061 7265  order things are
+00008fe0: 2064 6f6e 6520 6c61 7465 720a 2020 2020   done later.    
+00008ff0: 2020 2020 7965 6172 203d 2073 656c 662e      year = self.
+00009000: 7965 6172 7665 635b 745d 0a0a 2020 2020  yearvec[t]..    
+00009010: 2020 2020 2320 4d61 6b65 2048 4956 2d72      # Make HIV-r
+00009020: 656c 6174 6564 2075 7064 6174 6573 0a20  elated updates. 
+00009030: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00009040: 6172 735b 276d 6f64 656c 5f68 6976 275d  ars['model_hiv']
+00009050: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009060: 6c66 2e68 6976 7369 6d2e 7374 6570 2870  lf.hivsim.step(p
+00009070: 656f 706c 653d 7365 6c66 2e70 656f 706c  eople=self.peopl
+00009080: 652c 2079 6561 723d 7965 6172 290a 0a20  e, year=year).. 
+00009090: 2020 2020 2020 2023 2055 7064 6174 6520         # Update 
+000090a0: 6465 6d6f 6772 6170 6869 6373 2c20 7374  demographics, st
+000090b0: 6174 6573 2c20 616e 6420 7061 7274 6e65  ates, and partne
+000090c0: 7273 6869 7073 0a20 2020 2020 2020 2073  rships.        s
+000090d0: 656c 662e 7065 6f70 6c65 2e75 7064 6174  elf.people.updat
+000090e0: 655f 7374 6174 6573 5f70 7265 2874 3d74  e_states_pre(t=t
+000090f0: 2c20 7965 6172 3d79 6561 7229 2023 2054  , year=year) # T
+00009100: 6869 7320 616c 736f 2061 6765 7320 7065  his also ages pe
+00009110: 6f70 6c65 2c20 6170 706c 6965 7320 6465  ople, applies de
+00009120: 6174 6873 2c20 616e 6420 6765 6e65 7261  aths, and genera
+00009130: 7465 7320 6e65 7720 6269 7274 6873 0a20  tes new births. 
+00009140: 2020 2020 2020 2070 656f 706c 6520 3d20         people = 
+00009150: 7365 6c66 2e70 656f 706c 6520 2320 5368  self.people # Sh
+00009160: 6f72 7465 6e0a 2020 2020 2020 2020 7065  orten.        pe
+00009170: 6f70 6c65 2e64 6973 736f 6c76 655f 7061  ople.dissolve_pa
+00009180: 7274 6e65 7273 6869 7073 2874 3d74 2920  rtnerships(t=t) 
+00009190: 2320 4469 7373 6f6c 7665 2070 6172 746e  # Dissolve partn
+000091a0: 6572 7368 6970 730a 2020 2020 2020 2020  erships.        
+000091b0: 7469 6e64 203d 2073 656c 662e 7965 6172  tind = self.year
+000091c0: 7665 635b 745d 202d 2073 656c 665b 2773  vec[t] - self['s
+000091d0: 7461 7274 275d 0a20 2020 2020 2020 2070  tart'].        p
+000091e0: 656f 706c 652e 6372 6561 7465 5f70 6172  eople.create_par
+000091f0: 746e 6572 7368 6970 7328 7469 6e64 2c20  tnerships(tind, 
+00009200: 6d69 7869 6e67 2c20 6c61 7965 725f 7072  mixing, layer_pr
+00009210: 6f62 732c 2063 726f 7373 5f6c 6179 6572  obs, cross_layer
+00009220: 2c20 6475 725f 7073 6869 702c 2061 6374  , dur_pship, act
+00009230: 732c 2061 6765 5f61 6374 5f70 6172 7329  s, age_act_pars)
+00009240: 0a0a 2020 2020 2020 2020 2320 4170 706c  ..        # Appl
+00009250: 7920 696e 7465 7276 656e 7469 6f6e 730a  y interventions.
+00009260: 2020 2020 2020 2020 666f 7220 692c 696e          for i,in
+00009270: 7465 7276 656e 7469 6f6e 2069 6e20 656e  tervention in en
+00009280: 756d 6572 6174 6528 7365 6c66 2e69 6e74  umerate(self.int
+00009290: 6572 7665 6e74 696f 6e73 293a 0a20 2020  erventions):.   
+000092a0: 2020 2020 2020 2020 2069 6e74 6572 7665           interve
+000092b0: 6e74 696f 6e28 7365 6c66 2920 2320 4966  ntion(self) # If
+000092c0: 2069 7427 7320 6120 6675 6e63 7469 6f6e   it's a function
+000092d0: 2c20 6361 6c6c 2069 7420 6469 7265 6374  , call it direct
+000092e0: 6c79 0a0a 2020 2020 2020 2020 2320 4173  ly..        # As
+000092f0: 7369 676e 2073 7573 5f69 6d6d 2076 616c  sign sus_imm val
+00009300: 7565 732c 2069 2e65 2e20 7468 6520 7072  ues, i.e. the pr
+00009310: 6f74 6563 7469 6f6e 2061 6761 696e 7374  otection against
+00009320: 2069 6e66 6563 7469 6f6e 2062 6173 6564   infection based
+00009330: 206f 6e20 7072 696f 7220 696d 6d75 6e65   on prior immune
+00009340: 2068 6973 746f 7279 0a20 2020 2020 2020   history.       
+00009350: 2069 6620 7365 6c66 5b27 7573 655f 7761   if self['use_wa
+00009360: 6e69 6e67 275d 3a0a 2020 2020 2020 2020  ning']:.        
+00009370: 2020 2020 696e 6473 203d 2068 7075 2e74      inds = hpu.t
+00009380: 7275 6528 7065 6f70 6c65 2e70 6561 6b5f  rue(people.peak_
+00009390: 696d 6d2e 7375 6d28 6178 6973 3d30 2929  imm.sum(axis=0))
+000093a0: 2e61 7374 7970 6528 6870 642e 6465 6661  .astype(hpd.defa
+000093b0: 756c 745f 696e 7429 0a20 2020 2020 2020  ult_int).       
+000093c0: 2020 2020 2069 6620 6c65 6e28 696e 6473       if len(inds
+000093d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000093e0: 2020 2073 7320 3d20 7065 6f70 6c65 2e74     ss = people.t
+000093f0: 5f69 6d6d 5f65 7665 6e74 5b3a 2c20 696e  _imm_event[:, in
+00009400: 6473 5d2e 7368 6170 650a 2020 2020 2020  ds].shape.      
+00009410: 2020 2020 2020 2020 2020 745f 7369 6e63            t_sinc
+00009420: 655f 626f 6f73 7420 3d20 2874 202d 2070  e_boost = (t - p
+00009430: 656f 706c 652e 745f 696d 6d5f 6576 656e  eople.t_imm_even
+00009440: 745b 3a2c 696e 6473 5d29 2e72 6176 656c  t[:,inds]).ravel
+00009450: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00009460: 2020 2063 7572 7265 6e74 5f69 6d6d 203d     current_imm =
+00009470: 2069 6d6d 5f6b 696e 5f70 6172 735b 745f   imm_kin_pars[t_
+00009480: 7369 6e63 655f 626f 6f73 745d 2e72 6573  since_boost].res
+00009490: 6861 7065 2873 7329 2023 2047 6574 2070  hape(ss) # Get p
+000094a0: 656f 706c 6527 7320 6375 7272 656e 7420  eople's current 
+000094b0: 6c65 7665 6c20 6f66 2069 6d6d 756e 6974  level of immunit
+000094c0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+000094d0: 2020 7065 6f70 6c65 2e6e 6162 5f69 6d6d    people.nab_imm
+000094e0: 5b3a 2c69 6e64 735d 203d 2063 7572 7265  [:,inds] = curre
+000094f0: 6e74 5f69 6d6d 2a70 656f 706c 652e 7065  nt_imm*people.pe
+00009500: 616b 5f69 6d6d 5b3a 2c69 6e64 735d 2023  ak_imm[:,inds] #
+00009510: 2053 6574 2069 6d6d 756e 6974 7920 7265   Set immunity re
+00009520: 6c61 7469 7665 2074 6f20 7065 616b 0a20  lative to peak. 
+00009530: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00009540: 2020 2020 2020 2020 2070 656f 706c 652e           people.
+00009550: 6e61 625f 696d 6d5b 3a5d 203d 2070 656f  nab_imm[:] = peo
+00009560: 706c 652e 7065 616b 5f69 6d6d 0a20 2020  ple.peak_imm.   
+00009570: 2020 2020 2068 7069 6d6d 2e63 6865 636b       hpimm.check
+00009580: 5f69 6d6d 756e 6974 7928 7065 6f70 6c65  _immunity(people
+00009590: 290a 0a20 2020 2020 2020 2023 2053 686f  )..        # Sho
+000095a0: 7274 656e 206d 6f72 6520 7661 7269 6162  rten more variab
+000095b0: 6c65 730a 2020 2020 2020 2020 6765 6e5f  les.        gen_
+000095c0: 6265 7461 7320 3d20 6e70 2e61 7272 6179  betas = np.array
+000095d0: 285b 675b 2772 656c 5f62 6574 6127 5d20  ([g['rel_beta'] 
+000095e0: 2a20 6265 7461 2066 6f72 2067 2069 6e20  * beta for g in 
+000095f0: 6765 6e5f 7061 7273 2e76 616c 7565 7328  gen_pars.values(
+00009600: 295d 2c20 6474 7970 653d 6870 642e 6465  )], dtype=hpd.de
+00009610: 6661 756c 745f 666c 6f61 7429 0a20 2020  fault_float).   
+00009620: 2020 2020 2073 7573 5f69 6d6d 203d 2070       sus_imm = p
+00009630: 656f 706c 652e 7375 735f 696d 6d0a 2020  eople.sus_imm.  
+00009640: 2020 2020 2020 7265 6c5f 7375 7320 3d20        rel_sus = 
+00009650: 7065 6f70 6c65 2e72 656c 5f73 7573 0a0a  people.rel_sus..
+00009660: 2020 2020 2020 2020 696e 6620 3d20 7065          inf = pe
+00009670: 6f70 6c65 2e69 6e66 6563 7469 6f75 732e  ople.infectious.
+00009680: 636f 7079 2829 2023 2063 616c 6375 6c61  copy() # calcula
+00009690: 7465 2074 7261 6e73 6d69 7373 696f 6e20  te transmission 
+000096a0: 6261 7365 6420 6f6e 2069 6e66 6563 7469  based on infecti
+000096b0: 6f75 736e 6573 7320 6174 2073 7461 7274  ousness at start
+000096c0: 206f 6620 7469 6d65 7374 6570 2069 2e65   of timestep i.e
+000096d0: 2e20 736f 6d65 6f6e 6520 696e 6665 6374  . someone infect
+000096e0: 6564 2069 6e20 6f6e 6520 6c61 7965 7220  ed in one layer 
+000096f0: 6361 6e6e 6f74 2074 7261 6e73 6d69 7420  cannot transmit 
+00009700: 7468 6520 696e 6665 6374 696f 6e20 7669  the infection vi
+00009710: 6120 6120 6469 6666 6572 656e 7420 6c61  a a different la
+00009720: 7965 7220 696e 2074 6865 2073 616d 6520  yer in the same 
+00009730: 7469 6d65 7374 6570 0a0a 2020 2020 2020  timestep..      
+00009740: 2020 2320 4c6f 6f70 206f 7665 7220 6c61    # Loop over la
+00009750: 7965 7273 0a20 2020 2020 2020 2066 6f72  yers.        for
+00009760: 206c 6b65 792c 206c 6179 6572 2069 6e20   lkey, layer in 
+00009770: 7065 6f70 6c65 2e63 6f6e 7461 6374 732e  people.contacts.
+00009780: 6974 656d 7328 293a 0a0a 2020 2020 2020  items():..      
+00009790: 2020 2020 2020 7375 7320 3d20 7065 6f70        sus = peop
+000097a0: 6c65 2e73 7573 6365 7074 6962 6c65 2e63  le.susceptible.c
+000097b0: 6f70 7928 2920 2320 666f 7220 6561 6368  opy() # for each
+000097c0: 206c 6179 6572 2c20 7570 6461 7465 2077   layer, update w
+000097d0: 686f 2773 2073 7469 6c6c 2073 7573 6365  ho's still susce
+000097e0: 7074 6962 6c65 0a0a 2020 2020 2020 2020  ptible..        
+000097f0: 2020 2020 2320 5368 6f72 7465 6e20 7661      # Shorten va
+00009800: 7269 6162 6c65 730a 2020 2020 2020 2020  riables.        
+00009810: 2020 2020 6620 3d20 6c61 7965 725b 2766      f = layer['f
+00009820: 275d 0a20 2020 2020 2020 2020 2020 206d  '].            m
+00009830: 203d 206c 6179 6572 5b27 6d27 5d0a 2020   = layer['m'].  
+00009840: 2020 2020 2020 2020 2020 6163 7473 203d            acts =
+00009850: 206c 6179 6572 5b27 6163 7473 275d 202a   layer['acts'] *
+00009860: 2064 740a 2020 2020 2020 2020 2020 2020   dt.            
+00009870: 6672 6163 5f61 6374 732c 2077 686f 6c65  frac_acts, whole
+00009880: 5f61 6374 7320 3d20 6e70 2e6d 6f64 6628  _acts = np.modf(
+00009890: 6163 7473 290a 2020 2020 2020 2020 2020  acts).          
+000098a0: 2020 7768 6f6c 655f 6163 7473 203d 2077    whole_acts = w
+000098b0: 686f 6c65 5f61 6374 732e 6173 7479 7065  hole_acts.astype
+000098c0: 2868 7064 2e64 6566 6175 6c74 5f69 6e74  (hpd.default_int
+000098d0: 290a 2020 2020 2020 2020 2020 2020 6566  ).            ef
+000098e0: 6665 6374 6976 655f 636f 6e64 6f6d 7320  fective_condoms 
+000098f0: 3d20 6870 642e 6465 6661 756c 745f 666c  = hpd.default_fl
+00009900: 6f61 7428 636f 6e64 6f6d 735b 6c6b 6579  oat(condoms[lkey
+00009910: 5d20 2a20 6566 665f 636f 6e64 6f6d 7329  ] * eff_condoms)
+00009920: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00009930: 436f 6d70 7574 6520 7472 616e 736d 6973  Compute transmis
+00009940: 7369 6f6e 7320 6279 2067 656e 6f74 7970  sions by genotyp
+00009950: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
+00009960: 7220 6720 696e 2072 616e 6765 286e 6729  r g in range(ng)
+00009970: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
+00009980: 2020 2066 5f73 6f75 7263 655f 696e 6473     f_source_inds
+00009990: 203d 2028 696e 665b 675d 5b66 5d20 2620   = (inf[g][f] & 
+000099a0: 7375 735b 675d 5b6d 5d29 2e6e 6f6e 7a65  sus[g][m]).nonze
+000099b0: 726f 2829 5b30 5d20 2023 2067 6574 2066  ro()[0]  # get f
+000099c0: 656d 616c 6520 736f 7572 6365 7320 7768  emale sources wh
+000099d0: 6572 6520 6665 6d61 6c65 2070 6172 746e  ere female partn
+000099e0: 6572 2069 7320 696e 6665 6374 696f 7573  er is infectious
+000099f0: 2077 6974 6820 6765 6e6f 7479 7065 2061   with genotype a
+00009a00: 6e64 206d 616c 6520 7061 7274 6e65 7220  nd male partner 
+00009a10: 6973 2073 7573 6365 7074 6962 6c65 2074  is susceptible t
+00009a20: 6f20 7468 6174 2067 656e 6f74 7970 650a  o that genotype.
+00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a40: 6d5f 736f 7572 6365 5f69 6e64 7320 3d20  m_source_inds = 
+00009a50: 2869 6e66 5b67 5d5b 6d5d 2026 2073 7573  (inf[g][m] & sus
+00009a60: 5b67 5d5b 665d 292e 6e6f 6e7a 6572 6f28  [g][f]).nonzero(
+00009a70: 295b 305d 2020 2320 6765 7420 6d61 6c65  )[0]  # get male
+00009a80: 2073 6f75 7263 6573 2077 6865 7265 2074   sources where t
+00009a90: 6865 206d 616c 6520 7061 7274 6e65 7220  he male partner 
+00009aa0: 6973 2069 6e66 6563 7469 6f75 7320 7769  is infectious wi
+00009ab0: 7468 2067 656e 6f74 7970 6520 616e 6420  th genotype and 
+00009ac0: 7468 6520 6665 6d61 6c65 2070 6172 746e  the female partn
+00009ad0: 6572 2069 7320 7375 7363 6570 7469 626c  er is susceptibl
+00009ae0: 6520 746f 2074 6861 7420 6765 6e6f 7479  e to that genoty
+00009af0: 7065 0a0a 2020 2020 2020 2020 2020 2020  pe..            
+00009b00: 2020 2020 666f 695f 6672 6163 203d 2031      foi_frac = 1
+00009b10: 202d 2066 7261 635f 6163 7473 202a 2067   - frac_acts * g
+00009b20: 656e 5f62 6574 6173 5b67 5d20 2a20 7472  en_betas[g] * tr
+00009b30: 616e 735b 3a2c 204e 6f6e 655d 202a 2028  ans[:, None] * (
+00009b40: 3120 2d20 6566 6665 6374 6976 655f 636f  1 - effective_co
+00009b50: 6e64 6f6d 7329 2020 2320 5072 6f62 6162  ndoms)  # Probab
+00009b60: 696c 6974 7920 6f66 206e 6f74 2067 6574  ility of not get
+00009b70: 7469 6e67 2069 6e66 6563 7465 6420 6672  ting infected fr
+00009b80: 6f6d 2061 6e79 2066 7261 6374 696f 6e61  om any fractiona
+00009b90: 6c20 6163 7473 0a20 2020 2020 2020 2020  l acts.         
+00009ba0: 2020 2020 2020 2066 6f69 5f77 686f 6c65         foi_whole
+00009bb0: 203d 2028 3120 2d20 6765 6e5f 6265 7461   = (1 - gen_beta
+00009bc0: 735b 675d 202a 2074 7261 6e73 5b3a 2c20  s[g] * trans[:, 
+00009bd0: 4e6f 6e65 5d20 2a20 2831 202d 2065 6666  None] * (1 - eff
+00009be0: 6563 7469 7665 5f63 6f6e 646f 6d73 2929  ective_condoms))
+00009bf0: 202a 2a20 7768 6f6c 655f 6163 7473 2020   ** whole_acts  
+00009c00: 2320 5072 6f62 6162 696c 6974 7920 6f66  # Probability of
+00009c10: 206e 6f74 2067 6574 7469 6e67 2069 6e66   not getting inf
+00009c20: 6563 7465 6420 6672 6f6d 2077 686f 6c65  ected from whole
+00009c30: 2061 6374 730a 2020 2020 2020 2020 2020   acts.          
+00009c40: 2020 2020 2020 666f 6920 3d20 2831 202d        foi = (1 -
+00009c50: 2028 666f 695f 7768 6f6c 6520 2a20 666f   (foi_whole * fo
+00009c60: 695f 6672 6163 2929 2e61 7374 7970 6528  i_frac)).astype(
+00009c70: 6870 642e 6465 6661 756c 745f 666c 6f61  hpd.default_floa
+00009c80: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
+00009c90: 2020 2020 6469 7363 6f72 6461 6e74 5f70      discordant_p
+00009ca0: 6169 7273 203d 205b 5b66 5f73 6f75 7263  airs = [[f_sourc
+00009cb0: 655f 696e 6473 2c20 665b 665f 736f 7572  e_inds, f[f_sour
+00009cc0: 6365 5f69 6e64 735d 2c20 6d5b 665f 736f  ce_inds], m[f_so
+00009cd0: 7572 6365 5f69 6e64 735d 2c20 666f 695b  urce_inds], foi[
+00009ce0: 302c 3a5d 5d2c 0a20 2020 2020 2020 2020  0,:]],.         
+00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d00: 2020 2020 2020 2020 2020 205b 6d5f 736f             [m_so
+00009d10: 7572 6365 5f69 6e64 732c 206d 5b6d 5f73  urce_inds, m[m_s
+00009d20: 6f75 7263 655f 696e 6473 5d2c 2066 5b6d  ource_inds], f[m
+00009d30: 5f73 6f75 7263 655f 696e 6473 5d2c 2066  _source_inds], f
+00009d40: 6f69 5b31 2c3a 5d5d 5d0a 0a20 2020 2020  oi[1,:]]]..     
+00009d50: 2020 2020 2020 2020 2020 2023 2043 6f6d             # Com
+00009d60: 7075 7465 2074 7261 6e73 6d69 7373 6962  pute transmissib
+00009d70: 696c 6974 7920 666f 7220 6561 6368 2070  ility for each p
+00009d80: 6172 746e 6572 7368 6970 0a20 2020 2020  artnership.     
+00009d90: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+00009da0: 7368 6970 5f69 6e64 732c 2073 6f75 7263  ship_inds, sourc
+00009db0: 6573 2c20 7461 7267 6574 732c 2074 6869  es, targets, thi
+00009dc0: 735f 666f 6920 696e 2064 6973 636f 7264  s_foi in discord
+00009dd0: 616e 745f 7061 6972 733a 0a20 2020 2020  ant_pairs:.     
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00009df0: 6574 6173 203d 2074 6869 735f 666f 695b  etas = this_foi[
+00009e00: 7073 6869 705f 696e 6473 5d20 2a20 2831  pship_inds] * (1
+00009e10: 2e20 2d20 7375 735f 696d 6d5b 672c 7461  . - sus_imm[g,ta
+00009e20: 7267 6574 735d 2920 2a20 7265 6c5f 7375  rgets]) * rel_su
+00009e30: 735b 7461 7267 6574 735d 2023 2050 756c  s[targets] # Pul
+00009e40: 6c20 6f75 7420 7468 6520 7472 616e 736d  l out the transm
+00009e50: 6973 7369 6269 6c69 7479 2061 7373 6f63  issibility assoc
+00009e60: 6961 7465 6420 7769 7468 2074 6869 7320  iated with this 
+00009e70: 7061 7274 6e65 7273 6869 700a 2020 2020  partnership.    
+00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e90: 7472 616e 736d 6973 7369 6f6e 7320 3d20  transmissions = 
+00009ea0: 286e 702e 7261 6e64 6f6d 2e72 616e 646f  (np.random.rando
+00009eb0: 6d28 6c65 6e28 6265 7461 7329 2920 3c20  m(len(betas)) < 
+00009ec0: 6265 7461 7329 2e6e 6f6e 7a65 726f 2829  betas).nonzero()
+00009ed0: 5b30 5d20 2320 4170 706c 7920 7072 6f62  [0] # Apply prob
+00009ee0: 6162 696c 6974 6965 7320 746f 2064 6574  abilities to det
+00009ef0: 6572 6d69 6e65 2070 6172 746e 6572 7368  ermine partnersh
+00009f00: 6970 7320 696e 2077 6869 6368 2074 7261  ips in which tra
+00009f10: 6e73 6d69 7373 696f 6e20 6f63 6375 7272  nsmission occurr
+00009f20: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00009f30: 2020 2020 2020 2074 6172 6765 745f 696e         target_in
+00009f40: 6473 2020 203d 2074 6172 6765 7473 5b74  ds   = targets[t
+00009f50: 7261 6e73 6d69 7373 696f 6e73 5d20 2320  ransmissions] # 
+00009f60: 4578 7472 6163 7420 696e 6469 6365 7320  Extract indices 
+00009f70: 6f66 2074 686f 7365 2077 686f 2067 6f74  of those who got
+00009f80: 2069 6e66 6563 7465 640a 2020 2020 2020   infected.      
+00009f90: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00009fa0: 7267 6574 5f69 6e64 732c 2075 6e69 7175  rget_inds, uniqu
+00009fb0: 655f 696e 6473 203d 206e 702e 756e 6971  e_inds = np.uniq
+00009fc0: 7565 2874 6172 6765 745f 696e 6473 2c20  ue(target_inds, 
+00009fd0: 7265 7475 726e 5f69 6e64 6578 3d54 7275  return_index=Tru
+00009fe0: 6529 2020 2320 4475 6520 746f 206d 756c  e)  # Due to mul
+00009ff0: 7469 706c 6520 7061 7274 6e65 7273 6869  tiple partnershi
+0000a000: 7073 2c20 736f 6d65 2070 656f 706c 6520  ps, some people 
+0000a010: 7769 6c6c 2062 6520 636f 756e 7465 6420  will be counted 
+0000a020: 7477 6963 653b 2072 656d 6f76 6520 7468  twice; remove th
+0000a030: 656d 0a20 2020 2020 2020 2020 2020 2020  em.             
+0000a040: 2020 2020 2020 2070 656f 706c 652e 696e         people.in
+0000a050: 6665 6374 2869 6e64 733d 7461 7267 6574  fect(inds=target
+0000a060: 5f69 6e64 732c 2067 3d67 2c20 6c61 7965  _inds, g=g, laye
+0000a070: 723d 6c6b 6579 2920 2023 2049 6e66 6563  r=lkey)  # Infec
+0000a080: 7420 7065 6f70 6c65 0a0a 2020 2020 2020  t people..      
+0000a090: 2020 2320 4465 7465 726d 696e 6520 6966    # Determine if
+0000a0a0: 2074 6865 7265 2061 7265 2061 6e79 2072   there are any r
+0000a0b0: 6561 6374 6976 6174 6564 2069 6e66 6563  eactivated infec
+0000a0c0: 7469 6f6e 7320 6f6e 2074 6869 7320 7469  tions on this ti
+0000a0d0: 6d65 7374 6570 0a20 2020 2020 2020 2066  mestep.        f
+0000a0e0: 6f72 2067 2069 6e20 7261 6e67 6528 6e67  or g in range(ng
+0000a0f0: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+0000a100: 6174 656e 745f 696e 6473 203d 2068 7075  atent_inds = hpu
+0000a110: 2e74 7275 6528 7065 6f70 6c65 2e6c 6174  .true(people.lat
+0000a120: 656e 745b 672c 3a5d 290a 2020 2020 2020  ent[g,:]).      
+0000a130: 2020 2020 2020 6966 206c 656e 286c 6174        if len(lat
+0000a140: 656e 745f 696e 6473 293a 0a20 2020 2020  ent_inds):.     
+0000a150: 2020 2020 2020 2020 2020 2072 6561 6374             react
+0000a160: 6976 6174 696f 6e5f 7072 6f62 7320 3d20  ivation_probs = 
+0000a170: 6e70 2e66 756c 6c5f 6c69 6b65 286c 6174  np.full_like(lat
+0000a180: 656e 745f 696e 6473 2c20 7365 6c66 5b27  ent_inds, self['
+0000a190: 6870 765f 7265 6163 7469 7661 7469 6f6e  hpv_reactivation
+0000a1a0: 275d 202a 2064 742c 2064 7479 7065 3d68  '] * dt, dtype=h
+0000a1b0: 7064 2e64 6566 6175 6c74 5f66 6c6f 6174  pd.default_float
+0000a1c0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a1d0: 2020 2023 2069 6620 7365 6c66 5b27 6d6f     # if self['mo
+0000a1e0: 6465 6c5f 6869 7627 5d3a 0a20 2020 2020  del_hiv']:.     
+0000a1f0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0000a200: 2023 2064 6574 6572 6d69 6e65 2069 6620   # determine if 
+0000a210: 616e 7920 6f66 2074 6865 7365 2069 6e64  any of these ind
+0000a220: 7320 6861 7665 2048 4956 2061 6e64 2061  s have HIV and a
+0000a230: 646a 7573 7420 7468 6569 7220 7072 6f62  djust their prob
+0000a240: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000a250: 2020 2320 2020 2020 6869 765f 6c61 7465    #     hiv_late
+0000a260: 6e74 5f69 6e64 7320 3d20 6c61 7465 6e74  nt_inds = latent
+0000a270: 5f69 6e64 735b 6870 752e 7472 7565 2870  _inds[hpu.true(p
+0000a280: 656f 706c 652e 6869 765b 6c61 7465 6e74  eople.hiv[latent
+0000a290: 5f69 6e64 735d 295d 0a20 2020 2020 2020  _inds])].       
+0000a2a0: 2020 2020 2020 2020 2023 2020 2020 2069           #     i
+0000a2b0: 6620 6c65 6e28 6869 765f 6c61 7465 6e74  f len(hiv_latent
+0000a2c0: 5f69 6e64 7329 3a0a 2020 2020 2020 2020  _inds):.        
+0000a2d0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0000a2e0: 2020 696d 6d75 6e65 5f63 6f6d 7072 6f6d    immune_comprom
+0000a2f0: 6973 6520 3d20 3120 2d20 7065 6f70 6c65  ise = 1 - people
+0000a300: 2e61 7274 5f61 6468 6572 656e 6365 5b68  .art_adherence[h
+0000a310: 6976 5f6c 6174 656e 745f 696e 6473 5d0a  iv_latent_inds].
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a330: 2320 2020 2020 2020 2020 6d6f 6420 3d20  #         mod = 
+0000a340: 696d 6d75 6e65 5f63 6f6d 7072 6f6d 6973  immune_compromis
+0000a350: 6520 2a20 7365 6c66 5b27 6869 765f 7061  e * self['hiv_pa
+0000a360: 7273 275d 5b27 7265 6163 7469 7661 7469  rs']['reactivati
+0000a370: 6f6e 5f70 726f 6227 5d0a 2020 2020 2020  on_prob'].      
+0000a380: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0000a390: 2020 2020 6d6f 645b 6d6f 6420 3c20 315d      mod[mod < 1]
+0000a3a0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+0000a3b0: 2020 2020 2023 2020 2020 2020 2020 2072       #         r
+0000a3c0: 6561 6374 6976 6174 696f 6e5f 7072 6f62  eactivation_prob
+0000a3d0: 735b 6870 752e 7472 7565 2870 656f 706c  s[hpu.true(peopl
+0000a3e0: 652e 6869 765b 6c61 7465 6e74 5f69 6e64  e.hiv[latent_ind
+0000a3f0: 735d 295d 202a 3d20 6d6f 640a 2020 2020  s])] *= mod.    
+0000a400: 2020 2020 2020 2020 2020 2020 6973 5f72              is_r
+0000a410: 6561 6374 6976 6174 6564 203d 2068 7075  eactivated = hpu
+0000a420: 2e62 696e 6f6d 6961 6c5f 6172 7228 7265  .binomial_arr(re
+0000a430: 6163 7469 7661 7469 6f6e 5f70 726f 6273  activation_probs
+0000a440: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a450: 2020 7265 6163 7469 7661 7465 645f 696e    reactivated_in
+0000a460: 6473 203d 206c 6174 656e 745f 696e 6473  ds = latent_inds
+0000a470: 5b69 735f 7265 6163 7469 7661 7465 645d  [is_reactivated]
+0000a480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a490: 2070 656f 706c 652e 696e 6665 6374 2869   people.infect(i
+0000a4a0: 6e64 733d 7265 6163 7469 7661 7465 645f  nds=reactivated_
+0000a4b0: 696e 6473 2c20 673d 672c 206c 6179 6572  inds, g=g, layer
+0000a4c0: 3d27 7265 6163 7469 7661 7469 6f6e 2729  ='reactivation')
+0000a4d0: 0a0a 2020 2020 2020 2020 2320 496e 6465  ..        # Inde
+0000a4e0: 7820 666f 7220 7265 7375 6c74 730a 2020  x for results.  
+0000a4f0: 2020 2020 2020 6964 7820 3d20 696e 7428        idx = int(
+0000a500: 7420 2f20 7365 6c66 2e72 6573 6672 6571  t / self.resfreq
+0000a510: 290a 0a20 2020 2020 2020 2023 2055 7064  )..        # Upd
+0000a520: 6174 6520 636f 756e 7473 2066 6f72 2074  ate counts for t
+0000a530: 6869 7320 7469 6d65 2073 7465 703a 2066  his time step: f
+0000a540: 6c6f 7773 0a20 2020 2020 2020 2066 6f72  lows.        for
+0000a550: 206b 6579 2c63 6f75 6e74 2069 6e20 7065   key,count in pe
+0000a560: 6f70 6c65 2e66 6c6f 7773 2e69 7465 6d73  ople.flows.items
+0000a570: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000a580: 7365 6c66 2e72 6573 756c 7473 5b6b 6579  self.results[key
+0000a590: 5d5b 6964 785d 202b 3d20 636f 756e 740a  ][idx] += count.
+0000a5a0: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
+0000a5b0: 636f 756e 7420 696e 2070 656f 706c 652e  count in people.
+0000a5c0: 6465 6d6f 6772 6170 6869 635f 666c 6f77  demographic_flow
+0000a5d0: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
+0000a5e0: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
+0000a5f0: 6c74 735b 6b65 795d 5b69 6478 5d20 2b3d  lts[key][idx] +=
+0000a600: 2063 6f75 6e74 0a20 2020 2020 2020 2066   count.        f
+0000a610: 6f72 206b 6579 2c63 6f75 6e74 2069 6e20  or key,count in 
+0000a620: 7065 6f70 6c65 2e67 656e 6f74 7970 655f  people.genotype_
+0000a630: 666c 6f77 732e 6974 656d 7328 293a 0a20  flows.items():. 
+0000a640: 2020 2020 2020 2020 2020 2066 6c6f 775f             flow_
+0000a650: 696e 6420 3d20 5b66 6c6f 772e 6e61 6d65  ind = [flow.name
+0000a660: 2066 6f72 2066 6c6f 7720 696e 2068 7064   for flow in hpd
+0000a670: 2e66 6c6f 7773 5d2e 696e 6465 7828 6b65  .flows].index(ke
+0000a680: 7929 0a20 2020 2020 2020 2020 2020 2069  y).            i
+0000a690: 6620 6870 642e 666c 6f77 735b 666c 6f77  f hpd.flows[flow
+0000a6a0: 5f69 6e64 5d2e 6279 5f67 656e 6f74 7970  _ind].by_genotyp
+0000a6b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000a6c0: 2020 2066 6f72 2067 656e 6f74 7970 6520     for genotype 
+0000a6d0: 696e 2072 616e 6765 286e 6729 3a0a 2020  in range(ng):.  
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6f0: 2020 7365 6c66 2e72 6573 756c 7473 5b6b    self.results[k
+0000a700: 6579 2b27 5f62 795f 6765 6e6f 7479 7065  ey+'_by_genotype
+0000a710: 275d 5b67 656e 6f74 7970 655d 5b69 6478  '][genotype][idx
+0000a720: 5d20 2b3d 2063 6f75 6e74 5b67 656e 6f74  ] += count[genot
+0000a730: 7970 655d 0a20 2020 2020 2020 2066 6f72  ype].        for
+0000a740: 206b 6579 2c63 6f75 6e74 2069 6e20 7065   key,count in pe
+0000a750: 6f70 6c65 2e73 6578 5f66 6c6f 7773 2e69  ople.sex_flows.i
+0000a760: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+0000a770: 2020 2020 666f 7220 7365 7820 696e 2072      for sex in r
+0000a780: 616e 6765 2832 293a 0a20 2020 2020 2020  ange(2):.       
+0000a790: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0000a7a0: 7375 6c74 735b 6b65 795d 5b73 6578 5d5b  sults[key][sex][
+0000a7b0: 6964 785d 202b 3d20 636f 756e 745b 7365  idx] += count[se
+0000a7c0: 785d 0a20 2020 2020 2020 2066 6f72 206b  x].        for k
+0000a7d0: 6579 2c63 6f75 6e74 2069 6e20 7065 6f70  ey,count in peop
+0000a7e0: 6c65 2e61 6765 5f66 6c6f 7773 2e69 7465  le.age_flows.ite
+0000a7f0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0000a800: 2020 7365 6c66 2e72 6573 756c 7473 5b6b    self.results[k
+0000a810: 6579 2b27 5f62 795f 6167 6527 5d5b 3a2c  ey+'_by_age'][:,
+0000a820: 6964 785d 202b 3d20 636f 756e 740a 0a20  idx] += count.. 
+0000a830: 2020 2020 2020 2023 204d 616b 6520 7374         # Make st
+0000a840: 6f63 6b20 7570 6461 7465 7320 6576 6572  ock updates ever
+0000a850: 7920 6e74 6820 7374 6570 2c20 7768 6572  y nth step, wher
+0000a860: 6520 6e20 6973 2074 6865 2066 7265 7175  e n is the frequ
+0000a870: 656e 6379 206f 6620 7265 7375 6c74 206f  ency of result o
+0000a880: 7574 7075 740a 2020 2020 2020 2020 6966  utput.        if
+0000a890: 2074 2025 2073 656c 662e 7265 7366 7265   t % self.resfre
+0000a8a0: 7120 3d3d 2073 656c 662e 7265 7366 7265  q == self.resfre
+0000a8b0: 712d 313a 0a0a 2020 2020 2020 2020 2020  q-1:..          
+0000a8c0: 2020 2320 4e75 6d62 6572 2069 6e66 6563    # Number infec
+0000a8d0: 7469 6f75 732f 7375 7363 6570 7469 626c  tious/susceptibl
+0000a8e0: 6520 6279 2061 6765 2c20 666f 7220 7072  e by age, for pr
+0000a8f0: 6576 616c 656e 6365 2063 616c 6375 6c61  evalence calcula
+0000a900: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+0000a910: 2020 665f 696e 6473 203d 2068 7075 2e74    f_inds = hpu.t
+0000a920: 7275 6528 7065 6f70 6c65 5b27 7365 7827  rue(people['sex'
+0000a930: 5d3d 3d30 290a 2020 2020 2020 2020 2020  ]==0).          
+0000a940: 2020 696e 6669 6e64 7320 3d20 6870 752e    infinds = hpu.
+0000a950: 7472 7565 2870 656f 706c 655b 2769 6e66  true(people['inf
+0000a960: 6563 7469 6f75 7327 5d29 0a20 2020 2020  ectious']).     
+0000a970: 2020 2020 2020 2066 5f69 6e66 696e 6473         f_infinds
+0000a980: 203d 206e 702e 696e 7465 7273 6563 7431   = np.intersect1
+0000a990: 6428 665f 696e 6473 2c20 696e 6669 6e64  d(f_inds, infind
+0000a9a0: 7329 0a20 2020 2020 2020 2020 2020 2073  s).            s
+0000a9b0: 656c 662e 7265 7375 6c74 735b 6627 6e5f  elf.results[f'n_
+0000a9c0: 6665 6d61 6c65 735f 696e 6665 6374 696f  females_infectio
+0000a9d0: 7573 5f62 795f 6167 6527 5d5b 3a2c 2069  us_by_age'][:, i
+0000a9e0: 6478 5d20 3d20 6e70 2e68 6973 746f 6772  dx] = np.histogr
+0000a9f0: 616d 2870 656f 706c 652e 6167 655b 665f  am(people.age[f_
+0000aa00: 696e 6669 6e64 735d 2c20 6269 6e73 3d70  infinds], bins=p
+0000aa10: 656f 706c 652e 6167 655f 6269 6e5f 6564  eople.age_bin_ed
+0000aa20: 6765 732c 2077 6569 6768 7473 3d70 656f  ges, weights=peo
+0000aa30: 706c 652e 7363 616c 655b 665f 696e 6669  ple.scale[f_infi
+0000aa40: 6e64 735d 295b 305d 0a20 2020 2020 2020  nds])[0].       
+0000aa50: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+0000aa60: 735b 6627 6e5f 696e 6665 6374 696f 7573  s[f'n_infectious
+0000aa70: 5f62 795f 6167 6527 5d5b 3a2c 2069 6478  _by_age'][:, idx
+0000aa80: 5d20 3d20 6e70 2e68 6973 746f 6772 616d  ] = np.histogram
+0000aa90: 2870 656f 706c 652e 6167 655b 696e 6669  (people.age[infi
+0000aaa0: 6e64 735d 2c20 6269 6e73 3d70 656f 706c  nds], bins=peopl
+0000aab0: 652e 6167 655f 6269 6e5f 6564 6765 732c  e.age_bin_edges,
+0000aac0: 2077 6569 6768 7473 3d70 656f 706c 652e   weights=people.
+0000aad0: 7363 616c 655b 696e 6669 6e64 735d 295b  scale[infinds])[
+0000aae0: 305d 0a20 2020 2020 2020 2020 2020 2073  0].            s
+0000aaf0: 7573 696e 6473 203d 2068 7075 2e74 7275  usinds = hpu.tru
+0000ab00: 6528 7065 6f70 6c65 5b27 7375 7363 6570  e(people['suscep
+0000ab10: 7469 626c 6527 5d29 0a20 2020 2020 2020  tible']).       
+0000ab20: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+0000ab30: 735b 6627 6e5f 7375 7363 6570 7469 626c  s[f'n_susceptibl
+0000ab40: 655f 6279 5f61 6765 275d 5b3a 2c20 6964  e_by_age'][:, id
+0000ab50: 785d 203d 206e 702e 6869 7374 6f67 7261  x] = np.histogra
+0000ab60: 6d28 7065 6f70 6c65 2e61 6765 5b73 7573  m(people.age[sus
+0000ab70: 696e 6473 5d2c 2062 696e 733d 7065 6f70  inds], bins=peop
+0000ab80: 6c65 2e61 6765 5f62 696e 5f65 6467 6573  le.age_bin_edges
+0000ab90: 2c20 7765 6967 6874 733d 7065 6f70 6c65  , weights=people
+0000aba0: 2e73 6361 6c65 5b73 7573 696e 6473 5d29  .scale[susinds])
+0000abb0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0000abc0: 7472 616e 7366 6f72 6d65 6469 6e64 7320  transformedinds 
+0000abd0: 3d20 6870 752e 7472 7565 2870 656f 706c  = hpu.true(peopl
+0000abe0: 655b 2774 7261 6e73 666f 726d 6564 275d  e['transformed']
+0000abf0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000ac00: 6c66 2e72 6573 756c 7473 5b66 276e 5f74  lf.results[f'n_t
+0000ac10: 7261 6e73 666f 726d 6564 5f62 795f 6167  ransformed_by_ag
+0000ac20: 6527 5d5b 3a2c 2069 6478 5d20 3d20 6e70  e'][:, idx] = np
+0000ac30: 2e68 6973 746f 6772 616d 2870 656f 706c  .histogram(peopl
+0000ac40: 652e 6167 655b 7472 616e 7366 6f72 6d65  e.age[transforme
+0000ac50: 6469 6e64 735d 2c20 6269 6e73 3d70 656f  dinds], bins=peo
+0000ac60: 706c 652e 6167 655f 6269 6e5f 6564 6765  ple.age_bin_edge
+0000ac70: 732c 2077 6569 6768 7473 3d70 656f 706c  s, weights=peopl
+0000ac80: 652e 7363 616c 655b 7472 616e 7366 6f72  e.scale[transfor
+0000ac90: 6d65 6469 6e64 735d 295b 305d 0a20 2020  medinds])[0].   
+0000aca0: 2020 2020 2020 2020 2070 7265 6369 6e69           precini
+0000acb0: 6e64 7320 3d20 6870 752e 7472 7565 2870  nds = hpu.true(p
+0000acc0: 656f 706c 655b 2770 7265 6369 6e27 5d29  eople['precin'])
+0000acd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ace0: 662e 7265 7375 6c74 735b 6627 6e5f 7072  f.results[f'n_pr
+0000acf0: 6563 696e 5f62 795f 6167 6527 5d5b 3a2c  ecin_by_age'][:,
+0000ad00: 2069 6478 5d20 3d20 6e70 2e68 6973 746f   idx] = np.histo
+0000ad10: 6772 616d 2870 656f 706c 652e 6167 655b  gram(people.age[
+0000ad20: 7072 6563 696e 696e 6473 5d2c 2062 696e  precininds], bin
+0000ad30: 733d 7065 6f70 6c65 2e61 6765 5f62 696e  s=people.age_bin
+0000ad40: 5f65 6467 6573 2c20 7765 6967 6874 733d  _edges, weights=
+0000ad50: 7065 6f70 6c65 2e73 6361 6c65 5b70 7265  people.scale[pre
+0000ad60: 6369 6e69 6e64 735d 295b 305d 0a20 2020  cininds])[0].   
+0000ad70: 2020 2020 2020 2020 2063 696e 3169 6e64           cin1ind
+0000ad80: 7320 3d20 6870 752e 7472 7565 2870 656f  s = hpu.true(peo
+0000ad90: 706c 655b 2763 696e 3127 5d29 0a20 2020  ple['cin1']).   
+0000ada0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0000adb0: 7375 6c74 735b 6627 6e5f 6369 6e31 5f62  sults[f'n_cin1_b
+0000adc0: 795f 6167 6527 5d5b 3a2c 2069 6478 5d20  y_age'][:, idx] 
+0000add0: 3d20 6e70 2e68 6973 746f 6772 616d 2870  = np.histogram(p
+0000ade0: 656f 706c 652e 6167 655b 6369 6e31 696e  eople.age[cin1in
+0000adf0: 6473 5d2c 2062 696e 733d 7065 6f70 6c65  ds], bins=people
+0000ae00: 2e61 6765 5f62 696e 5f65 6467 6573 2c20  .age_bin_edges, 
+0000ae10: 7765 6967 6874 733d 7065 6f70 6c65 2e73  weights=people.s
+0000ae20: 6361 6c65 5b63 696e 3169 6e64 735d 295b  cale[cin1inds])[
+0000ae30: 305d 0a20 2020 2020 2020 2020 2020 2063  0].            c
+0000ae40: 696e 3269 6e64 7320 3d20 6870 752e 7472  in2inds = hpu.tr
+0000ae50: 7565 2870 656f 706c 655b 2763 696e 3227  ue(people['cin2'
+0000ae60: 5d29 0a20 2020 2020 2020 2020 2020 2073  ]).            s
+0000ae70: 656c 662e 7265 7375 6c74 735b 6627 6e5f  elf.results[f'n_
+0000ae80: 6369 6e32 5f62 795f 6167 6527 5d5b 3a2c  cin2_by_age'][:,
+0000ae90: 2069 6478 5d20 3d20 6e70 2e68 6973 746f   idx] = np.histo
+0000aea0: 6772 616d 2870 656f 706c 652e 6167 655b  gram(people.age[
+0000aeb0: 6369 6e32 696e 6473 5d2c 2062 696e 733d  cin2inds], bins=
+0000aec0: 7065 6f70 6c65 2e61 6765 5f62 696e 5f65  people.age_bin_e
+0000aed0: 6467 6573 2c20 7765 6967 6874 733d 7065  dges, weights=pe
+0000aee0: 6f70 6c65 2e73 6361 6c65 5b63 696e 3269  ople.scale[cin2i
+0000aef0: 6e64 735d 295b 305d 0a20 2020 2020 2020  nds])[0].       
+0000af00: 2020 2020 2063 696e 3369 6e64 7320 3d20       cin3inds = 
+0000af10: 6870 752e 7472 7565 2870 656f 706c 655b  hpu.true(people[
+0000af20: 2763 696e 3327 5d29 0a20 2020 2020 2020  'cin3']).       
+0000af30: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+0000af40: 735b 6627 6e5f 6369 6e33 5f62 795f 6167  s[f'n_cin3_by_ag
+0000af50: 6527 5d5b 3a2c 2069 6478 5d20 3d20 6e70  e'][:, idx] = np
+0000af60: 2e68 6973 746f 6772 616d 2870 656f 706c  .histogram(peopl
+0000af70: 652e 6167 655b 6369 6e33 696e 6473 5d2c  e.age[cin3inds],
+0000af80: 2062 696e 733d 7065 6f70 6c65 2e61 6765   bins=people.age
+0000af90: 5f62 696e 5f65 6467 6573 2c20 7765 6967  _bin_edges, weig
+0000afa0: 6874 733d 7065 6f70 6c65 2e73 6361 6c65  hts=people.scale
+0000afb0: 5b63 696e 3369 6e64 735d 295b 305d 0a0a  [cin3inds])[0]..
+0000afc0: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+0000afd0: 6561 7465 2074 6f74 616c 2073 746f 636b  eate total stock
+0000afe0: 730a 2020 2020 2020 2020 2020 2020 666f  s.            fo
+0000aff0: 7220 6b65 7920 696e 2073 656c 662e 7065  r key in self.pe
+0000b000: 6f70 6c65 2e6d 6574 612e 6765 6e6f 7479  ople.meta.genoty
+0000b010: 7065 5f73 746f 636b 5f6b 6579 733a 0a0a  pe_stock_keys:..
+0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b030: 2320 5374 6f63 6b73 2062 7920 6765 6e6f  # Stocks by geno
+0000b040: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
+0000b050: 2020 2020 2066 6f72 2067 2069 6e20 7261       for g in ra
+0000b060: 6e67 6528 6e67 293a 0a20 2020 2020 2020  nge(ng):.       
+0000b070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b080: 662e 7265 7375 6c74 735b 6627 6e5f 7b6b  f.results[f'n_{k
+0000b090: 6579 7d5f 6279 5f67 656e 6f74 7970 6527  ey}_by_genotype'
+0000b0a0: 5d5b 672c 2069 6478 5d20 3d20 7065 6f70  ][g, idx] = peop
+0000b0b0: 6c65 2e63 6f75 6e74 5f62 795f 6765 6e6f  le.count_by_geno
+0000b0c0: 7479 7065 286b 6579 2c20 6729 0a0a 2020  type(key, g)..  
+0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000b0e0: 546f 7461 6c20 7374 6f63 6b73 0a20 2020  Total stocks.   
+0000b0f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000b100: 6b65 7920 6e6f 7420 696e 205b 2773 7573  key not in ['sus
+0000b110: 6365 7074 6962 6c65 275d 3a0a 2020 2020  ceptible']:.    
+0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b130: 2320 466f 7220 6e5f 696e 6665 6374 696f  # For n_infectio
+0000b140: 7573 2065 7463 2c20 7765 2067 6574 2074  us etc, we get t
+0000b150: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
+0000b160: 7768 6572 6520 7468 6973 2073 7461 7465  where this state
+0000b170: 2069 7320 7472 7565 2066 6f72 2061 7420   is true for at 
+0000b180: 6c65 6173 7420 6f6e 6520 6765 6e6f 7479  least one genoty
+0000b190: 7065 0a20 2020 2020 2020 2020 2020 2020  pe.             
+0000b1a0: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
+0000b1b0: 6c74 735b 6627 6e5f 7b6b 6579 7d27 5d5b  lts[f'n_{key}'][
+0000b1c0: 6964 785d 203d 2070 656f 706c 652e 636f  idx] = people.co
+0000b1d0: 756e 745f 616e 7928 6b65 7929 0a20 2020  unt_any(key).   
+0000b1e0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000b1f0: 6620 6b65 7920 3d3d 2027 7375 7363 6570  f key == 'suscep
+0000b200: 7469 626c 6527 3a0a 2020 2020 2020 2020  tible':.        
+0000b210: 2020 2020 2020 2020 2020 2020 2320 466f              # Fo
+0000b220: 7220 6e5f 746f 7461 6c5f 7375 7363 6570  r n_total_suscep
+0000b230: 7469 626c 652c 2077 6520 6765 7420 7468  tible, we get th
+0000b240: 6520 746f 7461 6c20 6e75 6d62 6572 206f  e total number o
+0000b250: 6620 696e 6665 6374 696f 6e73 2074 6861  f infections tha
+0000b260: 7420 636f 756c 6420 7468 656f 7265 7469  t could theoreti
+0000b270: 6361 6c6c 7920 6861 7070 656e 2069 6e20  cally happen in 
+0000b280: 7468 6520 706f 7075 6c61 7469 6f6e 2c20  the population, 
+0000b290: 7768 6963 6820 6361 6e20 6265 2067 7265  which can be gre
+0000b2a0: 6174 6572 2074 6861 6e20 7468 6520 706f  ater than the po
+0000b2b0: 7075 6c61 7469 6f6e 2073 697a 650a 2020  pulation size.  
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 7365 6c66 2e72 6573 756c 7473 5b66    self.results[f
+0000b2e0: 276e 5f7b 6b65 797d 275d 5b69 6478 5d20  'n_{key}'][idx] 
+0000b2f0: 3d20 7065 6f70 6c65 2e63 6f75 6e74 286b  = people.count(k
+0000b300: 6579 290a 0a20 2020 2020 2020 2020 2020  ey)..           
+0000b310: 2023 2043 7265 6174 6520 7374 6f63 6b73   # Create stocks
+0000b320: 206f 6620 696e 7465 7276 656e 7469 6f6e   of intervention
+0000b330: 730a 2020 2020 2020 2020 2020 2020 666f  s.            fo
+0000b340: 7220 6b65 7920 696e 2073 656c 662e 7065  r key in self.pe
+0000b350: 6f70 6c65 2e6d 6574 612e 696e 7476 5f73  ople.meta.intv_s
+0000b360: 746f 636b 5f6b 6579 733a 0a20 2020 2020  tock_keys:.     
+0000b370: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b380: 7265 7375 6c74 735b 6627 6e5f 7b6b 6579  results[f'n_{key
+0000b390: 7d27 5d5b 6964 785d 203d 2070 656f 706c  }'][idx] = peopl
+0000b3a0: 652e 636f 756e 7428 6b65 7929 0a0a 2020  e.count(key)..  
+0000b3b0: 2020 2020 2020 2020 2020 2320 5570 6461            # Upda
+0000b3c0: 7465 2063 616e 6365 7273 2061 6e64 2063  te cancers and c
+0000b3d0: 616e 6365 7273 2062 7920 6167 650a 2020  ancers by age.  
+0000b3e0: 2020 2020 2020 2020 2020 6361 7365 735f            cases_
+0000b3f0: 6279 5f61 6765 203d 2073 656c 662e 7265  by_age = self.re
+0000b400: 7375 6c74 735b 2763 616e 6365 7273 5f62  sults['cancers_b
+0000b410: 795f 6167 6527 5d5b 3a2c 2069 6478 5d0a  y_age'][:, idx].
+0000b420: 2020 2020 2020 2020 2020 2020 696e 6473              inds
+0000b430: 203d 2070 656f 706c 652e 616c 6976 6520   = people.alive 
+0000b440: 2a20 2873 656c 662e 7065 6f70 6c65 2e73  * (self.people.s
+0000b450: 6578 3d3d 3029 202a 207e 7065 6f70 6c65  ex==0) * ~people
+0000b460: 2e63 616e 6365 726f 7573 2e61 6e79 2861  .cancerous.any(a
+0000b470: 7869 733d 3029 0a20 2020 2020 2020 2020  xis=0).         
+0000b480: 2020 2076 616c 7320 3d20 7365 6c66 2e70     vals = self.p
+0000b490: 656f 706c 652e 6167 655b 696e 6473 5d0a  eople.age[inds].
+0000b4a0: 2020 2020 2020 2020 2020 2020 6269 6e73              bins
+0000b4b0: 203d 2073 656c 662e 7061 7273 5b27 7374   = self.pars['st
+0000b4c0: 616e 6461 7264 5f70 6f70 275d 5b30 2c5d  andard_pop'][0,]
+0000b4d0: 0a20 2020 2020 2020 2020 2020 2077 6569  .            wei
+0000b4e0: 6768 7473 203d 2070 656f 706c 652e 7363  ghts = people.sc
+0000b4f0: 616c 655b 696e 6473 5d0a 2020 2020 2020  ale[inds].      
+0000b500: 2020 2020 2020 6465 6e6f 6d20 3d20 6e70        denom = np
+0000b510: 2e68 6973 746f 6772 616d 2876 616c 732c  .histogram(vals,
+0000b520: 2062 696e 732c 2077 6569 6768 7473 3d77   bins, weights=w
+0000b530: 6569 6768 7473 295b 305d 0a20 2020 2020  eights)[0].     
+0000b540: 2020 2020 2020 2061 6765 5f73 7065 6369         age_speci
+0000b550: 6669 635f 696e 6369 6465 6e63 6520 3d20  fic_incidence = 
+0000b560: 7363 2e73 6166 6564 6976 6964 6528 6361  sc.safedivide(ca
+0000b570: 7365 735f 6279 5f61 6765 2c20 6465 6e6f  ses_by_age, deno
+0000b580: 6d29 2a31 3030 6533 0a20 2020 2020 2020  m)*100e3.       
+0000b590: 2020 2020 2073 7461 6e64 6172 645f 706f       standard_po
+0000b5a0: 7020 3d20 7365 6c66 2e70 6172 735b 2773  p = self.pars['s
+0000b5b0: 7461 6e64 6172 645f 706f 7027 5d5b 312c  tandard_pop'][1,
+0000b5c0: 203a 2d31 5d0a 2020 2020 2020 2020 2020   :-1].          
+0000b5d0: 2020 7365 6c66 2e72 6573 756c 7473 5b27    self.results['
+0000b5e0: 6173 725f 6361 6e63 6572 5f69 6e63 6964  asr_cancer_incid
+0000b5f0: 656e 6365 275d 5b69 6478 5d20 3d20 6e70  ence'][idx] = np
+0000b600: 2e64 6f74 2861 6765 5f73 7065 6369 6669  .dot(age_specifi
+0000b610: 635f 696e 6369 6465 6e63 652c 7374 616e  c_incidence,stan
+0000b620: 6461 7264 5f70 6f70 290a 0a20 2020 2020  dard_pop)..     
+0000b630: 2020 2020 2020 2023 2053 6176 6520 6e75         # Save nu
+0000b640: 6d62 6572 2061 6c69 7665 0a20 2020 2020  mber alive.     
+0000b650: 2020 2020 2020 2061 6c69 7665 5f69 6e64         alive_ind
+0000b660: 7320 3d20 6870 752e 7472 7565 2870 656f  s = hpu.true(peo
+0000b670: 706c 652e 616c 6976 6529 0a20 2020 2020  ple.alive).     
+0000b680: 2020 2020 2020 2061 6c69 7665 5f66 656d         alive_fem
+0000b690: 616c 655f 696e 6473 203d 2068 7075 2e74  ale_inds = hpu.t
+0000b6a0: 7275 6528 7065 6f70 6c65 2e61 6c69 7665  rue(people.alive
+0000b6b0: 2a70 656f 706c 652e 6973 5f66 656d 616c  *people.is_femal
+0000b6c0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+0000b6d0: 656c 662e 7265 7375 6c74 735b 276e 5f61  elf.results['n_a
+0000b6e0: 6c69 7665 275d 5b69 6478 5d20 3d20 7065  live'][idx] = pe
+0000b6f0: 6f70 6c65 2e73 6361 6c65 5f66 6c6f 7773  ople.scale_flows
+0000b700: 2861 6c69 7665 5f69 6e64 7329 0a20 2020  (alive_inds).   
+0000b710: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0000b720: 7375 6c74 735b 276e 5f61 6c69 7665 5f62  sults['n_alive_b
+0000b730: 795f 7365 7827 5d5b 302c 6964 785d 203d  y_sex'][0,idx] =
+0000b740: 2070 656f 706c 652e 7363 616c 655f 666c   people.scale_fl
+0000b750: 6f77 7328 2870 656f 706c 652e 616c 6976  ows((people.aliv
+0000b760: 652a 7065 6f70 6c65 2e69 735f 6665 6d61  e*people.is_fema
+0000b770: 6c65 292e 6e6f 6e7a 6572 6f28 295b 305d  le).nonzero()[0]
+0000b780: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000b790: 6c66 2e72 6573 756c 7473 5b27 6e5f 616c  lf.results['n_al
+0000b7a0: 6976 655f 6279 5f73 6578 275d 5b31 2c69  ive_by_sex'][1,i
+0000b7b0: 6478 5d20 3d20 7065 6f70 6c65 2e73 6361  dx] = people.sca
+0000b7c0: 6c65 5f66 6c6f 7773 2828 7065 6f70 6c65  le_flows((people
+0000b7d0: 2e61 6c69 7665 2a70 656f 706c 652e 6973  .alive*people.is
+0000b7e0: 5f6d 616c 6529 2e6e 6f6e 7a65 726f 2829  _male).nonzero()
+0000b7f0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0000b800: 2073 656c 662e 7265 7375 6c74 735b 276e   self.results['n
+0000b810: 5f61 6c69 7665 5f62 795f 6167 6527 5d5b  _alive_by_age'][
+0000b820: 3a2c 6964 785d 203d 206e 702e 6869 7374  :,idx] = np.hist
+0000b830: 6f67 7261 6d28 7065 6f70 6c65 2e61 6765  ogram(people.age
+0000b840: 5b61 6c69 7665 5f69 6e64 735d 2c20 6269  [alive_inds], bi
+0000b850: 6e73 3d70 656f 706c 652e 6167 655f 6269  ns=people.age_bi
+0000b860: 6e5f 6564 6765 732c 2077 6569 6768 7473  n_edges, weights
+0000b870: 3d70 656f 706c 652e 7363 616c 655b 616c  =people.scale[al
+0000b880: 6976 655f 696e 6473 5d29 5b30 5d0a 2020  ive_inds])[0].  
+0000b890: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000b8a0: 6573 756c 7473 5b27 6e5f 6665 6d61 6c65  esults['n_female
+0000b8b0: 735f 616c 6976 655f 6279 5f61 6765 275d  s_alive_by_age']
+0000b8c0: 5b3a 2c69 6478 5d20 3d20 6e70 2e68 6973  [:,idx] = np.his
+0000b8d0: 746f 6772 616d 2870 656f 706c 652e 6167  togram(people.ag
+0000b8e0: 655b 616c 6976 655f 6665 6d61 6c65 5f69  e[alive_female_i
+0000b8f0: 6e64 735d 2c20 6269 6e73 3d70 656f 706c  nds], bins=peopl
+0000b900: 652e 6167 655f 6269 6e5f 6564 6765 732c  e.age_bin_edges,
+0000b910: 2077 6569 6768 7473 3d70 656f 706c 652e   weights=people.
+0000b920: 7363 616c 655b 616c 6976 655f 6665 6d61  scale[alive_fema
+0000b930: 6c65 5f69 6e64 735d 295b 305d 0a0a 2020  le_inds])[0]..  
+0000b940: 2020 2020 2020 2320 4170 706c 7920 616e        # Apply an
+0000b950: 616c 797a 6572 730a 2020 2020 2020 2020  alyzers.        
+0000b960: 666f 7220 692c 616e 616c 797a 6572 2069  for i,analyzer i
+0000b970: 6e20 656e 756d 6572 6174 6528 7365 6c66  n enumerate(self
+0000b980: 2e61 6e61 6c79 7a65 7273 293a 0a20 2020  .analyzers):.   
+0000b990: 2020 2020 2020 2020 2061 6e61 6c79 7a65           analyze
+0000b9a0: 7228 7365 6c66 290a 0a20 2020 2020 2020  r(self)..       
+0000b9b0: 2023 2054 6964 7920 7570 0a20 2020 2020   # Tidy up.     
+0000b9c0: 2020 2073 656c 662e 7420 2b3d 2031 0a20     self.t += 1. 
+0000b9d0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+0000b9e0: 203d 3d20 7365 6c66 2e6e 7074 733a 0a20   == self.npts:. 
+0000b9f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ba00: 636f 6d70 6c65 7465 203d 2054 7275 650a  complete = True.
+0000ba10: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
+0000ba20: 0a0a 2020 2020 6465 6620 7275 6e28 7365  ..    def run(se
+0000ba30: 6c66 2c20 646f 5f70 6c6f 743d 4661 6c73  lf, do_plot=Fals
+0000ba40: 652c 2075 6e74 696c 3d4e 6f6e 652c 2072  e, until=None, r
+0000ba50: 6573 746f 7265 5f70 6172 733d 5472 7565  estore_pars=True
+0000ba60: 2c20 7265 7365 745f 7365 6564 3d54 7275  , reset_seed=Tru
+0000ba70: 652c 2076 6572 626f 7365 3d4e 6f6e 6529  e, verbose=None)
+0000ba80: 3a0a 2020 2020 2020 2020 2727 2720 5275  :.        ''' Ru
+0000ba90: 6e20 7468 6520 6d6f 6465 6c20 6f6e 6365  n the model once
+0000baa0: 2027 2727 0a20 2020 2020 2020 2023 2049   '''.        # I
+0000bab0: 6e69 7469 616c 697a 6174 696f 6e20 7374  nitialization st
+0000bac0: 6570 7320 2d2d 2073 7461 7274 2074 6865  eps -- start the
+0000bad0: 2074 696d 6572 2c20 696e 6974 6961 6c69   timer, initiali
+0000bae0: 7a65 2074 6865 2073 696d 2061 6e64 2074  ze the sim and t
+0000baf0: 6865 2073 6565 642c 2061 6e64 2063 6865  he seed, and che
+0000bb00: 636b 2074 6861 7420 7468 6520 7369 6d20  ck that the sim 
+0000bb10: 6861 736e 2774 2062 6565 6e20 7275 6e0a  hasn't been run.
+0000bb20: 2020 2020 2020 2020 5420 3d20 7363 2e74          T = sc.t
+0000bb30: 696d 6572 2829 0a0a 2020 2020 2020 2020  imer()..        
+0000bb40: 6966 206e 6f74 2073 656c 662e 696e 6974  if not self.init
+0000bb50: 6961 6c69 7a65 643a 0a20 2020 2020 2020  ialized:.       
+0000bb60: 2020 2020 2073 656c 662e 696e 6974 6961       self.initia
+0000bb70: 6c69 7a65 2829 0a20 2020 2020 2020 2020  lize().         
+0000bb80: 2020 2073 656c 662e 5f6f 7269 675f 7061     self._orig_pa
+0000bb90: 7273 203d 2073 632e 6463 7028 7365 6c66  rs = sc.dcp(self
+0000bba0: 2e70 6172 7329 2023 2043 7265 6174 6520  .pars) # Create 
+0000bbb0: 6120 636f 7079 206f 6620 7468 6520 7061  a copy of the pa
+0000bbc0: 7261 6d65 7465 7273 2c20 746f 2072 6573  rameters, to res
+0000bbd0: 746f 7265 2061 6674 6572 2074 6865 2072  tore after the r
+0000bbe0: 756e 2c20 696e 2063 6173 6520 7468 6579  un, in case they
+0000bbf0: 2061 7265 2064 796e 616d 6963 616c 6c79   are dynamically
+0000bc00: 206d 6f64 6966 6965 640a 0a20 2020 2020   modified..     
+0000bc10: 2020 2069 6620 7665 7262 6f73 6520 6973     if verbose is
+0000bc20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000bc30: 2020 2076 6572 626f 7365 203d 2073 656c     verbose = sel
+0000bc40: 665b 2776 6572 626f 7365 275d 0a0a 2020  f['verbose']..  
+0000bc50: 2020 2020 2020 6966 2072 6573 6574 5f73        if reset_s
+0000bc60: 6565 643a 0a20 2020 2020 2020 2020 2020  eed:.           
+0000bc70: 2023 2052 6573 6574 2074 6865 2052 4e47   # Reset the RNG
+0000bc80: 2e20 5468 6520 7072 696d 6172 7920 7573  . The primary us
+0000bc90: 6520 6361 7365 2028 616e 6420 7768 7920  e case (and why 
+0000bca0: 6974 2064 6566 6175 6c74 7320 746f 2054  it defaults to T
+0000bcb0: 7275 6529 2069 7320 746f 2065 6e73 7572  rue) is to ensur
+0000bcc0: 6520 7468 6174 0a20 2020 2020 2020 2020  e that.         
+0000bcd0: 2020 2023 0a20 2020 2020 2020 2020 2020     #.           
+0000bce0: 2023 203e 3e3e 2073 696d 302e 696e 6974   # >>> sim0.init
+0000bcf0: 6961 6c69 7a65 2829 0a20 2020 2020 2020  ialize().       
+0000bd00: 2020 2020 2023 203e 3e3e 2073 696d 302e       # >>> sim0.
+0000bd10: 7275 6e28 290a 2020 2020 2020 2020 2020  run().          
+0000bd20: 2020 2320 3e3e 3e20 7369 6d31 2e69 6e69    # >>> sim1.ini
+0000bd30: 7469 616c 697a 6528 290a 2020 2020 2020  tialize().      
+0000bd40: 2020 2020 2020 2320 3e3e 3e20 7369 6d31        # >>> sim1
+0000bd50: 2e72 756e 2829 0a20 2020 2020 2020 2020  .run().         
+0000bd60: 2020 2023 0a20 2020 2020 2020 2020 2020     #.           
+0000bd70: 2023 2070 726f 6475 6365 7320 7468 6520   # produces the 
+0000bd80: 7361 6d65 206f 7574 7075 7420 6173 0a20  same output as. 
+0000bd90: 2020 2020 2020 2020 2020 2023 0a20 2020             #.   
+0000bda0: 2020 2020 2020 2020 2023 203e 3e3e 2073           # >>> s
+0000bdb0: 696d 302e 696e 6974 6961 6c69 7a65 2829  im0.initialize()
+0000bdc0: 0a20 2020 2020 2020 2020 2020 2023 203e  .            # >
+0000bdd0: 3e3e 2073 696d 312e 696e 6974 6961 6c69  >> sim1.initiali
+0000bde0: 7a65 2829 0a20 2020 2020 2020 2020 2020  ze().           
+0000bdf0: 2023 203e 3e3e 2073 696d 302e 7275 6e28   # >>> sim0.run(
+0000be00: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+0000be10: 3e3e 3e20 7369 6d31 2e72 756e 2829 0a20  >>> sim1.run(). 
+0000be20: 2020 2020 2020 2020 2020 2023 0a20 2020             #.   
+0000be30: 2020 2020 2020 2020 2023 2054 6865 2073           # The s
+0000be40: 6565 6420 6973 206f 6666 7365 7420 6279  eed is offset by
+0000be50: 2031 2074 6f20 6176 6f69 6420 6472 6177   1 to avoid draw
+0000be60: 696e 6720 7468 6520 7361 6d65 2072 616e  ing the same ran
+0000be70: 646f 6d20 6e75 6d62 6572 7320 6173 2074  dom numbers as t
+0000be80: 686f 7365 2075 7365 6420 666f 7220 706f  hose used for po
+0000be90: 7075 6c61 7469 6f6e 2067 656e 6572 6174  pulation generat
+0000bea0: 696f 6e2c 206f 7468 6572 7769 7365 0a20  ion, otherwise. 
+0000beb0: 2020 2020 2020 2020 2020 2023 2074 6865             # the
+0000bec0: 2066 6972 7374 2073 6574 206f 6620 7261   first set of ra
+0000bed0: 6e64 6f6d 206e 756d 6265 7273 2069 6e20  ndom numbers in 
+0000bee0: 7468 6520 6d6f 6465 6c20 2865 2e67 2e2c  the model (e.g.,
+0000bef0: 2064 6561 7468 7329 2077 696c 6c20 6265   deaths) will be
+0000bf00: 2063 6f72 7265 6c61 7465 6420 7769 7468   correlated with
+0000bf10: 2074 6865 2066 6972 7374 2073 6574 206f   the first set o
+0000bf20: 6620 7261 6e64 6f6d 206e 756d 6265 7273  f random numbers
+0000bf30: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
+0000bf40: 7261 776e 2069 6e20 706f 7075 6c61 7469  rawn in populati
+0000bf50: 6f6e 2067 656e 6572 6174 696f 6e20 2865  on generation (e
+0000bf60: 2e67 2e2c 2073 6578 290a 2020 2020 2020  .g., sex).      
+0000bf70: 2020 2020 2020 6870 752e 7365 745f 7365        hpu.set_se
+0000bf80: 6564 2873 656c 665b 2772 616e 645f 7365  ed(self['rand_se
+0000bf90: 6564 275d 2b31 290a 0a20 2020 2020 2020  ed']+1)..       
+0000bfa0: 2023 2043 6865 636b 2066 6f72 2041 6c72   # Check for Alr
+0000bfb0: 6561 6479 5275 6e20 6572 726f 7273 0a20  eadyRun errors. 
+0000bfc0: 2020 2020 2020 2065 7272 6f72 6d73 6720         errormsg 
+0000bfd0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2075  = None.        u
+0000bfe0: 6e74 696c 203d 2073 656c 662e 6e70 7473  ntil = self.npts
+0000bff0: 2069 6620 756e 7469 6c20 6973 204e 6f6e   if until is Non
+0000c000: 6520 656c 7365 2073 656c 662e 6765 745f  e else self.get_
+0000c010: 7428 756e 7469 6c29 0a20 2020 2020 2020  t(until).       
+0000c020: 2069 6620 756e 7469 6c20 3e20 7365 6c66   if until > self
+0000c030: 2e6e 7074 733a 0a20 2020 2020 2020 2020  .npts:.         
+0000c040: 2020 2065 7272 6f72 6d73 6720 3d20 6627     errormsg = f'
+0000c050: 5265 7175 6573 7465 6420 746f 2072 756e  Requested to run
+0000c060: 2075 6e74 696c 2074 3d7b 756e 7469 6c7d   until t={until}
+0000c070: 2062 7574 2074 6865 2073 696d 756c 6174   but the simulat
+0000c080: 696f 6e20 656e 6420 6973 2074 3d7b 7365  ion end is t={se
+0000c090: 6c66 2e6e 7074 737d 270a 2020 2020 2020  lf.npts}'.      
+0000c0a0: 2020 6966 2073 656c 662e 7420 3e3d 2075    if self.t >= u
+0000c0b0: 6e74 696c 3a20 2320 4e42 2e20 4174 2074  ntil: # NB. At t
+0000c0c0: 6865 2073 7461 7274 2c20 7365 6c66 2e74  he start, self.t
+0000c0d0: 2069 7320 4e6f 6e65 2073 6f20 7468 6973   is None so this
+0000c0e0: 2063 6865 636b 206d 7573 7420 6f63 6375   check must occu
+0000c0f0: 7220 6166 7465 7220 696e 6974 6961 6c69  r after initiali
+0000c100: 7a61 7469 6f6e 0a20 2020 2020 2020 2020  zation.         
+0000c110: 2020 2065 7272 6f72 6d73 6720 3d20 6627     errormsg = f'
+0000c120: 5369 6d75 6c61 7469 6f6e 2069 7320 6375  Simulation is cu
+0000c130: 7272 656e 746c 7920 6174 2074 3d7b 7365  rrently at t={se
+0000c140: 6c66 2e74 7d2c 2072 6571 7565 7374 6564  lf.t}, requested
+0000c150: 2074 6f20 7275 6e20 756e 7469 6c20 743d   to run until t=
+0000c160: 7b75 6e74 696c 7d20 7768 6963 6820 6861  {until} which ha
+0000c170: 7320 616c 7265 6164 7920 6265 656e 2072  s already been r
+0000c180: 6561 6368 6564 270a 2020 2020 2020 2020  eached'.        
+0000c190: 6966 2073 656c 662e 636f 6d70 6c65 7465  if self.complete
+0000c1a0: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
+0000c1b0: 726f 726d 7367 203d 2027 5369 6d75 6c61  rormsg = 'Simula
+0000c1c0: 7469 6f6e 2069 7320 616c 7265 6164 7920  tion is already 
+0000c1d0: 636f 6d70 6c65 7465 2028 6361 6c6c 2073  complete (call s
+0000c1e0: 696d 2e69 6e69 7469 616c 697a 6528 2920  im.initialize() 
+0000c1f0: 746f 2072 652d 7275 6e29 270a 2020 2020  to re-run)'.    
+0000c200: 2020 2020 6966 2073 656c 662e 7065 6f70      if self.peop
+0000c210: 6c65 2e74 206e 6f74 2069 6e20 5b73 656c  le.t not in [sel
+0000c220: 662e 742c 2073 656c 662e 742d 315d 3a20  f.t, self.t-1]: 
+0000c230: 2320 4465 7065 6e64 696e 6720 6f6e 2068  # Depending on h
+0000c240: 6f77 2074 6865 2073 696d 2073 746f 7070  ow the sim stopp
+0000c250: 6564 2c20 6569 7468 6572 206f 6620 7468  ed, either of th
+0000c260: 6573 6520 7374 6174 6573 2061 7265 2070  ese states are p
+0000c270: 6f73 7369 626c 650a 2020 2020 2020 2020  ossible.        
+0000c280: 2020 2020 6572 726f 726d 7367 203d 2066      errormsg = f
+0000c290: 2754 6865 2073 696d 756c 6174 696f 6e20  'The simulation 
+0000c2a0: 6861 7320 6265 656e 2072 756e 2069 6e64  has been run ind
+0000c2b0: 6570 656e 6465 6e74 6c79 2066 726f 6d20  ependently from 
+0000c2c0: 7468 6520 7065 6f70 6c65 2028 743d 7b73  the people (t={s
+0000c2d0: 656c 662e 747d 2c20 7065 6f70 6c65 2e74  elf.t}, people.t
+0000c2e0: 3d7b 7365 6c66 2e70 656f 706c 652e 747d  ={self.people.t}
+0000c2f0: 293a 2069 6620 7468 6973 2069 7320 696e  ): if this is in
+0000c300: 7465 6e74 696f 6e61 6c2c 206d 616e 7561  tentional, manua
+0000c310: 6c6c 7920 7365 7420 7369 6d2e 7065 6f70  lly set sim.peop
+0000c320: 6c65 2e74 203d 2073 696d 2e74 2e20 5265  le.t = sim.t. Re
+0000c330: 6d65 6d62 6572 2074 6f20 7361 7665 2074  member to save t
+0000c340: 6865 2070 656f 706c 6520 6f62 6a65 6374  he people object
+0000c350: 2062 6566 6f72 6520 7275 6e6e 696e 6720   before running 
+0000c360: 7468 6520 7369 6d2e 270a 2020 2020 2020  the sim.'.      
+0000c370: 2020 6966 2065 7272 6f72 6d73 673a 0a20    if errormsg:. 
+0000c380: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000c390: 2041 6c72 6561 6479 5275 6e45 7272 6f72   AlreadyRunError
+0000c3a0: 2865 7272 6f72 6d73 6729 0a0a 2020 2020  (errormsg)..    
+0000c3b0: 2020 2020 2320 4d61 696e 2073 696d 756c      # Main simul
+0000c3c0: 6174 696f 6e20 6c6f 6f70 0a20 2020 2020  ation loop.     
+0000c3d0: 2020 2077 6869 6c65 2073 656c 662e 7420     while self.t 
+0000c3e0: 3c20 756e 7469 6c3a 0a0a 2020 2020 2020  < until:..      
+0000c3f0: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
+0000c400: 2077 6520 7765 7265 2061 736b 6564 2074   we were asked t
+0000c410: 6f20 7374 6f70 0a20 2020 2020 2020 2020  o stop.         
+0000c420: 2020 2065 6c61 7073 6564 203d 2054 2e74     elapsed = T.t
+0000c430: 6f63 286f 7574 7075 743d 5472 7565 290a  oc(output=True).
+0000c440: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000c450: 656c 665b 2774 696d 656c 696d 6974 275d  elf['timelimit']
+0000c460: 2061 6e64 2065 6c61 7073 6564 203e 2073   and elapsed > s
+0000c470: 656c 665b 2774 696d 656c 696d 6974 275d  elf['timelimit']
+0000c480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c490: 2020 7363 2e70 7269 6e74 7628 6622 5469    sc.printv(f"Ti
+0000c4a0: 6d65 206c 696d 6974 2028 7b73 656c 665b  me limit ({self[
+0000c4b0: 2774 696d 656c 696d 6974 275d 7d20 7329  'timelimit']} s)
+0000c4c0: 2065 7863 6565 6465 643b 2063 616c 6c20   exceeded; call 
+0000c4d0: 7369 6d2e 6669 6e61 6c69 7a65 2829 2074  sim.finalize() t
+0000c4e0: 6f20 636f 6d70 7574 6520 7265 7375 6c74  o compute result
+0000c4f0: 7320 6966 2064 6573 6972 6564 222c 2031  s if desired", 1
+0000c500: 2c20 7665 7262 6f73 6529 0a20 2020 2020  , verbose).     
+0000c510: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c520: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
+0000c530: 6966 2073 656c 665b 2773 746f 7070 696e  if self['stoppin
+0000c540: 675f 6675 6e63 275d 2061 6e64 2073 656c  g_func'] and sel
+0000c550: 665b 2773 746f 7070 696e 675f 6675 6e63  f['stopping_func
+0000c560: 275d 2873 656c 6629 3a0a 2020 2020 2020  '](self):.      
+0000c570: 2020 2020 2020 2020 2020 7363 2e70 7269            sc.pri
+0000c580: 6e74 7628 2253 746f 7070 696e 6720 6675  ntv("Stopping fu
+0000c590: 6e63 7469 6f6e 2074 6572 6d69 6e61 7465  nction terminate
+0000c5a0: 6420 7468 6520 7369 6d75 6c61 7469 6f6e  d the simulation
+0000c5b0: 3b20 6361 6c6c 2073 696d 2e66 696e 616c  ; call sim.final
+0000c5c0: 697a 6528 2920 746f 2063 6f6d 7075 7465  ize() to compute
+0000c5d0: 2072 6573 756c 7473 2069 6620 6465 7369   results if desi
+0000c5e0: 7265 6422 2c20 312c 2076 6572 626f 7365  red", 1, verbose
+0000c5f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c600: 2020 7265 7475 726e 0a0a 2020 2020 2020    return..      
+0000c610: 2020 2020 2020 2320 5072 696e 7420 7072        # Print pr
+0000c620: 6f67 7265 7373 0a20 2020 2020 2020 2020  ogress.         
+0000c630: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0000c640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c650: 696d 6c61 6265 6c20 3d20 6627 227b 7365  imlabel = f'"{se
+0000c660: 6c66 2e6c 6162 656c 7d22 3a20 2720 6966  lf.label}": ' if
+0000c670: 2073 656c 662e 6c61 6265 6c20 656c 7365   self.label else
+0000c680: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
+0000c690: 2020 2020 7374 7269 6e67 203d 2066 2720      string = f' 
+0000c6a0: 2052 756e 6e69 6e67 207b 7369 6d6c 6162   Running {simlab
+0000c6b0: 656c 7d7b 7365 6c66 2e79 6561 7276 6563  el}{self.yearvec
+0000c6c0: 5b73 656c 662e 745d 3a30 2e31 667d 2028  [self.t]:0.1f} (
+0000c6d0: 7b73 656c 662e 743a 322e 3066 7d2f 7b73  {self.t:2.0f}/{s
+0000c6e0: 656c 662e 6e70 7473 7d29 2028 7b65 6c61  elf.npts}) ({ela
+0000c6f0: 7073 6564 3a30 2e32 667d 2073 2920 270a  psed:0.2f} s) '.
+0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c710: 6966 2076 6572 626f 7365 203e 3d20 323a  if verbose >= 2:
+0000c720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c730: 2020 2020 2073 632e 6865 6164 696e 6728       sc.heading(
+0000c740: 7374 7269 6e67 290a 2020 2020 2020 2020  string).        
+0000c750: 2020 2020 2020 2020 656c 6966 2076 6572          elif ver
+0000c760: 626f 7365 3e30 3a0a 2020 2020 2020 2020  bose>0:.        
+0000c770: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000c780: 6f74 2028 7365 6c66 2e74 2025 2069 6e74  ot (self.t % int
+0000c790: 2831 2e30 2f76 6572 626f 7365 2929 3a0a  (1.0/verbose)):.
+0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 2020 2020 2020 7363 2e70 726f 6772          sc.progr
+0000c7c0: 6573 7362 6172 2873 656c 662e 742b 312c  essbar(self.t+1,
+0000c7d0: 2073 656c 662e 6e70 7473 2c20 6c61 6265   self.npts, labe
+0000c7e0: 6c3d 7374 7269 6e67 2c20 6c65 6e67 7468  l=string, length
+0000c7f0: 3d32 302c 206e 6577 6c69 6e65 3d54 7275  =20, newline=Tru
+0000c800: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
+0000c810: 2320 446f 2074 6865 2068 6561 7679 206c  # Do the heavy l
+0000c820: 6966 7469 6e67 202d 2d20 6163 7475 616c  ifting -- actual
+0000c830: 6c79 2072 756e 2074 6865 206d 6f64 656c  ly run the model
+0000c840: 210a 2020 2020 2020 2020 2020 2020 7365  !.            se
+0000c850: 6c66 2e73 7465 7028 290a 0a20 2020 2020  lf.step()..     
+0000c860: 2020 2023 2049 6620 7369 6d75 6c61 7469     # If simulati
+0000c870: 6f6e 2072 6561 6368 6564 2074 6865 2065  on reached the e
+0000c880: 6e64 2c20 6669 6e61 6c69 7a65 2074 6865  nd, finalize the
+0000c890: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+0000c8a0: 2069 6620 7365 6c66 2e63 6f6d 706c 6574   if self.complet
+0000c8b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000c8c0: 656c 662e 6669 6e61 6c69 7a65 2876 6572  elf.finalize(ver
+0000c8d0: 626f 7365 3d76 6572 626f 7365 2c20 7265  bose=verbose, re
+0000c8e0: 7374 6f72 655f 7061 7273 3d72 6573 746f  store_pars=resto
+0000c8f0: 7265 5f70 6172 7329 0a20 2020 2020 2020  re_pars).       
+0000c900: 2020 2020 2073 632e 7072 696e 7476 2866       sc.printv(f
+0000c910: 2752 756e 2066 696e 6973 6865 6420 6166  'Run finished af
+0000c920: 7465 7220 7b65 6c61 7073 6564 3a30 2e32  ter {elapsed:0.2
+0000c930: 667d 2073 2e5c 6e27 2c20 312c 2076 6572  f} s.\n', 1, ver
+0000c940: 626f 7365 290a 0a20 2020 2020 2020 2072  bose)..        r
+0000c950: 6574 7572 6e20 7365 6c66 0a0a 0a20 2020  eturn self...   
+0000c960: 2064 6566 2066 696e 616c 697a 6528 7365   def finalize(se
+0000c970: 6c66 2c20 7665 7262 6f73 653d 4e6f 6e65  lf, verbose=None
+0000c980: 2c20 7265 7374 6f72 655f 7061 7273 3d54  , restore_pars=T
+0000c990: 7275 6529 3a0a 2020 2020 2020 2020 2727  rue):.        ''
+0000c9a0: 2720 436f 6d70 7574 6520 6669 6e61 6c20  ' Compute final 
+0000c9b0: 7265 7375 6c74 7320 2727 270a 0a20 2020  results '''..   
+0000c9c0: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
+0000c9d0: 756c 7473 5f72 6561 6479 3a0a 2020 2020  ults_ready:.    
+0000c9e0: 2020 2020 2020 2020 2320 4265 6361 7573          # Becaus
+0000c9f0: 6520 7468 6520 7265 7375 6c74 7320 6172  e the results ar
+0000ca00: 6520 7265 7363 616c 6564 2069 6e2d 706c  e rescaled in-pl
+0000ca10: 6163 652c 2066 696e 616c 697a 696e 6720  ace, finalizing 
+0000ca20: 7468 6520 7369 6d20 6361 6e6e 6f74 2062  the sim cannot b
+0000ca30: 6520 7275 6e20 6d6f 7265 2074 6861 6e20  e run more than 
+0000ca40: 6f6e 6365 206f 720a 2020 2020 2020 2020  once or.        
+0000ca50: 2020 2020 2320 6f74 6865 7277 6973 6520      # otherwise 
+0000ca60: 7468 6520 7363 616c 6520 6661 6374 6f72  the scale factor
+0000ca70: 2077 696c 6c20 6265 2061 7070 6c69 6564   will be applied
+0000ca80: 206d 756c 7469 706c 6520 7469 6d65 730a   multiple times.
+0000ca90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000caa0: 6520 416c 7265 6164 7952 756e 4572 726f  e AlreadyRunErro
+0000cab0: 7228 2753 696d 756c 6174 696f 6e20 6861  r('Simulation ha
+0000cac0: 7320 616c 7265 6164 7920 6265 656e 2066  s already been f
+0000cad0: 696e 616c 697a 6564 2729 0a0a 2020 2020  inalized')..    
+0000cae0: 2020 2020 2320 4669 6e61 6c69 7a65 2061      # Finalize a
+0000caf0: 6e61 6c79 7a65 7273 2061 6e64 2069 6e74  nalyzers and int
+0000cb00: 6572 7665 6e74 696f 6e73 0a20 2020 2020  erventions.     
+0000cb10: 2020 2073 656c 662e 6669 6e61 6c69 7a65     self.finalize
+0000cb20: 5f61 6e61 6c79 7a65 7273 2829 0a20 2020  _analyzers().   
+0000cb30: 2020 2020 2023 2073 656c 662e 6669 6e61       # self.fina
+0000cb40: 6c69 7a65 5f69 6e74 6572 7665 6e74 696f  lize_interventio
+0000cb50: 6e73 2829 2023 544f 444f 3a20 7768 7920  ns() #TODO: why 
+0000cb60: 6973 2074 6869 7320 636f 6d6d 656e 7465  is this commente
+0000cb70: 6420 6f75 743f 0a0a 2020 2020 2020 2020  d out?..        
+0000cb80: 6966 2073 656c 665b 276d 6f64 656c 5f68  if self['model_h
+0000cb90: 6976 275d 3a0a 2020 2020 2020 2020 2020  iv']:.          
+0000cba0: 2020 7365 6c66 2e68 6976 7369 6d2e 6669    self.hivsim.fi
+0000cbb0: 6e61 6c69 7a65 2873 656c 6629 0a0a 2020  nalize(self)..  
+0000cbc0: 2020 2020 2020 2320 4669 6e61 6c20 7365        # Final se
+0000cbd0: 7474 696e 6773 0a20 2020 2020 2020 2073  ttings.        s
+0000cbe0: 656c 662e 7265 7375 6c74 735f 7265 6164  elf.results_read
+0000cbf0: 7920 3d20 5472 7565 2023 2053 6574 2074  y = True # Set t
+0000cc00: 6869 7320 6669 7273 7420 736f 2073 656c  his first so sel
+0000cc10: 662e 7375 6d6d 6172 7928 2920 6b6e 6f77  f.summary() know
+0000cc20: 7320 746f 2070 7269 6e74 2074 6865 2072  s to print the r
+0000cc30: 6573 756c 7473 0a20 2020 2020 2020 2073  esults.        s
+0000cc40: 656c 662e 7420 2d3d 2031 2023 2044 7572  elf.t -= 1 # Dur
+0000cc50: 696e 6720 7468 6520 7275 6e2c 2074 6869  ing the run, thi
+0000cc60: 7320 6b65 6570 7320 7472 6163 6b20 6f66  s keeps track of
+0000cc70: 2074 6865 206e 6578 7420 7374 6570 3b20   the next step; 
+0000cc80: 7265 7374 6f72 6520 7468 6973 2062 6520  restore this be 
+0000cc90: 7468 6520 6669 6e61 6c20 6461 7920 6f66  the final day of
+0000cca0: 2074 6865 2073 696d 0a0a 2020 2020 2020   the sim..      
+0000ccb0: 2020 2320 5065 7266 6f72 6d20 6361 6c63    # Perform calc
+0000ccc0: 756c 6174 696f 6e73 206f 6e20 7265 7375  ulations on resu
+0000ccd0: 6c74 730a 2020 2020 2020 2020 7365 6c66  lts.        self
+0000cce0: 2e63 6f6d 7075 7465 5f72 6573 756c 7473  .compute_results
+0000ccf0: 2876 6572 626f 7365 3d76 6572 626f 7365  (verbose=verbose
+0000cd00: 2920 2320 4361 6c63 756c 6174 6520 7468  ) # Calculate th
+0000cd10: 6520 7265 7374 206f 6620 7468 6520 7265  e rest of the re
+0000cd20: 7375 6c74 730a 2020 2020 2020 2020 7365  sults.        se
+0000cd30: 6c66 2e72 6573 756c 7473 203d 2073 632e  lf.results = sc.
+0000cd40: 6f62 6a64 6963 7428 7365 6c66 2e72 6573  objdict(self.res
+0000cd50: 756c 7473 2920 2320 436f 6e76 6572 7420  ults) # Convert 
+0000cd60: 7265 7375 6c74 7320 746f 2061 206f 6469  results to a odi
+0000cd70: 6374 732f 6f62 6a64 6963 7420 746f 2061  cts/objdict to a
+0000cd80: 6c6c 6f77 2065 2e67 2e20 7369 6d2e 7265  llow e.g. sim.re
+0000cd90: 7375 6c74 732e 6469 6167 6e6f 7365 730a  sults.diagnoses.
+0000cda0: 0a20 2020 2020 2020 2023 204f 7074 696f  .        # Optio
+0000cdb0: 6e61 6c6c 7920 7072 696e 7420 7375 6d6d  nally print summ
+0000cdc0: 6172 7920 6f75 7470 7574 0a20 2020 2020  ary output.     
+0000cdd0: 2020 2069 6620 7665 7262 6f73 653a 2023     if verbose: #
+0000cde0: 2056 6572 626f 7365 2069 7320 616e 7920   Verbose is any 
+0000cdf0: 6e6f 6e2d 7a65 726f 2076 616c 7565 0a20  non-zero value. 
+0000ce00: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
+0000ce10: 7262 6f73 653e 303a 2023 2056 6572 626f  rbose>0: # Verbo
+0000ce20: 7365 2069 7320 616e 7920 706f 7369 7469  se is any positi
+0000ce30: 7665 206e 756d 6265 720a 2020 2020 2020  ve number.      
+0000ce40: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000ce50: 756d 6d61 7269 7a65 2829 2023 2050 7269  ummarize() # Pri
+0000ce60: 6e74 206d 6564 6975 6d2d 6c65 6e67 7468  nt medium-length
+0000ce70: 2073 756d 6d61 7279 206f 6620 7468 6520   summary of the 
+0000ce80: 7369 6d0a 2020 2020 2020 2020 2020 2020  sim.            
+0000ce90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000cea0: 2020 2020 2020 7365 6c66 2e62 7269 6566        self.brief
+0000ceb0: 2829 2023 2050 7269 6e74 2062 7269 6566  () # Print brief
+0000cec0: 2073 756d 6d61 7279 206f 6620 7468 6520   summary of the 
+0000ced0: 7369 6d0a 0a20 2020 2020 2020 2072 6574  sim..        ret
+0000cee0: 7572 6e0a 0a0a 2020 2020 6465 6620 636f  urn...    def co
+0000cef0: 6d70 7574 655f 7265 7375 6c74 7328 7365  mpute_results(se
+0000cf00: 6c66 2c20 7665 7262 6f73 653d 4e6f 6e65  lf, verbose=None
+0000cf10: 293a 0a20 2020 2020 2020 2027 2727 2050  ):.        ''' P
+0000cf20: 6572 666f 726d 2066 696e 616c 2063 616c  erform final cal
+0000cf30: 6375 6c61 7469 6f6e 7320 6f6e 2074 6865  culations on the
+0000cf40: 2072 6573 756c 7473 2027 2727 0a20 2020   results '''.   
+0000cf50: 2020 2020 2073 656c 662e 636f 6d70 7574       self.comput
+0000cf60: 655f 7374 6174 6573 2829 0a20 2020 2020  e_states().     
+0000cf70: 2020 2073 656c 662e 636f 6d70 7574 655f     self.compute_
+0000cf80: 7375 6d6d 6172 7928 290a 2020 2020 2020  summary().      
+0000cf90: 2020 7265 7475 726e 0a0a 0a20 2020 2064    return...    d
+0000cfa0: 6566 2063 6f6d 7075 7465 5f73 7461 7465  ef compute_state
+0000cfb0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+0000cfc0: 2027 2727 0a20 2020 2020 2020 2043 6f6d   '''.        Com
+0000cfd0: 7075 7465 2070 7265 7661 6c65 6e63 652c  pute prevalence,
+0000cfe0: 2069 6e63 6964 656e 6365 2c20 616e 6420   incidence, and 
+0000cff0: 6f74 6865 7220 7374 6174 6573 2e0a 2020  other states..  
+0000d000: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0000d010: 2020 7265 7320 3d20 7365 6c66 2e72 6573    res = self.res
+0000d020: 756c 7473 0a0a 2020 2020 2020 2020 2320  ults..        # 
+0000d030: 436f 6d70 7574 6520 4850 5620 696e 6369  Compute HPV inci
+0000d040: 6465 6e63 6520 616e 6420 7072 6576 616c  dence and preval
+0000d050: 656e 6365 0a20 2020 2020 2020 2064 6566  ence.        def
+0000d060: 2073 6166 6564 6976 6964 6528 6e75 6d2c   safedivide(num,
+0000d070: 6465 6e6f 6d29 3a0a 2020 2020 2020 2020  denom):.        
+0000d080: 2020 2020 2727 2720 4465 6669 6e65 2061      ''' Define a
+0000d090: 2076 6172 6961 7469 6f6e 206f 6e20 7363   variation on sc
+0000d0a0: 2e73 6166 6564 6976 6964 6520 7468 6174  .safedivide that
+0000d0b0: 2072 6573 7065 6374 7320 7368 6170 6520   respects shape 
+0000d0c0: 6f66 206e 756d 6572 6174 6f72 2027 2727  of numerator '''
+0000d0d0: 0a20 2020 2020 2020 2020 2020 2061 6e73  .            ans
+0000d0e0: 7765 7220 3d20 6e70 2e7a 6572 6f73 5f6c  wer = np.zeros_l
+0000d0f0: 696b 6528 6e75 6d29 0a20 2020 2020 2020  ike(num).       
+0000d100: 2020 2020 2066 696c 6c5f 696e 6473 203d       fill_inds =
+0000d110: 2028 6465 6e6f 6d21 3d30 292e 6e6f 6e7a   (denom!=0).nonz
+0000d120: 6572 6f28 290a 2020 2020 2020 2020 2020  ero().          
+0000d130: 2020 6966 206c 656e 286e 756d 2e73 6861    if len(num.sha
+0000d140: 7065 293d 3d6c 656e 2864 656e 6f6d 2e73  pe)==len(denom.s
+0000d150: 6861 7065 293a 0a20 2020 2020 2020 2020  hape):.         
+0000d160: 2020 2020 2020 2061 6e73 7765 725b 6669         answer[fi
+0000d170: 6c6c 5f69 6e64 735d 203d 206e 756d 5b66  ll_inds] = num[f
+0000d180: 696c 6c5f 696e 6473 5d20 2f20 6465 6e6f  ill_inds] / deno
+0000d190: 6d5b 6669 6c6c 5f69 6e64 735d 0a20 2020  m[fill_inds].   
+0000d1a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000d1c0: 6e73 7765 725b 3a2c 2066 696c 6c5f 696e  nswer[:, fill_in
+0000d1d0: 6473 5d20 3d20 6e75 6d5b 3a2c 2066 696c  ds] = num[:, fil
+0000d1e0: 6c5f 696e 6473 5d20 2f20 6465 6e6f 6d5b  l_inds] / denom[
+0000d1f0: 6669 6c6c 5f69 6e64 735d 0a20 2020 2020  fill_inds].     
+0000d200: 2020 2020 2020 2072 6574 7572 6e20 616e         return an
+0000d210: 7377 6572 0a20 2020 2020 2020 206e 6720  swer.        ng 
+0000d220: 3d20 7365 6c66 2e70 6172 735b 276e 5f67  = self.pars['n_g
+0000d230: 656e 6f74 7970 6573 275d 0a20 2020 2020  enotypes'].     
+0000d240: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
+0000d250: 2768 7076 5f69 6e63 6964 656e 6365 275d  'hpv_incidence']
+0000d260: 5b3a 5d20 2020 2020 2020 2020 2020 2020  [:]             
+0000d270: 2020 203d 2073 6166 6564 6976 6964 6528     = safedivide(
+0000d280: 7265 735b 2769 6e66 6563 7469 6f6e 7327  res['infections'
+0000d290: 5d5b 3a5d 2c20 6e67 2a72 6573 5b27 6e5f  ][:], ng*res['n_
+0000d2a0: 7375 7363 6570 7469 626c 6527 5d5b 3a5d  susceptible'][:]
+0000d2b0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+0000d2c0: 6573 756c 7473 5b27 6870 765f 696e 6369  esults['hpv_inci
+0000d2d0: 6465 6e63 655f 6279 5f67 656e 6f74 7970  dence_by_genotyp
+0000d2e0: 6527 5d5b 3a5d 2020 2020 3d20 7361 6665  e'][:]    = safe
+0000d2f0: 6469 7669 6465 2872 6573 5b27 696e 6665  divide(res['infe
+0000d300: 6374 696f 6e73 5f62 795f 6765 6e6f 7479  ctions_by_genoty
+0000d310: 7065 275d 5b3a 5d2c 2072 6573 5b27 6e5f  pe'][:], res['n_
+0000d320: 7375 7363 6570 7469 626c 655f 6279 5f67  susceptible_by_g
+0000d330: 656e 6f74 7970 6527 5d5b 3a5d 290a 2020  enotype'][:]).  
+0000d340: 2020 2020 2020 7365 6c66 2e72 6573 756c        self.resul
+0000d350: 7473 5b27 6870 765f 696e 6369 6465 6e63  ts['hpv_incidenc
+0000d360: 655f 6279 5f61 6765 275d 5b3a 5d20 2020  e_by_age'][:]   
+0000d370: 2020 2020 2020 3d20 7361 6665 6469 7669        = safedivi
+0000d380: 6465 2872 6573 5b27 696e 6665 6374 696f  de(res['infectio
+0000d390: 6e73 5f62 795f 6167 6527 5d5b 3a5d 2c20  ns_by_age'][:], 
+0000d3a0: 6e67 2a72 6573 5b27 6e5f 7375 7363 6570  ng*res['n_suscep
+0000d3b0: 7469 626c 655f 6279 5f61 6765 275d 5b3a  tible_by_age'][:
+0000d3c0: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
+0000d3d0: 7265 7375 6c74 735b 2768 7076 5f70 7265  results['hpv_pre
+0000d3e0: 7661 6c65 6e63 6527 5d5b 3a5d 2020 2020  valence'][:]    
+0000d3f0: 2020 2020 2020 2020 2020 203d 2073 6166             = saf
+0000d400: 6564 6976 6964 6528 7265 735b 276e 5f69  edivide(res['n_i
+0000d410: 6e66 6563 7469 6f75 7327 5d5b 3a5d 2c20  nfectious'][:], 
+0000d420: 6e67 2a72 6573 5b27 6e5f 616c 6976 6527  ng*res['n_alive'
+0000d430: 5d5b 3a5d 290a 2020 2020 2020 2020 7365  ][:]).        se
+0000d440: 6c66 2e72 6573 756c 7473 5b27 6870 765f  lf.results['hpv_
+0000d450: 7072 6576 616c 656e 6365 5f62 795f 6765  prevalence_by_ge
+0000d460: 6e6f 7479 7065 275d 5b3a 5d20 2020 3d20  notype'][:]   = 
+0000d470: 7361 6665 6469 7669 6465 2872 6573 5b27  safedivide(res['
+0000d480: 6e5f 696e 6665 6374 696f 7573 5f62 795f  n_infectious_by_
+0000d490: 6765 6e6f 7479 7065 275d 5b3a 5d2c 2072  genotype'][:], r
+0000d4a0: 6573 5b27 6e5f 616c 6976 6527 5d5b 3a5d  es['n_alive'][:]
+0000d4b0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+0000d4c0: 6573 756c 7473 5b27 6870 765f 7072 6576  esults['hpv_prev
+0000d4d0: 616c 656e 6365 5f62 795f 6167 6527 5d5b  alence_by_age'][
+0000d4e0: 3a5d 2020 2020 2020 2020 3d20 7361 6665  :]        = safe
+0000d4f0: 6469 7669 6465 2872 6573 5b27 6e5f 696e  divide(res['n_in
+0000d500: 6665 6374 696f 7573 5f62 795f 6167 6527  fectious_by_age'
+0000d510: 5d5b 3a5d 2c20 7265 735b 276e 5f61 6c69  ][:], res['n_ali
+0000d520: 7665 5f62 795f 6167 6527 5d5b 3a5d 290a  ve_by_age'][:]).
+0000d530: 0a20 2020 2020 2020 2061 6c69 7665 5f66  .        alive_f
+0000d540: 656d 616c 6573 203d 2072 6573 5b27 6e5f  emales = res['n_
+0000d550: 616c 6976 655f 6279 5f73 6578 275d 5b30  alive_by_sex'][0
+0000d560: 2c3a 5d0a 0a20 2020 2020 2020 2073 656c  ,:]..        sel
+0000d570: 662e 7265 7375 6c74 735b 2766 656d 616c  f.results['femal
+0000d580: 655f 6870 765f 7072 6576 616c 656e 6365  e_hpv_prevalence
+0000d590: 5f62 795f 6167 6527 5d5b 3a5d 203d 2073  _by_age'][:] = s
+0000d5a0: 6166 6564 6976 6964 6528 2872 6573 5b27  afedivide((res['
+0000d5b0: 6e5f 6665 6d61 6c65 735f 696e 6665 6374  n_females_infect
+0000d5c0: 696f 7573 5f62 795f 6167 6527 5d5b 3a5d  ious_by_age'][:]
+0000d5d0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d610: 2020 2020 2020 2020 7265 735b 276e 5f66          res['n_f
+0000d620: 656d 616c 6573 5f61 6c69 7665 5f62 795f  emales_alive_by_
+0000d630: 6167 6527 5d5b 3a5d 290a 0a20 2020 2020  age'][:])..     
+0000d640: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
+0000d650: 2770 7265 6369 6e5f 7072 6576 616c 656e  'precin_prevalen
+0000d660: 6365 275d 5b3a 5d20 3d20 7361 6665 6469  ce'][:] = safedi
+0000d670: 7669 6465 2872 6573 5b27 6e5f 7072 6563  vide(res['n_prec
+0000d680: 696e 275d 5b3a 5d2c 206e 6720 2a20 616c  in'][:], ng * al
+0000d690: 6976 655f 6665 6d61 6c65 7329 0a20 2020  ive_females).   
+0000d6a0: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+0000d6b0: 735b 2770 7265 6369 6e5f 7072 6576 616c  s['precin_preval
+0000d6c0: 656e 6365 5f62 795f 6765 6e6f 7479 7065  ence_by_genotype
+0000d6d0: 275d 5b3a 5d20 3d20 7361 6665 6469 7669  '][:] = safedivi
+0000d6e0: 6465 2872 6573 5b27 6e5f 7072 6563 696e  de(res['n_precin
+0000d6f0: 5f62 795f 6765 6e6f 7479 7065 275d 5b3a  _by_genotype'][:
+0000d700: 5d2c 2061 6c69 7665 5f66 656d 616c 6573  ], alive_females
+0000d710: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+0000d720: 6573 756c 7473 5b27 7072 6563 696e 5f70  esults['precin_p
+0000d730: 7265 7661 6c65 6e63 655f 6279 5f61 6765  revalence_by_age
+0000d740: 275d 5b3a 5d20 3d20 7361 6665 6469 7669  '][:] = safedivi
+0000d750: 6465 2872 6573 5b27 6e5f 7072 6563 696e  de(res['n_precin
+0000d760: 5f62 795f 6167 6527 5d5b 3a5d 2c0a 2020  _by_age'][:],.  
+0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0000d7b0: 5b27 6e5f 6665 6d61 6c65 735f 616c 6976  ['n_females_aliv
+0000d7c0: 655f 6279 5f61 6765 275d 5b3a 5d29 0a20  e_by_age'][:]). 
+0000d7d0: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
+0000d7e0: 6c74 735b 2763 696e 315f 7072 6576 616c  lts['cin1_preval
+0000d7f0: 656e 6365 275d 5b3a 5d20 3d20 7361 6665  ence'][:] = safe
+0000d800: 6469 7669 6465 2872 6573 5b27 6e5f 6369  divide(res['n_ci
+0000d810: 6e31 275d 5b3a 5d2c 206e 672a 616c 6976  n1'][:], ng*aliv
+0000d820: 655f 6665 6d61 6c65 7329 0a20 2020 2020  e_females).     
+0000d830: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
+0000d840: 2763 696e 315f 7072 6576 616c 656e 6365  'cin1_prevalence
+0000d850: 5f62 795f 6765 6e6f 7479 7065 275d 5b3a  _by_genotype'][:
+0000d860: 5d20 3d20 7361 6665 6469 7669 6465 2872  ] = safedivide(r
+0000d870: 6573 5b27 6e5f 6369 6e31 5f62 795f 6765  es['n_cin1_by_ge
+0000d880: 6e6f 7479 7065 275d 5b3a 5d2c 2061 6c69  notype'][:], ali
+0000d890: 7665 5f66 656d 616c 6573 290a 2020 2020  ve_females).    
+0000d8a0: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
+0000d8b0: 5b27 6369 6e31 5f70 7265 7661 6c65 6e63  ['cin1_prevalenc
+0000d8c0: 655f 6279 5f61 6765 275d 5b3a 5d20 3d20  e_by_age'][:] = 
+0000d8d0: 7361 6665 6469 7669 6465 2872 6573 5b27  safedivide(res['
+0000d8e0: 6e5f 6369 6e31 5f62 795f 6167 6527 5d5b  n_cin1_by_age'][
+0000d8f0: 3a5d 2c0a 2020 2020 2020 2020 2020 2020  :],.            
+0000d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d930: 2020 2072 6573 5b27 6e5f 6665 6d61 6c65     res['n_female
+0000d940: 735f 616c 6976 655f 6279 5f61 6765 275d  s_alive_by_age']
+0000d950: 5b3a 5d29 0a20 2020 2020 2020 2073 656c  [:]).        sel
+0000d960: 662e 7265 7375 6c74 735b 2763 696e 325f  f.results['cin2_
+0000d970: 7072 6576 616c 656e 6365 275d 5b3a 5d20  prevalence'][:] 
+0000d980: 3d20 7361 6665 6469 7669 6465 2872 6573  = safedivide(res
+0000d990: 5b27 6e5f 6369 6e32 275d 5b3a 5d2c 206e  ['n_cin2'][:], n
+0000d9a0: 672a 616c 6976 655f 6665 6d61 6c65 7329  g*alive_females)
+0000d9b0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0000d9c0: 7375 6c74 735b 2763 696e 325f 7072 6576  sults['cin2_prev
+0000d9d0: 616c 656e 6365 5f62 795f 6765 6e6f 7479  alence_by_genoty
+0000d9e0: 7065 275d 5b3a 5d20 3d20 7361 6665 6469  pe'][:] = safedi
+0000d9f0: 7669 6465 2872 6573 5b27 6e5f 6369 6e32  vide(res['n_cin2
+0000da00: 5f62 795f 6765 6e6f 7479 7065 275d 5b3a  _by_genotype'][:
+0000da10: 5d2c 2061 6c69 7665 5f66 656d 616c 6573  ], alive_females
+0000da20: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+0000da30: 6573 756c 7473 5b27 6369 6e32 5f70 7265  esults['cin2_pre
+0000da40: 7661 6c65 6e63 655f 6279 5f61 6765 275d  valence_by_age']
+0000da50: 5b3a 5d20 3d20 7361 6665 6469 7669 6465  [:] = safedivide
+0000da60: 2872 6573 5b27 6e5f 6369 6e32 5f62 795f  (res['n_cin2_by_
+0000da70: 6167 6527 5d5b 3a5d 2c0a 2020 2020 2020  age'][:],.      
+0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dab0: 2020 2020 2020 2020 2072 6573 5b27 6e5f           res['n_
+0000dac0: 6665 6d61 6c65 735f 616c 6976 655f 6279  females_alive_by
+0000dad0: 5f61 6765 275d 5b3a 5d29 0a20 2020 2020  _age'][:]).     
+0000dae0: 2020 2073 656c 662e 7265 7375 6c74 735b     self.results[
+0000daf0: 2763 696e 335f 7072 6576 616c 656e 6365  'cin3_prevalence
+0000db00: 275d 5b3a 5d20 3d20 7361 6665 6469 7669  '][:] = safedivi
+0000db10: 6465 2872 6573 5b27 6e5f 6369 6e33 275d  de(res['n_cin3']
+0000db20: 5b3a 5d2c 206e 672a 616c 6976 655f 6665  [:], ng*alive_fe
+0000db30: 6d61 6c65 7329 0a20 2020 2020 2020 2073  males).        s
+0000db40: 656c 662e 7265 7375 6c74 735b 2763 696e  elf.results['cin
+0000db50: 335f 7072 6576 616c 656e 6365 5f62 795f  3_prevalence_by_
+0000db60: 6765 6e6f 7479 7065 275d 5b3a 5d20 3d20  genotype'][:] = 
+0000db70: 7361 6665 6469 7669 6465 2872 6573 5b27  safedivide(res['
+0000db80: 6e5f 6369 6e33 5f62 795f 6765 6e6f 7479  n_cin3_by_genoty
+0000db90: 7065 275d 5b3a 5d2c 2061 6c69 7665 5f66  pe'][:], alive_f
+0000dba0: 656d 616c 6573 290a 2020 2020 2020 2020  emales).        
+0000dbb0: 7365 6c66 2e72 6573 756c 7473 5b27 6369  self.results['ci
+0000dbc0: 6e33 5f70 7265 7661 6c65 6e63 655f 6279  n3_prevalence_by
+0000dbd0: 5f61 6765 275d 5b3a 5d20 3d20 7361 6665  _age'][:] = safe
+0000dbe0: 6469 7669 6465 2872 6573 5b27 6e5f 6369  divide(res['n_ci
+0000dbf0: 6e33 5f62 795f 6167 6527 5d5b 3a5d 2c0a  n3_by_age'][:],.
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000dc40: 6573 5b27 6e5f 6665 6d61 6c65 735f 616c  es['n_females_al
+0000dc50: 6976 655f 6279 5f61 6765 275d 5b3a 5d29  ive_by_age'][:])
+0000dc60: 0a20 2020 2020 2020 2023 2043 6f6d 7075  .        # Compu
+0000dc70: 7465 2063 616e 6365 7220 696e 6369 6465  te cancer incide
+0000dc80: 6e63 652e 0a20 2020 2020 2020 2061 745f  nce..        at_
+0000dc90: 7269 736b 5f66 656d 616c 6573 203d 2061  risk_females = a
+0000dca0: 6c69 7665 5f66 656d 616c 6573 202d 2072  live_females - r
+0000dcb0: 6573 5b27 6e5f 6361 6e63 6572 6f75 7327  es['n_cancerous'
+0000dcc0: 5d5b 3a5d 0a20 2020 2020 2020 2073 6361  ][:].        sca
+0000dcd0: 6c65 5f66 6163 746f 7220 3d20 3165 3520  le_factor = 1e5 
+0000dce0: 2023 2043 616e 6365 7220 696e 6369 6465   # Cancer incide
+0000dcf0: 6e63 6520 6172 6520 6469 7370 6c61 7965  nce are displaye
+0000dd00: 6420 6173 2072 6174 6573 2070 6572 2031  d as rates per 1
+0000dd10: 3030 6b20 776f 6d65 6e0a 2020 2020 2020  00k women.      
+0000dd20: 2020 6465 6d6f 6e69 6e61 746f 7220 3d20    demoninator = 
+0000dd30: 6174 5f72 6973 6b5f 6665 6d61 6c65 7320  at_risk_females 
+0000dd40: 2f20 7363 616c 655f 6661 6374 6f72 0a20  / scale_factor. 
 0000dd50: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-0000dd60: 6c74 735b 2763 756d 5f63 696e 5f74 7265  lts['cum_cin_tre
-0000dd70: 6174 6564 275d 5b3a 5d20 3d20 6e70 2e63  ated'][:] = np.c
-0000dd80: 756d 7375 6d28 7365 6c66 2e72 6573 756c  umsum(self.resul
-0000dd90: 7473 5b27 6e65 775f 6369 6e5f 7472 6561  ts['new_cin_trea
-0000dda0: 7465 6427 5d5b 3a5d 2c20 6178 6973 3d30  ted'][:], axis=0
-0000ddb0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-0000ddc0: 6573 756c 7473 5b27 6375 6d5f 6361 6e63  esults['cum_canc
-0000ddd0: 6572 5f74 7265 6174 6d65 6e74 7327 5d5b  er_treatments'][
-0000dde0: 3a5d 203d 206e 702e 6375 6d73 756d 2873  :] = np.cumsum(s
-0000ddf0: 656c 662e 7265 7375 6c74 735b 276e 6577  elf.results['new
-0000de00: 5f63 616e 6365 725f 7472 6561 746d 656e  _cancer_treatmen
-0000de10: 7473 275d 5b3a 5d2c 2061 7869 733d 3029  ts'][:], axis=0)
-0000de20: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000de30: 7375 6c74 735b 2763 756d 5f63 616e 6365  sults['cum_cance
-0000de40: 725f 7472 6561 7465 6427 5d5b 3a5d 203d  r_treated'][:] =
-0000de50: 206e 702e 6375 6d73 756d 2873 656c 662e   np.cumsum(self.
-0000de60: 7265 7375 6c74 735b 276e 6577 5f63 616e  results['new_can
-0000de70: 6365 725f 7472 6561 746d 656e 7473 275d  cer_treatments']
-0000de80: 5b3a 5d2c 2061 7869 733d 3029 0a0a 2020  [:], axis=0)..  
-0000de90: 2020 2020 2020 7265 7475 726e 0a0a 0a20        return... 
-0000dea0: 2020 2064 6566 2063 6f6d 7075 7465 5f73     def compute_s
-0000deb0: 756d 6d61 7279 2873 656c 662c 2074 3d4e  ummary(self, t=N
-0000dec0: 6f6e 652c 2075 7064 6174 653d 5472 7565  one, update=True
-0000ded0: 2c20 6f75 7470 7574 3d46 616c 7365 2c20  , output=False, 
-0000dee0: 7265 7175 6972 655f 7275 6e3d 4661 6c73  require_run=Fals
-0000def0: 6529 3a0a 2020 2020 2020 2020 2727 270a  e):.        '''.
-0000df00: 2020 2020 2020 2020 436f 6d70 7574 6520          Compute 
-0000df10: 7468 6520 7375 6d6d 6172 7920 6469 6374  the summary dict
-0000df20: 2061 6e64 2073 7472 696e 6720 666f 7220   and string for 
-0000df30: 7468 6520 7369 6d2e 2055 7365 6420 696e  the sim. Used in
-0000df40: 7465 726e 616c 6c79 3b20 7365 650a 2020  ternally; see.  
-0000df50: 2020 2020 2020 7369 6d2e 7375 6d6d 6172        sim.summar
-0000df60: 697a 6528 2920 666f 7220 7468 6520 7573  ize() for the us
-0000df70: 6572 2076 6572 7369 6f6e 2e0a 0a20 2020  er version...   
-0000df80: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000df90: 2020 2020 2020 2074 2028 696e 742f 7374         t (int/st
-0000dfa0: 7229 3a20 6461 7920 6f72 2064 6174 6520  r): day or date 
-0000dfb0: 746f 2063 6f6d 7075 7465 2073 756d 6d61  to compute summa
-0000dfc0: 7279 2066 6f72 2028 6279 2064 6566 6175  ry for (by defau
-0000dfd0: 6c74 2c20 7468 6520 6c61 7374 2070 6f69  lt, the last poi
-0000dfe0: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
-0000dff0: 7570 6461 7465 2028 626f 6f6c 293a 2077  update (bool): w
-0000e000: 6865 7468 6572 2074 6f20 7570 6461 7465  hether to update
-0000e010: 2074 6865 2073 746f 7265 6420 7369 6d2e   the stored sim.
-0000e020: 7375 6d6d 6172 790a 2020 2020 2020 2020  summary.        
-0000e030: 2020 2020 6f75 7470 7574 2028 626f 6f6c      output (bool
-0000e040: 293a 2077 6865 7468 6572 2074 6f20 7265  ): whether to re
-0000e050: 7475 726e 2074 6865 2073 756d 6d61 7279  turn the summary
-0000e060: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-0000e070: 7569 7265 5f72 756e 2028 626f 6f6c 293a  uire_run (bool):
-0000e080: 2077 6865 7468 6572 2074 6f20 7261 6973   whether to rais
-0000e090: 6520 616e 2065 7863 6570 7469 6f6e 2069  e an exception i
-0000e0a0: 6620 7369 6d75 6c61 7469 6f6e 7320 6861  f simulations ha
-0000e0b0: 7665 206e 6f74 2062 6565 6e20 7275 6e20  ve not been run 
-0000e0c0: 7965 740a 2020 2020 2020 2020 2727 270a  yet.        '''.
-0000e0d0: 2020 2020 2020 2020 6966 2074 2069 7320          if t is 
-0000e0e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000e0f0: 2020 7420 3d20 2d31 0a0a 2020 2020 2020    t = -1..      
-0000e100: 2020 2320 436f 6d70 7574 6520 7468 6520    # Compute the 
-0000e110: 7375 6d6d 6172 790a 2020 2020 2020 2020  summary.        
-0000e120: 6966 2072 6571 7569 7265 5f72 756e 2061  if require_run a
-0000e130: 6e64 206e 6f74 2073 656c 662e 7265 7375  nd not self.resu
-0000e140: 6c74 735f 7265 6164 793a 0a20 2020 2020  lts_ready:.     
-0000e150: 2020 2020 2020 2065 7272 6f72 6d73 6720         errormsg 
-0000e160: 3d20 2753 696d 756c 6174 696f 6e20 6e6f  = 'Simulation no
-0000e170: 7420 7965 7420 7275 6e27 0a20 2020 2020  t yet run'.     
-0000e180: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-0000e190: 7469 6d65 4572 726f 7228 6572 726f 726d  timeError(errorm
-0000e1a0: 7367 290a 0a20 2020 2020 2020 2073 756d  sg)..        sum
-0000e1b0: 6d61 7279 203d 2073 632e 6f62 6a64 6963  mary = sc.objdic
-0000e1c0: 7428 290a 2020 2020 2020 2020 666f 7220  t().        for 
-0000e1d0: 6b65 7920 696e 2073 656c 662e 7265 7375  key in self.resu
-0000e1e0: 6c74 5f6b 6579 7328 2774 6f74 616c 2729  lt_keys('total')
-0000e1f0: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
-0000e200: 6d6d 6172 795b 6b65 795d 203d 2073 656c  mmary[key] = sel
-0000e210: 662e 7265 7375 6c74 735b 6b65 795d 5b74  f.results[key][t
-0000e220: 5d0a 0a20 2020 2020 2020 2023 2055 7064  ]..        # Upd
-0000e230: 6174 6520 7468 6520 7374 6f72 6564 2073  ate the stored s
-0000e240: 7461 7465 0a20 2020 2020 2020 2069 6620  tate.        if 
-0000e250: 7570 6461 7465 3a0a 2020 2020 2020 2020  update:.        
-0000e260: 2020 2020 7365 6c66 2e73 756d 6d61 7279      self.summary
-0000e270: 203d 2073 756d 6d61 7279 0a0a 2020 2020   = summary..    
-0000e280: 2020 2020 2320 4f70 7469 6f6e 616c 6c79      # Optionally
-0000e290: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000e2a0: 6966 206f 7574 7075 743a 0a20 2020 2020  if output:.     
-0000e2b0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-0000e2c0: 6d6d 6172 790a 2020 2020 2020 2020 656c  mmary.        el
-0000e2d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000e2e0: 7265 7475 726e 0a0a 0a20 2020 2064 6566  return...    def
-0000e2f0: 2073 756d 6d61 7269 7a65 2873 656c 662c   summarize(self,
-0000e300: 2066 756c 6c3d 4661 6c73 652c 2074 3d4e   full=False, t=N
-0000e310: 6f6e 652c 2073 6570 3d4e 6f6e 652c 206f  one, sep=None, o
-0000e320: 7574 7075 743d 4661 6c73 6529 3a0a 2020  utput=False):.  
-0000e330: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000e340: 2020 5072 696e 7420 6120 6d65 6469 756d    Print a medium
-0000e350: 2d6c 656e 6774 6820 7375 6d6d 6172 7920  -length summary 
-0000e360: 6f66 2074 6865 2073 696d 756c 6174 696f  of the simulatio
-0000e370: 6e2c 2064 7261 7769 6e67 2066 726f 6d20  n, drawing from 
-0000e380: 7468 6520 6c61 7374 2074 696d 650a 2020  the last time.  
-0000e390: 2020 2020 2020 706f 696e 7420 696e 2074        point in t
-0000e3a0: 6865 2073 696d 756c 6174 696f 6e20 6279  he simulation by
-0000e3b0: 2064 6566 6175 6c74 2e20 4361 6c6c 6564   default. Called
-0000e3c0: 2062 7920 6465 6661 756c 7420 6174 2074   by default at t
-0000e3d0: 6865 2065 6e64 206f 6620 6120 7369 6d20  he end of a sim 
-0000e3e0: 7275 6e2e 0a20 2020 2020 2020 2070 6f69  run..        poi
-0000e3f0: 6e74 2069 6e20 7468 6520 7369 6d75 6c61  nt in the simula
-0000e400: 7469 6f6e 2062 7920 6465 6661 756c 742e  tion by default.
-0000e410: 2043 616c 6c65 6420 6279 2064 6566 6175   Called by defau
-0000e420: 6c74 2061 7420 7468 6520 656e 6420 6f66  lt at the end of
-0000e430: 2061 2073 696d 2072 756e 2e0a 2020 2020   a sim run..    
-0000e440: 2020 2020 5365 6520 616c 736f 2073 696d      See also sim
-0000e450: 2e64 6973 7028 2920 2864 6574 6169 6c65  .disp() (detaile
-0000e460: 6420 6f75 7470 7574 2920 616e 6420 7369  d output) and si
-0000e470: 6d2e 6272 6965 6628 2920 2873 686f 7274  m.brief() (short
-0000e480: 206f 7574 7075 7429 2e0a 0a20 2020 2020   output)...     
-0000e490: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000e4a0: 2020 2020 2066 756c 6c20 2020 2862 6f6f       full   (boo
-0000e4b0: 6c29 3a20 2020 2077 6865 7468 6572 206f  l):    whether o
-0000e4c0: 7220 6e6f 7420 746f 2070 7269 6e74 2061  r not to print a
-0000e4d0: 6c6c 2072 6573 756c 7473 2028 6279 2064  ll results (by d
-0000e4e0: 6566 6175 6c74 2c20 6f6e 6c79 2063 756d  efault, only cum
-0000e4f0: 756c 6174 6976 6529 0a20 2020 2020 2020  ulative).       
-0000e500: 2020 2020 2074 2020 2020 2020 2869 6e74       t      (int
-0000e510: 2f73 7472 293a 2064 6179 206f 7220 6461  /str): day or da
-0000e520: 7465 2074 6f20 636f 6d70 7574 6520 7375  te to compute su
-0000e530: 6d6d 6172 7920 666f 7220 2862 7920 6465  mmary for (by de
-0000e540: 6661 756c 742c 2074 6865 206c 6173 7420  fault, the last 
-0000e550: 706f 696e 7429 0a20 2020 2020 2020 2020  point).         
-0000e560: 2020 2073 6570 2020 2020 2873 7472 293a     sep    (str):
-0000e570: 2020 2020 2074 686f 7573 616e 6473 2073       thousands s
-0000e580: 6570 6172 6174 6f72 2028 6465 6661 756c  eparator (defaul
-0000e590: 7420 272c 2729 0a20 2020 2020 2020 2020  t ',').         
-0000e5a0: 2020 206f 7574 7075 7420 2862 6f6f 6c29     output (bool)
-0000e5b0: 3a20 2020 2077 6865 7468 6572 2074 6f20  :    whether to 
-0000e5c0: 7265 7475 726e 2074 6865 2073 756d 6d61  return the summa
-0000e5d0: 7279 2069 6e73 7465 6164 206f 6620 7072  ry instead of pr
-0000e5e0: 696e 7469 6e67 2069 740a 0a20 2020 2020  inting it..     
-0000e5f0: 2020 202a 2a45 7861 6d70 6c65 732a 2a3a     **Examples**:
-0000e600: 3a0a 0a20 2020 2020 2020 2020 2020 2073  :..            s
-0000e610: 696d 203d 2068 7076 2e53 696d 286c 6162  im = hpv.Sim(lab
-0000e620: 656c 3d27 4578 616d 706c 6520 7369 6d27  el='Example sim'
-0000e630: 2c20 7665 7262 6f73 653d 3029 2023 2053  , verbose=0) # S
-0000e640: 6574 2074 6f20 7275 6e20 7369 6c65 6e74  et to run silent
-0000e650: 6c79 0a20 2020 2020 2020 2020 2020 2073  ly.            s
-0000e660: 696d 2e72 756e 2829 2023 2052 756e 2074  im.run() # Run t
-0000e670: 6865 2073 696d 0a20 2020 2020 2020 2020  he sim.         
-0000e680: 2020 2073 696d 2e73 756d 6d61 7269 7a65     sim.summarize
-0000e690: 2829 2023 2050 7269 6e74 206d 6564 6975  () # Print mediu
-0000e6a0: 6d2d 6c65 6e67 7468 2073 756d 6d61 7279  m-length summary
-0000e6b0: 206f 6620 7468 6520 7369 6d0a 2020 2020   of the sim.    
-0000e6c0: 2020 2020 2020 2020 7369 6d2e 7375 6d6d          sim.summ
-0000e6d0: 6172 697a 6528 743d 3234 2c20 6675 6c6c  arize(t=24, full
-0000e6e0: 3d54 7275 6529 2023 2050 7269 6e74 2061  =True) # Print a
-0000e6f0: 2022 736c 6963 6522 206f 6620 616c 6c20   "slice" of all 
-0000e700: 7369 6d20 7265 7375 6c74 7320 6f6e 2064  sim results on d
-0000e710: 6179 2032 340a 2020 2020 2020 2020 2727  ay 24.        ''
-0000e720: 270a 2020 2020 2020 2020 2320 436f 6d70  '.        # Comp
-0000e730: 7574 6520 7468 6520 7375 6d6d 6172 790a  ute the summary.
-0000e740: 2020 2020 2020 2020 7375 6d6d 6172 7920          summary 
-0000e750: 3d20 7365 6c66 2e63 6f6d 7075 7465 5f73  = self.compute_s
-0000e760: 756d 6d61 7279 2874 3d74 2c20 7570 6461  ummary(t=t, upda
-0000e770: 7465 3d46 616c 7365 2c20 6f75 7470 7574  te=False, output
-0000e780: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-0000e790: 2320 436f 6e73 7472 7563 7420 7468 6520  # Construct the 
-0000e7a0: 6f75 7470 7574 2073 7472 696e 670a 2020  output string.  
-0000e7b0: 2020 2020 2020 6966 2073 6570 2069 7320        if sep is 
-0000e7c0: 4e6f 6e65 3a20 7365 7020 3d20 6870 6f2e  None: sep = hpo.
-0000e7d0: 7365 7020 2320 4465 6661 756c 7420 7365  sep # Default se
-0000e7e0: 7061 7261 746f 720a 2020 2020 2020 2020  parator.        
-0000e7f0: 6c61 6265 6c73 7472 203d 2066 2720 227b  labelstr = f' "{
-0000e800: 7365 6c66 2e6c 6162 656c 7d22 2720 6966  self.label}"' if
-0000e810: 2073 656c 662e 6c61 6265 6c20 656c 7365   self.label else
-0000e820: 2027 270a 2020 2020 2020 2020 7374 7269   ''.        stri
-0000e830: 6e67 203d 2066 2753 696d 756c 6174 696f  ng = f'Simulatio
-0000e840: 6e7b 6c61 6265 6c73 7472 7d20 7375 6d6d  n{labelstr} summ
-0000e850: 6172 793a 5c6e 270a 2020 2020 2020 2020  ary:\n'.        
-0000e860: 666f 7220 6b65 7920 696e 2073 656c 662e  for key in self.
-0000e870: 7265 7375 6c74 5f6b 6579 7328 2774 6f74  result_keys('tot
-0000e880: 616c 2729 3a0a 2020 2020 2020 2020 2020  al'):.          
-0000e890: 2020 7661 6c20 3d20 7375 6d6d 6172 795b    val = summary[
-0000e8a0: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
-0000e8b0: 2070 7269 6e74 7661 6c20 3d20 6627 2020   printval = f'  
-0000e8c0: 207b 7661 6c3a 3130 2c2e 3066 7d20 270a   {val:10,.0f} '.
-0000e8d0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-0000e8e0: 6c20 3d20 7365 6c66 2e72 6573 756c 7473  l = self.results
-0000e8f0: 5b6b 6579 5d2e 6e61 6d65 2e6c 6f77 6572  [key].name.lower
-0000e900: 2829 2e72 6570 6c61 6365 2827 2c27 2c20  ().replace(',', 
-0000e910: 7365 7029 0a20 2020 2020 2020 2020 2020  sep).           
-0000e920: 2069 6620 2769 6e63 6964 656e 6365 2720   if 'incidence' 
-0000e930: 696e 206b 6579 206f 7220 2770 7265 7661  in key or 'preva
-0000e940: 6c65 6e63 6527 2069 6e20 6b65 793a 0a20  lence' in key:. 
-0000e950: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e960: 6620 6b65 7920 696e 205b 2768 7076 5f70  f key in ['hpv_p
-0000e970: 7265 7661 6c65 6e63 6527 2c20 2768 7076  revalence', 'hpv
-0000e980: 5f69 6e63 6964 656e 6365 275d 3a0a 2020  _incidence']:.  
-0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9a0: 2020 7072 696e 7476 616c 203d 2066 2720    printval = f' 
-0000e9b0: 2020 7b76 616c 2a31 3030 3a31 302e 3266    {val*100:10.2f
-0000e9c0: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
-0000e9d0: 2020 2020 2020 2020 6c61 6265 6c20 2b3d          label +=
-0000e9e0: 2027 2028 2f31 3030 2927 0a20 2020 2020   ' (/100)'.     
-0000e9f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000ea00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea10: 2020 2020 206c 6162 656c 202b 3d20 2720       label += ' 
-0000ea20: 282f 3130 302c 3030 3029 270a 2020 2020  (/100,000)'.    
-0000ea30: 2020 2020 2020 2020 7374 7269 6e67 202b          string +
-0000ea40: 3d20 7072 696e 7476 616c 202b 206c 6162  = printval + lab
-0000ea50: 656c 202b 2027 5c6e 270a 0a20 2020 2020  el + '\n'..     
-0000ea60: 2020 2023 2050 7269 6e74 206f 7220 7265     # Print or re
-0000ea70: 7475 726e 2073 7472 696e 670a 2020 2020  turn string.    
-0000ea80: 2020 2020 6966 206e 6f74 206f 7574 7075      if not outpu
-0000ea90: 743a 0a20 2020 2020 2020 2020 2020 2070  t:.            p
-0000eaa0: 7269 6e74 2873 7472 696e 6729 0a20 2020  rint(string).   
-0000eab0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000eac0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-0000ead0: 7269 6e67 0a0a 0a20 2020 2064 6566 2070  ring...    def p
-0000eae0: 6c6f 7428 7365 6c66 2c20 2a61 7267 732c  lot(self, *args,
-0000eaf0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-0000eb00: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0000eb10: 506c 6f74 2074 6865 206f 7574 7075 7473  Plot the outputs
-0000eb20: 206f 6620 7468 6520 6d6f 6465 6c0a 2020   of the model.  
-0000eb30: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000eb40: 2020 6669 6720 3d20 6870 706c 742e 706c    fig = hpplt.pl
-0000eb50: 6f74 5f73 696d 2873 696d 3d73 656c 662c  ot_sim(sim=self,
-0000eb60: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-0000eb70: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000eb80: 2066 6967 0a0a 0a20 2020 2064 6566 2063   fig...    def c
-0000eb90: 6f6d 7075 7465 5f66 6974 2873 656c 6629  ompute_fit(self)
-0000eba0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-0000ebb0: 2020 2020 2020 436f 6d70 7574 6520 6669        Compute fi
-0000ebc0: 7420 6265 7477 6565 6e20 6d6f 6465 6c20  t between model 
-0000ebd0: 616e 6420 6461 7461 2e0a 2020 2020 2020  and data..      
-0000ebe0: 2020 2727 270a 2020 2020 2020 2020 7265    '''.        re
-0000ebf0: 7475 726e 2073 656c 662e 6669 740a 0a0a  turn self.fit...
-0000ec00: 636c 6173 7320 416c 7265 6164 7952 756e  class AlreadyRun
-0000ec10: 4572 726f 7228 5275 6e74 696d 6545 7272  Error(RuntimeErr
-0000ec20: 6f72 293a 0a20 2020 2027 2727 0a20 2020  or):.    '''.   
-0000ec30: 2054 6869 7320 6572 726f 7220 6973 2072   This error is r
-0000ec40: 6169 7365 6420 6966 2061 2073 696d 756c  aised if a simul
-0000ec50: 6174 696f 6e20 6973 2072 756e 2069 6e20  ation is run in 
-0000ec60: 7375 6368 2061 2077 6179 2074 6861 7420  such a way that 
-0000ec70: 6e6f 2074 696d 6573 7465 7073 0a20 2020  no timesteps.   
-0000ec80: 2077 696c 6c20 6265 2074 616b 656e 2e20   will be taken. 
-0000ec90: 5468 6973 2065 7272 6f72 2069 7320 6120  This error is a 
-0000eca0: 6469 7374 696e 6374 2074 7970 6520 736f  distinct type so
-0000ecb0: 2074 6861 7420 6974 2063 616e 2062 6520   that it can be 
-0000ecc0: 7361 6665 6c79 2063 6175 6768 740a 2020  safely caught.  
-0000ecd0: 2020 616e 6420 6967 6e6f 7265 6420 6966    and ignored if
-0000ece0: 2072 6571 7569 7265 642c 2062 7574 2069   required, but i
-0000ecf0: 7420 6973 2061 6e74 6963 6970 6174 6564  t is anticipated
-0000ed00: 2074 6861 7420 6d6f 7374 206f 6620 7468   that most of th
-0000ed10: 6520 7469 6d65 2c20 6361 6c6c 696e 670a  e time, calling.
-0000ed20: 2020 2020 3a70 793a 6675 6e63 3a60 5369      :py:func:`Si
-0000ed30: 6d2e 7275 6e60 2061 6e64 206e 6f74 2074  m.run` and not t
-0000ed40: 616b 696e 6720 616e 7920 7469 6d65 7374  aking any timest
-0000ed50: 6570 732c 2077 6f75 6c64 2062 6520 616e  eps, would be an
-0000ed60: 2069 6e61 6476 6572 7465 6e74 2065 7272   inadvertent err
-0000ed70: 6f72 2e0a 2020 2020 2727 270a 2020 2020  or..    '''.    
-0000ed80: 7061 7373 0a0a 0a64 6566 2064 6966 665f  pass...def diff_
-0000ed90: 7369 6d73 2873 696d 312c 2073 696d 322c  sims(sim1, sim2,
-0000eda0: 2073 6b69 705f 6b65 795f 6469 6666 733d   skip_key_diffs=
-0000edb0: 4661 6c73 652c 2073 6b69 703d 4e6f 6e65  False, skip=None
-0000edc0: 2c20 6f75 7470 7574 3d46 616c 7365 2c20  , output=False, 
-0000edd0: 6469 653d 4661 6c73 6529 3a0a 2020 2020  die=False):.    
-0000ede0: 2727 270a 2020 2020 436f 6d70 7574 6520  '''.    Compute 
-0000edf0: 7468 6520 6469 6666 6572 656e 6365 206f  the difference o
-0000ee00: 6620 7468 6520 7375 6d6d 6172 6965 7320  f the summaries 
-0000ee10: 6f66 2074 776f 2073 696d 756c 6174 696f  of two simulatio
-0000ee20: 6e73 2c20 616e 6420 7072 696e 7420 616e  ns, and print an
-0000ee30: 790a 2020 2020 7661 6c75 6573 2077 6869  y.    values whi
-0000ee40: 6368 2064 6966 6665 722e 0a0a 2020 2020  ch differ...    
-0000ee50: 4172 6773 3a0a 2020 2020 2020 2020 7369  Args:.        si
-0000ee60: 6d31 2028 7369 6d2f 6469 6374 293a 2065  m1 (sim/dict): e
-0000ee70: 6974 6865 7220 6120 7369 6d75 6c61 7469  ither a simulati
-0000ee80: 6f6e 206f 626a 6563 7420 6f72 2074 6865  on object or the
-0000ee90: 2073 696d 2e73 756d 6d61 7279 2064 6963   sim.summary dic
-0000eea0: 7469 6f6e 6172 790a 2020 2020 2020 2020  tionary.        
-0000eeb0: 7369 6d32 2028 7369 6d2f 6469 6374 293a  sim2 (sim/dict):
-0000eec0: 2064 6974 746f 0a20 2020 2020 2020 2073   ditto.        s
-0000eed0: 6b69 705f 6b65 795f 6469 6666 7320 2862  kip_key_diffs (b
-0000eee0: 6f6f 6c29 3a20 7768 6574 6865 7220 746f  ool): whether to
-0000eef0: 2073 6b69 7020 6b65 7973 2074 6861 7420   skip keys that 
-0000ef00: 646f 6e27 7420 6d61 7463 6820 6265 7477  don't match betw
-0000ef10: 6565 6e20 7369 6d73 0a20 2020 2020 2020  een sims.       
-0000ef20: 2073 6b69 7020 286c 6973 7429 3a20 6120   skip (list): a 
-0000ef30: 6c69 7374 206f 6620 7661 6c75 6573 2074  list of values t
-0000ef40: 6f20 736b 6970 0a20 2020 2020 2020 206f  o skip.        o
-0000ef50: 7574 7075 7420 2862 6f6f 6c29 3a20 7768  utput (bool): wh
-0000ef60: 6574 6865 7220 746f 2072 6574 7572 6e20  ether to return 
-0000ef70: 7468 6520 6f75 7470 7574 2061 7320 6120  the output as a 
-0000ef80: 7374 7269 6e67 2028 6f74 6865 7277 6973  string (otherwis
-0000ef90: 6520 7072 696e 7429 0a20 2020 2020 2020  e print).       
-0000efa0: 2064 6965 2028 626f 6f6c 293a 2077 6865   die (bool): whe
-0000efb0: 7468 6572 2074 6f20 7261 6973 6520 616e  ther to raise an
-0000efc0: 2065 7863 6570 7469 6f6e 2069 6620 7468   exception if th
-0000efd0: 6520 7369 6d73 2064 6f6e 2774 206d 6174  e sims don't mat
-0000efe0: 6368 0a20 2020 2020 2020 2072 6571 7569  ch.        requi
-0000eff0: 7265 5f72 756e 2028 626f 6f6c 293a 2072  re_run (bool): r
-0000f000: 6571 7569 7265 2074 6861 7420 7468 6520  equire that the 
-0000f010: 7369 6d75 6c61 7469 6f6e 7320 6861 7665  simulations have
-0000f020: 2062 6565 6e20 7275 6e0a 0a20 2020 202a   been run..    *
-0000f030: 2a45 7861 6d70 6c65 2a2a 3a3a 0a0a 2020  *Example**::..  
-0000f040: 2020 2020 2020 7331 203d 2068 7076 2e53        s1 = hpv.S
-0000f050: 696d 2872 616e 645f 7365 6564 3d31 292e  im(rand_seed=1).
-0000f060: 7275 6e28 290a 2020 2020 2020 2020 7332  run().        s2
-0000f070: 203d 2068 7076 2e53 696d 2872 616e 645f   = hpv.Sim(rand_
-0000f080: 7365 6564 3d32 292e 7275 6e28 290a 2020  seed=2).run().  
-0000f090: 2020 2020 2020 6870 762e 6469 6666 5f73        hpv.diff_s
-0000f0a0: 696d 7328 7331 2c20 7332 290a 2020 2020  ims(s1, s2).    
-0000f0b0: 2727 270a 0a20 2020 2069 6620 6973 696e  '''..    if isin
-0000f0c0: 7374 616e 6365 2873 696d 312c 2053 696d  stance(sim1, Sim
-0000f0d0: 293a 0a20 2020 2020 2020 2073 696d 3120  ):.        sim1 
-0000f0e0: 3d20 7369 6d31 2e63 6f6d 7075 7465 5f73  = sim1.compute_s
-0000f0f0: 756d 6d61 7279 2875 7064 6174 653d 4661  ummary(update=Fa
-0000f100: 6c73 652c 206f 7574 7075 743d 5472 7565  lse, output=True
-0000f110: 2c20 7265 7175 6972 655f 7275 6e3d 5472  , require_run=Tr
-0000f120: 7565 290a 2020 2020 6966 2069 7369 6e73  ue).    if isins
-0000f130: 7461 6e63 6528 7369 6d32 2c20 5369 6d29  tance(sim2, Sim)
-0000f140: 3a0a 2020 2020 2020 2020 7369 6d32 203d  :.        sim2 =
-0000f150: 2073 696d 322e 636f 6d70 7574 655f 7375   sim2.compute_su
-0000f160: 6d6d 6172 7928 7570 6461 7465 3d46 616c  mmary(update=Fal
-0000f170: 7365 2c20 6f75 7470 7574 3d54 7275 652c  se, output=True,
-0000f180: 2072 6571 7569 7265 5f72 756e 3d54 7275   require_run=Tru
-0000f190: 6529 0a20 2020 2066 6f72 2073 696d 2069  e).    for sim i
-0000f1a0: 6e20 5b73 696d 312c 2073 696d 325d 3a0a  n [sim1, sim2]:.
-0000f1b0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0000f1c0: 7369 6e73 7461 6e63 6528 7369 6d2c 2064  sinstance(sim, d
-0000f1d0: 6963 7429 3a20 2320 7072 6167 6d61 3a20  ict): # pragma: 
-0000f1e0: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
-0000f1f0: 2020 2020 2065 7272 6f72 6d73 6720 3d20       errormsg = 
-0000f200: 6627 4361 6e6e 6f74 2063 6f6d 7061 7265  f'Cannot compare
-0000f210: 206f 626a 6563 7420 6f66 2074 7970 6520   object of type 
-0000f220: 7b74 7970 6528 7369 6d29 7d2c 206d 7573  {type(sim)}, mus
-0000f230: 7420 6265 2061 2073 696d 206f 7220 6120  t be a sim or a 
-0000f240: 7369 6d2e 7375 6d6d 6172 7920 6469 6374  sim.summary dict
-0000f250: 270a 2020 2020 2020 2020 2020 2020 7261  '.            ra
-0000f260: 6973 6520 5479 7065 4572 726f 7228 6572  ise TypeError(er
-0000f270: 726f 726d 7367 290a 0a20 2020 2023 2043  rormsg)..    # C
-0000f280: 6f6d 7061 7265 206b 6579 730a 2020 2020  ompare keys.    
-0000f290: 6b65 796d 6174 6368 6d73 6720 3d20 2727  keymatchmsg = ''
-0000f2a0: 0a20 2020 2073 696d 315f 6b65 7973 203d  .    sim1_keys =
-0000f2b0: 2073 6574 2873 696d 312e 6b65 7973 2829   set(sim1.keys()
-0000f2c0: 290a 2020 2020 7369 6d32 5f6b 6579 7320  ).    sim2_keys 
-0000f2d0: 3d20 7365 7428 7369 6d32 2e6b 6579 7328  = set(sim2.keys(
-0000f2e0: 2929 0a20 2020 2069 6620 7369 6d31 5f6b  )).    if sim1_k
-0000f2f0: 6579 7320 213d 2073 696d 325f 6b65 7973  eys != sim2_keys
-0000f300: 2061 6e64 206e 6f74 2073 6b69 705f 6b65   and not skip_ke
-0000f310: 795f 6469 6666 733a 2023 2070 7261 676d  y_diffs: # pragm
-0000f320: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
-0000f330: 2020 2020 6b65 796d 6174 6368 6d73 6720      keymatchmsg 
-0000f340: 3d20 224b 6579 7320 646f 6e27 7420 6d61  = "Keys don't ma
-0000f350: 7463 6821 5c6e 220a 2020 2020 2020 2020  tch!\n".        
-0000f360: 6d69 7373 696e 6720 3d20 6c69 7374 2873  missing = list(s
-0000f370: 696d 315f 6b65 7973 202d 2073 696d 325f  im1_keys - sim2_
-0000f380: 6b65 7973 290a 2020 2020 2020 2020 6578  keys).        ex
-0000f390: 7472 6120 2020 3d20 6c69 7374 2873 696d  tra   = list(sim
-0000f3a0: 325f 6b65 7973 202d 2073 696d 315f 6b65  2_keys - sim1_ke
-0000f3b0: 7973 290a 2020 2020 2020 2020 6966 206d  ys).        if m
-0000f3c0: 6973 7369 6e67 3a0a 2020 2020 2020 2020  issing:.        
-0000f3d0: 2020 2020 6b65 796d 6174 6368 6d73 6720      keymatchmsg 
-0000f3e0: 2b3d 2066 2720 204d 6973 7369 6e67 2073  += f'  Missing s
-0000f3f0: 696d 3120 6b65 7973 3a20 7b6d 6973 7369  im1 keys: {missi
-0000f400: 6e67 7d5c 6e73 270a 2020 2020 2020 2020  ng}\ns'.        
-0000f410: 6966 2065 7874 7261 3a0a 2020 2020 2020  if extra:.      
-0000f420: 2020 2020 2020 6b65 796d 6174 6368 6d73        keymatchms
-0000f430: 6720 2b3d 2066 2720 2045 7874 7261 2073  g += f'  Extra s
-0000f440: 696d 3220 6b65 7973 3a20 7b65 7874 7261  im2 keys: {extra
-0000f450: 7d5c 6e27 0a0a 2020 2020 2320 436f 6d70  }\n'..    # Comp
-0000f460: 6172 6520 7661 6c75 6573 0a20 2020 2076  are values.    v
-0000f470: 616c 6d61 7463 686d 7367 203d 2027 270a  almatchmsg = ''.
-0000f480: 2020 2020 6d69 736d 6174 6368 6573 203d      mismatches =
-0000f490: 207b 7d0a 2020 2020 736b 6970 203d 2073   {}.    skip = s
-0000f4a0: 632e 746f 6c69 7374 2873 6b69 7029 0a20  c.tolist(skip). 
-0000f4b0: 2020 2066 6f72 206b 6579 2069 6e20 7369     for key in si
-0000f4c0: 6d32 2e6b 6579 7328 293a 2023 2054 6f20  m2.keys(): # To 
-0000f4d0: 656e 7375 7265 206f 7264 6572 0a20 2020  ensure order.   
-0000f4e0: 2020 2020 2069 6620 6b65 7920 696e 2073       if key in s
-0000f4f0: 696d 315f 6b65 7973 2061 6e64 206b 6579  im1_keys and key
-0000f500: 206e 6f74 2069 6e20 736b 6970 3a20 2320   not in skip: # 
-0000f510: 4966 2061 206b 6579 2069 7320 6d69 7373  If a key is miss
-0000f520: 696e 672c 2064 6f6e 2774 2063 6f75 6e74  ing, don't count
-0000f530: 2069 7420 6173 2061 206d 6973 6d61 7463   it as a mismatc
-0000f540: 680a 2020 2020 2020 2020 2020 2020 7369  h.            si
-0000f550: 6d31 5f76 616c 203d 2073 696d 315b 6b65  m1_val = sim1[ke
-0000f560: 795d 2069 6620 6b65 7920 696e 2073 696d  y] if key in sim
-0000f570: 3120 656c 7365 2027 6e6f 7420 7072 6573  1 else 'not pres
-0000f580: 656e 7427 0a20 2020 2020 2020 2020 2020  ent'.           
-0000f590: 2073 696d 325f 7661 6c20 3d20 7369 6d32   sim2_val = sim2
-0000f5a0: 5b6b 6579 5d20 6966 206b 6579 2069 6e20  [key] if key in 
-0000f5b0: 7369 6d32 2065 6c73 6520 276e 6f74 2070  sim2 else 'not p
-0000f5c0: 7265 7365 6e74 270a 2020 2020 2020 2020  resent'.        
-0000f5d0: 2020 2020 6966 206e 6f74 206e 702e 6973      if not np.is
-0000f5e0: 636c 6f73 6528 7369 6d31 5f76 616c 2c20  close(sim1_val, 
-0000f5f0: 7369 6d32 5f76 616c 2c20 6571 7561 6c5f  sim2_val, equal_
-0000f600: 6e61 6e3d 5472 7565 293a 0a20 2020 2020  nan=True):.     
-0000f610: 2020 2020 2020 2020 2020 206d 6973 6d61             misma
-0000f620: 7463 6865 735b 6b65 795d 203d 207b 2773  tches[key] = {'s
-0000f630: 696d 3127 3a20 7369 6d31 5f76 616c 2c20  im1': sim1_val, 
-0000f640: 2773 696d 3227 3a20 7369 6d32 5f76 616c  'sim2': sim2_val
-0000f650: 7d0a 0a20 2020 2069 6620 6c65 6e28 6d69  }..    if len(mi
-0000f660: 736d 6174 6368 6573 293a 0a20 2020 2020  smatches):.     
-0000f670: 2020 2076 616c 6d61 7463 686d 7367 203d     valmatchmsg =
-0000f680: 2027 5c6e 5468 6520 666f 6c6c 6f77 696e   '\nThe followin
-0000f690: 6720 7661 6c75 6573 2064 6966 6665 7220  g values differ 
-0000f6a0: 6265 7477 6565 6e20 7468 6520 7477 6f20  between the two 
-0000f6b0: 7369 6d75 6c61 7469 6f6e 733a 5c6e 270a  simulations:\n'.
-0000f6c0: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
-0000f6d0: 4461 7461 4672 616d 652e 6672 6f6d 5f64  DataFrame.from_d
-0000f6e0: 6963 7428 6d69 736d 6174 6368 6573 292e  ict(mismatches).
-0000f6f0: 7472 616e 7370 6f73 6528 290a 2020 2020  transpose().    
-0000f700: 2020 2020 6469 6666 2020 203d 205b 5d0a      diff   = [].
-0000f710: 2020 2020 2020 2020 7261 7469 6f20 203d          ratio  =
-0000f720: 205b 5d0a 2020 2020 2020 2020 6368 616e   [].        chan
-0000f730: 6765 203d 205b 5d0a 2020 2020 2020 2020  ge = [].        
-0000f740: 736d 616c 6c5f 6368 616e 6765 203d 2031  small_change = 1
-0000f750: 652d 3320 2320 4465 6669 6e65 2061 2073  e-3 # Define a s
-0000f760: 6d61 6c6c 2063 6861 6e67 652c 2065 2e67  mall change, e.g
-0000f770: 2e20 6120 726f 756e 6469 6e67 2065 7272  . a rounding err
-0000f780: 6f72 0a20 2020 2020 2020 2066 6f72 206d  or.        for m
-0000f790: 6469 6374 2069 6e20 6d69 736d 6174 6368  dict in mismatch
-0000f7a0: 6573 2e76 616c 7565 7328 293a 0a20 2020  es.values():.   
-0000f7b0: 2020 2020 2020 2020 206f 6c64 203d 206d           old = m
-0000f7c0: 6469 6374 5b27 7369 6d31 275d 0a20 2020  dict['sim1'].   
-0000f7d0: 2020 2020 2020 2020 206e 6577 203d 206d           new = m
-0000f7e0: 6469 6374 5b27 7369 6d32 275d 0a20 2020  dict['sim2'].   
-0000f7f0: 2020 2020 2020 2020 206e 756d 6572 6963           numeric
-0000f800: 203d 2073 632e 6973 6e75 6d62 6572 2873   = sc.isnumber(s
-0000f810: 696d 315f 7661 6c29 2061 6e64 2073 632e  im1_val) and sc.
-0000f820: 6973 6e75 6d62 6572 2873 696d 325f 7661  isnumber(sim2_va
-0000f830: 6c29 0a20 2020 2020 2020 2020 2020 2069  l).            i
-0000f840: 6620 6e75 6d65 7269 6320 616e 6420 6f6c  f numeric and ol
-0000f850: 643e 303a 0a20 2020 2020 2020 2020 2020  d>0:.           
-0000f860: 2020 2020 2074 6869 735f 6469 6666 2020       this_diff  
-0000f870: 3d20 6e65 7720 2d20 6f6c 640a 2020 2020  = new - old.    
-0000f880: 2020 2020 2020 2020 2020 2020 7468 6973              this
-0000f890: 5f72 6174 696f 203d 206e 6577 2f6f 6c64  _ratio = new/old
-0000f8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f8b0: 2061 6273 5f72 6174 696f 2020 3d20 6d61   abs_ratio  = ma
-0000f8c0: 7828 7468 6973 5f72 6174 696f 2c20 312e  x(this_ratio, 1.
-0000f8d0: 302f 7468 6973 5f72 6174 696f 290a 0a20  0/this_ratio).. 
-0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f8f0: 2053 6574 2074 6865 2063 6861 7261 6374   Set the charact
-0000f900: 6572 2074 6f20 7573 650a 2020 2020 2020  er to use.      
-0000f910: 2020 2020 2020 2020 2020 6966 2061 6273            if abs
-0000f920: 5f72 6174 696f 3c73 6d61 6c6c 5f63 6861  _ratio<small_cha
-0000f930: 6e67 653a 0a20 2020 2020 2020 2020 2020  nge:.           
-0000f940: 2020 2020 2020 2020 2063 6861 6e67 655f           change_
-0000f950: 6368 6172 203d 2027 e289 8827 0a20 2020  char = '...'.   
-0000f960: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-0000f970: 6620 6e65 7720 3e20 6f6c 643a 0a20 2020  f new > old:.   
-0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f990: 2063 6861 6e67 655f 6368 6172 203d 2027   change_char = '
-0000f9a0: e286 9127 0a20 2020 2020 2020 2020 2020  ...'.           
-0000f9b0: 2020 2020 2065 6c69 6620 6e65 7720 3c20       elif new < 
-0000f9c0: 6f6c 643a 0a20 2020 2020 2020 2020 2020  old:.           
-0000f9d0: 2020 2020 2020 2020 2063 6861 6e67 655f           change_
-0000f9e0: 6368 6172 203d 2027 e286 9327 0a20 2020  char = '...'.   
-0000f9f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000fa00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000fa10: 2020 2020 2020 2065 7272 6f72 6d73 6720         errormsg 
-0000fa20: 3d20 6627 436f 756c 6420 6e6f 7420 6465  = f'Could not de
-0000fa30: 7465 726d 696e 6520 7265 6c61 7469 6f6e  termine relation
-0000fa40: 7368 6970 2062 6574 7765 656e 2073 696d  ship between sim
-0000fa50: 313d 7b6f 6c64 7d20 616e 6420 7369 6d32  1={old} and sim2
-0000fa60: 3d7b 6e65 777d 270a 2020 2020 2020 2020  ={new}'.        
-0000fa70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000fa80: 6520 5661 6c75 6545 7272 6f72 2865 7272  e ValueError(err
-0000fa90: 6f72 6d73 6729 0a0a 2020 2020 2020 2020  ormsg)..        
-0000faa0: 2020 2020 2020 2020 2320 5365 7420 686f          # Set ho
-0000fab0: 7720 6d61 6e79 2072 6570 6561 7473 2069  w many repeats i
-0000fac0: 7420 7368 6f75 6c64 2068 6176 650a 2020  t should have.  
-0000fad0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000fae0: 7065 6174 7320 3d20 310a 2020 2020 2020  peats = 1.      
-0000faf0: 2020 2020 2020 2020 2020 6966 2061 6273            if abs
-0000fb00: 5f72 6174 696f 203e 3d20 312e 313a 0a20  _ratio >= 1.1:. 
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 2020 2072 6570 6561 7473 203d 2032 0a20     repeats = 2. 
-0000fb30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fb40: 6620 6162 735f 7261 7469 6f20 3e3d 2032  f abs_ratio >= 2
-0000fb50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fb60: 2020 2020 2020 7265 7065 6174 7320 3d20        repeats = 
-0000fb70: 330a 2020 2020 2020 2020 2020 2020 2020  3.              
-0000fb80: 2020 6966 2061 6273 5f72 6174 696f 203e    if abs_ratio >
-0000fb90: 3d20 3130 3a0a 2020 2020 2020 2020 2020  = 10:.          
-0000fba0: 2020 2020 2020 2020 2020 7265 7065 6174            repeat
-0000fbb0: 7320 3d20 340a 0a20 2020 2020 2020 2020  s = 4..         
-0000fbc0: 2020 2020 2020 2074 6869 735f 6368 616e         this_chan
-0000fbd0: 6765 203d 2063 6861 6e67 655f 6368 6172  ge = change_char
-0000fbe0: 2a72 6570 6561 7473 0a20 2020 2020 2020  *repeats.       
-0000fbf0: 2020 2020 2065 6c73 653a 2023 2070 7261       else: # pra
-0000fc00: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-0000fc10: 2020 2020 2020 2020 2020 2020 2020 7468                th
-0000fc20: 6973 5f64 6966 6620 2020 3d20 6e70 2e6e  is_diff   = np.n
-0000fc30: 616e 0a20 2020 2020 2020 2020 2020 2020  an.             
-0000fc40: 2020 2074 6869 735f 7261 7469 6f20 203d     this_ratio  =
-0000fc50: 206e 702e 6e61 6e0a 2020 2020 2020 2020   np.nan.        
-0000fc60: 2020 2020 2020 2020 7468 6973 5f63 6861          this_cha
-0000fc70: 6e67 6520 3d20 274e 2f41 270a 0a20 2020  nge = 'N/A'..   
-0000fc80: 2020 2020 2020 2020 2064 6966 662e 6170           diff.ap
-0000fc90: 7065 6e64 2874 6869 735f 6469 6666 290a  pend(this_diff).
-0000fca0: 2020 2020 2020 2020 2020 2020 7261 7469              rati
-0000fcb0: 6f2e 6170 7065 6e64 2874 6869 735f 7261  o.append(this_ra
-0000fcc0: 7469 6f29 0a20 2020 2020 2020 2020 2020  tio).           
-0000fcd0: 2063 6861 6e67 652e 6170 7065 6e64 2874   change.append(t
-0000fce0: 6869 735f 6368 616e 6765 290a 0a20 2020  his_change)..   
-0000fcf0: 2020 2020 2064 665b 2764 6966 6627 5d20       df['diff'] 
-0000fd00: 3d20 6469 6666 0a20 2020 2020 2020 2064  = diff.        d
-0000fd10: 665b 2772 6174 696f 275d 203d 2072 6174  f['ratio'] = rat
-0000fd20: 696f 0a20 2020 2020 2020 2066 6f72 2063  io.        for c
-0000fd30: 6f6c 2069 6e20 5b27 7369 6d31 272c 2027  ol in ['sim1', '
-0000fd40: 7369 6d32 272c 2027 6469 6666 272c 2027  sim2', 'diff', '
-0000fd50: 7261 7469 6f27 5d3a 0a20 2020 2020 2020  ratio']:.       
-0000fd60: 2020 2020 2064 665b 636f 6c5d 203d 2064       df[col] = d
-0000fd70: 665b 636f 6c5d 2e72 6f75 6e64 2864 6563  f[col].round(dec
-0000fd80: 696d 616c 733d 3329 0a20 2020 2020 2020  imals=3).       
-0000fd90: 2064 665b 2763 6861 6e67 6527 5d20 3d20   df['change'] = 
-0000fda0: 6368 616e 6765 0a20 2020 2020 2020 2076  change.        v
-0000fdb0: 616c 6d61 7463 686d 7367 202b 3d20 7374  almatchmsg += st
-0000fdc0: 7228 6466 290a 0a20 2020 2023 2052 6169  r(df)..    # Rai
-0000fdd0: 7365 2061 6e20 6572 726f 7220 6966 206d  se an error if m
-0000fde0: 6973 6d61 7463 6865 7320 7765 7265 2066  ismatches were f
-0000fdf0: 6f75 6e64 0a20 2020 206d 6973 6d61 7463  ound.    mismatc
-0000fe00: 686d 7367 203d 206b 6579 6d61 7463 686d  hmsg = keymatchm
-0000fe10: 7367 202b 2076 616c 6d61 7463 686d 7367  sg + valmatchmsg
-0000fe20: 0a20 2020 2069 6620 6d69 736d 6174 6368  .    if mismatch
-0000fe30: 6d73 673a 2023 2070 7261 676d 613a 206e  msg: # pragma: n
-0000fe40: 6f20 636f 7665 720a 2020 2020 2020 2020  o cover.        
-0000fe50: 6966 2064 6965 3a0a 2020 2020 2020 2020  if die:.        
-0000fe60: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000fe70: 7272 6f72 286d 6973 6d61 7463 686d 7367  rror(mismatchmsg
-0000fe80: 290a 2020 2020 2020 2020 656c 6966 206f  ).        elif o
-0000fe90: 7574 7075 743a 0a20 2020 2020 2020 2020  utput:.         
-0000fea0: 2020 2072 6574 7572 6e20 6d69 736d 6174     return mismat
-0000feb0: 6368 6d73 670a 2020 2020 2020 2020 656c  chmsg.        el
-0000fec0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000fed0: 7072 696e 7428 6d69 736d 6174 6368 6d73  print(mismatchms
-0000fee0: 6729 0a20 2020 2065 6c73 653a 0a20 2020  g).    else:.   
-0000fef0: 2020 2020 2069 6620 6e6f 7420 6f75 7470       if not outp
-0000ff00: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
-0000ff10: 7072 696e 7428 2753 696d 7320 6d61 7463  print('Sims matc
-0000ff20: 6827 290a 2020 2020 7265 7475 726e 0a    h').    return.
+0000dd60: 6c74 735b 2763 616e 6365 725f 696e 6369  lts['cancer_inci
+0000dd70: 6465 6e63 6527 5d5b 3a5d 2020 2020 2020  dence'][:]      
+0000dd80: 2020 2020 2020 203d 2072 6573 5b27 6361         = res['ca
+0000dd90: 6e63 6572 7327 5d5b 3a5d 202f 2064 656d  ncers'][:] / dem
+0000dda0: 6f6e 696e 6174 6f72 0a20 2020 2020 2020  oninator.       
+0000ddb0: 2073 656c 662e 7265 7375 6c74 735b 2763   self.results['c
+0000ddc0: 616e 6365 725f 696e 6369 6465 6e63 655f  ancer_incidence_
+0000ddd0: 6279 5f67 656e 6f74 7970 6527 5d5b 3a5d  by_genotype'][:]
+0000dde0: 203d 2072 6573 5b27 6361 6e63 6572 735f   = res['cancers_
+0000ddf0: 6279 5f67 656e 6f74 7970 6527 5d5b 3a5d  by_genotype'][:]
+0000de00: 202f 2064 656d 6f6e 696e 6174 6f72 0a20   / demoninator. 
+0000de10: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
+0000de20: 6c74 735b 2763 616e 6365 725f 696e 6369  lts['cancer_inci
+0000de30: 6465 6e63 655f 6279 5f61 6765 275d 5b3a  dence_by_age'][:
+0000de40: 5d20 2020 2020 203d 2073 6166 6564 6976  ]      = safediv
+0000de50: 6964 6528 7265 735b 2763 616e 6365 7273  ide(res['cancers
+0000de60: 5f62 795f 6167 6527 5d5b 3a5d 2c20 7265  _by_age'][:], re
+0000de70: 735b 276e 5f66 656d 616c 6573 5f61 6c69  s['n_females_ali
+0000de80: 7665 5f62 795f 6167 6527 5d5b 3a5d 2f73  ve_by_age'][:]/s
+0000de90: 6361 6c65 5f66 6163 746f 7229 0a0a 2020  cale_factor)..  
+0000dea0: 2020 2020 2020 2320 436f 6d70 7574 6520        # Compute 
+0000deb0: 6361 6e63 6572 206d 6f72 7461 6c69 7479  cancer mortality
+0000dec0: 2e20 4465 6e6f 6d69 6e61 746f 7220 6973  . Denominator is
+0000ded0: 2061 6c6c 2077 6f6d 656e 2061 6c69 7665   all women alive
+0000dee0: 0a20 2020 2020 2020 2064 656e 6f6d 696e  .        denomin
+0000def0: 6174 6f72 203d 2061 6c69 7665 5f66 656d  ator = alive_fem
+0000df00: 616c 6573 2f73 6361 6c65 5f66 6163 746f  ales/scale_facto
+0000df10: 720a 2020 2020 2020 2020 7365 6c66 2e72  r.        self.r
+0000df20: 6573 756c 7473 5b27 6361 6e63 6572 5f6d  esults['cancer_m
+0000df30: 6f72 7461 6c69 7479 275d 5b3a 5d20 2020  ortality'][:]   
+0000df40: 2020 2020 2020 3d20 7265 735b 2763 616e        = res['can
+0000df50: 6365 725f 6465 6174 6873 275d 5b3a 5d2f  cer_deaths'][:]/
+0000df60: 6465 6e6f 6d69 6e61 746f 720a 0a20 2020  denominator..   
+0000df70: 2020 2020 2023 2043 6f6d 7075 7465 2048       # Compute H
+0000df80: 5056 2074 7970 6520 6469 7374 7269 6275  PV type distribu
+0000df90: 7469 6f6e 2062 7920 6379 746f 6c6f 6779  tion by cytology
+0000dfa0: 0a20 2020 2020 2020 2066 6f72 2077 6869  .        for whi
+0000dfb0: 6368 2069 6e20 6870 642e 7479 7065 5f64  ch in hpd.type_d
+0000dfc0: 6973 745f 6b65 7973 3a0a 2020 2020 2020  ist_keys:.      
+0000dfd0: 2020 2020 2020 6279 5f74 7970 6520 3d20        by_type = 
+0000dfe0: 7265 735b 6627 6e5f 7b77 6869 6368 7d5f  res[f'n_{which}_
+0000dff0: 6279 5f67 656e 6f74 7970 6527 5d5b 3a5d  by_genotype'][:]
+0000e000: 0a20 2020 2020 2020 2020 2020 2074 6f74  .            tot
+0000e010: 616c 7320 3d20 6279 5f74 7970 652e 7375  als = by_type.su
+0000e020: 6d28 6178 6973 3d30 290a 2020 2020 2020  m(axis=0).      
+0000e030: 2020 2020 2020 696e 6473 5f74 6f5f 6669        inds_to_fi
+0000e040: 6c6c 203d 2074 6f74 616c 7320 3e20 300a  ll = totals > 0.
+0000e050: 2020 2020 2020 2020 2020 2020 7265 735b              res[
+0000e060: 7768 6963 6820 2b20 275f 6765 6e6f 7479  which + '_genoty
+0000e070: 7065 5f64 6973 7427 5d5b 3a2c 2069 6e64  pe_dist'][:, ind
+0000e080: 735f 746f 5f66 696c 6c5d 203d 2062 795f  s_to_fill] = by_
+0000e090: 7479 7065 5b3a 2c20 696e 6473 5f74 6f5f  type[:, inds_to_
+0000e0a0: 6669 6c6c 5d20 2f20 746f 7461 6c73 5b69  fill] / totals[i
+0000e0b0: 6e64 735f 746f 5f66 696c 6c5d 0a0a 2020  nds_to_fill]..  
+0000e0c0: 2020 2020 2020 2320 4465 6d6f 6772 6170        # Demograp
+0000e0d0: 6869 6320 7265 7375 6c74 730a 2020 2020  hic results.    
+0000e0e0: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
+0000e0f0: 5b27 6364 7227 5d5b 3a5d 2020 3d20 7365  ['cdr'][:]  = se
+0000e100: 6c66 2e72 6573 756c 7473 5b27 6f74 6865  lf.results['othe
+0000e110: 725f 6465 6174 6873 275d 5b3a 5d20 2f20  r_deaths'][:] / 
+0000e120: 2873 656c 662e 7265 7375 6c74 735b 276e  (self.results['n
+0000e130: 5f61 6c69 7665 275d 5b3a 5d29 0a20 2020  _alive'][:]).   
+0000e140: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+0000e150: 735b 2763 6272 275d 5b3a 5d20 203d 2073  s['cbr'][:]  = s
+0000e160: 656c 662e 7265 7375 6c74 735b 2762 6972  elf.results['bir
+0000e170: 7468 7327 5d5b 3a5d 202f 2028 7365 6c66  ths'][:] / (self
+0000e180: 2e72 6573 756c 7473 5b27 6e5f 616c 6976  .results['n_aliv
+0000e190: 6527 5d5b 3a5d 290a 0a20 2020 2020 2020  e'][:])..       
+0000e1a0: 2023 2056 6163 6369 6e61 7469 6f6e 2072   # Vaccination r
+0000e1b0: 6573 756c 7473 0a20 2020 2020 2020 2073  esults.        s
+0000e1c0: 656c 662e 7265 7375 6c74 735b 2763 756d  elf.results['cum
+0000e1d0: 5f76 6163 6369 6e61 7465 6427 5d5b 3a5d  _vaccinated'][:]
+0000e1e0: 203d 206e 702e 6375 6d73 756d 2873 656c   = np.cumsum(sel
+0000e1f0: 662e 7265 7375 6c74 735b 276e 6577 5f76  f.results['new_v
+0000e200: 6163 6369 6e61 7465 6427 5d5b 3a5d 2c20  accinated'][:], 
+0000e210: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+0000e220: 7365 6c66 2e72 6573 756c 7473 5b27 6375  self.results['cu
+0000e230: 6d5f 746f 7461 6c5f 7661 6363 696e 6174  m_total_vaccinat
+0000e240: 6564 275d 5b3a 5d20 3d20 6e70 2e63 756d  ed'][:] = np.cum
+0000e250: 7375 6d28 7365 6c66 2e72 6573 756c 7473  sum(self.results
+0000e260: 5b27 6e65 775f 746f 7461 6c5f 7661 6363  ['new_total_vacc
+0000e270: 696e 6174 6564 275d 5b3a 5d29 0a20 2020  inated'][:]).   
+0000e280: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+0000e290: 735b 2763 756d 5f64 6f73 6573 275d 5b3a  s['cum_doses'][:
+0000e2a0: 5d20 3d20 6e70 2e63 756d 7375 6d28 7365  ] = np.cumsum(se
+0000e2b0: 6c66 2e72 6573 756c 7473 5b27 6e65 775f  lf.results['new_
+0000e2c0: 646f 7365 7327 5d5b 3a5d 290a 0a20 2020  doses'][:])..   
+0000e2d0: 2020 2020 2023 2054 6865 7261 7065 7574       # Therapeut
+0000e2e0: 6963 2076 6163 6369 6e61 7469 6f6e 2072  ic vaccination r
+0000e2f0: 6573 756c 7473 0a20 2020 2020 2020 2073  esults.        s
+0000e300: 656c 662e 7265 7375 6c74 735b 2763 756d  elf.results['cum
+0000e310: 5f74 785f 7661 6363 696e 6174 6564 275d  _tx_vaccinated']
+0000e320: 5b3a 5d20 3d20 6e70 2e63 756d 7375 6d28  [:] = np.cumsum(
+0000e330: 7365 6c66 2e72 6573 756c 7473 5b27 6e65  self.results['ne
+0000e340: 775f 7478 5f76 6163 6369 6e61 7465 6427  w_tx_vaccinated'
+0000e350: 5d5b 3a5d 2c20 6178 6973 3d30 290a 2020  ][:], axis=0).  
+0000e360: 2020 2020 2020 7365 6c66 2e72 6573 756c        self.resul
+0000e370: 7473 5b27 6375 6d5f 7478 7678 5f64 6f73  ts['cum_txvx_dos
+0000e380: 6573 275d 5b3a 5d20 3d20 6e70 2e63 756d  es'][:] = np.cum
+0000e390: 7375 6d28 7365 6c66 2e72 6573 756c 7473  sum(self.results
+0000e3a0: 5b27 6e65 775f 7478 7678 5f64 6f73 6573  ['new_txvx_doses
+0000e3b0: 275d 5b3a 5d29 0a0a 2020 2020 2020 2020  '][:])..        
+0000e3c0: 2320 5363 7265 656e 2026 2074 7265 6174  # Screen & treat
+0000e3d0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+0000e3e0: 2073 656c 662e 7265 7375 6c74 735b 2763   self.results['c
+0000e3f0: 756d 5f73 6372 6565 6e73 275d 5b3a 5d20  um_screens'][:] 
+0000e400: 3d20 6e70 2e63 756d 7375 6d28 7365 6c66  = np.cumsum(self
+0000e410: 2e72 6573 756c 7473 5b27 6e65 775f 7363  .results['new_sc
+0000e420: 7265 656e 7327 5d5b 3a5d 2c20 6178 6973  reens'][:], axis
+0000e430: 3d30 290a 2020 2020 2020 2020 7365 6c66  =0).        self
+0000e440: 2e72 6573 756c 7473 5b27 6375 6d5f 7363  .results['cum_sc
+0000e450: 7265 656e 6564 275d 5b3a 5d20 3d20 6e70  reened'][:] = np
+0000e460: 2e63 756d 7375 6d28 7365 6c66 2e72 6573  .cumsum(self.res
+0000e470: 756c 7473 5b27 6e65 775f 7363 7265 656e  ults['new_screen
+0000e480: 6564 275d 5b3a 5d2c 2061 7869 733d 3029  ed'][:], axis=0)
+0000e490: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0000e4a0: 7375 6c74 735b 2763 756d 5f63 696e 5f74  sults['cum_cin_t
+0000e4b0: 7265 6174 6d65 6e74 7327 5d5b 3a5d 203d  reatments'][:] =
+0000e4c0: 206e 702e 6375 6d73 756d 2873 656c 662e   np.cumsum(self.
+0000e4d0: 7265 7375 6c74 735b 276e 6577 5f63 696e  results['new_cin
+0000e4e0: 5f74 7265 6174 6d65 6e74 7327 5d5b 3a5d  _treatments'][:]
+0000e4f0: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
+0000e500: 2020 7365 6c66 2e72 6573 756c 7473 5b27    self.results['
+0000e510: 6375 6d5f 6369 6e5f 7472 6561 7465 6427  cum_cin_treated'
+0000e520: 5d5b 3a5d 203d 206e 702e 6375 6d73 756d  ][:] = np.cumsum
+0000e530: 2873 656c 662e 7265 7375 6c74 735b 276e  (self.results['n
+0000e540: 6577 5f63 696e 5f74 7265 6174 6564 275d  ew_cin_treated']
+0000e550: 5b3a 5d2c 2061 7869 733d 3029 0a20 2020  [:], axis=0).   
+0000e560: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+0000e570: 735b 2763 756d 5f63 616e 6365 725f 7472  s['cum_cancer_tr
+0000e580: 6561 746d 656e 7473 275d 5b3a 5d20 3d20  eatments'][:] = 
+0000e590: 6e70 2e63 756d 7375 6d28 7365 6c66 2e72  np.cumsum(self.r
+0000e5a0: 6573 756c 7473 5b27 6e65 775f 6361 6e63  esults['new_canc
+0000e5b0: 6572 5f74 7265 6174 6d65 6e74 7327 5d5b  er_treatments'][
+0000e5c0: 3a5d 2c20 6178 6973 3d30 290a 2020 2020  :], axis=0).    
+0000e5d0: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
+0000e5e0: 5b27 6375 6d5f 6361 6e63 6572 5f74 7265  ['cum_cancer_tre
+0000e5f0: 6174 6564 275d 5b3a 5d20 3d20 6e70 2e63  ated'][:] = np.c
+0000e600: 756d 7375 6d28 7365 6c66 2e72 6573 756c  umsum(self.resul
+0000e610: 7473 5b27 6e65 775f 6361 6e63 6572 5f74  ts['new_cancer_t
+0000e620: 7265 6174 6d65 6e74 7327 5d5b 3a5d 2c20  reatments'][:], 
+0000e630: 6178 6973 3d30 290a 0a20 2020 2020 2020  axis=0)..       
+0000e640: 2072 6574 7572 6e0a 0a0a 2020 2020 6465   return...    de
+0000e650: 6620 636f 6d70 7574 655f 7375 6d6d 6172  f compute_summar
+0000e660: 7928 7365 6c66 2c20 743d 4e6f 6e65 2c20  y(self, t=None, 
+0000e670: 7570 6461 7465 3d54 7275 652c 206f 7574  update=True, out
+0000e680: 7075 743d 4661 6c73 652c 2072 6571 7569  put=False, requi
+0000e690: 7265 5f72 756e 3d46 616c 7365 293a 0a20  re_run=False):. 
+0000e6a0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000e6b0: 2020 2043 6f6d 7075 7465 2074 6865 2073     Compute the s
+0000e6c0: 756d 6d61 7279 2064 6963 7420 616e 6420  ummary dict and 
+0000e6d0: 7374 7269 6e67 2066 6f72 2074 6865 2073  string for the s
+0000e6e0: 696d 2e20 5573 6564 2069 6e74 6572 6e61  im. Used interna
+0000e6f0: 6c6c 793b 2073 6565 0a20 2020 2020 2020  lly; see.       
+0000e700: 2073 696d 2e73 756d 6d61 7269 7a65 2829   sim.summarize()
+0000e710: 2066 6f72 2074 6865 2075 7365 7220 7665   for the user ve
+0000e720: 7273 696f 6e2e 0a0a 2020 2020 2020 2020  rsion...        
+0000e730: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0000e740: 2020 7420 2869 6e74 2f73 7472 293a 2064    t (int/str): d
+0000e750: 6179 206f 7220 6461 7465 2074 6f20 636f  ay or date to co
+0000e760: 6d70 7574 6520 7375 6d6d 6172 7920 666f  mpute summary fo
+0000e770: 7220 2862 7920 6465 6661 756c 742c 2074  r (by default, t
+0000e780: 6865 206c 6173 7420 706f 696e 7429 0a20  he last point). 
+0000e790: 2020 2020 2020 2020 2020 2075 7064 6174             updat
+0000e7a0: 6520 2862 6f6f 6c29 3a20 7768 6574 6865  e (bool): whethe
+0000e7b0: 7220 746f 2075 7064 6174 6520 7468 6520  r to update the 
+0000e7c0: 7374 6f72 6564 2073 696d 2e73 756d 6d61  stored sim.summa
+0000e7d0: 7279 0a20 2020 2020 2020 2020 2020 206f  ry.            o
+0000e7e0: 7574 7075 7420 2862 6f6f 6c29 3a20 7768  utput (bool): wh
+0000e7f0: 6574 6865 7220 746f 2072 6574 7572 6e20  ether to return 
+0000e800: 7468 6520 7375 6d6d 6172 790a 2020 2020  the summary.    
+0000e810: 2020 2020 2020 2020 7265 7175 6972 655f          require_
+0000e820: 7275 6e20 2862 6f6f 6c29 3a20 7768 6574  run (bool): whet
+0000e830: 6865 7220 746f 2072 6169 7365 2061 6e20  her to raise an 
+0000e840: 6578 6365 7074 696f 6e20 6966 2073 696d  exception if sim
+0000e850: 756c 6174 696f 6e73 2068 6176 6520 6e6f  ulations have no
+0000e860: 7420 6265 656e 2072 756e 2079 6574 0a20  t been run yet. 
+0000e870: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000e880: 2020 2069 6620 7420 6973 204e 6f6e 653a     if t is None:
+0000e890: 0a20 2020 2020 2020 2020 2020 2074 203d  .            t =
+0000e8a0: 202d 310a 0a20 2020 2020 2020 2023 2043   -1..        # C
+0000e8b0: 6f6d 7075 7465 2074 6865 2073 756d 6d61  ompute the summa
+0000e8c0: 7279 0a20 2020 2020 2020 2069 6620 7265  ry.        if re
+0000e8d0: 7175 6972 655f 7275 6e20 616e 6420 6e6f  quire_run and no
+0000e8e0: 7420 7365 6c66 2e72 6573 756c 7473 5f72  t self.results_r
+0000e8f0: 6561 6479 3a0a 2020 2020 2020 2020 2020  eady:.          
+0000e900: 2020 6572 726f 726d 7367 203d 2027 5369    errormsg = 'Si
+0000e910: 6d75 6c61 7469 6f6e 206e 6f74 2079 6574  mulation not yet
+0000e920: 2072 756e 270a 2020 2020 2020 2020 2020   run'.          
+0000e930: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
+0000e940: 7272 6f72 2865 7272 6f72 6d73 6729 0a0a  rror(errormsg)..
+0000e950: 2020 2020 2020 2020 7375 6d6d 6172 7920          summary 
+0000e960: 3d20 7363 2e6f 626a 6469 6374 2829 0a20  = sc.objdict(). 
+0000e970: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
+0000e980: 6e20 7365 6c66 2e72 6573 756c 745f 6b65  n self.result_ke
+0000e990: 7973 2827 746f 7461 6c27 293a 0a20 2020  ys('total'):.   
+0000e9a0: 2020 2020 2020 2020 2073 756d 6d61 7279           summary
+0000e9b0: 5b6b 6579 5d20 3d20 7365 6c66 2e72 6573  [key] = self.res
+0000e9c0: 756c 7473 5b6b 6579 5d5b 745d 0a0a 2020  ults[key][t]..  
+0000e9d0: 2020 2020 2020 2320 5570 6461 7465 2074        # Update t
+0000e9e0: 6865 2073 746f 7265 6420 7374 6174 650a  he stored state.
+0000e9f0: 2020 2020 2020 2020 6966 2075 7064 6174          if updat
+0000ea00: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000ea10: 656c 662e 7375 6d6d 6172 7920 3d20 7375  elf.summary = su
+0000ea20: 6d6d 6172 790a 0a20 2020 2020 2020 2023  mmary..        #
+0000ea30: 204f 7074 696f 6e61 6c6c 7920 7265 7475   Optionally retu
+0000ea40: 726e 0a20 2020 2020 2020 2069 6620 6f75  rn.        if ou
+0000ea50: 7470 7574 3a0a 2020 2020 2020 2020 2020  tput:.          
+0000ea60: 2020 7265 7475 726e 2073 756d 6d61 7279    return summary
+0000ea70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000ea80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ea90: 6e0a 0a0a 2020 2020 6465 6620 7375 6d6d  n...    def summ
+0000eaa0: 6172 697a 6528 7365 6c66 2c20 6675 6c6c  arize(self, full
+0000eab0: 3d46 616c 7365 2c20 743d 4e6f 6e65 2c20  =False, t=None, 
+0000eac0: 7365 703d 4e6f 6e65 2c20 6f75 7470 7574  sep=None, output
+0000ead0: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
+0000eae0: 2027 2727 0a20 2020 2020 2020 2050 7269   '''.        Pri
+0000eaf0: 6e74 2061 206d 6564 6975 6d2d 6c65 6e67  nt a medium-leng
+0000eb00: 7468 2073 756d 6d61 7279 206f 6620 7468  th summary of th
+0000eb10: 6520 7369 6d75 6c61 7469 6f6e 2c20 6472  e simulation, dr
+0000eb20: 6177 696e 6720 6672 6f6d 2074 6865 206c  awing from the l
+0000eb30: 6173 7420 7469 6d65 0a20 2020 2020 2020  ast time.       
+0000eb40: 2070 6f69 6e74 2069 6e20 7468 6520 7369   point in the si
+0000eb50: 6d75 6c61 7469 6f6e 2062 7920 6465 6661  mulation by defa
+0000eb60: 756c 742e 2043 616c 6c65 6420 6279 2064  ult. Called by d
+0000eb70: 6566 6175 6c74 2061 7420 7468 6520 656e  efault at the en
+0000eb80: 6420 6f66 2061 2073 696d 2072 756e 2e0a  d of a sim run..
+0000eb90: 2020 2020 2020 2020 706f 696e 7420 696e          point in
+0000eba0: 2074 6865 2073 696d 756c 6174 696f 6e20   the simulation 
+0000ebb0: 6279 2064 6566 6175 6c74 2e20 4361 6c6c  by default. Call
+0000ebc0: 6564 2062 7920 6465 6661 756c 7420 6174  ed by default at
+0000ebd0: 2074 6865 2065 6e64 206f 6620 6120 7369   the end of a si
+0000ebe0: 6d20 7275 6e2e 0a20 2020 2020 2020 2053  m run..        S
+0000ebf0: 6565 2061 6c73 6f20 7369 6d2e 6469 7370  ee also sim.disp
+0000ec00: 2829 2028 6465 7461 696c 6564 206f 7574  () (detailed out
+0000ec10: 7075 7429 2061 6e64 2073 696d 2e62 7269  put) and sim.bri
+0000ec20: 6566 2829 2028 7368 6f72 7420 6f75 7470  ef() (short outp
+0000ec30: 7574 292e 0a0a 2020 2020 2020 2020 4172  ut)...        Ar
+0000ec40: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000ec50: 6675 6c6c 2020 2028 626f 6f6c 293a 2020  full   (bool):  
+0000ec60: 2020 7768 6574 6865 7220 6f72 206e 6f74    whether or not
+0000ec70: 2074 6f20 7072 696e 7420 616c 6c20 7265   to print all re
+0000ec80: 7375 6c74 7320 2862 7920 6465 6661 756c  sults (by defaul
+0000ec90: 742c 206f 6e6c 7920 6375 6d75 6c61 7469  t, only cumulati
+0000eca0: 7665 290a 2020 2020 2020 2020 2020 2020  ve).            
+0000ecb0: 7420 2020 2020 2028 696e 742f 7374 7229  t      (int/str)
+0000ecc0: 3a20 6461 7920 6f72 2064 6174 6520 746f  : day or date to
+0000ecd0: 2063 6f6d 7075 7465 2073 756d 6d61 7279   compute summary
+0000ece0: 2066 6f72 2028 6279 2064 6566 6175 6c74   for (by default
+0000ecf0: 2c20 7468 6520 6c61 7374 2070 6f69 6e74  , the last point
+0000ed00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000ed10: 7020 2020 2028 7374 7229 3a20 2020 2020  p    (str):     
+0000ed20: 7468 6f75 7361 6e64 7320 7365 7061 7261  thousands separa
+0000ed30: 746f 7220 2864 6566 6175 6c74 2027 2c27  tor (default ','
+0000ed40: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
+0000ed50: 7470 7574 2028 626f 6f6c 293a 2020 2020  tput (bool):    
+0000ed60: 7768 6574 6865 7220 746f 2072 6574 7572  whether to retur
+0000ed70: 6e20 7468 6520 7375 6d6d 6172 7920 696e  n the summary in
+0000ed80: 7374 6561 6420 6f66 2070 7269 6e74 696e  stead of printin
+0000ed90: 6720 6974 0a0a 2020 2020 2020 2020 2a2a  g it..        **
+0000eda0: 4578 616d 706c 6573 2a2a 3a3a 0a0a 2020  Examples**::..  
+0000edb0: 2020 2020 2020 2020 2020 7369 6d20 3d20            sim = 
+0000edc0: 6870 762e 5369 6d28 6c61 6265 6c3d 2745  hpv.Sim(label='E
+0000edd0: 7861 6d70 6c65 2073 696d 272c 2076 6572  xample sim', ver
+0000ede0: 626f 7365 3d30 2920 2320 5365 7420 746f  bose=0) # Set to
+0000edf0: 2072 756e 2073 696c 656e 746c 790a 2020   run silently.  
+0000ee00: 2020 2020 2020 2020 2020 7369 6d2e 7275            sim.ru
+0000ee10: 6e28 2920 2320 5275 6e20 7468 6520 7369  n() # Run the si
+0000ee20: 6d0a 2020 2020 2020 2020 2020 2020 7369  m.            si
+0000ee30: 6d2e 7375 6d6d 6172 697a 6528 2920 2320  m.summarize() # 
+0000ee40: 5072 696e 7420 6d65 6469 756d 2d6c 656e  Print medium-len
+0000ee50: 6774 6820 7375 6d6d 6172 7920 6f66 2074  gth summary of t
+0000ee60: 6865 2073 696d 0a20 2020 2020 2020 2020  he sim.         
+0000ee70: 2020 2073 696d 2e73 756d 6d61 7269 7a65     sim.summarize
+0000ee80: 2874 3d32 342c 2066 756c 6c3d 5472 7565  (t=24, full=True
+0000ee90: 2920 2320 5072 696e 7420 6120 2273 6c69  ) # Print a "sli
+0000eea0: 6365 2220 6f66 2061 6c6c 2073 696d 2072  ce" of all sim r
+0000eeb0: 6573 756c 7473 206f 6e20 6461 7920 3234  esults on day 24
+0000eec0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+0000eed0: 2020 2020 2023 2043 6f6d 7075 7465 2074       # Compute t
+0000eee0: 6865 2073 756d 6d61 7279 0a20 2020 2020  he summary.     
+0000eef0: 2020 2073 756d 6d61 7279 203d 2073 656c     summary = sel
+0000ef00: 662e 636f 6d70 7574 655f 7375 6d6d 6172  f.compute_summar
+0000ef10: 7928 743d 742c 2075 7064 6174 653d 4661  y(t=t, update=Fa
+0000ef20: 6c73 652c 206f 7574 7075 743d 5472 7565  lse, output=True
+0000ef30: 290a 0a20 2020 2020 2020 2023 2043 6f6e  )..        # Con
+0000ef40: 7374 7275 6374 2074 6865 206f 7574 7075  struct the outpu
+0000ef50: 7420 7374 7269 6e67 0a20 2020 2020 2020  t string.       
+0000ef60: 2069 6620 7365 7020 6973 204e 6f6e 653a   if sep is None:
+0000ef70: 2073 6570 203d 2068 706f 2e73 6570 2023   sep = hpo.sep #
+0000ef80: 2044 6566 6175 6c74 2073 6570 6172 6174   Default separat
+0000ef90: 6f72 0a20 2020 2020 2020 206c 6162 656c  or.        label
+0000efa0: 7374 7220 3d20 6627 2022 7b73 656c 662e  str = f' "{self.
+0000efb0: 6c61 6265 6c7d 2227 2069 6620 7365 6c66  label}"' if self
+0000efc0: 2e6c 6162 656c 2065 6c73 6520 2727 0a20  .label else ''. 
+0000efd0: 2020 2020 2020 2073 7472 696e 6720 3d20         string = 
+0000efe0: 6627 5369 6d75 6c61 7469 6f6e 7b6c 6162  f'Simulation{lab
+0000eff0: 656c 7374 727d 2073 756d 6d61 7279 3a5c  elstr} summary:\
+0000f000: 6e27 0a20 2020 2020 2020 2066 6f72 206b  n'.        for k
+0000f010: 6579 2069 6e20 7365 6c66 2e72 6573 756c  ey in self.resul
+0000f020: 745f 6b65 7973 2827 746f 7461 6c27 293a  t_keys('total'):
+0000f030: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+0000f040: 203d 2073 756d 6d61 7279 5b6b 6579 5d0a   = summary[key].
+0000f050: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000f060: 7476 616c 203d 2066 2720 2020 7b76 616c  tval = f'   {val
+0000f070: 3a31 302c 2e30 667d 2027 0a20 2020 2020  :10,.0f} '.     
+0000f080: 2020 2020 2020 206c 6162 656c 203d 2073         label = s
+0000f090: 656c 662e 7265 7375 6c74 735b 6b65 795d  elf.results[key]
+0000f0a0: 2e6e 616d 652e 6c6f 7765 7228 292e 7265  .name.lower().re
+0000f0b0: 706c 6163 6528 272c 272c 2073 6570 290a  place(',', sep).
+0000f0c0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+0000f0d0: 696e 6369 6465 6e63 6527 2069 6e20 6b65  incidence' in ke
+0000f0e0: 7920 6f72 2027 7072 6576 616c 656e 6365  y or 'prevalence
+0000f0f0: 2720 696e 206b 6579 3a0a 2020 2020 2020  ' in key:.      
+0000f100: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+0000f110: 2069 6e20 5b27 6870 765f 7072 6576 616c   in ['hpv_preval
+0000f120: 656e 6365 272c 2027 6870 765f 696e 6369  ence', 'hpv_inci
+0000f130: 6465 6e63 6527 5d3a 0a20 2020 2020 2020  dence']:.       
+0000f140: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000f150: 6e74 7661 6c20 3d20 6627 2020 207b 7661  ntval = f'   {va
+0000f160: 6c2a 3130 303a 3130 2e32 667d 2027 0a20  l*100:10.2f} '. 
+0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f180: 2020 206c 6162 656c 202b 3d20 2720 282f     label += ' (/
+0000f190: 3130 3029 270a 2020 2020 2020 2020 2020  100)'.          
+0000f1a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1c0: 6c61 6265 6c20 2b3d 2027 2028 2f31 3030  label += ' (/100
+0000f1d0: 2c30 3030 2927 0a20 2020 2020 2020 2020  ,000)'.         
+0000f1e0: 2020 2073 7472 696e 6720 2b3d 2070 7269     string += pri
+0000f1f0: 6e74 7661 6c20 2b20 6c61 6265 6c20 2b20  ntval + label + 
+0000f200: 275c 6e27 0a0a 2020 2020 2020 2020 2320  '\n'..        # 
+0000f210: 5072 696e 7420 6f72 2072 6574 7572 6e20  Print or return 
+0000f220: 7374 7269 6e67 0a20 2020 2020 2020 2069  string.        i
+0000f230: 6620 6e6f 7420 6f75 7470 7574 3a0a 2020  f not output:.  
+0000f240: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000f250: 7374 7269 6e67 290a 2020 2020 2020 2020  string).        
+0000f260: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000f270: 2020 7265 7475 726e 2073 7472 696e 670a    return string.
+0000f280: 0a0a 2020 2020 6465 6620 706c 6f74 2873  ..    def plot(s
+0000f290: 656c 662c 202a 6172 6773 2c20 2a2a 6b77  elf, *args, **kw
+0000f2a0: 6172 6773 293a 0a20 2020 2020 2020 2027  args):.        '
+0000f2b0: 2727 0a20 2020 2020 2020 2050 6c6f 7420  ''.        Plot 
+0000f2c0: 7468 6520 6f75 7470 7574 7320 6f66 2074  the outputs of t
+0000f2d0: 6865 206d 6f64 656c 0a20 2020 2020 2020  he model.       
+0000f2e0: 2027 2727 0a20 2020 2020 2020 2066 6967   '''.        fig
+0000f2f0: 203d 2068 7070 6c74 2e70 6c6f 745f 7369   = hpplt.plot_si
+0000f300: 6d28 7369 6d3d 7365 6c66 2c20 2a61 7267  m(sim=self, *arg
+0000f310: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
+0000f320: 2020 2020 2072 6574 7572 6e20 6669 670a       return fig.
+0000f330: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+0000f340: 655f 6669 7428 7365 6c66 293a 0a20 2020  e_fit(self):.   
+0000f350: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0000f360: 2043 6f6d 7075 7465 2066 6974 2062 6574   Compute fit bet
+0000f370: 7765 656e 206d 6f64 656c 2061 6e64 2064  ween model and d
+0000f380: 6174 612e 0a20 2020 2020 2020 2027 2727  ata..        '''
+0000f390: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f3a0: 7365 6c66 2e66 6974 0a0a 0a63 6c61 7373  self.fit...class
+0000f3b0: 2041 6c72 6561 6479 5275 6e45 7272 6f72   AlreadyRunError
+0000f3c0: 2852 756e 7469 6d65 4572 726f 7229 3a0a  (RuntimeError):.
+0000f3d0: 2020 2020 2727 270a 2020 2020 5468 6973      '''.    This
+0000f3e0: 2065 7272 6f72 2069 7320 7261 6973 6564   error is raised
+0000f3f0: 2069 6620 6120 7369 6d75 6c61 7469 6f6e   if a simulation
+0000f400: 2069 7320 7275 6e20 696e 2073 7563 6820   is run in such 
+0000f410: 6120 7761 7920 7468 6174 206e 6f20 7469  a way that no ti
+0000f420: 6d65 7374 6570 730a 2020 2020 7769 6c6c  mesteps.    will
+0000f430: 2062 6520 7461 6b65 6e2e 2054 6869 7320   be taken. This 
+0000f440: 6572 726f 7220 6973 2061 2064 6973 7469  error is a disti
+0000f450: 6e63 7420 7479 7065 2073 6f20 7468 6174  nct type so that
+0000f460: 2069 7420 6361 6e20 6265 2073 6166 656c   it can be safel
+0000f470: 7920 6361 7567 6874 0a20 2020 2061 6e64  y caught.    and
+0000f480: 2069 676e 6f72 6564 2069 6620 7265 7175   ignored if requ
+0000f490: 6972 6564 2c20 6275 7420 6974 2069 7320  ired, but it is 
+0000f4a0: 616e 7469 6369 7061 7465 6420 7468 6174  anticipated that
+0000f4b0: 206d 6f73 7420 6f66 2074 6865 2074 696d   most of the tim
+0000f4c0: 652c 2063 616c 6c69 6e67 0a20 2020 203a  e, calling.    :
+0000f4d0: 7079 3a66 756e 633a 6053 696d 2e72 756e  py:func:`Sim.run
+0000f4e0: 6020 616e 6420 6e6f 7420 7461 6b69 6e67  ` and not taking
+0000f4f0: 2061 6e79 2074 696d 6573 7465 7073 2c20   any timesteps, 
+0000f500: 776f 756c 6420 6265 2061 6e20 696e 6164  would be an inad
+0000f510: 7665 7274 656e 7420 6572 726f 722e 0a20  vertent error.. 
+0000f520: 2020 2027 2727 0a20 2020 2070 6173 730a     '''.    pass.
+0000f530: 0a0a 6465 6620 6469 6666 5f73 696d 7328  ..def diff_sims(
+0000f540: 7369 6d31 2c20 7369 6d32 2c20 736b 6970  sim1, sim2, skip
+0000f550: 5f6b 6579 5f64 6966 6673 3d46 616c 7365  _key_diffs=False
+0000f560: 2c20 736b 6970 3d4e 6f6e 652c 206f 7574  , skip=None, out
+0000f570: 7075 743d 4661 6c73 652c 2064 6965 3d46  put=False, die=F
+0000f580: 616c 7365 293a 0a20 2020 2027 2727 0a20  alse):.    '''. 
+0000f590: 2020 2043 6f6d 7075 7465 2074 6865 2064     Compute the d
+0000f5a0: 6966 6665 7265 6e63 6520 6f66 2074 6865  ifference of the
+0000f5b0: 2073 756d 6d61 7269 6573 206f 6620 7477   summaries of tw
+0000f5c0: 6f20 7369 6d75 6c61 7469 6f6e 732c 2061  o simulations, a
+0000f5d0: 6e64 2070 7269 6e74 2061 6e79 0a20 2020  nd print any.   
+0000f5e0: 2076 616c 7565 7320 7768 6963 6820 6469   values which di
+0000f5f0: 6666 6572 2e0a 0a20 2020 2041 7267 733a  ffer...    Args:
+0000f600: 0a20 2020 2020 2020 2073 696d 3120 2873  .        sim1 (s
+0000f610: 696d 2f64 6963 7429 3a20 6569 7468 6572  im/dict): either
+0000f620: 2061 2073 696d 756c 6174 696f 6e20 6f62   a simulation ob
+0000f630: 6a65 6374 206f 7220 7468 6520 7369 6d2e  ject or the sim.
+0000f640: 7375 6d6d 6172 7920 6469 6374 696f 6e61  summary dictiona
+0000f650: 7279 0a20 2020 2020 2020 2073 696d 3220  ry.        sim2 
+0000f660: 2873 696d 2f64 6963 7429 3a20 6469 7474  (sim/dict): ditt
+0000f670: 6f0a 2020 2020 2020 2020 736b 6970 5f6b  o.        skip_k
+0000f680: 6579 5f64 6966 6673 2028 626f 6f6c 293a  ey_diffs (bool):
+0000f690: 2077 6865 7468 6572 2074 6f20 736b 6970   whether to skip
+0000f6a0: 206b 6579 7320 7468 6174 2064 6f6e 2774   keys that don't
+0000f6b0: 206d 6174 6368 2062 6574 7765 656e 2073   match between s
+0000f6c0: 696d 730a 2020 2020 2020 2020 736b 6970  ims.        skip
+0000f6d0: 2028 6c69 7374 293a 2061 206c 6973 7420   (list): a list 
+0000f6e0: 6f66 2076 616c 7565 7320 746f 2073 6b69  of values to ski
+0000f6f0: 700a 2020 2020 2020 2020 6f75 7470 7574  p.        output
+0000f700: 2028 626f 6f6c 293a 2077 6865 7468 6572   (bool): whether
+0000f710: 2074 6f20 7265 7475 726e 2074 6865 206f   to return the o
+0000f720: 7574 7075 7420 6173 2061 2073 7472 696e  utput as a strin
+0000f730: 6720 286f 7468 6572 7769 7365 2070 7269  g (otherwise pri
+0000f740: 6e74 290a 2020 2020 2020 2020 6469 6520  nt).        die 
+0000f750: 2862 6f6f 6c29 3a20 7768 6574 6865 7220  (bool): whether 
+0000f760: 746f 2072 6169 7365 2061 6e20 6578 6365  to raise an exce
+0000f770: 7074 696f 6e20 6966 2074 6865 2073 696d  ption if the sim
+0000f780: 7320 646f 6e27 7420 6d61 7463 680a 2020  s don't match.  
+0000f790: 2020 2020 2020 7265 7175 6972 655f 7275        require_ru
+0000f7a0: 6e20 2862 6f6f 6c29 3a20 7265 7175 6972  n (bool): requir
+0000f7b0: 6520 7468 6174 2074 6865 2073 696d 756c  e that the simul
+0000f7c0: 6174 696f 6e73 2068 6176 6520 6265 656e  ations have been
+0000f7d0: 2072 756e 0a0a 2020 2020 2a2a 4578 616d   run..    **Exam
+0000f7e0: 706c 652a 2a3a 3a0a 0a20 2020 2020 2020  ple**::..       
+0000f7f0: 2073 3120 3d20 6870 762e 5369 6d28 7261   s1 = hpv.Sim(ra
+0000f800: 6e64 5f73 6565 643d 3129 2e72 756e 2829  nd_seed=1).run()
+0000f810: 0a20 2020 2020 2020 2073 3220 3d20 6870  .        s2 = hp
+0000f820: 762e 5369 6d28 7261 6e64 5f73 6565 643d  v.Sim(rand_seed=
+0000f830: 3229 2e72 756e 2829 0a20 2020 2020 2020  2).run().       
+0000f840: 2068 7076 2e64 6966 665f 7369 6d73 2873   hpv.diff_sims(s
+0000f850: 312c 2073 3229 0a20 2020 2027 2727 0a0a  1, s2).    '''..
+0000f860: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000f870: 6528 7369 6d31 2c20 5369 6d29 3a0a 2020  e(sim1, Sim):.  
+0000f880: 2020 2020 2020 7369 6d31 203d 2073 696d        sim1 = sim
+0000f890: 312e 636f 6d70 7574 655f 7375 6d6d 6172  1.compute_summar
+0000f8a0: 7928 7570 6461 7465 3d46 616c 7365 2c20  y(update=False, 
+0000f8b0: 6f75 7470 7574 3d54 7275 652c 2072 6571  output=True, req
+0000f8c0: 7569 7265 5f72 756e 3d54 7275 6529 0a20  uire_run=True). 
+0000f8d0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000f8e0: 2873 696d 322c 2053 696d 293a 0a20 2020  (sim2, Sim):.   
+0000f8f0: 2020 2020 2073 696d 3220 3d20 7369 6d32       sim2 = sim2
+0000f900: 2e63 6f6d 7075 7465 5f73 756d 6d61 7279  .compute_summary
+0000f910: 2875 7064 6174 653d 4661 6c73 652c 206f  (update=False, o
+0000f920: 7574 7075 743d 5472 7565 2c20 7265 7175  utput=True, requ
+0000f930: 6972 655f 7275 6e3d 5472 7565 290a 2020  ire_run=True).  
+0000f940: 2020 666f 7220 7369 6d20 696e 205b 7369    for sim in [si
+0000f950: 6d31 2c20 7369 6d32 5d3a 0a20 2020 2020  m1, sim2]:.     
+0000f960: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+0000f970: 616e 6365 2873 696d 2c20 6469 6374 293a  ance(sim, dict):
+0000f980: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+0000f990: 7665 720a 2020 2020 2020 2020 2020 2020  ver.            
+0000f9a0: 6572 726f 726d 7367 203d 2066 2743 616e  errormsg = f'Can
+0000f9b0: 6e6f 7420 636f 6d70 6172 6520 6f62 6a65  not compare obje
+0000f9c0: 6374 206f 6620 7479 7065 207b 7479 7065  ct of type {type
+0000f9d0: 2873 696d 297d 2c20 6d75 7374 2062 6520  (sim)}, must be 
+0000f9e0: 6120 7369 6d20 6f72 2061 2073 696d 2e73  a sim or a sim.s
+0000f9f0: 756d 6d61 7279 2064 6963 7427 0a20 2020  ummary dict'.   
+0000fa00: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+0000fa10: 7970 6545 7272 6f72 2865 7272 6f72 6d73  ypeError(errorms
+0000fa20: 6729 0a0a 2020 2020 2320 436f 6d70 6172  g)..    # Compar
+0000fa30: 6520 6b65 7973 0a20 2020 206b 6579 6d61  e keys.    keyma
+0000fa40: 7463 686d 7367 203d 2027 270a 2020 2020  tchmsg = ''.    
+0000fa50: 7369 6d31 5f6b 6579 7320 3d20 7365 7428  sim1_keys = set(
+0000fa60: 7369 6d31 2e6b 6579 7328 2929 0a20 2020  sim1.keys()).   
+0000fa70: 2073 696d 325f 6b65 7973 203d 2073 6574   sim2_keys = set
+0000fa80: 2873 696d 322e 6b65 7973 2829 290a 2020  (sim2.keys()).  
+0000fa90: 2020 6966 2073 696d 315f 6b65 7973 2021    if sim1_keys !
+0000faa0: 3d20 7369 6d32 5f6b 6579 7320 616e 6420  = sim2_keys and 
+0000fab0: 6e6f 7420 736b 6970 5f6b 6579 5f64 6966  not skip_key_dif
+0000fac0: 6673 3a20 2320 7072 6167 6d61 3a20 6e6f  fs: # pragma: no
+0000fad0: 2063 6f76 6572 0a20 2020 2020 2020 206b   cover.        k
+0000fae0: 6579 6d61 7463 686d 7367 203d 2022 4b65  eymatchmsg = "Ke
+0000faf0: 7973 2064 6f6e 2774 206d 6174 6368 215c  ys don't match!\
+0000fb00: 6e22 0a20 2020 2020 2020 206d 6973 7369  n".        missi
+0000fb10: 6e67 203d 206c 6973 7428 7369 6d31 5f6b  ng = list(sim1_k
+0000fb20: 6579 7320 2d20 7369 6d32 5f6b 6579 7329  eys - sim2_keys)
+0000fb30: 0a20 2020 2020 2020 2065 7874 7261 2020  .        extra  
+0000fb40: 203d 206c 6973 7428 7369 6d32 5f6b 6579   = list(sim2_key
+0000fb50: 7320 2d20 7369 6d31 5f6b 6579 7329 0a20  s - sim1_keys). 
+0000fb60: 2020 2020 2020 2069 6620 6d69 7373 696e         if missin
+0000fb70: 673a 0a20 2020 2020 2020 2020 2020 206b  g:.            k
+0000fb80: 6579 6d61 7463 686d 7367 202b 3d20 6627  eymatchmsg += f'
+0000fb90: 2020 4d69 7373 696e 6720 7369 6d31 206b    Missing sim1 k
+0000fba0: 6579 733a 207b 6d69 7373 696e 677d 5c6e  eys: {missing}\n
+0000fbb0: 7327 0a20 2020 2020 2020 2069 6620 6578  s'.        if ex
+0000fbc0: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+0000fbd0: 206b 6579 6d61 7463 686d 7367 202b 3d20   keymatchmsg += 
+0000fbe0: 6627 2020 4578 7472 6120 7369 6d32 206b  f'  Extra sim2 k
+0000fbf0: 6579 733a 207b 6578 7472 617d 5c6e 270a  eys: {extra}\n'.
+0000fc00: 0a20 2020 2023 2043 6f6d 7061 7265 2076  .    # Compare v
+0000fc10: 616c 7565 730a 2020 2020 7661 6c6d 6174  alues.    valmat
+0000fc20: 6368 6d73 6720 3d20 2727 0a20 2020 206d  chmsg = ''.    m
+0000fc30: 6973 6d61 7463 6865 7320 3d20 7b7d 0a20  ismatches = {}. 
+0000fc40: 2020 2073 6b69 7020 3d20 7363 2e74 6f6c     skip = sc.tol
+0000fc50: 6973 7428 736b 6970 290a 2020 2020 666f  ist(skip).    fo
+0000fc60: 7220 6b65 7920 696e 2073 696d 322e 6b65  r key in sim2.ke
+0000fc70: 7973 2829 3a20 2320 546f 2065 6e73 7572  ys(): # To ensur
+0000fc80: 6520 6f72 6465 720a 2020 2020 2020 2020  e order.        
+0000fc90: 6966 206b 6579 2069 6e20 7369 6d31 5f6b  if key in sim1_k
+0000fca0: 6579 7320 616e 6420 6b65 7920 6e6f 7420  eys and key not 
+0000fcb0: 696e 2073 6b69 703a 2023 2049 6620 6120  in skip: # If a 
+0000fcc0: 6b65 7920 6973 206d 6973 7369 6e67 2c20  key is missing, 
+0000fcd0: 646f 6e27 7420 636f 756e 7420 6974 2061  don't count it a
+0000fce0: 7320 6120 6d69 736d 6174 6368 0a20 2020  s a mismatch.   
+0000fcf0: 2020 2020 2020 2020 2073 696d 315f 7661           sim1_va
+0000fd00: 6c20 3d20 7369 6d31 5b6b 6579 5d20 6966  l = sim1[key] if
+0000fd10: 206b 6579 2069 6e20 7369 6d31 2065 6c73   key in sim1 els
+0000fd20: 6520 276e 6f74 2070 7265 7365 6e74 270a  e 'not present'.
+0000fd30: 2020 2020 2020 2020 2020 2020 7369 6d32              sim2
+0000fd40: 5f76 616c 203d 2073 696d 325b 6b65 795d  _val = sim2[key]
+0000fd50: 2069 6620 6b65 7920 696e 2073 696d 3220   if key in sim2 
+0000fd60: 656c 7365 2027 6e6f 7420 7072 6573 656e  else 'not presen
+0000fd70: 7427 0a20 2020 2020 2020 2020 2020 2069  t'.            i
+0000fd80: 6620 6e6f 7420 6e70 2e69 7363 6c6f 7365  f not np.isclose
+0000fd90: 2873 696d 315f 7661 6c2c 2073 696d 325f  (sim1_val, sim2_
+0000fda0: 7661 6c2c 2065 7175 616c 5f6e 616e 3d54  val, equal_nan=T
+0000fdb0: 7275 6529 3a0a 2020 2020 2020 2020 2020  rue):.          
+0000fdc0: 2020 2020 2020 6d69 736d 6174 6368 6573        mismatches
+0000fdd0: 5b6b 6579 5d20 3d20 7b27 7369 6d31 273a  [key] = {'sim1':
+0000fde0: 2073 696d 315f 7661 6c2c 2027 7369 6d32   sim1_val, 'sim2
+0000fdf0: 273a 2073 696d 325f 7661 6c7d 0a0a 2020  ': sim2_val}..  
+0000fe00: 2020 6966 206c 656e 286d 6973 6d61 7463    if len(mismatc
+0000fe10: 6865 7329 3a0a 2020 2020 2020 2020 7661  hes):.        va
+0000fe20: 6c6d 6174 6368 6d73 6720 3d20 275c 6e54  lmatchmsg = '\nT
+0000fe30: 6865 2066 6f6c 6c6f 7769 6e67 2076 616c  he following val
+0000fe40: 7565 7320 6469 6666 6572 2062 6574 7765  ues differ betwe
+0000fe50: 656e 2074 6865 2074 776f 2073 696d 756c  en the two simul
+0000fe60: 6174 696f 6e73 3a5c 6e27 0a20 2020 2020  ations:\n'.     
+0000fe70: 2020 2064 6620 3d20 7064 2e44 6174 6146     df = pd.DataF
+0000fe80: 7261 6d65 2e66 726f 6d5f 6469 6374 286d  rame.from_dict(m
+0000fe90: 6973 6d61 7463 6865 7329 2e74 7261 6e73  ismatches).trans
+0000fea0: 706f 7365 2829 0a20 2020 2020 2020 2064  pose().        d
+0000feb0: 6966 6620 2020 3d20 5b5d 0a20 2020 2020  iff   = [].     
+0000fec0: 2020 2072 6174 696f 2020 3d20 5b5d 0a20     ratio  = []. 
+0000fed0: 2020 2020 2020 2063 6861 6e67 6520 3d20         change = 
+0000fee0: 5b5d 0a20 2020 2020 2020 2073 6d61 6c6c  [].        small
+0000fef0: 5f63 6861 6e67 6520 3d20 3165 2d33 2023  _change = 1e-3 #
+0000ff00: 2044 6566 696e 6520 6120 736d 616c 6c20   Define a small 
+0000ff10: 6368 616e 6765 2c20 652e 672e 2061 2072  change, e.g. a r
+0000ff20: 6f75 6e64 696e 6720 6572 726f 720a 2020  ounding error.  
+0000ff30: 2020 2020 2020 666f 7220 6d64 6963 7420        for mdict 
+0000ff40: 696e 206d 6973 6d61 7463 6865 732e 7661  in mismatches.va
+0000ff50: 6c75 6573 2829 3a0a 2020 2020 2020 2020  lues():.        
+0000ff60: 2020 2020 6f6c 6420 3d20 6d64 6963 745b      old = mdict[
+0000ff70: 2773 696d 3127 5d0a 2020 2020 2020 2020  'sim1'].        
+0000ff80: 2020 2020 6e65 7720 3d20 6d64 6963 745b      new = mdict[
+0000ff90: 2773 696d 3227 5d0a 2020 2020 2020 2020  'sim2'].        
+0000ffa0: 2020 2020 6e75 6d65 7269 6320 3d20 7363      numeric = sc
+0000ffb0: 2e69 736e 756d 6265 7228 7369 6d31 5f76  .isnumber(sim1_v
+0000ffc0: 616c 2920 616e 6420 7363 2e69 736e 756d  al) and sc.isnum
+0000ffd0: 6265 7228 7369 6d32 5f76 616c 290a 2020  ber(sim2_val).  
+0000ffe0: 2020 2020 2020 2020 2020 6966 206e 756d            if num
+0000fff0: 6572 6963 2061 6e64 206f 6c64 3e30 3a0a  eric and old>0:.
+00010000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010010: 7468 6973 5f64 6966 6620 203d 206e 6577  this_diff  = new
+00010020: 202d 206f 6c64 0a20 2020 2020 2020 2020   - old.         
+00010030: 2020 2020 2020 2074 6869 735f 7261 7469         this_rati
+00010040: 6f20 3d20 6e65 772f 6f6c 640a 2020 2020  o = new/old.    
+00010050: 2020 2020 2020 2020 2020 2020 6162 735f              abs_
+00010060: 7261 7469 6f20 203d 206d 6178 2874 6869  ratio  = max(thi
+00010070: 735f 7261 7469 6f2c 2031 2e30 2f74 6869  s_ratio, 1.0/thi
+00010080: 735f 7261 7469 6f29 0a0a 2020 2020 2020  s_ratio)..      
+00010090: 2020 2020 2020 2020 2020 2320 5365 7420            # Set 
+000100a0: 7468 6520 6368 6172 6163 7465 7220 746f  the character to
+000100b0: 2075 7365 0a20 2020 2020 2020 2020 2020   use.           
+000100c0: 2020 2020 2069 6620 6162 735f 7261 7469       if abs_rati
+000100d0: 6f3c 736d 616c 6c5f 6368 616e 6765 3a0a  o<small_change:.
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100f0: 2020 2020 6368 616e 6765 5f63 6861 7220      change_char 
+00010100: 3d20 27e2 8988 270a 2020 2020 2020 2020  = '...'.        
+00010110: 2020 2020 2020 2020 656c 6966 206e 6577          elif new
+00010120: 203e 206f 6c64 3a0a 2020 2020 2020 2020   > old:.        
+00010130: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+00010140: 6765 5f63 6861 7220 3d20 27e2 8691 270a  ge_char = '...'.
+00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010160: 656c 6966 206e 6577 203c 206f 6c64 3a0a  elif new < old:.
+00010170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010180: 2020 2020 6368 616e 6765 5f63 6861 7220      change_char 
+00010190: 3d20 27e2 8693 270a 2020 2020 2020 2020  = '...'.        
+000101a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000101b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101c0: 2020 6572 726f 726d 7367 203d 2066 2743    errormsg = f'C
+000101d0: 6f75 6c64 206e 6f74 2064 6574 6572 6d69  ould not determi
+000101e0: 6e65 2072 656c 6174 696f 6e73 6869 7020  ne relationship 
+000101f0: 6265 7477 6565 6e20 7369 6d31 3d7b 6f6c  between sim1={ol
+00010200: 647d 2061 6e64 2073 696d 323d 7b6e 6577  d} and sim2={new
+00010210: 7d27 0a20 2020 2020 2020 2020 2020 2020  }'.             
+00010220: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00010230: 7565 4572 726f 7228 6572 726f 726d 7367  ueError(errormsg
+00010240: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010250: 2020 2023 2053 6574 2068 6f77 206d 616e     # Set how man
+00010260: 7920 7265 7065 6174 7320 6974 2073 686f  y repeats it sho
+00010270: 756c 6420 6861 7665 0a20 2020 2020 2020  uld have.       
+00010280: 2020 2020 2020 2020 2072 6570 6561 7473           repeats
+00010290: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+000102a0: 2020 2020 2069 6620 6162 735f 7261 7469       if abs_rati
+000102b0: 6f20 3e3d 2031 2e31 3a0a 2020 2020 2020  o >= 1.1:.      
+000102c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000102d0: 7065 6174 7320 3d20 320a 2020 2020 2020  peats = 2.      
+000102e0: 2020 2020 2020 2020 2020 6966 2061 6273            if abs
+000102f0: 5f72 6174 696f 203e 3d20 323a 0a20 2020  _ratio >= 2:.   
+00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010310: 2072 6570 6561 7473 203d 2033 0a20 2020   repeats = 3.   
+00010320: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010330: 6162 735f 7261 7469 6f20 3e3d 2031 303a  abs_ratio >= 10:
+00010340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010350: 2020 2020 2072 6570 6561 7473 203d 2034       repeats = 4
+00010360: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010370: 2020 7468 6973 5f63 6861 6e67 6520 3d20    this_change = 
+00010380: 6368 616e 6765 5f63 6861 722a 7265 7065  change_char*repe
+00010390: 6174 730a 2020 2020 2020 2020 2020 2020  ats.            
+000103a0: 656c 7365 3a20 2320 7072 6167 6d61 3a20  else: # pragma: 
+000103b0: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
+000103c0: 2020 2020 2020 2020 2074 6869 735f 6469           this_di
+000103d0: 6666 2020 203d 206e 702e 6e61 6e0a 2020  ff   = np.nan.  
+000103e0: 2020 2020 2020 2020 2020 2020 2020 7468                th
+000103f0: 6973 5f72 6174 696f 2020 3d20 6e70 2e6e  is_ratio  = np.n
+00010400: 616e 0a20 2020 2020 2020 2020 2020 2020  an.             
+00010410: 2020 2074 6869 735f 6368 616e 6765 203d     this_change =
+00010420: 2027 4e2f 4127 0a0a 2020 2020 2020 2020   'N/A'..        
+00010430: 2020 2020 6469 6666 2e61 7070 656e 6428      diff.append(
+00010440: 7468 6973 5f64 6966 6629 0a20 2020 2020  this_diff).     
+00010450: 2020 2020 2020 2072 6174 696f 2e61 7070         ratio.app
+00010460: 656e 6428 7468 6973 5f72 6174 696f 290a  end(this_ratio).
+00010470: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+00010480: 6765 2e61 7070 656e 6428 7468 6973 5f63  ge.append(this_c
+00010490: 6861 6e67 6529 0a0a 2020 2020 2020 2020  hange)..        
+000104a0: 6466 5b27 6469 6666 275d 203d 2064 6966  df['diff'] = dif
+000104b0: 660a 2020 2020 2020 2020 6466 5b27 7261  f.        df['ra
+000104c0: 7469 6f27 5d20 3d20 7261 7469 6f0a 2020  tio'] = ratio.  
+000104d0: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
+000104e0: 205b 2773 696d 3127 2c20 2773 696d 3227   ['sim1', 'sim2'
+000104f0: 2c20 2764 6966 6627 2c20 2772 6174 696f  , 'diff', 'ratio
+00010500: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00010510: 6466 5b63 6f6c 5d20 3d20 6466 5b63 6f6c  df[col] = df[col
+00010520: 5d2e 726f 756e 6428 6465 6369 6d61 6c73  ].round(decimals
+00010530: 3d33 290a 2020 2020 2020 2020 6466 5b27  =3).        df['
+00010540: 6368 616e 6765 275d 203d 2063 6861 6e67  change'] = chang
+00010550: 650a 2020 2020 2020 2020 7661 6c6d 6174  e.        valmat
+00010560: 6368 6d73 6720 2b3d 2073 7472 2864 6629  chmsg += str(df)
+00010570: 0a0a 2020 2020 2320 5261 6973 6520 616e  ..    # Raise an
+00010580: 2065 7272 6f72 2069 6620 6d69 736d 6174   error if mismat
+00010590: 6368 6573 2077 6572 6520 666f 756e 640a  ches were found.
+000105a0: 2020 2020 6d69 736d 6174 6368 6d73 6720      mismatchmsg 
+000105b0: 3d20 6b65 796d 6174 6368 6d73 6720 2b20  = keymatchmsg + 
+000105c0: 7661 6c6d 6174 6368 6d73 670a 2020 2020  valmatchmsg.    
+000105d0: 6966 206d 6973 6d61 7463 686d 7367 3a20  if mismatchmsg: 
+000105e0: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+000105f0: 6572 0a20 2020 2020 2020 2069 6620 6469  er.        if di
+00010600: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00010610: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00010620: 6d69 736d 6174 6368 6d73 6729 0a20 2020  mismatchmsg).   
+00010630: 2020 2020 2065 6c69 6620 6f75 7470 7574       elif output
+00010640: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00010650: 7475 726e 206d 6973 6d61 7463 686d 7367  turn mismatchmsg
+00010660: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00010670: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00010680: 286d 6973 6d61 7463 686d 7367 290a 2020  (mismatchmsg).  
+00010690: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000106a0: 6966 206e 6f74 206f 7574 7075 743a 0a20  if not output:. 
+000106b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000106c0: 2827 5369 6d73 206d 6174 6368 2729 0a20  ('Sims match'). 
+000106d0: 2020 2072 6574 7572 6e0a                    return.
```

### Comparing `hpvsim-1.1.1/hpvsim/utils.py` & `hpvsim-1.2.0/hpvsim/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,89 +57,144 @@
         if p1[i] in inds:
             pairing_partners.add(p2[i])
         if p2[i] in inds:
             pairing_partners.add(p1[i])
     return pairing_partners
 
 
-def logf1(x, k):
+def logf1(x, k, ttc=25):
     '''
-    The concave part of a logistic function, with point of inflexion at 0,0
-    and upper asymptote at 1. Accepts 1 parameter which determines the growth rate.
-    '''
-    return (2 / (1 + np.exp(-k * x))) - 1
-
-
-def invlogf1(y, k):
-    '''
-    The inverse of the concave part of a logistic function, with point of inflexion at 0,0
-    and upper asymptote at 1. Accepts 1 parameter which determines the growth rate.
+    Logistic function passing through (0,0) and (ttc,1).
+    Accepts 1 parameter which determines the growth rate.
     '''
-    return (-1/k)*np.log(2/(y + 1) - 1)
+    return logf3(x, k, 0, 1, ttc=ttc)
 
 
-def logf2(x, x_infl, k):
+def get_asymptotes(k, x_infl, s, ttc=25):
     '''
-    Logistic function, constrained to pass through 0,0 and with upper asymptote
-    at 1. Accepts 2 parameters: growth rate and point of inflection.
+    Get upper asymptotes for logistic functions
     '''
-    l_asymp = -1/(1+np.exp(k*x_infl))
-    return l_asymp + 1/( 1 + np.exp(-k*(x-x_infl)))
-
-
-def get_asymptotes(x_infl, k, ttc=25, s=1):
-    term1 = (1 + np.exp(k*(x_infl-ttc)))**s
+    term1 = (1 + np.exp(k*(x_infl-ttc)))**s # Note, this is 1 for most parameter combinations
     term2 = (1 + np.exp(k*x_infl))**s
     u_asymp_num = term1*(1-term2)
     u_asymp_denom = term1 - term2
     u_asymp = u_asymp_num / u_asymp_denom
     l_asymp = term1 / (term1 - term2)
     return l_asymp, u_asymp
 
-def logf3(x, x_infl, k, ttc=25, s=1):
-    l_asymp, u_asymp = get_asymptotes(x_infl, k, ttc, s)
+
+def logf3(x, k, x_infl, s, ttc=25):
+    '''
+    Logistic function passing through (0,0) and (ttc,1).
+    This version is derived from the 5-parameter version here: https://www.r-bloggers.com/2019/11/five-parameters-logistic-regression/
+    However, since it's constrained to pass through 2 points, there are 3 free parameters remaining.
+    Args:
+         k: growth rate, equivalent to b in https://www.r-bloggers.com/2019/11/five-parameters-logistic-regression/
+         x_infl: a location parameter, equivalent to C in https://www.r-bloggers.com/2019/11/five-parameters-logistic-regression/
+         s: asymmetry parameter, equivalent to s in https://www.r-bloggers.com/2019/11/five-parameters-logistic-regression/
+         ttc (time to cancer): x value for which the curve passess through 1. For x values beyond this, the function returns 1
+    '''
+    l_asymp, u_asymp = get_asymptotes(k, x_infl, s, ttc)
     return np.minimum(1, l_asymp + (u_asymp-l_asymp)/(1+np.exp(k*(x_infl-x)))**s)
 
 
-def invlogf3(y, x_infl, k, ttc=25, s=1):
-    l_asymp, u_asymp = get_asymptotes(x_infl, k, ttc, s)
+def logf2(x, k, x_infl, ttc=25):
+    '''
+    Logistic function constrained to pass through (0,0) and (ttc,1).
+    This version is derived from the 5-parameter version here: https://www.r-bloggers.com/2019/11/five-parameters-logistic-regression/
+    Since it's constrained to pass through 2 points, there are 3 free parameters remaining, and this verison fixes s=1
+    Args:
+         k: growth rate, equivalent to b in https://www.r-bloggers.com/2019/11/five-parameters-logistic-regression/
+         x_infl: point of inflection, equivalent to C in https://www.r-bloggers.com/2019/11/five-parameters-logistic-regression/
+         ttc (time to cancer): x value for which the curve passess through 1. For x values beyond this, the function returns 1
+    '''
+    return logf3(x, k, x_infl, s=1, ttc=ttc)
+
+
+def invlogf3(y, k, x_infl, s, ttc=25):
+    '''
+    Inverse of logf3; see definition there for arguments
+    '''
+    l_asymp, u_asymp = get_asymptotes(k, x_infl, s, ttc)
     part1 = np.log((u_asymp-l_asymp)/(y-l_asymp))/s
     part2 = np.log(np.exp(part1)-1)
     final = 1/k * (k*x_infl - part2)
     return final
 
 
-def invlogf2(y, x_infl, k):
+def invlogf2(y, k, x_infl, ttc=25):
     '''
-    Inverse logistic function, constrained to pass through 0,0 and with upper asymptote
-    at 1. Accepts 2 parameters: growth rate and point of inflection.
+    Inverse of logf2; see definition there for arguments
     '''
-    l_asymp = -1/(1+np.exp(k*x_infl))
-    val = (1/(y - l_asymp)) - 1
-    if (val < 0).any():
-        val[true(val < 0)] = 0.001
-        # raise ValueError
-    result = (-1/k)*np.log(val) + x_infl
-    return result
+    return invlogf3(y, k, x_infl, 1, ttc=ttc)
 
 
-def transform_prob(tp,dysp):
+def invlogf1(y, k, ttc=25):
     '''
-    Returns transformation probability given % of dysplastic cells
+    The inverse of the concave part of a logistic function, with point of inflexion at 0,0
+    and upper asymptote at 1. Accepts 1 parameter which determines the growth rate.
+    '''
+    return invlogf3(y, k, 0, 1, ttc=ttc)
+
+
+def indef_int_logf2(x, k, x_infl, ttc=25):
+    '''
+    Indefinite integral of logf2; see definition there for arguments
+    '''
+    num = np.exp(-x_infl*k)*(np.exp(k*ttc)+np.exp(x_infl*k))*((np.exp(x_infl*k)+1)*np.log(np.exp(k*x)+np.exp(x_infl*k))-k*x)
+    denom = k*(np.exp(k*ttc)-1)
+    return num/denom
+
+
+def intlogf2(upper, k, x_infl, ttc=25):
+    '''
+    Integral of logf2 between 0 and the limit given by upper
     '''
+    # Find the upper limits not including the part past time to cancer
+    exceeding_ttc_inds = (upper > ttc).nonzero()
+    lims_to_find = np.minimum(ttc, upper)
 
-    return 1-np.power(1-tp, dysp*100)
+    # Take the integral
+    val_at_0 = indef_int_logf2(0, k, x_infl, ttc)
+    val_at_lim = indef_int_logf2(lims_to_find, k, x_infl, ttc)
+    integral = val_at_lim - val_at_0
 
+    # Deal with those whose duration of infection exceeds the time to cancer
+    # Note, another option would be to set their transformation probability to 1
+    excess_integral = upper[exceeding_ttc_inds] - ttc
+    integral[exceeding_ttc_inds] += excess_integral
 
-def clearance_prob(init_clearance_prob, clearance_decay, dysp):
+    return integral
+
+
+def indef_int_logf1(x, k, ttc=25):
     '''
-    Returns clearance probability given % of transformed cells
+    Indefinite integral of logf1; see definition there for arguments
     '''
+    return indef_int_logf2(x, k, 0, ttc=ttc)
+
 
-    return init_clearance_prob*(1-(1 - np.power(1 - clearance_decay, dysp * 100)))
+def intlogf1(upper, k, ttc=25):
+    '''
+    Integral of logf1 between 0 and the limit given by upper
+    '''
+    return intlogf2(x, k, 0, ttc=ttc)
+
+
+def transform_prob(tp, dysp):
+    '''
+    Returns transformation probability given dysplasia
+    Using formula for half an ellipsoid:
+        V = 1/2 * 4/3 * pi * a*b*c
+          = 2 * a*b*c
+          = 2* dysp * (dysp/2)**2, assuming that b = c = 1/2 a
+          = 1/2 * dysp**3
+    '''
+    # return 1-np.power(1-tp, ((dysp*100)**2))
+    return 1-np.power(1-tp, 0.5*((dysp*100)**3))
 
 
 #%% Sampling and seed methods
 
 __all__ += ['sample', 'get_pdf', 'set_seed']
```

### Comparing `hpvsim-1.1.1/hpvsim.egg-info/PKG-INFO` & `hpvsim-1.2.0/hpvsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpvsim
-Version: 1.1.1
+Version: 1.2.0
 Summary: HPVsim: Human Papillomavirus Simulator
 Home-page: http://hpvsim.org
 Author: Robyn Stuart, Jamie Cohen, Cliff Kerr, Romesh Abeysuriya, Mariah Boudreau, Daniel Klein, Hao Hu
 Author-email: robyn.stuart@gatesfoundation.org
 Keywords: HPV,agent-based model,simulation
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `hpvsim-1.1.1/hpvsim.egg-info/SOURCES.txt` & `hpvsim-1.2.0/hpvsim.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 hpvsim.egg-info/requires.txt
 hpvsim.egg-info/top_level.txt
 hpvsim/data/__init__.py
 hpvsim/data/get_data.py
 hpvsim/data/loaders.py
 hpvsim/data/products_dx.csv
 hpvsim/data/products_tx.csv
+hpvsim/data/products_txvx.csv
 hpvsim/data/products_vx.csv
 hpvsim/data/files/metadata.json
 hpvsim/regression/pars_v0.2.6.json
 hpvsim/regression/pars_v0.2.9.json
 hpvsim/regression/pars_v0.3.0.json
 hpvsim/regression/pars_v0.3.1.json
 tests/requirements.txt
```

### Comparing `hpvsim-1.1.1/setup.py` & `hpvsim-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,13 +38,13 @@
     classifiers=CLASSIFIERS,
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy',
         'scipy',
         'pandas>=1.4.0', 
-        'sciris>=2.0.4',
+        'sciris>=3.0.0',
         'matplotlib',
         'seaborn',
         'optuna',
     ],
-)
+)
```

