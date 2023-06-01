# Comparing `tmp/django-vectortiles-1.0.0b2.tar.gz` & `tmp/django-vectortiles-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-vectortiles-1.0.0b2.tar", last modified: Wed May 24 08:38:55 2023, max compression
+gzip compressed data, was "dist/django-vectortiles-1.0.0b3.tar", last modified: Thu Jun  1 14:56:14 2023, max compression
```

## Comparing `django-vectortiles-1.0.0b2.tar` & `django-vectortiles-1.0.0b3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/django_vectortiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/VERSION.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/backends/postgis/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/postgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/postgis/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/backends/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/backends/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:55.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/rest_framework/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 08:38:47.000000 django-vectortiles-1.0.0b2/vectortiles/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/django_vectortiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/django_vectortiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/django_vectortiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/django_vectortiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/django_vectortiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/django_vectortiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/vectortiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/VERSION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/vectortiles/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/vectortiles/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/backends/postgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/backends/postgis/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/vectortiles/backends/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/backends/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:14.000000 django-vectortiles-1.0.0b3/vectortiles/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/rest_framework/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-01 14:56:11.000000 django-vectortiles-1.0.0b3/vectortiles/views.py
```

### Comparing `django-vectortiles-1.0.0b2/LICENSE` & `django-vectortiles-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b2/PKG-INFO` & `django-vectortiles-1.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vectortiles
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Django vector tile generation
 Home-page: https://github.com/submarcos/django-vectortiles.git
 Author: Jean-Etienne Castagnede
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `django-vectortiles-1.0.0b2/README.md` & `django-vectortiles-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b2/django_vectortiles.egg-info/PKG-INFO` & `django-vectortiles-1.0.0b3/django_vectortiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vectortiles
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Django vector tile generation
 Home-page: https://github.com/submarcos/django-vectortiles.git
 Author: Jean-Etienne Castagnede
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `django-vectortiles-1.0.0b2/django_vectortiles.egg-info/SOURCES.txt` & `django-vectortiles-1.0.0b3/django_vectortiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b2/setup.py` & `django-vectortiles-1.0.0b3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     version=open(os.path.join(HERE, 'vectortiles', 'VERSION.md')).read().strip(),
     include_package_data=True,
     author="Jean-Etienne Castagnede",
     description='Django vector tile generation',
     long_description=README,
     description_content_type="text/markdown",
     long_description_content_type="text/markdown",
-    packages=find_packages(),
+    packages=find_packages(exclude=['*tests', 'test*']),
     url='https://github.com/submarcos/django-vectortiles.git',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
```

### Comparing `django-vectortiles-1.0.0b2/vectortiles/backends/__init__.py` & `django-vectortiles-1.0.0b3/vectortiles/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b2/vectortiles/backends/postgis/__init__.py` & `django-vectortiles-1.0.0b3/vectortiles/backends/postgis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib.gis.db.models.functions import Transform
-from django.db import connection
+from django.db import connections
 
 from vectortiles.backends import BaseVectorLayerMixin
 from vectortiles.backends.postgis.functions import AsMVTGeom, MakeEnvelope
 
 
 class VectorLayer(BaseVectorLayerMixin):
     def get_tile(self, x, y, z):
@@ -37,15 +37,15 @@
         limit = self.get_queryset_limit()
         if limit:
             features = features[:limit]
         # keep values to include in tile (extra included_fields + geometry)
         features = features.values(*fields)
         # generate MVT
         sql, params = features.query.sql_with_params()
-        with connection.cursor() as cursor:
+        with connections[features.db].cursor() as cursor:
             cursor.execute(
                 "SELECT ST_ASMVT(subquery.*, %s, %s, %s) FROM ({}) as subquery".format(
                     sql
                 ),
                 params=[
                     self.get_id(),
                     self.tile_extent,
```

### Comparing `django-vectortiles-1.0.0b2/vectortiles/backends/postgis/functions.py` & `django-vectortiles-1.0.0b3/vectortiles/backends/postgis/functions.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b2/vectortiles/backends/python/__init__.py` & `django-vectortiles-1.0.0b3/vectortiles/backends/python/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b2/vectortiles/mixins.py` & `django-vectortiles-1.0.0b3/vectortiles/mixins.py`

 * *Files identical despite different names*

### Comparing `django-vectortiles-1.0.0b2/vectortiles/views.py` & `django-vectortiles-1.0.0b3/vectortiles/views.py`

 * *Files identical despite different names*

