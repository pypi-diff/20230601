# Comparing `tmp/swh.alter-0.0.0.tar.gz` & `tmp/swh.alter-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.alter-0.0.0.tar", last modified: Wed Mar  1 10:23:20 2023, max compression
+gzip compressed data, was "dist/swh.alter-0.0.1.tar", last modified: Thu Jun  1 09:40:06 2023, max compression
```

## Comparing `swh.alter-0.0.0.tar` & `swh.alter-0.0.1.tar`

### file list

```diff
@@ -1,47 +1,73 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-03-01 10:23:19.000000 swh.alter-0.0.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-01 10:23:19.000000 swh.alter-0.0.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      847 2023-03-01 10:23:19.000000 swh.alter-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-01 10:23:19.000000 swh.alter-0.0.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-01 10:23:19.000000 swh.alter-0.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:19.000000 swh.alter-0.0.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-01 10:23:19.000000 swh.alter-0.0.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-01 10:23:19.000000 swh.alter-0.0.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-01 10:23:19.000000 swh.alter-0.0.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1275 2023-03-01 10:23:20.000000 swh.alter-0.0.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-03-01 10:23:19.000000 swh.alter-0.0.0/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-01 10:23:19.000000 swh.alter-0.0.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-01 10:23:19.000000 swh.alter-0.0.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-03-01 10:23:19.000000 swh.alter-0.0.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:19.000000 swh.alter-0.0.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:19.000000 swh.alter-0.0.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-01 10:23:19.000000 swh.alter-0.0.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      235 2023-03-01 10:23:19.000000 swh.alter-0.0.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      267 2023-03-01 10:23:19.000000 swh.alter-0.0.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-01 10:23:19.000000 swh.alter-0.0.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-03-01 10:23:19.000000 swh.alter-0.0.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      136 2023-03-01 10:23:19.000000 swh.alter-0.0.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        7 2023-03-01 10:23:19.000000 swh.alter-0.0.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      226 2023-03-01 10:23:19.000000 swh.alter-0.0.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-01 10:23:20.000000 swh.alter-0.0.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2441 2023-03-01 10:23:19.000000 swh.alter-0.0.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-01 10:23:19.000000 swh.alter-0.0.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh/alter/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:19.000000 swh.alter-0.0.0/swh/alter/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      403 2023-03-01 10:23:19.000000 swh.alter-0.0.0/swh/alter/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-01 10:23:19.000000 swh.alter-0.0.0/swh/alter/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh/alter/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:19.000000 swh.alter-0.0.0/swh/alter/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)       85 2023-03-01 10:23:19.000000 swh.alter-0.0.0/swh/alter/tests/test_nothing.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh.alter.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1275 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh.alter.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      722 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh.alter.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh.alter.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh.alter.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       38 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh.alter.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-01 10:23:20.000000 swh.alter-0.0.0/swh.alter.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1508 2023-03-01 10:23:19.000000 swh.alter-0.0.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-06-01 09:40:03.000000 swh.alter-0.0.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-01 09:40:03.000000 swh.alter-0.0.1/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      847 2023-06-01 09:40:03.000000 swh.alter-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-01 09:40:03.000000 swh.alter-0.0.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-01 09:40:03.000000 swh.alter-0.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:03.000000 swh.alter-0.0.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-01 09:40:03.000000 swh.alter-0.0.1/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-01 09:40:03.000000 swh.alter-0.0.1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-01 09:40:03.000000 swh.alter-0.0.1/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2077 2023-06-01 09:40:06.000000 swh.alter-0.0.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1135 2023-06-01 09:40:03.000000 swh.alter-0.0.1/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-06-01 09:40:03.000000 swh.alter-0.0.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       63 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     1135 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/conf.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)        6 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      231 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2844 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/dataset.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4511 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-01.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4377 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-02.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4375 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-03.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4277 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-04.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4130 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-05.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4119 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-06.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4117 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-07.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4071 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-08.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4069 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-09.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4009 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-10.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4007 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-11.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     3987 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/inventory-12.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)     4100 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/images/mark.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     8767 2023-06-01 09:40:03.000000 swh.alter-0.0.1/docs/removal-algorithm.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-06-01 09:40:03.000000 swh.alter-0.0.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-01 09:40:03.000000 swh.alter-0.0.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-01 09:40:03.000000 swh.alter-0.0.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-06-01 09:40:03.000000 swh.alter-0.0.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       47 2023-06-01 09:40:03.000000 swh.alter-0.0.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       13 2023-06-01 09:40:03.000000 swh.alter-0.0.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-01 09:40:06.000000 swh.alter-0.0.1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2441 2023-06-01 09:40:03.000000 swh.alter-0.0.1/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh/alter/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4395 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13973 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/inventory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     8356 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/removable.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9579 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/subgraph.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh/alter/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4640 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    25153 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/tests/test_inventory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9818 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/tests/test_removable.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5875 2023-06-01 09:40:03.000000 swh.alter-0.0.1/swh/alter/tests/test_subgraph.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh.alter.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2077 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh.alter.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1383 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh.alter.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh.alter.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh.alter.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh.alter.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-01 09:40:06.000000 swh.alter-0.0.1/swh.alter.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1508 2023-06-01 09:40:03.000000 swh.alter-0.0.1/tox.ini
```

### Comparing `swh.alter-0.0.0/.pre-commit-config.yaml` & `swh.alter-0.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.alter-0.0.0/CODE_OF_CONDUCT.md` & `swh.alter-0.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.alter-0.0.0/LICENSE` & `swh.alter-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.alter-0.0.0/setup.py` & `swh.alter-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `swh.alter-0.0.0/tox.ini` & `swh.alter-0.0.1/tox.ini`

 * *Files identical despite different names*

