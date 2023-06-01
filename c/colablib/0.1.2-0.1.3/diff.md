# Comparing `tmp/colablib-0.1.2.tar.gz` & `tmp/colablib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.2.tar", last modified: Thu Jun  1 09:48:07 2023, max compression
+gzip compressed data, was "colablib-0.1.3.tar", last modified: Thu Jun  1 10:16:53 2023, max compression
```

## Comparing `colablib-0.1.2.tar` & `colablib-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:07.168077 colablib-0.1.2/
--rw-rw-rw-   0        0        0      213 2023-06-01 09:48:07.168077 colablib-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:07.152372 colablib-0.1.2/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.2/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.2/colablib/cprint.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.2/colablib/git_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:07.166886 colablib-0.1.2/colablib.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-01 09:48:06.000000 colablib-0.1.2/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-01 09:48:07.000000 colablib-0.1.2/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:48:06.000000 colablib-0.1.2/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 09:48:06.000000 colablib-0.1.2/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:48:07.168077 colablib-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-06-01 09:47:22.000000 colablib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:16:53.843595 colablib-0.1.3/
+-rw-rw-rw-   0        0        0      213 2023-06-01 10:16:53.842596 colablib-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 10:16:53.834077 colablib-0.1.3/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.3/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.3/colablib/cprint.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.3/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     1580 2023-06-01 10:15:05.000000 colablib-0.1.3/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:16:53.841597 colablib-0.1.3/colablib.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 10:16:53.000000 colablib-0.1.3/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 10:16:53.843595 colablib-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-06-01 10:15:43.000000 colablib-0.1.3/setup.py
```

### Comparing `colablib-0.1.2/colablib/cprint.py` & `colablib-0.1.3/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.2/colablib/git_utils.py` & `colablib-0.1.3/colablib/git_utils.py`

 * *Files identical despite different names*

