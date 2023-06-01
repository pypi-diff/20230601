# Comparing `tmp/goerrpy-1.0.0.tar.gz` & `tmp/goerrpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goerrpy-1.0.0.tar", last modified: Thu Jun  1 21:13:45 2023, max compression
+gzip compressed data, was "goerrpy-1.0.1.tar", last modified: Thu Jun  1 21:22:36 2023, max compression
```

## Comparing `goerrpy-1.0.0.tar` & `goerrpy-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:13:45.981915 goerrpy-1.0.0/
--rw-r--r--   0 mbozhilov   (505) staff       (20)      433 2023-06-01 21:13:45.981783 goerrpy-1.0.0/PKG-INFO
--rw-r--r--   0 mbozhilov   (505) staff       (20)       67 2023-06-01 21:07:37.000000 goerrpy-1.0.0/README.md
--rw-r--r--   0 mbozhilov   (505) staff       (20)      457 2023-06-01 09:14:30.000000 goerrpy-1.0.0/decorators.py
-drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:13:45.981579 goerrpy-1.0.0/goerrpy.egg-info/
--rw-r--r--   0 mbozhilov   (505) staff       (20)      433 2023-06-01 21:13:45.000000 goerrpy-1.0.0/goerrpy.egg-info/PKG-INFO
--rw-r--r--   0 mbozhilov   (505) staff       (20)      156 2023-06-01 21:13:45.000000 goerrpy-1.0.0/goerrpy.egg-info/SOURCES.txt
--rw-r--r--   0 mbozhilov   (505) staff       (20)        1 2023-06-01 21:13:45.000000 goerrpy-1.0.0/goerrpy.egg-info/dependency_links.txt
--rw-r--r--   0 mbozhilov   (505) staff       (20)       11 2023-06-01 21:13:45.000000 goerrpy-1.0.0/goerrpy.egg-info/top_level.txt
--rw-r--r--   0 mbozhilov   (505) staff       (20)       38 2023-06-01 21:13:45.981963 goerrpy-1.0.0/setup.cfg
--rw-r--r--   0 mbozhilov   (505) staff       (20)      496 2023-06-01 21:13:43.000000 goerrpy-1.0.0/setup.py
+drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:22:36.090809 goerrpy-1.0.1/
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      433 2023-06-01 21:22:36.090674 goerrpy-1.0.1/PKG-INFO
+-rw-r--r--   0 mbozhilov   (505) staff       (20)       67 2023-06-01 21:07:37.000000 goerrpy-1.0.1/README.md
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      457 2023-06-01 09:14:30.000000 goerrpy-1.0.1/decorators.py
+drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:22:36.090465 goerrpy-1.0.1/goerrpy.egg-info/
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      433 2023-06-01 21:22:36.000000 goerrpy-1.0.1/goerrpy.egg-info/PKG-INFO
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      156 2023-06-01 21:22:36.000000 goerrpy-1.0.1/goerrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mbozhilov   (505) staff       (20)        1 2023-06-01 21:22:36.000000 goerrpy-1.0.1/goerrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mbozhilov   (505) staff       (20)       11 2023-06-01 21:22:36.000000 goerrpy-1.0.1/goerrpy.egg-info/top_level.txt
+-rw-r--r--   0 mbozhilov   (505) staff       (20)       38 2023-06-01 21:22:36.090858 goerrpy-1.0.1/setup.cfg
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      496 2023-06-01 21:21:45.000000 goerrpy-1.0.1/setup.py
```

