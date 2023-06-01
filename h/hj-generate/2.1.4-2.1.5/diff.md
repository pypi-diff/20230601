# Comparing `tmp/hj-generate-2.1.4.tar.gz` & `tmp/hj-generate-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-2.1.4.tar", last modified: Thu Jun  1 15:17:52 2023, max compression
+gzip compressed data, was "hj-generate-2.1.5.tar", last modified: Thu Jun  1 15:20:35 2023, max compression
```

## Comparing `hj-generate-2.1.4.tar` & `hj-generate-2.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:17:52.068911 hj-generate-2.1.4/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:17:52.068566 hj-generate-2.1.4/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:17:52.064790 hj-generate-2.1.4/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-2.1.4/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     2999 2023-06-01 15:17:39.000000 hj-generate-2.1.4/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:17:52.065830 hj-generate-2.1.4/generate/templates/
--rw-r--r--   0 hj         (501) staff       (20)      463 2023-06-01 14:59:14.000000 hj-generate-2.1.4/generate/templates/controller.tpl
--rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-2.1.4/generate/templates/service.tpl
--rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-2.1.4/generate/templates/sql.tpl
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:17:52.067927 hj-generate-2.1.4/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:17:52.000000 hj-generate-2.1.4/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 15:17:52.000000 hj-generate-2.1.4/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 15:17:52.000000 hj-generate-2.1.4/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 15:17:52.000000 hj-generate-2.1.4/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 15:17:52.000000 hj-generate-2.1.4/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 15:17:52.000000 hj-generate-2.1.4/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 15:17:52.069048 hj-generate-2.1.4/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 15:17:39.000000 hj-generate-2.1.4/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:20:35.815127 hj-generate-2.1.5/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:20:35.814319 hj-generate-2.1.5/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:20:35.810083 hj-generate-2.1.5/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-2.1.5/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     2999 2023-06-01 15:17:39.000000 hj-generate-2.1.5/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:20:35.810864 hj-generate-2.1.5/generate/templates/
+-rw-r--r--   0 hj         (501) staff       (20)      461 2023-06-01 15:19:37.000000 hj-generate-2.1.5/generate/templates/controller.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-2.1.5/generate/templates/service.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      111 2023-06-01 15:20:28.000000 hj-generate-2.1.5/generate/templates/sql.tpl
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:20:35.813799 hj-generate-2.1.5/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:20:35.000000 hj-generate-2.1.5/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 15:20:35.000000 hj-generate-2.1.5/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 15:20:35.000000 hj-generate-2.1.5/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 15:20:35.000000 hj-generate-2.1.5/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 15:20:35.000000 hj-generate-2.1.5/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 15:20:35.000000 hj-generate-2.1.5/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 15:20:35.815486 hj-generate-2.1.5/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 15:20:28.000000 hj-generate-2.1.5/setup.py
```

### Comparing `hj-generate-2.1.4/generate/generate_code.py` & `hj-generate-2.1.5/generate/generate_code.py`

 * *Files identical despite different names*

