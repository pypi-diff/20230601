# Comparing `tmp/ReliabilityDiagram-0.0.2.tar.gz` & `tmp/ReliabilityDiagram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ReliabilityDiagram-0.0.2.tar", last modified: Fri Oct 21 08:43:25 2022, max compression
+gzip compressed data, was "dist/ReliabilityDiagram-0.0.3.tar", last modified: Thu Jun  1 19:07:55 2023, max compression
```

## Comparing `ReliabilityDiagram-0.0.2.tar` & `ReliabilityDiagram-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ngoutham  (1001) ngoutham  (1001)        0 2022-10-21 08:43:25.000000 ReliabilityDiagram-0.0.2/
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    11364 2022-10-21 07:44:05.000000 ReliabilityDiagram-0.0.2/LICENSE
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    13696 2022-10-21 08:43:25.000000 ReliabilityDiagram-0.0.2/PKG-INFO
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    12853 2022-10-21 08:41:47.000000 ReliabilityDiagram-0.0.2/README.md
-drwxrwxr-x   0 ngoutham  (1001) ngoutham  (1001)        0 2022-10-21 08:43:25.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram/
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    11125 2022-10-21 08:09:57.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram/ReliabilityDiagram.py
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       51 2022-10-21 07:56:02.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram/__init__.py
-drwxrwxr-x   0 ngoutham  (1001) ngoutham  (1001)        0 2022-10-21 08:43:25.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram.egg-info/
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    13696 2022-10-21 08:43:24.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram.egg-info/PKG-INFO
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)      317 2022-10-21 08:43:24.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram.egg-info/SOURCES.txt
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)        1 2022-10-21 08:43:24.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram.egg-info/dependency_links.txt
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       18 2022-10-21 08:43:24.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram.egg-info/requires.txt
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       19 2022-10-21 08:43:24.000000 ReliabilityDiagram-0.0.2/ReliabilityDiagram.egg-info/top_level.txt
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       79 2022-10-21 08:43:25.000000 ReliabilityDiagram-0.0.2/setup.cfg
--rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)     1370 2022-10-21 08:42:07.000000 ReliabilityDiagram-0.0.2/setup.py
+drwxrwxr-x   0 ngoutham  (1001) ngoutham  (1001)        0 2023-06-01 19:07:55.000000 ReliabilityDiagram-0.0.3/
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    11364 2022-10-21 07:44:05.000000 ReliabilityDiagram-0.0.3/LICENSE
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    13696 2023-06-01 19:07:55.000000 ReliabilityDiagram-0.0.3/PKG-INFO
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    12853 2022-10-21 08:41:47.000000 ReliabilityDiagram-0.0.3/README.md
+drwxrwxr-x   0 ngoutham  (1001) ngoutham  (1001)        0 2023-06-01 19:07:55.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram/
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    11179 2023-06-01 19:04:21.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram/ReliabilityDiagram.py
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       51 2022-10-21 07:56:02.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram/__init__.py
+drwxrwxr-x   0 ngoutham  (1001) ngoutham  (1001)        0 2023-06-01 19:07:55.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram.egg-info/
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)    13696 2023-06-01 19:07:54.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram.egg-info/PKG-INFO
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)      317 2023-06-01 19:07:54.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram.egg-info/SOURCES.txt
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)        1 2023-06-01 19:07:54.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram.egg-info/dependency_links.txt
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       18 2023-06-01 19:07:54.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram.egg-info/requires.txt
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       19 2023-06-01 19:07:54.000000 ReliabilityDiagram-0.0.3/ReliabilityDiagram.egg-info/top_level.txt
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)       79 2023-06-01 19:07:55.000000 ReliabilityDiagram-0.0.3/setup.cfg
+-rw-rw-r--   0 ngoutham  (1001) ngoutham  (1001)     1370 2023-06-01 19:05:06.000000 ReliabilityDiagram-0.0.3/setup.py
```

### Comparing `ReliabilityDiagram-0.0.2/LICENSE` & `ReliabilityDiagram-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ReliabilityDiagram-0.0.2/PKG-INFO` & `ReliabilityDiagram-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReliabilityDiagram
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package which provides the contingency table and all the other ingredients required to plot a reliability diagram. A reliability diagram is a diagnostic plot which helps to understand the joint distribution of forecasts and observations for probabilistic forecasts of a dichotomous event (i.e., yes/no event).
 Home-page: https://github.com/clecoz/ReliabilityDiagram
 Author: Naveen Goutham, Camille Le Coz
 Author-email: naveen.goutham@outlook.com, camille.lecoz@laposte.net
 License: Apache License 2.0
 Keywords: reliability table,contingency table,reliability diagram,attributes diagram,reliability,resolution,forecast attributes,brier score,ensemble forecast,forecast,climatology,python
 Platform: UNKNOWN
```

### Comparing `ReliabilityDiagram-0.0.2/README.md` & `ReliabilityDiagram-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ReliabilityDiagram-0.0.2/ReliabilityDiagram/ReliabilityDiagram.py` & `ReliabilityDiagram-0.0.3/ReliabilityDiagram/ReliabilityDiagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,17 +225,17 @@
         Returns:
             Brier score: float
             Reliability: float
             Resolution: float
         '''
         c_table = self.contingency_table()
         #
-        yi = self.bins  # forecast probability
+        yi = self.bins + (self.bins[1]-self.bins[0])/2  # forecast probability (middle of the bins)
         oi = self.observed_frequency()    # observed frequency
         wti = np.sum(c_table,axis=1)/np.sum(c_table)    # weights=number of forecasts yi / total number of forecasts
         om = np.sum(c_table[:,0])/np.sum(c_table)   # overall (unconditional) relative frequency
         o_bar = np.repeat(om,len(self.bins))
         #
         rel = np.nansum(((yi - oi)**2)*wti)    # reliability component of the Brier score
         res = np.nansum(((oi - o_bar)**2)*wti) # resolution component of the Brier score
         bs = rel - res + om*(1-om)             # brier score
-        return bs, rel, res
+        return bs, rel, res
```

### Comparing `ReliabilityDiagram-0.0.2/ReliabilityDiagram.egg-info/PKG-INFO` & `ReliabilityDiagram-0.0.3/ReliabilityDiagram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReliabilityDiagram
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package which provides the contingency table and all the other ingredients required to plot a reliability diagram. A reliability diagram is a diagnostic plot which helps to understand the joint distribution of forecasts and observations for probabilistic forecasts of a dichotomous event (i.e., yes/no event).
 Home-page: https://github.com/clecoz/ReliabilityDiagram
 Author: Naveen Goutham, Camille Le Coz
 Author-email: naveen.goutham@outlook.com, camille.lecoz@laposte.net
 License: Apache License 2.0
 Keywords: reliability table,contingency table,reliability diagram,attributes diagram,reliability,resolution,forecast attributes,brier score,ensemble forecast,forecast,climatology,python
 Platform: UNKNOWN
```

### Comparing `ReliabilityDiagram-0.0.2/setup.py` & `ReliabilityDiagram-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 PACKAGE_NAME = 'ReliabilityDiagram'
 AUTHOR = 'Naveen Goutham, Camille Le Coz'
 AUTHOR_EMAIL = 'naveen.goutham@outlook.com, camille.lecoz@laposte.net'
 URL = 'https://github.com/clecoz/ReliabilityDiagram'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'A package which provides the contingency table and all the other ingredients required to plot a reliability diagram. A reliability diagram is a diagnostic plot which helps to understand the joint distribution of forecasts and observations for probabilistic forecasts of a dichotomous event (i.e., yes/no event).'
```

