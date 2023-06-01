# Comparing `tmp/django-admin-multi-select-filter-1.2.0.tar.gz` & `tmp/django-admin-multi-select-filter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-multi-select-filter-1.2.0.tar", last modified: Thu Jun  1 09:21:49 2023, max compression
+gzip compressed data, was "django-admin-multi-select-filter-1.2.1.tar", last modified: Thu Jun  1 09:24:05 2023, max compression
```

## Comparing `django-admin-multi-select-filter-1.2.0.tar` & `django-admin-multi-select-filter-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:21:49.963283 django-admin-multi-select-filter-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 09:21:35.000000 django-admin-multi-select-filter-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-01 09:21:49.963283 django-admin-multi-select-filter-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-01 09:21:35.000000 django-admin-multi-select-filter-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 09:21:35.000000 django-admin-multi-select-filter-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:21:49.963283 django-admin-multi-select-filter-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:21:49.963283 django-admin-multi-select-filter-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:21:49.963283 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:21:35.000000 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-01 09:21:35.000000 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:21:49.963283 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-01 09:21:49.000000 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 09:21:49.000000 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:21:49.000000 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:21:49.000000 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 09:21:49.000000 django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:24:05.399124 django-admin-multi-select-filter-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 09:23:53.000000 django-admin-multi-select-filter-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-01 09:24:05.399124 django-admin-multi-select-filter-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-01 09:23:53.000000 django-admin-multi-select-filter-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 09:23:53.000000 django-admin-multi-select-filter-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:24:05.399124 django-admin-multi-select-filter-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:24:05.395124 django-admin-multi-select-filter-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:24:05.399124 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:23:53.000000 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-01 09:23:53.000000 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:24:05.399124 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-01 09:24:05.000000 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 09:24:05.000000 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:24:05.000000 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 09:24:05.000000 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 09:24:05.000000 django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter.egg-info/top_level.txt
```

### Comparing `django-admin-multi-select-filter-1.2.0/LICENSE` & `django-admin-multi-select-filter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-multi-select-filter-1.2.0/PKG-INFO` & `django-admin-multi-select-filter-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-multi-select-filter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Django admin filter for multiple select
 Author-email: Job Doesburg <job.doesburg@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Job Doesburg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 Django admin multi-select filter is a Django app that allows you to add a multi-select filter to the Django admin.
 
 ## Installation
 1. Install using pip:
     ```bash
     pip install django-admin-multi-select-filter
     ```
-2. Use the `MultiSelectFilter` in your admin classes (you do **not** need to add the app to `INSTALLED_APPS`):
+2. Use the `MultiSelectFilter` (or `MultiSelectRelatedFieldListFilter` when using on related fields) in your admin classes (you do **not** need to add the app to `INSTALLED_APPS`):
     ```python
     from django.contrib import admin
     from django_admin_multi_select_filter.filters import MultiSelectFieldListFilter
 
     class MyModelAdmin(admin.ModelAdmin):
         list_filter = (
             ...
```

### Comparing `django-admin-multi-select-filter-1.2.0/README.md` & `django-admin-multi-select-filter-1.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Django admin multi-select filter is a Django app that allows you to add a multi-select filter to the Django admin.
 
 ## Installation
 1. Install using pip:
     ```bash
     pip install django-admin-multi-select-filter
     ```
-2. Use the `MultiSelectFilter` in your admin classes (you do **not** need to add the app to `INSTALLED_APPS`):
+2. Use the `MultiSelectFilter` (or `MultiSelectRelatedFieldListFilter` when using on related fields) in your admin classes (you do **not** need to add the app to `INSTALLED_APPS`):
     ```python
     from django.contrib import admin
     from django_admin_multi_select_filter.filters import MultiSelectFieldListFilter
 
     class MyModelAdmin(admin.ModelAdmin):
         list_filter = (
             ...
```

### Comparing `django-admin-multi-select-filter-1.2.0/pyproject.toml` & `django-admin-multi-select-filter-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-admin-multi-select-filter"
-version = "1.2.0"
+version = "1.2.1"
 description = "Django admin filter for multiple select"
 readme = "README.md"
 authors = [{ name = "Job Doesburg", email = "job.doesburg@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter/filters.py` & `django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter/filters.py`

 * *Files identical despite different names*

### Comparing `django-admin-multi-select-filter-1.2.0/src/django_admin_multi_select_filter.egg-info/PKG-INFO` & `django-admin-multi-select-filter-1.2.1/src/django_admin_multi_select_filter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-multi-select-filter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Django admin filter for multiple select
 Author-email: Job Doesburg <job.doesburg@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Job Doesburg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 Django admin multi-select filter is a Django app that allows you to add a multi-select filter to the Django admin.
 
 ## Installation
 1. Install using pip:
     ```bash
     pip install django-admin-multi-select-filter
     ```
-2. Use the `MultiSelectFilter` in your admin classes (you do **not** need to add the app to `INSTALLED_APPS`):
+2. Use the `MultiSelectFilter` (or `MultiSelectRelatedFieldListFilter` when using on related fields) in your admin classes (you do **not** need to add the app to `INSTALLED_APPS`):
     ```python
     from django.contrib import admin
     from django_admin_multi_select_filter.filters import MultiSelectFieldListFilter
 
     class MyModelAdmin(admin.ModelAdmin):
         list_filter = (
             ...
```

