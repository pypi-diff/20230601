# Comparing `tmp/colablib-0.1.4.dev1.tar.gz` & `tmp/colablib-0.1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.4.dev1.tar", last modified: Thu Jun  1 11:13:02 2023, max compression
+gzip compressed data, was "colablib-0.1.5.dev1.tar", last modified: Thu Jun  1 11:14:19 2023, max compression
```

## Comparing `colablib-0.1.4.dev1.tar` & `colablib-0.1.5.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 11:13:02.109045 colablib-0.1.4.dev1/
--rw-rw-rw-   0        0        0      218 2023-06-01 11:13:02.109045 colablib-0.1.4.dev1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.4.dev1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 11:13:02.096471 colablib-0.1.4.dev1/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.4.dev1/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.4.dev1/colablib/cprint.py
--rw-rw-rw-   0        0        0     1181 2023-06-01 11:12:05.000000 colablib-0.1.4.dev1/colablib/deb_utils.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.4.dev1/colablib/git_utils.py
--rw-rw-rw-   0        0        0     2594 2023-06-01 10:44:06.000000 colablib-0.1.4.dev1/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:13:02.108071 colablib-0.1.4.dev1/colablib.egg-info/
--rw-rw-rw-   0        0        0      218 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 11:13:02.109045 colablib-0.1.4.dev1/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-06-01 11:12:27.000000 colablib-0.1.4.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:14:19.015235 colablib-0.1.5.dev1/
+-rw-rw-rw-   0        0        0      218 2023-06-01 11:14:19.014366 colablib-0.1.5.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 11:14:19.001542 colablib-0.1.5.dev1/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev1/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev1/colablib/cprint.py
+-rw-rw-rw-   0        0        0     1181 2023-06-01 11:12:05.000000 colablib-0.1.5.dev1/colablib/deb_utils.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev1/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     2594 2023-06-01 10:44:06.000000 colablib-0.1.5.dev1/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:14:19.012722 colablib-0.1.5.dev1/colablib.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-06-01 11:14:18.000000 colablib-0.1.5.dev1/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-01 11:14:18.000000 colablib-0.1.5.dev1/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:14:18.000000 colablib-0.1.5.dev1/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 11:14:18.000000 colablib-0.1.5.dev1/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 11:14:19.015235 colablib-0.1.5.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-06-01 11:13:54.000000 colablib-0.1.5.dev1/setup.py
```

### Comparing `colablib-0.1.4.dev1/colablib/cprint.py` & `colablib-0.1.5.dev1/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.4.dev1/colablib/deb_utils.py` & `colablib-0.1.5.dev1/colablib/deb_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.4.dev1/colablib/git_utils.py` & `colablib-0.1.5.dev1/colablib/git_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.4.dev1/colablib/py_utils.py` & `colablib-0.1.5.dev1/colablib/py_utils.py`

 * *Files identical despite different names*

