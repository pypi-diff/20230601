# Comparing `tmp/SNPfilter-0.0.3.tar.gz` & `tmp/SNPfilter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPfilter-0.0.3.tar", last modified: Thu May 11 05:55:54 2023, max compression
+gzip compressed data, was "SNPfilter-0.0.4.tar", last modified: Thu Jun  1 08:32:31 2023, max compression
```

## Comparing `SNPfilter-0.0.3.tar` & `SNPfilter-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2023-05-02 03:30:38.000000 SNPfilter-0.0.3/LICENSE
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       19 2023-05-02 03:45:18.000000 SNPfilter-0.0.3/MANIFEST.in
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3965 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3633 2023-05-07 03:58:28.000000 SNPfilter-0.0.3/README.md
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/SNPfilter.egg-info/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     3965 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      354 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/SNPfilter.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       49 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/entry_points.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       31 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/requires.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2023-05-11 05:55:53.000000 SNPfilter-0.0.3/SNPfilter.egg-info/top_level.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/setup.cfg
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      756 2023-05-07 02:49:23.000000 SNPfilter-0.0.3/setup.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/snpfilter/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-02 03:35:02.000000 SNPfilter-0.0.3/snpfilter/__init__.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    12776 2023-05-11 05:51:01.000000 SNPfilter-0.0.3/snpfilter/cli.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-11 05:55:54.000000 SNPfilter-0.0.3/snpfilter/scripts/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-07 03:02:58.000000 SNPfilter-0.0.3/snpfilter/scripts/__init__.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      605 2023-05-07 03:04:06.000000 SNPfilter-0.0.3/snpfilter/scripts/map.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      502 2023-05-11 05:51:59.000000 SNPfilter-0.0.3/snpfilter/versions.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2023-05-02 03:30:38.000000 SNPfilter-0.0.4/LICENSE
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       19 2023-05-02 03:45:18.000000 SNPfilter-0.0.4/MANIFEST.in
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     4963 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     4631 2023-05-30 02:03:07.000000 SNPfilter-0.0.4/README.md
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/SNPfilter.egg-info/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     4963 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/SNPfilter.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      354 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/SNPfilter.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/SNPfilter.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       49 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/SNPfilter.egg-info/entry_points.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       31 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/SNPfilter.egg-info/requires.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/SNPfilter.egg-info/top_level.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/setup.cfg
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      756 2023-05-07 02:49:23.000000 SNPfilter-0.0.4/setup.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/snpfilter/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-02 03:35:02.000000 SNPfilter-0.0.4/snpfilter/__init__.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    12776 2023-05-11 05:51:01.000000 SNPfilter-0.0.4/snpfilter/cli.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-06-01 08:32:31.000000 SNPfilter-0.0.4/snpfilter/scripts/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-05-07 03:02:58.000000 SNPfilter-0.0.4/snpfilter/scripts/__init__.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      605 2023-05-07 03:04:06.000000 SNPfilter-0.0.4/snpfilter/scripts/map.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      610 2023-05-30 02:03:56.000000 SNPfilter-0.0.4/snpfilter/versions.py
```

### Comparing `SNPfilter-0.0.3/LICENSE` & `SNPfilter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPfilter-0.0.3/setup.py` & `SNPfilter-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `SNPfilter-0.0.3/snpfilter/cli.py` & `SNPfilter-0.0.4/snpfilter/cli.py`

 * *Files identical despite different names*

### Comparing `SNPfilter-0.0.3/snpfilter/scripts/map.py` & `SNPfilter-0.0.4/snpfilter/scripts/map.py`

 * *Files identical despite different names*

