# Comparing `tmp/planetmapper-1.7.1.tar.gz` & `tmp/planetmapper-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.7.1.tar", last modified: Tue May 23 15:24:52 2023, max compression
+gzip compressed data, was "planetmapper-1.7.2.tar", last modified: Thu Jun  1 14:34:34 2023, max compression
```

## Comparing `planetmapper-1.7.1.tar` & `planetmapper-1.7.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.612048 planetmapper-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-23 15:24:52.612048 planetmapper-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-23 15:24:38.000000 planetmapper-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.608048 planetmapper-1.7.1/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    80314 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   112086 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.608048 planetmapper-1.7.1/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/data/ring_aliases.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118001 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46384 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.608048 planetmapper-1.7.1/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-23 15:24:38.000000 planetmapper-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:24:52.612048 planetmapper-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-23 15:24:38.000000 planetmapper-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.612048 planetmapper-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    28382 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.386503 planetmapper-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 14:34:23.000000 planetmapper-1.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-01 14:34:34.386503 planetmapper-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-01 14:34:23.000000 planetmapper-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.382503 planetmapper-1.7.2/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28536 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80564 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112233 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.382503 planetmapper-1.7.2/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118018 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46500 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-06-01 14:34:23.000000 planetmapper-1.7.2/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.382503 planetmapper-1.7.2/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 14:34:34.000000 planetmapper-1.7.2/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-01 14:34:23.000000 planetmapper-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:34:34.386503 planetmapper-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-01 14:34:23.000000 planetmapper-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:34:34.386503 planetmapper-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34896 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39958 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28477 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-01 14:34:23.000000 planetmapper-1.7.2/tests/test_utils.py
```

### Comparing `planetmapper-1.7.1/PKG-INFO` & `planetmapper-1.7.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,42 @@
-Metadata-Version: 2.1
-Name: planetmapper
-Version: 1.7.1
-Summary: A Python module for visualising, navigating and mapping Solar System observations
-Home-page: https://github.com/ortk95/planetmapper
-Download-URL: https://pypi.org/project/planetmapper/
-Author: Oliver King
-Author-email: oliver.king95@gmail.com
-Project-URL: Documentation, https://planetmapper.readthedocs.io/
-Project-URL: GitHub, https://github.com/ortk95/planetmapper
-Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-
-# PlanetMapper
+# ![PlanetMapper logo](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/logo_wide_transparent.png)
 
 [![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
-[![Upload Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
-[![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
-[![Format](https://github.com/ortk95/planetmapper/actions/workflows/format.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/format.yml)
-[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/test.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/test.yml)
+[![Publish](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
+[![Checks](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml)
 [![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
-
-A Python module for visualising, navigating and mapping Solar System observations.
+PlanetMapper is a Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
 
 
 ## [Installation](https://planetmapper.readthedocs.io/en/latest/installation.html)
 ```
 pip install planetmapper --upgrade
 ```
 
 _Requires Python 3.10+_
 
 ## Key features
 ### [Fit and map astronomical observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
-![PlanetMapper graphical user interface](https://github.com/ortk95/planetmapper/blob/main/docs/images/gui_fitting.png?raw=true)
+[![Screenshot of the PlanetMapper graphical user interface showing an observation of Europa being navigated](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/gui_fitting.png)](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
 
 ### [Easily visualise solar system observations with just a few lines of code](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ```python
 body = planetmapper.Body('saturn', '2020-01-01')
 body.plot_wireframe_radec()
 plt.show()
 ```
 
-![Image of Saturn generated with PlanetMapper](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/saturn_wireframe_radec.png)
+[![Image of Saturn generated with PlanetMapper showing the orientation of Saturn and its rings](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/saturn_wireframe_radec.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ### [Convert coordinates, generate backplanes and project maps of telescope observations](https://planetmapper.readthedocs.io/en/latest/general_python_api.html)
-![Plot of a mapped Jupiter observation, generated with PlanetMapper](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/jupiter_mapped.png)
+[![Plot of a mapped Jupiter observation, generated with PlanetMapper, showing observed and mapped versions of the Jupiter data](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/jupiter_mapped.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html)
+
+
+## Contributing
+
+If you spot a bug, have a suggestion, or want contribute code to PlanetMapper, check out the [contributing guidelines](https://github.com/ortk95/planetmapper/blob/main/CONTRIBUTING.md)!
```

### Comparing `planetmapper-1.7.1/planetmapper/__init__.py` & `planetmapper-1.7.2/planetmapper/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -69,32 +69,56 @@
 for more information.
 
 .. warning::
 
     This code is in active development, so may contain bugs! Any issues, bugs and 
     suggestions can be 
     `reported on GitHub <https://github.com/ortk95/planetmapper/issues/new>`__.
+
+..
+    MIT License
+
+    Copyright (c) 2022 Oliver King
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+    SOFTWARE.
 """
-from . import data_loader, gui, kernel_downloader, utils
+from . import base, data_loader, gui, kernel_downloader, utils
 from .base import SpiceBase, get_kernel_path, set_kernel_path
 from .basic_body import BasicBody
 from .body import DEFAULT_WIREFRAME_FORMATTING, Body
 from .body_xy import Backplane, BodyXY
-from .common import __author__, __url__, __version__
+from .common import __author__, __description__, __license__, __url__, __version__
 from .observation import Observation
 
 __all__ = [
     'set_kernel_path',
     'get_kernel_path',
     'SpiceBase',
     'Body',
     'Backplane',
     'BodyXY',
     'Observation',
     'BasicBody',
+    'base',
     'gui',
     'utils',
     'kernel_downloader',
     'data_loader',
     'DEFAULT_WIREFRAME_FORMATTING',
 ]
```

### Comparing `planetmapper-1.7.1/planetmapper/base.py` & `planetmapper-1.7.2/planetmapper/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 import datetime
 import functools
 import glob
 import numbers
 import os
-from typing import Any, Callable, Concatenate, ParamSpec, TypeVar, cast
+from collections.abc import Iterable
+from pathlib import Path
+from typing import (
+    Any,
+    Callable,
+    Concatenate,
+    Literal,
+    ParamSpec,
+    TypeVar,
+    cast,
+    overload,
+)
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 import astropy.time
 import numpy as np
 import spiceypy as spice
+from spiceypy.utils.exceptions import SpiceyPyError
 
 from . import progress
 
 DEFAULT_KERNEL_PATH = '~/spice_kernels/'
 
 _KERNEL_DATA = {
     'kernel_path': None,
@@ -27,14 +39,22 @@
 Numeric = TypeVar('Numeric', bound=float | np.ndarray)
 
 
 T = TypeVar('T')
 S = TypeVar('S')
 P = ParamSpec('P')
 
+_SPICE_ERROR_HELP_URL = (
+    'https://planetmapper.readthedocs.io/en/latest/common_issues.html#spice-errors'
+)
+_SPICE_ERROR_HELP_TEXT = (
+    'Check your SPICE kernels are set up correctly - see the help page for more info:\n'
+    + _SPICE_ERROR_HELP_URL
+)
+
 
 def _cache_clearable_result(
     fn: Callable[Concatenate[S, P], T]
 ) -> Callable[Concatenate[S, P], T]:
     """
     Decorator to cache the output of a method call with variable arguments.
 
@@ -48,15 +68,15 @@
     stable (i.e. backplane maps) then use `_cache_stable_result` instead.
 
     Note that any numpy arguments will be converted to (nested) tuples.
     """
     # pylint: disable=protected-access
 
     @functools.wraps(fn)
-    def decorated(self, *args_in: P.args, **kwargs_in: P.kwargs):
+    def decorated(self, *args_in: P.args, **kwargs_in: P.kwargs) -> T:
         args, kwargs = _replace_np_arrr_args_with_tuples(args_in, kwargs_in)
         k = (fn.__name__, args, frozenset(kwargs.items()))
         if k not in self._cache:
             self._cache[k] = fn(self, *args, **kwargs)  # type: ignore
         return self._cache[k]
 
     return decorated
@@ -72,24 +92,55 @@
     cache self.
 
     See _cache_clearable_result for more details.
     """
 
     # pylint: disable=protected-access
     @functools.wraps(fn)
-    def decorated(self, *args_in: P.args, **kwargs_in: P.kwargs):
+    def decorated(self, *args_in: P.args, **kwargs_in: P.kwargs) -> T:
         args, kwargs = _replace_np_arrr_args_with_tuples(args_in, kwargs_in)
         k = (fn.__name__, args, frozenset(kwargs.items()))
         if k not in self._stable_cache:
             self._stable_cache[k] = fn(self, *args, **kwargs)  # type: ignore
         return self._stable_cache[k]
 
     return decorated
 
 
+def _add_help_note_to_spice_errors(fn: Callable[P, T]) -> Callable[P, T]:
+    """
+    Decorator to add help text to spice errors
+
+    This modifies the error message for specific spice errors to include PlanetMapper
+    specific help about kernel loading.
+    """
+
+    @functools.wraps(fn)
+    def decorated(*args: P.args, **kwargs: P.kwargs) -> T:
+        try:
+            return fn(*args, **kwargs)
+        except SpiceyPyError as e:
+            e.message += '\n\n' + _get_spice_error_help_note()
+            raise e
+
+    return decorated
+
+
+def _get_spice_error_help_note() -> str:
+    kernel_path, kernel_source = get_kernel_path(return_source=True)
+    return '\n'.join(
+        (
+            _SPICE_ERROR_HELP_TEXT,
+            '',
+            f'Kernel directory path: {kernel_path}',
+            f'Kernel path source: {kernel_source}',
+        )
+    )
+
+
 def _replace_np_arrr_args_with_tuples(args, kwargs) -> tuple[tuple, dict[str, Any]]:
     args = tuple(_maybe_np_arr_to_tuple(a) for a in args)
     kwargs = {k: _maybe_np_arr_to_tuple(v) for k, v in kwargs.items()}
     return args, kwargs
 
 
 def _maybe_np_arr_to_tuple(o: Any) -> Any:
@@ -102,15 +153,15 @@
     if arr.ndim > 1:
         return tuple(_to_tuple(a) for a in arr)
     elif arr.ndim == 1:
         return tuple(arr)
     elif arr.ndim == 0:
         return float(arr)
     else:
-        raise ValueError(f'Error converting arr {arr!r} to tuple')
+        raise ValueError(f'Error converting arr {arr!r} to tuple')  # pragma: no cover
 
 
 class SpiceBase:
     """
     Class containing methods to interface with spice and manipulate coordinates.
 
     This is the base class for all the main classes used in planetmapper.
@@ -121,16 +172,21 @@
             generation in :class:`BodyXY`. These progress bars can be quite messy, but
             can be useful to keep track of very long operations.
         optimize_speed: Toggle speed optimizations. For typical observations, the
             optimizations can make code significantly faster with no effect on accuracy,
             so should generally be left enabled.
         auto_load_kernels: Toggle automatic kernel loading with
             :func:`load_spice_kernels`.
-        kernel_path: Passed to  :func:`load_spice_kernels` if `load_kernels` is True.
+        kernel_path: Passed to  :func:`load_spice_kernels` if `load_kernels` is True. It
+            is recommended to use :func:`set_kernel_path` instead of passing this
+            argument.
         manual_kernels: Passed to  :func:`load_spice_kernels` if `load_kernels` is True.
+            It is recommended to use
+            :func:`planetmapper.base.prevent_kernel_loading` then manually
+            load kernels yourself instead of passing this argument.
     """
 
     _DEFAULT_DTM_FORMAT_STRING = '%Y-%m-%dT%H:%M:%S.%f'
 
     def __init__(
         self,
         show_progress: bool = False,
@@ -321,15 +377,16 @@
     @staticmethod
     def load_spice_kernels(
         kernel_path: str | None = None,
         manual_kernels: None | list[str] = None,
         only_if_needed: bool = True,
     ) -> None:
         """
-        Attempt to intelligently SPICE kernels using `spice.furnsh`.
+        Attempt to intelligently SPICE kernels using
+        :func:`planetmapper.base.load_kernels`.
 
         If `manual_kernels` is `None` (the default), then all kernels in the directory
         given by `kernel_path` which match the following patterns are loaded:
 
         - `**/*.bsp`
         - `**/*.tpc`
         - `**/*.tls`
@@ -497,14 +554,15 @@
     """
     Base class for :class:`planetmapper.Body` and :class:`planetmapper.BasicBody`.
 
     You are unlikely to need to use this class directly - use :class:`planetmapper.Body`
     or :class:`planetmapper.BasicBody` instead.
     """
 
+    @_add_help_note_to_spice_errors
     def __init__(
         self,
         *,
         target: str | int,
         utc: str | datetime.datetime | float | None,
         observer: str | int,
         aberration_correction: str,
@@ -592,32 +650,111 @@
         """
         _, ra, dec = spice.recrad(obsvec)
         return ra, dec
 
 
 def load_kernels(*paths, clear_before: bool = False) -> list[str]:
     """
-    Load spice kernels defined by patterns
+    Load spice kernels defined by patterns.
+
+    This function calls `spice.furnsh` on all kernels matching the provided patterns.
+    The kernel paths returned by `glob.glob` are sorted by :func:`sort_kernel_paths`
+    before being passed to `spice.furnsh`.
+
+    .. hint::
+
+        You generally don't need to call this function directly - it is called
+        automatically the first time you create any object that inherits from
+        :class:`planetmapper.SpiceBase` (e.g. :class:`planetmapper.Body` or
+        :class:`planetmapper.Observation`).
 
     Args:
         *paths: Paths to spice kernels, evaluated using `glob.glob` with
             `recursive=True`.
         clear_before: Clear kernel pool before loading new kernels.
     """
     if clear_before:
         spice.kclear()
     kernels = set()
     for pattern in paths:
         kernels.update(glob.glob(os.path.expanduser(pattern), recursive=True))
-    for kernel in sorted(kernels):
+    for kernel in sort_kernel_paths(kernels):
         spice.furnsh(kernel)
     return list(kernels)
 
 
-def _clear_kernels() -> None:
+def sort_kernel_paths(kernels: Iterable[str]) -> list[str]:
+    """
+    Sort kernel paths by path depth and alphabetically.
+
+    Kernels are sorted so that kernels in subdirectories are loaded before kernels in
+    parent directories, and kernels in the same directory are sorted alphabetically.
+    Kernels loaded later will take precedence over kernels loaded earlier, so this means
+    that when kernels contain overlapping data:
+
+    - `spk/kernel.bsp` should take precedence over `spk/old/kernel.bsp`
+    - `kernel_101.bsp` should take precedence over `kernel_100.bsp`
+    - `a/kernel.bsp` should take precedence over `x/y/z/kernel.bsp`
+
+    .. warning ::
+
+        Although this function attempts to sort kernels in a sensible way, it is
+        possible that it will not always do the right thing. If you have multiple
+        kernels containing overlapping data (e.g. old predicted JWST ephemerides), it
+        is generally safer to delete the old kernels, move them into a completely
+        separate directory, or load them manually yourself using `spice.furnsh`.
+
+    Args:
+        kernels: Iterable of kernel paths.
+
+    Returns:
+        Sorted list of kernel paths.
+    """
+    # Sort by depth, then dirname, then basename, then the path itself (as a tiebreaker
+    # to ensure sort is deterministic).
+    return sorted(
+        kernels,
+        key=lambda p: (
+            -len(Path(p).resolve().parts),  # -ve so deeper paths are sorted first
+            os.path.dirname(p),
+            os.path.basename(p),
+            os.path.normpath(p),
+            p,
+        ),
+    )
+
+
+def prevent_kernel_loading() -> None:
+    """
+    Prevent PlanetMapper from automatically loading kernels.
+
+    This function can be used if want to load kernels manually using `spice.furnsh`.
+
+    ::
+
+        import spiceypy as spice
+        import planetmapper
+
+        # Call this function before creating any objects that inherit from SpiceBase,
+        # then load your desired kernels manually
+        planetmapper.base.prevent_kernel_loading()
+        kernels_to_load = [...]
+        for kernel in kernels_to_load:
+            spice.furnsh(kernel)
+
+        # After setting up the kernels, you can use PlanetMapper as normal
+        body = planetmapper.Body('mars', '2021-01-01T00:00:00')
+        body.plot_wireframe_km()
+
+    Calling :func:`clear_kernels` will re-enable automatic kernel loading.
+    """
+    _KERNEL_DATA['kernels_loaded'] = True
+
+
+def clear_kernels() -> None:
     """
     Clear spice kernel pool.
 
     This function calls `spice.kclear()`, and also indicates to PlanetMapper that
     kernels will need to be reloaded when a new object is created.
     """
     spice.kclear()
@@ -632,31 +769,57 @@
     Args:
         path: Directory which PlanetMapper will search for SPICE kernels. If `None`,
             then the default value of `'~/spice_kernels/'` will be used.
     """
     _KERNEL_DATA['kernel_path'] = path
 
 
-def get_kernel_path() -> str:
+@overload
+def get_kernel_path(return_source: Literal[False] = False) -> str:
+    ...
+
+
+@overload
+def get_kernel_path(return_source: Literal[True]) -> tuple[str, str]:
+    ...
+
+
+def get_kernel_path(return_source: bool = False) -> str | tuple[str, str]:
     """
     Get the path of the directory of SPICE kernels used in PlanetMapper.
 
     #. If a kernel path has been manually set using :func:`set_kernel_path`, then this
        path is used.
 
     #. Otherwise the value of the environment variable `PLANETMAPPER_KERNEL_PATH` is
        used.
 
     #. If `PLANETMAPPER_KERNEL_PATH` is not set, then the default value,
        `'~/spice_kernels/'` is used.
-    """
-    if _KERNEL_DATA['kernel_path'] is not None:
-        return _KERNEL_DATA['kernel_path']
+
+    Args:
+        return_source: If `True`, return a tuple of the kernel path and a string which
+            indicates the source of the kernel path. If `False` (the default), return
+            only the kernel path. The possible source strings are:
+            `'set_kernel_path()'`, `'PLANETMAPPER_KERNEL_PATH'`, and `'default'`.
+
+    Returns:
+        The path of the directory of SPICE kernels used in PlanetMapper. If
+        `return_source` is `True`, then a tuple of the kernel path and a string
+        indicating the source of the kernel path is returned.
+    """
+    if (path := _KERNEL_DATA['kernel_path']) is not None:
+        if return_source:
+            return path, 'set_kernel_path()'
+        return path
 
     try:
-        path = os.environ['PLANETMAPPER_KERNEL_PATH']
-        if path:
+        if path := os.environ['PLANETMAPPER_KERNEL_PATH']:
+            if return_source:
+                return path, 'PLANETMAPPER_KERNEL_PATH'
             return path
     except KeyError:
         pass
 
+    if return_source:
+        return DEFAULT_KERNEL_PATH, 'default'
     return DEFAULT_KERNEL_PATH
```

### Comparing `planetmapper-1.7.1/planetmapper/basic_body.py` & `planetmapper-1.7.2/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/planetmapper/body.py` & `planetmapper-1.7.2/planetmapper/body.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,34 +422,38 @@
                 :class:`BasicBody` instance instead.
 
         Returns:
             :class:`Body` or :class:`BasicBody` instance which corresponds to
             `other_target`.
         """
         try:
-            return Body(
-                target=other_target,
-                utc=self.utc,
-                observer=self.observer,
-                observer_frame=self.observer_frame,
-                illumination_source=self.illumination_source,
-                aberration_correction=self.aberration_correction,
-                subpoint_method=self.subpoint_method,
-                surface_method=self.surface_method,
-            )
-        except SpiceKERNELVARNOTFOUND:
-            if not fallback_to_basic_body:
-                raise
-            return BasicBody(
-                target=other_target,
-                utc=self.utc,
-                observer=self.observer,
-                observer_frame=self.observer_frame,
-                aberration_correction=self.aberration_correction,
-            )
+            try:
+                return Body(
+                    target=other_target,
+                    utc=self.utc,
+                    observer=self.observer,
+                    observer_frame=self.observer_frame,
+                    illumination_source=self.illumination_source,
+                    aberration_correction=self.aberration_correction,
+                    subpoint_method=self.subpoint_method,
+                    surface_method=self.surface_method,
+                )
+            except SpiceKERNELVARNOTFOUND:
+                if not fallback_to_basic_body:
+                    raise
+                return BasicBody(
+                    target=other_target,
+                    utc=self.utc,
+                    observer=self.observer,
+                    observer_frame=self.observer_frame,
+                    aberration_correction=self.aberration_correction,
+                )
+        except NotFoundError as e:
+            e.message += f'\n\nBody name: {other_target!r}'  #  type: ignore
+            raise e
 
     # Stuff to customise wireframe plots
     def add_other_bodies_of_interest(
         self, *other_targets: str | int, only_visible: bool = False
     ) -> None:
         """
         Add targets to the list of :attr:`other_bodies_of_interest` of interest to mark
@@ -1190,15 +1194,15 @@
                 return 'part hidden'
             case 0:
                 return None
             case -1 | -3:
                 return 'part transit'
             case -2:
                 return 'transit'
-        raise ValueError(f'Unknown occultation code: {occultation}')
+        raise ValueError(f'Unknown occultation code: {occultation}')  # pragma: no cover
 
     def test_if_other_body_visible(self, other: 'str | int | Body | BasicBody') -> bool:
         """
         Test if another body is visible, or is hidden behind the target body.
 
         This is a convenience method equivalent to: ::
```

### Comparing `planetmapper-1.7.1/planetmapper/body_xy.py` & `planetmapper-1.7.2/planetmapper/body_xy.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,17 @@
             self.centre_disc()
 
         self._mpl_transform_radec2xy: matplotlib.transforms.Affine2D | None = None
         self._mpl_transform_xy2radec: matplotlib.transforms.Transform | None = None
         self._mpl_transform_radec2xy_radians: matplotlib.transforms.Affine2D | None = (
             None
         )
+        self._mpl_transform_xy2radec_radians: matplotlib.transforms.Affine2D | None = (
+            None
+        )
 
         self.backplanes = {}
         self._register_default_backplanes()
 
     @classmethod
     def from_body(
         cls, body: Body, nx: int = 0, ny: int = 0, *, sz: int | None = None
@@ -863,44 +866,22 @@
     ) -> matplotlib.transforms.Affine2D:
         if self._mpl_transform_radec2xy_radians is None:
             self._mpl_transform_radec2xy_radians = matplotlib.transforms.Affine2D(
                 self._get_radec2xy_matrix_radians()
             )
         return self._mpl_transform_radec2xy_radians
 
-    def matplotlib_radec2xy_transform(
-        self, ax: Axes | None = None
-    ) -> matplotlib.transforms.Transform:
-        """
-        Get matplotlib transform which converts RA/Dec sky coordinates to image pixel
-        coordinates.
-
-        The transform is a mutable object which can be dynamically updated using
-        :func:`update_transform` when the `radec` to `xy` coordinate conversion changes.
-        This can be useful for plotting data (e.g. the planet's limb) using RA/Dec
-        coordinates onto an axis using image pixel coordinates when fitting the disc.
-
-        Args:
-            ax: Optionally specify a matplotlib axis to return
-                `transform_radec2xy + ax.transData`. This value can then be used in the
-                `transform` keyword argument of a Matplotlib function without any
-                further modification.
-
-        Returns:
-            Matplotlib transformation from `radec` to `xy` coordinates.
-        """
-        if self._mpl_transform_radec2xy is None:
-            transform_rad2deg = matplotlib.transforms.Affine2D().scale(np.deg2rad(1))
-            self._mpl_transform_radec2xy = (
-                transform_rad2deg + self._get_matplotlib_radec2xy_transform_radians()
-            )  #  type: ignore
-        transform = self._mpl_transform_radec2xy
-        if ax:
-            transform = transform + ax.transData
-        return transform
+    def _get_matplotlib_xy2radec_transform_radians(
+        self,
+    ) -> matplotlib.transforms.Affine2D:
+        if self._mpl_transform_xy2radec_radians is None:
+            self._mpl_transform_xy2radec_radians = matplotlib.transforms.Affine2D(
+                self._get_xy2radec_matrix_radians()
+            )
+        return self._mpl_transform_xy2radec_radians
 
     def matplotlib_xy2radec_transform(
         self, ax: Axes | None = None
     ) -> matplotlib.transforms.Transform:
         """
         Get matplotlib transform which converts image pixel coordinates to RA/Dec sky
         coordinates.
@@ -918,54 +899,72 @@
                 img,
                 origin='lower',
                 transform=obs.matplotlib_xy2radec_transform(ax),
                 )
 
         Args:
             ax: Optionally specify a matplotlib axis to return
-                `transform_radec2xy + ax.transData`. This value can then be used in the
+                `transform_xy2radec + ax.transData`. This value can then be used in the
                 `transform` keyword argument of a Matplotlib function without any
                 further modification.
 
         Returns:
             Matplotlib transformation from `xy` to `radec` coordinates.
         """
         if self._mpl_transform_xy2radec is None:
+            transform_deg2rad = matplotlib.transforms.Affine2D().scale(np.rad2deg(1))
             self._mpl_transform_xy2radec = (
-                self.matplotlib_radec2xy_transform().inverted()
+                self._get_matplotlib_xy2radec_transform_radians() + transform_deg2rad
             )
         transform = self._mpl_transform_xy2radec
         if ax:
             transform = transform + ax.transData
         return transform
 
+    def matplotlib_radec2xy_transform(
+        self, ax: Axes | None = None
+    ) -> matplotlib.transforms.Transform:
+        if self._mpl_transform_radec2xy is None:
+            transform_rad2deg = matplotlib.transforms.Affine2D().scale(np.deg2rad(1))
+            self._mpl_transform_radec2xy = (
+                transform_rad2deg + self._get_matplotlib_radec2xy_transform_radians()
+            )  # type: ignore
+        transform = self._mpl_transform_radec2xy
+        if ax:
+            transform = transform + ax.transData
+        return transform
+
     def matplotlib_xy2km_transform(
-        self, ax: Axes | None
+        self, ax: Axes | None = None
     ) -> matplotlib.transforms.Transform:
         return (
             self.matplotlib_xy2radec_transform()
             + self.matplotlib_radec2km_transform(ax)
         )
 
     def matplotlib_km2xy_transform(
-        self, ax: Axes | None
+        self, ax: Axes | None = None
     ) -> matplotlib.transforms.Transform:
         return (
             self.matplotlib_km2radec_transform()
             + self.matplotlib_radec2xy_transform(ax)
         )
 
     def update_transform(self) -> None:
         """
-        Update the transformation returned by :func:`matplotlib_radec2xy_transform`
-        to use the latest disc parameter values `(x0, y0, r0, rotation)`.
+        Update the transformations returned by :func:`matplotlib_radec2xy_transform`
+        and :func:`matplotlib_xy2radec_transform` to use the latest disc parameter
+        values `(x0, y0, r0, rotation)`.
         """
         self._get_matplotlib_radec2xy_transform_radians().set_matrix(
             self._get_radec2xy_matrix_radians()
         )
+        self._get_matplotlib_xy2radec_transform_radians().set_matrix(
+            self._get_xy2radec_matrix_radians()
+        )
 
     # Mapping
     def map_img(
         self,
         img: np.ndarray,
         *,
         interpolation: Literal['nearest', 'linear', 'quadratic', 'cubic'] = 'linear',
@@ -1121,15 +1120,15 @@
         grid_interval: float = 30,
         indicate_equator: bool = True,
         indicate_prime_meridian: bool = True,
         aspect_adjustable: Literal['box', 'datalim'] = 'box',
         formatting: dict[_WireframeComponent, dict[str, Any]] | None = None,
         common_formatting: dict[str, Any] | None = None,
         **map_kwargs: Unpack[_MapKwargs],
-    ):
+    ) -> Axes:
         """
         Plot wireframe (e.g. gridlines) of the map projection of the observation. See
         :func:`Body.plot_wireframe_radec` for details of accepted arguments.
 
         For example, to plot an orthographic map's wireframe with a red boundary and
         dashed gridlines, you can use: ::
 
@@ -1802,27 +1801,29 @@
             the longitude and latitude coordinates of the map, `xx` and `yy` are the
             projected coordinates of the map, `transformer` is a `pyproj.Transformer`
             object that can be used to transform between the two coordinate systems, and
             `info` is a dictionary containing the arguments used to build the map (e.g.
             for the default case this is
             `{'projection': 'rectangular', 'degree_interval': 1}`).
         """
+        info: dict[str, Any]  # Explicitly declare type of info to make pyright happy
         if projection == 'rectangular':
             lon_coords = np.arange(degree_interval / 2, 360, degree_interval)
             if self.positive_longitude_direction == 'W':
                 lon_coords = lon_coords[::-1]
             lat_coords = np.arange(-90 + degree_interval / 2, 90, degree_interval)
             lon_coords, lat_coords = np.meshgrid(lon_coords, lat_coords)
+            info = dict(projection=projection, degree_interval=degree_interval)
             return (
                 lon_coords,
                 lat_coords,
                 lon_coords,
                 lat_coords,
                 self._get_pyproj_transformer(),
-                dict(projection=projection, degree_interval=degree_interval),
+                info,
             )
         elif projection == 'manual':
             if lon_coords is None or lat_coords is None:
                 raise ValueError('lons and lats must be provided for manual projection')
             lon_coords = np.asarray(lon_coords)
             lat_coords = np.asarray(lat_coords)
             if lon_coords.ndim != lat_coords.ndim:
@@ -1831,54 +1832,58 @@
                 )
             if lon_coords.ndim == 1:
                 lon_coords, lat_coords = np.meshgrid(lon_coords, lat_coords)
             if lon_coords.ndim != 2:
                 raise ValueError('lon_coords and lat_coords must be 1D or 2D arrays')
             if lon_coords.shape != lat_coords.shape:
                 raise ValueError('lon_coords and lat_coords must have the same shape')
+            info = dict(projection=projection)
             return (
                 lon_coords,
                 lat_coords,
                 lon_coords,
                 lat_coords,
                 self._get_pyproj_transformer(),
-                dict(projection=projection),
+                info,
             )
         elif projection == 'orthographic':
             proj = '+proj=ortho +a={a} +b={b} +lon_0={lon_0} +lat_0={lat_0} +y_0={y_0} +type=crs'.format(
                 a=self.r_eq,
                 b=self.r_polar,
                 lon_0=lon,
                 lat_0=lat,
                 y_0=(self.r_polar - self.r_eq) * np.sin(np.radians(lat * 2)),
             )
             lim = max(self.r_eq, self.r_polar) * 1.01
+            info = dict(projection=projection, lon=lon, lat=lat, size=size)
             return (
                 *self._get_pyproj_map_coords(proj, np.linspace(-lim, lim, size)),
-                dict(projection=projection, lon=lon, lat=lat, size=size),
+                info,
             )
         elif projection == 'azimuthal':
             proj = '+proj=aeqd +R={a} +lon_0={lon_0} +lat_0={lat_0} +type=crs'.format(
                 a=self.r_eq,
                 lon_0=lon,
                 lat_0=lat,
             )
             lim = max(self.r_eq, self.r_polar) * np.pi * 1.01
+            info = dict(projection=projection, lon=lon, lat=lat, size=size)
             return (
                 *self._get_pyproj_map_coords(proj, np.linspace(-lim, lim, size)),
-                dict(projection=projection, lon=lon, lat=lat, size=size),
+                info,
             )
         else:
             if projection_x_coords is None:
                 raise ValueError('x coords must be provided')
+            info = dict(projection=projection)
             return (
                 *self._get_pyproj_map_coords(
                     projection, projection_x_coords, projection_y_coords
                 ),
-                dict(projection=projection),
+                info,
             )
 
     def _get_pyproj_map_coords(
         self,
         projection: str,
         xx: np.ndarray | tuple,
         yy: np.ndarray | tuple | None = None,
```

### Comparing `planetmapper-1.7.1/planetmapper/data/rings.json` & `planetmapper-1.7.2/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/planetmapper/data_loader.py` & `planetmapper-1.7.2/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/planetmapper/gui.py` & `planetmapper-1.7.2/planetmapper/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
 import numpy as np
 import spiceypy as spice
 from astropy.io import fits
 from matplotlib.artist import Artist
 from matplotlib.backend_bases import MouseButton, MouseEvent
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
+from matplotlib.backends.backend_tkagg import NavigationToolbar2Tk  # type: ignore
+from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.text import Text
 
 from . import base, common, data_loader, progress, utils
 from .body import BasicBody, Body, NotFoundError
 from .body_xy import _MapKwargs
 from .observation import Observation
 
@@ -1668,15 +1669,15 @@
                 )
                 return False
 
         string = self.kernel_txt.get('1.0', 'end')
         kernels = [k.strip() for k in string.splitlines()]
         base.load_kernels(*kernels, clear_before=True)
 
-        kernel_help = 'Check for typos and make sure you have listed all the required SPICE kernels'
+        kernel_help = '\n' + base._SPICE_ERROR_HELP_TEXT
 
         sb = base.SpiceBase(auto_load_kernels=False)
         try:
             target = sb.standardise_body_name(kwargs['target'])
         # pylint: disable-next=bare-except
         except:
             tkinter.messagebox.showwarning(
```

### Comparing `planetmapper-1.7.1/planetmapper/kernel_downloader.py` & `planetmapper-1.7.2/planetmapper/kernel_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         if p.startswith(prefix):
             return _standardise_path(os.path.relpath(p, prefix))
     raise ValueError('Cannot get kernel path from "{}"'.format(p))
 
 
 def _kernel_path_to_url(kp: str) -> str:
     """Create URL from a kernel path"""
-    return URL_ROOT + os.path.sep + kp
+    return URL_ROOT + kp
 
 
 def _kernel_path_to_local_path(kp: str) -> str:
     """Create a local path from a kernel path"""
     return _standardise_path(get_kernel_path() + os.path.sep + kp)
```

### Comparing `planetmapper-1.7.1/planetmapper/observation.py` & `planetmapper-1.7.2/planetmapper/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,17 +324,21 @@
         wcs = self._get_wcs_from_header(suppress_warnings=suppress_warnings)
 
         if wcs.naxis == 0:
             raise ValueError('No WCS information found in FITS header')
 
         if validate:
             if not all(u == 'deg' for u in wcs.world_axis_units):
-                raise ValueError('WCS coordinates are not in degrees')
+                raise ValueError(
+                    'WCS coordinates are not in degrees'
+                )  # pragma: no cover
             if not wcs.world_axis_physical_types == ['pos.eq.ra', 'pos.eq.dec']:
-                raise ValueError('WCS axes are not RA/Dec coordinates')
+                raise ValueError(
+                    'WCS axes are not RA/Dec coordinates'
+                )  # pragma: no cover
             if wcs.has_distortion:
                 raise ValueError('WCS conversion contains distortion terms')
 
         x0, y0 = wcs.world_to_pixel_values(self.target_ra, self.target_dec)
 
         b1, b2 = wcs.pixel_to_world_values(x0, y0 + 1)
         c1, c2 = wcs.pixel_to_world_values(x0, y0)
```

### Comparing `planetmapper-1.7.1/planetmapper/progress.py` & `planetmapper-1.7.2/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/planetmapper/utils.py` & `planetmapper-1.7.2/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.1
-Summary: A Python module for visualising, navigating and mapping Solar System observations
+Version: 1.7.2
+Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
+License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
 Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-# PlanetMapper
+# ![PlanetMapper logo](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/logo_wide_transparent.png)
 
 [![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
-[![Upload Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
-[![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
-[![Format](https://github.com/ortk95/planetmapper/actions/workflows/format.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/format.yml)
-[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/test.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/test.yml)
+[![Publish](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
+[![Checks](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/checks.yml)
 [![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
-
-A Python module for visualising, navigating and mapping Solar System observations.
+PlanetMapper is a Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
 
 
 ## [Installation](https://planetmapper.readthedocs.io/en/latest/installation.html)
 ```
 pip install planetmapper --upgrade
 ```
 
 _Requires Python 3.10+_
 
 ## Key features
 ### [Fit and map astronomical observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
-![PlanetMapper graphical user interface](https://github.com/ortk95/planetmapper/blob/main/docs/images/gui_fitting.png?raw=true)
+[![Screenshot of the PlanetMapper graphical user interface showing an observation of Europa being navigated](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/gui_fitting.png)](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
 
 ### [Easily visualise solar system observations with just a few lines of code](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ```python
 body = planetmapper.Body('saturn', '2020-01-01')
 body.plot_wireframe_radec()
 plt.show()
 ```
 
-![Image of Saturn generated with PlanetMapper](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/saturn_wireframe_radec.png)
+[![Image of Saturn generated with PlanetMapper showing the orientation of Saturn and its rings](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/saturn_wireframe_radec.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ### [Convert coordinates, generate backplanes and project maps of telescope observations](https://planetmapper.readthedocs.io/en/latest/general_python_api.html)
-![Plot of a mapped Jupiter observation, generated with PlanetMapper](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/jupiter_mapped.png)
+[![Plot of a mapped Jupiter observation, generated with PlanetMapper, showing observed and mapped versions of the Jupiter data](https://raw.githubusercontent.com/ortk95/planetmapper/main/docs/images/jupiter_mapped.png)](https://planetmapper.readthedocs.io/en/latest/general_python_api.html)
+
+
+## Contributing
+
+If you spot a bug, have a suggestion, or want contribute code to PlanetMapper, check out the [contributing guidelines](https://github.com/ortk95/planetmapper/blob/main/CONTRIBUTING.md)!
```

### Comparing `planetmapper-1.7.1/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.7.2/planetmapper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 planetmapper/__init__.py
 planetmapper/base.py
 planetmapper/basic_body.py
 planetmapper/body.py
```

### Comparing `planetmapper-1.7.1/setup.py` & `planetmapper-1.7.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     long_description = f.read()
 
 setuptools.setup(
     name='planetmapper',
     version=common.__version__,
     author=common.__author__,
     author_email='oliver.king95@gmail.com',
-    description='A Python module for visualising, navigating and mapping Solar System observations',
+    description=common.__description__,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url=common.__url__,
+    license=common.__license__,
     download_url='https://pypi.org/project/planetmapper/',
     packages=['planetmapper'],
     package_dir={'planetmapper': 'planetmapper'},
     package_data={'planetmapper': ['data/*.json']},
     include_package_data=True,
     project_urls={
         'Documentation': 'https://planetmapper.readthedocs.io/',
```

### Comparing `planetmapper-1.7.1/tests/test_basic_body.py` & `planetmapper-1.7.2/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/tests/test_body.py` & `planetmapper-1.7.2/tests/test_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import datetime
 import unittest
+from unittest.mock import MagicMock, patch
 
 import common_testing
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy import array, nan
-from spiceypy.utils.exceptions import NotFoundError, SpiceSPKINSUFFDATA
+from spiceypy.utils.exceptions import (
+    NotFoundError,
+    SpiceKERNELVARNOTFOUND,
+    SpiceSPKINSUFFDATA,
+)
 
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
 from planetmapper import Body
 
 
@@ -26,14 +31,41 @@
         self.assertEqual(
             Body(
                 'Jupiter', utc='2005-01-01', aberration_correction='CN+S'
             ).subpoint_lon,
             153.12614128206837,
         )
 
+        # Test Saturrn automatically has A, B & C rings added
+        saturn = Body('saturn', '2000-01-01')
+        self.assertEqual(saturn.target, 'SATURN')
+        self.assertEqual(saturn.target_body_id, 699)
+        self.assertEqual(
+            saturn.ring_radii, {74658.0, 91975.0, 117507.0, 122340.0, 136780.0}
+        )
+
+    def test_rotation_sense(self):
+        comparisons: list[tuple[str, str, bool]] = [
+            ('sun', 'E', True),
+            ('moon', 'E', True),
+            ('earth', 'E', True),
+            ('jupiter', 'W', True),
+            ('amalthea', 'W', True),
+            ('uranus', 'E', False),
+        ]
+        for target, positive_dir, prograde in comparisons:
+            with self.subTest(target=target):
+                body = planetmapper.Body(
+                    target,
+                    observer='HST',
+                    utc='2005-01-01T00:00:00',
+                )
+                self.assertEqual(body.positive_longitude_direction, positive_dir)
+                self.assertEqual(body.prograde, prograde)
+
     def test_attributes(self):
         self.assertEqual(self.body.target, 'JUPITER')
         self.assertEqual(self.body.utc, '2005-01-01T00:00:00.000000')
         self.assertEqual(self.body.observer, 'HST')
         self.assertAlmostEqual(self.body.et, 157809664.1839331)
         self.assertEqual(
             self.body.dtm,
@@ -169,14 +201,30 @@
         )
 
     def test_create_other_body(self):
         self.assertEqual(
             self.body.create_other_body('amalthea'),
             Body('AMALTHEA', observer='HST', utc='2005-01-01T00:00:00'),
         )
+        self.assertEqual(
+            self.body.create_other_body('daphnis'),
+            planetmapper.BasicBody(
+                'DAPHNIS', observer='HST', utc='2005-01-01T00:00:00'
+            ),
+        )
+        with self.assertRaises(SpiceKERNELVARNOTFOUND):
+            self.body.create_other_body('daphnis', fallback_to_basic_body=False)
+
+        target = '<<< test >>>'
+        with self.assertRaises(NotFoundError):
+            self.body.create_other_body(target)
+        try:
+            self.body.create_other_body(target)
+        except NotFoundError as e:
+            self.assertIn(target, e.message)
 
     def test_add_other_bodies_of_interest(self):
         self.body.add_other_bodies_of_interest('amalthea')
         self.assertEqual(
             self.body.other_bodies_of_interest,
             [Body('AMALTHEA', observer='HST', utc='2005-01-01T00:00:00')],
         )
@@ -204,31 +252,45 @@
         self.assertEqual(jupiter.other_bodies_of_interest, [])
 
         jupiter.add_other_bodies_of_interest('AMALTHEA', 'THEBE')
         self.assertEqual(
             jupiter.other_bodies_of_interest,
             [Body('AMALTHEA', utc), Body('THEBE', utc)],
         )
+        # Check duplicate bodies are not added
+        jupiter.add_other_bodies_of_interest('AMALTHEA', 'THEBE')
+        self.assertEqual(
+            jupiter.other_bodies_of_interest,
+            [Body('AMALTHEA', utc), Body('THEBE', utc)],
+        )
 
     def test_add_satellites_to_bodies_of_interest(self):
         self.body.other_bodies_of_interest.clear()
         with self.assertRaises(SpiceSPKINSUFFDATA):
             self.body.add_satellites_to_bodies_of_interest()
 
+        expected = [
+            Body('AMALTHEA', '2005-01-01T00:00:00.000000', 'HST'),
+            Body('THEBE', '2005-01-01T00:00:00.000000', 'HST'),
+            Body('ADRASTEA', '2005-01-01T00:00:00.000000', 'HST'),
+            Body('METIS', '2005-01-01T00:00:00.000000', 'HST'),
+        ]
         self.body.other_bodies_of_interest.clear()
         self.body.add_satellites_to_bodies_of_interest(skip_insufficient_data=True)
-        self.assertEqual(
-            self.body.other_bodies_of_interest,
-            [
-                Body('AMALTHEA', '2005-01-01T00:00:00.000000', 'HST'),
-                Body('THEBE', '2005-01-01T00:00:00.000000', 'HST'),
-                Body('ADRASTEA', '2005-01-01T00:00:00.000000', 'HST'),
-                Body('METIS', '2005-01-01T00:00:00.000000', 'HST'),
-            ],
-        )
+        self.assertEqual(self.body.other_bodies_of_interest, expected)
+
+        # Test duplicates aren't added
+        self.body.add_satellites_to_bodies_of_interest(skip_insufficient_data=True)
+        self.assertEqual(self.body.other_bodies_of_interest, expected)
+        self.body.other_bodies_of_interest.clear()
+        self.assertEqual(self.body.other_bodies_of_interest, [])
+        self.body.add_other_bodies_of_interest('amalthea', 'thebe')
+        self.assertEqual(self.body.other_bodies_of_interest, expected[:2])
+        self.body.add_satellites_to_bodies_of_interest(skip_insufficient_data=True)
+        self.assertEqual(self.body.other_bodies_of_interest, expected)
         self.body.other_bodies_of_interest.clear()
         self.assertEqual(self.body.other_bodies_of_interest, [])
 
         utc = '2005-01-01 04:00:00'
         jupiter = planetmapper.Body('Jupiter', utc)
         jupiter.add_satellites_to_bodies_of_interest(
             skip_insufficient_data=True, only_visible=True
@@ -441,14 +503,23 @@
                             -5.56152901,
                         ]
                     ),
                 ),
                 equal_nan=True,
             )
         )
+        self.assertTrue(
+            np.allclose(
+                self.body.limb_radec(npts=3, close_loop=False),
+                (
+                    array([196.37390736, 196.37487476, 196.36707757]),
+                    array([-5.56152901, -5.56977427, -5.56629386]),
+                ),
+            )
+        )
 
     def test_limb_radec_by_illumination(self):
         self.assertTrue(
             np.allclose(
                 self.body.limb_radec_by_illumination(npts=5),
                 (
                     array(
@@ -536,14 +607,21 @@
                 (
                     array([nan, nan, nan, 196.36784184, 196.36838618, nan]),
                     array([nan, nan, nan, -5.56815505, -5.56246241, nan]),
                 ),
                 equal_nan=True,
             )
         )
+        self.assertTrue(
+            np.allclose(
+                self.body.terminator_radec(npts=3, close_loop=False),
+                (array([nan, nan, 196.36713568]), array([nan, nan, -5.56628042])),
+                equal_nan=True,
+            )
+        )
 
     def test_if_lonlat_illuminated(self):
         pairs: list[tuple[tuple[float, float], bool]] = [
             ((0, 0), False),
             ((180, 12), True),
         ]
         for (lon, lat), illuminated in pairs:
@@ -551,24 +629,47 @@
                 self.assertEqual(
                     self.body.test_if_lonlat_illuminated(lon, lat), illuminated
                 )
 
     def test_ring_plane_coordinates(self):
         self.assertTrue(
             np.allclose(
+                self.body.ring_plane_coordinates(0, 0),
+                (nan, nan, nan),
+                equal_nan=True,
+            ),
+        )
+        self.assertTrue(
+            np.allclose(
                 self.body.ring_plane_coordinates(
                     196.37198562427025, -5.565793847134351
                 ),
                 (nan, nan, nan),
                 equal_nan=True,
             ),
         )
         self.assertTrue(
             np.allclose(
                 self.body.ring_plane_coordinates(
+                    196.37347182693253, -5.561472466522512
+                ),
+                (1377914.753652832, 152.91772706249577, 818261707.8278764),
+                equal_nan=True,
+            ),
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.ring_plane_coordinates(196.3696997398314, -5.569843641306982),
+                (nan, nan, nan),
+                equal_nan=True,
+            ),
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.ring_plane_coordinates(
                     196.37198562427025, -5.565793847134351, only_visible=False
                 ),
                 (4638.105239104683, 156.0690984698183, 819638074.3312378),
                 equal_nan=True,
             ),
         )
         self.assertTrue(
@@ -586,14 +687,24 @@
                 (
                     array([nan, 196.37142013, 196.37228744, nan, nan]),
                     array([nan, -5.5655251, -5.56589635, nan, nan]),
                 ),
                 equal_nan=True,
             )
         )
+        self.assertTrue(
+            np.allclose(
+                self.body.ring_radec(123456.789, npts=3, only_visible=False),
+                (
+                    array([196.36825958, 196.37571178, 196.36825958]),
+                    array([-5.56452821, -5.56705935, -5.56452821]),
+                ),
+                equal_nan=True,
+            )
+        )
 
     def test_visible_lonlat_grid_radec(self):
         self.assertTrue(
             np.allclose(
                 self.body.visible_lonlat_grid_radec(interval=45, npts=5),
                 [
                     (
@@ -712,15 +823,19 @@
             self.body.get_description(),
             'JUPITER (599)\nfrom HST\nat 2005-01-01 00:00 UTC',
         )
 
     def test_get_poles_to_plot(self):
         self.assertEqual(self.body.get_poles_to_plot(), [(0, -90, 'S')])
 
-    def test_plot_wireframe(self):
+        moon = Body('moon', utc='2000-01-08 03:00:00')
+        self.assertEqual(moon.get_poles_to_plot(), [(0, 90, '(N)'), (0, -90, '(S)')])
+
+    @patch('matplotlib.pyplot.show')
+    def test_plot_wireframe(self, mock_show: MagicMock):
         fig, ax = plt.subplots()
         self.body.plot_wireframe_radec(ax, color='red')
         plt.close(fig)
 
         ax = self.body.plot_wireframe_km()
         plt.close(ax.figure)
 
@@ -751,7 +866,65 @@
 
         # Test hidden other bodies
         jupiter = planetmapper.Body('jupiter', utc='2005-01-01T04:00')
         jupiter.add_other_bodies_of_interest('thebe', 'metis', 'amalthea', 'adrastea')
         fig, ax = plt.subplots()
         jupiter.plot_wireframe_radec(ax)
         plt.close(fig)
+
+        # Test show
+        fig, ax = plt.subplots()
+        jupiter.plot_wireframe_radec(ax, show=True)
+        plt.close(fig)
+        mock_show.assert_called_once()
+        mock_show.reset_mock()
+
+        fig, ax = plt.subplots()
+        jupiter.plot_wireframe_km(ax, show=True)
+        plt.close(fig)
+        mock_show.assert_called_once()
+        mock_show.reset_mock()
+
+    def test_matplotlib_transforms(self):
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_km2radec_transform().get_matrix(),
+                array(
+                    [
+                        [-6.40343479e-08, 2.88537788e-08, 1.96371986e02],
+                        [2.87177471e-08, 6.37324567e-08, -5.56579385e00],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_radec2km_transform().get_matrix(),
+                array(
+                    [
+                        [-1.29809749e07, 5.87691418e06, 2.58180951e09],
+                        [5.84920736e06, 1.30424639e07, -1.07602880e09],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+
+        fig, axis = plt.subplots()
+        for ax in [None, axis]:
+            with self.subTest(ax=ax):
+                # Test caching works
+                self.body.matplotlib_radec2km_transform(ax)
+                t1 = self.body.matplotlib_radec2km_transform(ax)
+                self.body._mpl_transform_radec2km = None
+                t2 = self.body.matplotlib_radec2km_transform(ax)
+                self.assertEqual(t1, t2)
+
+                self.body.matplotlib_km2radec_transform(ax)
+                t1 = self.body.matplotlib_km2radec_transform(ax)
+                self.body._mpl_transform_km2radec = None
+                t2 = self.body.matplotlib_km2radec_transform(ax)
+                self.assertEqual(t1, t2)
+
+        plt.close(fig)
```

### Comparing `planetmapper-1.7.1/tests/test_body_xy.py` & `planetmapper-1.7.2/tests/test_body_xy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+from unittest.mock import MagicMock, patch
 
 import common_testing
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy import array, nan
 
 import planetmapper
@@ -327,14 +328,17 @@
                 with self.assertRaises(ValueError):
                     setter(np.nan)
                 with self.assertRaises(TypeError):
                     setter('a string')
                 with self.assertRaises(TypeError):
                     setter(np.array([1, 2, 3]))
 
+        with self.assertRaises(ValueError):
+            self.body.set_r0(-1.23)
+
         self.body.set_plate_scale_arcsec(1)
         self.assertAlmostEqual(self.body.get_plate_scale_arcsec(), 1)
         self.assertAlmostEqual(self.body.get_r0(), 17.991213518286685)
 
         self.body.set_plate_scale_km(1)
         self.assertAlmostEqual(self.body.get_plate_scale_km(), 1)
         self.assertAlmostEqual(self.body.get_r0(), 71492.0)
@@ -471,15 +475,15 @@
                     array([nan, nan, nan, 7.49990606, 14.92008563, nan]),
                     array([nan, nan, nan, -1.2293739, 7.50713047, nan]),
                 ),
                 equal_nan=True,
             )
         )
 
-    def test_termrinator_xy(self):
+    def test_terminator_xy(self):
         self.body.set_disc_params(5, 8, 10, 45)
         self.assertTrue(
             np.allclose(
                 self.body.terminator_xy(npts=3),
                 (
                     array([nan, nan, 11.14140527, nan]),
                     array([nan, nan, 0.48169876, nan]),
@@ -523,101 +527,152 @@
                     array([nan, 5.09062199, 4.8390282, nan]),
                     array([nan, 7.97280096, 8.06177746, nan]),
                 ),
                 equal_nan=True,
             )
         )
 
-    def test_plot_wireframe(self):
+    @patch('matplotlib.pyplot.show')
+    def test_plot_wireframe(self, mock_show: MagicMock):
+        fig, ax = plt.subplots()
+        self.body.plot_wireframe_xy(ax=ax)
+        plt.close(fig)
+
         fig, ax = plt.subplots()
-        self.body.plot_wireframe_km(ax=ax)
+        self.body.plot_wireframe_xy(ax=ax, show=True)
         plt.close(fig)
+        mock_show.assert_called_once()
+        mock_show.reset_mock()
 
         fig, ax = plt.subplots()
-        self.body.plot_map_wireframe(ax=ax)
+        self.body_zero_size.plot_wireframe_xy(ax=ax)
         plt.close(fig)
 
+        ax = self.body.plot_map_wireframe()
+        self.assertEqual(ax.get_xlim(), (360, 0))
+        plt.close('all')
+
+        uranus = BodyXY('uranus', utc='2000-01-01', sz=5)  # Uranus is +ve E
+        ax = uranus.plot_map_wireframe(ax=ax)
+        self.assertEqual(ax.get_xlim(), (0, 360))
+        plt.close('all')
+
         fig, ax = plt.subplots()
         self.body.plot_map_wireframe(ax=ax, projection='orthographic', lat=56)
         plt.close(fig)
 
         fig, ax = plt.subplots()
         self.body.plot_map_wireframe(ax=ax, projection='azimuthal', lat=-90)
         plt.close(fig)
 
+        fig, ax = plt.subplots()
+        self.body.plot_map_wireframe(
+            ax=ax,
+            projection='manual',
+            lon_coords=np.linspace(-180, 180, 5),
+            lat_coords=np.linspace(0, 90, 3),
+        )
+        plt.close(fig)
+
     def test_get_wireframe_overlay(self):
         img = self.body.get_wireframe_overlay_img(output_size=100)
         self.assertEqual(max(img.shape), 100)
         self.assertEqual(len(img.shape), 2)
 
         img = self.body.get_wireframe_overlay_map(output_size=100)
         self.assertEqual(max(img.shape), 100)
         self.assertEqual(len(img.shape), 2)
 
-    def test_map_img(self):
+        img = self.body.get_wireframe_overlay_map(output_size=100, rgba=True)
+        self.assertEqual(max(img.shape), 100)
+        self.assertEqual(len(img.shape), 3)
+        self.assertEqual(img.shape[2], 4)
+
+    @patch('builtins.print')
+    def test_map_img(self, mock_print: MagicMock):
         self.body.set_img_size(4, 3)
         self.body.set_disc_params(2, 1, 1.5, 45.678)
 
         image = np.array(
             [
                 [-1.0, 2.2, 3.3, 4.4],
                 [999.0, nan, 1.0, 1.0],
                 [0.0, 3.0, 0.0, nan],
+                [0.0, 3.0, 0.1, nan],
             ]
         )
         expected = {
             'nearest': array(
                 [
-                    [nan, nan, nan, 2.31866428, 2.74706312, 3.19651992, nan, nan],
-                    [nan, nan, nan, nan, nan, 3.31150404, nan, nan],
-                    [nan, nan, nan, nan, nan, nan, nan, nan],
-                    [nan, nan, 0.28286675, nan, nan, nan, nan, nan],
+                    [nan, nan, 2.2, 2.2, 2.2, 3.3, nan, nan],
+                    [nan, nan, nan, nan, 1.0, 4.4, nan, nan],
+                    [nan, nan, 3.0, 3.0, 0.0, 1.0, nan, nan],
+                    [nan, nan, 0.0, 0.0, 0.0, nan, nan, nan],
                 ]
             ),
             'linear': array(
                 [
                     [nan, nan, nan, 2.31866428, 2.74706312, 3.19651992, nan, nan],
                     [nan, nan, nan, nan, nan, 3.31150404, nan, nan],
                     [nan, nan, nan, nan, nan, nan, nan, nan],
-                    [nan, nan, 0.28286675, nan, nan, nan, nan, nan],
+                    [nan, nan, 0.32017562, nan, nan, nan, nan, nan],
                 ]
             ),
             'quadratic': array(
                 [
-                    [nan, nan, nan, 2.31866428, 2.74706312, 3.19651992, nan, nan],
-                    [nan, nan, nan, nan, nan, 3.31150404, nan, nan],
+                    [nan, nan, nan, 2.39880056, 2.87923885, 3.21453136, nan, nan],
+                    [nan, nan, nan, nan, nan, 11.73917107, nan, nan],
                     [nan, nan, nan, nan, nan, nan, nan, nan],
-                    [nan, nan, 0.28286675, nan, nan, nan, nan, nan],
+                    [nan, nan, 1.75206632, nan, nan, nan, nan, nan],
                 ]
             ),
             'cubic': array(
                 [
-                    [nan, nan, nan, 2.31866428, 2.74706312, 3.19651992, nan, nan],
-                    [nan, nan, nan, nan, nan, 3.31150404, nan, nan],
+                    [nan, nan, nan, 2.38239808, 2.87854299, 3.22915402, nan, nan],
+                    [nan, nan, nan, nan, nan, 38.97003701, nan, nan],
                     [nan, nan, nan, nan, nan, nan, nan, nan],
-                    [nan, nan, 0.28286675, nan, nan, nan, nan, nan],
+                    [nan, nan, 4.84799586, nan, nan, nan, nan, nan],
                 ]
             ),
         }
         for interpolation, expected_img in expected.items():
             with self.subTest(interpolation=interpolation):
                 self.assertTrue(
                     np.allclose(
-                        self.body.map_img(image, degree_interval=45),
+                        self.body.map_img(
+                            image,
+                            degree_interval=45,
+                            interpolation=interpolation,  # type: ignore
+                        ),
                         expected_img,
                         equal_nan=True,
                     )
                 )
 
+        self.body.map_img(
+            image, interpolation='linear', degree_interval=45, warn_nan=True
+        )
+        mock_print.assert_called_once()
+        mock_print.reset_mock()
+
+        with self.assertRaises(ValueError):
+            self.body.map_img(image, interpolation='<<<test>>>')  # type: ignore
+
         with self.assertRaises(ValueError):
             self.body.map_img(image, projection='manual')
 
         lons = np.linspace(-180, 180, 5)
         lats = np.linspace(0, 90, 3)
-
+        image = np.array(
+            [
+                [-1.0, 2.2, 3.3, 4.4],
+                [999.0, nan, 1.0, 1.0],
+                [0.0, 3.0, 0.0, nan],
+            ]
+        )
         for attempt in range(2):
             with self.subTest(attempt=attempt):
                 # Test twice to check cache behaviour
                 self.assertTrue(
                     np.allclose(
                         self.body.map_img(
                             image, projection='manual', lon_coords=lons, lat_coords=lats
@@ -649,14 +704,70 @@
                 ),
                 equal_nan=True,
             )
         )
 
         self.body.set_img_size(15, 10)
 
+    def test_generate_map_coordinates(self):
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates(projection='manual')
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates(
+                'manual',
+                lon_coords=np.array([1, 2, 3]),
+                lat_coords=np.array([[1, 2, 3], [4, 5, 6]]),
+            )
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates(
+                'manual',
+                lon_coords=np.array([[[1, 2, 3]]]),
+                lat_coords=np.array([[[1, 2, 3]]]),
+            )
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates(
+                'manual',
+                lon_coords=np.array([[1, 2, 3]]),
+                lat_coords=np.array([[1, 2, 3], [4, 5, 6]]),
+            )
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates('proj=ortho +R=1 +type=crs')
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates(
+                'proj=ortho +R=1 +type=crs',
+                projection_x_coords=np.array([1, 2, 3]),
+                projection_y_coords=np.array([[1, 2, 3], [4, 5, 6]]),
+            )
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates(
+                'proj=ortho +R=1 +type=crs',
+                projection_x_coords=np.array([[[1, 2, 3]]]),
+            )
+        with self.assertRaises(ValueError):
+            self.body.generate_map_coordinates(
+                'proj=ortho +R=1 +type=crs',
+                projection_x_coords=np.array([[1, 2, 3]]),
+                projection_y_coords=np.array([[1, 2, 3], [4, 5, 6]]),
+            )
+        output_a = self.body.generate_map_coordinates(
+            '+proj=ortho +R=1 +type=crs', projection_x_coords=np.array([0, 0.25, 0.5])
+        )
+        output_b = self.body.generate_map_coordinates(
+            '+proj=ortho +R=1 +type=crs',
+            projection_x_coords=np.array([0, 0.25, 0.5]),
+            projection_y_coords=np.array([0, 0.25, 0.5]),
+        )
+        for idx, (a, b) in enumerate(zip(output_a, output_b)):
+            with self.subTest(idx=idx):
+                self.assertEqual(type(a), type(b))
+                if isinstance(a, np.ndarray):
+                    self.assertTrue(np.array_equal(a, b))
+                else:
+                    self.assertEqual(a, b)
+
     def test_standardise_backplane_name(self):
         self.assertEqual(self.body.standardise_backplane_name('EMISSION'), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name(' EMISSION '), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name('emission'), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name('EmIsSiOn'), 'EMISSION')
 
     def test_register_backplane(self):
@@ -715,14 +826,19 @@
             'RING-DISTANCE: Equatorial (ring) plane distance to observer [km]',
         ]
         self.assertEqual(
             self.body.backplane_summary_string(),
             '\n'.join(lines),
         )
 
+    @patch('builtins.print')
+    def test_print_backplanes(self, mock_print: MagicMock):
+        self.body.print_backplanes()
+        mock_print.assert_called_once_with(self.body.backplane_summary_string())
+
     def test_get_backplane(self):
         self.assertEqual(
             self.body.get_backplane(' emission '),
             Backplane(
                 'EMISSION',
                 'Emission angle [deg]',
                 self.body.get_emission_angle_img,
@@ -764,22 +880,170 @@
                     ]
                 ),
                 equal_nan=True,
             )
         )
         self.body.set_img_size(15, 10)
 
-    def test_plot_backplane(self):
+    @patch('matplotlib.pyplot.show')
+    def test_plot_backplane(self, mock_show: MagicMock):
         fig, ax = plt.subplots()
         self.body.plot_backplane_img(' emission ', ax=ax)
         plt.close(fig)
 
         fig, ax = plt.subplots()
-        self.body.plot_backplane_map(' emission ', degree_interval=90, ax=ax)
+        self.body.plot_backplane_img(' EmissioN ', ax=ax, show=True)
         plt.close(fig)
+        mock_show.assert_called_once()
+        mock_show.reset_mock()
+
+        fig, ax = plt.subplots()
+        self.body.plot_backplane_map(' emission ', ax=ax, show=True)
+        plt.close(fig)
+        mock_show.assert_called_once()
+        mock_show.reset_mock()
+
+        self.body.plot_backplane_map(' emission ', degree_interval=90)
+        plt.close('all')
 
     def test_plot_map(self):
         fig, ax = plt.subplots()
         self.body.plot_map(np.ones((180, 360)), ax=ax)
         plt.close(fig)
 
+        self.body.imshow_map(np.ones((180, 360)))
+        plt.close('all')
+
+    def test_matplotlib_transforms(self):
+        self.body.set_disc_params(2, 1, 3.5, 45.678)
+        self.body.set_img_size(15, 10)
+
+        # Test outputs
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_radec2xy_transform().get_matrix(),
+                array(
+                    [
+                        [-4.87014969e02, 5.01041735e02, 9.84267915e04],
+                        [4.98679564e02, 4.89321887e02, -9.52022315e04],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_xy2radec_transform().get_matrix(),
+                array(
+                    [
+                        [-1.00236708e-03, 1.02637498e-03, 1.96372964e02],
+                        [1.02153611e-03, 9.97641401e-04, -5.56883456e00],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_km2xy_transform().get_matrix(),
+                array(
+                    [
+                        [4.55744758e-05, 1.78803986e-05, 2.00000000e00],
+                        [-1.78803986e-05, 4.55744758e-05, 1.00000000e00],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_xy2km_transform().get_matrix(),
+                array(
+                    [
+                        [1.90151820e04, -7.46029498e03, -3.05700690e04],
+                        [7.46029498e03, 1.90151820e04, -3.39357720e04],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_radec2km_transform().get_matrix(),
+                array(
+                    [
+                        [-1.29809749e07, 5.87691418e06, 2.58180951e09],
+                        [5.84920736e06, 1.30424639e07, -1.07602880e09],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.matplotlib_km2radec_transform().get_matrix(),
+                array(
+                    [
+                        [-6.40343479e-08, 2.88537788e-08, 1.96371986e02],
+                        [2.87177471e-08, 6.37324567e-08, -5.56579385e00],
+                        [0.00000000e00, 0.00000000e00, 1.00000000e00],
+                    ]
+                ),
+            )
+        )
+
+        # Test caching works
+        fig, axis = plt.subplots()
+        for ax in [None, axis]:
+            for transform, attr in (
+                (self.body.matplotlib_radec2xy_transform, '_mpl_transform_radec2xy'),
+                (self.body.matplotlib_xy2radec_transform, '_mpl_transform_xy2radec'),
+                (self.body.matplotlib_km2xy_transform, '_mpl_transform_km2xy'),
+                (self.body.matplotlib_xy2km_transform, '_mpl_transform_xy2km'),
+                (self.body.matplotlib_radec2km_transform, '_mpl_transform_radec2km'),
+                (self.body.matplotlib_km2radec_transform, '_mpl_transform_km2radec'),
+            ):
+                with self.subTest(ax=ax, transform=transform, attr=attr):
+                    transform(ax)
+                    t1 = transform(ax)
+                    setattr(self.body, attr, None)
+                    t2 = transform(ax)
+                    self.assertEqual(t1, t2)
+
+        plt.close(fig)
+
+        # Test inverse
+        pairs = [
+            (
+                self.body.matplotlib_radec2xy_transform(),
+                self.body.matplotlib_xy2radec_transform(),
+            ),
+            (
+                self.body.matplotlib_km2xy_transform(),
+                self.body.matplotlib_xy2km_transform(),
+            ),
+            (
+                self.body.matplotlib_radec2km_transform(),
+                self.body.matplotlib_km2radec_transform(),
+            ),
+        ]
+        for t1, t2 in pairs:
+            self.assertTrue(np.allclose(t1.inverted().get_matrix(), t2.get_matrix()))
+            self.assertTrue(np.allclose(t2.inverted().get_matrix(), t1.get_matrix()))
+
+        # Test update
+        for transform in [
+            self.body.matplotlib_radec2xy_transform,
+            self.body.matplotlib_xy2radec_transform,
+            self.body.matplotlib_km2xy_transform,
+            self.body.matplotlib_xy2km_transform,
+        ]:
+            with self.subTest(transform=transform):
+                self.body.set_disc_params(10, 9, 8, 7)
+                self.body.update_transform()
+                m1 = transform().get_matrix()
+                self.body.set_disc_params(1.2, 3.4, 5.6, 178.9)
+                self.assertTrue(np.array_equal(m1, transform().get_matrix()))
+                self.body.update_transform()
+                self.assertFalse(np.array_equal(m1, transform().get_matrix()))
+
     # Backplane contents tested against FITS reference in test_observation
```

### Comparing `planetmapper-1.7.1/tests/test_data_loader.py` & `planetmapper-1.7.2/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/tests/test_kernel_downloader.py` & `planetmapper-1.7.2/tests/test_kernel_downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,7 +84,23 @@
                 'https://naif.jpl.nasa.gov/pub/naif/VIKING/kernels/spk/vo1_ext_gem.bsp',
                 'https://naif.jpl.nasa.gov/pub/naif/VIKING/kernels/spk/vo1_rcon.bsp',
                 'https://naif.jpl.nasa.gov/pub/naif/VIKING/kernels/spk/vo1_sedr.bsp',
                 'https://naif.jpl.nasa.gov/pub/naif/VIKING/kernels/spk/vo2_rcon.bsp',
                 'https://naif.jpl.nasa.gov/pub/naif/VIKING/kernels/spk/vo2_sedr.bsp',
             },
         )
+
+    def test_get_kernel_path(self):
+        self.assertEqual(
+            kernel_downloader._get_kernel_path(
+                'https://naif.jpl.nasa.gov/pub/abc/def/ghi.txt'
+            ),
+            kernel_downloader._standardise_path('abc/def/ghi.txt'),
+        )
+        with self.assertRaises(ValueError):
+            kernel_downloader._get_kernel_path('/abc/def/ghi')
+
+    def test_kernel_path_to_url(self):
+        self.assertEqual(
+            kernel_downloader._kernel_path_to_url('abc/def/ghi.txt'),
+            'https://naif.jpl.nasa.gov/pub/abc/def/ghi.txt',
+        )
```

### Comparing `planetmapper-1.7.1/tests/test_observation.py` & `planetmapper-1.7.2/tests/test_observation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import fnmatch
 import os
 import unittest
+import warnings
+from unittest.mock import MagicMock, patch
 
 import common_testing
 import numpy as np
 from astropy.io import fits
+from astropy.utils.exceptions import AstropyWarning
 
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
 from planetmapper import Observation
 
 
@@ -225,14 +228,55 @@
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
+        with self.subTest('data+header (DATE-OBS + TIME-OBS)'):
+            data = np.ones((5, 6, 7))
+            header = fits.Header(
+                {
+                    'OBJECT': 'jupiter',
+                    'TELESCOP': 'HST',
+                    'DATE-OBS': '2005-01-01',
+                    'TIME-OBS': '12:34',
+                }
+            )
+            obs = Observation(
+                data=data,
+                header=header,
+            )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
+            self.assertIsNone(obs.path)
+            self.assertEqual(obs.target, 'JUPITER')
+            self.assertEqual(obs.observer, 'HST')
+            self.assertEqual(obs.utc, '2005-01-01T12:34:00.000000')
+            self.assertEqual(obs.header, header)
+            self.assertTrue(np.array_equal(obs.data, data))
+
+        with self.subTest('empty.fits'):
+            path = os.path.join(common_testing.DATA_PATH, 'inputs', 'empty.fits')
+            with self.assertRaises(ValueError):
+                Observation(path)
+
+        with self.subTest('2d_image.fits (including MJD avg.)'):
+            path = os.path.join(common_testing.DATA_PATH, 'inputs', '2d_image.fits')
+            obs = Observation(path)
+            self.assertTrue(
+                np.array_equal(obs.data, np.array([[[1.0, 2.0], [3.0, 4.0]]]))
+            )
+            self.assertEqual(obs.utc, '2000-01-01T12:00:00.000000')
+
+        with self.subTest('2d_image.png'):
+            path = os.path.join(common_testing.DATA_PATH, 'inputs', '2d_image.png')
+            obs = Observation(path, target='JUPITER', utc='2000-01-01')
+            self.assertTrue(np.array_equal(obs.data, np.array([[[1, 2], [3, 4]]])))
+
     def test_attributes(self):
         self.assertEqual(self.observation.path, self.path)
         self.assertEqual(self.observation.target, 'JUPITER')
         self.assertEqual(self.observation.observer, 'HST')
         self.assertEqual(self.observation.utc, '2005-01-01T00:00:00.000000')
         self.assertEqual(self.observation._nx, 7)
         self.assertEqual(self.observation._ny, 10)
@@ -270,14 +314,48 @@
 
         obs.disc_from_header()
         self.assertAlmostEqual(obs.get_x0(), 1.1)
         self.assertAlmostEqual(obs.get_y0(), 2.2)
         self.assertAlmostEqual(obs.get_r0(), 3.3)
         self.assertAlmostEqual(obs.get_rotation(), 4.4)
 
+        data = np.ones((5, 6, 7))
+        header = fits.Header(
+            {
+                'OBJECT': 'jupiter',
+                'DATE-OBS': '2005-01-01',
+                'PLANMAP DEGREE-INTERVAL': 1,
+            }
+        )
+        obs = Observation(data=data, header=header)
+        with self.assertRaises(ValueError):
+            obs.disc_from_header()
+
+        del header['PLANMAP DEGREE-INTERVAL']
+        header['PLANMAP MAP PROJECTION'] = 'rectangular'
+        obs = Observation(data=data, header=header)
+        with self.assertRaises(ValueError):
+            obs.disc_from_header()
+
+        header['PLANMAP DISC X0'] = 1
+        header['PLANMAP DISC Y0'] = 2
+        header['PLANMAP DISC R0'] = 3
+        header['PLANMAP DISC ROT'] = 4
+        obs = Observation(data=data, header=header)
+        with self.assertRaises(ValueError):
+            obs.disc_from_header()
+
+        del header['PLANMAP MAP PROJECTION']
+        obs = Observation(data=data, header=header)
+        obs.disc_from_header()
+        self.assertAlmostEqual(obs.get_x0(), 1)
+        self.assertAlmostEqual(obs.get_y0(), 2)
+        self.assertAlmostEqual(obs.get_r0(), 3)
+        self.assertAlmostEqual(obs.get_rotation(), 4)
+
     def test_stuff_from_wcs(self):
         with self.assertRaises(ValueError):
             self.observation.disc_from_wcs(suppress_warnings=True)
         with self.assertRaises(ValueError):
             self.observation.position_from_wcs(suppress_warnings=True)
         with self.assertRaises(ValueError):
             self.observation.rotation_from_wcs(suppress_warnings=True)
@@ -316,14 +394,61 @@
         self.assertAlmostEqual(obs.get_rotation(), rotation, delta=0.2)
 
         obs.set_disc_params(0, 0, 1, 0)
         obs.plate_scale_from_wcs(suppress_warnings=True)
         self.assertEqual(obs.get_disc_method(), 'wcs_plate_scale')
         self.assertAlmostEqual(obs.get_r0(), r0, delta=0.2)
 
+        data = np.ones((5, 6, 7))
+        header = fits.Header(
+            {
+                'OBJECT': 'jupiter',
+                'DATE-OBS': '2005-01-01',
+                'CRPIX1': 1,
+                'CRPIX2': 1,
+                'CRVAL1': 196.3,
+                'CRVAL2': -5.5,
+                'CDELT1': 1,
+                'CDELT2': 1,
+                'CTYPE1': 'RA---TAN',
+                'CTYPE2': 'DEC--TAN',
+                'CUNIT1': 'deg',
+                'CUNIT2': 'deg',
+            }
+        )
+        obs = Observation(data=data, header=header)
+        obs.disc_from_wcs(suppress_warnings=True)
+
+        h2 = header.copy()
+        h2['CTYPE1'] = 'DEC--TAN'
+        obs = Observation(data=data, header=h2)
+        with self.assertRaises(ValueError):
+            obs.disc_from_wcs(suppress_warnings=True)
+
+        h2 = header.copy()
+        h2['A_ORDER'] = 2
+        h2['B_ORDER'] = 2
+        for n in range(3):
+            for m in range(3):
+                h2[f'A_{n}_{m}'] = 0.1
+                h2[f'B_{n}_{m}'] = 0.2
+        obs = Observation(data=data, header=h2)
+        with self.assertRaises(ValueError):
+            obs.disc_from_wcs(suppress_warnings=True)
+        obs.disc_from_wcs(validate=False, suppress_warnings=True)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('always')
+            with self.assertWarns(AstropyWarning):
+                obs.disc_from_wcs(validate=False, suppress_warnings=False)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('error')
+            obs.position_from_wcs(validate=False, suppress_warnings=True)
+
     def test_fit_disc(self):
         data = np.ones((5, 10, 8))
         data[:, 3:5, 2:4] = 10
         obs = Observation(
             data=data,
             target='Jupiter',
             observer='hst',
@@ -338,14 +463,31 @@
 
         obs.fit_disc_radius()
         self.assertAlmostEqual(obs.get_r0(), 1.5)
         self.assertEqual(obs.get_disc_method(), 'fit_r0')
 
         self.assertAlmostEqual(obs.get_rotation(), 99)
 
+        obs = Observation(
+            data=np.ones((300, 300)),
+            target='Jupiter',
+            observer='hst',
+            utc='2005-01-01T00:00:00',
+        )
+        obs.set_disc_params(x0=-1)
+        with self.assertRaises(ValueError):
+            obs.fit_disc_radius()
+
+        obs.set_disc_params(x0=1, y0=301)
+        with self.assertRaises(ValueError):
+            obs.fit_disc_radius()
+
+        obs.set_disc_params(x0=150, y0=150)
+        obs.fit_disc_radius()
+
     # get_mapped_data tested against output references
 
     def test_append_to_header(self):
         obs = Observation(
             data=np.ones((5, 10, 8)),
             target='Jupiter',
             observer='hst',
@@ -358,28 +500,68 @@
             obs.header.comments['HIERARCH PLANMAP TESTING'], 'Testing comment'
         )
 
         header = fits.Header()
         obs.append_to_header('TESTING', 123, 'Testing comment', header=header)
         self.assertEqual(header['HIERARCH PLANMAP TESTING'], 123)
         self.assertEqual(header.comments['HIERARCH PLANMAP TESTING'], 'Testing comment')
+        self.assertNotIn('TESTING', header)
+
+        header = fits.Header()
+        obs.append_to_header(
+            'TESTING', 123, 'Testing comment', header=header, hierarch_keyword=False
+        )
+        self.assertEqual(header['TESTING'], 123)
+        self.assertEqual(header.comments['TESTING'], 'Testing comment')
+        self.assertNotIn('HIERARCH PLANMAP TESTING', header)
+
+        header = fits.Header()
+        obs.append_to_header('A', 0, header=header, hierarch_keyword=False)
+        obs.append_to_header('B', 1, header=header, hierarch_keyword=False)
+        obs.append_to_header('A', 1, header=header, hierarch_keyword=False)
+        self.assertEqual(header['A'], 1)
+        self.assertEqual(list(header.keys()), ['B', 'A'])
+
+        header = fits.Header()
+        obs.append_to_header('A', 0, header=header, hierarch_keyword=False)
+        obs.append_to_header('B', 1, header=header, hierarch_keyword=False)
+        obs.append_to_header(
+            'A', 1, header=header, hierarch_keyword=False, remove_existing=False
+        )
+        self.assertEqual(header['A'], 0)
+        self.assertEqual(list(header.keys()), ['A', 'B', 'A'])
 
         for n in range(100):
             with self.subTest(n=n):
                 s = 'x' * n
                 obs.append_to_header('TESTING', s)
                 if n >= 53:
                     s = 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx...'
                 self.assertEqual(obs.header['HIERARCH PLANMAP TESTING'], s)
 
         with self.assertRaises(ValueError):
             obs.append_to_header('TESTING', 'x' * 100, truncate_strings=False)
             obs.header.tostring()
 
-    # add_header_metadata tested against output references
+    def test_add_header_metadata(self):
+        obs = planetmapper.Observation(
+            data=np.ones((5, 10, 8)),
+            target='Jupiter',
+            observer='hst',
+            utc='2005-01-01T00:00:00',
+        )
+        obs.add_header_metadata()
+        self.assertNotIn('HIERARCH PLANMAP INFILE', obs.header)
+
+        path = os.path.join(common_testing.DATA_PATH, 'inputs', 'test.fits')
+        obs = planetmapper.Observation(path)
+        obs.add_header_metadata()
+        self.assertEqual(obs.header['HIERARCH PLANMAP INFILE'], os.path.split(path)[1])
+
+        # add_header_metadata also tested against output references
 
     def test_make_filename(self):
         self.assertEqual(
             self.observation.make_filename(), 'JUPITER_2005-01-01T000000.fits'
         )
         self.assertEqual(
             self.observation.make_filename(extension='.txt'),
@@ -392,14 +574,22 @@
 
     def test_save_observation(self):
         self.observation.set_disc_params(2.5, 3.1, 3.9, 123.456)
         self.observation.set_disc_method('<<<test>>>')
 
         path = os.path.join(common_testing.TEMP_PATH, 'test_nav.fits')
 
+        # test skip wireframe here
+        self.observation.save_observation(
+            path,
+            show_progress=True,
+            include_wireframe=False,
+        )
+        self.compare_fits_to_reference(path, skip_wireframe=True)
+
         # test print info here
         self.observation.save_observation(
             path, print_info=True, wireframe_kwargs=dict(output_size=20, dpi=20)
         )
         self.compare_fits_to_reference(path)
 
         # test progress bar here too
@@ -469,18 +659,22 @@
             ):
                 path = os.path.join(common_testing.TEMP_PATH, f'map_{map_type}.fits')
                 self.observation.save_mapped_observation(
                     path, **map_kw, wireframe_kwargs=dict(output_size=20, dpi=20)
                 )
                 self.compare_fits_to_reference(path)
 
-    def compare_fits_to_reference(self, path: str):
+    def compare_fits_to_reference(self, path: str, skip_wireframe: bool = False):
         filename = os.path.basename(path)
         path_ref = os.path.join(common_testing.DATA_PATH, 'outputs', filename)
         with fits.open(path) as hdul, fits.open(path_ref) as hdul_ref:
+            if skip_wireframe:
+                hdul_ref = fits.HDUList(
+                    [hdu for hdu in hdul_ref if hdu.name != 'WIREFRAME']
+                )
             with self.subTest('Number of backplanes', filename=filename):
                 self.assertEqual(len(hdul), len(hdul_ref))
             for hdu, hdu_ref in zip(hdul, hdul_ref):
                 self.assertEqual(hdu.name, hdu_ref.name)
                 extname = hdu.name
                 with self.subTest(filename=filename, extname=extname):
                     data = hdu.data
@@ -512,7 +706,13 @@
                     value = header[key]
                     value_ref = header_ref[key]
                     with self.subTest(filename=filename, extname=extname, key=key):
                         if isinstance(value, float):
                             self.assertAlmostEqual(value, value_ref)
                         else:
                             self.assertEqual(value, value_ref)
+
+    @patch('planetmapper.gui.GUI.run')
+    def test_run_gui(self, mock_run: MagicMock):
+        out = self.observation.run_gui()
+        self.assertEqual(out, [])
+        mock_run.assert_called_once()
```

### Comparing `planetmapper-1.7.1/tests/test_progress.py` & `planetmapper-1.7.2/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.1/tests/test_utils.py` & `planetmapper-1.7.2/tests/test_utils.py`

 * *Files identical despite different names*

