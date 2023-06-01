# Comparing `tmp/git-versiointi-1.6rc2.tar.gz` & `tmp/git-versiointi-1.6rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-versiointi-1.6rc2.tar", last modified: Wed May 31 12:56:57 2023, max compression
+gzip compressed data, was "git-versiointi-1.6rc3.tar", last modified: Thu Jun  1 11:13:00 2023, max compression
```

## Comparing `git-versiointi-1.6rc2.tar` & `git-versiointi-1.6rc3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-31 12:56:57.461923 git-versiointi-1.6rc2/
--rw-r--r--   0 aha        (501) staff       (20)     6656 2023-05-31 12:56:57.461802 git-versiointi-1.6rc2/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)     6306 2023-01-20 12:41:07.000000 git-versiointi-1.6rc2/README.md
--rw-r--r--   0 aha        (501) staff       (20)      100 2022-06-20 07:59:54.000000 git-versiointi-1.6rc2/_versiointi_setuptools_build_meta.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-31 12:56:57.459659 git-versiointi-1.6rc2/git_versiointi.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)     6656 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      509 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      247 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)       25 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)       45 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)      140 2023-05-15 12:45:13.000000 git-versiointi-1.6rc2/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-05-31 12:56:57.461959 git-versiointi-1.6rc2/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)     1143 2023-05-15 12:45:03.000000 git-versiointi-1.6rc2/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-31 12:56:57.461524 git-versiointi-1.6rc2/versiointi/
--rw-r--r--   0 aha        (501) staff       (20)     5262 2023-05-15 13:01:31.000000 git-versiointi-1.6rc2/versiointi/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      566 2022-06-08 07:34:13.000000 git-versiointi-1.6rc2/versiointi/egg_info.py
--rw-r--r--   0 aha        (501) staff       (20)     5174 2023-01-20 15:11:25.000000 git-versiointi-1.6rc2/versiointi/kaytanto.py
--rw-r--r--   0 aha        (501) staff       (20)     1051 2023-05-31 12:55:13.000000 git-versiointi-1.6rc2/versiointi/oletus.py
--rw-r--r--   0 aha        (501) staff       (20)     1815 2022-06-08 07:34:13.000000 git-versiointi-1.6rc2/versiointi/parametrit.py
--rw-r--r--   0 aha        (501) staff       (20)     5491 2023-01-20 15:11:25.000000 git-versiointi-1.6rc2/versiointi/repo.py
--rw-r--r--   0 aha        (501) staff       (20)     2530 2022-06-08 07:51:15.000000 git-versiointi-1.6rc2/versiointi/tiedostot.py
--rw-r--r--   0 aha        (501) staff       (20)      654 2022-06-08 07:34:13.000000 git-versiointi-1.6rc2/versiointi/vaatimukset.py
--rw-r--r--   0 aha        (501) staff       (20)     3325 2023-01-20 12:41:07.000000 git-versiointi-1.6rc2/versiointi/versiointi.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:13:00.810223 git-versiointi-1.6rc3/
+-rw-r--r--   0 aha        (501) staff       (20)     6656 2023-06-01 11:13:00.810093 git-versiointi-1.6rc3/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)     6306 2023-01-20 12:41:07.000000 git-versiointi-1.6rc3/README.md
+-rw-r--r--   0 aha        (501) staff       (20)      100 2022-06-20 07:59:54.000000 git-versiointi-1.6rc3/_versiointi_setuptools_build_meta.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:13:00.807717 git-versiointi-1.6rc3/git_versiointi.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)     6656 2023-06-01 11:13:00.000000 git-versiointi-1.6rc3/git_versiointi.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      547 2023-06-01 11:13:00.000000 git-versiointi-1.6rc3/git_versiointi.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-01 11:13:00.000000 git-versiointi-1.6rc3/git_versiointi.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-01 11:13:00.000000 git-versiointi-1.6rc3/git_versiointi.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)        2 2023-05-31 12:59:41.000000 git-versiointi-1.6rc3/git_versiointi.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)       25 2023-06-01 11:13:00.000000 git-versiointi-1.6rc3/git_versiointi.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)       45 2023-06-01 11:13:00.000000 git-versiointi-1.6rc3/git_versiointi.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)      140 2023-05-15 12:45:13.000000 git-versiointi-1.6rc3/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-01 11:13:00.810259 git-versiointi-1.6rc3/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)     1143 2023-05-15 12:45:03.000000 git-versiointi-1.6rc3/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:13:00.809826 git-versiointi-1.6rc3/versiointi/
+-rw-r--r--   0 aha        (501) staff       (20)     5262 2023-05-15 13:01:31.000000 git-versiointi-1.6rc3/versiointi/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      566 2022-06-08 07:34:13.000000 git-versiointi-1.6rc3/versiointi/egg_info.py
+-rw-r--r--   0 aha        (501) staff       (20)     5174 2023-01-20 15:11:25.000000 git-versiointi-1.6rc3/versiointi/kaytanto.py
+-rw-r--r--   0 aha        (501) staff       (20)     1010 2023-06-01 07:56:10.000000 git-versiointi-1.6rc3/versiointi/oletus.py
+-rw-r--r--   0 aha        (501) staff       (20)     1815 2022-06-08 07:34:13.000000 git-versiointi-1.6rc3/versiointi/parametrit.py
+-rw-r--r--   0 aha        (501) staff       (20)     5491 2023-01-20 15:11:25.000000 git-versiointi-1.6rc3/versiointi/repo.py
+-rw-r--r--   0 aha        (501) staff       (20)     2530 2022-06-08 07:51:15.000000 git-versiointi-1.6rc3/versiointi/tiedostot.py
+-rw-r--r--   0 aha        (501) staff       (20)      654 2022-06-08 07:34:13.000000 git-versiointi-1.6rc3/versiointi/vaatimukset.py
+-rw-r--r--   0 aha        (501) staff       (20)     3325 2023-01-20 12:41:07.000000 git-versiointi-1.6rc3/versiointi/versiointi.py
```

### Comparing `git-versiointi-1.6rc2/PKG-INFO` & `git-versiointi-1.6rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-versiointi
-Version: 1.6rc2
+Version: 1.6rc3
 Summary: Asennettavan pakettiversion haku git-leimojen mukaan
 Home-page: https://github.com/an7oine/git-versiointi.git
 Author: Antti Hautaniemi
 Author-email: antti.hautaniemi@pispalanit.fi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `git-versiointi-1.6rc2/README.md` & `git-versiointi-1.6rc3/README.md`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/git_versiointi.egg-info/PKG-INFO` & `git-versiointi-1.6rc3/git_versiointi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-versiointi
-Version: 1.6rc2
+Version: 1.6rc3
 Summary: Asennettavan pakettiversion haku git-leimojen mukaan
 Home-page: https://github.com/an7oine/git-versiointi.git
 Author: Antti Hautaniemi
 Author-email: antti.hautaniemi@pispalanit.fi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `git-versiointi-1.6rc2/setup.py` & `git-versiointi-1.6rc3/setup.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/__init__.py` & `git-versiointi-1.6rc3/versiointi/__init__.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/egg_info.py` & `git-versiointi-1.6rc3/versiointi/egg_info.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/kaytanto.py` & `git-versiointi-1.6rc3/versiointi/kaytanto.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/oletus.py` & `git-versiointi-1.6rc3/versiointi/oletus.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,16 @@
   'refs/heads/ refs/remotes/origin/': (
     '''{pohja}{int(indeksi)+etaisyys if indeksi else f'+{tunnus}.{etaisyys}'}'''
   ),
 
   # Master-haara tai versiohaara (v-X.Y):
   # indeksoitu kehitysversio tai etäisyyden mukainen pääte.
   ' '.join((
-    'refs/heads/master',
-    'refs/remotes/origin/master',
-    'refs/heads/v-[0-9].*',
-    'refs/remotes/origin/v-[0-9].*',
+    'refs/heads/(master|v-[0-9].*)',
+    'refs/remotes/origin/(master|v-[0-9].*)',
   )): (
     '''{pohja}{int(indeksi)+etaisyys if indeksi else f'.{etaisyys}'}'''
   ),
 
   # Leimattu kehitysversiosarja: tulkitaan viimeinen luku indeksinä.
   'refs/tags/v[0-9].*': '''{tunnus[1:]}{indeksoitu}''',
```

### Comparing `git-versiointi-1.6rc2/versiointi/parametrit.py` & `git-versiointi-1.6rc3/versiointi/parametrit.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/repo.py` & `git-versiointi-1.6rc3/versiointi/repo.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/tiedostot.py` & `git-versiointi-1.6rc3/versiointi/tiedostot.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/vaatimukset.py` & `git-versiointi-1.6rc3/versiointi/vaatimukset.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc2/versiointi/versiointi.py` & `git-versiointi-1.6rc3/versiointi/versiointi.py`

 * *Files identical despite different names*

