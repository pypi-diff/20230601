# Comparing `tmp/hj-generate-1.4.0.tar.gz` & `tmp/hj-generate-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-1.4.0.tar", last modified: Thu Jun  1 14:21:16 2023, max compression
+gzip compressed data, was "hj-generate-1.5.0.tar", last modified: Thu Jun  1 14:25:05 2023, max compression
```

## Comparing `hj-generate-1.4.0.tar` & `hj-generate-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:21:16.161782 hj-generate-1.4.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:21:16.161539 hj-generate-1.4.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:21:16.159298 hj-generate-1.4.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.4.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     1490 2023-06-01 14:20:47.000000 hj-generate-1.4.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:21:16.161069 hj-generate-1.4.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      267 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:21:16.161878 hj-generate-1.4.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      314 2023-06-01 14:20:47.000000 hj-generate-1.4.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:25:05.927158 hj-generate-1.5.0/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:25:05.926777 hj-generate-1.5.0/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:25:05.921863 hj-generate-1.5.0/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.5.0/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     1490 2023-06-01 14:20:47.000000 hj-generate-1.5.0/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:25:05.923456 hj-generate-1.5.0/generate/templates/
+-rw-r--r--   0 hj         (501) staff       (20)      470 2023-06-01 13:34:18.000000 hj-generate-1.5.0/generate/templates/controller.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 13:52:14.000000 hj-generate-1.5.0/generate/templates/service.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-1.5.0/generate/templates/sql.tpl
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:25:05.926217 hj-generate-1.5.0/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:25:05.000000 hj-generate-1.5.0/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 14:25:05.000000 hj-generate-1.5.0/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:25:05.000000 hj-generate-1.5.0/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:25:05.000000 hj-generate-1.5.0/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:25:05.000000 hj-generate-1.5.0/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:25:05.000000 hj-generate-1.5.0/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:25:05.927322 hj-generate-1.5.0/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 14:25:04.000000 hj-generate-1.5.0/setup.py
```

### Comparing `hj-generate-1.4.0/generate/generate_code.py` & `hj-generate-1.5.0/generate/generate_code.py`

 * *Files identical despite different names*

