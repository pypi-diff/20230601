# Comparing `tmp/repository-cli-0.7.0.tar.gz` & `tmp/repository-cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repository-cli-0.7.0.tar", last modified: Tue May 30 08:35:56 2023, max compression
+gzip compressed data, was "repository-cli-0.8.0.tar", last modified: Thu Jun  1 10:48:17 2023, max compression
```

## Comparing `repository-cli-0.7.0.tar` & `repository-cli-0.8.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.653745 repository-cli-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.653745 repository-cli-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-30 08:35:49.000000 repository-cli-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-30 08:35:49.000000 repository-cli-0.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-30 08:35:49.000000 repository-cli-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 08:35:49.000000 repository-cli-0.7.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-30 08:35:49.000000 repository-cli-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 08:35:49.000000 repository-cli-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-30 08:35:56.657745 repository-cli-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-30 08:35:49.000000 repository-cli-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/repository_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/click_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/click_param_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/repository_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 08:35:49.000000 repository-cli-0.7.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-05-30 08:35:49.000000 repository-cli-0.7.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-30 08:35:56.657745 repository-cli-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 08:35:49.000000 repository-cli-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_rdmrecords.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_rdmrecords_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_rdmrecords_pids.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_repository_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.625273 repository-cli-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.625273 repository-cli-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 10:48:11.000000 repository-cli-0.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-01 10:48:11.000000 repository-cli-0.8.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-01 10:48:11.000000 repository-cli-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 10:48:11.000000 repository-cli-0.8.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 10:48:11.000000 repository-cli-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 10:48:11.000000 repository-cli-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-01 10:48:17.629273 repository-cli-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-01 10:48:11.000000 repository-cli-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.625273 repository-cli-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/repository_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/click_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/click_param_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20795 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/repository_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 10:48:11.000000 repository-cli-0.8.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-06-01 10:48:11.000000 repository-cli-0.8.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-01 10:48:17.629273 repository-cli-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 10:48:11.000000 repository-cli-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_rdmrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_rdmrecords_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_rdmrecords_pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_repository_cli.py
```

### Comparing `repository-cli-0.7.0/.github/workflows/tests.yml` & `repository-cli-0.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/CHANGES.rst` & `repository-cli-0.8.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-06-01)
+
+- records: make arguments ready for drafts too
+- records: add argument delete-file
+
+
 Version v0.7.0 (release 2023-05-30)
 
 - test: fix and pin due flask-babelex
 - records: separate replace-file from add-file
 - fix: black color on black background, bad
 - types: otherwise it is not working with 3.9
 - global: migrate to ruff
```

### Comparing `repository-cli-0.7.0/CONTRIBUTING.rst` & `repository-cli-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/LICENSE` & `repository-cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/MANIFEST.in` & `repository-cli-0.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/PKG-INFO` & `repository-cli-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.7.0
+Version: 0.8.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-06-01)
+
+- records: make arguments ready for drafts too
+- records: add argument delete-file
+
+
 Version v0.7.0 (release 2023-05-30)
 
 - test: fix and pin due flask-babelex
 - records: separate replace-file from add-file
 - fix: black color on black background, bad
 - types: otherwise it is not working with 3.9
 - global: migrate to ruff
```

### Comparing `repository-cli-0.7.0/README.rst` & `repository-cli-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/docs/Makefile` & `repository-cli-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/docs/api.rst` & `repository-cli-0.8.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/docs/conf.py` & `repository-cli-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/docs/index.rst` & `repository-cli-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/docs/make.bat` & `repository-cli-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli/cli.py` & `repository-cli-0.8.0/repository_cli/cli.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli/click_options.py` & `repository-cli-0.8.0/repository_cli/click_options.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli/click_param_types.py` & `repository-cli-0.8.0/repository_cli/click_param_types.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli/ext.py` & `repository-cli-0.8.0/repository_cli/ext.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli/records.py` & `repository-cli-0.8.0/repository_cli/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,14 +467,55 @@
     except Exception as error:
         secho(f"'{pid}', problem during update, {error}", fg=Color.error)
         return
 
     secho(f"Identifier for '{pid}' replaced.", fg=Color.success)
 
 
+@group_records.command("delete-file")
+@option_data_model
+@option_pid
+@option("--filename", type=STRING, required=True)
+@with_appcontext
+def delete_file(data_model: str, pid: str, filename: str) -> None:
+    """Delete the file."""
+    identity = get_identity("system_process", role_name="admin")
+    service = get_records_service(data_model=data_model)
+
+    try:
+        record = service.read(identity=identity, id_=pid)._record
+    except PIDDoesNotExistError:
+        try:
+            record = service.read_draft(identity=identity, id_=pid)._record
+        except PIDDoesNotExistError as error:
+            msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
+            secho(msg, fg=Color.error)
+            return
+
+    files = record.files
+    obj = None
+
+    try:
+        obj = files[filename]
+    except KeyError:
+        secho(
+            f"File with filename: {filename} not found. Check filename or PID",
+            fg=Color.error,
+        )
+        return
+
+    files.unlock()
+    files.delete(obj.key)
+    files.lock()
+
+    record.commit()
+    db.session.commit()
+    secho("File deleted successfully", fg=Color.success)
+
+
 @group_records.command("replace-file")
 @option_data_model
 @option_pid
 @option_input_file(type_=File("rb"))
 @option("--override-name-match-check", is_flag=True, default=False)
 @with_appcontext
 def replace_file(
@@ -484,19 +525,22 @@
     override_name_match_check: bool,  # noqa: FBT001
 ) -> None:
     """Replace the file."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     try:
-        record = service.read(identity=identity, id_=pid)._record  # noqa: SLF001
-    except PIDDoesNotExistError as error:
-        msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
-        secho(msg, fg=Color.error)
-        return
+        record = service.read(identity=identity, id_=pid)._record
+    except PIDDoesNotExistError:
+        try:
+            record = service.read_draft(identity=identity, id_=pid)._record
+        except PIDDoesNotExistError as error:
+            msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
+            secho(msg, fg=Color.error)
+            return
 
     files = record.files
     filename = Path(input_file.name).name  # Path().name gets the filename only
     obj = None
 
     try:
         obj = files[filename]
@@ -539,19 +583,22 @@
     enable_files: bool,  # noqa: FBT001
 ) -> None:
     """Add a new file to a published record."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     try:
-        record = service.read(identity=identity, id_=pid)._record  # noqa: SLF001
-    except PIDDoesNotExistError as error:
-        msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
-        secho(msg, fg=Color.error)
-        return
+        record = service.read(identity=identity, id_=pid)._record
+    except PIDDoesNotExistError:
+        try:
+            record = service.read_draft(identity=identity, id_=pid)._record
+        except PIDDoesNotExistError as error:
+            msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
+            secho(msg, fg=Color.error)
+            return
 
     files = record.files
     filename = Path(input_file.name).name
 
     if files.enabled:
         obj = files.get(filename, None)
         if obj is not None:
```

### Comparing `repository-cli-0.7.0/repository_cli/types.py` & `repository-cli-0.8.0/repository_cli/types.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli/users.py` & `repository-cli-0.8.0/repository_cli/users.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli/utils.py` & `repository-cli-0.8.0/repository_cli/utils.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/repository_cli.egg-info/PKG-INFO` & `repository-cli-0.8.0/repository_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.7.0
+Version: 0.8.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-06-01)
+
+- records: make arguments ready for drafts too
+- records: add argument delete-file
+
+
 Version v0.7.0 (release 2023-05-30)
 
 - test: fix and pin due flask-babelex
 - records: separate replace-file from add-file
 - fix: black color on black background, bad
 - types: otherwise it is not working with 3.9
 - global: migrate to ruff
```

### Comparing `repository-cli-0.7.0/repository_cli.egg-info/SOURCES.txt` & `repository-cli-0.8.0/repository_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/run-tests.sh` & `repository-cli-0.8.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/setup.cfg` & `repository-cli-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/tests/conftest.py` & `repository-cli-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/tests/test_rdmrecords.py` & `repository-cli-0.8.0/tests/test_rdmrecords.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/tests/test_rdmrecords_identifiers.py` & `repository-cli-0.8.0/tests/test_rdmrecords_identifiers.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/tests/test_rdmrecords_pids.py` & `repository-cli-0.8.0/tests/test_rdmrecords_pids.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.7.0/tests/test_repository_cli.py` & `repository-cli-0.8.0/tests/test_repository_cli.py`

 * *Files identical despite different names*

