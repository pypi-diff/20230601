# Comparing `tmp/mltkit-0.3.0.tar.gz` & `tmp/mltkit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltkit-0.3.0.tar", last modified: Fri Feb 17 23:39:54 2023, max compression
+gzip compressed data, was "mltkit-0.3.1.tar", last modified: Thu Jun  1 03:44:47 2023, max compression
```

## Comparing `mltkit-0.3.0.tar` & `mltkit-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-02-17 23:39:54.089884 mltkit-0.3.0/
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      375 2023-02-17 23:39:54.089676 mltkit-0.3.0/PKG-INFO
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-02-17 18:41:38.000000 mltkit-0.3.0/README.md
-drwxr-xr-x   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-02-17 23:39:54.087123 mltkit-0.3.0/mltkit/
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)     8066 2023-02-17 18:41:38.000000 mltkit-0.3.0/mltkit/Display.py
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)    17964 2023-02-17 18:41:38.000000 mltkit-0.3.0/mltkit/JobManager.py
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)     3216 2023-02-17 23:22:04.000000 mltkit-0.3.0/mltkit/LossBuffer.py
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      260 2023-02-17 23:22:40.000000 mltkit-0.3.0/mltkit/__init__.py
-drwxr-xr-x   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-02-17 23:39:54.089333 mltkit-0.3.0/mltkit.egg-info/
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      375 2023-02-17 23:39:53.000000 mltkit-0.3.0/mltkit.egg-info/PKG-INFO
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      217 2023-02-17 23:39:53.000000 mltkit-0.3.0/mltkit.egg-info/SOURCES.txt
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)        1 2023-02-17 23:39:53.000000 mltkit-0.3.0/mltkit.egg-info/dependency_links.txt
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)        7 2023-02-17 23:39:53.000000 mltkit-0.3.0/mltkit.egg-info/top_level.txt
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)       38 2023-02-17 23:39:54.089942 mltkit-0.3.0/setup.cfg
--rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      770 2023-02-17 18:41:38.000000 mltkit-0.3.0/setup.py
+drwxr-xr-x   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-06-01 03:44:47.402197 mltkit-0.3.1/
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)     1064 2023-02-17 23:43:47.000000 mltkit-0.3.1/LICENSE.rst
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      429 2023-06-01 03:44:47.402287 mltkit-0.3.1/PKG-INFO
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-02-17 18:41:38.000000 mltkit-0.3.1/README.md
+drwxr-xr-x   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-06-01 03:44:47.400307 mltkit-0.3.1/mltkit/
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)     8066 2023-02-17 18:41:38.000000 mltkit-0.3.1/mltkit/Display.py
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)    17964 2023-02-17 18:41:38.000000 mltkit-0.3.1/mltkit/JobManager.py
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)     3228 2023-06-01 03:43:50.000000 mltkit-0.3.1/mltkit/LossBuffer.py
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      260 2023-06-01 03:36:01.000000 mltkit-0.3.1/mltkit/__init__.py
+drwxr-xr-x   0 mlockyer  (6903) AM\nis.vasg   (431)        0 2023-06-01 03:44:47.401962 mltkit-0.3.1/mltkit.egg-info/
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      429 2023-06-01 03:44:46.000000 mltkit-0.3.1/mltkit.egg-info/PKG-INFO
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      239 2023-06-01 03:44:46.000000 mltkit-0.3.1/mltkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)        1 2023-06-01 03:44:46.000000 mltkit-0.3.1/mltkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)        7 2023-06-01 03:44:46.000000 mltkit-0.3.1/mltkit.egg-info/top_level.txt
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      107 2023-06-01 03:44:47.402672 mltkit-0.3.1/setup.cfg
+-rw-r--r--   0 mlockyer  (6903) AM\nis.vasg   (431)      770 2023-02-17 18:41:38.000000 mltkit-0.3.1/setup.py
```

### Comparing `mltkit-0.3.0/mltkit/Display.py` & `mltkit-0.3.1/mltkit/Display.py`

 * *Files identical despite different names*

### Comparing `mltkit-0.3.0/mltkit/JobManager.py` & `mltkit-0.3.1/mltkit/JobManager.py`

 * *Files identical despite different names*

### Comparing `mltkit-0.3.0/mltkit/LossBuffer.py` & `mltkit-0.3.1/mltkit/LossBuffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-
 from statistics import mean
 from collections import OrderedDict
-from typing import Dict, List, Optional, OrderedDict as T_OrderedDict
+from typing import Dict, List, Optional, OrderedDict as T_OrderedDict, Union
 
 _T_Values = List[float]
 _T_BufferDict = T_OrderedDict[str, _T_Values]
-_T_BufferArg = T_OrderedDict[str, float] | Dict[str, float]
+_T_BufferArg = Union[T_OrderedDict[str, float], Dict[str, float]]
 
 
 class LossBuffer(object):
     __slots__ = ['_buffers', '_mean_cache']
     _buffers: Dict[str, _T_BufferDict]
     _mean_cache: Dict[str, Dict[str, float]]
```

### Comparing `mltkit-0.3.0/setup.py` & `mltkit-0.3.1/setup.py`

 * *Files identical despite different names*

