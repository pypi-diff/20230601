# Comparing `tmp/ewoksutils-0.1.1.tar.gz` & `tmp/ewoksutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksutils-0.1.1.tar", last modified: Tue Mar 21 17:26:36 2023, max compression
+gzip compressed data, was "dist/ewoksutils-0.1.2.tar", last modified: Thu Jun  1 13:13:46 2023, max compression
```

## Comparing `ewoksutils-0.1.1.tar` & `ewoksutils-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      992 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-21 17:25:16.000000 ewoksutils-0.1.1/src/ewoksutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/datetime_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/event_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/import_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils/logging_utils/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/logging_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/logging_utils/asyncwrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/logging_utils/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/logging_utils/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/logging_utils/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/path_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3785 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/sqlite3_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-21 17:26:30.000000 ewoksutils-0.1.1/src/ewoksutils/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/tests/test_datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     4406 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/tests/test_logging_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-03-21 17:18:09.000000 ewoksutils-0.1.1/src/ewoksutils/tests/test_sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      992 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      785 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      115 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-21 17:26:36.000000 ewoksutils-0.1.1/src/ewoksutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      992 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-01 13:12:23.000000 ewoksutils-0.1.2/src/ewoksutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/datetime_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/event_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2023-06-01 13:09:59.000000 ewoksutils-0.1.2/src/ewoksutils/import_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils/logging_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/logging_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/logging_utils/asyncwrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/logging_utils/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/logging_utils/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/logging_utils/sqlite3.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/path_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3785 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/sqlite3_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 13:13:40.000000 ewoksutils-0.1.2/src/ewoksutils/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/tests/test_datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/tests/test_import_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4406 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/tests/test_logging_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-06-01 12:45:39.000000 ewoksutils-0.1.2/src/ewoksutils/tests/test_sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      827 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-01 13:13:46.000000 ewoksutils-0.1.2/src/ewoksutils.egg-info/top_level.txt
```

### Comparing `ewoksutils-0.1.1/LICENSE.md` & `ewoksutils-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/PKG-INFO` & `ewoksutils-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksutils/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksutils/
 Project-URL: Documentation, https://ewoksutils.readthedocs.io/
```

### Comparing `ewoksutils-0.1.1/setup.cfg` & `ewoksutils-0.1.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -40,19 +40,14 @@
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
-[build_sphinx]
-project = ewoksutils
-version = attr: ewoksutils.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [mypy]
 python_version = 3.7
```

### Comparing `ewoksutils-0.1.1/src/ewoksutils/logging_utils/asyncwrapper.py` & `ewoksutils-0.1.2/src/ewoksutils/logging_utils/asyncwrapper.py`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/src/ewoksutils/logging_utils/cleanup.py` & `ewoksutils-0.1.2/src/ewoksutils/logging_utils/cleanup.py`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/src/ewoksutils/logging_utils/connection.py` & `ewoksutils-0.1.2/src/ewoksutils/logging_utils/connection.py`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/src/ewoksutils/logging_utils/sqlite3.py` & `ewoksutils-0.1.2/src/ewoksutils/logging_utils/sqlite3.py`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/src/ewoksutils/sqlite3_utils.py` & `ewoksutils-0.1.2/src/ewoksutils/sqlite3_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/src/ewoksutils/tests/test_logging_utils.py` & `ewoksutils-0.1.2/src/ewoksutils/tests/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/src/ewoksutils/tests/test_sqlite3.py` & `ewoksutils-0.1.2/src/ewoksutils/tests/test_sqlite3.py`

 * *Files identical despite different names*

### Comparing `ewoksutils-0.1.1/src/ewoksutils.egg-info/PKG-INFO` & `ewoksutils-0.1.2/src/ewoksutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksutils/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksutils/
 Project-URL: Documentation, https://ewoksutils.readthedocs.io/
```

### Comparing `ewoksutils-0.1.1/src/ewoksutils.egg-info/SOURCES.txt` & `ewoksutils-0.1.2/src/ewoksutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 src/ewoksutils/logging_utils/__init__.py
 src/ewoksutils/logging_utils/asyncwrapper.py
 src/ewoksutils/logging_utils/cleanup.py
 src/ewoksutils/logging_utils/connection.py
 src/ewoksutils/logging_utils/sqlite3.py
 src/ewoksutils/tests/__init__.py
 src/ewoksutils/tests/test_datetime.py
+src/ewoksutils/tests/test_import_utils.py
 src/ewoksutils/tests/test_logging_utils.py
 src/ewoksutils/tests/test_sqlite3.py
```

