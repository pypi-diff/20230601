# Comparing `tmp/colablib-0.1.5.dev3.tar.gz` & `tmp/colablib-0.1.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.5.dev3.tar", last modified: Thu Jun  1 13:52:00 2023, max compression
+gzip compressed data, was "colablib-0.1.5.dev4.tar", last modified: Thu Jun  1 14:06:00 2023, max compression
```

## Comparing `colablib-0.1.5.dev3.tar` & `colablib-0.1.5.dev4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:52:00.142321 colablib-0.1.5.dev3/
--rw-rw-rw-   0        0        0      218 2023-06-01 13:52:00.141308 colablib-0.1.5.dev3/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 13:52:00.129443 colablib-0.1.5.dev3/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev3/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev3/colablib/cprint.py
--rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev3/colablib/deb_utils.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev3/colablib/git_utils.py
--rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev3/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:52:00.140306 colablib-0.1.5.dev3/colablib.egg-info/
--rw-rw-rw-   0        0        0      218 2023-06-01 13:51:59.000000 colablib-0.1.5.dev3/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-01 13:52:00.000000 colablib-0.1.5.dev3/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:51:59.000000 colablib-0.1.5.dev3/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 13:51:59.000000 colablib-0.1.5.dev3/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 13:52:00.142321 colablib-0.1.5.dev3/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-06-01 13:50:59.000000 colablib-0.1.5.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:06:00.619721 colablib-0.1.5.dev4/
+-rw-rw-rw-   0        0        0      218 2023-06-01 14:06:00.618667 colablib-0.1.5.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 14:06:00.604750 colablib-0.1.5.dev4/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev4/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev4/colablib/cprint.py
+-rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev4/colablib/deb_utils.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev4/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     9467 2023-06-01 12:35:18.000000 colablib-0.1.5.dev4/colablib/model_validators.py
+-rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev4/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:06:00.617355 colablib-0.1.5.dev4/colablib.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 14:06:00.000000 colablib-0.1.5.dev4/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 14:06:00.619721 colablib-0.1.5.dev4/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-06-01 14:05:44.000000 colablib-0.1.5.dev4/setup.py
```

### Comparing `colablib-0.1.5.dev3/colablib/cprint.py` & `colablib-0.1.5.dev4/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev3/colablib/deb_utils.py` & `colablib-0.1.5.dev4/colablib/deb_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev3/colablib/git_utils.py` & `colablib-0.1.5.dev4/colablib/git_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev3/colablib/py_utils.py` & `colablib-0.1.5.dev4/colablib/py_utils.py`

 * *Files identical despite different names*

