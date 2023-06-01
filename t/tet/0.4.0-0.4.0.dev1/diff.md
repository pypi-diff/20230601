# Comparing `tmp/tet-0.4.0.tar.gz` & `tmp/tet-0.4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tet-0.4.0.tar", last modified: Thu Jun  1 21:34:07 2023, max compression
+gzip compressed data, was "dist/tet-0.4.0.dev1.tar", last modified: Fri Mar 19 14:33:07 2021, max compression
```

## Comparing `tet-0.4.0.tar` & `tet-0.4.0.dev1.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.106720 tet-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-01 21:33:55.000000 tet-0.4.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (122)     1674 2023-06-01 21:33:55.000000 tet-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-01 21:33:55.000000 tet-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-01 21:34:07.106720 tet-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-01 21:33:55.000000 tet-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-01 21:34:07.106720 tet-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-06-01 21:33:55.000000 tet-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-01 21:33:55.000000 tet-0.4.0/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-01 21:33:55.000000 tet-0.4.0/tet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/config/
--rw-r--r--   0 runner    (1001) docker     (122)     8530 2023-06-01 21:33:55.000000 tet-0.4.0/tet/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/decorators/
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-01 21:33:55.000000 tet-0.4.0/tet/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/i18n/
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-06-01 21:33:55.000000 tet-0.4.0/tet/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/interface/
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-01 21:33:55.000000 tet-0.4.0/tet/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/renderers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 21:33:55.000000 tet-0.4.0/tet/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-06-01 21:33:55.000000 tet-0.4.0/tet/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-06-01 21:33:55.000000 tet-0.4.0/tet/renderers/tonnikala.py
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-01 21:33:55.000000 tet-0.4.0/tet/request.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-01 21:33:55.000000 tet-0.4.0/tet/response.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/security/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 21:33:55.000000 tet-0.4.0/tet/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-01 21:33:55.000000 tet-0.4.0/tet/security/authorization.py
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-01 21:33:55.000000 tet-0.4.0/tet/security/csrf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet/services/
--rw-r--r--   0 runner    (1001) docker     (122)     4507 2023-06-01 21:33:55.000000 tet-0.4.0/tet/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-01 21:33:55.000000 tet-0.4.0/tet/session.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.106720 tet-0.4.0/tet/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 21:33:55.000000 tet-0.4.0/tet/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-06-01 21:33:55.000000 tet-0.4.0/tet/sqlalchemy/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-01 21:33:55.000000 tet-0.4.0/tet/sqlalchemy/password.py
--rw-r--r--   0 runner    (1001) docker     (122)     4968 2023-06-01 21:33:55.000000 tet-0.4.0/tet/sqlalchemy/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.106720 tet-0.4.0/tet/static/
--rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-01 21:33:55.000000 tet-0.4.0/tet/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.106720 tet-0.4.0/tet/util/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/base64.py
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/crypt.py
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/export.py
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/json.py
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-01 21:33:55.000000 tet-0.4.0/tet/util/pshell.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.106720 tet-0.4.0/tet/view/
--rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-06-01 21:33:55.000000 tet-0.4.0/tet/view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.106720 tet-0.4.0/tet/viewlet/
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-06-01 21:33:55.000000 tet-0.4.0/tet/viewlet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.106720 tet-0.4.0/tet/zodb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 21:33:55.000000 tet-0.4.0/tet/zodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-01 21:33:55.000000 tet-0.4.0/tet/zodb/password.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:34:07.102720 tet-0.4.0/tet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-01 21:34:07.000000 tet-0.4.0/tet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-06-01 21:34:07.000000 tet-0.4.0/tet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 21:34:07.000000 tet-0.4.0/tet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 21:34:06.000000 tet-0.4.0/tet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-01 21:34:07.000000 tet-0.4.0/tet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-01 21:34:07.000000 tet-0.4.0/tet.egg-info/top_level.txt
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      470 2021-03-19 14:30:37.000000 tet-0.4.0.dev1/CHANGES.txt
+-rw-r--r--   0 ztane     (1000) ztane     (1000)       60 2017-08-29 07:23:25.000000 tet-0.4.0.dev1/MANIFEST.in
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     2525 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/PKG-INFO
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      494 2017-08-29 07:23:25.000000 tet-0.4.0.dev1/README.txt
+-rw-r--r--   0 ztane     (1000) ztane     (1000)       38 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/setup.cfg
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     1919 2021-03-19 14:32:59.000000 tet-0.4.0.dev1/setup.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.600541 tet-0.4.0.dev1/tet/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)       77 2017-08-29 07:27:44.000000 tet-0.4.0.dev1/tet/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/config/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     8526 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/config/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/decorators/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     1620 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/decorators/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/i18n/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     2028 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/i18n/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/interface/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     1560 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/interface/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/renderers/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/renderers/__init__.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     1812 2017-08-29 07:24:56.000000 tet-0.4.0.dev1/tet/renderers/json.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      278 2017-08-29 07:27:58.000000 tet-0.4.0.dev1/tet/renderers/tonnikala.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)       31 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/request.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)       32 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/response.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/security/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/security/__init__.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     2248 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/security/authorization.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      141 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/security/csrf.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/services/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     4507 2021-03-19 14:29:29.000000 tet-0.4.0.dev1/tet/services/__init__.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      298 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/session.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/sqlalchemy/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/sqlalchemy/__init__.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      397 2017-08-29 07:26:17.000000 tet-0.4.0.dev1/tet/sqlalchemy/factory.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      801 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/sqlalchemy/password.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     4968 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/sqlalchemy/simple.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/static/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     1934 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/static/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/util/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/util/__init__.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     2112 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/base64.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      445 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/collections.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      539 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/crypt.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      262 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/export.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      356 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/json.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      737 2017-08-29 07:25:11.000000 tet-0.4.0.dev1/tet/util/path.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     1355 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/util/pshell.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/tet/view/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     2245 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/view/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/tet/viewlet/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     1401 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/viewlet/__init__.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/tet/zodb/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/zodb/__init__.py
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      413 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/zodb/password.py
+drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet.egg-info/
+-rw-r--r--   0 ztane     (1000) ztane     (1000)     2525 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/PKG-INFO
+-rw-r--r--   0 ztane     (1000) ztane     (1000)      907 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/SOURCES.txt
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        1 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/dependency_links.txt
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        1 2017-08-29 07:32:39.000000 tet-0.4.0.dev1/tet.egg-info/not-zip-safe
+-rw-r--r--   0 ztane     (1000) ztane     (1000)       49 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/requires.txt
+-rw-r--r--   0 ztane     (1000) ztane     (1000)        4 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/top_level.txt
```

### Comparing `tet-0.4.0/PKG-INFO` & `tet-0.4.0.dev1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,67 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: tet
-Version: 0.4.0
+Version: 0.4.0.dev1
 Summary: Unearthly intelligent batteries-included application framework built on Pyramid
 Home-page: http://www.anttipatterns.com
 Author: Antti Haapala
 Author-email: antti.haapala@anttipatterns.com
+License: UNKNOWN
+Description: tet
+        ===
+        
+        Unearthly intelligent batteries-included application framework built on Pyramid
+        
+        
+        How to install
+        --------------
+        
+            git clone https://github.com/ztane/tet.git
+            cd tet
+            python setup.py develop
+        
+        
+        What do you get out of the box
+        ------------------------------
+        
+        1. Awesome scaffold(s):
+        
+                pcreate -s basictet MyProject
+                cd MyProject
+                python setup.py develop
+                initialize_myproject_db development.ini
+                # go to http://localhost://6543 and feel awesome
+        
+        
+        2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+        
+            * The tet.di request scoped services are now truly instantiated per request!
+        
+        2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+        
+            * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
+              fixed backports.typing to greater than or equal to 1.1.
+        
+        2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
+        
+            * renamed the package to `tet`
+        
+        
 Keywords: web wsgi bfg pylons pyramid
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Provides-Extra: dev
-License-File: LICENSE
-
-# tet
-
-Unearthly intelligent batteries-included application framework built on Pyramid
-
-
-## How to install
-
-```
-pip install tet
-```
-
-
-# Changes
-
-
-2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-
-    * The tet.di request scoped services are now truly instantiated per request!
-
-2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-
-    * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
-      fixed backports.typing to greater than or equal to 1.1.
-
-2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
-
-    * renamed the package to `tet`
-
```

### Comparing `tet-0.4.0/setup.py` & `tet-0.4.0.dev1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-from pathlib import Path
+import os, sys
 
-from setuptools import find_packages, setup
+from setuptools import setup, find_packages
 
-here = Path(__file__).parent
-README = (here / "README.md").read_text()
-CHANGES = (here / "CHANGES.md").read_text()
+here = os.path.abspath(os.path.dirname(__file__))
 
+def readfile(name):
+    with open(os.path.join(here, name)) as f:
+        return f.read()
+
+README = readfile('README.txt')
+CHANGES = readfile('CHANGES.txt')
 
 requires = """
     pyramid>=1.9
     passlib
-    sqlalchemy<2.0
+    sqlalchemy
     pyramid_services
 """.split()
 
-dev_requires = ["pytest"]
+if sys.version_info < (3, 5, 2):
+    requires.append('backports.typing>=1.1,<1.2')
+
 
-setup(
-    name="tet",
-    version="0.4.0",
-    description="Unearthly intelligent batteries-included application framework built on Pyramid",
-    long_description=README + "\n\n" + CHANGES,
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Framework :: Pyramid",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: Python Software Foundation License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3 :: Only",
-        "Topic :: Internet :: WWW/HTTP :: WSGI",
-        "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
-        "Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware",
-        "Topic :: Software Development :: Libraries :: Application Frameworks",
-    ],
-    author="Antti Haapala",
-    author_email="antti.haapala@anttipatterns.com",
-    url="http://www.anttipatterns.com",
-    keywords="web wsgi bfg pylons pyramid",
-    packages=find_packages(),
-    include_package_data=True,
-    zip_safe=False,
-    test_suite="tet",
-    install_requires=requires,
-    extras_require={"dev": dev_requires},
+setup(name='tet',
+      version='0.4.0.dev1',
+      description='Unearthly intelligent batteries-included application framework built on Pyramid',
+      long_description=README + '\n\n' + CHANGES,
+      classifiers=[
+          "Development Status :: 4 - Beta",
+          "Framework :: Pyramid",
+          "Intended Audience :: Developers",
+          "License :: OSI Approved :: Python Software Foundation License",
+          "Programming Language :: Python :: 3.3",
+          "Programming Language :: Python :: 3.4",
+          "Programming Language :: Python :: 3.5",
+          "Programming Language :: Python :: 3.6",
+          "Programming Language :: Python :: 3.7",
+          "Programming Language :: Python :: 3.8",
+          "Programming Language :: Python :: 3.9",
+          "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3 :: Only",
+          "Topic :: Internet :: WWW/HTTP :: WSGI",
+          "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
+          "Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware",
+          "Topic :: Software Development :: Libraries :: Application Frameworks"
+      ],
+      author='Antti Haapala',
+      author_email='antti.haapala@anttipatterns.com',
+      url='http://www.anttipatterns.com',
+      keywords='web wsgi bfg pylons pyramid',
+      packages=find_packages(),
+      include_package_data=True,
+      zip_safe=False,
+      test_suite='tet',
+      install_requires=requires,
 )
```

### Comparing `tet-0.4.0/tet/config/__init__.py` & `tet-0.4.0.dev1/tet/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 raise
 
     return config
 
 
 def application_factory(factory_function: Callable[[Configurator], Any]=None,
                         configure_only=False,
-                        included_features=MINIMAL_FEATURES,
+                        included_features=ALL_FEATURES,
                         excluded_features=(),
                         package=None,
                         **extra_parameters):
     """
     A decorator for main method / application configurator for Tet. The
     wrapped function must accept a single argument - the Configurator. The
     wrapper itself accepts arguments (global_config, **settings) like an
```

### Comparing `tet-0.4.0/tet/decorators/__init__.py` & `tet-0.4.0.dev1/tet/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/i18n/__init__.py` & `tet-0.4.0.dev1/tet/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/interface/__init__.py` & `tet-0.4.0.dev1/tet/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/renderers/json.py` & `tet-0.4.0.dev1/tet/renderers/json.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/security/authorization.py` & `tet-0.4.0.dev1/tet/security/authorization.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/services/__init__.py` & `tet-0.4.0.dev1/tet/services/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/sqlalchemy/password.py` & `tet-0.4.0.dev1/tet/sqlalchemy/password.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/sqlalchemy/simple.py` & `tet-0.4.0.dev1/tet/sqlalchemy/simple.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/static/__init__.py` & `tet-0.4.0.dev1/tet/static/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/util/base64.py` & `tet-0.4.0.dev1/tet/util/base64.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/util/crypt.py` & `tet-0.4.0.dev1/tet/util/crypt.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/util/path.py` & `tet-0.4.0.dev1/tet/util/path.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/util/pshell.py` & `tet-0.4.0.dev1/tet/util/pshell.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/view/__init__.py` & `tet-0.4.0.dev1/tet/view/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet/viewlet/__init__.py` & `tet-0.4.0.dev1/tet/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0/tet.egg-info/PKG-INFO` & `tet-0.4.0.dev1/tet.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,67 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: tet
-Version: 0.4.0
+Version: 0.4.0.dev1
 Summary: Unearthly intelligent batteries-included application framework built on Pyramid
 Home-page: http://www.anttipatterns.com
 Author: Antti Haapala
 Author-email: antti.haapala@anttipatterns.com
+License: UNKNOWN
+Description: tet
+        ===
+        
+        Unearthly intelligent batteries-included application framework built on Pyramid
+        
+        
+        How to install
+        --------------
+        
+            git clone https://github.com/ztane/tet.git
+            cd tet
+            python setup.py develop
+        
+        
+        What do you get out of the box
+        ------------------------------
+        
+        1. Awesome scaffold(s):
+        
+                pcreate -s basictet MyProject
+                cd MyProject
+                python setup.py develop
+                initialize_myproject_db development.ini
+                # go to http://localhost://6543 and feel awesome
+        
+        
+        2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+        
+            * The tet.di request scoped services are now truly instantiated per request!
+        
+        2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+        
+            * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
+              fixed backports.typing to greater than or equal to 1.1.
+        
+        2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
+        
+            * renamed the package to `tet`
+        
+        
 Keywords: web wsgi bfg pylons pyramid
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Provides-Extra: dev
-License-File: LICENSE
-
-# tet
-
-Unearthly intelligent batteries-included application framework built on Pyramid
-
-
-## How to install
-
-```
-pip install tet
-```
-
-
-# Changes
-
-
-2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-
-    * The tet.di request scoped services are now truly instantiated per request!
-
-2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-
-    * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
-      fixed backports.typing to greater than or equal to 1.1.
-
-2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
-
-    * renamed the package to `tet`
-
```

### Comparing `tet-0.4.0/tet.egg-info/SOURCES.txt` & `tet-0.4.0.dev1/tet.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-CHANGES.md
-LICENSE
+CHANGES.txt
 MANIFEST.in
-README.md
-setup.cfg
+README.txt
 setup.py
-tests/test_integration.py
 tet/__init__.py
 tet/request.py
 tet/response.py
 tet/session.py
 tet.egg-info/PKG-INFO
 tet.egg-info/SOURCES.txt
 tet.egg-info/dependency_links.txt
```

