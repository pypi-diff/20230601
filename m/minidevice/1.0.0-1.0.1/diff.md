# Comparing `tmp/minidevice-1.0.0.tar.gz` & `tmp/minidevice-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.0.tar", last modified: Thu Jun  1 01:34:47 2023, max compression
+gzip compressed data, was "minidevice-1.0.1.tar", last modified: Thu Jun  1 01:41:03 2023, max compression
```

## Comparing `minidevice-1.0.0.tar` & `minidevice-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 01:34:47.329339 minidevice-1.0.0/
--rw-rw-rw-   0        0        0      263 2023-06-01 01:34:47.328342 minidevice-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-06-01 01:33:14.000000 minidevice-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 01:34:47.308394 minidevice-1.0.0/minidevice/
--rw-rw-rw-   0        0        0       29 2023-05-31 10:12:15.000000 minidevice-1.0.0/minidevice/__init__.py
--rw-rw-rw-   0        0        0     2040 2023-06-01 01:14:31.000000 minidevice-1.0.0/minidevice/adb.py
--rw-rw-rw-   0        0        0      269 2023-05-31 10:26:49.000000 minidevice-1.0.0/minidevice/config.py
--rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.0/minidevice/device.py
--rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.0/minidevice/minicap.py
--rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.0/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.0/minidevice/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:34:47.327345 minidevice-1.0.0/minidevice.egg-info/
--rw-rw-rw-   0        0        0      263 2023-06-01 01:34:46.000000 minidevice-1.0.0/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-06-01 01:34:47.000000 minidevice-1.0.0/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 01:34:46.000000 minidevice-1.0.0/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-01 01:34:47.000000 minidevice-1.0.0/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 01:34:47.000000 minidevice-1.0.0/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 01:34:47.329339 minidevice-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      451 2023-06-01 01:10:48.000000 minidevice-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:41:03.344519 minidevice-1.0.1/
+-rw-rw-rw-   0        0        0     1205 2023-06-01 01:41:03.343521 minidevice-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-06-01 01:33:14.000000 minidevice-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 01:41:03.333548 minidevice-1.0.1/minidevice/
+-rw-rw-rw-   0        0        0       29 2023-05-31 10:12:15.000000 minidevice-1.0.1/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     2040 2023-06-01 01:14:31.000000 minidevice-1.0.1/minidevice/adb.py
+-rw-rw-rw-   0        0        0      269 2023-05-31 10:26:49.000000 minidevice-1.0.1/minidevice/config.py
+-rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.1/minidevice/device.py
+-rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.1/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.1/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.1/minidevice/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:41:03.342524 minidevice-1.0.1/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1205 2023-06-01 01:41:02.000000 minidevice-1.0.1/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-06-01 01:41:03.000000 minidevice-1.0.1/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 01:41:02.000000 minidevice-1.0.1/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-01 01:41:03.000000 minidevice-1.0.1/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-01 01:41:03.000000 minidevice-1.0.1/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 01:41:03.344519 minidevice-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      644 2023-06-01 01:40:04.000000 minidevice-1.0.1/setup.py
```

### Comparing `minidevice-1.0.0/README.md` & `minidevice-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.0/minidevice/adb.py` & `minidevice-1.0.1/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.0/minidevice/device.py` & `minidevice-1.0.1/minidevice/device.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.0/minidevice/minicap.py` & `minidevice-1.0.1/minidevice/minicap.py`

 * *Files identical despite different names*

