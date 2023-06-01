# Comparing `tmp/unicef-security-1.4.3.tar.gz` & `tmp/unicef-security-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicef-security-1.4.3.tar", last modified: Thu May 11 13:55:17 2023, max compression
+gzip compressed data, was "unicef-security-1.4.4.tar", last modified: Thu Jun  1 07:50:04 2023, max compression
```

## Comparing `unicef-security-1.4.3.tar` & `unicef-security-1.4.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.216199 unicef-security-1.4.3/
--rw-r--r--   0 jojo       (501) staff       (20)     2025 2023-05-11 13:54:23.000000 unicef-security-1.4.3/CHANGES
--rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:23:06.000000 unicef-security-1.4.3/LICENSE
--rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-security-1.4.3/MANIFEST.in
--rw-r--r--   0 jojo       (501) staff       (20)     1791 2023-05-05 13:23:06.000000 unicef-security-1.4.3/Makefile
--rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 13:55:17.216430 unicef-security-1.4.3/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     2618 2023-05-05 13:23:06.000000 unicef-security-1.4.3/README.rst
--rw-r--r--   0 jojo       (501) staff       (20)       82 2023-05-11 13:55:17.217378 unicef-security-1.4.3/setup.cfg
--rwxr-xr-x   0 jojo       (501) staff       (20)     1921 2023-05-05 13:23:06.000000 unicef-security-1.4.3/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.172741 unicef-security-1.4.3/src/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.188282 unicef-security-1.4.3/src/unicef_security/
--rw-r--r--   0 jojo       (501) staff       (20)       57 2023-05-11 13:54:23.000000 unicef-security-1.4.3/src/unicef_security/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     6144 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/admin.py
--rw-r--r--   0 jojo       (501) staff       (20)      127 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/apps.py
--rw-r--r--   0 jojo       (501) staff       (20)     1373 2023-05-11 11:07:37.000000 unicef-security-1.4.3/src/unicef_security/backends.py
--rw-r--r--   0 jojo       (501) staff       (20)     1023 2023-05-11 13:54:23.000000 unicef-security-1.4.3/src/unicef_security/config.py
--rw-r--r--   0 jojo       (501) staff       (20)    11031 2023-05-11 10:50:08.000000 unicef-security-1.4.3/src/unicef_security/graph.py
--rw-r--r--   0 jojo       (501) staff       (20)     2276 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/middleware.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.193615 unicef-security-1.4.3/src/unicef_security/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     7279 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/0001_initial.py
--rw-r--r--   0 jojo       (501) staff       (20)      454 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/0002_auto_20201028_0154.py
--rw-r--r--   0 jojo       (501) staff       (20)      528 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/0003_auto_20220406_2307.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1314 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/models.py
--rw-r--r--   0 jojo       (501) staff       (20)     3006 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/pipeline.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.194013 unicef-security-1.4.3/src/unicef_security/templates/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.196548 unicef-security-1.4.3/src/unicef_security/templates/admin/
--rw-r--r--   0 jojo       (501) staff       (20)      650 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/ad.html
--rw-r--r--   0 jojo       (501) staff       (20)     1380 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/link_user.html
--rw-r--r--   0 jojo       (501) staff       (20)      786 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/load_users.html
--rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/login.html
--rw-r--r--   0 jojo       (501) staff       (20)     2625 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/unauthorized.html
--rw-r--r--   0 jojo       (501) staff       (20)      316 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)      223 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/utils.py
--rw-r--r--   0 jojo       (501) staff       (20)      925 2023-05-11 13:54:23.000000 unicef-security-1.4.3/src/unicef_security/views.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.191437 unicef-security-1.4.3/src/unicef_security.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1867 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)      295 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       16 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/top_level.txt
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.202236 unicef-security-1.4.3/tests/
--rw-r--r--   0 jojo       (501) staff       (20)      218 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/.coveragerc
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      129 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/conftest.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.203795 unicef-security-1.4.3/tests/demoproject/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.207776 unicef-security-1.4.3/tests/demoproject/demo/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      172 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/admin.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.212909 unicef-security-1.4.3/tests/demoproject/demo/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/migrations/0001_initial.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/migrations/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      138 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/models.py
--rw-r--r--   0 jojo       (501) staff       (20)     2432 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/settings.py
--rw-r--r--   0 jojo       (501) staff       (20)      210 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/wsgi.py
--rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/factories.py
--rwxr-xr-x   0 jojo       (501) staff       (20)      810 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/manage.py
--rw-r--r--   0 jojo       (501) staff       (20)      219 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/fixtures.py
--rw-r--r--   0 jojo       (501) staff       (20)      208 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_admin.py
--rw-r--r--   0 jojo       (501) staff       (20)     1095 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_azure.py
--rw-r--r--   0 jojo       (501) staff       (20)      216 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_backends.py
--rw-r--r--   0 jojo       (501) staff       (20)      439 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_models.py
--rw-r--r--   0 jojo       (501) staff       (20)     2601 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_pipeline.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.215711 unicef-security-1.4.3/tests/vcr_cassettes/
--rw-r--r--   0 jojo       (501) staff       (20)     9126 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/_test_user_data.yml
--rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/load_business_area.yml
--rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/load_region.yml
--rw-r--r--   0 jojo       (501) staff       (20)     2984 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/test_token.yml
--rw-r--r--   0 jojo       (501) staff       (20)     7655 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/test_user_data.yml
--rw-r--r--   0 jojo       (501) staff       (20)      823 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcrpy.py
--rw-r--r--   0 jojo       (501) staff       (20)      997 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tox.ini
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.182134 unicef-security-1.4.4/
+-rw-r--r--   0 jojo       (501) staff       (20)     2108 2023-06-01 07:30:28.000000 unicef-security-1.4.4/CHANGES
+-rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:23:06.000000 unicef-security-1.4.4/LICENSE
+-rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-security-1.4.4/MANIFEST.in
+-rw-r--r--   0 jojo       (501) staff       (20)     1791 2023-05-05 13:23:06.000000 unicef-security-1.4.4/Makefile
+-rw-r--r--   0 jojo       (501) staff       (20)      611 2023-06-01 07:50:04.182333 unicef-security-1.4.4/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2618 2023-05-05 13:23:06.000000 unicef-security-1.4.4/README.rst
+-rw-r--r--   0 jojo       (501) staff       (20)       82 2023-06-01 07:50:04.183038 unicef-security-1.4.4/setup.cfg
+-rwxr-xr-x   0 jojo       (501) staff       (20)     1921 2023-05-05 13:23:06.000000 unicef-security-1.4.4/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.123567 unicef-security-1.4.4/src/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.145442 unicef-security-1.4.4/src/unicef_security/
+-rw-r--r--   0 jojo       (501) staff       (20)       57 2023-06-01 07:30:28.000000 unicef-security-1.4.4/src/unicef_security/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6144 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)      127 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/apps.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1373 2023-05-11 11:07:37.000000 unicef-security-1.4.4/src/unicef_security/backends.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1023 2023-05-11 13:54:23.000000 unicef-security-1.4.4/src/unicef_security/config.py
+-rw-r--r--   0 jojo       (501) staff       (20)    11070 2023-06-01 07:48:20.000000 unicef-security-1.4.4/src/unicef_security/graph.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2276 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/middleware.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.154676 unicef-security-1.4.4/src/unicef_security/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     7279 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)      454 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/migrations/0002_auto_20201028_0154.py
+-rw-r--r--   0 jojo       (501) staff       (20)      528 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/migrations/0003_auto_20220406_2307.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/migrations/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1314 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3016 2023-06-01 07:30:28.000000 unicef-security-1.4.4/src/unicef_security/pipeline.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.155099 unicef-security-1.4.4/src/unicef_security/templates/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.158654 unicef-security-1.4.4/src/unicef_security/templates/admin/
+-rw-r--r--   0 jojo       (501) staff       (20)      650 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/templates/admin/ad.html
+-rw-r--r--   0 jojo       (501) staff       (20)     1380 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/templates/admin/link_user.html
+-rw-r--r--   0 jojo       (501) staff       (20)      786 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/templates/admin/load_users.html
+-rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/templates/admin/login.html
+-rw-r--r--   0 jojo       (501) staff       (20)     2625 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/templates/unauthorized.html
+-rw-r--r--   0 jojo       (501) staff       (20)      316 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      223 2023-05-05 13:23:06.000000 unicef-security-1.4.4/src/unicef_security/utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)      925 2023-05-11 13:54:23.000000 unicef-security-1.4.4/src/unicef_security/views.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.150791 unicef-security-1.4.4/src/unicef_security.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      611 2023-06-01 07:50:04.000000 unicef-security-1.4.4/src/unicef_security.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1867 2023-06-01 07:50:04.000000 unicef-security-1.4.4/src/unicef_security.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-01 07:50:04.000000 unicef-security-1.4.4/src/unicef_security.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      295 2023-06-01 07:50:04.000000 unicef-security-1.4.4/src/unicef_security.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       16 2023-06-01 07:50:04.000000 unicef-security-1.4.4/src/unicef_security.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.167954 unicef-security-1.4.4/tests/
+-rw-r--r--   0 jojo       (501) staff       (20)      218 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/.coveragerc
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      129 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/conftest.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.170046 unicef-security-1.4.4/tests/demoproject/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.174675 unicef-security-1.4.4/tests/demoproject/demo/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      172 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/admin.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.176317 unicef-security-1.4.4/tests/demoproject/demo/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/migrations/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      138 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2432 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/settings.py
+-rw-r--r--   0 jojo       (501) staff       (20)      210 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/demo/wsgi.py
+-rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/factories.py
+-rwxr-xr-x   0 jojo       (501) staff       (20)      810 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/demoproject/manage.py
+-rw-r--r--   0 jojo       (501) staff       (20)      219 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/fixtures.py
+-rw-r--r--   0 jojo       (501) staff       (20)      208 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/test_admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1095 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/test_azure.py
+-rw-r--r--   0 jojo       (501) staff       (20)      216 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/test_backends.py
+-rw-r--r--   0 jojo       (501) staff       (20)      439 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/test_models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2601 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/test_pipeline.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-01 07:50:04.181469 unicef-security-1.4.4/tests/vcr_cassettes/
+-rw-r--r--   0 jojo       (501) staff       (20)     9126 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/vcr_cassettes/_test_user_data.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/vcr_cassettes/load_business_area.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/vcr_cassettes/load_region.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     2984 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/vcr_cassettes/test_token.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     7655 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/vcr_cassettes/test_user_data.yml
+-rw-r--r--   0 jojo       (501) staff       (20)      823 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tests/vcrpy.py
+-rw-r--r--   0 jojo       (501) staff       (20)      997 2023-05-05 13:23:06.000000 unicef-security-1.4.4/tox.ini
```

### Comparing `unicef-security-1.4.3/CHANGES` & `unicef-security-1.4.4/CHANGES`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Release 1.4.4
+-----------------------------
+* fix create unicef user - new claim
+
+
 Release 1.4.3
 -----------------------------
 * fix logout url
 
 
 Release 1.4.2
 -----------------------------
```

### Comparing `unicef-security-1.4.3/LICENSE` & `unicef-security-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/Makefile` & `unicef-security-1.4.4/Makefile`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/PKG-INFO` & `unicef-security-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-security
-Version: 1.4.3
+Version: 1.4.4
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 Author-email: rapidpro@unicef.org
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `unicef-security-1.4.3/README.rst` & `unicef-security-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/setup.py` & `unicef-security-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/admin.py` & `unicef-security-1.4.4/src/unicef_security/admin.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/backends.py` & `unicef-security-1.4.4/src/unicef_security/backends.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/config.py` & `unicef-security-1.4.4/src/unicef_security/config.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/graph.py` & `unicef-security-1.4.4/src/unicef_security/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,17 @@
                         f"Code {response.status_code}. "
                         f"Error processing the response {response.content}"
                     )
                 break
             except ConnectionError as e:
                 logger.exception(e)
                 raise
+        breakpoint()
 
+        QueryDict
         jresponse = response.json()
         self.next_link = jresponse.get("@odata.nextLink", None)
         self.delta_link = jresponse.get("@odata.deltaLink", None)
         if single:
             return jresponse
         return jresponse.get("value", [])
```

### Comparing `unicef-security-1.4.3/src/unicef_security/middleware.py` & `unicef-security-1.4.4/src/unicef_security/middleware.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/migrations/0001_initial.py` & `unicef-security-1.4.4/src/unicef_security/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/migrations/0003_auto_20220406_2307.py` & `unicef-security-1.4.4/src/unicef_security/migrations/0003_auto_20220406_2307.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/models.py` & `unicef-security-1.4.4/src/unicef_security/models.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/pipeline.py` & `unicef-security-1.4.4/src/unicef_security/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     if not (fields and details.get("email", "").endswith(UNICEF_EMAIL)):
         return
 
     response = kwargs.get("response")
     if response:
         email = response.get("email") or response.get("signInNames.emailAddress")
-        if not email.endswith(UNICEF_EMAIL):
+        if email and not email.endswith(UNICEF_EMAIL):
             return
 
     return {"is_new": True, "user": strategy.create_user(**fields)}
 
 
 def user_details(strategy, details, backend, user=None, *args, **kwargs):
     """This is where we update the user see what the property to map by is here updates_available = False"""
```

### Comparing `unicef-security-1.4.3/src/unicef_security/templates/admin/ad.html` & `unicef-security-1.4.4/src/unicef_security/templates/admin/ad.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/templates/admin/link_user.html` & `unicef-security-1.4.4/src/unicef_security/templates/admin/link_user.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/templates/admin/load_users.html` & `unicef-security-1.4.4/src/unicef_security/templates/admin/load_users.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/templates/unauthorized.html` & `unicef-security-1.4.4/src/unicef_security/templates/unauthorized.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security/views.py` & `unicef-security-1.4.4/src/unicef_security/views.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/src/unicef_security.egg-info/PKG-INFO` & `unicef-security-1.4.4/src/unicef_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-security
-Version: 1.4.3
+Version: 1.4.4
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 Author-email: rapidpro@unicef.org
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `unicef-security-1.4.3/src/unicef_security.egg-info/SOURCES.txt` & `unicef-security-1.4.4/src/unicef_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/demoproject/demo/migrations/0001_initial.py` & `unicef-security-1.4.4/tests/demoproject/demo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/demoproject/demo/settings.py` & `unicef-security-1.4.4/tests/demoproject/demo/settings.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/demoproject/manage.py` & `unicef-security-1.4.4/tests/demoproject/manage.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/test_azure.py` & `unicef-security-1.4.4/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/test_pipeline.py` & `unicef-security-1.4.4/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/vcr_cassettes/_test_user_data.yml` & `unicef-security-1.4.4/tests/vcr_cassettes/_test_user_data.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/vcr_cassettes/load_business_area.yml` & `unicef-security-1.4.4/tests/vcr_cassettes/load_business_area.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/vcr_cassettes/load_region.yml` & `unicef-security-1.4.4/tests/vcr_cassettes/load_region.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/vcr_cassettes/test_token.yml` & `unicef-security-1.4.4/tests/vcr_cassettes/test_token.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/vcr_cassettes/test_user_data.yml` & `unicef-security-1.4.4/tests/vcr_cassettes/test_user_data.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tests/vcrpy.py` & `unicef-security-1.4.4/tests/vcrpy.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.3/tox.ini` & `unicef-security-1.4.4/tox.ini`

 * *Files identical despite different names*

