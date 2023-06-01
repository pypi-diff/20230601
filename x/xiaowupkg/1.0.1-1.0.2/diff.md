# Comparing `tmp/xiaowupkg-1.0.1.tar.gz` & `tmp/xiaowupkg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaowupkg-1.0.1.tar", last modified: Thu Jun  1 07:50:01 2023, max compression
+gzip compressed data, was "xiaowupkg-1.0.2.tar", last modified: Thu Jun  1 08:49:58 2023, max compression
```

## Comparing `xiaowupkg-1.0.1.tar` & `xiaowupkg-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:50:00.917079 xiaowupkg-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 07:50:00.913079 xiaowupkg-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 07:50:00.921079 xiaowupkg-1.0.1/setup.cfg
--rwxrw-rw-   0 root         (0) root         (0)      344 2023-06-01 07:49:07.000000 xiaowupkg-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:50:00.833077 xiaowupkg-1.0.1/tools/
--rwxrw-rw-   0 root         (0) root         (0)      151 2023-06-01 07:49:50.000000 xiaowupkg-1.0.1/tools/__init__.py
--rwxrw-rw-   0 root         (0) root         (0)      697 2023-06-01 06:46:27.000000 xiaowupkg-1.0.1/tools/filefunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:50:00.897079 xiaowupkg-1.0.1/xiaowupkg.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      152 2023-06-01 07:50:00.000000 xiaowupkg-1.0.1/xiaowupkg.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      208 2023-06-01 07:50:00.000000 xiaowupkg-1.0.1/xiaowupkg.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-06-01 07:50:00.000000 xiaowupkg-1.0.1/xiaowupkg.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       30 2023-06-01 07:50:00.000000 xiaowupkg-1.0.1/xiaowupkg.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        6 2023-06-01 07:50:00.000000 xiaowupkg-1.0.1/xiaowupkg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:49:58.484458 xiaowupkg-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 08:49:58.472458 xiaowupkg-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 08:49:58.484458 xiaowupkg-1.0.2/setup.cfg
+-rwxrw-rw-   0 root         (0) root         (0)      342 2023-06-01 08:49:13.000000 xiaowupkg-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:49:58.384457 xiaowupkg-1.0.2/xiaowupkg/
+-rwxrw-rw-   0 root         (0) root         (0)      151 2023-06-01 08:45:25.000000 xiaowupkg-1.0.2/xiaowupkg/__init__.py
+-rwxrw-rw-   0 root         (0) root         (0)      697 2023-06-01 06:46:27.000000 xiaowupkg-1.0.2/xiaowupkg/filefunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 08:49:58.456457 xiaowupkg-1.0.2/xiaowupkg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 08:49:57.000000 xiaowupkg-1.0.2/xiaowupkg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-01 08:49:58.000000 xiaowupkg-1.0.2/xiaowupkg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 08:49:58.000000 xiaowupkg-1.0.2/xiaowupkg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-01 08:49:58.000000 xiaowupkg-1.0.2/xiaowupkg.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-01 08:49:58.000000 xiaowupkg-1.0.2/xiaowupkg.egg-info/top_level.txt
```

### Comparing `xiaowupkg-1.0.1/tools/filefunc.py` & `xiaowupkg-1.0.2/xiaowupkg/filefunc.py`

 * *Files identical despite different names*

