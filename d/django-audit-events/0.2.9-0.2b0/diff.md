# Comparing `tmp/django-audit-events-0.2.9.tar.gz` & `tmp/django-audit-events-0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-audit-events-0.2.9.tar", last modified: Wed Apr 27 10:43:48 2022, max compression
+gzip compressed data, was "dist/django-audit-events-0.2b0.tar", last modified: Fri Jun  5 08:21:55 2020, max compression
```

## Comparing `django-audit-events-0.2.9.tar` & `django-audit-events-0.2b0.tar`

### file list

```diff
@@ -1,69 +1,64 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)      220 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       27 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3199 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1714 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2408 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      251 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4439 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/context.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/filters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/locale/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/locale/tr/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1544 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/locale/tr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/middleware.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1984 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2207 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/migrations/0002_archivedauditevent.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/migrations/0003_auto_20201218_1113.py
--rw-rw-rw-   0 root         (0) root         (0)      650 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/migrations/0004_auto_20210127_2021.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/migrations/0005_auto_20220215_0756.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4463 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/models.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/test_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6001 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/test_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/test_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2062 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2500 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/urls.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/tests/utils/models.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/django_audit_events/views.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3199 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1740 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/django_audit_events.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1609 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/advanced.rst
--rw-rw-rw-   0 root         (0) root         (0)     2080 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)      944 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1252 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/introduction.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     2265 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2218 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-04-27 10:43:48.000000 django-audit-events-0.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2327 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2022-04-27 10:43:31.000000 django-audit-events-0.2.9/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)       94 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       27 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      251 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3628 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/context.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/filters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/locale/
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/locale/tr/
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/locale/tr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      843 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/middleware.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2007 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4032 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2062 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/urls.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/utils/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/views.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       20 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/advanced.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      944 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/introduction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/tox.ini
```

### Comparing `django-audit-events-0.2.9/LICENSE.txt` & `django-audit-events-0.2b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/PKG-INFO` & `django-audit-events-0.2b0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.2.9
+Version: 0.2b0
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
 Project-URL: Documentation, https://django-audit-events.readthedocs.io/
 Project-URL: Source Code, https://bitbucket.org/akinonteam/django-audit-events
+Description: # Django Audit Events
+        
+        [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
+        [![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
+        ![PyPI](https://img.shields.io/pypi/v/django-audit-events)
+        ![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
+        ![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
+        ![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
+        [![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
+        [![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
+        
+        Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
+        
+        Let's have a look:
+        
+        ```python
+        def awesome_view(request):
+            foo_obj = Foo.objects.get(pk=1)
+            # Do something with foo_obj...
+            request.audit_context.create_event(
+                foo_obj,
+                something="done",
+                bar="baz"
+            )
+        ```
+        
+        This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
+        
+        ```
+        >>> event.content
+        {"something": "done", "bar: "baz"}
+        ```
+        
+        For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
+        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Django Audit Events
-
-[![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
-[![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
-![PyPI](https://img.shields.io/pypi/v/django-audit-events)
-![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
-![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
-![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
-[![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
-[![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
-
-Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
-
-Let's have a look:
-
-```python
-def awesome_view(request):
-    foo_obj = Foo.objects.get(pk=1)
-    # Do something with foo_obj...
-    request.audit_context.create_event(
-        foo_obj,
-        something="done",
-        bar="baz"
-    )
-```
-
-This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
-
-```
->>> event.content
-{"something": "done", "bar: "baz"}
-```
-
-For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
-
-
```

### Comparing `django-audit-events-0.2.9/README.md` & `django-audit-events-0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/bitbucket-pipelines.yml` & `django-audit-events-0.2b0/bitbucket-pipelines.yml`

 * *Files 14% similar despite different names*

```diff
@@ -64,15 +64,15 @@
   tags:
     '*':
       - step:
           name: Publish to PyPI
           image: python:3.7-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
-            - CRYPTOGRAPHY_DONT_BUILD_RUST=1 pip install setuptools setuptools_scm twine
+            - pip install setuptools setuptools_scm twine
             - python setup.py sdist bdist_wheel
             - twine upload -u $PYPI_USERNAME -p $PYPI_PASSWORD dist/*
 definitions:
   services:
     postgres:
       image: postgres
       variables:
```

### Comparing `django-audit-events-0.2.9/django_audit_events/context.py` & `django-audit-events-0.2b0/django_audit_events/context.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 from copy import deepcopy
 
 from django.apps import apps
 from django.contrib.auth.models import AnonymousUser
-from django.utils.module_loading import import_string
 
 from django_audit_events.conf import settings
 
 MASK_VALUE = "*" * 16
 
 
 class AuditContext(object):
     extra_data = {}
-    __slots__ = ["url", "remote_addr", "user", "query_params", "post_data", "headers"]
+    __slots__ = ["url", "remote_addr", "user", "query_params", "post_data"]
 
     def __init__(
-        self,
-        url=None,
-        remote_addr=None,
-        user=None,
-        query_params=None,
-        post_data=None,
-        headers=None,
+        self, url=None, remote_addr=None, user=None, query_params=None, post_data=None
     ):
         super(AuditContext, self).__setattr__("url", url)
         super(AuditContext, self).__setattr__("remote_addr", remote_addr)
         super(AuditContext, self).__setattr__("user", user)
         super(AuditContext, self).__setattr__("query_params", query_params or {})
         super(AuditContext, self).__setattr__("post_data", post_data or {})
-        super(AuditContext, self).__setattr__("headers", headers or {})
 
     def __setattr__(self, key, value):
         raise NotImplementedError
 
     def __delattr__(self, item):
         raise NotImplementedError
 
@@ -41,44 +33,33 @@
         Create a context from HTTP request
 
         :type request: django.http.HttpRequest
         :return: An audit context
         :rtype: AuditContext
         """
         # noinspection PyUnresolvedReferences
-        client_ip_function = cls.get_client_ip_function()
         context = {
             "url": request.build_absolute_uri(),
-            "remote_addr": client_ip_function(request),
+            "remote_addr": request.META.get("REMOTE_ADDR"),
             "user": request.user,
         }
 
         if isinstance(context["user"], AnonymousUser):
             context["user"] = None
 
         if settings.AUDIT_INCLUDE_QUERY_PARAMS:
             context["query_params"] = request.GET
 
         if settings.AUDIT_INCLUDE_POST_DATA:
             # Copy POST data before masking sensitive fields
             # noinspection PyArgumentList
             context["post_data"] = cls.mask_fields(
-                request.POST.copy(),
-                settings.AUDIT_MASK_POST_FIELDS,
+                request.POST.copy(), settings.AUDIT_MASK_POST_FIELDS,
             )
 
-        if settings.AUDIT_INCLUDE_HEADERS and isinstance(
-            settings.AUDIT_INCLUDE_HEADERS, list
-        ):
-            context["headers"] = {
-                header: request.META.get(header)
-                for header in settings.AUDIT_INCLUDE_HEADERS
-                if request.META.get(header)
-            }
-
         return cls(**context)
 
     @staticmethod
     def mask_fields(data, fields_to_mask):
         """
         Replace sensitive information in POST data
         :param data: POST data
@@ -122,14 +103,7 @@
         :param content: Event content
         :return: Saved audit event
         :rtype: django_audit_events.models.AbstractAuditEvent
         """
         for field in fields:
             content[field] = getattr(content_object, field)
         return self.create_event(content_object, **content)
-
-    @classmethod
-    def get_client_ip_function(cls):
-        _function = settings.AUDIT_CLIENT_IP_RESOLVER_FUNCTION
-        if callable(_function):
-            return _function
-        return import_string(_function)
```

### Comparing `django-audit-events-0.2.9/django_audit_events/locale/tr/LC_MESSAGES/django.po` & `django-audit-events-0.2b0/django_audit_events/locale/tr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -54,18 +54,14 @@
 msgid "Query params"
 msgstr "Sorgu parametreleri"
 
 #: models.py:28
 msgid "Post data"
 msgstr "Form verisi"
 
-#: models.py:54
-msgid "Headers"
-msgstr "İstek başlıkları"
-
 #: models.py:32
 msgid "Content"
 msgstr "İçerik"
 
 #: models.py:35
 msgid "Audit event"
 msgstr "Denetim olayı"
```

### Comparing `django-audit-events-0.2.9/django_audit_events/middleware.py` & `django-audit-events-0.2b0/django_audit_events/middleware.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/django_audit_events/migrations/0001_initial.py` & `django-audit-events-0.2b0/django_audit_events/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # Generated by Django 3.0.1 on 2019-12-26 14:35
 
 import uuid
 
+import django.contrib.postgres.fields.jsonb
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
-try:
-    from django.db.models import JSONField
-except ImportError:
-    from django.contrib.postgres.fields.jsonb import JSONField
-
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         ('contenttypes', '0002_remove_content_type_name'),
@@ -25,18 +21,18 @@
         migrations.CreateModel(
             name='AuditEvent',
             fields=[
                 ('uuid', models.UUIDField(default=uuid.uuid4, primary_key=True, serialize=False, verbose_name='ID')),
                 ('timestamp', models.DateTimeField(auto_now_add=True, verbose_name='Timestamp')),
                 ('remote_addr', models.GenericIPAddressField(blank=True, null=True, verbose_name='IP address')),
                 ('url', models.URLField(blank=True, null=True, verbose_name='URL')),
-                ('query_params', JSONField(blank=True, default=dict, null=True, verbose_name='Query params')),
-                ('post_data', JSONField(blank=True, default=dict, null=True, verbose_name='Post data')),
+                ('query_params', django.contrib.postgres.fields.jsonb.JSONField(blank=True, default=dict, null=True, verbose_name='Query params')),
+                ('post_data', django.contrib.postgres.fields.jsonb.JSONField(blank=True, default=dict, null=True, verbose_name='Post data')),
                 ('object_id', models.PositiveIntegerField()),
-                ('content', JSONField(default=dict, verbose_name='Content')),
+                ('content', django.contrib.postgres.fields.jsonb.JSONField(default=dict, verbose_name='Content')),
                 ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='contenttypes.ContentType')),
                 ('user', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL, verbose_name='User')),
             ],
             options={
                 'ordering': ('-timestamp',),
                 'verbose_name': 'Audit event',
                 'verbose_name_plural': 'Audit events',
```

### Comparing `django-audit-events-0.2.9/django_audit_events/mixin.py` & `django-audit-events-0.2b0/django_audit_events/mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/django_audit_events/models.py` & `django-audit-events-0.2b0/django_audit_events/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,79 +2,46 @@
 
 import uuid
 
 from django.apps import apps
 from django.conf import settings as django_settings
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
+from django.contrib.postgres.fields import JSONField
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.utils.translation import ugettext_lazy as _
 
 from django_audit_events.conf import settings
 
-try:
-    from django.db.models import JSONField
-except ImportError:
-    from django.contrib.postgres.fields import JSONField
-
 
 class AbstractAuditEvent(models.Model):
-    uuid = models.UUIDField(
-        verbose_name=_("ID"),
-        default=uuid.uuid4,
-        primary_key=True,
-    )
+    uuid = models.UUIDField(verbose_name=_("ID"), default=uuid.uuid4, primary_key=True,)
     timestamp = models.DateTimeField(verbose_name=_("Timestamp"), auto_now_add=True)
     user = models.ForeignKey(
         django_settings.AUTH_USER_MODEL,
         on_delete=models.SET_NULL,
         verbose_name=_("User"),
         blank=True,
         null=True,
     )
     remote_addr = models.GenericIPAddressField(
-        verbose_name=_("IP address"),
-        blank=True,
-        null=True,
-    )
-    url = models.URLField(
-        verbose_name=_("URL"),
-        blank=True,
-        null=True,
-        max_length=1000,
+        verbose_name=_("IP address"), blank=True, null=True,
     )
+    url = models.URLField(verbose_name=_("URL"), blank=True, null=True,)
     query_params = JSONField(
-        verbose_name=_("Query params"),
-        default=dict,
-        blank=True,
-        null=True,
+        verbose_name=_("Query params"), default=dict, blank=True, null=True,
     )
     post_data = JSONField(
-        verbose_name=_("Post data"),
-        default=dict,
-        blank=True,
-        null=True,
-    )
-    headers = JSONField(
-        verbose_name=_("Headers"),
-        default=dict,
-        blank=True,
-        null=True,
-    )
-    content_type = models.ForeignKey(
-        ContentType,
-        on_delete=models.CASCADE,
+        verbose_name=_("Post data"), default=dict, blank=True, null=True,
     )
+    content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE,)
     object_id = models.PositiveIntegerField()
     content_object = GenericForeignKey("content_type", "object_id")
-    content = JSONField(
-        verbose_name=_("Content"),
-        default=dict,
-    )
+    content = JSONField(verbose_name=_("Content"), default=dict,)
 
     class Meta:
         verbose_name = _("Audit event")
         verbose_name_plural = _("Audit events")
         ordering = ("-timestamp",)
         abstract = True
 
@@ -90,15 +57,14 @@
 
         obj = cls()
         obj.user = context.user
         obj.remote_addr = context.remote_addr
         obj.url = context.url
         obj.query_params = context.query_params
         obj.post_data = context.post_data
-        obj.headers = context.headers
         return obj
 
     def as_archive_event(self):
         archive_model = get_audit_event_archive_model()
         fields = archive_model._meta.get_fields()
         return archive_model(
             **{field.name: getattr(self, field.name, None) for field in fields}
```

### Comparing `django-audit-events-0.2.9/django_audit_events/tasks.py` & `django-audit-events-0.2b0/django_audit_events/tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,29 +24,17 @@
 
 @app.task
 def archive_old_audit_events(older_than=90):
     audit_event_model = get_audit_event_model()
     archived_audit_event_model = get_audit_event_archive_model()
 
     reference_date = timezone.now() - timedelta(days=older_than)
-    events_to_delete = set()
-
-    for event in audit_event_model.objects.iterator():
-        if event.content_object is None:
-            events_to_delete.add(event.uuid)
-
-    events_to_delete = list(events_to_delete)
-
-    for chunk in _chunks(events_to_delete):
-        with transaction.atomic():
-            audit_event_model.objects.filter(uuid__in=[e for e in chunk]).delete()
-
     events_to_archive = audit_event_model.objects.filter(timestamp__lte=reference_date)
+
     archive_items = [event.as_archive_event() for event in events_to_archive]
 
     for chunk in _chunks(archive_items):
         with transaction.atomic():
             archived_audit_event_model.objects.bulk_create(chunk)
             audit_event_model.objects.filter(uuid__in=[e.uuid for e in chunk]).delete()
 
     logger.info("Archived %d audit events." % events_to_archive.count())
-    logger.info("Deleted %d audit events." % len(events_to_delete))
```

### Comparing `django-audit-events-0.2.9/django_audit_events/tests/test_middleware.py` & `django-audit-events-0.2b0/django_audit_events/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/django_audit_events/tests/test_mixin.py` & `django-audit-events-0.2b0/django_audit_events/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/django_audit_events/tests/test_models.py` & `django-audit-events-0.2b0/django_audit_events/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/django_audit_events/tests/test_tasks.py` & `django-audit-events-0.2b0/django_audit_events/tests/test_tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,52 +18,32 @@
             for _ in range(100)
         ]
         AuditEvent.objects.bulk_create(events)
         for event in events:
             event.timestamp = self.get_random_past_date()
             event.save()
 
-        for _ in range(25):
-            random_event = random.choice(events)
-
-            if random_event.content_object:
-                random_event.content_object.delete()
-
-            random_event.save()
-
     def tearDown(self):
         AuditEvent.objects.all().delete()
         ArchivedAuditEvent.objects.all().delete()
 
     @override_settings(CELERY_ALWAYS_EAGER=True)
     def test_archiver_task(self):
         older_than = 90
         query = Q(timestamp__lte=timezone.now() - timedelta(days=older_than))
-        events_to_delete = set()
-
-        for event in AuditEvent.objects.iterator():
-            if event.content_object is None:
-                events_to_delete.add(event.uuid)
-
-        events_to_archive = AuditEvent.objects.filter(query).exclude(
-            uuid__in=events_to_delete
-        )
+        events_to_archive = AuditEvent.objects.filter(query)
         uuids = set([e.uuid for e in events_to_archive])
 
         archive_old_audit_events(older_than=older_than)
 
         archived_events = ArchivedAuditEvent.objects.all()
         archived_uuids = set([e.uuid for e in archived_events])
         self.assertEqual(len(events_to_archive), len(archived_events))
         self.assertSetEqual(uuids, archived_uuids)
         self.assertFalse(AuditEvent.objects.filter(uuid__in=archived_uuids).exists())
-        self.assertFalse(
-            ArchivedAuditEvent.objects.filter(uuid__in=events_to_delete).exists()
-        )
-        self.assertFalse(AuditEvent.objects.filter(uuid__in=events_to_delete).exists())
 
     def get_random_past_date(self, base=timezone.now, date_range=timedelta(days=365)):
         if callable(base):
             base = base()
         seconds = date_range.total_seconds()
         minus_seconds = random.randint(0, seconds)
         return base - timedelta(seconds=minus_seconds)
```

### Comparing `django-audit-events-0.2.9/django_audit_events/views.py` & `django-audit-events-0.2b0/django_audit_events/views.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/django_audit_events.egg-info/PKG-INFO` & `django-audit-events-0.2b0/django_audit_events.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.2.9
+Version: 0.2b0
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
 Project-URL: Documentation, https://django-audit-events.readthedocs.io/
 Project-URL: Source Code, https://bitbucket.org/akinonteam/django-audit-events
+Description: # Django Audit Events
+        
+        [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
+        [![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
+        ![PyPI](https://img.shields.io/pypi/v/django-audit-events)
+        ![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
+        ![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
+        ![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
+        [![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
+        [![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
+        
+        Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
+        
+        Let's have a look:
+        
+        ```python
+        def awesome_view(request):
+            foo_obj = Foo.objects.get(pk=1)
+            # Do something with foo_obj...
+            request.audit_context.create_event(
+                foo_obj,
+                something="done",
+                bar="baz"
+            )
+        ```
+        
+        This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
+        
+        ```
+        >>> event.content
+        {"something": "done", "bar: "baz"}
+        ```
+        
+        For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
+        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Django Audit Events
-
-[![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
-[![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
-![PyPI](https://img.shields.io/pypi/v/django-audit-events)
-![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
-![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
-![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
-[![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
-[![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
-
-Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
-
-Let's have a look:
-
-```python
-def awesome_view(request):
-    foo_obj = Foo.objects.get(pk=1)
-    # Do something with foo_obj...
-    request.audit_context.create_event(
-        foo_obj,
-        something="done",
-        bar="baz"
-    )
-```
-
-This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
-
-```
->>> event.content
-{"something": "done", "bar: "baz"}
-```
-
-For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
-
-
```

### Comparing `django-audit-events-0.2.9/django_audit_events.egg-info/SOURCES.txt` & `django-audit-events-0.2b0/django_audit_events.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,28 +18,23 @@
 django_audit_events/filters.py
 django_audit_events/middleware.py
 django_audit_events/mixin.py
 django_audit_events/models.py
 django_audit_events/serializers.py
 django_audit_events/tasks.py
 django_audit_events/urls.py
-django_audit_events/utils.py
 django_audit_events/version.py
 django_audit_events/views.py
 django_audit_events.egg-info/PKG-INFO
 django_audit_events.egg-info/SOURCES.txt
 django_audit_events.egg-info/dependency_links.txt
 django_audit_events.egg-info/not-zip-safe
 django_audit_events.egg-info/top_level.txt
 django_audit_events/locale/tr/LC_MESSAGES/django.po
 django_audit_events/migrations/0001_initial.py
-django_audit_events/migrations/0002_archivedauditevent.py
-django_audit_events/migrations/0003_auto_20201218_1113.py
-django_audit_events/migrations/0004_auto_20210127_2021.py
-django_audit_events/migrations/0005_auto_20220215_0756.py
 django_audit_events/migrations/__init__.py
 django_audit_events/tests/__init__.py
 django_audit_events/tests/test_conf.py
 django_audit_events/tests/test_context.py
 django_audit_events/tests/test_middleware.py
 django_audit_events/tests/test_mixin.py
 django_audit_events/tests/test_models.py
```

### Comparing `django-audit-events-0.2.9/docs/Makefile` & `django-audit-events-0.2b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/docs/advanced.rst` & `django-audit-events-0.2b0/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/docs/conf.py` & `django-audit-events-0.2b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/docs/index.rst` & `django-audit-events-0.2b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/docs/introduction.rst` & `django-audit-events-0.2b0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/docs/make.bat` & `django-audit-events-0.2b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/docs/quickstart.rst` & `django-audit-events-0.2b0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/runtests.py` & `django-audit-events-0.2b0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2.9/setup.py` & `django-audit-events-0.2b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         "Framework :: Django",
         "Framework :: Django :: 1.10",
         "Framework :: Django :: 1.11",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
```

### Comparing `django-audit-events-0.2.9/tox.ini` & `django-audit-events-0.2b0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -5,37 +5,33 @@
 
 [tox]
 isolated_build = True
 skip_missing_interpreters = True
 envlist = py27-{django110,django111}
           py34-{django110,django111,django20}
           py35-{django110,django111,django20,django21,django22}
-          {py36,py37}-{django111,django20,django21,django22,django30,django31}
-          py38-{django22,django30,django31}
+          {py36,py37}-{django111,django20,django21,django22,django30}
+          py38-{django22,django30}
           linting
 
 [testenv]
 deps = celery>=4.3.0,<4.4.0
-       django110: Django>=1.10,<1.11.1
+       django110: Django>=1.10,<1.11
        django111: Django>=1.11.7,<2.0
        django20: Django>=2.0,<2.1
        django21: Django>=2.1,<2.2
        django22: Django>=2.2.8,<3.0
        django30: Django>=3.0,<3.1
-       django31: Django>=3.1,<3.2
-       model-bakery==1.1.0
+       model-bakery
        psycopg2-binary
-       vine==1.3.0
 commands = python runtests.py
 
 [testenv:linting]
-deps = black==21.12b0
+deps = black
        celery
-       isort==5.0.4
-       Django>=2.2.8,<3.2
+       isort
+       Django>=2.2.8,<3.0
        djangorestframework<3.12
        djangorestframework-filters<0.12
        model-bakery
-       vine==1.3.0
-       click==7.1.2
-commands = black --check django_audit_events
-           isort -c django_audit_events
+commands = black --check --quiet django_audit_events
+           isort -rc -c django_audit_events
```

