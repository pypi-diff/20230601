# Comparing `tmp/vstt-0.25.0.tar.gz` & `tmp/vstt-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-0.25.0.tar", last modified: Tue May 30 12:43:24 2023, max compression
+gzip compressed data, was "vstt-0.26.0.tar", last modified: Thu Jun  1 13:11:05 2023, max compression
```

## Comparing `vstt-0.25.0.tar` & `vstt-0.26.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:43:24.657825 vstt-0.25.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-30 12:43:15.000000 vstt-0.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-30 12:43:24.657825 vstt-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-30 12:43:15.000000 vstt-0.25.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-30 12:43:15.000000 vstt-0.25.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:43:24.657825 vstt-0.25.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:43:24.653825 vstt-0.25.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:43:24.653825 vstt-0.25.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-30 12:43:15.000000 vstt-0.25.0/src/vstt/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:43:24.657825 vstt-0.25.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-30 12:43:24.000000 vstt-0.25.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-30 12:43:24.000000 vstt-0.25.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:43:24.000000 vstt-0.25.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 12:43:24.000000 vstt-0.25.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-30 12:43:24.000000 vstt-0.25.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 12:43:24.000000 vstt-0.25.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:43:24.657825 vstt-0.25.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-30 12:43:15.000000 vstt-0.25.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.591822 vstt-0.26.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-01 13:10:53.000000 vstt-0.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 13:11:05.591822 vstt-0.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-01 13:10:53.000000 vstt-0.26.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-01 13:10:53.000000 vstt-0.26.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:11:05.591822 vstt-0.26.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.587822 vstt-0.26.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.587822 vstt-0.26.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.587822 vstt-0.26.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.591822 vstt-0.26.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_vstt.py
```

### Comparing `vstt-0.25.0/LICENSE` & `vstt-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/PKG-INFO` & `vstt-0.26.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.25.0
+Version: 0.26.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
-Project-URL: Documentation, https://ssciwr.github.io/vstt/
+Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,17 +24,20 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # Visuomotor Serial Targeting Task (VSTT)
 
-[![Docs](https://readthedocs.org/projects/vstt/badge/?version=latest)](https://vstt.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/vstt.svg)](https://pypi.org/project/vstt)
+[![Docs](https://readthedocs.org/projects/vstt/badge/?version=main)](https://vstt.readthedocs.io)
 [![CI](https://github.com/ssciwr/vstt/actions/workflows/ci.yml/badge.svg)](https://github.com/ssciwr/vstt/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/ssciwr/vstt/branch/main/graph/badge.svg?token=sjsAdTyLH1)](https://codecov.io/gh/ssciwr/vstt)
+[![Sonar](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_vstt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_vstt)
 
 Visuomotor Serial Targeting Task (VSTT)
 
 Documentation: [vstt.readthedocs.io](https://vstt.readthedocs.io/)
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/gui.png)
+
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/results.png)
```

### Comparing `vstt-0.25.0/README.md` & `vstt-0.26.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Visuomotor Serial Targeting Task (VSTT)
 
-[![Docs](https://readthedocs.org/projects/vstt/badge/?version=latest)](https://vstt.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/vstt.svg)](https://pypi.org/project/vstt)
+[![Docs](https://readthedocs.org/projects/vstt/badge/?version=main)](https://vstt.readthedocs.io)
 [![CI](https://github.com/ssciwr/vstt/actions/workflows/ci.yml/badge.svg)](https://github.com/ssciwr/vstt/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/ssciwr/vstt/branch/main/graph/badge.svg?token=sjsAdTyLH1)](https://codecov.io/gh/ssciwr/vstt)
+[![Sonar](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_vstt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_vstt)
 
 Visuomotor Serial Targeting Task (VSTT)
 
 Documentation: [vstt.readthedocs.io](https://vstt.readthedocs.io/)
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/gui.png)
+
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/results.png)
```

### Comparing `vstt-0.25.0/pyproject.toml` & `vstt-0.26.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 [project.scripts]
 vstt = "vstt.__main__:main"
 
 [project.urls]
 Github = "https://github.com/ssciwr/vstt"
 Issues = "https://github.com/ssciwr/vstt/issues"
-Documentation = "https://ssciwr.github.io/vstt/"
+Documentation = "https://vstt.readthedocs.io/"
 
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-cov",
   "pytest-randomly",
   "pyautogui",
@@ -47,14 +47,15 @@
 docs = [
   "ipykernel",
   "matplotlib",
   "nbsphinx",
   "pandoc",
   "sphinx>=4.5.0",
   "sphinx_rtd_theme>=1.0.0",
+  "shapely",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "vstt.__version__" }
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `vstt-0.25.0/src/vstt/__main__.py` & `vstt-0.26.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/common.py` & `vstt-0.26.0/src/vstt/common.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/display.py` & `vstt-0.26.0/src/vstt/display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/display_widget.py` & `vstt-0.26.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/experiment.py` & `vstt-0.26.0/src/vstt/experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/geom.py` & `vstt-0.26.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/gui.py` & `vstt-0.26.0/src/vstt/gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/joystick_wrapper.py` & `vstt-0.26.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/meta.py` & `vstt-0.26.0/src/vstt/meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/meta_widget.py` & `vstt-0.26.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/results_widget.py` & `vstt-0.26.0/src/vstt/results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/stat.py` & `vstt-0.26.0/src/vstt/stat.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/task.py` & `vstt-0.26.0/src/vstt/task.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/trial.py` & `vstt-0.26.0/src/vstt/trial.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/trials_widget.py` & `vstt-0.26.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/types.py` & `vstt-0.26.0/src/vstt/types.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt/vis.py` & `vstt-0.26.0/src/vstt/vis.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/src/vstt.egg-info/PKG-INFO` & `vstt-0.26.0/src/vstt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.25.0
+Version: 0.26.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
-Project-URL: Documentation, https://ssciwr.github.io/vstt/
+Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,17 +24,20 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # Visuomotor Serial Targeting Task (VSTT)
 
-[![Docs](https://readthedocs.org/projects/vstt/badge/?version=latest)](https://vstt.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/vstt.svg)](https://pypi.org/project/vstt)
+[![Docs](https://readthedocs.org/projects/vstt/badge/?version=main)](https://vstt.readthedocs.io)
 [![CI](https://github.com/ssciwr/vstt/actions/workflows/ci.yml/badge.svg)](https://github.com/ssciwr/vstt/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/ssciwr/vstt/branch/main/graph/badge.svg?token=sjsAdTyLH1)](https://codecov.io/gh/ssciwr/vstt)
+[![Sonar](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_vstt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_vstt)
 
 Visuomotor Serial Targeting Task (VSTT)
 
 Documentation: [vstt.readthedocs.io](https://vstt.readthedocs.io/)
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/gui.png)
+
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/results.png)
```

### Comparing `vstt-0.25.0/src/vstt.egg-info/SOURCES.txt` & `vstt-0.26.0/src/vstt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_display.py` & `vstt-0.26.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_display_widget.py` & `vstt-0.26.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_experiment.py` & `vstt-0.26.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_geom.py` & `vstt-0.26.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_gui.py` & `vstt-0.26.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_joystick_wrapper.py` & `vstt-0.26.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_meta.py` & `vstt-0.26.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_meta_widget.py` & `vstt-0.26.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_results_widget.py` & `vstt-0.26.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_stat.py` & `vstt-0.26.0/tests/test_stat.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_task.py` & `vstt-0.26.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_trial.py` & `vstt-0.26.0/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_trials_widget.py` & `vstt-0.26.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.25.0/tests/test_vis.py` & `vstt-0.26.0/tests/test_vis.py`

 * *Files identical despite different names*

