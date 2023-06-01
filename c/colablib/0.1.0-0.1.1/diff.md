# Comparing `tmp/colablib-0.1.0.tar.gz` & `tmp/colablib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.0.tar", last modified: Thu Jun  1 09:07:44 2023, max compression
+gzip compressed data, was "colablib-0.1.1.tar", last modified: Thu Jun  1 09:28:25 2023, max compression
```

## Comparing `colablib-0.1.0.tar` & `colablib-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:07:44.504113 colablib-0.1.0/
--rw-rw-rw-   0        0        0      213 2023-06-01 09:07:44.503163 colablib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:07:44.496438 colablib-0.1.0/colablib.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-01 09:07:44.000000 colablib-0.1.0/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-01 09:07:44.000000 colablib-0.1.0/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:07:44.000000 colablib-0.1.0/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-01 09:07:44.000000 colablib-0.1.0/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:07:44.505195 colablib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-06-01 09:06:52.000000 colablib-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:07:44.501094 colablib-0.1.0/utils/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.0/utils/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 08:39:35.000000 colablib-0.1.0/utils/cprint.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:28:25.599040 colablib-0.1.1/
+-rw-rw-rw-   0        0        0      213 2023-06-01 09:28:25.598039 colablib-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 09:28:25.587536 colablib-0.1.1/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.1/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.1/colablib/color_print.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:28:25.597039 colablib-0.1.1/colablib.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-01 09:28:25.000000 colablib-0.1.1/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-06-01 09:28:25.000000 colablib-0.1.1/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:28:25.000000 colablib-0.1.1/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 09:28:25.000000 colablib-0.1.1/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:28:25.599040 colablib-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-06-01 09:27:02.000000 colablib-0.1.1/setup.py
```

### Comparing `colablib-0.1.0/utils/cprint.py` & `colablib-0.1.1/colablib/color_print.py`

 * *Files identical despite different names*

