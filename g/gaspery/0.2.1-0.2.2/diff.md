# Comparing `tmp/gaspery-0.2.1.tar.gz` & `tmp/gaspery-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaspery-0.2.1.tar", last modified: Tue May 30 00:36:20 2023, max compression
+gzip compressed data, was "gaspery-0.2.2.tar", last modified: Thu Jun  1 17:42:17 2023, max compression
```

## Comparing `gaspery-0.2.1.tar` & `gaspery-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.785873 gaspery-0.2.1/
--rw-r--r--   0 chris      (501) staff       (20)     1075 2023-04-08 21:45:04.000000 gaspery-0.2.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     4226 2023-05-30 00:36:20.785187 gaspery-0.2.1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     3661 2023-04-08 21:45:04.000000 gaspery-0.2.1/README.md
--rw-r--r--   0 chris      (501) staff       (20)      600 2023-05-30 00:36:01.000000 gaspery-0.2.1/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-30 00:36:20.786271 gaspery-0.2.1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      433 2023-05-30 00:35:50.000000 gaspery-0.2.1/setup.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.775098 gaspery-0.2.1/src/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.779580 gaspery-0.2.1/src/gaspery/
--rw-r--r--   0 chris      (501) staff       (20)      307 2023-04-08 21:45:05.000000 gaspery-0.2.1/src/gaspery/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    10860 2023-04-09 21:20:17.000000 gaspery-0.2.1/src/gaspery/calculate_fi.py
--rw-r--r--   0 chris      (501) staff       (20)    16325 2023-05-29 19:30:41.000000 gaspery-0.2.1/src/gaspery/strategies.py
--rw-r--r--   0 chris      (501) staff       (20)     1345 2023-04-09 21:21:27.000000 gaspery-0.2.1/src/gaspery/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.784462 gaspery-0.2.1/src/gaspery.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     4226 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      280 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-01 17:42:17.185809 gaspery-0.2.2/
+-rw-r--r--   0 chris      (501) staff       (20)     1075 2023-04-08 21:45:04.000000 gaspery-0.2.2/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     4226 2023-06-01 17:42:17.185151 gaspery-0.2.2/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     3661 2023-04-08 21:45:04.000000 gaspery-0.2.2/README.md
+-rw-r--r--   0 chris      (501) staff       (20)      600 2023-06-01 17:41:59.000000 gaspery-0.2.2/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-06-01 17:42:17.186026 gaspery-0.2.2/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      433 2023-06-01 17:41:51.000000 gaspery-0.2.2/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-01 17:42:17.177414 gaspery-0.2.2/src/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-01 17:42:17.181878 gaspery-0.2.2/src/gaspery/
+-rw-r--r--   0 chris      (501) staff       (20)      307 2023-04-08 21:45:05.000000 gaspery-0.2.2/src/gaspery/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    10860 2023-04-09 21:20:17.000000 gaspery-0.2.2/src/gaspery/calculate_fi.py
+-rw-r--r--   0 chris      (501) staff       (20)    16482 2023-06-01 17:38:18.000000 gaspery-0.2.2/src/gaspery/strategies.py
+-rw-r--r--   0 chris      (501) staff       (20)     1345 2023-04-09 21:21:27.000000 gaspery-0.2.2/src/gaspery/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-01 17:42:17.184315 gaspery-0.2.2/src/gaspery.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     4226 2023-06-01 17:42:17.000000 gaspery-0.2.2/src/gaspery.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      280 2023-06-01 17:42:17.000000 gaspery-0.2.2/src/gaspery.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-01 17:42:17.000000 gaspery-0.2.2/src/gaspery.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)        8 2023-06-01 17:42:17.000000 gaspery-0.2.2/src/gaspery.egg-info/top_level.txt
```

### Comparing `gaspery-0.2.1/LICENSE` & `gaspery-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gaspery-0.2.1/PKG-INFO` & `gaspery-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaspery
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fisher Information-based radial velocity observation scheduling
 Author: Chris Lam
 Author-email: Christopher Lam <c.lam@ufl.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/cl3425/gaspery
 Project-URL: Bug Tracker, https://github.com/cl3425/gaspery/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaspery-0.2.1/README.md` & `gaspery-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gaspery-0.2.1/pyproject.toml` & `gaspery-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaspery"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Christopher Lam", email="c.lam@ufl.edu" },
 ]
 description = "Fisher Information-based radial velocity observation scheduling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gaspery-0.2.1/src/gaspery/calculate_fi.py` & `gaspery-0.2.2/src/gaspery/calculate_fi.py`

 * *Files identical despite different names*

### Comparing `gaspery-0.2.1/src/gaspery/strategies.py` & `gaspery-0.2.2/src/gaspery/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,16 @@
                                 add = False
 
                         if add == True:
                             if len(strat) < n_obs:
                                 strat.append(curr)
 
                     elif len(offs) == 0:
-                        strat.append(curr)
+                        if len(strat) < n_obs:
+                            strat.append(curr)
 
                     curr += 1
 
                 # off block
                 curr += off
 
         # if we observe twice a day
@@ -412,17 +413,19 @@
                             if len(strat) < n_obs:
                                 strat.append(curr)
                                 
                         # cycle back to same time of night the next day
                         curr += (24-hours)/24
 
                     elif len(offs) == 0:
-                        strat.append(curr)
-                        curr += (24-hours)/24
-                        strat.append(curr)
+                        if len(strat) < n_obs:
+                            strat.append(curr)
+                        if len(strat) < n_obs:
+                            curr += (24-hours)/24
+                            strat.append(curr)
                         
                 # off block
                 curr += off
         
         return np.array(strat)
```

### Comparing `gaspery-0.2.1/src/gaspery/utils.py` & `gaspery-0.2.2/src/gaspery/utils.py`

 * *Files identical despite different names*

### Comparing `gaspery-0.2.1/src/gaspery.egg-info/PKG-INFO` & `gaspery-0.2.2/src/gaspery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaspery
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fisher Information-based radial velocity observation scheduling
 Author: Chris Lam
 Author-email: Christopher Lam <c.lam@ufl.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/cl3425/gaspery
 Project-URL: Bug Tracker, https://github.com/cl3425/gaspery/issues
 Classifier: Programming Language :: Python :: 3
```

