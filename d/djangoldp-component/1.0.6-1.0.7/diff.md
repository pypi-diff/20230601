# Comparing `tmp/djangoldp_component-1.0.6.tar.gz` & `tmp/djangoldp_component-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_component-1.0.6.tar", last modified: Wed May 24 10:29:13 2023, max compression
+gzip compressed data, was "dist/djangoldp_component-1.0.7.tar", last modified: Thu Jun  1 15:42:55 2023, max compression
```

## Comparing `djangoldp_component-1.0.6.tar` & `djangoldp_component-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      599 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component/
--rw-rw-rw-   0 root         (0) root         (0)     9713 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-24 10:29:11.000000 djangoldp_component-1.0.6/djangoldp_component/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:29:13.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    12897 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/0003_component_auto_menu.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-24 10:28:53.000000 djangoldp_component-1.0.6/djangoldp_component/migrations/0002_delete_dependency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      599 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component/
+-rw-rw-rw-   0 root         (0) root         (0)     9713 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-01 15:42:53.000000 djangoldp_component-1.0.7/djangoldp_component/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    12897 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/0003_component_auto_menu.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/0002_delete_dependency.py
```

### Comparing `djangoldp_component-1.0.6/README.md` & `djangoldp_component-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.6/djangoldp_component.egg-info/SOURCES.txt` & `djangoldp_component-1.0.7/djangoldp_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.6/setup.cfg` & `djangoldp_component-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.6/djangoldp_component/models.py` & `djangoldp_component-1.0.7/djangoldp_component/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.db.models.signals import pre_save
 from django.dispatch import receiver
 from django.utils.text import slugify
 from django.utils.translation import ugettext_lazy as _
@@ -264,15 +265,15 @@
         ):
             if (
                 sender.objects.local()
                 .filter(slug=slugify(instance.friendly_name))
                 .count()
                 > 0
             ):
-                raise ValidationError(sender.__name__  + str(_(" must be unique")))
+                raise ValidationError(sender.__name__ + str(_(" must be unique")))
             setattr(
                 instance, Model.slug_field(instance), slugify(instance.friendly_name)
             )
             setattr(instance, "urlid", "")
     else:
         # Is a distant object, generate a random slug
         setattr(instance, Model.slug_field(instance), uuid.uuid4().hex.upper()[0:8])
```

### Comparing `djangoldp_component-1.0.6/djangoldp_component/admin.py` & `djangoldp_component-1.0.7/djangoldp_component/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
-from .models import (
-    Component,
-    Parameter,
-    ComponentScriptTag,
-    Package,
-    ServerParameter,
-)
+
+from .models import Component, ComponentScriptTag, Package, Parameter, ServerParameter
 
 
 class EmptyAdmin(admin.ModelAdmin):
     def get_model_perms(self, request):
         return {}
```

### Comparing `djangoldp_component-1.0.6/djangoldp_component/migrations/0001_initial.py` & `djangoldp_component-1.0.7/djangoldp_component/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.6/djangoldp_component/migrations/0003_component_auto_menu.py` & `djangoldp_component-1.0.7/djangoldp_component/migrations/0003_component_auto_menu.py`

 * *Files identical despite different names*

