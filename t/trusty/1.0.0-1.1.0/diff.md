# Comparing `tmp/trusty-1.0.0.tar.gz` & `tmp/trusty-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trusty-1.0.0.tar", last modified: Fri Aug 12 20:47:31 2022, max compression
+gzip compressed data, was "trusty-1.1.0.tar", last modified: Thu Jun  1 03:50:11 2023, max compression
```

## Comparing `trusty-1.0.0.tar` & `trusty-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-12 20:47:31.710438 trusty-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1153 2022-08-12 20:47:31.709438 trusty-1.0.0/PKG-INFO
--rw-------   0 root         (0) root         (0)      850 2022-08-12 20:42:08.000000 trusty-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-12 20:47:31.710438 trusty-1.0.0/setup.cfg
--rw-------   0 root         (0) root         (0)      572 2022-08-12 20:46:50.000000 trusty-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-12 20:47:31.708438 trusty-1.0.0/trusty/
--rw-------   0 root         (0) root         (0)       24 2022-08-12 20:29:11.000000 trusty-1.0.0/trusty/__init__.py
--rw-------   0 root         (0) root         (0)     1262 2022-08-12 20:38:13.000000 trusty-1.0.0/trusty/trusty.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-12 20:47:31.709438 trusty-1.0.0/trusty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1153 2022-08-12 20:47:31.000000 trusty-1.0.0/trusty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      174 2022-08-12 20:47:31.000000 trusty-1.0.0/trusty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-12 20:47:31.000000 trusty-1.0.0/trusty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-08-12 20:47:31.000000 trusty-1.0.0/trusty.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 03:50:11.875165 trusty-1.1.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1055 2023-06-01 03:50:11.875165 trusty-1.1.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      699 2023-05-30 22:03:05.000000 trusty-1.1.0/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-06-01 03:50:11.875165 trusty-1.1.0/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      598 2023-06-01 03:48:11.000000 trusty-1.1.0/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 03:50:11.875165 trusty-1.1.0/trusty/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       24 2023-05-30 22:03:05.000000 trusty-1.1.0/trusty/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      743 2023-06-01 03:48:34.000000 trusty-1.1.0/trusty/trusty.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 03:50:11.875165 trusty-1.1.0/trusty.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1055 2023-06-01 03:50:11.000000 trusty-1.1.0/trusty.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      174 2023-06-01 03:50:11.000000 trusty-1.1.0/trusty.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-01 03:50:11.000000 trusty-1.1.0/trusty.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-06-01 03:50:11.000000 trusty-1.1.0/trusty.egg-info/top_level.txt
```

