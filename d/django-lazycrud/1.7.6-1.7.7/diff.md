# Comparing `tmp/django-lazycrud-1.7.6.tar.gz` & `tmp/django-lazycrud-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lazycrud-1.7.6.tar", last modified: Tue Nov 22 17:51:24 2022, max compression
+gzip compressed data, was "django-lazycrud-1.7.7.tar", last modified: Thu Jun  1 13:30:39 2023, max compression
```

## Comparing `django-lazycrud-1.7.6.tar` & `django-lazycrud-1.7.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.867733 django-lazycrud-1.7.6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1083 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2022-11-22 17:51:24.867733 django-lazycrud-1.7.6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2297 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.859733 django-lazycrud-1.7.6/django_lazycrud.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2022-11-22 17:51:24.000000 django-lazycrud-1.7.6/django_lazycrud.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2437 2022-11-22 17:51:24.000000 django-lazycrud-1.7.6/django_lazycrud.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-11-22 17:51:24.000000 django-lazycrud-1.7.6/django_lazycrud.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-11-22 17:51:24.000000 django-lazycrud-1.7.6/django_lazycrud.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2022-11-22 17:51:24.000000 django-lazycrud-1.7.6/django_lazycrud.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2022-11-22 17:51:24.000000 django-lazycrud-1.7.6/django_lazycrud.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      364 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/context_processors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2402 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/forms.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.859733 django-lazycrud-1.7.6/lazycrud/locale/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.859733 django-lazycrud-1.7.6/lazycrud/locale/it/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/locale/it/LC_MESSAGES/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1015 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1973 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.859733 django-lazycrud-1.7.6/lazycrud/static/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.859733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4571 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/dataTables.bootstrap.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3362 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/dataTables.fontAwesome.css
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8486 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/datatables.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33704 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/datepicker3.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7785 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/datetimepicker.min.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/fixedHeader.dataTables.min.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datepicker/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.it.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46821 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datetimepicker/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38510 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datetimepicker/datetimepicker.min.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9614 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/dataTables.bootstrap.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6945 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/dataTables.fixedHeader.min.js
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    96574 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/datatables.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1803 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/datetime-moment.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1266 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/de.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/es.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1015 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/fr.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      899 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/it.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   423608 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/jquery.dataTables.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33783 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/moment.min.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.863733 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/moment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2254 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/moment/it.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   369019 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/moment/moment-with-locales.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61318 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/moment/moment.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/object_form.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1365 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/object_list.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.859733 django-lazycrud-1.7.6/lazycrud/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.867733 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/_datatables_css.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/_datatables_js.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1944 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/_table.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_confirm_delete.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1463 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_detail.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_detail_with_related_list.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3251 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_form.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_form_with_related_formset.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_formset.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_list.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1973 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templates/lazycrud/table_inline_formset.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:51:24.867733 django-lazycrud-1.7.6/lazycrud/templatetags/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templatetags/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2019 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/templatetags/lazycrud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/lazycrud/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2022-11-22 17:51:24.867733 django-lazycrud-1.7.6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      587 2022-11-22 17:50:59.000000 django-lazycrud-1.7.6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.664956 django-lazycrud-1.7.7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1083 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-06-01 13:30:39.664956 django-lazycrud-1.7.7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2297 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/django_lazycrud.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-06-01 13:30:39.000000 django-lazycrud-1.7.7/django_lazycrud.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2437 2023-06-01 13:30:39.000000 django-lazycrud-1.7.7/django_lazycrud.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 13:30:39.000000 django-lazycrud-1.7.7/django_lazycrud.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 13:30:39.000000 django-lazycrud-1.7.7/django_lazycrud.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2023-06-01 13:30:39.000000 django-lazycrud-1.7.7/django_lazycrud.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-01 13:30:39.000000 django-lazycrud-1.7.7/django_lazycrud.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/lazycrud/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      364 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/context_processors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2402 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/forms.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.656956 django-lazycrud-1.7.7/lazycrud/locale/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.656956 django-lazycrud-1.7.7/lazycrud/locale/it/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/lazycrud/locale/it/LC_MESSAGES/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1015 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1973 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.656956 django-lazycrud-1.7.7/lazycrud/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.656956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4571 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/dataTables.bootstrap.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3362 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/dataTables.fontAwesome.css
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8486 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/datatables.min.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33704 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/datepicker3.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7785 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/datetimepicker.min.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/fixedHeader.dataTables.min.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datepicker/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.it.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    46821 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datetimepicker/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38510 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datetimepicker/datetimepicker.min.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.660956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9614 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/dataTables.bootstrap.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6945 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/dataTables.fixedHeader.min.js
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    96574 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/datatables.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1803 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/datetime-moment.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.664956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1266 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/de.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/es.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1015 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/fr.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      899 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/it.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   423608 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/jquery.dataTables.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33783 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/moment.min.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.664956 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/moment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2254 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/moment/it.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   369019 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/moment/moment-with-locales.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61318 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/moment/moment.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/object_form.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1365 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/object_list.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.656956 django-lazycrud-1.7.7/lazycrud/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.664956 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/_datatables_css.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/_datatables_js.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2099 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/_table.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_confirm_delete.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1463 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_detail.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_detail_with_related_list.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3251 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_form.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_form_with_related_formset.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_formset.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_list.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1973 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templates/lazycrud/table_inline_formset.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:39.664956 django-lazycrud-1.7.7/lazycrud/templatetags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templatetags/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2019 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/templatetags/lazycrud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/lazycrud/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-06-01 13:30:39.664956 django-lazycrud-1.7.7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      587 2023-06-01 13:30:20.000000 django-lazycrud-1.7.7/setup.py
```

### Comparing `django-lazycrud-1.7.6/LICENSE.txt` & `django-lazycrud-1.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/README.rst` & `django-lazycrud-1.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/django_lazycrud.egg-info/SOURCES.txt` & `django-lazycrud-1.7.7/django_lazycrud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/forms.py` & `django-lazycrud-1.7.7/lazycrud/forms.py`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/locale/it/LC_MESSAGES/django.mo` & `django-lazycrud-1.7.7/lazycrud/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/locale/it/LC_MESSAGES/django.po` & `django-lazycrud-1.7.7/lazycrud/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/dataTables.bootstrap.css` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/dataTables.fontAwesome.css` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/dataTables.fontAwesome.css`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/datatables.min.css` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/datepicker3.css` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/datepicker3.css`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/css/datetimepicker.min.css` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/css/datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.it.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.it.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/bootstrap-datetimepicker/datetimepicker.min.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/bootstrap-datetimepicker/datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/dataTables.bootstrap.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/dataTables.fixedHeader.min.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/dataTables.fixedHeader.min.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/datatables.min.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/datetime-moment.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/datetime-moment.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/de.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/es.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/fr.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/i18n/it.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/jquery.dataTables.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/dataTables/moment.min.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/dataTables/moment.min.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/moment/it.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/moment/it.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/moment/moment-with-locales.min.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/moment/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/moment/moment.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/moment/moment.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/object_form.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/object_form.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/static/lazycrud/js/object_list.js` & `django-lazycrud-1.7.7/lazycrud/static/lazycrud/js/object_list.js`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/_table.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/_table.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 {% load lazycrud %}
 {% load i18n %}
 
 <table class="table {% if table_classes %}{{ table_classes }}{% else %}table-striped table-hover table-datatables{% endif %}"
     {% if datatables_options %} data-datatables-options="{{ datatables_options }}"{% endif %}>
     <thead>
         <tr>
+    {% if table_headers %}
+        {% for header in table_headers %}
+            <th>{{ header }}</th>
+        {% endfor %}
+    {% else %}
         {% for name in object_fields %}
             <th>{{ object_model|fieldlabel:name }}</th>
         {% endfor %}
+    {% endif %}
         {% if object_actions is not None %}
             <th></th>
         {% endif %}
         </tr>
     </thead>
     <tbody>
         {% for o in object_list %}
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 {% load lazycrud %} {% load i18n %}
 % if datatables_options %} data-datatables-options="{{ datatables_options }}"{%
 endif %}>
-{% for name in object_fields %}
+{% if table_headers %} {% for header in table_headers %}
+{{ header }}
+{% endfor %} {% else %} {% for name in object_fields %}
 {{ object_model|fieldlabel:name }}
-{% endfor %} {% if object_actions is not None %}
+{% endfor %} {% endif %} {% if object_actions is not None %}
 {% endif %}
   {% for o in object_list %}
 % if object_url %} class="clickable_row" data-url="{% url object_url pk=o.pk
 %}" {% elif o.get_absolute_url %} class="clickable_row" data-url="{
 { o.get_absolute_url }}" {% endif %} {% if object_url_target %} data-target="{
 { object_url_target }}" {% endif %} > {% for name in object_fields %}
 {{ o|fieldvalue:name }}
```

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_confirm_delete.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_detail.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_detail.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_detail_with_related_list.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_detail_with_related_list.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_form.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_form.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_form_with_related_formset.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_form_with_related_formset.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_formset.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_formset.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/object_list.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/object_list.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templates/lazycrud/table_inline_formset.html` & `django-lazycrud-1.7.7/lazycrud/templates/lazycrud/table_inline_formset.html`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/templatetags/lazycrud.py` & `django-lazycrud-1.7.7/lazycrud/templatetags/lazycrud.py`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/lazycrud/utils.py` & `django-lazycrud-1.7.7/lazycrud/utils.py`

 * *Files identical despite different names*

### Comparing `django-lazycrud-1.7.6/setup.py` & `django-lazycrud-1.7.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'django-lazycrud',
-    version = '1.7.6',
+    version = '1.7.7',
     packages = find_packages(),
     author = 'Augusto Destrero',
     author_email = 'a.destrero@gmail.com',
     license='MIT',
     description = 'A little Django app to reduce boilerplate code at a minimum when you write class based views in a typical CRUD scenario.',
     url = 'https://github.com/baxeico/django-lazycrud',
     keywords = ['django', 'crud'],
```

