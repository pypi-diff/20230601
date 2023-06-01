# Comparing `tmp/django-admin-thumbnails-0.2.7.tar.gz` & `tmp/django-admin-thumbnails-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-admin-thumbnails-0.2.7.tar", last modified: Wed Apr 19 12:00:30 2023, max compression
+gzip compressed data, was "dist/django-admin-thumbnails-0.2.8.tar", last modified: Thu Jun  1 14:50:13 2023, max compression
```

## Comparing `django-admin-thumbnails-0.2.7.tar` & `django-admin-thumbnails-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10127 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/PKG-INFO
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10127 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-07 12:40:08.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/not-zip-safe
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      404 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       93 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       17 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       58 2019-04-07 10:23:12.000000 django-admin-thumbnails-0.2.7/MANIFEST.in
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4739 2023-04-19 11:27:10.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      248 2019-10-10 09:50:06.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/utils.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1300 2019-04-16 19:16:08.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/settings.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7443 2023-04-19 11:54:42.000000 django-admin-thumbnails-0.2.7/README.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2196 2023-04-19 11:58:42.000000 django-admin-thumbnails-0.2.7/setup.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       79 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/setup.cfg
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10244 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/PKG-INFO
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10244 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-07 12:40:08.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/not-zip-safe
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      404 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       93 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       17 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       58 2019-04-07 10:23:12.000000 django-admin-thumbnails-0.2.8/MANIFEST.in
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4806 2023-06-01 14:48:48.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      248 2019-10-10 09:50:06.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1300 2019-04-16 19:16:08.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/settings.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7443 2023-04-19 11:54:42.000000 django-admin-thumbnails-0.2.8/README.md
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2298 2023-06-01 14:47:54.000000 django-admin-thumbnails-0.2.8/setup.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       79 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/setup.cfg
```

### Comparing `django-admin-thumbnails-0.2.7/PKG-INFO` & `django-admin-thumbnails-0.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-thumbnails
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Django app for DRY thumbnails in admin list views and forms.
 Home-page: http://github.com/BigglesZX/django-admin-thumbnails
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Description: # django-admin-thumbnails
         
@@ -200,10 +200,13 @@
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=2.6,<4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/PKG-INFO` & `django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-thumbnails
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Django app for DRY thumbnails in admin list views and forms.
 Home-page: http://github.com/BigglesZX/django-admin-thumbnails
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Description: # django-admin-thumbnails
         
@@ -200,10 +200,13 @@
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=2.6,<4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `django-admin-thumbnails-0.2.7/admin_thumbnails/__init__.py` & `django-admin-thumbnails-0.2.8/admin_thumbnails/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,25 +48,30 @@
             )
 
         ''' define the thumbnail field method using the above configuration '''
         def thumbnail_field(self, obj):
             if isinstance(getattr(type(obj), field_name, None), property) or isinstance(getattr(type(obj), field_name, None), cached_property):  # noqa: E501
                 ''' the supplied field_name is a property of the of model '''
                 value = getattr(obj, field_name)
+
+                if value is None:
+                    return ''
+
                 if not isinstance(value, FieldFile):
                     raise TypeError(
                         'admin_thumbnails: Found a model property matching the'
                         ' supplied field name, but it did not return an '
                         'instance of `FieldFile` or a descendent. If using a '
                         'property as the thumbnail source, it must return a '
                         'value from a field that is an instance of Django’s '
                         '`ImageField`, `FileField` or easy_thumbnails’ '
                         '`ThumbnailerImageField` (received: {0})'.format(
                             type(value))
                     )
+
                 field = value.field
                 field_value = value
             else:
                 ''' default: access field_name as a field on the model '''
                 field = obj._meta.get_field(field_name)
                 field_value = getattr(obj, field_name)
```

### Comparing `django-admin-thumbnails-0.2.7/admin_thumbnails/settings.py` & `django-admin-thumbnails-0.2.8/admin_thumbnails/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-thumbnails-0.2.7/README.md` & `django-admin-thumbnails-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-thumbnails-0.2.7/setup.py` & `django-admin-thumbnails-0.2.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     4. $ git tag -a x.x.x  # see `git tags` for latest
     5. $ git push origin master
     6. $ git push --tags
     7. $ python setup.py register sdist
     8. $ twine upload dist/*
 '''
 
-VERSION = '.'.join(('0', '2', '7'))
+VERSION = '.'.join(('0', '2', '8'))
 
 DESCRIPTION = 'A Django app for DRY thumbnails in admin list views and forms.'
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
@@ -41,14 +41,17 @@
     'Framework :: Django :: 1.11',
     'Framework :: Django :: 2.0',
     'Framework :: Django :: 2.1',
     'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.0',
     'Framework :: Django :: 3.1',
     'Framework :: Django :: 3.2',
+    'Framework :: Django :: 4.0',
+    'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
 ]
 
 setup(
     name='django-admin-thumbnails',
     version=VERSION,
     description=DESCRIPTION,
     long_description=open('README.md', 'r', encoding='utf-8').read(),
```

