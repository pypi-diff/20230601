# Comparing `tmp/django-admin-multi-select-filter-1.0.0.tar.gz` & `tmp/django-admin-multi-select-filter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-multi-select-filter-1.0.0.tar", last modified: Sun Oct 16 13:53:33 2022, max compression
+gzip compressed data, was "django-admin-multi-select-filter-1.1.0.tar", last modified: Thu Jun  1 08:30:55 2023, max compression
```

## Comparing `django-admin-multi-select-filter-1.0.0.tar` & `django-admin-multi-select-filter-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 13:53:33.715756 django-admin-multi-select-filter-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-16 13:53:19.000000 django-admin-multi-select-filter-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-10-16 13:53:33.715756 django-admin-multi-select-filter-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-10-16 13:53:19.000000 django-admin-multi-select-filter-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-10-16 13:53:19.000000 django-admin-multi-select-filter-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-16 13:53:33.715756 django-admin-multi-select-filter-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 13:53:33.711756 django-admin-multi-select-filter-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 13:53:33.711756 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-16 13:53:19.000000 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3004 2022-10-16 13:53:19.000000 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 13:53:33.715756 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-10-16 13:53:33.000000 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-16 13:53:33.000000 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-16 13:53:33.000000 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-16 13:53:33.000000 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-16 13:53:33.000000 django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:30:55.642694 django-admin-multi-select-filter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 08:30:38.000000 django-admin-multi-select-filter-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-01 08:30:55.642694 django-admin-multi-select-filter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-01 08:30:38.000000 django-admin-multi-select-filter-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 08:30:38.000000 django-admin-multi-select-filter-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 08:30:55.642694 django-admin-multi-select-filter-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:30:55.642694 django-admin-multi-select-filter-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:30:55.642694 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:30:38.000000 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-01 08:30:38.000000 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:30:55.642694 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-01 08:30:55.000000 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 08:30:55.000000 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:30:55.000000 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 08:30:55.000000 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 08:30:55.000000 django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter.egg-info/top_level.txt
```

### Comparing `django-admin-multi-select-filter-1.0.0/LICENSE` & `django-admin-multi-select-filter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-multi-select-filter-1.0.0/PKG-INFO` & `django-admin-multi-select-filter-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-multi-select-filter
-Version: 1.0.0
+Version: 1.1.0
 Summary: Django admin filter for multiple select
 Author-email: Job Doesburg <job.doesburg@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Job Doesburg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-admin-multi-select-filter-1.0.0/README.md` & `django-admin-multi-select-filter-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-multi-select-filter-1.0.0/pyproject.toml` & `django-admin-multi-select-filter-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-admin-multi-select-filter"
-version = "1.0.0"
+version = "1.1.0"
 description = "Django admin filter for multiple select"
 readme = "README.md"
 authors = [{ name = "Job Doesburg", email = "job.doesburg@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter/filters.py` & `django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,21 @@
         self.lookup_val_isnull = self.used_parameters.get(self.lookup_kwarg_isnull)
 
         self.empty_value_display = model_admin.get_empty_value_display()
         parent_model, reverse_path = reverse_field_path(model, field_path)
         # Obey parent ModelAdmin queryset when deciding which options to show
         if model == parent_model:
             queryset = model_admin.get_queryset(request)
+            self.lookup_choices = (
+                queryset.distinct().order_by(field.name).values_list(field.name, flat=True)
+            )
         else:
             queryset = parent_model._default_manager.all()
-        self.lookup_choices = (
-            queryset.distinct().order_by(field.name).values_list(field.name, flat=True)
-        )
-
+            self.lookup_choices = queryset.distinct()
+            
     def expected_parameters(self):
         return [self.lookup_kwarg, self.lookup_kwarg_isnull]
 
     def choices(self, changelist):
         yield {
             "selected": not self.lookup_val and self.lookup_val_isnull is None,
             "query_string": changelist.get_query_string(
```

### Comparing `django-admin-multi-select-filter-1.0.0/src/django_admin_multi_select_filter.egg-info/PKG-INFO` & `django-admin-multi-select-filter-1.1.0/src/django_admin_multi_select_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-multi-select-filter
-Version: 1.0.0
+Version: 1.1.0
 Summary: Django admin filter for multiple select
 Author-email: Job Doesburg <job.doesburg@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Job Doesburg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

