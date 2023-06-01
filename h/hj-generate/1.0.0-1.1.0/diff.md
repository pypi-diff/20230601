# Comparing `tmp/hj-generate-1.0.0.tar.gz` & `tmp/hj-generate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-1.0.0.tar", last modified: Thu Jun  1 14:06:11 2023, max compression
+gzip compressed data, was "hj-generate-1.1.0.tar", last modified: Thu Jun  1 14:09:15 2023, max compression
```

## Comparing `hj-generate-1.0.0.tar` & `hj-generate-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:06:11.165748 hj-generate-1.0.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:06:11.165481 hj-generate-1.0.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:06:11.163481 hj-generate-1.0.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.0.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     1481 2023-06-01 14:01:26.000000 hj-generate-1.0.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:06:11.165054 hj-generate-1.0.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:06:11.000000 hj-generate-1.0.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      267 2023-06-01 14:06:11.000000 hj-generate-1.0.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:06:11.000000 hj-generate-1.0.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       46 2023-06-01 14:06:11.000000 hj-generate-1.0.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:06:11.000000 hj-generate-1.0.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:06:11.000000 hj-generate-1.0.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:06:11.165835 hj-generate-1.0.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      300 2023-06-01 14:05:45.000000 hj-generate-1.0.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:09:15.760226 hj-generate-1.1.0/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:09:15.759948 hj-generate-1.1.0/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:09:15.757734 hj-generate-1.1.0/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.1.0/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     1481 2023-06-01 14:01:26.000000 hj-generate-1.1.0/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:09:15.759328 hj-generate-1.1.0/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:09:15.000000 hj-generate-1.1.0/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      267 2023-06-01 14:09:15.000000 hj-generate-1.1.0/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:09:15.000000 hj-generate-1.1.0/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       54 2023-06-01 14:09:15.000000 hj-generate-1.1.0/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:09:15.000000 hj-generate-1.1.0/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:09:15.000000 hj-generate-1.1.0/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:09:15.760353 hj-generate-1.1.0/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      308 2023-06-01 14:08:58.000000 hj-generate-1.1.0/setup.py
```

### Comparing `hj-generate-1.0.0/generate/generate_code.py` & `hj-generate-1.1.0/generate/generate_code.py`

 * *Files identical despite different names*

