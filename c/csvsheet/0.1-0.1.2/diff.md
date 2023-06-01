# Comparing `tmp/csvsheet-0.1.tar.gz` & `tmp/csvsheet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvsheet-0.1.tar", last modified: Mon May 15 10:20:35 2023, max compression
+gzip compressed data, was "csvsheet-0.1.2.tar", last modified: Thu Jun  1 07:32:53 2023, max compression
```

## Comparing `csvsheet-0.1.tar` & `csvsheet-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.521126 csvsheet-0.1/
--rw-r--r--   0 jesus      (501) staff       (20)      591 2023-05-12 06:31:50.000000 csvsheet-0.1/.coveragerc
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.509856 csvsheet-0.1/.github/
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.514103 csvsheet-0.1/.github/workflows/
--rw-r--r--   0 jesus      (501) staff       (20)     4349 2023-05-15 09:25:16.000000 csvsheet-0.1/.github/workflows/ci.yml
--rw-r--r--   0 jesus      (501) staff       (20)      566 2023-05-12 06:31:50.000000 csvsheet-0.1/.gitignore
--rw-r--r--   0 jesus      (501) staff       (20)       56 2023-05-12 06:31:50.000000 csvsheet-0.1/.isort.cfg
--rw-r--r--   0 jesus      (501) staff       (20)     1344 2023-05-14 19:51:30.000000 csvsheet-0.1/.pre-commit-config.yaml
--rw-r--r--   0 jesus      (501) staff       (20)      530 2023-05-12 06:31:50.000000 csvsheet-0.1/.readthedocs.yml
--rw-r--r--   0 jesus      (501) staff       (20)       80 2023-05-12 06:31:50.000000 csvsheet-0.1/AUTHORS.rst
--rw-r--r--   0 jesus      (501) staff       (20)      128 2023-05-12 06:31:50.000000 csvsheet-0.1/CHANGELOG.rst
--rw-r--r--   0 jesus      (501) staff       (20)    12791 2023-05-12 10:11:01.000000 csvsheet-0.1/CONTRIBUTING.rst
--rw-r--r--   0 jesus      (501) staff       (20)     1081 2023-05-12 06:31:50.000000 csvsheet-0.1/LICENSE.txt
--rw-r--r--   0 jesus      (501) staff       (20)     4374 2023-05-15 10:20:35.521243 csvsheet-0.1/PKG-INFO
--rw-r--r--   0 jesus      (501) staff       (20)     3680 2023-05-12 09:55:49.000000 csvsheet-0.1/README.rst
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.516785 csvsheet-0.1/docs/
--rw-r--r--   0 jesus      (501) staff       (20)     1154 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/Makefile
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.517000 csvsheet-0.1/docs/_static/
--rw-r--r--   0 jesus      (501) staff       (20)       18 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/_static/.gitignore
--rw-r--r--   0 jesus      (501) staff       (20)       41 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/authors.rst
--rw-r--r--   0 jesus      (501) staff       (20)       43 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/changelog.rst
--rw-r--r--   0 jesus      (501) staff       (20)     9743 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/conf.py
--rw-r--r--   0 jesus      (501) staff       (20)       33 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/contributing.rst
--rw-r--r--   0 jesus      (501) staff       (20)     1657 2023-05-12 10:12:07.000000 csvsheet-0.1/docs/index.rst
--rw-r--r--   0 jesus      (501) staff       (20)       67 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/license.rst
--rw-r--r--   0 jesus      (501) staff       (20)       39 2023-05-15 09:25:16.000000 csvsheet-0.1/docs/readme.rst
--rw-r--r--   0 jesus      (501) staff       (20)      233 2023-05-12 06:31:50.000000 csvsheet-0.1/docs/requirements.txt
--rw-r--r--   0 jesus      (501) staff       (20)      346 2023-05-12 06:31:50.000000 csvsheet-0.1/pyproject.toml
--rw-r--r--   0 jesus      (501) staff       (20)     1448 2023-05-15 10:20:35.521694 csvsheet-0.1/setup.cfg
--rw-r--r--   0 jesus      (501) staff       (20)      684 2023-05-15 09:25:40.000000 csvsheet-0.1/setup.py
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.510205 csvsheet-0.1/src/
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.518088 csvsheet-0.1/src/csvsheet/
--rw-r--r--   0 jesus      (501) staff       (20)      577 2023-05-15 09:25:16.000000 csvsheet-0.1/src/csvsheet/__init__.py
--rw-r--r--   0 jesus      (501) staff       (20)      605 2023-05-12 06:31:50.000000 csvsheet-0.1/src/csvsheet/__init__.py,cover
--rw-r--r--   0 jesus      (501) staff       (20)     7354 2023-05-14 19:54:33.000000 csvsheet-0.1/src/csvsheet/csvsheet.py
--rw-r--r--   0 jesus      (501) staff       (20)     7910 2023-05-12 06:31:50.000000 csvsheet-0.1/src/csvsheet/csvsheet.py,cover
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.519251 csvsheet-0.1/src/csvsheet.egg-info/
--rw-r--r--   0 jesus      (501) staff       (20)     4374 2023-05-15 10:20:35.000000 csvsheet-0.1/src/csvsheet.egg-info/PKG-INFO
--rw-r--r--   0 jesus      (501) staff       (20)      881 2023-05-15 10:20:35.000000 csvsheet-0.1/src/csvsheet.egg-info/SOURCES.txt
--rw-r--r--   0 jesus      (501) staff       (20)        1 2023-05-15 10:20:35.000000 csvsheet-0.1/src/csvsheet.egg-info/dependency_links.txt
--rw-r--r--   0 jesus      (501) staff       (20)       51 2023-05-15 10:20:35.000000 csvsheet-0.1/src/csvsheet.egg-info/entry_points.txt
--rw-r--r--   0 jesus      (501) staff       (20)        1 2023-05-12 09:57:01.000000 csvsheet-0.1/src/csvsheet.egg-info/not-zip-safe
--rw-r--r--   0 jesus      (501) staff       (20)       86 2023-05-15 10:20:35.000000 csvsheet-0.1/src/csvsheet.egg-info/requires.txt
--rw-r--r--   0 jesus      (501) staff       (20)        9 2023-05-15 10:20:35.000000 csvsheet-0.1/src/csvsheet.egg-info/top_level.txt
-drwxr-xr-x   0 jesus      (501) staff       (20)        0 2023-05-15 10:20:35.520883 csvsheet-0.1/tests/
--rw-r--r--   0 jesus      (501) staff       (20)      255 2023-05-14 19:32:49.000000 csvsheet-0.1/tests/conftest.py
--rw-r--r--   0 jesus      (501) staff       (20)       98 2023-05-12 06:31:50.000000 csvsheet-0.1/tests/test_a.csv
--rw-r--r--   0 jesus      (501) staff       (20)       67 2023-05-15 10:18:02.000000 csvsheet-0.1/tests/test_a.csv.out
--rw-r--r--   0 jesus      (501) staff       (20)       98 2023-05-12 06:31:50.000000 csvsheet-0.1/tests/test_a.ssv
--rw-r--r--   0 jesus      (501) staff       (20)       56 2023-05-12 06:31:50.000000 csvsheet-0.1/tests/test_b.csv
--rw-r--r--   0 jesus      (501) staff       (20)      103 2023-05-12 06:31:50.000000 csvsheet-0.1/tests/test_c.csv
--rw-r--r--   0 jesus      (501) staff       (20)     2769 2023-05-14 19:55:00.000000 csvsheet-0.1/tests/test_csvsheet.py
--rw-r--r--   0 jesus      (501) staff       (20)     2862 2023-05-12 06:31:50.000000 csvsheet-0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.738346 csvsheet-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-01 07:31:57.000000 csvsheet-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.730347 csvsheet-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.730347 csvsheet-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-01 07:31:57.000000 csvsheet-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 07:31:57.000000 csvsheet-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 07:31:57.000000 csvsheet-0.1.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-01 07:31:57.000000 csvsheet-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 07:31:57.000000 csvsheet-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 07:31:57.000000 csvsheet-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-01 07:31:57.000000 csvsheet-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-06-01 07:31:57.000000 csvsheet-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 07:31:57.000000 csvsheet-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-01 07:32:53.738346 csvsheet-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-01 07:31:57.000000 csvsheet-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.734346 csvsheet-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.734346 csvsheet-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-01 07:31:57.000000 csvsheet-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 07:31:57.000000 csvsheet-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-01 07:32:53.738346 csvsheet-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-01 07:31:57.000000 csvsheet-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.730347 csvsheet-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.734346 csvsheet-0.1.2/src/csvsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-01 07:31:57.000000 csvsheet-0.1.2/src/csvsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-01 07:31:57.000000 csvsheet-0.1.2/src/csvsheet/__init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-06-01 07:31:57.000000 csvsheet-0.1.2/src/csvsheet/csvsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-01 07:31:57.000000 csvsheet-0.1.2/src/csvsheet/csvsheet.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.734346 csvsheet-0.1.2/src/csvsheet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-01 07:32:53.000000 csvsheet-0.1.2/src/csvsheet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-01 07:32:53.000000 csvsheet-0.1.2/src/csvsheet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:32:53.000000 csvsheet-0.1.2/src/csvsheet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 07:32:53.000000 csvsheet-0.1.2/src/csvsheet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:32:53.000000 csvsheet-0.1.2/src/csvsheet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-01 07:32:53.000000 csvsheet-0.1.2/src/csvsheet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 07:32:53.000000 csvsheet-0.1.2/src/csvsheet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:32:53.738346 csvsheet-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-01 07:31:57.000000 csvsheet-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 07:31:57.000000 csvsheet-0.1.2/tests/test_a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 07:31:57.000000 csvsheet-0.1.2/tests/test_a.ssv
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 07:31:57.000000 csvsheet-0.1.2/tests/test_b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 07:31:57.000000 csvsheet-0.1.2/tests/test_c.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-01 07:31:57.000000 csvsheet-0.1.2/tests/test_csvsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-01 07:31:57.000000 csvsheet-0.1.2/tox.ini
```

### Comparing `csvsheet-0.1/.coveragerc` & `csvsheet-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/.github/workflows/ci.yml` & `csvsheet-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/.gitignore` & `csvsheet-0.1.2/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -48,7 +48,10 @@
 cover/*
 MANIFEST
 
 # Per-project virtualenvs
 .venv*/
 .conda*/
 .python-version
+
+# hypothesis
+.hypothesis/
```

### Comparing `csvsheet-0.1/.pre-commit-config.yaml` & `csvsheet-0.1.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   rev: v1.2.0
   hooks:
   - id: csvlint
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   rev: "v0.0.265"
   hooks:
   - id: ruff
-    args: [--show-source, --fix, --exit-non-zero-on-fix, --select=E, --select=F, --select=B, --select=W, --select=N, --select=EM, --select=EXE, --select=PYI, --select=PT, --select=Q, --select=RET]
+    args: [--show-source, --fix, --exit-non-zero-on-fix, --select=E, --select=F, --select=B, --select=W, --select=N, --select=EM, --select=EXE, --select=PYI, --select=PT, --select=Q, --select=RET, --select=SIM]
 - repo: https://github.com/Zac-HD/shed
   rev: 2023.5.1
   hooks:
   - id: shed
     # args: [--refactor, --py39-plus]
     types_or: [python, pyi, markdown, rst]
 # - repo: https://github.com/PyCQA/bandit
```

### Comparing `csvsheet-0.1/.readthedocs.yml` & `csvsheet-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/CONTRIBUTING.rst` & `csvsheet-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/LICENSE.txt` & `csvsheet-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/PKG-INFO` & `csvsheet-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvsheet
-Version: 0.1
+Version: 0.1.2
 Summary: Simple formula support for CSV
 Home-page: https://github.com/jtplaarj/csvsheet/
 Author: Jesús Lázaro
 Author-email: jesus.lazaro@ehu.eus
 License: MIT
 Project-URL: Documentation, https://csvsheet.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/jtplaarj/csvsheet/
@@ -19,20 +19,14 @@
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/csvsheet.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/csvsheet
-    .. image:: https://readthedocs.org/projects/csvsheet/badge/?version=latest
-        :alt: ReadTheDocs
-        :target: https://csvsheet.readthedocs.io/en/stable/
-    .. image:: https://img.shields.io/coveralls/github/<USER>/csvsheet/main.svg
-        :alt: Coveralls
-        :target: https://coveralls.io/r/<USER>/csvsheet
     .. image:: https://img.shields.io/conda/vn/conda-forge/csvsheet.svg
         :alt: Conda-Forge
         :target: https://anaconda.org/conda-forge/csvsheet
     .. image:: https://pepy.tech/badge/csvsheet/month
         :alt: Monthly Downloads
         :target: https://pepy.tech/project/csvsheet
     .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
@@ -40,19 +34,24 @@
         :target: https://twitter.com/csvsheet
 .. image:: https://readthedocs.org/projects/csvsheet/badge/?version=latest
     :alt: ReadTheDocs
     :target: https://csvsheet.readthedocs.io/en/stable/
 .. image:: https://img.shields.io/pypi/v/csvsheet.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/csvsheet/
+.. image:: https://img.shields.io/coveralls/github/jtplaarj/csvsheet/main.svg
+    :alt: Coveralls
+    :target: https://coveralls.io/r/jtplaarj/csvsheet
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
+.. image:: https://img.shields.io/coveralls/github/jtplaarj/csvsheet/main.svg
+    :alt: Coveralls
+    :target: https://coveralls.io/r/jtplaarj/csvsheet
 
-|
 
 ========
 csvsheet
 ========
 
 
     Simple formula support for CSV
@@ -69,21 +68,24 @@
 ==================
 
 The command line requires a single compulsory arugment, the CSV fileto process::
 
     csvsheet <file.csv> -o <output.csv> -d <delimiter> -q <quotechar> -m <equation_delimiter> -v -vv
     csvsheet --help
 
+The input file is required, if '-' is used, stdin is used.
 The output file is optional, if not provided, the output will be printed to stdout.
 The delimiter is also optional, if not provided, the default delimiter is `,`.
 The quotechar is also optional, if not provided, the default quotechar is `"`.
 The equation delimiter is also optional, if not provided, the default equation delimiter is `=`.
 
 The `-v` and `-vv` flags are optional, they are used to increase the verbosity of the output.
 
+Read the `extended docs`_ for extra information.
+
 Example
 =======
 
 The following example shows how to use the command line::
 
     csvsheet example.csv
 
@@ -130,7 +132,9 @@
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
+
+.. _extended docs: https://csvsheet.readthedocs.io/en/stable/
```

### Comparing `csvsheet-0.1/README.rst` & `csvsheet-0.1.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/csvsheet.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/csvsheet
-    .. image:: https://readthedocs.org/projects/csvsheet/badge/?version=latest
-        :alt: ReadTheDocs
-        :target: https://csvsheet.readthedocs.io/en/stable/
-    .. image:: https://img.shields.io/coveralls/github/<USER>/csvsheet/main.svg
-        :alt: Coveralls
-        :target: https://coveralls.io/r/<USER>/csvsheet
     .. image:: https://img.shields.io/conda/vn/conda-forge/csvsheet.svg
         :alt: Conda-Forge
         :target: https://anaconda.org/conda-forge/csvsheet
     .. image:: https://pepy.tech/badge/csvsheet/month
         :alt: Monthly Downloads
         :target: https://pepy.tech/project/csvsheet
     .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
@@ -21,19 +15,24 @@
         :target: https://twitter.com/csvsheet
 .. image:: https://readthedocs.org/projects/csvsheet/badge/?version=latest
     :alt: ReadTheDocs
     :target: https://csvsheet.readthedocs.io/en/stable/
 .. image:: https://img.shields.io/pypi/v/csvsheet.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/csvsheet/
+.. image:: https://img.shields.io/coveralls/github/jtplaarj/csvsheet/main.svg
+    :alt: Coveralls
+    :target: https://coveralls.io/r/jtplaarj/csvsheet
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
+.. image:: https://img.shields.io/coveralls/github/jtplaarj/csvsheet/main.svg
+    :alt: Coveralls
+    :target: https://coveralls.io/r/jtplaarj/csvsheet
 
-|
 
 ========
 csvsheet
 ========
 
 
     Simple formula support for CSV
@@ -50,21 +49,24 @@
 ==================
 
 The command line requires a single compulsory arugment, the CSV fileto process::
 
     csvsheet <file.csv> -o <output.csv> -d <delimiter> -q <quotechar> -m <equation_delimiter> -v -vv
     csvsheet --help
 
+The input file is required, if '-' is used, stdin is used.
 The output file is optional, if not provided, the output will be printed to stdout.
 The delimiter is also optional, if not provided, the default delimiter is `,`.
 The quotechar is also optional, if not provided, the default quotechar is `"`.
 The equation delimiter is also optional, if not provided, the default equation delimiter is `=`.
 
 The `-v` and `-vv` flags are optional, they are used to increase the verbosity of the output.
 
+Read the `extended docs`_ for extra information.
+
 Example
 =======
 
 The following example shows how to use the command line::
 
     csvsheet example.csv
 
@@ -111,7 +113,9 @@
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
+
+.. _extended docs: https://csvsheet.readthedocs.io/en/stable/
```

### Comparing `csvsheet-0.1/docs/Makefile` & `csvsheet-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/docs/conf.py` & `csvsheet-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/docs/index.rst` & `csvsheet-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/setup.cfg` & `csvsheet-0.1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
+	hypothesis
 	pytest-cov
+	pytest-mock
+	faker
 
 [options.entry_points]
 console_scripts = 
 	csvsheet = csvsheet.csvsheet:run
 
 [tool:pytest]
 addopts =
```

### Comparing `csvsheet-0.1/setup.py` & `csvsheet-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/src/csvsheet/__init__.py` & `csvsheet-0.1.2/src/csvsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/src/csvsheet/__init__.py,cover` & `csvsheet-0.1.2/src/csvsheet/__init__.py,cover`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/src/csvsheet/csvsheet.py` & `csvsheet-0.1.2/src/csvsheet/csvsheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 # when using this Python module as a library.
 
 
 def sanitize_cell(cell: str, mathdelimiter: str = "=") -> str:
     """Sanitize a cell.
 
     Args:
-    ----
+    -----
         cell (str): string from CSV cell
         mathdelimiter (str, optional): delimiter to identify formulas. Defaults to "=".
 
     Raises:
-    ------
+    -------
         ValueError: cell contains invalid functions
 
     Returns:
-    -------
+    --------
         str: Sanitized string to be used in eval()
     """
     if cell.startswith(mathdelimiter):
         # formula!!!
         # remove the '='
         cell = cell[1:]
         # eliminate all spaces
@@ -86,27 +86,27 @@
 # executable/script.
 
 
 def parse_args(args: list[str]) -> argparse.Namespace:
     """Parse command line parameters.
 
     Args:
-    ----
+    -----
       args (List[str]): command line parameters as list of strings
           (for example  ``["--help"]``).
 
     Returns:
-    -------
+    --------
       :obj:`argparse.Namespace`: command line parameters namespace
     """
     parser = argparse.ArgumentParser(description="Just a Fibonacci demonstration")
     # add input file as positional argument
     parser.add_argument(
         "input",
-        help="Input CSV file to read",
+        help="Input CSV file to read. '-' for stdin",
         type=argparse.FileType("r"),
         metavar="INPUT_FILE",
     )
     parser.add_argument(
         "--version",
         action="version",
         version=f"csvsheet {__version__}",
@@ -114,15 +114,15 @@
     parser.add_argument(
         "-o",
         "--output",
         dest="output",
         help="Output file to write result, if none given, \
             it will be writen to stdout",
         default="-",
-        type=str,
+        type=argparse.FileType("w"),
         metavar="OUTPUT_FILE",
     )
     parser.add_argument(
         "-d",
         "--delimiter",
         dest="delimiter",
         help="CSV file delimiter, default is ','",
@@ -167,28 +167,28 @@
     return parser.parse_args(args)
 
 
 def setup_logging(loglevel: int):
     """Setup basic logging.
 
     Args:
-    ----
+    -----
       loglevel (int): minimum loglevel for emitting messages
     """
     logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
     logging.basicConfig(
         level=loglevel, stream=sys.stdout, format=logformat, datefmt="%Y-%m-%d %H:%M:%S"
     )
 
 
 def main(args: list[str]):
     """Deals with command line parameters and input/output.
 
     Args:
-    ----
+    -----
       args (List[str]): command line parameters as list of strings
           (for example  ``["--verbose", "42"]``).
     """
     args_parsed = parse_args(args)
     setup_logging(args_parsed.loglevel)
 
     _logger.info(f"Starting csvsheet calculation: {args_parsed}")
@@ -196,15 +196,15 @@
     # create delimiter and quotechar
     delimiter = args_parsed.delimiter
     quotechar = args_parsed.quotechar
 
     # open reader
     csvreader = csv.reader(args_parsed.input, delimiter=delimiter, quotechar=quotechar)
     # open writer
-    fh = sys.stdout if args_parsed.output == "-" else open(args_parsed.output, "w")
+    fh = args_parsed.output
     csvwriter = csv.writer(fh, delimiter=delimiter, quotechar=quotechar)
     # loop
     for row_idx, row in enumerate(csvreader):
         # loop
         for (
             col_idx,
             cell,
@@ -226,15 +226,15 @@
             # update row
             row[col_idx] = cell
         # write row
         csvwriter.writerow(row)
     # close reader
     args_parsed.input.close()
     # close writer
-    if args_parsed.output != "-":
+    if args_parsed.output != sys.stdout:
         fh.close()
 
     _logger.info("Script ends here")
 
 
 def run():
     """Calls :func:`main` passing the CLI arguments extracted from :obj:`sys.argv`.
```

### Comparing `csvsheet-0.1/src/csvsheet/csvsheet.py,cover` & `csvsheet-0.1.2/src/csvsheet/csvsheet.py,cover`

 * *Files identical despite different names*

### Comparing `csvsheet-0.1/src/csvsheet.egg-info/PKG-INFO` & `csvsheet-0.1.2/src/csvsheet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvsheet
-Version: 0.1
+Version: 0.1.2
 Summary: Simple formula support for CSV
 Home-page: https://github.com/jtplaarj/csvsheet/
 Author: Jesús Lázaro
 Author-email: jesus.lazaro@ehu.eus
 License: MIT
 Project-URL: Documentation, https://csvsheet.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/jtplaarj/csvsheet/
@@ -19,20 +19,14 @@
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/csvsheet.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/csvsheet
-    .. image:: https://readthedocs.org/projects/csvsheet/badge/?version=latest
-        :alt: ReadTheDocs
-        :target: https://csvsheet.readthedocs.io/en/stable/
-    .. image:: https://img.shields.io/coveralls/github/<USER>/csvsheet/main.svg
-        :alt: Coveralls
-        :target: https://coveralls.io/r/<USER>/csvsheet
     .. image:: https://img.shields.io/conda/vn/conda-forge/csvsheet.svg
         :alt: Conda-Forge
         :target: https://anaconda.org/conda-forge/csvsheet
     .. image:: https://pepy.tech/badge/csvsheet/month
         :alt: Monthly Downloads
         :target: https://pepy.tech/project/csvsheet
     .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
@@ -40,19 +34,24 @@
         :target: https://twitter.com/csvsheet
 .. image:: https://readthedocs.org/projects/csvsheet/badge/?version=latest
     :alt: ReadTheDocs
     :target: https://csvsheet.readthedocs.io/en/stable/
 .. image:: https://img.shields.io/pypi/v/csvsheet.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/csvsheet/
+.. image:: https://img.shields.io/coveralls/github/jtplaarj/csvsheet/main.svg
+    :alt: Coveralls
+    :target: https://coveralls.io/r/jtplaarj/csvsheet
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
+.. image:: https://img.shields.io/coveralls/github/jtplaarj/csvsheet/main.svg
+    :alt: Coveralls
+    :target: https://coveralls.io/r/jtplaarj/csvsheet
 
-|
 
 ========
 csvsheet
 ========
 
 
     Simple formula support for CSV
@@ -69,21 +68,24 @@
 ==================
 
 The command line requires a single compulsory arugment, the CSV fileto process::
 
     csvsheet <file.csv> -o <output.csv> -d <delimiter> -q <quotechar> -m <equation_delimiter> -v -vv
     csvsheet --help
 
+The input file is required, if '-' is used, stdin is used.
 The output file is optional, if not provided, the output will be printed to stdout.
 The delimiter is also optional, if not provided, the default delimiter is `,`.
 The quotechar is also optional, if not provided, the default quotechar is `"`.
 The equation delimiter is also optional, if not provided, the default equation delimiter is `=`.
 
 The `-v` and `-vv` flags are optional, they are used to increase the verbosity of the output.
 
+Read the `extended docs`_ for extra information.
+
 Example
 =======
 
 The following example shows how to use the command line::
 
     csvsheet example.csv
 
@@ -130,7 +132,9 @@
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
+
+.. _extended docs: https://csvsheet.readthedocs.io/en/stable/
```

### Comparing `csvsheet-0.1/src/csvsheet.egg-info/SOURCES.txt` & `csvsheet-0.1.2/src/csvsheet.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,11 @@
 src/csvsheet.egg-info/dependency_links.txt
 src/csvsheet.egg-info/entry_points.txt
 src/csvsheet.egg-info/not-zip-safe
 src/csvsheet.egg-info/requires.txt
 src/csvsheet.egg-info/top_level.txt
 tests/conftest.py
 tests/test_a.csv
-tests/test_a.csv.out
 tests/test_a.ssv
 tests/test_b.csv
 tests/test_c.csv
 tests/test_csvsheet.py
```

### Comparing `csvsheet-0.1/tox.ini` & `csvsheet-0.1.2/tox.ini`

 * *Files identical despite different names*

