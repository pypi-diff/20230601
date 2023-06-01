# Comparing `tmp/lchelper-0.0.1.tar.gz` & `tmp/lchelper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lchelper-0.0.1.tar", last modified: Thu Jun  1 04:08:00 2023, max compression
+gzip compressed data, was "lchelper-0.0.2.tar", last modified: Thu Jun  1 04:25:33 2023, max compression
```

## Comparing `lchelper-0.0.1.tar` & `lchelper-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:08:00.639639 lchelper-0.0.1/
--rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 04:08:00.639306 lchelper-0.0.1/PKG-INFO
-drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:08:00.636768 lchelper-0.0.1/lchelper/
--rw-r--r--   0 edwhan     (501) staff       (20)        0 2023-06-01 04:00:06.000000 lchelper-0.0.1/lchelper/__init__.py
--rw-r--r--   0 edwhan     (501) staff       (20)       19 2023-06-01 04:01:52.000000 lchelper-0.0.1/lchelper/constants.py
--rw-r--r--   0 edwhan     (501) staff       (20)       95 2023-06-01 04:01:18.000000 lchelper-0.0.1/lchelper/node.py
-drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:08:00.638802 lchelper-0.0.1/lchelper.egg-info/
--rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 04:08:00.000000 lchelper-0.0.1/lchelper.egg-info/PKG-INFO
--rw-r--r--   0 edwhan     (501) staff       (20)      196 2023-06-01 04:08:00.000000 lchelper-0.0.1/lchelper.egg-info/SOURCES.txt
--rw-r--r--   0 edwhan     (501) staff       (20)        1 2023-06-01 04:08:00.000000 lchelper-0.0.1/lchelper.egg-info/dependency_links.txt
--rw-r--r--   0 edwhan     (501) staff       (20)        9 2023-06-01 04:08:00.000000 lchelper-0.0.1/lchelper.egg-info/top_level.txt
--rw-r--r--   0 edwhan     (501) staff       (20)       38 2023-06-01 04:08:00.639749 lchelper-0.0.1/setup.cfg
--rw-r--r--   0 edwhan     (501) staff       (20)      306 2023-06-01 04:03:22.000000 lchelper-0.0.1/setup.py
+drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:25:33.981713 lchelper-0.0.2/
+-rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 04:25:33.981315 lchelper-0.0.2/PKG-INFO
+drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:25:33.978748 lchelper-0.0.2/lchelper/
+-rw-r--r--   0 edwhan     (501) staff       (20)        0 2023-06-01 04:00:06.000000 lchelper-0.0.2/lchelper/__init__.py
+-rw-r--r--   0 edwhan     (501) staff       (20)       19 2023-06-01 04:25:27.000000 lchelper-0.0.2/lchelper/constants.py
+-rw-r--r--   0 edwhan     (501) staff       (20)       95 2023-06-01 04:01:18.000000 lchelper-0.0.2/lchelper/linkedlist.py
+drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:25:33.980801 lchelper-0.0.2/lchelper.egg-info/
+-rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 04:25:33.000000 lchelper-0.0.2/lchelper.egg-info/PKG-INFO
+-rw-r--r--   0 edwhan     (501) staff       (20)      202 2023-06-01 04:25:33.000000 lchelper-0.0.2/lchelper.egg-info/SOURCES.txt
+-rw-r--r--   0 edwhan     (501) staff       (20)        1 2023-06-01 04:25:33.000000 lchelper-0.0.2/lchelper.egg-info/dependency_links.txt
+-rw-r--r--   0 edwhan     (501) staff       (20)        9 2023-06-01 04:25:33.000000 lchelper-0.0.2/lchelper.egg-info/top_level.txt
+-rw-r--r--   0 edwhan     (501) staff       (20)       38 2023-06-01 04:25:33.981835 lchelper-0.0.2/setup.cfg
+-rw-r--r--   0 edwhan     (501) staff       (20)      306 2023-06-01 04:03:22.000000 lchelper-0.0.2/setup.py
```

