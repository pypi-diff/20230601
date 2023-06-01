# Comparing `tmp/common-logging-library-django-2.1.0.tar.gz` & `tmp/common-logging-library-django-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-logging-library-django-2.1.0.tar", last modified: Thu Jun  1 13:23:38 2023, max compression
+gzip compressed data, was "common-logging-library-django-2.2.0.tar", last modified: Thu Jun  1 13:55:53 2023, max compression
```

## Comparing `common-logging-library-django-2.1.0.tar` & `common-logging-library-django-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxr-xr-x   0 turja      (501) staff       (20)        0 2023-06-01 13:23:38.811671 common-logging-library-django-2.1.0/
--rw-r--r--   0 turja      (501) staff       (20)      287 2023-06-01 13:23:38.811535 common-logging-library-django-2.1.0/PKG-INFO
--rw-r--r--   0 turja      (501) staff       (20)        0 2023-06-01 11:53:11.000000 common-logging-library-django-2.1.0/README.md
-drwxr-xr-x   0 turja      (501) staff       (20)        0 2023-06-01 13:23:38.811355 common-logging-library-django-2.1.0/common_logging_library_django.egg-info/
--rw-r--r--   0 turja      (501) staff       (20)      287 2023-06-01 13:23:38.000000 common-logging-library-django-2.1.0/common_logging_library_django.egg-info/PKG-INFO
--rw-r--r--   0 turja      (501) staff       (20)      297 2023-06-01 13:23:38.000000 common-logging-library-django-2.1.0/common_logging_library_django.egg-info/SOURCES.txt
--rw-r--r--   0 turja      (501) staff       (20)        1 2023-06-01 13:23:38.000000 common-logging-library-django-2.1.0/common_logging_library_django.egg-info/dependency_links.txt
--rw-r--r--   0 turja      (501) staff       (20)       12 2023-06-01 13:23:38.000000 common-logging-library-django-2.1.0/common_logging_library_django.egg-info/requires.txt
--rw-r--r--   0 turja      (501) staff       (20)        1 2023-06-01 13:23:38.000000 common-logging-library-django-2.1.0/common_logging_library_django.egg-info/top_level.txt
--rw-r--r--   0 turja      (501) staff       (20)      108 2023-06-01 11:30:31.000000 common-logging-library-django-2.1.0/pyproject.toml
--rw-r--r--   0 turja      (501) staff       (20)       38 2023-06-01 13:23:38.811706 common-logging-library-django-2.1.0/setup.cfg
--rw-r--r--   0 turja      (501) staff       (20)     1936 2023-06-01 13:21:32.000000 common-logging-library-django-2.1.0/setup.py
+drwxr-xr-x   0 turja      (501) staff       (20)        0 2023-06-01 13:55:53.074102 common-logging-library-django-2.2.0/
+-rw-r--r--   0 turja      (501) staff       (20)      287 2023-06-01 13:55:53.073971 common-logging-library-django-2.2.0/PKG-INFO
+-rw-r--r--   0 turja      (501) staff       (20)        0 2023-06-01 11:53:11.000000 common-logging-library-django-2.2.0/README.md
+drwxr-xr-x   0 turja      (501) staff       (20)        0 2023-06-01 13:55:53.072799 common-logging-library-django-2.2.0/common_logging_library_django.egg-info/
+-rw-r--r--   0 turja      (501) staff       (20)      287 2023-06-01 13:55:53.000000 common-logging-library-django-2.2.0/common_logging_library_django.egg-info/PKG-INFO
+-rw-r--r--   0 turja      (501) staff       (20)      478 2023-06-01 13:55:53.000000 common-logging-library-django-2.2.0/common_logging_library_django.egg-info/SOURCES.txt
+-rw-r--r--   0 turja      (501) staff       (20)        1 2023-06-01 13:55:53.000000 common-logging-library-django-2.2.0/common_logging_library_django.egg-info/dependency_links.txt
+-rw-r--r--   0 turja      (501) staff       (20)       12 2023-06-01 13:55:53.000000 common-logging-library-django-2.2.0/common_logging_library_django.egg-info/requires.txt
+-rw-r--r--   0 turja      (501) staff       (20)       43 2023-06-01 13:55:53.000000 common-logging-library-django-2.2.0/common_logging_library_django.egg-info/top_level.txt
+drwxr-xr-x   0 turja      (501) staff       (20)        0 2023-06-01 13:55:53.073264 common-logging-library-django-2.2.0/logging_library/
+-rw-r--r--   0 turja      (501) staff       (20)        0 2023-06-01 13:54:48.000000 common-logging-library-django-2.2.0/logging_library/__init__.py
+drwxr-xr-x   0 turja      (501) staff       (20)        0 2023-06-01 13:55:53.073667 common-logging-library-django-2.2.0/logging_library/access_log/
+-rw-r--r--   0 turja      (501) staff       (20)        0 2023-06-01 11:58:05.000000 common-logging-library-django-2.2.0/logging_library/access_log/__init__.py
+-rw-r--r--   0 turja      (501) staff       (20)     1469 2023-06-01 12:54:52.000000 common-logging-library-django-2.2.0/logging_library/access_log/middleware.py
+-rw-r--r--   0 turja      (501) staff       (20)     1290 2023-06-01 11:54:05.000000 common-logging-library-django-2.2.0/logging_library/logging_filters.py
+-rw-r--r--   0 turja      (501) staff       (20)     1982 2023-06-01 11:55:25.000000 common-logging-library-django-2.2.0/logging_library/logging_formatters.py
+-rw-r--r--   0 turja      (501) staff       (20)      108 2023-06-01 11:30:31.000000 common-logging-library-django-2.2.0/pyproject.toml
+-rw-r--r--   0 turja      (501) staff       (20)       38 2023-06-01 13:55:53.074142 common-logging-library-django-2.2.0/setup.cfg
+-rw-r--r--   0 turja      (501) staff       (20)     1922 2023-06-01 13:55:46.000000 common-logging-library-django-2.2.0/setup.py
```

### Comparing `common-logging-library-django-2.1.0/setup.py` & `common-logging-library-django-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import sys
 import codecs
 
 
 
 name = 'common-logging-library-django'
-package = 'common_logging_library_django'
+package = 'logging_library'
 description = 'A Django library for logging'
 url = 'https://github.com/nhst/common-logging-library-django/'
 author = 'simantaturja'
 author_email = 'simanta.turja@nhst.no'
 license = 'BSD'
 install_requires = ["django>=3.2"]
```

