# Comparing `tmp/circuitpython-mag-cal-1.1.2.tar.gz` & `tmp/circuitpython-mag-cal-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-mag-cal-1.1.2.tar", last modified: Wed May  3 12:56:53 2023, max compression
+gzip compressed data, was "circuitpython-mag-cal-1.1.3.tar", last modified: Thu Jun  1 21:20:51 2023, max compression
```

## Comparing `circuitpython-mag-cal-1.1.2.tar` & `circuitpython-mag-cal-1.1.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.272386 circuitpython-mag-cal-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.260384 circuitpython-mag-cal-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.260384 circuitpython-mag-cal-1.1.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.264385 circuitpython-mag-cal-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.264385 circuitpython-mag-cal-1.1.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-03 12:56:53.272386 circuitpython-mag-cal-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.264385 circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-03 12:56:53.000000 circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-03 12:56:53.000000 circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:56:53.000000 circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 12:56:53.000000 circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 12:56:53.000000 circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.268385 circuitpython-mag-cal-1.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.268385 circuitpython-mag-cal-1.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/howto.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.268385 circuitpython-mag-cal-1.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/examples/mag_cal_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.268385 circuitpython-mag-cal-1.1.2/mag_cal/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25232 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/nm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/rbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/mag_cal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:56:53.272386 circuitpython-mag-cal-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.268385 circuitpython-mag-cal-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.260384 circuitpython-mag-cal-1.1.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:56:53.272386 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ab.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ai.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ai.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/bh.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/bh.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/bi.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/bi.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ee.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ee.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/fb.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/fb.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/hj.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/hj.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/hj2.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/hj2.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/jd.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 12:56:32.000000 circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/jd.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-03 12:56:44.000000 circuitpython-mag-cal-1.1.2/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.181326 circuitpython-mag-cal-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.173325 circuitpython-mag-cal-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.173325 circuitpython-mag-cal-1.1.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.173325 circuitpython-mag-cal-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.173325 circuitpython-mag-cal-1.1.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-01 21:20:51.181326 circuitpython-mag-cal-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.177326 circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-01 21:20:51.000000 circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-01 21:20:51.000000 circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:20:51.000000 circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 21:20:51.000000 circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 21:20:51.000000 circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.177326 circuitpython-mag-cal-1.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.177326 circuitpython-mag-cal-1.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/howto.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.177326 circuitpython-mag-cal-1.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/examples/mag_cal_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.177326 circuitpython-mag-cal-1.1.3/mag_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/mag_cal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:20:51.181326 circuitpython-mag-cal-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.177326 circuitpython-mag-cal-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.173325 circuitpython-mag-cal-1.1.3/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:20:51.181326 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ab.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ai.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ai.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/bh.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/bh.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/bi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/bi.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ee.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ee.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/fb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/fb.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/hj.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/hj.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/hj2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/hj2.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/jd.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:20:34.000000 circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/jd.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-01 21:20:43.000000 circuitpython-mag-cal-1.1.3/tests/test_sensor.py
```

### Comparing `circuitpython-mag-cal-1.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-mag-cal-1.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/.gitignore` & `circuitpython-mag-cal-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/.pre-commit-config.yaml` & `circuitpython-mag-cal-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/.pylintrc` & `circuitpython-mag-cal-1.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/CODE_OF_CONDUCT.md` & `circuitpython-mag-cal-1.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/LICENSE` & `circuitpython-mag-cal-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/LICENSES/CC-BY-4.0.txt` & `circuitpython-mag-cal-1.1.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/LICENSES/MIT.txt` & `circuitpython-mag-cal-1.1.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/LICENSES/Unlicense.txt` & `circuitpython-mag-cal-1.1.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/PKG-INFO` & `circuitpython-mag-cal-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.1.2
+Version: 1.1.3
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.1.2/README.rst` & `circuitpython-mag-cal-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/PKG-INFO` & `circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.1.2
+Version: 1.1.3
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.1.2/circuitpython_mag_cal.egg-info/SOURCES.txt` & `circuitpython-mag-cal-1.1.3/circuitpython_mag_cal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/docs/_static/favicon.ico` & `circuitpython-mag-cal-1.1.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/docs/conf.py` & `circuitpython-mag-cal-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/docs/howto.rst` & `circuitpython-mag-cal-1.1.3/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/docs/index.rst` & `circuitpython-mag-cal-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/examples/mag_cal_simpletest.py` & `circuitpython-mag-cal-1.1.3/examples/mag_cal_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/__init__.py` & `circuitpython-mag-cal-1.1.3/mag_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/axes.py` & `circuitpython-mag-cal-1.1.3/mag_cal/axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/calibration.py` & `circuitpython-mag-cal-1.1.3/mag_cal/calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 try:
     # work with normal numpy
     import numpy as np
 except ImportError:
     # or work with ulab if we are in CircuitPython
     from ulab import numpy as np
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 __repo__ = "https://github.com/furbrain/CircuitPython_mag_cal.git"
 
 
 def _vector_from_matrices(matrix: np.ndarray, i: int, j: int):
     return np.array([x[i, j] for x in matrix])
 
 
@@ -510,14 +510,17 @@
         :param grav: numpy array of accelerometer data
         :param precision: number of degrees shots should be within
         :param min_run: minimum length of run to find
         :return: list of start and finish indices for each run
         """
         angles = [self.get_angles(m, g) for m, g in zip(mag, grav)]
         azimuths, inclinations, _ = zip(*angles)
+        azimuths = np.array(
+            azimuths
+        )  # convert to numpy array so we can do addition and modulo
         groups = []
         i = 0
         while i < len(azimuths) - min_run:
             for j in reversed(range(i + min_run, len(azimuths) + 1)):
                 if self._is_a_run(azimuths[i:j], inclinations[i:j], precision):
                     groups.append([i, j])
                     i = j
```

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/lstsq.py` & `circuitpython-mag-cal-1.1.3/mag_cal/lstsq.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/nm.py` & `circuitpython-mag-cal-1.1.3/mag_cal/nm.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/rbf.py` & `circuitpython-mag-cal-1.1.3/mag_cal/rbf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/sensor.py` & `circuitpython-mag-cal-1.1.3/mag_cal/sensor.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/mag_cal/utils.py` & `circuitpython-mag-cal-1.1.3/mag_cal/utils.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/pyproject.toml` & `circuitpython-mag-cal-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-mag-cal"
 description = "Calibrate magnetometer and accelerometer readings"
-version = "1.1.2"
+version = "1.1.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_mag_cal"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ab.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ab.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ai.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ai.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/bh.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/bh.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/bi.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/bi.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/ee.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/ee.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/fb.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/fb.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/hj.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/hj.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/hj2.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/hj2.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/fixtures/cal_data/jd.json` & `circuitpython-mag-cal-1.1.3/tests/fixtures/cal_data/jd.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/test_axes.py` & `circuitpython-mag-cal-1.1.3/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.2/tests/test_calibration.py` & `circuitpython-mag-cal-1.1.3/tests/test_calibration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: Copyright (c) 2022 Phil Underwood for Underwood Underground
 #
 # SPDX-License-Identifier: MIT
 import itertools
 import unittest
 from pathlib import Path
 from unittest import TestCase
+from unittest.mock import patch
 
 import numpy as np
 
 from mag_cal.calibration import Calibration
 from mag_cal.utils import read_fixture
 
 
@@ -103,14 +104,30 @@
         for mag, grav, _ in self.fixtures.values():
             calib = Calibration()
             calib.fit_ellipsoid(mag, grav)
             self.assertListEqual(
                 [[8, 16], [16, 24]], calib.find_similar_shots(mag, grav)
             )
 
+    def test_find_runs_near_360_azimuth(self):
+        results = [
+            (20, 0, 0),
+            (60, 0, 0),
+            (358, 0, 0),
+            (359, 0, 0),
+            (0, 0, 0),
+            (1, 0, 0),
+            (2, 0, 0),
+        ]
+        mags = [[0, 0, 0]] * 7
+        gravs = mags
+        with patch("mag_cal.calibration.Calibration.get_angles", side_effect=results):
+            calib = Calibration()
+            self.assertListEqual([[2, 7]], calib.find_similar_shots(mags, gravs))
+
     def test_integration_calibrate(self):
         for mag, grav, _ in self.fixtures.values():
             calib = Calibration()
             accuracy = calib.calibrate(mag, grav)
             self.assertGreater(0.5, accuracy)
 
     @unittest.skip
```

### Comparing `circuitpython-mag-cal-1.1.2/tests/test_sensor.py` & `circuitpython-mag-cal-1.1.3/tests/test_sensor.py`

 * *Files identical despite different names*

