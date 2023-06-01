# Comparing `tmp/mafese-0.1.3.tar.gz` & `tmp/mafese-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.3.tar", last modified: Wed May 31 10:58:54 2023, max compression
+gzip compressed data, was "mafese-0.1.4.tar", last modified: Thu Jun  1 14:58:30 2023, max compression
```

## Comparing `mafese-0.1.3.tar` & `mafese-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-31 10:57:59.000000 mafese-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-31 10:57:59.000000 mafese-0.1.3/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 10:57:59.000000 mafese-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 10:57:59.000000 mafese-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-31 10:58:54.615399 mafese-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-05-31 10:57:59.000000 mafese-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.611399 mafese-0.1.3/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.611399 mafese-0.1.3/mafese/embedded/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/embedded/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/embedded/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-31 10:57:59.000000 mafese-0.1.3/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.611399 mafese-0.1.3/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 10:58:54.000000 mafese-0.1.3/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:58:54.615399 mafese-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-31 10:57:59.000000 mafese-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:58:54.615399 mafese-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-31 10:57:59.000000 mafese-0.1.3/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-31 10:57:59.000000 mafese-0.1.3/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-31 10:57:59.000000 mafese-0.1.3/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-01 14:57:37.000000 mafese-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 14:57:37.000000 mafese-0.1.4/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 14:57:37.000000 mafese-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 14:57:37.000000 mafese-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-01 14:58:30.515283 mafese-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-01 14:57:37.000000 mafese-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/embedded/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/embedded/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:58:30.515283 mafese-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-01 14:57:37.000000 mafese-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_wrapper.py
```

### Comparing `mafese-0.1.3/CODE_OF_CONDUCT.md` & `mafese-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/LICENSE` & `mafese-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/PKG-INFO` & `mafese-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.3
+Version: 0.1.4
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,55 +43,54 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.3-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.4-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/mafese.svg)
 [![Documentation Status](https://readthedocs.org/projects/mafese/badge/?version=latest)](https://mafese.readthedocs.io/en/latest/?badge=latest)
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
-[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/thieu1995/mafese.svg)](http://isitmaintained.com/project/thieu1995/mafese "Average time to resolve an issue")
-[![Percentage of issues still open](http://isitmaintained.com/badge/open/thieu1995/mafese.svg)](http://isitmaintained.com/project/thieu1995/mafese "Percentage of issues still open")
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
 * **Total Filter-based (Statistical-based)**: > 12 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
+* **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
 * **Total regression dataset**: >= 3 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
-* **Dependencies:** numpy, scipy, scikit-learn, pandas, matplotlib, mealpy, permetrics
+* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.3
+$ pip install mafese==0.1.4
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -112,14 +111,15 @@
         mha.py
         recursive.py
         sequential.py
     embedded/
         lasso.py
         tree.py
     filter.py
+    unsupervised.py
     utils/
         correlation.py
         data_loader.py
         encoder.py
         estimator.py
         mealpy_util.py
         transfer.py
```

### Comparing `mafese-0.1.3/README.md` & `mafese-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.3-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.4-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/mafese.svg)
 [![Documentation Status](https://readthedocs.org/projects/mafese/badge/?version=latest)](https://mafese.readthedocs.io/en/latest/?badge=latest)
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
-[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/thieu1995/mafese.svg)](http://isitmaintained.com/project/thieu1995/mafese "Average time to resolve an issue")
-[![Percentage of issues still open](http://isitmaintained.com/badge/open/thieu1995/mafese.svg)](http://isitmaintained.com/project/thieu1995/mafese "Percentage of issues still open")
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
 * **Total Filter-based (Statistical-based)**: > 12 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
+* **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
 * **Total regression dataset**: >= 3 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
-* **Dependencies:** numpy, scipy, scikit-learn, pandas, matplotlib, mealpy, permetrics
+* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.3
+$ pip install mafese==0.1.4
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -69,14 +68,15 @@
         mha.py
         recursive.py
         sequential.py
     embedded/
         lasso.py
         tree.py
     filter.py
+    unsupervised.py
     utils/
         correlation.py
         data_loader.py
         encoder.py
         estimator.py
         mealpy_util.py
         transfer.py
```

### Comparing `mafese-0.1.3/mafese/__init__.py` & `mafese-0.1.4/mafese/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 06/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 from mafese.utils.data_loader import Data, get_dataset
 from mafese.filter import FilterSelector
 from mafese.wrapper.recursive import RecursiveSelector
 from mafese.wrapper.sequential import SequentialSelector
 from mafese.wrapper.mha import MhaSelector
 from mafese.embedded.lasso import LassoSelector
 from mafese.embedded.tree import TreeSelector
+from mafese.unsupervised import UnsupervisedSelector
```

### Comparing `mafese-0.1.3/mafese/embedded/lasso.py` & `mafese-0.1.4/mafese/embedded/lasso.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/embedded/tree.py` & `mafese-0.1.4/mafese/embedded/tree.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/evaluator.py` & `mafese-0.1.4/mafese/evaluator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/filter.py` & `mafese-0.1.4/mafese/filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/selector.py` & `mafese-0.1.4/mafese/selector.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/utils/correlation.py` & `mafese-0.1.4/mafese/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/utils/data_loader.py` & `mafese-0.1.4/mafese/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/utils/encoder.py` & `mafese-0.1.4/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/utils/estimator.py` & `mafese-0.1.4/mafese/utils/estimator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/utils/mealpy_util.py` & `mafese-0.1.4/mafese/utils/mealpy_util.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/utils/transfer.py` & `mafese-0.1.4/mafese/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/utils/validator.py` & `mafese-0.1.4/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/wrapper/mha.py` & `mafese-0.1.4/mafese/wrapper/mha.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/wrapper/recursive.py` & `mafese-0.1.4/mafese/wrapper/recursive.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese/wrapper/sequential.py` & `mafese-0.1.4/mafese/wrapper/sequential.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/mafese.egg-info/PKG-INFO` & `mafese-0.1.4/mafese.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.3
+Version: 0.1.4
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,55 +43,54 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.3-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.4-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/mafese.svg)
 [![Documentation Status](https://readthedocs.org/projects/mafese/badge/?version=latest)](https://mafese.readthedocs.io/en/latest/?badge=latest)
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
-[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/thieu1995/mafese.svg)](http://isitmaintained.com/project/thieu1995/mafese "Average time to resolve an issue")
-[![Percentage of issues still open](http://isitmaintained.com/badge/open/thieu1995/mafese.svg)](http://isitmaintained.com/project/thieu1995/mafese "Percentage of issues still open")
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
 * **Total Filter-based (Statistical-based)**: > 12 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
+* **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
 * **Total regression dataset**: >= 3 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
-* **Dependencies:** numpy, scipy, scikit-learn, pandas, matplotlib, mealpy, permetrics
+* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.3
+$ pip install mafese==0.1.4
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -112,14 +111,15 @@
         mha.py
         recursive.py
         sequential.py
     embedded/
         lasso.py
         tree.py
     filter.py
+    unsupervised.py
     utils/
         correlation.py
         data_loader.py
         encoder.py
         estimator.py
         mealpy_util.py
         transfer.py
```

### Comparing `mafese-0.1.3/mafese.egg-info/SOURCES.txt` & `mafese-0.1.4/mafese.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.md
 setup.py
 mafese/__init__.py
 mafese/evaluator.py
 mafese/filter.py
 mafese/selector.py
+mafese/unsupervised.py
 mafese.egg-info/PKG-INFO
 mafese.egg-info/SOURCES.txt
 mafese.egg-info/dependency_links.txt
 mafese.egg-info/requires.txt
 mafese.egg-info/top_level.txt
 mafese/embedded/__init__.py
 mafese/embedded/lasso.py
@@ -26,8 +27,9 @@
 mafese/utils/validator.py
 mafese/wrapper/__init__.py
 mafese/wrapper/mha.py
 mafese/wrapper/recursive.py
 mafese/wrapper/sequential.py
 tests/test_embedded.py
 tests/test_filter.py
+tests/test_unsupervised.py
 tests/test_wrapper.py
```

### Comparing `mafese-0.1.3/setup.py` & `mafese-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.3",
+    version="0.1.4",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
@@ -66,14 +66,14 @@
         "Topic :: Scientific/Engineering :: Visualization",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
-    install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2", "pandas>=1.3.5",
-                      "matplotlib>=3.3.0", "mealpy>=2.5.3", "permetrics>=1.3.3"],
+    install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2",
+                      "pandas>=1.3.5", "mealpy>=2.5.3", "permetrics>=1.3.3"],
     extras_require={
         "dev": ["pytest>=7.0", "pytest-cov==4.0.0", "flake8>=4.0.1"],
     },
     python_requires='>=3.7',
 )
```

### Comparing `mafese-0.1.3/tests/test_embedded.py` & `mafese-0.1.4/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.3/tests/test_filter.py` & `mafese-0.1.4/tests/test_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 from mafese.filter import FilterSelector
 
 np.random.seed(42)
 
 
-def test_Filter_class():
+def test_FilterSelector_class():
     X = np.random.rand(10, 6)
     y = np.random.randint(0, 2, size=10)
     n_features = 3
     feat_selector = FilterSelector(problem="classification", method="ANOVA", n_features=3)
     feat_selector.fit(X, y)
     X_selected = feat_selector.transform(X)
     assert X_selected.shape[1] == n_features
```

### Comparing `mafese-0.1.3/tests/test_wrapper.py` & `mafese-0.1.4/tests/test_wrapper.py`

 * *Files identical despite different names*

