# Comparing `tmp/doremi-1.0.0.tar.gz` & `tmp/doremi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doremi-1.0.0.tar", last modified: Thu Jun  1 02:47:23 2023, max compression
+gzip compressed data, was "doremi-1.0.1.tar", last modified: Thu Jun  1 02:54:43 2023, max compression
```

## Comparing `doremi-1.0.0.tar` & `doremi-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-01 02:47:23.640768 doremi-1.0.0/
--rw-r--r--   0 james      (501) staff       (20)     1081 2023-05-30 21:29:00.000000 doremi-1.0.0/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      311 2023-06-01 02:47:23.640597 doremi-1.0.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1006 2023-06-01 02:45:30.000000 doremi-1.0.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-01 02:47:23.639575 doremi-1.0.0/doremi/
--rw-r--r--   0 james      (501) staff       (20)       24 2023-06-01 02:42:07.000000 doremi-1.0.0/doremi/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1653 2023-05-30 21:24:13.000000 doremi-1.0.0/doremi/doremi.py
--rw-r--r--   0 james      (501) staff       (20)     2404 2023-05-30 21:10:58.000000 doremi-1.0.0/doremi/td_psola.py
--rw-r--r--   0 james      (501) staff       (20)     5352 2023-05-30 21:00:33.000000 doremi-1.0.0/doremi/tuners.py
--rw-r--r--   0 james      (501) staff       (20)     2676 2023-05-30 21:10:33.000000 doremi-1.0.0/doremi/util.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-01 02:47:23.640427 doremi-1.0.0/doremi.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      311 2023-06-01 02:47:23.000000 doremi-1.0.0/doremi.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      281 2023-06-01 02:47:23.000000 doremi-1.0.0/doremi.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-01 02:47:23.000000 doremi-1.0.0/doremi.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        6 2023-06-01 02:47:23.000000 doremi-1.0.0/doremi.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        7 2023-06-01 02:47:23.000000 doremi-1.0.0/doremi.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       85 2023-05-30 20:36:42.000000 doremi-1.0.0/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-01 02:47:23.640830 doremi-1.0.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      427 2023-06-01 02:42:01.000000 doremi-1.0.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-01 02:54:43.437936 doremi-1.0.1/
+-rw-r--r--   0 james      (501) staff       (20)     1081 2023-06-01 02:52:06.000000 doremi-1.0.1/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      312 2023-06-01 02:54:43.437775 doremi-1.0.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1006 2023-06-01 02:52:06.000000 doremi-1.0.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-01 02:54:43.436882 doremi-1.0.1/doremi/
+-rw-r--r--   0 james      (501) staff       (20)       24 2023-06-01 02:52:06.000000 doremi-1.0.1/doremi/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1653 2023-06-01 02:52:06.000000 doremi-1.0.1/doremi/doremi.py
+-rw-r--r--   0 james      (501) staff       (20)     2404 2023-06-01 02:52:06.000000 doremi-1.0.1/doremi/td_psola.py
+-rw-r--r--   0 james      (501) staff       (20)     5352 2023-06-01 02:52:06.000000 doremi-1.0.1/doremi/tuners.py
+-rw-r--r--   0 james      (501) staff       (20)     2676 2023-06-01 02:52:06.000000 doremi-1.0.1/doremi/util.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-01 02:54:43.437583 doremi-1.0.1/doremi.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)      312 2023-06-01 02:54:43.000000 doremi-1.0.1/doremi.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      281 2023-06-01 02:54:43.000000 doremi-1.0.1/doremi.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-01 02:54:43.000000 doremi-1.0.1/doremi.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       16 2023-06-01 02:54:43.000000 doremi-1.0.1/doremi.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        7 2023-06-01 02:54:43.000000 doremi-1.0.1/doremi.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       85 2023-06-01 02:52:07.000000 doremi-1.0.1/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-01 02:54:43.437989 doremi-1.0.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)      441 2023-06-01 02:54:10.000000 doremi-1.0.1/setup.py
```

### Comparing `doremi-1.0.0/LICENSE.txt` & `doremi-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `doremi-1.0.0/README.md` & `doremi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `doremi-1.0.0/doremi/doremi.py` & `doremi-1.0.1/doremi/doremi.py`

 * *Files identical despite different names*

### Comparing `doremi-1.0.0/doremi/td_psola.py` & `doremi-1.0.1/doremi/td_psola.py`

 * *Files identical despite different names*

### Comparing `doremi-1.0.0/doremi/tuners.py` & `doremi-1.0.1/doremi/tuners.py`

 * *Files identical despite different names*

### Comparing `doremi-1.0.0/doremi/util.py` & `doremi-1.0.1/doremi/util.py`

 * *Files identical despite different names*

