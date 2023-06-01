# Comparing `tmp/colablib-0.1.5.dev5.tar.gz` & `tmp/colablib-0.1.5.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.5.dev5.tar", last modified: Thu Jun  1 14:18:06 2023, max compression
+gzip compressed data, was "colablib-0.1.5.dev6.tar", last modified: Thu Jun  1 16:36:06 2023, max compression
```

## Comparing `colablib-0.1.5.dev5.tar` & `colablib-0.1.5.dev6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:18:06.973576 colablib-0.1.5.dev5/
--rw-rw-rw-   0        0        0      218 2023-06-01 14:18:06.973576 colablib-0.1.5.dev5/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 14:18:06.956185 colablib-0.1.5.dev5/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev5/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev5/colablib/cprint.py
--rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev5/colablib/deb_utils.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev5/colablib/git_utils.py
--rw-rw-rw-   0        0        0     8696 2023-06-01 14:17:34.000000 colablib-0.1.5.dev5/colablib/model_validators.py
--rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev5/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:18:06.971576 colablib-0.1.5.dev5/colablib.egg-info/
--rw-rw-rw-   0        0        0      218 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 14:18:06.000000 colablib-0.1.5.dev5/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 14:18:06.974575 colablib-0.1.5.dev5/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-06-01 14:16:52.000000 colablib-0.1.5.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:36:06.878610 colablib-0.1.5.dev6/
+-rw-rw-rw-   0        0        0      218 2023-06-01 16:36:06.877610 colablib-0.1.5.dev6/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 16:36:06.854871 colablib-0.1.5.dev6/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev6/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev6/colablib/cprint.py
+-rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev6/colablib/deb_utils.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev6/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     3799 2023-06-01 16:34:44.000000 colablib-0.1.5.dev6/colablib/model_downloader.py
+-rw-rw-rw-   0        0        0     8696 2023-06-01 14:17:34.000000 colablib-0.1.5.dev6/colablib/model_validators.py
+-rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev6/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:36:06.877610 colablib-0.1.5.dev6/colablib.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 16:36:06.879613 colablib-0.1.5.dev6/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-06-01 16:35:05.000000 colablib-0.1.5.dev6/setup.py
```

### Comparing `colablib-0.1.5.dev5/colablib/cprint.py` & `colablib-0.1.5.dev6/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev5/colablib/deb_utils.py` & `colablib-0.1.5.dev6/colablib/deb_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev5/colablib/git_utils.py` & `colablib-0.1.5.dev6/colablib/git_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev5/colablib/model_validators.py` & `colablib-0.1.5.dev6/colablib/model_validators.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev5/colablib/py_utils.py` & `colablib-0.1.5.dev6/colablib/py_utils.py`

 * *Files identical despite different names*

