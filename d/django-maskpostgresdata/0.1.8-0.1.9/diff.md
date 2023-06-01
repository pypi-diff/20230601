# Comparing `tmp/django-maskpostgresdata-0.1.8.tar.gz` & `tmp/django-maskpostgresdata-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-maskpostgresdata-0.1.8.tar", last modified: Fri Aug 30 14:43:00 2019, max compression
+gzip compressed data, was "dist/django-maskpostgresdata-0.1.9.tar", last modified: Fri Oct  4 08:50:20 2019, max compression
```

## Comparing `django-maskpostgresdata-0.1.8.tar` & `django-maskpostgresdata-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/
--rw-r--r--   0 tomkins    (501) staff       (20)     2618 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/PKG-INFO
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/maskpostgresdata/
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/maskpostgresdata/management/
--rw-r--r--   0 tomkins    (501) staff       (20)        0 2019-08-13 10:47:54.000000 django-maskpostgresdata-0.1.8/maskpostgresdata/management/__init__.py
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/maskpostgresdata/management/commands/
--rw-r--r--   0 tomkins    (501) staff       (20)        0 2019-08-13 10:47:54.000000 django-maskpostgresdata-0.1.8/maskpostgresdata/management/commands/__init__.py
--rw-r--r--   0 tomkins    (501) staff       (20)     4241 2019-08-30 14:41:41.000000 django-maskpostgresdata-0.1.8/maskpostgresdata/management/commands/dump_masked_data.py
--rw-r--r--   0 tomkins    (501) staff       (20)       92 2019-08-28 22:56:39.000000 django-maskpostgresdata-0.1.8/maskpostgresdata/__init__.py
--rw-r--r--   0 tomkins    (501) staff       (20)       19 2019-08-13 10:47:54.000000 django-maskpostgresdata-0.1.8/MANIFEST.in
--rw-r--r--   0 tomkins    (501) staff       (20)     1792 2019-08-28 22:56:39.000000 django-maskpostgresdata-0.1.8/README.md
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/
--rw-r--r--   0 tomkins    (501) staff       (20)     2618 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/PKG-INFO
--rw-r--r--   0 tomkins    (501) staff       (20)        1 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/not-zip-safe
--rw-r--r--   0 tomkins    (501) staff       (20)      495 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/SOURCES.txt
--rw-r--r--   0 tomkins    (501) staff       (20)       21 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/requires.txt
--rw-r--r--   0 tomkins    (501) staff       (20)       17 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/top_level.txt
--rw-r--r--   0 tomkins    (501) staff       (20)        1 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/dependency_links.txt
--rw-r--r--   0 tomkins    (501) staff       (20)      630 2019-08-30 14:41:41.000000 django-maskpostgresdata-0.1.8/setup.py
--rw-r--r--   0 tomkins    (501) staff       (20)       79 2019-08-30 14:43:00.000000 django-maskpostgresdata-0.1.8/setup.cfg
+drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/
+-rw-r--r--   0 ikonitas   (501) staff       (20)     2618 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/PKG-INFO
+drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/
+drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/
+-rw-r--r--   0 ikonitas   (501) staff       (20)        0 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/__init__.py
+drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/commands/
+-rw-r--r--   0 ikonitas   (501) staff       (20)        0 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/commands/__init__.py
+-rw-r--r--   0 ikonitas   (501) staff       (20)     5074 2019-10-04 08:21:41.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/commands/dump_masked_data.py
+-rw-r--r--   0 ikonitas   (501) staff       (20)       92 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/__init__.py
+-rw-r--r--   0 ikonitas   (501) staff       (20)       19 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/MANIFEST.in
+-rw-r--r--   0 ikonitas   (501) staff       (20)     1792 2019-10-03 08:24:56.000000 django-maskpostgresdata-0.1.9/README.md
+drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/
+-rw-r--r--   0 ikonitas   (501) staff       (20)     2618 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/PKG-INFO
+-rw-r--r--   0 ikonitas   (501) staff       (20)        1 2019-10-03 08:19:49.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/not-zip-safe
+-rw-r--r--   0 ikonitas   (501) staff       (20)      495 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/SOURCES.txt
+-rw-r--r--   0 ikonitas   (501) staff       (20)       21 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/requires.txt
+-rw-r--r--   0 ikonitas   (501) staff       (20)       17 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/top_level.txt
+-rw-r--r--   0 ikonitas   (501) staff       (20)        1 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/dependency_links.txt
+-rw-r--r--   0 ikonitas   (501) staff       (20)      656 2019-10-04 08:44:05.000000 django-maskpostgresdata-0.1.9/setup.py
+-rw-r--r--   0 ikonitas   (501) staff       (20)       79 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/setup.cfg
```

### Comparing `django-maskpostgresdata-0.1.8/PKG-INFO` & `django-maskpostgresdata-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-maskpostgresdata
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates a pg_dumpish output which masks data without saving changes to the source database.
 Home-page: https://github.com/developersociety/django-maskpostgresdata
 Author: Developer Society
 Author-email: hello@dev.ngo
 License: BSD
 Description: Django Mask Postgres Data
         =========================
```

### Comparing `django-maskpostgresdata-0.1.8/README.md` & `django-maskpostgresdata-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django-maskpostgresdata-0.1.8/django_maskpostgresdata.egg-info/PKG-INFO` & `django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-maskpostgresdata
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates a pg_dumpish output which masks data without saving changes to the source database.
 Home-page: https://github.com/developersociety/django-maskpostgresdata
 Author: Developer Society
 Author-email: hello@dev.ngo
 License: BSD
 Description: Django Mask Postgres Data
         =========================
```

### Comparing `django-maskpostgresdata-0.1.8/setup.py` & `django-maskpostgresdata-0.1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='django-maskpostgresdata',
     packages=find_packages(),
-    version='0.1.8',
-    description='Creates a pg_dumpish output which masks data without saving changes to the source database.',
+    version='0.1.9',
+    description=(
+        'Creates a pg_dumpish output which masks data without saving changes to the source '
+        'database.'
+    ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/developersociety/django-maskpostgresdata',
     author='Developer Society',
     author_email='hello@dev.ngo',
     license='BSD',
     zip_safe=False,
-    install_requires = ['django>=1.8','psycopg2']
+    install_requires=['django>=1.8', 'psycopg2']
 )
```

