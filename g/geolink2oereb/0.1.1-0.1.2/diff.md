# Comparing `tmp/geolink2oereb-0.1.1.tar.gz` & `tmp/geolink2oereb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.1.1.tar", last modified: Wed May 31 07:00:48 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.2.tar", last modified: Thu Jun  1 14:22:15 2023, max compression
```

## Comparing `geolink2oereb-0.1.1.tar` & `geolink2oereb-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.138275 geolink2oereb-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 07:00:48.138275 geolink2oereb-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 07:00:48.138275 geolink2oereb-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.134275 geolink2oereb-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.134275 geolink2oereb-0.1.1/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.134275 geolink2oereb-0.1.1/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.134275 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.134275 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.138275 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.138275 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-31 07:00:10.000000 geolink2oereb-0.1.1/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:00:48.134275 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 07:00:48.000000 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-31 07:00:48.000000 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:00:48.000000 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 07:00:48.000000 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:00:48.000000 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 07:00:48.000000 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 07:00:48.000000 geolink2oereb-0.1.1/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.940505 geolink2oereb-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.940505 geolink2oereb-0.1.2/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-01 14:21:38.000000 geolink2oereb-0.1.2/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:15.944505 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 14:22:15.000000 geolink2oereb-0.1.2/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.1.1/LICENSE` & `geolink2oereb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.1/PKG-INFO` & `geolink2oereb-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.1/README.md` & `geolink2oereb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.1/setup.py` & `geolink2oereb-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.1.1',
+    version='0.1.2',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `geolink2oereb-0.1.1/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.2/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.1/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.2/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from pyramid_oereb.core.records.law_status import LawStatusRecord
 from pyramid_oereb.core.config import Config
-from src.geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes import (
+from geolink2oereb.lib.interfaces.oerebkrmtrsfr.v2_0.classes import (
     OeREBKRM_V2_0_DokumentTyp,
 )
 from pyramid_oereb.core.records.document_types import DocumentTypeRecord
 from pyramid_oereb.contrib.data_sources.oereblex.sources.document import OEREBlexSource
 from pyramid_oereb.core.views.webservice import Parameter
 from pyramid.path import DottedNameResolver
```

### Comparing `geolink2oereb-0.1.1/src/geolink2oereb/transform.py` & `geolink2oereb-0.1.2/src/geolink2oereb/transform.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.1.1/src/geolink2oereb.egg-info/PKG-INFO` & `geolink2oereb-0.1.2/src/geolink2oereb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolink2oereb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities
 Home-page: https://github.com/openoereb/geolink2oereb
 Author: Clemens Rudert
 Author-email: rudert-geoinformatik@posteo.ch
 License: BSD
 Keywords: oereb lex geolink formatter html OeREBKRMtrsfr_V2_0
 Platform: UNKNOWN
```

### Comparing `geolink2oereb-0.1.1/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.2/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

