# Comparing `tmp/python-takauma-0.5.1.tar.gz` & `tmp/python-takauma-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-takauma-0.5.1.tar", last modified: Wed May 18 10:31:17 2022, max compression
+gzip compressed data, was "python-takauma-0.5.3.tar", last modified: Thu Jun  1 11:16:40 2023, max compression
```

## Comparing `python-takauma-0.5.1.tar` & `python-takauma-0.5.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:31:17.607713 python-takauma-0.5.1/
--rw-r--r--   0 aha        (501) staff       (20)      310 2022-05-18 10:31:17.607274 python-takauma-0.5.1/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)     2229 2020-05-15 10:48:55.000000 python-takauma-0.5.1/README.md
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:31:17.602905 python-takauma-0.5.1/python_takauma.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      310 2022-05-18 10:31:17.000000 python-takauma-0.5.1/python_takauma.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      378 2022-05-18 10:31:17.000000 python-takauma-0.5.1/python_takauma.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2022-05-18 10:31:17.000000 python-takauma-0.5.1/python_takauma.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)     3652 2022-05-18 10:31:17.000000 python-takauma-0.5.1/python_takauma.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2020-05-14 20:09:27.000000 python-takauma-0.5.1/python_takauma.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       47 2022-05-18 10:31:17.000000 python-takauma-0.5.1/python_takauma.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        8 2022-05-18 10:31:17.000000 python-takauma-0.5.1/python_takauma.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       38 2022-05-18 10:31:17.607847 python-takauma-0.5.1/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      569 2020-05-29 15:42:32.000000 python-takauma-0.5.1/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:31:17.606322 python-takauma-0.5.1/takauma/
--rw-r--r--   0 aha        (501) staff       (20)     1819 2021-01-08 13:44:33.000000 python-takauma-0.5.1/takauma/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     1715 2021-08-23 14:02:04.000000 python-takauma-0.5.1/takauma/hakemisto.py
--rw-r--r--   0 aha        (501) staff       (20)     2931 2022-03-09 07:37:11.000000 python-takauma-0.5.1/takauma/jakelu.py
--rw-r--r--   0 aha        (501) staff       (20)     1361 2020-05-22 14:28:49.000000 python-takauma-0.5.1/takauma/luokka.py
--rw-r--r--   0 aha        (501) staff       (20)     4465 2021-08-23 14:02:04.000000 python-takauma-0.5.1/takauma/moduuli.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:16:40.990776 python-takauma-0.5.3/
+-rw-r--r--   0 aha        (501) staff       (20)      254 2023-06-01 11:16:40.990588 python-takauma-0.5.3/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)     2229 2020-05-15 10:48:55.000000 python-takauma-0.5.3/README.md
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-01 11:13:49.000000 python-takauma-0.5.3/pyproject.toml
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:16:40.989229 python-takauma-0.5.3/python_takauma.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      254 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      393 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)     2697 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2020-05-14 20:09:27.000000 python-takauma-0.5.3/python_takauma.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       47 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-01 11:16:40.990818 python-takauma-0.5.3/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      569 2020-05-29 15:42:32.000000 python-takauma-0.5.3/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:16:40.990379 python-takauma-0.5.3/takauma/
+-rw-r--r--   0 aha        (501) staff       (20)     2086 2023-06-01 11:05:49.000000 python-takauma-0.5.3/takauma/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     1715 2021-08-23 14:02:04.000000 python-takauma-0.5.3/takauma/hakemisto.py
+-rw-r--r--   0 aha        (501) staff       (20)     2931 2022-03-09 07:37:11.000000 python-takauma-0.5.3/takauma/jakelu.py
+-rw-r--r--   0 aha        (501) staff       (20)     1361 2020-05-22 14:28:49.000000 python-takauma-0.5.3/takauma/luokka.py
+-rw-r--r--   0 aha        (501) staff       (20)     4465 2021-08-23 14:02:04.000000 python-takauma-0.5.3/takauma/moduuli.py
```

### Comparing `python-takauma-0.5.1/README.md` & `python-takauma-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.1/setup.py` & `python-takauma-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.1/takauma/__init__.py` & `python-takauma-0.5.3/takauma/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=invalid-name, unused-import
 
 import importlib
 import sys
 import threading
+import warnings
 
 import mmaare
 
 # pylint: disable=import-error
 from .hakemisto import Versiohakemisto
 from .jakelu import _jakelu
 from .luokka import Versio, Versiot
@@ -70,9 +71,15 @@
 
 # Lisää edellä kuvatut määreet automaattisesti
 # tämän jälkeen tuotuihin moduuleihin.
 sys.meta_path.insert(0, Etsija())
 
 
 # Lisää määreet heti aiemmin tuotuihin moduuleihin.
-for aiemmin_tuotu_moduuli in sys.modules.values():
-  tuotu(aiemmin_tuotu_moduuli)
+# Ohitetaan mahdolliset varoitukset __getattr__-
+# funktion ylikuormittamisen yhteydessä.
+# Huomaa, että kaikki Python-moduulit eivät salli
+# tämän funktion ylikuormittamista.
+with warnings.catch_warnings():
+  warnings.simplefilter('ignore')
+  for aiemmin_tuotu_moduuli in sys.modules.values():
+    tuotu(aiemmin_tuotu_moduuli)
```

### Comparing `python-takauma-0.5.1/takauma/hakemisto.py` & `python-takauma-0.5.3/takauma/hakemisto.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.1/takauma/jakelu.py` & `python-takauma-0.5.3/takauma/jakelu.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.1/takauma/luokka.py` & `python-takauma-0.5.3/takauma/luokka.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.1/takauma/moduuli.py` & `python-takauma-0.5.3/takauma/moduuli.py`

 * *Files identical despite different names*

