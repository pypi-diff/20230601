# Comparing `tmp/hj-generate-1.2.0.tar.gz` & `tmp/hj-generate-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-1.2.0.tar", last modified: Thu Jun  1 14:12:20 2023, max compression
+gzip compressed data, was "hj-generate-1.3.0.tar", last modified: Thu Jun  1 14:17:36 2023, max compression
```

## Comparing `hj-generate-1.2.0.tar` & `hj-generate-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:12:20.536335 hj-generate-1.2.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:12:20.536055 hj-generate-1.2.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:12:20.533955 hj-generate-1.2.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.2.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     1481 2023-06-01 14:01:26.000000 hj-generate-1.2.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:12:20.535637 hj-generate-1.2.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:12:20.000000 hj-generate-1.2.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      267 2023-06-01 14:12:20.000000 hj-generate-1.2.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:12:20.000000 hj-generate-1.2.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       54 2023-06-01 14:12:20.000000 hj-generate-1.2.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:12:20.000000 hj-generate-1.2.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:12:20.000000 hj-generate-1.2.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:12:20.536423 hj-generate-1.2.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      308 2023-06-01 14:12:09.000000 hj-generate-1.2.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:17:36.674997 hj-generate-1.3.0/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:17:36.674674 hj-generate-1.3.0/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:17:36.672557 hj-generate-1.3.0/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.3.0/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     1481 2023-06-01 14:01:26.000000 hj-generate-1.3.0/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:17:36.674251 hj-generate-1.3.0/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      267 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:17:36.675162 hj-generate-1.3.0/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      314 2023-06-01 14:17:26.000000 hj-generate-1.3.0/setup.py
```

### Comparing `hj-generate-1.2.0/generate/generate_code.py` & `hj-generate-1.3.0/generate/generate_code.py`

 * *Files identical despite different names*

