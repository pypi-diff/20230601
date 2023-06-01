# Comparing `tmp/testghapythonpackage-0.0.8.tar.gz` & `tmp/testghapythonpackage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testghapythonpackage-0.0.8.tar", last modified: Thu Dec  1 05:19:27 2022, max compression
+gzip compressed data, was "testghapythonpackage-0.0.9.tar", last modified: Sun Jan  1 05:16:24 2023, max compression
```

## Comparing `testghapythonpackage-0.0.8.tar` & `testghapythonpackage-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.610743 testghapythonpackage-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.606743 testghapythonpackage-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.606743 testghapythonpackage-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/FILESTRUCTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2022-12-01 05:19:27.610743 testghapythonpackage-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/TODO.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.606743 testghapythonpackage-0.0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/doc/demo.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/doc/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      759 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.606743 testghapythonpackage-0.0.8/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-01 05:19:27.610743 testghapythonpackage-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.606743 testghapythonpackage-0.0.8/testghapythonpackage/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/testghapythonpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-01 05:19:27.000000 testghapythonpackage-0.0.8/testghapythonpackage/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.610743 testghapythonpackage-0.0.8/testghapythonpackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2022-12-01 05:19:27.000000 testghapythonpackage-0.0.8/testghapythonpackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-01 05:19:27.000000 testghapythonpackage-0.0.8/testghapythonpackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 05:19:27.000000 testghapythonpackage-0.0.8/testghapythonpackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-01 05:19:27.000000 testghapythonpackage-0.0.8/testghapythonpackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-01 05:19:27.000000 testghapythonpackage-0.0.8/testghapythonpackage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:27.610743 testghapythonpackage-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-01 05:19:14.000000 testghapythonpackage-0.0.8/tests/test_testghapythonpackage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.299326 testghapythonpackage-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.299326 testghapythonpackage-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/FILESTRUCTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/doc/demo.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/doc/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/testghapythonpackage/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/testghapythonpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-01 05:16:24.000000 testghapythonpackage-0.0.9/testghapythonpackage/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/testghapythonpackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-01 05:16:24.000000 testghapythonpackage-0.0.9/testghapythonpackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-01 05:16:24.000000 testghapythonpackage-0.0.9/testghapythonpackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 05:16:24.000000 testghapythonpackage-0.0.9/testghapythonpackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-01 05:16:24.000000 testghapythonpackage-0.0.9/testghapythonpackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-01 05:16:24.000000 testghapythonpackage-0.0.9/testghapythonpackage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:24.303326 testghapythonpackage-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-01 05:16:15.000000 testghapythonpackage-0.0.9/tests/test_testghapythonpackage.py
```

### Comparing `testghapythonpackage-0.0.8/.github/workflows/ci.yml` & `testghapythonpackage-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/.github/workflows/pypi.yml` & `testghapythonpackage-0.0.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/.gitignore` & `testghapythonpackage-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/.pre-commit-config.yaml` & `testghapythonpackage-0.0.9/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 repos:
   # Run Black - the uncompromising Python code formatter
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 22.12.0
     hooks:
       - id: black-jupyter
 
   # Add some general purpose useful hooks
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       # Make sure that contained YAML files are well-formed
       - id: check-yaml
       # Trim trailing whitespace of all sorts
       - id: trailing-whitespace
       # Apply a file size limit of 500kB
       - id: check-added-large-files
```

### Comparing `testghapythonpackage-0.0.8/FILESTRUCTURE.md` & `testghapythonpackage-0.0.9/FILESTRUCTURE.md`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/LICENSE.md` & `testghapythonpackage-0.0.9/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022, The copyright holders according to COPYING.md
+Copyright 2023, The copyright holders according to COPYING.md
 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `testghapythonpackage-0.0.8/PKG-INFO` & `testghapythonpackage-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testghapythonpackage
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add short description here
 Maintainer-email: Your Name <your@email.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
@@ -12,15 +12,15 @@
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # Welcome to My Python Project
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dokempf/test-gha-python-package/CI)](https://github.com/dokempf/test-gha-python-package/actions?query=workflow%3ACI)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dokempf/test-gha-python-package/ci.yml?branch=main)](https://github.com/dokempf/test-gha-python-package/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/test-gha-python-package/badge/)](https://test-gha-python-package.readthedocs.io/)
 [![codecov](https://codecov.io/gh/dokempf/test-gha-python-package/branch/main/graph/badge.svg)](https://codecov.io/gh/dokempf/test-gha-python-package)
 
 ## Installation
 
 The Python packaage `testghapythonpackage` can be installed from PyPI:
```

### Comparing `testghapythonpackage-0.0.8/README.md` & `testghapythonpackage-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Welcome to My Python Project
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dokempf/test-gha-python-package/CI)](https://github.com/dokempf/test-gha-python-package/actions?query=workflow%3ACI)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dokempf/test-gha-python-package/ci.yml?branch=main)](https://github.com/dokempf/test-gha-python-package/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/test-gha-python-package/badge/)](https://test-gha-python-package.readthedocs.io/)
 [![codecov](https://codecov.io/gh/dokempf/test-gha-python-package/branch/main/graph/badge.svg)](https://codecov.io/gh/dokempf/test-gha-python-package)
 
 ## Installation
 
 The Python packaage `testghapythonpackage` can be installed from PyPI:
```

### Comparing `testghapythonpackage-0.0.8/TODO.md` & `testghapythonpackage-0.0.9/TODO.md`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/doc/Makefile` & `testghapythonpackage-0.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/doc/conf.py` & `testghapythonpackage-0.0.9/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 
 # -- Project information -----------------------------------------------------
 
 project = "test-gha-python-package"
-copyright = "2022, Your Name"
+copyright = "2023, Your Name"
 author = "Your Name"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `testghapythonpackage-0.0.8/doc/make.bat` & `testghapythonpackage-0.0.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/notebooks/demo.ipynb` & `testghapythonpackage-0.0.9/notebooks/demo.ipynb`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/pyproject.toml` & `testghapythonpackage-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `testghapythonpackage-0.0.8/testghapythonpackage.egg-info/PKG-INFO` & `testghapythonpackage-0.0.9/testghapythonpackage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testghapythonpackage
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add short description here
 Maintainer-email: Your Name <your@email.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
@@ -12,15 +12,15 @@
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # Welcome to My Python Project
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dokempf/test-gha-python-package/CI)](https://github.com/dokempf/test-gha-python-package/actions?query=workflow%3ACI)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dokempf/test-gha-python-package/ci.yml?branch=main)](https://github.com/dokempf/test-gha-python-package/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/test-gha-python-package/badge/)](https://test-gha-python-package.readthedocs.io/)
 [![codecov](https://codecov.io/gh/dokempf/test-gha-python-package/branch/main/graph/badge.svg)](https://codecov.io/gh/dokempf/test-gha-python-package)
 
 ## Installation
 
 The Python packaage `testghapythonpackage` can be installed from PyPI:
```

### Comparing `testghapythonpackage-0.0.8/testghapythonpackage.egg-info/SOURCES.txt` & `testghapythonpackage-0.0.9/testghapythonpackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

