# Comparing `tmp/FileKit-1.0.1.tar.gz` & `tmp/FileKit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileKit-1.0.1.tar", last modified: Thu Jun  1 14:19:13 2023, max compression
+gzip compressed data, was "FileKit-1.0.2.tar", last modified: Thu Jun  1 14:33:44 2023, max compression
```

## Comparing `FileKit-1.0.1.tar` & `FileKit-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:19:13.950407 FileKit-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-01 14:19:13.942690 FileKit-1.0.1/FileKit/
--rw-rw-rw-   0        0        0     1280 2023-06-01 13:44:42.000000 FileKit-1.0.1/FileKit/File.py
--rw-rw-rw-   0        0        0       24 2023-06-01 11:55:48.000000 FileKit-1.0.1/FileKit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:19:13.948403 FileKit-1.0.1/FileKit.egg-info/
--rw-rw-rw-   0        0        0       70 2023-06-01 14:19:13.000000 FileKit-1.0.1/FileKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-01 14:19:13.000000 FileKit-1.0.1/FileKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:19:13.000000 FileKit-1.0.1/FileKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 14:19:13.000000 FileKit-1.0.1/FileKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-06-01 14:19:13.949423 FileKit-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-06-01 14:18:17.000000 FileKit-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 14:19:13.950407 FileKit-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      229 2023-06-01 14:04:08.000000 FileKit-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:33:44.730394 FileKit-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-01 14:33:44.722716 FileKit-1.0.2/FileKit/
+-rw-rw-rw-   0        0        0     1280 2023-06-01 13:44:42.000000 FileKit-1.0.2/FileKit/File.py
+-rw-rw-rw-   0        0        0       24 2023-06-01 11:55:48.000000 FileKit-1.0.2/FileKit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:33:44.728672 FileKit-1.0.2/FileKit.egg-info/
+-rw-rw-rw-   0        0        0       70 2023-06-01 14:33:44.000000 FileKit-1.0.2/FileKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-01 14:33:44.000000 FileKit-1.0.2/FileKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:33:44.000000 FileKit-1.0.2/FileKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 14:33:44.000000 FileKit-1.0.2/FileKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-06-01 14:33:44.730394 FileKit-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-06-01 14:32:32.000000 FileKit-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 14:33:44.730394 FileKit-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      229 2023-06-01 14:33:24.000000 FileKit-1.0.2/setup.py
```

### Comparing `FileKit-1.0.1/FileKit/File.py` & `FileKit-1.0.2/FileKit/File.py`

 * *Files identical despite different names*

