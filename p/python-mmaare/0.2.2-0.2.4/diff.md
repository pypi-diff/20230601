# Comparing `tmp/python-mmaare-0.2.2.tar.gz` & `tmp/python-mmaare-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aha/git/python-mmaare/dist/tmparja7sx6/python-mmaare-0.2.2.tar", last modified: Wed May 18 10:32:46 2022, max compression
+gzip compressed data, was "python-mmaare-0.2.4.tar", last modified: Thu Jun  1 11:14:45 2023, max compression
```

## Comparing `python-mmaare-0.2.2.tar` & `python-mmaare-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:32:46.229888 python-mmaare-0.2.2/
--rw-r--r--   0 aha        (501) staff       (20)      222 2022-05-18 10:32:46.229622 python-mmaare-0.2.2/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      218 2020-05-25 07:05:46.000000 python-mmaare-0.2.2/README.md
--rw-r--r--   0 aha        (501) staff       (20)     4953 2021-09-27 06:39:03.000000 python-mmaare-0.2.2/mmaare.py
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-03-18 13:07:55.000000 python-mmaare-0.2.2/pyproject.toml
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-05-18 10:32:46.229244 python-mmaare-0.2.2/python_mmaare.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      222 2022-05-18 10:32:45.000000 python-mmaare-0.2.2/python_mmaare.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      228 2022-05-18 10:32:46.000000 python-mmaare-0.2.2/python_mmaare.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2022-05-18 10:32:45.000000 python-mmaare-0.2.2/python_mmaare.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)     1615 2022-05-18 10:32:45.000000 python-mmaare-0.2.2/python_mmaare.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        7 2022-05-18 10:32:46.000000 python-mmaare-0.2.2/python_mmaare.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       38 2022-05-18 10:32:46.229999 python-mmaare-0.2.2/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      327 2021-05-25 12:29:33.000000 python-mmaare-0.2.2/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:14:45.393906 python-mmaare-0.2.4/
+-rw-r--r--   0 aha        (501) staff       (20)      222 2023-06-01 11:14:45.393762 python-mmaare-0.2.4/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      218 2020-05-25 07:05:46.000000 python-mmaare-0.2.4/README.md
+-rw-r--r--   0 aha        (501) staff       (20)     5349 2023-06-01 10:54:16.000000 python-mmaare-0.2.4/mmaare.py
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-01 11:13:49.000000 python-mmaare-0.2.4/pyproject.toml
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:14:45.393594 python-mmaare-0.2.4/python_mmaare.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      222 2023-06-01 11:14:45.000000 python-mmaare-0.2.4/python_mmaare.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      228 2023-06-01 11:14:45.000000 python-mmaare-0.2.4/python_mmaare.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-01 11:14:45.000000 python-mmaare-0.2.4/python_mmaare.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)     1384 2023-06-01 11:14:45.000000 python-mmaare-0.2.4/python_mmaare.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        7 2023-06-01 11:14:45.000000 python-mmaare-0.2.4/python_mmaare.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-01 11:14:45.393943 python-mmaare-0.2.4/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      327 2023-06-01 11:11:59.000000 python-mmaare-0.2.4/setup.py
```

### Comparing `python-mmaare-0.2.2/mmaare.py` & `python-mmaare-0.2.4/mmaare.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 >>> ...
 >>>  print(sys.modules['__main__'].f) # --> __niam__
 >>>  print(xyz.__nimi_vaarinpain__) # --> zyx
 '''
 
 import functools
 import sys
+import warnings
 
 
 class _Py36:
   '''Python 3.6 -toteutus.
 
   Periytetään moduulin luokka, lisätään datakuvaaja.
   '''
@@ -104,20 +105,36 @@
 
       __getattr__.__rekursio__.add(avain)
       try:
         return __getattr__.__wrapped__(avain)
       finally:
         __getattr__.__rekursio__.discard(avain)
       # def __getattr__
-    self.moduuli.__getattr__ = functools.wraps(getattr(
-      self.moduuli,
-      '__getattr__',
-      functools.partial(self._ei_loydy, self.moduuli)
-    ))(__getattr__)
-    __getattr__.__rekursio__ = set()
+
+    try:
+      mod_getattr = self.moduuli.__getattr__
+    except AttributeError:
+      mod_getattr = functools.partial(
+        self._ei_loydy,
+        self.moduuli
+      )
+    try:
+      self.moduuli.__getattr__ = functools.wraps(
+        mod_getattr
+      )(__getattr__)
+    except AttributeError:
+      # Mikäli moduuli ei salli `__getattr__`-
+      # funktion asettamista, ohitetaan.
+      warnings.warn(
+        f'Funktion `{self.moduuli}.__getattr__`'
+        f' asettaminen ei sallittu, ohitetaan.',
+        stacklevel=3,
+      )
+    else:
+      __getattr__.__rekursio__ = set()
     # def __init__
 
   @staticmethod
   def _ei_loydy(moduuli, avain):
     raise AttributeError(f'{moduuli.__name__}: {avain!r}')
     # def _ei_loydy
```

