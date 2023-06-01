# Comparing `tmp/TPDNE-utils-0.0.1.tar.gz` & `tmp/TPDNE-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPDNE-utils-0.0.1.tar", last modified: Thu Jun  1 16:10:36 2023, max compression
+gzip compressed data, was "TPDNE-utils-0.0.2.tar", last modified: Thu Jun  1 16:42:02 2023, max compression
```

## Comparing `TPDNE-utils-0.0.1.tar` & `TPDNE-utils-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:10:36.406052 TPDNE-utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 16:10:20.000000 TPDNE-utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 16:10:36.406052 TPDNE-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-01 16:10:20.000000 TPDNE-utils-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:10:36.402052 TPDNE-utils-0.0.1/TPDNE_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 16:10:36.000000 TPDNE-utils-0.0.1/TPDNE_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-01 16:10:36.000000 TPDNE-utils-0.0.1/TPDNE_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:10:36.000000 TPDNE-utils-0.0.1/TPDNE_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 16:10:36.000000 TPDNE-utils-0.0.1/TPDNE_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:10:36.000000 TPDNE-utils-0.0.1/TPDNE_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:10:36.406052 TPDNE-utils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-01 16:10:20.000000 TPDNE-utils-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:42:02.217028 TPDNE-utils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 16:41:49.000000 TPDNE-utils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 16:42:02.217028 TPDNE-utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-01 16:41:49.000000 TPDNE-utils-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:42:02.213028 TPDNE-utils-0.0.2/TPDNE_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 16:41:49.000000 TPDNE-utils-0.0.2/TPDNE_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-01 16:41:49.000000 TPDNE-utils-0.0.2/TPDNE_utils/tpdne.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:42:02.213028 TPDNE-utils-0.0.2/TPDNE_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 16:42:02.000000 TPDNE-utils-0.0.2/TPDNE_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 16:42:02.000000 TPDNE-utils-0.0.2/TPDNE_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:42:02.000000 TPDNE-utils-0.0.2/TPDNE_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 16:42:02.000000 TPDNE-utils-0.0.2/TPDNE_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 16:42:02.000000 TPDNE-utils-0.0.2/TPDNE_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:42:02.217028 TPDNE-utils-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-01 16:41:49.000000 TPDNE-utils-0.0.2/setup.py
```

### Comparing `TPDNE-utils-0.0.1/LICENSE` & `TPDNE-utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TPDNE-utils-0.0.1/README.md` & `TPDNE-utils-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # some function that returns a sampled image in the form of a 3 dimensional ndarray
 
 def generate_image():
     import numpy as np
     return np.random.randn(3, 1024, 1024)
 
-# saves a new sampled image
+# saves a new sampled image every 250ms as out/sampled.webp
 
 sample_image_and_save_repeatedly(generate_image, 'out/sampled')
 
 # use pm2 (node process manager) to run this script
 # then use nginx to serve out/sampled.web
 # optionally put behind cloudflare
```

### Comparing `TPDNE-utils-0.0.1/setup.py` & `TPDNE-utils-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'TPDNE-utils',
   packages = find_packages(exclude=[]),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'TPDNE',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/TPDNE',
   keywords = [],
```

