# Comparing `tmp/django-vite-2.1.0.tar.gz` & `tmp/django-vite-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vite-2.1.0.tar", last modified: Thu May 25 13:33:07 2023, max compression
+gzip compressed data, was "django-vite-2.1.1.tar", last modified: Thu Jun  1 18:18:44 2023, max compression
```

## Comparing `django-vite-2.1.0.tar` & `django-vite-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-25 13:32:52.000000 django-vite-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 13:32:52.000000 django-vite-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-25 13:33:07.659424 django-vite-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-05-25 13:32:52.000000 django-vite-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/django_vite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:52.000000 django-vite-2.1.0/django_vite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/django_vite/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:52.000000 django-vite-2.1.0/django_vite/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-25 13:32:52.000000 django-vite-2.1.0/django_vite/templatetags/django_vite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/django_vite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 13:32:52.000000 django-vite-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:33:07.659424 django-vite-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 13:32:52.000000 django-vite-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:18:44.063406 django-vite-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-01 18:18:33.000000 django-vite-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 18:18:33.000000 django-vite-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-01 18:18:44.063406 django-vite-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-01 18:18:33.000000 django-vite-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:18:44.063406 django-vite-2.1.1/django_vite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:18:33.000000 django-vite-2.1.1/django_vite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-01 18:18:33.000000 django-vite-2.1.1/django_vite/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:18:44.063406 django-vite-2.1.1/django_vite/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:18:33.000000 django-vite-2.1.1/django_vite/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-06-01 18:18:33.000000 django-vite-2.1.1/django_vite/templatetags/django_vite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:18:44.063406 django-vite-2.1.1/django_vite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-01 18:18:43.000000 django-vite-2.1.1/django_vite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-01 18:18:44.000000 django-vite-2.1.1/django_vite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:18:43.000000 django-vite-2.1.1/django_vite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 18:18:43.000000 django-vite-2.1.1/django_vite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 18:18:43.000000 django-vite-2.1.1/django_vite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 18:18:33.000000 django-vite-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:18:44.063406 django-vite-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-01 18:18:33.000000 django-vite-2.1.1/setup.py
```

### Comparing `django-vite-2.1.0/LICENSE` & `django-vite-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vite-2.1.0/PKG-INFO` & `django-vite-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 2.1.0
+Version: 2.1.1
 Summary: Integration of ViteJS in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires: Django (>=1.11)
 Description-Content-Type: text/markdown
```

### Comparing `django-vite-2.1.0/README.md` & `django-vite-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-vite-2.1.0/django_vite/templatetags/django_vite.py` & `django-vite-2.1.1/django_vite/templatetags/django_vite.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,18 +462,14 @@
             return staticfiles_storage.url(
                 urljoin(DJANGO_VITE_STATIC_URL_PREFIX, path)
             )
         else:
             return urljoin(DJANGO_VITE_STATIC_URL_PREFIX, path)
 
 
-# Make Loader instance at startup to prevent threading problems
-DjangoViteAssetLoader.instance()
-
-
 @register.simple_tag
 @mark_safe
 def vite_hmr_client(**kwargs: Dict[str, str]) -> str:
     """
     Generates the script tag for the Vite WS client for HMR.
     Only used in development, in production this method returns
     an empty string.
```

### Comparing `django-vite-2.1.0/django_vite.egg-info/PKG-INFO` & `django-vite-2.1.1/django_vite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 2.1.0
+Version: 2.1.1
 Summary: Integration of ViteJS in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires: Django (>=1.11)
 Description-Content-Type: text/markdown
```

### Comparing `django-vite-2.1.0/setup.py` & `django-vite-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     README = f.read()
 
 
 setup(
     name="django-vite",
-    version="2.1.0",
+    version="2.1.1",
     description="Integration of ViteJS in a Django project.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="MrBin99",
     url="https://github.com/MrBin99/django-vite",
     license="Apache License, Version 2.0",
     include_package_data=True,
```

