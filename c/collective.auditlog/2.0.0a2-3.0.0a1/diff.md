# Comparing `tmp/collective.auditlog-2.0.0a2.tar.gz` & `tmp/collective.auditlog-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.auditlog-2.0.0a2.tar", last modified: Thu Mar 19 14:32:44 2020, max compression
+gzip compressed data, was "collective.auditlog-3.0.0a1.tar", last modified: Thu Jun  1 07:42:01 2023, max compression
```

## Comparing `collective.auditlog-2.0.0a2.tar` & `collective.auditlog-3.0.0a1.tar`

### file list

```diff
@@ -1,64 +1,69 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/
--rw-rw-r--   0 ale       (1000) ale       (1000)       63 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/MANIFEST.in
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)    13932 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)       11 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/namespace_packages.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1815 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      152 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/entry_points.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)      160 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       11 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective.auditlog.egg-info/top_level.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)    13932 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     1576 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/setup.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2295 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/CHANGES.rst
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/
--rw-rw-r--   0 ale       (1000) ale       (1000)       56 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/
--rw-rw-r--   0 ale       (1000) ale       (1000)     3879 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/catalog.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)     5725 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tests/test_actions.py
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tests/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2651 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/browser.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3958 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/td.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      855 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/models.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      336 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/tasks.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      326 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/permissions.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     4339 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1302 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.pt
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/
--rw-rw-r--   0 ale       (1000) ale       (1000)      326 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/to1001.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1957 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)       15 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/upgrades/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1126 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3705 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/handlers.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      399 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1121 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/asyncqueue.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4501 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/utils.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/locales/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1237 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/locales/collective.auditlog.pot
--rw-rw-r--   0 ale       (1000) ale       (1000)     1060 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/action.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     4123 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/logview.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)     2183 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1853 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/db.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/static/
--rw-rw-r--   0 ale       (1000) ale       (1000)    37031 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/static/infinitescroll.jquery.js
--rw-rw-r--   0 ale       (1000) ale       (1000)      330 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/permissions.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4978 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/interfaces.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1293 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/testing.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/
--rw-rw-r--   0 ale       (1000) ale       (1000)      170 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/metadata.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      355 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/rolemap.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      554 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/controlpanel.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      153 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/toolset.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)     7436 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/contentrules.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      819 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/actions.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      120 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/registry.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)     8638 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/collective/auditlog/action.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/
--rw-rw-r--   0 ale       (1000) ale       (1000)      736 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/LICENSE.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1504 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/INSTALL.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)    17987 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/docs/LICENSE.GPL
--rw-rw-r--   0 ale       (1000) ale       (1000)      435 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     8178 2020-03-19 14:32:44.000000 collective.auditlog-2.0.0a2/README.rst
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       72 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/.coveragerc
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2640 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/CHANGES.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)       98 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11591 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8178 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/README.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1288 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/base.cfg
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.249356 collective.auditlog-3.0.0a1/collective/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       56 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/collective/auditlog/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1090 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8564 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/action.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1060 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/action.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1121 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/asyncqueue.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2628 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/browser.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3875 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/catalog.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4339 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1331 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/controlpanel.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2103 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/controlpanel.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1813 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/db.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3823 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/handlers.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4936 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/interfaces.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/collective/auditlog/locales/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1237 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/locales/collective.auditlog.pot
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4069 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/logview.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      855 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/models.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      306 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/permissions.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      326 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/permissions.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.249356 collective.auditlog-3.0.0a1/collective/auditlog/profiles/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      836 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/actions.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7323 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/contentrules.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      570 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/controlpanel.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      187 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      137 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/registry.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      372 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/rolemap.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      170 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/toolset.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      398 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/profiles.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/collective/auditlog/static/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    37015 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/static/infinitescroll.jquery.js
+-rw-rw-r--   0 ale       (1000) ale       (1000)      328 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/tasks.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3976 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/td.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1278 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/testing.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/collective/auditlog/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/tests/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5553 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/tests/test_actions.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/collective/auditlog/upgrades/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/upgrades/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1957 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/upgrades/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      306 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/upgrades/to1001.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4477 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective/auditlog/utils.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.249356 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    11591 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1875 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       90 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/namespace_packages.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      168 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/collective.auditlog.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/docs/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1504 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/docs/INSTALL.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17987 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/docs/LICENSE.GPL
+-rw-rw-r--   0 ale       (1000) ale       (1000)      736 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/docs/LICENSE.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3803 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/requirements.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2023-06-01 07:42:01.253356 collective.auditlog-3.0.0a1/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1767 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/setup.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      155 2023-06-01 07:42:01.000000 collective.auditlog-3.0.0a1/test_plone52.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.auditlog-2.0.0a2/collective.auditlog.egg-info/PKG-INFO` & `collective.auditlog-3.0.0a1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,367 +1,393 @@
 Metadata-Version: 2.1
 Name: collective.auditlog
-Version: 2.0.0a2
+Version: 3.0.0a1
 Summary: Provides extra conditions and triggers for all content actions
 Home-page: http://svn.plone.org/svn/collective/
 Author: rain2o
 Author-email: Joel@rain2odesigns.com
 License: GPL
-Description: Introduction
-        ============
-        
-        The package allows you to audit actions being done on your site.
-        It accomplishes this by using configurable content rules.
-        
-        By default, after you activate this package,
-        it will create all the content rules
-        that can be used for auditing with only the Page type to audit OOTB.
-        If you want to audit more types of objects,
-        you will need to configure the content rules.
-        
-        The audits are stored into a relational database.
-        Once installed and called for the first time
-        it will create a table called "audit" if it does not already exist,
-        so there is no need to create the table manually.
-        
-        AuditLog attempts to use plone.app.async or collective.celery to
-        perform the store actions, but if that fails it will finish the task
-        directly. The advantage of this is to allow an individual 'worker'
-        client to run Async and handle all of these request.
-        If there is a lot of activity it will not get backed up.
-        Async queues the job up and handles it as it can
-        while the users request finishes and moves on
-        avoiding sacrifices in performance.
-        Refer to the collective.async pypi page
-        for instructions on setting it up if you use it.
-        Async is NOT required for AuditLog to work,
-        however it is advised, especially for high traffic sites.
-        
-        
-        Installation
-        ============
-        
-        Download the package from GitHub and extract into your src directory.
-        Add 'collective.auditlog' to your eggs and zcml slugs in buildout.
-        Include the location (src/collective.auditlog) in development slugs too.
-        Run buildout
-        
-        In Site Setup -> Add-ons, active Audit Log.
-        Once it is installed you will see "AuditLog" under Add-on Configuration.
-        This is where you can configuration the relational database.
-        The configuration string needs to be a valid SQLAlchemy connection string.
-        The control panel also allows you to enable/disable
-        tracking of actions performed on working copies.
-        
-        All that is left is to configure the new Content Rules
-        to track the content types and actions you desire.
-        
-        Upgrading
-        =========
-        
-        If you are upgrading from an older version, you will need to run the
-        upgrade steps from the add-ons control panel.
-        
-        USAGE
-        =====
-        For now, collective.auditlog uses SQLAlchemy for storing data. To use
-        postgres, it's necessary to add the 'psycopg2' egg to the buildout. Once
-        the product is installed, add the correct connection URL to the product
-        setup. Example::
-        
-            postgresql://enfold:enfold@localhost/auditlog
-        
-        By default, collective.auditlog uses content rules to define which events
-        to capture. An additional mechanism has been added that allows the site to
-        automatically log the various events supported by collective.auditlog.
-        Simply choose from the picklist in the config for this to work. If no
-        events are selected, no logging will occur.
-        
-        It is possible to log custom events from application code by using the
-        AuditableActionPerformedEvent, like this::
-        
-            from zope event import notify
-            from collective.auditlog.interfaces import AuditableActionPerformedEvent
-            notify(AuditableActionPerformedEvent(obj, request, "action", "note"))
-        
-        'obj', refers to the affected content object; 'request' is the current zope
-        request, 'action' and 'note' correspond to the logged action and its
-        description, respectively. All parameters are required, but everything
-        except obj can be set to None if no value is available.
-        
-        In addition to control panel configuration, connection parameters can be
-        set using the zope-conf-additional directive in the buildout. Note that
-        this will take precedence over any control panel configuration. Example::
-        
-            zope-conf-additional =
-                <product-config collective.auditlog>
-                    audit-connection-string postgres://enfold:enfold@localhost/auditlog
-                    audit-connection-params {"pool_recycle": 3600, "echo": true}
-                </product-config>
-        
-        There is now a view for the audit log entries, located at @@auditlog-view.
-        There is no link to it from the control panel at the moment. The view uses
-        infinite scrollong rather than pagination for looking at the logs.
-        
-        Searching the audit log
-        =======================
-        
-        Audit logs are stored in a SQL table, so you can use any SQL database tool
-        to analyse the audit log. However, sometimes you may need to query the logs
-        in the context of the Plone objects that generated them, for which the
-        information stored in SQL is not enough. For this purpose,
-        collective.auditlog offers a catalog based mechanism which can be used to
-        query the logs using any Plone based indexes available at the time of
-        logging. This can be used, for example, to develop a portlet that shows the
-        latest documents that have been modified.
-        
-        To enable catalog-based logging, choose sql+zodb storage in the audit log
-        control panel. Information will still be stored in the SQL database, but
-        a special catalog will be enabled to store plone indexing information as
-        well.
-        
-        Once this storage is enabled, you can search the logs using a catalog-like
-        query::
-        
-            from datetime import datetime
-            from collective.auditlog.catalog import searchAudited
-        
-            from = datatime(2018,6,1)
-            to = datetime(2018,12,31)
-            query = {'portal_type': 'Document',
-                    'review_state': 'published'}
-            audited = searchAudited(from_date=from,
-                                    to_date=to,
-                                    actions=['added', 'modified'],
-                                    **query)
-        
-        All of the parameters are optional, but an empty query will return all
-        indexed objects, so use with care.
-        
-        Note that the query will return catalog records, and any documents that have
-        multiple actions performed in the selected date range, will only appear once
-        in the list. There are also catalog records for deleted items, so a query
-        can be made to look for those even if they are gone from Plone.
-        
-        
-        Celery Integration
-        ==================
-        The collective.celery package requires adding the celery and
-        collective.celery eggs to the mian buildout section eggs. Example::
-        
-            eggs =
-                celery
-                Plone
-                collective.celery
-        
-        We still use the celery-broker part, for clarity. The celery part is
-        still required, but is simpler::
-        
-            [celery-broker]
-            host = 127.0.0.1
-            port = 6379
-        
-            [celery]
-            recipe = zc.recipe.egg
-            environment-vars = ${buildout:environment-vars}
-            eggs =
-                ${buildout:eggs}
-                flower
-            scripts = pcelery flower
-        
-        The celery part depends on having some variables added to the main
-        environment-vars section::
-        
-            environment-vars =
-                CELERY_BROKER_URL redis://${celery-broker:host}:${celery-broker:port}
-                CELERY_RESULT_BACKEND redis://${celery-broker:host}:${celery-broker:port}
-                CELERY_TASKS collective.es.index.tasks
-        
-        Additional Zope configuration
-        -----------------------------
-        
-        There's now a hook in collective.celery for carrying out additional zope
-        configuration before running the tasks. If the tasks module contains an
-        'extra_config' method, it is passed the zope startup object at worker
-        initialization time. This is used by collective.es.index to run the
-        elasticsearch configuration method.
-        
-        Monitoring celery tasks
-        -----------------------
-        
-        Celery needs to be started as an independent process. It's recommended to
-        use supervisord for this. To try it out from the command line, you can run
-        use supervisord for this. To try it out from the command line, you can run
-        "bin/pcelery worker" from the buildout directory. Note that the script is
-        now named 'pcelery' and it needs a path to the zope configuration. Example::
-        
-            $ bin/pcelery worker parts/client1/etc/zope.conf
-        
-        Flower is included in this setup. Run "bin/flower" from the buildout
-        directory and consult the dashboard at http://localhost:5555 using a
-        browser. Note that the broker is now a requried parameter::
-        
-            $ bin/flower --broker redis://127.0.0.1:6379
-        
-        Dependencies
-        ============
-        
-        All dependencies are installed automatically
-        when installing collective.auditlog.
-        Here is just a list of those for reference:
-        
-        - setuptools
-        - sqlalchemy
-        - five.globalrequest
-        - plone.app.async [OPTIONAL]
-        - collective.celery [OPTIONAL]
-        
-        Authors
-        =======
-        
-        - Joel Rainwater, initial author
-        - Nathan van Gheem, Async integration, bug fixes, optimization.
-        - Alessandro Pisa, bug fixing, testing
-        - Enfold Systems, celery integration and audit view
-        
-        
-        Changelog
-        =========
-        
-        2.0.0a2 (2020-03-19)
-        --------------------
-        
-        - Fix request not having an environment attribute in instance scripts
-          [ale-rt]
-        
-        
-        2.0.0a1 (2020-03-11)
-        --------------------
-        
-        - Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
-          [thet]
-        
-        - Remove deprecations.
-          action.canExecute is renamed to ``can_execute``, takes no paramters and is a property.
-          [thet]
-        
-        - Python 3 compatibility.
-          [thet]
-        
-        - Remove support for plone.app.async.
-          Due to  ``async`` being a reserved word, this cannot made Python 3 compatible.
-          Use collective.celeries instead.
-          [thet]
-        
-        - Drop support for Archetypes.
-          [thet]
-        
-        - Plone 5.2 compatibility.
-          Drop Support for Plone 5.0 and 4.3 (Both are missing zope.interface.interfaces.IObjectEvent).
-          [thet]
-        
-        - Make Arhcetype a soft dependency.
-          [ale-rt]
-        
-        - Align with Plone code style: black, isort.
-          [thet]
-        
-        - Fix soft dependency on formlib (#22)
-          [ale-rt]
-        
-        - Speed up rule retrieval
-          [ale-rt]
-        
-        - Added some memoized properties and methods to the `AuditActionExecutor` class
-          for easier customization
-          [ale-rt]
-        
-        - collective.celery integration
-          [enfold]
-        
-        - @@auditlog-view allows viewing/sorting/searching audit log entries
-          [enfold]
-        
-        - add login & logout audits
-          [enfold]
-        
-        - ability to specify the sqlalchemy DSN in config file
-          [enfold]
-        
-        - Notify an event before storing audit log entry.
-          [enfold]
-        
-        - Use custom permission for viewing audit log.
-          [enfold]
-        
-        - Fix tests.
-          [enfold]
-        
-        - Fix db connection leak.
-          [enfold]
-        
-        - Use valid json in info field.
-          [enfold]
-        
-        
-        1.3.3 (2018-07-12)
-        ------------------
-        
-        - Factored out getObjectInfo and addLogEntry.
-          [reinhardt]
-        
-        
-        1.3.2 (2018-07-11)
-        ------------------
-        
-        - Skip retrieving rule when audit log is disabled completely.
-          Improves performance.
-          [reinhardt]
-        
-        
-        1.3.1 (2017-04-13)
-        ------------------
-        
-        - Fix upgrade step title.
-          [ale-rt]
-        
-        
-        1.3.0 (2017-04-13)
-        ------------------
-        
-        - The engine parameters (like pool_recycle, echo, ...)
-          can be specified through a registry record
-          [ale-rt]
-        
-        
-        1.2.2 (2016-06-06)
-        ------------------
-        
-        - Make action more robust on IActionSucceededEvent
-          [ale-rt]
-        
-        
-        1.2.1 (2016-05-10)
-        ------------------
-        
-        - Fix unicode issues
-        - Tests are working again
-          [ale-rt]
-        
-        
-        1.2.0 (2016-05-03)
-        ------------------
-        
-        - First public release
-        
 Keywords: Plone Audit Log
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: Addon
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Provides-Extra: celery
 Provides-Extra: test
+
+Introduction
+============
+
+The package allows you to audit actions being done on your site.
+It accomplishes this by using configurable content rules.
+
+By default, after you activate this package,
+it will create all the content rules
+that can be used for auditing with only the Page type to audit OOTB.
+If you want to audit more types of objects,
+you will need to configure the content rules.
+
+The audits are stored into a relational database.
+Once installed and called for the first time
+it will create a table called "audit" if it does not already exist,
+so there is no need to create the table manually.
+
+AuditLog attempts to use plone.app.async or collective.celery to
+perform the store actions, but if that fails it will finish the task
+directly. The advantage of this is to allow an individual 'worker'
+client to run Async and handle all of these request.
+If there is a lot of activity it will not get backed up.
+Async queues the job up and handles it as it can
+while the users request finishes and moves on
+avoiding sacrifices in performance.
+Refer to the collective.async pypi page
+for instructions on setting it up if you use it.
+Async is NOT required for AuditLog to work,
+however it is advised, especially for high traffic sites.
+
+
+Installation
+============
+
+Download the package from GitHub and extract into your src directory.
+Add 'collective.auditlog' to your eggs and zcml slugs in buildout.
+Include the location (src/collective.auditlog) in development slugs too.
+Run buildout
+
+In Site Setup -> Add-ons, active Audit Log.
+Once it is installed you will see "AuditLog" under Add-on Configuration.
+This is where you can configuration the relational database.
+The configuration string needs to be a valid SQLAlchemy connection string.
+The control panel also allows you to enable/disable
+tracking of actions performed on working copies.
+
+All that is left is to configure the new Content Rules
+to track the content types and actions you desire.
+
+Upgrading
+=========
+
+If you are upgrading from an older version, you will need to run the
+upgrade steps from the add-ons control panel.
+
+USAGE
+=====
+For now, collective.auditlog uses SQLAlchemy for storing data. To use
+postgres, it's necessary to add the 'psycopg2' egg to the buildout. Once
+the product is installed, add the correct connection URL to the product
+setup. Example::
+
+    postgresql://enfold:enfold@localhost/auditlog
+
+By default, collective.auditlog uses content rules to define which events
+to capture. An additional mechanism has been added that allows the site to
+automatically log the various events supported by collective.auditlog.
+Simply choose from the picklist in the config for this to work. If no
+events are selected, no logging will occur.
+
+It is possible to log custom events from application code by using the
+AuditableActionPerformedEvent, like this::
+
+    from zope event import notify
+    from collective.auditlog.interfaces import AuditableActionPerformedEvent
+    notify(AuditableActionPerformedEvent(obj, request, "action", "note"))
+
+'obj', refers to the affected content object; 'request' is the current zope
+request, 'action' and 'note' correspond to the logged action and its
+description, respectively. All parameters are required, but everything
+except obj can be set to None if no value is available.
+
+In addition to control panel configuration, connection parameters can be
+set using the zope-conf-additional directive in the buildout. Note that
+this will take precedence over any control panel configuration. Example::
+
+    zope-conf-additional =
+        <product-config collective.auditlog>
+            audit-connection-string postgres://enfold:enfold@localhost/auditlog
+            audit-connection-params {"pool_recycle": 3600, "echo": true}
+        </product-config>
+
+There is now a view for the audit log entries, located at @@auditlog-view.
+There is no link to it from the control panel at the moment. The view uses
+infinite scrollong rather than pagination for looking at the logs.
+
+Searching the audit log
+=======================
+
+Audit logs are stored in a SQL table, so you can use any SQL database tool
+to analyse the audit log. However, sometimes you may need to query the logs
+in the context of the Plone objects that generated them, for which the
+information stored in SQL is not enough. For this purpose,
+collective.auditlog offers a catalog based mechanism which can be used to
+query the logs using any Plone based indexes available at the time of
+logging. This can be used, for example, to develop a portlet that shows the
+latest documents that have been modified.
+
+To enable catalog-based logging, choose sql+zodb storage in the audit log
+control panel. Information will still be stored in the SQL database, but
+a special catalog will be enabled to store plone indexing information as
+well.
+
+Once this storage is enabled, you can search the logs using a catalog-like
+query::
+
+    from datetime import datetime
+    from collective.auditlog.catalog import searchAudited
+
+    from = datatime(2018,6,1)
+    to = datetime(2018,12,31)
+    query = {'portal_type': 'Document',
+            'review_state': 'published'}
+    audited = searchAudited(from_date=from,
+                            to_date=to,
+                            actions=['added', 'modified'],
+                            **query)
+
+All of the parameters are optional, but an empty query will return all
+indexed objects, so use with care.
+
+Note that the query will return catalog records, and any documents that have
+multiple actions performed in the selected date range, will only appear once
+in the list. There are also catalog records for deleted items, so a query
+can be made to look for those even if they are gone from Plone.
+
+
+Celery Integration
+==================
+The collective.celery package requires adding the celery and
+collective.celery eggs to the mian buildout section eggs. Example::
+
+    eggs =
+        celery
+        Plone
+        collective.celery
+
+We still use the celery-broker part, for clarity. The celery part is
+still required, but is simpler::
+
+    [celery-broker]
+    host = 127.0.0.1
+    port = 6379
+
+    [celery]
+    recipe = zc.recipe.egg
+    environment-vars = ${buildout:environment-vars}
+    eggs =
+        ${buildout:eggs}
+        flower
+    scripts = pcelery flower
+
+The celery part depends on having some variables added to the main
+environment-vars section::
+
+    environment-vars =
+        CELERY_BROKER_URL redis://${celery-broker:host}:${celery-broker:port}
+        CELERY_RESULT_BACKEND redis://${celery-broker:host}:${celery-broker:port}
+        CELERY_TASKS collective.es.index.tasks
+
+Additional Zope configuration
+-----------------------------
+
+There's now a hook in collective.celery for carrying out additional zope
+configuration before running the tasks. If the tasks module contains an
+'extra_config' method, it is passed the zope startup object at worker
+initialization time. This is used by collective.es.index to run the
+elasticsearch configuration method.
+
+Monitoring celery tasks
+-----------------------
+
+Celery needs to be started as an independent process. It's recommended to
+use supervisord for this. To try it out from the command line, you can run
+use supervisord for this. To try it out from the command line, you can run
+"bin/pcelery worker" from the buildout directory. Note that the script is
+now named 'pcelery' and it needs a path to the zope configuration. Example::
+
+    $ bin/pcelery worker parts/client1/etc/zope.conf
+
+Flower is included in this setup. Run "bin/flower" from the buildout
+directory and consult the dashboard at http://localhost:5555 using a
+browser. Note that the broker is now a required parameter::
+
+    $ bin/flower --broker redis://127.0.0.1:6379
+
+Dependencies
+============
+
+All dependencies are installed automatically
+when installing collective.auditlog.
+Here is just a list of those for reference:
+
+- setuptools
+- sqlalchemy
+- five.globalrequest
+- plone.app.async [OPTIONAL]
+- collective.celery [OPTIONAL]
+
+Authors
+=======
+
+- Joel Rainwater, initial author
+- Nathan van Gheem, Async integration, bug fixes, optimization.
+- Alessandro Pisa, bug fixing, testing
+- Enfold Systems, celery integration and audit view
+
+
+3.0.0a1 (2023-06-01)
+--------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c)
+
+
+Changelog
+=========
+
+3.0.0a1 (unreleased)
+--------------------
+
+- Drop Python 2.7
+- Use SQLAlchemy 1.4
+  [ale-rt]
+
+2.0.0 (2023-05-31)
+------------------
+
+- Re-release 2.0.0a2 as 2.0.0.
+  This will be the last release supporting Python2.7.
+  [ale-rt]
+
+
+2.0.0a2 (2020-03-19)
+--------------------
+
+- Fix request not having an environment attribute in instance scripts
+  [ale-rt]
+
+
+2.0.0a1 (2020-03-11)
+--------------------
+
+- Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
+  [thet]
+
+- Remove deprecations.
+  action.canExecute is renamed to ``can_execute``, takes no parameters and is a property.
+  [thet]
+
+- Python 3 compatibility.
+  [thet]
+
+- Remove support for plone.app.async.
+  Due to  ``async`` being a reserved word, this cannot made Python 3 compatible.
+  Use collective.celeries instead.
+  [thet]
+
+- Drop support for Archetypes.
+  [thet]
+
+- Plone 5.2 compatibility.
+  Drop Support for Plone 5.0 and 4.3 (Both are missing zope.interface.interfaces.IObjectEvent).
+  [thet]
+
+- Make Arhcetype a soft dependency.
+  [ale-rt]
+
+- Align with Plone code style: black, isort.
+  [thet]
+
+- Fix soft dependency on formlib (#22)
+  [ale-rt]
+
+- Speed up rule retrieval
+  [ale-rt]
+
+- Added some memoized properties and methods to the `AuditActionExecutor` class
+  for easier customization
+  [ale-rt]
+
+- collective.celery integration
+  [enfold]
+
+- @@auditlog-view allows viewing/sorting/searching audit log entries
+  [enfold]
+
+- add login & logout audits
+  [enfold]
+
+- ability to specify the sqlalchemy DSN in config file
+  [enfold]
+
+- Notify an event before storing audit log entry.
+  [enfold]
+
+- Use custom permission for viewing audit log.
+  [enfold]
+
+- Fix tests.
+  [enfold]
+
+- Fix db connection leak.
+  [enfold]
+
+- Use valid json in info field.
+  [enfold]
+
+
+1.3.3 (2018-07-12)
+------------------
+
+- Factored out getObjectInfo and addLogEntry.
+  [reinhardt]
+
+
+1.3.2 (2018-07-11)
+------------------
+
+- Skip retrieving rule when audit log is disabled completely.
+  Improves performance.
+  [reinhardt]
+
+
+1.3.1 (2017-04-13)
+------------------
+
+- Fix upgrade step title.
+  [ale-rt]
+
+
+1.3.0 (2017-04-13)
+------------------
+
+- The engine parameters (like pool_recycle, echo, ...)
+  can be specified through a registry record
+  [ale-rt]
+
+
+1.2.2 (2016-06-06)
+------------------
+
+- Make action more robust on IActionSucceededEvent
+  [ale-rt]
+
+
+1.2.1 (2016-05-10)
+------------------
+
+- Fix unicode issues
+- Tests are working again
+  [ale-rt]
+
+
+1.2.0 (2016-05-03)
+------------------
+
+- First public release
```

### Comparing `collective.auditlog-2.0.0a2/collective.auditlog.egg-info/SOURCES.txt` & `collective.auditlog-3.0.0a1/collective.auditlog.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+.coveragerc
 CHANGES.rst
 MANIFEST.in
 README.rst
-setup.cfg
+base.cfg
+pyproject.toml
+requirements.txt
 setup.py
+test_plone52.cfg
 collective/__init__.py
 collective.auditlog.egg-info/PKG-INFO
 collective.auditlog.egg-info/SOURCES.txt
 collective.auditlog.egg-info/dependency_links.txt
 collective.auditlog.egg-info/entry_points.txt
 collective.auditlog.egg-info/namespace_packages.txt
 collective.auditlog.egg-info/not-zip-safe
```

### Comparing `collective.auditlog-2.0.0a2/PKG-INFO` & `collective.auditlog-3.0.0a1/collective.auditlog.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,367 +1,393 @@
 Metadata-Version: 2.1
 Name: collective.auditlog
-Version: 2.0.0a2
+Version: 3.0.0a1
 Summary: Provides extra conditions and triggers for all content actions
 Home-page: http://svn.plone.org/svn/collective/
 Author: rain2o
 Author-email: Joel@rain2odesigns.com
 License: GPL
-Description: Introduction
-        ============
-        
-        The package allows you to audit actions being done on your site.
-        It accomplishes this by using configurable content rules.
-        
-        By default, after you activate this package,
-        it will create all the content rules
-        that can be used for auditing with only the Page type to audit OOTB.
-        If you want to audit more types of objects,
-        you will need to configure the content rules.
-        
-        The audits are stored into a relational database.
-        Once installed and called for the first time
-        it will create a table called "audit" if it does not already exist,
-        so there is no need to create the table manually.
-        
-        AuditLog attempts to use plone.app.async or collective.celery to
-        perform the store actions, but if that fails it will finish the task
-        directly. The advantage of this is to allow an individual 'worker'
-        client to run Async and handle all of these request.
-        If there is a lot of activity it will not get backed up.
-        Async queues the job up and handles it as it can
-        while the users request finishes and moves on
-        avoiding sacrifices in performance.
-        Refer to the collective.async pypi page
-        for instructions on setting it up if you use it.
-        Async is NOT required for AuditLog to work,
-        however it is advised, especially for high traffic sites.
-        
-        
-        Installation
-        ============
-        
-        Download the package from GitHub and extract into your src directory.
-        Add 'collective.auditlog' to your eggs and zcml slugs in buildout.
-        Include the location (src/collective.auditlog) in development slugs too.
-        Run buildout
-        
-        In Site Setup -> Add-ons, active Audit Log.
-        Once it is installed you will see "AuditLog" under Add-on Configuration.
-        This is where you can configuration the relational database.
-        The configuration string needs to be a valid SQLAlchemy connection string.
-        The control panel also allows you to enable/disable
-        tracking of actions performed on working copies.
-        
-        All that is left is to configure the new Content Rules
-        to track the content types and actions you desire.
-        
-        Upgrading
-        =========
-        
-        If you are upgrading from an older version, you will need to run the
-        upgrade steps from the add-ons control panel.
-        
-        USAGE
-        =====
-        For now, collective.auditlog uses SQLAlchemy for storing data. To use
-        postgres, it's necessary to add the 'psycopg2' egg to the buildout. Once
-        the product is installed, add the correct connection URL to the product
-        setup. Example::
-        
-            postgresql://enfold:enfold@localhost/auditlog
-        
-        By default, collective.auditlog uses content rules to define which events
-        to capture. An additional mechanism has been added that allows the site to
-        automatically log the various events supported by collective.auditlog.
-        Simply choose from the picklist in the config for this to work. If no
-        events are selected, no logging will occur.
-        
-        It is possible to log custom events from application code by using the
-        AuditableActionPerformedEvent, like this::
-        
-            from zope event import notify
-            from collective.auditlog.interfaces import AuditableActionPerformedEvent
-            notify(AuditableActionPerformedEvent(obj, request, "action", "note"))
-        
-        'obj', refers to the affected content object; 'request' is the current zope
-        request, 'action' and 'note' correspond to the logged action and its
-        description, respectively. All parameters are required, but everything
-        except obj can be set to None if no value is available.
-        
-        In addition to control panel configuration, connection parameters can be
-        set using the zope-conf-additional directive in the buildout. Note that
-        this will take precedence over any control panel configuration. Example::
-        
-            zope-conf-additional =
-                <product-config collective.auditlog>
-                    audit-connection-string postgres://enfold:enfold@localhost/auditlog
-                    audit-connection-params {"pool_recycle": 3600, "echo": true}
-                </product-config>
-        
-        There is now a view for the audit log entries, located at @@auditlog-view.
-        There is no link to it from the control panel at the moment. The view uses
-        infinite scrollong rather than pagination for looking at the logs.
-        
-        Searching the audit log
-        =======================
-        
-        Audit logs are stored in a SQL table, so you can use any SQL database tool
-        to analyse the audit log. However, sometimes you may need to query the logs
-        in the context of the Plone objects that generated them, for which the
-        information stored in SQL is not enough. For this purpose,
-        collective.auditlog offers a catalog based mechanism which can be used to
-        query the logs using any Plone based indexes available at the time of
-        logging. This can be used, for example, to develop a portlet that shows the
-        latest documents that have been modified.
-        
-        To enable catalog-based logging, choose sql+zodb storage in the audit log
-        control panel. Information will still be stored in the SQL database, but
-        a special catalog will be enabled to store plone indexing information as
-        well.
-        
-        Once this storage is enabled, you can search the logs using a catalog-like
-        query::
-        
-            from datetime import datetime
-            from collective.auditlog.catalog import searchAudited
-        
-            from = datatime(2018,6,1)
-            to = datetime(2018,12,31)
-            query = {'portal_type': 'Document',
-                    'review_state': 'published'}
-            audited = searchAudited(from_date=from,
-                                    to_date=to,
-                                    actions=['added', 'modified'],
-                                    **query)
-        
-        All of the parameters are optional, but an empty query will return all
-        indexed objects, so use with care.
-        
-        Note that the query will return catalog records, and any documents that have
-        multiple actions performed in the selected date range, will only appear once
-        in the list. There are also catalog records for deleted items, so a query
-        can be made to look for those even if they are gone from Plone.
-        
-        
-        Celery Integration
-        ==================
-        The collective.celery package requires adding the celery and
-        collective.celery eggs to the mian buildout section eggs. Example::
-        
-            eggs =
-                celery
-                Plone
-                collective.celery
-        
-        We still use the celery-broker part, for clarity. The celery part is
-        still required, but is simpler::
-        
-            [celery-broker]
-            host = 127.0.0.1
-            port = 6379
-        
-            [celery]
-            recipe = zc.recipe.egg
-            environment-vars = ${buildout:environment-vars}
-            eggs =
-                ${buildout:eggs}
-                flower
-            scripts = pcelery flower
-        
-        The celery part depends on having some variables added to the main
-        environment-vars section::
-        
-            environment-vars =
-                CELERY_BROKER_URL redis://${celery-broker:host}:${celery-broker:port}
-                CELERY_RESULT_BACKEND redis://${celery-broker:host}:${celery-broker:port}
-                CELERY_TASKS collective.es.index.tasks
-        
-        Additional Zope configuration
-        -----------------------------
-        
-        There's now a hook in collective.celery for carrying out additional zope
-        configuration before running the tasks. If the tasks module contains an
-        'extra_config' method, it is passed the zope startup object at worker
-        initialization time. This is used by collective.es.index to run the
-        elasticsearch configuration method.
-        
-        Monitoring celery tasks
-        -----------------------
-        
-        Celery needs to be started as an independent process. It's recommended to
-        use supervisord for this. To try it out from the command line, you can run
-        use supervisord for this. To try it out from the command line, you can run
-        "bin/pcelery worker" from the buildout directory. Note that the script is
-        now named 'pcelery' and it needs a path to the zope configuration. Example::
-        
-            $ bin/pcelery worker parts/client1/etc/zope.conf
-        
-        Flower is included in this setup. Run "bin/flower" from the buildout
-        directory and consult the dashboard at http://localhost:5555 using a
-        browser. Note that the broker is now a requried parameter::
-        
-            $ bin/flower --broker redis://127.0.0.1:6379
-        
-        Dependencies
-        ============
-        
-        All dependencies are installed automatically
-        when installing collective.auditlog.
-        Here is just a list of those for reference:
-        
-        - setuptools
-        - sqlalchemy
-        - five.globalrequest
-        - plone.app.async [OPTIONAL]
-        - collective.celery [OPTIONAL]
-        
-        Authors
-        =======
-        
-        - Joel Rainwater, initial author
-        - Nathan van Gheem, Async integration, bug fixes, optimization.
-        - Alessandro Pisa, bug fixing, testing
-        - Enfold Systems, celery integration and audit view
-        
-        
-        Changelog
-        =========
-        
-        2.0.0a2 (2020-03-19)
-        --------------------
-        
-        - Fix request not having an environment attribute in instance scripts
-          [ale-rt]
-        
-        
-        2.0.0a1 (2020-03-11)
-        --------------------
-        
-        - Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
-          [thet]
-        
-        - Remove deprecations.
-          action.canExecute is renamed to ``can_execute``, takes no paramters and is a property.
-          [thet]
-        
-        - Python 3 compatibility.
-          [thet]
-        
-        - Remove support for plone.app.async.
-          Due to  ``async`` being a reserved word, this cannot made Python 3 compatible.
-          Use collective.celeries instead.
-          [thet]
-        
-        - Drop support for Archetypes.
-          [thet]
-        
-        - Plone 5.2 compatibility.
-          Drop Support for Plone 5.0 and 4.3 (Both are missing zope.interface.interfaces.IObjectEvent).
-          [thet]
-        
-        - Make Arhcetype a soft dependency.
-          [ale-rt]
-        
-        - Align with Plone code style: black, isort.
-          [thet]
-        
-        - Fix soft dependency on formlib (#22)
-          [ale-rt]
-        
-        - Speed up rule retrieval
-          [ale-rt]
-        
-        - Added some memoized properties and methods to the `AuditActionExecutor` class
-          for easier customization
-          [ale-rt]
-        
-        - collective.celery integration
-          [enfold]
-        
-        - @@auditlog-view allows viewing/sorting/searching audit log entries
-          [enfold]
-        
-        - add login & logout audits
-          [enfold]
-        
-        - ability to specify the sqlalchemy DSN in config file
-          [enfold]
-        
-        - Notify an event before storing audit log entry.
-          [enfold]
-        
-        - Use custom permission for viewing audit log.
-          [enfold]
-        
-        - Fix tests.
-          [enfold]
-        
-        - Fix db connection leak.
-          [enfold]
-        
-        - Use valid json in info field.
-          [enfold]
-        
-        
-        1.3.3 (2018-07-12)
-        ------------------
-        
-        - Factored out getObjectInfo and addLogEntry.
-          [reinhardt]
-        
-        
-        1.3.2 (2018-07-11)
-        ------------------
-        
-        - Skip retrieving rule when audit log is disabled completely.
-          Improves performance.
-          [reinhardt]
-        
-        
-        1.3.1 (2017-04-13)
-        ------------------
-        
-        - Fix upgrade step title.
-          [ale-rt]
-        
-        
-        1.3.0 (2017-04-13)
-        ------------------
-        
-        - The engine parameters (like pool_recycle, echo, ...)
-          can be specified through a registry record
-          [ale-rt]
-        
-        
-        1.2.2 (2016-06-06)
-        ------------------
-        
-        - Make action more robust on IActionSucceededEvent
-          [ale-rt]
-        
-        
-        1.2.1 (2016-05-10)
-        ------------------
-        
-        - Fix unicode issues
-        - Tests are working again
-          [ale-rt]
-        
-        
-        1.2.0 (2016-05-03)
-        ------------------
-        
-        - First public release
-        
 Keywords: Plone Audit Log
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: Addon
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Provides-Extra: celery
 Provides-Extra: test
+
+Introduction
+============
+
+The package allows you to audit actions being done on your site.
+It accomplishes this by using configurable content rules.
+
+By default, after you activate this package,
+it will create all the content rules
+that can be used for auditing with only the Page type to audit OOTB.
+If you want to audit more types of objects,
+you will need to configure the content rules.
+
+The audits are stored into a relational database.
+Once installed and called for the first time
+it will create a table called "audit" if it does not already exist,
+so there is no need to create the table manually.
+
+AuditLog attempts to use plone.app.async or collective.celery to
+perform the store actions, but if that fails it will finish the task
+directly. The advantage of this is to allow an individual 'worker'
+client to run Async and handle all of these request.
+If there is a lot of activity it will not get backed up.
+Async queues the job up and handles it as it can
+while the users request finishes and moves on
+avoiding sacrifices in performance.
+Refer to the collective.async pypi page
+for instructions on setting it up if you use it.
+Async is NOT required for AuditLog to work,
+however it is advised, especially for high traffic sites.
+
+
+Installation
+============
+
+Download the package from GitHub and extract into your src directory.
+Add 'collective.auditlog' to your eggs and zcml slugs in buildout.
+Include the location (src/collective.auditlog) in development slugs too.
+Run buildout
+
+In Site Setup -> Add-ons, active Audit Log.
+Once it is installed you will see "AuditLog" under Add-on Configuration.
+This is where you can configuration the relational database.
+The configuration string needs to be a valid SQLAlchemy connection string.
+The control panel also allows you to enable/disable
+tracking of actions performed on working copies.
+
+All that is left is to configure the new Content Rules
+to track the content types and actions you desire.
+
+Upgrading
+=========
+
+If you are upgrading from an older version, you will need to run the
+upgrade steps from the add-ons control panel.
+
+USAGE
+=====
+For now, collective.auditlog uses SQLAlchemy for storing data. To use
+postgres, it's necessary to add the 'psycopg2' egg to the buildout. Once
+the product is installed, add the correct connection URL to the product
+setup. Example::
+
+    postgresql://enfold:enfold@localhost/auditlog
+
+By default, collective.auditlog uses content rules to define which events
+to capture. An additional mechanism has been added that allows the site to
+automatically log the various events supported by collective.auditlog.
+Simply choose from the picklist in the config for this to work. If no
+events are selected, no logging will occur.
+
+It is possible to log custom events from application code by using the
+AuditableActionPerformedEvent, like this::
+
+    from zope event import notify
+    from collective.auditlog.interfaces import AuditableActionPerformedEvent
+    notify(AuditableActionPerformedEvent(obj, request, "action", "note"))
+
+'obj', refers to the affected content object; 'request' is the current zope
+request, 'action' and 'note' correspond to the logged action and its
+description, respectively. All parameters are required, but everything
+except obj can be set to None if no value is available.
+
+In addition to control panel configuration, connection parameters can be
+set using the zope-conf-additional directive in the buildout. Note that
+this will take precedence over any control panel configuration. Example::
+
+    zope-conf-additional =
+        <product-config collective.auditlog>
+            audit-connection-string postgres://enfold:enfold@localhost/auditlog
+            audit-connection-params {"pool_recycle": 3600, "echo": true}
+        </product-config>
+
+There is now a view for the audit log entries, located at @@auditlog-view.
+There is no link to it from the control panel at the moment. The view uses
+infinite scrollong rather than pagination for looking at the logs.
+
+Searching the audit log
+=======================
+
+Audit logs are stored in a SQL table, so you can use any SQL database tool
+to analyse the audit log. However, sometimes you may need to query the logs
+in the context of the Plone objects that generated them, for which the
+information stored in SQL is not enough. For this purpose,
+collective.auditlog offers a catalog based mechanism which can be used to
+query the logs using any Plone based indexes available at the time of
+logging. This can be used, for example, to develop a portlet that shows the
+latest documents that have been modified.
+
+To enable catalog-based logging, choose sql+zodb storage in the audit log
+control panel. Information will still be stored in the SQL database, but
+a special catalog will be enabled to store plone indexing information as
+well.
+
+Once this storage is enabled, you can search the logs using a catalog-like
+query::
+
+    from datetime import datetime
+    from collective.auditlog.catalog import searchAudited
+
+    from = datatime(2018,6,1)
+    to = datetime(2018,12,31)
+    query = {'portal_type': 'Document',
+            'review_state': 'published'}
+    audited = searchAudited(from_date=from,
+                            to_date=to,
+                            actions=['added', 'modified'],
+                            **query)
+
+All of the parameters are optional, but an empty query will return all
+indexed objects, so use with care.
+
+Note that the query will return catalog records, and any documents that have
+multiple actions performed in the selected date range, will only appear once
+in the list. There are also catalog records for deleted items, so a query
+can be made to look for those even if they are gone from Plone.
+
+
+Celery Integration
+==================
+The collective.celery package requires adding the celery and
+collective.celery eggs to the mian buildout section eggs. Example::
+
+    eggs =
+        celery
+        Plone
+        collective.celery
+
+We still use the celery-broker part, for clarity. The celery part is
+still required, but is simpler::
+
+    [celery-broker]
+    host = 127.0.0.1
+    port = 6379
+
+    [celery]
+    recipe = zc.recipe.egg
+    environment-vars = ${buildout:environment-vars}
+    eggs =
+        ${buildout:eggs}
+        flower
+    scripts = pcelery flower
+
+The celery part depends on having some variables added to the main
+environment-vars section::
+
+    environment-vars =
+        CELERY_BROKER_URL redis://${celery-broker:host}:${celery-broker:port}
+        CELERY_RESULT_BACKEND redis://${celery-broker:host}:${celery-broker:port}
+        CELERY_TASKS collective.es.index.tasks
+
+Additional Zope configuration
+-----------------------------
+
+There's now a hook in collective.celery for carrying out additional zope
+configuration before running the tasks. If the tasks module contains an
+'extra_config' method, it is passed the zope startup object at worker
+initialization time. This is used by collective.es.index to run the
+elasticsearch configuration method.
+
+Monitoring celery tasks
+-----------------------
+
+Celery needs to be started as an independent process. It's recommended to
+use supervisord for this. To try it out from the command line, you can run
+use supervisord for this. To try it out from the command line, you can run
+"bin/pcelery worker" from the buildout directory. Note that the script is
+now named 'pcelery' and it needs a path to the zope configuration. Example::
+
+    $ bin/pcelery worker parts/client1/etc/zope.conf
+
+Flower is included in this setup. Run "bin/flower" from the buildout
+directory and consult the dashboard at http://localhost:5555 using a
+browser. Note that the broker is now a required parameter::
+
+    $ bin/flower --broker redis://127.0.0.1:6379
+
+Dependencies
+============
+
+All dependencies are installed automatically
+when installing collective.auditlog.
+Here is just a list of those for reference:
+
+- setuptools
+- sqlalchemy
+- five.globalrequest
+- plone.app.async [OPTIONAL]
+- collective.celery [OPTIONAL]
+
+Authors
+=======
+
+- Joel Rainwater, initial author
+- Nathan van Gheem, Async integration, bug fixes, optimization.
+- Alessandro Pisa, bug fixing, testing
+- Enfold Systems, celery integration and audit view
+
+
+3.0.0a1 (2023-06-01)
+--------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c)
+
+
+Changelog
+=========
+
+3.0.0a1 (unreleased)
+--------------------
+
+- Drop Python 2.7
+- Use SQLAlchemy 1.4
+  [ale-rt]
+
+2.0.0 (2023-05-31)
+------------------
+
+- Re-release 2.0.0a2 as 2.0.0.
+  This will be the last release supporting Python2.7.
+  [ale-rt]
+
+
+2.0.0a2 (2020-03-19)
+--------------------
+
+- Fix request not having an environment attribute in instance scripts
+  [ale-rt]
+
+
+2.0.0a1 (2020-03-11)
+--------------------
+
+- Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
+  [thet]
+
+- Remove deprecations.
+  action.canExecute is renamed to ``can_execute``, takes no parameters and is a property.
+  [thet]
+
+- Python 3 compatibility.
+  [thet]
+
+- Remove support for plone.app.async.
+  Due to  ``async`` being a reserved word, this cannot made Python 3 compatible.
+  Use collective.celeries instead.
+  [thet]
+
+- Drop support for Archetypes.
+  [thet]
+
+- Plone 5.2 compatibility.
+  Drop Support for Plone 5.0 and 4.3 (Both are missing zope.interface.interfaces.IObjectEvent).
+  [thet]
+
+- Make Arhcetype a soft dependency.
+  [ale-rt]
+
+- Align with Plone code style: black, isort.
+  [thet]
+
+- Fix soft dependency on formlib (#22)
+  [ale-rt]
+
+- Speed up rule retrieval
+  [ale-rt]
+
+- Added some memoized properties and methods to the `AuditActionExecutor` class
+  for easier customization
+  [ale-rt]
+
+- collective.celery integration
+  [enfold]
+
+- @@auditlog-view allows viewing/sorting/searching audit log entries
+  [enfold]
+
+- add login & logout audits
+  [enfold]
+
+- ability to specify the sqlalchemy DSN in config file
+  [enfold]
+
+- Notify an event before storing audit log entry.
+  [enfold]
+
+- Use custom permission for viewing audit log.
+  [enfold]
+
+- Fix tests.
+  [enfold]
+
+- Fix db connection leak.
+  [enfold]
+
+- Use valid json in info field.
+  [enfold]
+
+
+1.3.3 (2018-07-12)
+------------------
+
+- Factored out getObjectInfo and addLogEntry.
+  [reinhardt]
+
+
+1.3.2 (2018-07-11)
+------------------
+
+- Skip retrieving rule when audit log is disabled completely.
+  Improves performance.
+  [reinhardt]
+
+
+1.3.1 (2017-04-13)
+------------------
+
+- Fix upgrade step title.
+  [ale-rt]
+
+
+1.3.0 (2017-04-13)
+------------------
+
+- The engine parameters (like pool_recycle, echo, ...)
+  can be specified through a registry record
+  [ale-rt]
+
+
+1.2.2 (2016-06-06)
+------------------
+
+- Make action more robust on IActionSucceededEvent
+  [ale-rt]
+
+
+1.2.1 (2016-05-10)
+------------------
+
+- Fix unicode issues
+- Tests are working again
+  [ale-rt]
+
+
+1.2.0 (2016-05-03)
+------------------
+
+- First public release
```

### Comparing `collective.auditlog-2.0.0a2/setup.py` & `collective.auditlog-3.0.0a1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,59 @@
-# coding=utf-8
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.0a2"
+version = "3.0.0a1"
 
 
-long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read(),])
+long_description = "\n\n".join(
+    [
+        open("README.rst").read(),
+        open("CHANGES.rst").read(),
+    ]
+)
 
 
 setup(
     name="collective.auditlog",
     version=version,
     description=("Provides extra conditions and triggers for all content " "actions"),
     long_description=long_description,
     # Get more strings from
     # http://pypi.python.org/pypi?:action=list_classifiers
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.1",
         "Framework :: Plone :: 5.2",
         "Framework :: Plone :: Addon",
+        "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     keywords="Plone Audit Log",
     author="rain2o",
     author_email="Joel@rain2odesigns.com",
     url="http://svn.plone.org/svn/collective/",
     license="GPL",
     packages=find_packages(),
     namespace_packages=["collective"],
     include_package_data=True,
     zip_safe=False,
-    install_requires=["setuptools", "sqlalchemy", "plone.app.contentrules",],
+    install_requires=[
+        "setuptools",
+        "sqlalchemy>=1.4,<2",
+        "plone.app.contentrules",
+    ],
+    python_requires=">=3.7",
     extras_require={
-        "celery": ["collective.celery",],
+        "celery": [
+            "collective.celery",
+        ],
         "test": [
             "plone.app.testing",
             "plone.app.contenttypes",
             "pysqlite;python_version<'3'",
         ],
     },
     entry_points="""
```

### Comparing `collective.auditlog-2.0.0a2/CHANGES.rst` & `collective.auditlog-3.0.0a1/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,50 @@
+3.0.0a1 (2023-06-01)
+--------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c)
+
+
 Changelog
 =========
 
+3.0.0a1 (unreleased)
+--------------------
+
+- Drop Python 2.7
+- Use SQLAlchemy 1.4
+  [ale-rt]
+
+2.0.0 (2023-05-31)
+------------------
+
+- Re-release 2.0.0a2 as 2.0.0.
+  This will be the last release supporting Python2.7.
+  [ale-rt]
+
+
 2.0.0a2 (2020-03-19)
 --------------------
 
 - Fix request not having an environment attribute in instance scripts
   [ale-rt]
 
 
 2.0.0a1 (2020-03-11)
 --------------------
 
 - Remove inconsistent passing of ``request`` parameter and use zope.globalrequest instead.
   [thet]
 
 - Remove deprecations.
-  action.canExecute is renamed to ``can_execute``, takes no paramters and is a property.
+  action.canExecute is renamed to ``can_execute``, takes no parameters and is a property.
   [thet]
 
 - Python 3 compatibility.
   [thet]
 
 - Remove support for plone.app.async.
   Due to  ``async`` being a reserved word, this cannot made Python 3 compatible.
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/catalog.py` & `collective.auditlog-3.0.0a1/collective/auditlog/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,20 @@
 except ImportError:
     try:
         from App.class_init import InitializeClass
     except ImportError:
         from Globals import InitializeClass
 
 
-class Empty(object):
-    """
-    """
+class Empty:
+    """ """
 
 
 class IAuditCatalog(Interface):
-    """
-    """
+    """ """
 
 
 @implementer(IAuditCatalog)
 class AuditCatalog(CatalogTool):
     """
     A specific launch catalog tool
     """
@@ -57,22 +55,22 @@
             self.addIndex("last_audited_date", "DateIndex")
             self.addIndex("audited_action", "KeywordIndex")
             self.addColumn("Title")
             self.addColumn("id")
             self.addColumn("UID")
             self.addColumn("last_audited_date")
             self.addColumn("audited_action")
-            l = PLexicon(
+            lexicon = PLexicon(
                 "audit_lexicon",
                 "",
                 HTMLWordSplitter(),
                 CaseNormalizer(),
                 StopWordRemover(),
             )
-            self._setObject("audit_lexicon", l)
+            self._setObject("audit_lexicon", lexicon)
         catalog = portal_api.get_tool("portal_catalog")
         indexes = catalog._catalog.indexes
         for name, index in indexes.items():
             if name in list(self._catalog.indexes.keys()):
                 continue
             if index.meta_type == "DateRecurringIndex":
                 continue
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/tests/test_actions.py` & `collective.auditlog-3.0.0a1/collective/auditlog/tests/test_actions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from collective.auditlog.db import getSession
 from collective.auditlog.interfaces import IAuditLogSettings
 from collective.auditlog.models import Base
 from collective.auditlog.models import LogEntry
 from collective.auditlog.testing import AuditLog_FUNCTIONAL_TESTING
 from plone.app.contentrules.handlers import _status
 from plone.app.testing import login
@@ -18,85 +17,76 @@
 
 import json
 import os
 import transaction
 import unittest
 
 
-try:
-    # Archetypes
-    from Products.Archetypes.event import ObjectEditedEvent
-    from Products.Archetypes.event import ObjectInitializedEvent
-
-    HAS_AT = True
-except ImportError:
-    HAS_AT = False
-
-
-class tempDb(object):
-
+class tempDb:
     registry_key = "{iface}.connectionstring".format(
         iface=IAuditLogSettings.__identifier__
     )
     session = None
 
     def __init__(self):
         _, self.tempfilename = mkstemp()
 
     @property
     def logs(self):
         return self.session.query(LogEntry).all()
 
     def __enter__(self):
         self.registry = registry = getUtility(IRegistry)
-        registry[self.registry_key] = u"sqlite:///%s" % (self.tempfilename)
+        registry[self.registry_key] = "sqlite:///%s" % (self.tempfilename)
         self.session = getSession()
         Base.metadata.create_all(self.session.bind.engine)
         return self
 
     def __exit__(self, type, value, traceback):
         os.remove(self.tempfilename)
 
 
 class TestActions(unittest.TestCase):
-
     layer = AuditLog_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"].clone()
         login(self.portal, TEST_USER_NAME)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         registry_key = "{iface}.automaticevents".format(
             iface=IAuditLogSettings.__identifier__
         )
         registry = getUtility(IRegistry)
         registry[registry_key] = [
-            u"OFS.interfaces.IObjectClonedEvent",
-            u"plone.app.iterate.interfaces.IBeforeCheckoutEvent",
-            u"plone.app.iterate.interfaces.ICancelCheckoutEvent",
-            u"plone.app.iterate.interfaces.ICheckinEvent",
-            u"Products.CMFCore.interfaces.IActionSucceededEvent",
-            u"zope.lifecycleevent.interfaces.IObjectAddedEvent",
-            u"zope.lifecycleevent.interfaces.IObjectModifiedEvent",
-            u"zope.lifecycleevent.interfaces.IObjectMovedEvent",
+            "OFS.interfaces.IObjectClonedEvent",
+            "plone.app.iterate.interfaces.IBeforeCheckoutEvent",
+            "plone.app.iterate.interfaces.ICancelCheckoutEvent",
+            "plone.app.iterate.interfaces.ICheckinEvent",
+            "Products.CMFCore.interfaces.IActionSucceededEvent",
+            "zope.lifecycleevent.interfaces.IObjectAddedEvent",
+            "zope.lifecycleevent.interfaces.IObjectModifiedEvent",
+            "zope.lifecycleevent.interfaces.IObjectMovedEvent",
         ]
 
     def create_page(self, title="Page"):
-        """ Create a page and return it
-        """
-        obj_id = self.portal.invokeFactory("Document", id="page", title=title,)
+        """Create a page and return it"""
+        obj_id = self.portal.invokeFactory(
+            "Document",
+            id="page",
+            title=title,
+        )
         obj = self.portal[obj_id]
         notify(ObjectAddedEvent(obj))
         # We need to commit here so that _p_jar isn't None and move will work
         transaction.savepoint(optimistic=True)
         return obj
 
     def reset_rule_filter(self):
-        """ If we want to execute a rule multiple times in the same test
+        """If we want to execute a rule multiple times in the same test
         we need to reset the rule filter, mocking a fresh request
         """
         _status.rule_filter.reset()
 
     def test_add(self):
         with tempDb() as db:
             self.create_page()
@@ -115,15 +105,17 @@
             cd = self.portal.manage_cutObjects("page")
             self.portal.folder.manage_pasteObjects(cd)
             self.assertEqual(db.logs[-1].action, "moved")
 
     def test_copied(self):
         self.create_page()
         self.portal.invokeFactory(
-            "Folder", id="folder", title="folder",
+            "Folder",
+            id="folder",
+            title="folder",
         )
         with tempDb() as db:
             cd = self.portal.manage_copyObjects("page")
             self.portal.folder.manage_pasteObjects(cd)
             self.assertEqual(db.logs[-1].action, "copied")
 
     @unittest.skip("The ObjectModifiedEvent seems not to be fired")
@@ -143,21 +135,22 @@
 
     def test_transition(self):
         self.create_page()
         pw = getToolByName(self.portal, "portal_workflow")
         with tempDb() as db:
             # publish and ...
             pw.doActionFor(
-                self.portal.page, "publish",
+                self.portal.page,
+                "publish",
             )
-            self.assertEqual(db.logs[-1].action, u"workflow")
+            self.assertEqual(db.logs[-1].action, "workflow")
             info = json.loads(db.logs[-1].info)
-            self.assertEqual(info["transition"], u"publish")
-            self.assertEqual(info["comments"], u"")
+            self.assertEqual(info["transition"], "publish")
+            self.assertEqual(info["comments"], "")
 
             self.reset_rule_filter()
             # ... retract the test page (adding a comment)
             pw.doActionFor(self.portal.page, "retract", comment="I've been commented ♥")
-            self.assertEqual(db.logs[-1].action, u"workflow")
+            self.assertEqual(db.logs[-1].action, "workflow")
             info = json.loads(db.logs[-1].info)
-            self.assertEqual(info["transition"], u"retract")
-            self.assertEqual(info["comments"], u"I've been commented \u2665")
+            self.assertEqual(info["transition"], "retract")
+            self.assertEqual(info["comments"], "I've been commented \u2665")
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/browser.py` & `collective.auditlog-3.0.0a1/collective/auditlog/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from collective.auditlog import db
 from collective.auditlog.models import LogEntry
 from Products.Five.browser import BrowserView
 from sqlalchemy import desc
 from sqlalchemy import or_
 
-import six
-
 
 class LogView(BrowserView):
-
     page_size = 100
 
     columns = [
         {"name": "user", "label": "User"},
         {"name": "performed_on", "label": "Date"},
         {"name": "uid", "label": "UID"},
         {"name": "type", "label": "Type"},
@@ -59,15 +56,15 @@
         query = self.request.get("query", "")
         session = db.getSession()
         if self.direction == "asc":
             lines = session.query(LogEntry).order_by(order)
         else:
             lines = session.query(LogEntry).order_by(desc(order))
         if query:
-            query = six.text_type(query)
+            query = str(query)
             lines = lines.filter(
                 or_(
                     LogEntry.user.contains(query),
                     LogEntry.uid.contains(query),
                     LogEntry.type.contains(query),
                     LogEntry.title.contains(query),
                     LogEntry.path.contains(query),
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/td.py` & `collective.auditlog-3.0.0a1/collective/auditlog/td.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 on the zope transaction
 """
 
 from collective.auditlog import db
 from collective.auditlog.models import Base
 from logging import getLogger
 from plone.app.contentrules import handlers as cr_handlers
+from sqlalchemy import inspect
 from transaction.interfaces import IDataManagerSavepoint
 from transaction.interfaces import ISavepointDataManager
 from zope.interface import implementer
 
 import threading
 import traceback
 import transaction as transaction_manager
@@ -28,34 +29,34 @@
         return tranaction_data.data
     except AttributeError:
         tranaction_data.data = TransactionData()
         return tranaction_data.data
 
 
 @implementer(ISavepointDataManager)
-class DataManager(object):
+class DataManager:
     def __init__(self, td):
         self._session = None
         self.td = td
         self.savepoints = []
 
     @property
     def session(self):
         if self._session is None:
             self._session = db.getSession()
             engine = db.getEngine()
-            if not engine.dialect.has_table(engine, "audit"):
+            if not inspect(engine).has_table("audit"):
                 Base.metadata.create_all(bind=engine)
         return self._session
 
     def commit(self, trans):
         if self.td.registered:
             try:
                 self.session.commit()
-            except:
+            except Exception:
                 logger.error(
                     "Error during audit log commit. "
                     "Error stack: %s" % (traceback.format_exc())
                 )
         self.td.reset()
         self._clear_session()
 
@@ -115,15 +116,15 @@
                 for ob in self.old:
                     self.dm.session.add(ob)
             else:
                 # allow content rules to run again
                 cr_handlers.close(None)
 
 
-class TransactionData(object):
+class TransactionData:
     def __init__(self):
         self.joined = False
         self.registered = False
         self.items = []
         self.dm = None
 
     def join(self):
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/models.py` & `collective.auditlog-3.0.0a1/collective/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/configure.zcml` & `collective.auditlog-3.0.0a1/collective/auditlog/configure.zcml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,69 +13,69 @@
   <include package=".upgrades" />
 
 
   <!-- Control panel -->
   <browser:page
       name="auditlog-settings"
       for="Products.CMFPlone.interfaces.IPloneSiteRoot"
-      permission="cmf.ManagePortal"
       class=".controlpanel.AuditLogSettingsControlPanel"
       template="controlpanel.pt"
+      permission="cmf.ManagePortal"
       />
 
   <browser:resourceDirectory
       name="collective.auditlog"
       directory="static"
       />
 
   <browser:page
       name="auditlog-view"
       for="Products.CMFPlone.interfaces.IPloneSiteRoot"
-      permission="collective.auditlog.ViewAuditlog"
       class="collective.auditlog.browser.LogView"
       template="logview.pt"
+      permission="collective.auditlog.ViewAuditlog"
       />
 
   <interface
-      name="A working copy has been checked in."
       interface="plone.app.iterate.interfaces.ICheckinEvent"
       type="plone.contentrules.rule.interfaces.IRuleEventType"
+      name="A working copy has been checked in."
       />
 
   <interface
-      name="An object has been checked out."
       interface="plone.app.iterate.interfaces.IBeforeCheckoutEvent"
       type="plone.contentrules.rule.interfaces.IRuleEventType"
+      name="An object has been checked out."
       />
 
   <interface
-      name="A working copy has been cancelled."
       interface="plone.app.iterate.interfaces.ICancelCheckoutEvent"
       type="plone.contentrules.rule.interfaces.IRuleEventType"
+      name="A working copy has been cancelled."
       />
 
   <interface
-      name="An object has been moved"
       interface="zope.lifecycleevent.interfaces.IObjectMovedEvent"
       type="plone.contentrules.rule.interfaces.IRuleEventType"
+      name="An object has been moved"
       />
   <interface
-      name="An object has been added"
       interface="zope.lifecycleevent.interfaces.IObjectAddedEvent"
       type="plone.contentrules.rule.interfaces.IRuleEventType"
+      name="An object has been added"
       />
   <interface
-      name="An object has been created"
       interface="zope.lifecycleevent.interfaces.IObjectCreatedEvent"
       type="plone.contentrules.rule.interfaces.IRuleEventType"
+      name="An object has been created"
       />
   <interface
-      name="An object has been copied"
       interface="OFS.interfaces.IObjectClonedEvent"
       type="plone.contentrules.rule.interfaces.IRuleEventType"
+      name="An object has been copied"
       />
 
   <!-- Rule triggers -->
   <subscriber
       for="plone.app.iterate.interfaces.ICheckinEvent"
       handler=".handlers.execute_event"
       />
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.pt` & `collective.auditlog-3.0.0a1/collective/auditlog/controlpanel.pt`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,19 @@
 
       <h1 class="documentFirstHeading"
           tal:content="view/label"
       >View Title</h1>
       <p>
         <a tal:attributes="
              href string:${portal_url}/@@auditlog-view?order=performed_on&amp;direction=desc;
-           "
-        ><img tal:attributes="
+           "><img tal:attributes="
                  src string:${portal_url}/topic_icon.png;
-               "
-          />
-          View Audit Log</a>
+               " />
+          <tal:i18n i18n:translate="">View Audit Log</tal:i18n>
+        </a>
       </p>
 
       <div metal:use-macro="context/global_statusmessage/macros/portal_message">
       Portal status message
       </div>
 
       <div id="content-core">
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/upgrades/configure.zcml` & `collective.auditlog-3.0.0a1/collective/auditlog/upgrades/configure.zcml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,77 +2,77 @@
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     >
 
   <genericsetup:upgradeStep
       title="Update the registry records"
       description=""
-      destination="1001"
-      handler=".to1001.fix_registry_records"
       profile="collective.auditlog:default"
       source="*"
+      destination="1001"
+      handler=".to1001.fix_registry_records"
       />
 
   <genericsetup:upgradeStep
       title="Update the registry records"
       description=""
-      destination="1002"
-      handler=".to1001.fix_registry_records"
       profile="collective.auditlog:default"
       source="*"
+      destination="1002"
+      handler=".to1001.fix_registry_records"
       />
 
   <genericsetup:upgradeStep
       title="Update the registry records"
       description=""
-      destination="1003"
-      handler=".to1001.fix_registry_records"
       profile="collective.auditlog:default"
       source="*"
+      destination="1003"
+      handler=".to1001.fix_registry_records"
       />
 
   <genericsetup:upgradeStep
       title="Update the registry records"
       description=""
-      destination="1004"
-      handler=".to1001.fix_registry_records"
       profile="collective.auditlog:default"
       source="*"
+      destination="1004"
+      handler=".to1001.fix_registry_records"
       />
 
   <genericsetup:upgradeStep
       title="Update the registry records"
       description=""
-      destination="1005"
-      handler=".to1001.fix_registry_records"
       profile="collective.auditlog:default"
       source="*"
+      destination="1005"
+      handler=".to1001.fix_registry_records"
       />
 
   <genericsetup:upgradeStep
       title="Update the registry records"
       description=""
-      destination="1006"
-      handler=".to1001.fix_registry_records"
       profile="collective.auditlog:default"
       source="*"
+      destination="1006"
+      handler=".to1001.fix_registry_records"
       />
 
   <genericsetup:upgradeDepends
       title="Add new catalog"
       description=""
-      destination="1007"
-      import_steps="toolset"
       profile="collective.auditlog:default"
       source="*"
+      destination="1007"
+      import_steps="toolset"
       />
 
   <genericsetup:upgradeDepends
       title="Add new permission"
       description=""
-      destination="1008"
-      import_steps="rolemap actions"
       profile="collective.auditlog:default"
       source="*"
+      destination="1008"
+      import_steps="rolemap actions"
       />
 
 </configure>
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/__init__.py` & `collective.auditlog-3.0.0a1/collective/auditlog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from App.Undo import decode64
-from App.Undo import UndoSupport
 from collective.auditlog.interfaces import AuditableActionPerformedEvent
 from zope.event import notify
 from zope.i18nmessageid import MessageFactory
 
 import transaction
 
 
 MessageFactory = MessageFactory("collective.auditlog")
 
 
 def manage_undo_transactions_with_audit(self, transaction_info=(), REQUEST=None):
-    """
-    """
+    """ """
     tids = []
     descriptions = []
     for tid in transaction_info:
         tid = tid.split()
         if tid:
             tids.append(decode64(tid[0]))
             descriptions.append(tid[-1])
@@ -30,9 +28,9 @@
 
     if REQUEST is None:
         return
     REQUEST["RESPONSE"].redirect("%s/manage_UndoForm" % REQUEST["URL1"])
     return ""
 
 
-# monkey patch undo to be able to audit ZMI undo operations
-## UndoSupport.manage_undo_transactions = manage_undo_transactions_with_audit
+# # monkey patch undo to be able to audit ZMI undo operations
+# UndoSupport.manage_undo_transactions = manage_undo_transactions_with_audit
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/handlers.py` & `collective.auditlog-3.0.0a1/collective/auditlog/handlers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from collective.auditlog.action import AuditActionExecutor
 from collective.auditlog.utils import addLogEntry
 from collective.auditlog.utils import getObjectInfo
 from collective.auditlog.utils import getSite
 from collective.auditlog.utils import is_installed
 from importlib import import_module
 from plone.app.discussion.interfaces import IComment
@@ -14,29 +13,29 @@
 from zope.lifecycleevent.interfaces import IObjectCopiedEvent
 from zope.lifecycleevent.interfaces import IObjectRemovedEvent
 
 import json
 
 
 try:
-    from plone.app.contentrules.handlers import (
-        execute_rules,
-        execute,
-        is_portal_factory,
-    )
+    from plone.app.contentrules.handlers import execute
+    from plone.app.contentrules.handlers import execute_rules
+    from plone.app.contentrules.handlers import is_portal_factory
 except ImportError:
-    from Acquisition import aq_inner, aq_parent
-    from plone.app.contentrules.handlers import execute, is_portal_factory
+    from Acquisition import aq_inner
+    from Acquisition import aq_parent
+    from plone.app.contentrules.handlers import execute
+    from plone.app.contentrules.handlers import is_portal_factory
 
     # copied from plone.app.iterate 2.0:
 
     def execute_rules(event):
-        """ When an action is invoked on an object,
+        """When an action is invoked on an object,
         execute rules assigned to its parent.
-        Base action executor handler """
+        Base action executor handler"""
 
         if is_portal_factory(event.object):
             return
 
         execute(aq_parent(aq_inner(event.object)), event)
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/asyncqueue.py` & `collective.auditlog-3.0.0a1/collective/auditlog/asyncqueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# coding=utf-8
 from collective.auditlog import db
 from collective.auditlog import td
 from collective.auditlog.models import LogEntry
 from Products.CMFPlone.utils import safe_unicode
 
 
 try:
-    import collective.celery
-    from collective.auditlog.tasks import queue_job
     from celery.utils.log import get_task_logger
+    from collective.auditlog.tasks import queue_job
+
+    import collective.celery  # noqa: F401
 
     logger = get_task_logger(__name__)
 except ImportError:
     queue_job = None
     import logging
 
     logger = logging.getLogger("collective.auditlog")
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/utils.py` & `collective.auditlog-3.0.0a1/collective/auditlog/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from Acquisition import aq_parent
 from collective.auditlog import td
 from collective.auditlog.asyncqueue import queueJob
 from collective.auditlog.catalog import catalogEntry
 from collective.auditlog.interfaces import BeforeStoreAuditlogEntryEvent
 from datetime import datetime
 from plone.registry.interfaces import IRegistry
@@ -85,15 +84,15 @@
             site = zope_root[plone_sites[0]]
         elif len(plone_sites) > 1:
             # many sites. Might be an undo attempt
             request = getRequest()
             if request and "transaction_info" in request.other:
                 info = " ".join(request.other["transaction_info"])
                 for plone_site in plone_sites:
-                    if " /{}/".format(plone_site) in info:
+                    if f" /{plone_site}/" in info:
                         site = zope_root[plone_site]
     return site
 
 
 def getUser():
     username = "unknown"
     try:
@@ -105,15 +104,15 @@
             username = getRequest().other.get("AUTHENTICATED_USER").getUserName()
         except AttributeError:
             pass
     return username
 
 
 def getObjectInfo(obj):
-    """ Get basic information about an object for logging.
+    """Get basic information about an object for logging.
     This only includes information available on the object itself. Some fields
     are missing because they depend on the event or rule that was triggered.
     """
     obj_id = obj.id
     if callable(obj_id):
         obj_id = obj_id()
     if not obj_id:
@@ -130,15 +129,15 @@
         else "/",
     )
     return data
 
 
 def addLogEntry(obj, data):
     # XXX getLogEntry sometime returns True, probably it should just return None
-    if not data or data == True:
+    if not data or data is True:
         return
     tdata = td.get()
     if not tdata.registered:
         tdata.register()
 
     notify(BeforeStoreAuditlogEntryEvent(obj, data))
     queueJob(getSite(), **data)
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/locales/collective.auditlog.pot` & `collective.auditlog-3.0.0a1/collective/auditlog/locales/collective.auditlog.pot`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/action.zcml` & `collective.auditlog-3.0.0a1/collective/auditlog/action.zcml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,30 +13,30 @@
   <!-- RunScript action definition -->
 
   <adapter factory=".action.AuditActionExecutor" />
 
   <browser:page
       name="plone.actions.Audit"
       for="plone.app.contentrules.browser.interfaces.IRuleActionAdding"
-      permission="cmf.ManagePortal"
       class=".action.AuditAddForm"
+      permission="cmf.ManagePortal"
       />
 
   <browser:page
       name="edit"
       for=".action.IAuditAction"
-      permission="cmf.ManagePortal"
       class=".action.AuditEditForm"
+      permission="cmf.ManagePortal"
       />
 
   <plone:ruleAction
       name="plone.actions.Audit"
       title="Audit"
       description="Audit action"
       for="*"
+      event="zope.interface.interfaces.IObjectEvent"
+      schema=".action.IAuditAction"
       factory=".action.AuditAction"
       addview="plone.actions.Audit"
       editview="edit"
-      event="zope.interface.interfaces.IObjectEvent"
-      schema=".action.IAuditAction"
       />
 </configure>
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/logview.pt` & `collective.auditlog-3.0.0a1/collective/auditlog/logview.pt`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
                    disable_column_one python:request.set('disable_plone.leftcolumn', 1);
                    disable_column_two python:request.set('disable_plone.rightcolumn', 1);
                  "
     />
     <metal:js fill-slot="javascript_head_slot">
       <script tal:attributes="
                 src string:${portal_url}/++resource++collective.auditlog/infinitescroll.jquery.js;
-              "
-      ></script>
+              "></script>
     </metal:js>
   </head>
   <body>
     <metal:title metal:fill-slot="content-title">
       <h1 class="documentFirstHeading"
           i18n:translate=""
       >
@@ -66,16 +65,15 @@
         </span>
       </form>
       <table class="listing">
         <tbody id="logview">
           <tr tal:define="
                 order python:request.get('order', 'performed_on');
                 direction view/direction;
-              "
-          >
+              ">
             <th style="white-space: nowrap"
                 tal:repeat="column view/columns"
             >
               <a tal:define="
                    new_direction python:view.new_direction(order, column['name']);
                  "
                  tal:content="column/label"
@@ -84,22 +82,20 @@
                  "
               >
               </a>
               <tal:block condition="python:order==column['name']">
                 <span tal:condition="python:direction == 'asc'">
                   <img tal:attributes="
                          src string:${portal_url}/arrowTop.png;
-                       "
-                  />
+                       " />
                 </span>
                 <span tal:condition="python:direction == 'desc'">
                   <img tal:attributes="
                          src string:${portal_url}/arrowBottom.png;
-                       "
-                  />
+                       " />
                 </span>
               </tal:block>
             </th>
           </tr>
           <tr class="logline"
               tal:repeat="line view/loglines"
               tal:on-error="string:"
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/controlpanel.py` & `collective.auditlog-3.0.0a1/collective/auditlog/controlpanel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-# coding=utf-8
 from collective.auditlog.db import config
 from collective.auditlog.interfaces import _
 from collective.auditlog.interfaces import IAuditLogSettings
 from plone.app.registry.browser import controlpanel
 
 
 class AuditLogSettingsEditForm(controlpanel.RegistryEditForm):
-
     schema = IAuditLogSettings
-    label = _(u"Audit Log settings")
-    description = _(u"""""")
+    label = _("Audit Log settings")
+    description = _("""""")
 
     def updateFields(self):
-        super(AuditLogSettingsEditForm, self).updateFields()
+        super().updateFields()
         conn_string = config.get("audit-connection-string", None)
         conn_string_field = self.fields.get("connectionstring", None)
         if conn_string is not None and conn_string_field is not None:
-            desc = u"""Read-only. The connection string was defined in
+            desc = """Read-only. The connection string was defined in
                 the configuration file.
             """
             conn_string_field.field.required = False
             conn_string_field.field.description = desc
         conn_params = config.get("audit-connection-params", None)
         conn_params_field = self.fields.get("connectionparameters", None)
         if conn_params is not None and conn_params_field is not None:
-            desc = u"""Read-only. The connection parameters were
+            desc = """Read-only. The connection parameters were
                 defined in the configuration file.
             """
             conn_params_field.field.required = False
             conn_params_field.field.description = desc
 
     def updateWidgets(self):
-        super(AuditLogSettingsEditForm, self).updateWidgets()
+        super().updateWidgets()
         conn_string = config.get("audit-connection-string", None)
         conn_string_widget = self.widgets.get("connectionstring", None)
         if conn_string is not None and conn_string_widget is not None:
             conn_string_widget.value = conn_string
             conn_string_widget.mode = "display"
         conn_params = config.get("audit-connection-params", None)
         conn_params_widget = self.widgets.get("connectionparameters", None)
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/db.py` & `collective.auditlog-3.0.0a1/collective/auditlog/db.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# coding=utf-8
 from App.config import getConfiguration
 from json import loads
 from plone.registry.interfaces import IRegistry
 from sqlalchemy import create_engine
 from sqlalchemy.orm import scoped_session
 from sqlalchemy.orm import sessionmaker
 from zope.component import getUtility
 
-import six
-
 
 zope_conf = getConfiguration()
 product_conf = getattr(zope_conf, "product_config", {})
 config = product_conf.get("collective.auditlog", {})
 
 engine = None
 session_factory = None
@@ -35,15 +32,15 @@
             conn_parameters = config.get("audit-connection-params", None)
         if conn_parameters is None:
             conn_parameters = registry[
                 "collective.auditlog.interfaces.IAuditLogSettings.connectionparameters"
             ]  # noqa
         if not conn_parameters:
             conn_parameters = {}
-        elif isinstance(conn_parameters, six.string_types):
+        elif isinstance(conn_parameters, str):
             conn_parameters = loads(conn_parameters)
         engine = create_engine(conn_string, **conn_parameters)
     return engine
 
 
 def getSession(conn_string=None, req=None):
     """
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/static/infinitescroll.jquery.js` & `collective.auditlog-3.0.0a1/collective/auditlog/static/infinitescroll.jquery.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -63,15 +63,15 @@
         path: undefined, // Either parts of a URL as an array (e.g. ["/page/", "/"] or a function that takes in the page number and returns a URL
         prefill: false, // When the document is smaller than the window, load data until the document is larger or links are exhausted
         maxPage: undefined // to manually control maximum page (when maxPage is undefined, maximum page limitation is not work)
     };
 
     $.infinitescroll.prototype = {
 
-        /*	
+        /*
             ----------------------------
             Private methods
             ----------------------------
             */
 
         // Bind or unbind from scroll
         _binding: function infscr_binding(binding) {
@@ -258,15 +258,15 @@
 
                 this._debug('pathParse manual');
                 return opts.pathParse(path, this.options.state.currPage + 1);
 
             } else if (path.match(/^(.*?)\b2\b(.*?$)/)) {
                 path = path.match(/^(.*?)\b2\b(.*?$)/).slice(1);
 
-                // if there is any 2 in the url at all.    
+                // if there is any 2 in the url at all.
             } else if (path.match(/^(.*?)2(.*?$)/)) {
 
                 // page= is used in django:
                 // http://www.infinite-scroll.com/changelog/comment-page-1/#comment-127
                 if (path.match(/^(.*?page=)2(\/.*|$)/)) {
                     path = path.match(/^(.*?page=)2(\/.*|$)/).slice(1);
                     return path;
@@ -278,15 +278,15 @@
 
                 // page= is used in drupal too but second page is page=1 not page=2:
                 // thx Jerod Fritz, vladikoff
                 if (path.match(/^(.*?page=)1(\/.*|$)/)) {
                     path = path.match(/^(.*?page=)1(\/.*|$)/).slice(1);
                     return path;
                 } else {
-                    this._debug('Sorry, we couldn\'t parse your Next (Previous Posts) URL. Verify your the css selector points to the correct A tag. If you still get this error: yell, scream, and kindly ask for help at infinite-scroll.com.');
+                    this._debug('Sorry, we could not parse your Next (Previous Posts) URL. Verify your the css selector points to the correct A tag. If you still get this error: yell, scream, and kindly ask for help at infinite-scroll.com.');
                     // Get rid of isInvalidPage to allow permalink to state
                     opts.state.isInvalidPage = true; //prevent it from running on this page.
                 }
             }
             this._debug('determinePath', path);
             return path;
 
@@ -402,15 +402,15 @@
             // if behavior is defined and this function is extended, call that instead of default
             if (!!opts.behavior && this['_nearbottom_' + opts.behavior] !== undefined) {
                 return this['_nearbottom_' + opts.behavior].call(this);
             }
 
             this._debug('math:', pixelsFromWindowBottomToBottom, opts.pixelsFromNavToBottom);
 
-            // if distance remaining in the scroll (including buffer) is less than the orignal nav to bottom....
+            // if distance remaining in the scroll (including buffer) is less than the original nav to bottom....
             return (pixelsFromWindowBottomToBottom - opts.bufferPx < opts.pixelsFromNavToBottom);
 
         },
 
         // Pause / temporarily disable plugin from firing
         _pausing: function infscr_pausing(pause) {
 
@@ -483,15 +483,15 @@
                 .parent()
                 .find('div').html(opts.loading.finishedMsg).animate({
                     opacity: 1
                 }, 2000, function() {
                     $(this).parent().fadeOut(opts.loading.speed);
                 });
 
-            // user provided callback when done    
+            // user provided callback when done
             opts.errorCallback.call($(opts.contentSelector)[0], 'done');
         },
 
         // grab each selector option and see if any fail
         _validate: function infscr_validate(opts) {
             for (var key in opts) {
                 if (key.indexOf && key.indexOf('Selector') > -1 && $(opts[key]).length === 0) {
@@ -499,15 +499,15 @@
                     return false;
                 }
             }
 
             return true;
         },
 
-        /*	
+        /*
             ----------------------------
             Public methods
             ----------------------------
             */
 
         // Bind to scroll
         bind: function infscr_bind() {
@@ -535,15 +535,15 @@
             var instance = this,
                 path = opts.path,
                 box, desturl, method, condition;
 
             // increment the URL bit. e.g. /page/3/
             opts.state.currPage++;
 
-            // Manually control maximum page 
+            // Manually control maximum page
             if (opts.maxPage != undefined && opts.state.currPage > opts.maxPage) {
                 this.destroy();
                 return;
             }
 
             // if we're dealing with a table we can't use DIVs
             box = $(opts.contentSelector).is('table') ? $('<tbody/>') : $('<div/>');
@@ -688,40 +688,40 @@
             if ($.isPlainObject(key)) {
                 this.options = $.extend(true, this.options, key);
             }
         }
     };
 
 
-    /*	
+    /*
         ----------------------------
         Infinite Scroll function
         ----------------------------
 
         Borrowed logic from the following...
 
         jQuery UI
         - https://github.com/jquery/jquery-ui/blob/master/ui/jquery.ui.widget.js
 
         jCarousel
         - https://github.com/jsor/jcarousel/blob/master/lib/jquery.jcarousel.js
 
         Masonry
-        - https://github.com/desandro/masonry/blob/master/jquery.masonry.js		
+        - https://github.com/desandro/masonry/blob/master/jquery.masonry.js
 
 */
 
     $.fn.infinitescroll = function infscr_init(options, callback) {
 
 
         var thisCall = typeof options;
 
         switch (thisCall) {
 
-            // method 
+            // method
             case 'string':
                 var args = Array.prototype.slice.call(arguments, 1);
 
                 this.each(function() {
                     var instance = $.data(this, 'infinitescroll');
 
                     if (!instance) {
@@ -737,15 +737,15 @@
 
                     // no errors!
                     instance[options].apply(instance, args);
                 });
 
                 break;
 
-                // creation 
+                // creation
             case 'object':
 
                 this.each(function() {
 
                     var instance = $.data(this, 'infinitescroll');
 
                     if (instance) {
@@ -772,15 +772,15 @@
         }
 
         return this;
     };
 
 
 
-    /* 
+    /*
      * smartscroll: debounced scroll event for jQuery *
      * https://github.com/lukeshumard/smartscroll
      * Based on smartresize by @louis_remi: https://github.com/lrbabe/jquery.smartresize.js *
      * Copyright 2011 Louis-Remi & Luke Shumard * Licensed under the MIT license. *
      */
 
     var event = $.event,
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/interfaces.py` & `collective.auditlog-3.0.0a1/collective/auditlog/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,76 +52,76 @@
 
 class IAuditLogSettings(Interface):
     """Audit Log settings.
     This allows you to set the database connection string.
     """
 
     storage = schema.Choice(
-        title=_(u"Log storage"),
+        title=_("Log storage"),
         description=_(
-            u"help_auditlog_storage",
+            "help_auditlog_storage",
             default=(
-                u"Audit Log is designed for use with a SQL database, "
-                u"but the data can be stored in the ZODB catalog for "
-                u"allowing audit log searches with catalog indexes."
+                "Audit Log is designed for use with a SQL database, "
+                "but the data can be stored in the ZODB catalog for "
+                "allowing audit log searches with catalog indexes."
             ),
         ),
         required=True,
         default="sql",
         values=("sql", "sql+zodb"),
     )
 
     connectionstring = schema.TextLine(
-        title=_(u"Audit Log Connection String"),
+        title=_("Audit Log Connection String"),
         description=_(
-            u"help_auditlog_connection",
+            "help_auditlog_connection",
             default=(
-                u"Enter the connection string for the database Audit Log "
-                u"is to write to. "
-                u"Must be a valid SQLAlchemy connection string."
+                "Enter the connection string for the database Audit Log "
+                "is to write to. "
+                "Must be a valid SQLAlchemy connection string."
             ),
         ),
         required=True,
-        default=u"sqlite:///:memory:",
+        default="sqlite:///:memory:",
     )
 
     connectionparameters = schema.TextLine(
-        title=_(u"Audit Log Connection Parameters"),
+        title=_("Audit Log Connection Parameters"),
         description=_(
-            u"help_auditlog_connection_parameteers",
+            "help_auditlog_connection_parameteers",
             default=(
-                u"Enter the connection parametes in a json form. "
-                u'E.g.: \'{"pool_recycle": 3600, "echo": true}\' '
+                "Enter the connection parameters in a json form. "
+                'E.g.: \'{"pool_recycle": 3600, "echo": true}\' '
             ),
         ),
         required=True,
-        default=u"",
+        default="",
     )
 
     trackworkingcopies = schema.Bool(
-        title=_(u"Track Working Copy Activity?"),
+        title=_("Track Working Copy Activity?"),
         description=_(
-            u"help_auditlog_trackworkingcopies",
+            "help_auditlog_trackworkingcopies",
             default=(
-                u"When checked AuditLog will track all actions "
-                u"to Working Copies. "
-                u"When unchecked, only cancel check out and check-in actions "
-                u"will be tracked."
+                "When checked AuditLog will track all actions "
+                "to Working Copies. "
+                "When unchecked, only cancel check out and check-in actions "
+                "will be tracked."
             ),
         ),
         required=False,
     )
 
     automaticevents = schema.List(
-        title=_(u"Trigger Without Content Rule"),
+        title=_("Trigger Without Content Rule"),
         description=_(
-            u"help_auditlog_automaticevents",
+            "help_auditlog_automaticevents",
             default=(
-                u"The selected events will not require a content rule "
-                u"to trigger them, so all instances will be logged."
+                "The selected events will not require a content rule "
+                "to trigger them, so all instances will be logged."
             ),
         ),
         default=[],
         value_type=schema.Choice(vocabulary=SimpleVocabulary(EVENT_TYPES_VOCAB)),
     )
 
 
@@ -131,27 +131,27 @@
     object = Attribute("The subject of the event.")
     request = Attribute("The current request.")
     action = Attribute("A title for the performed action.")
     note = Attribute("Additional information for the action.")
 
 
 @implementer(IAuditableActionPerformedEvent)
-class AuditableActionPerformedEvent(object):
+class AuditableActionPerformedEvent:
     def __init__(self, object, request, action, info=None):
         self.object = object
         self.request = request
         self.action = action
         self.info = info
 
 
 class IBeforeStoreAuditlogEntryEvent(Interface):
-    """ Event fired before storing an entry into the auditlog"""
+    """Event fired before storing an entry into the auditlog"""
 
     object = Attribute("The subject of the event.")
     data = Attribute("The data stored in the log")
 
 
 @implementer(IBeforeStoreAuditlogEntryEvent)
-class BeforeStoreAuditlogEntryEvent(object):
+class BeforeStoreAuditlogEntryEvent:
     def __init__(self, object, data):
         self.object = object
         self.data = data
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/testing.py` & `collective.auditlog-3.0.0a1/collective/auditlog/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# coding=utf-8
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 
 
 class AuditLog(PloneSandboxLayer):
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
-        import plone.app.contenttypes
         import collective.auditlog
         import collective.auditlog.asyncqueue
+        import plone.app.contenttypes
 
         self.loadZCML(package=plone.app.contenttypes)
         self.loadZCML(package=collective.auditlog)
 
         collective.auditlog.asyncqueue.queue_job = False
 
     def setUpPloneSite(self, portal):
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/controlpanel.xml` & `collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/controlpanel.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 223f 3e0a 3c6f 626a 6563 7420 786d  .0"?>.<object xm
-00000020: 6c6e 733a 6931 386e 3d22 6874 7470 3a2f  lns:i18n="http:/
-00000030: 2f78 6d6c 2e7a 6f70 652e 6f72 672f 6e61  /xml.zope.org/na
-00000040: 6d65 7370 6163 6573 2f69 3138 6e22 0a20  mespaces/i18n". 
-00000050: 2020 2020 2020 206e 616d 653d 2270 6f72         name="por
-00000060: 7461 6c5f 636f 6e74 726f 6c70 616e 656c  tal_controlpanel
-00000070: 220a 2020 2020 2020 2020 7075 7267 653d  ".        purge=
-00000080: 2246 616c 7365 220a 2020 2020 2020 2020  "False".        
-00000090: 6931 386e 3a64 6f6d 6169 6e3d 2263 6f6c  i18n:domain="col
-000000a0: 6c65 6374 6976 652e 6175 6469 746c 6f67  lective.auditlog
-000000b0: 220a 3e0a 0a20 203c 636f 6e66 6967 6c65  ".>..  <configle
-000000c0: 7420 6163 7469 6f6e 5f69 643d 2261 7564  t action_id="aud
-000000d0: 6974 6c6f 6722 0a20 2020 2020 2020 2020  itlog".         
-000000e0: 2020 2020 6170 7049 643d 2263 6f6c 6c65      appId="colle
-000000f0: 6374 6976 652e 6175 6469 746c 6f67 220a  ctive.auditlog".
-00000100: 2020 2020 2020 2020 2020 2020 2063 6174               cat
-00000110: 6567 6f72 793d 2250 726f 6475 6374 7322  egory="Products"
-00000120: 0a20 2020 2020 2020 2020 2020 2020 636f  .             co
-00000130: 6e64 6974 696f 6e5f 6578 7072 3d22 220a  ndition_expr="".
-00000140: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-00000150: 6c65 3d22 4175 6469 744c 6f67 220a 2020  le="AuditLog".  
-00000160: 2020 2020 2020 2020 2020 2075 726c 5f65             url_e
-00000170: 7870 723d 2273 7472 696e 673a 247b 706f  xpr="string:${po
-00000180: 7274 616c 5f75 726c 7d2f 4040 6175 6469  rtal_url}/@@audi
-00000190: 746c 6f67 2d73 6574 7469 6e67 7322 0a20  tlog-settings". 
-000001a0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
-000001b0: 626c 653d 2254 7275 6522 0a20 2020 2020  ble="True".     
-000001c0: 2020 2020 2020 2020 6931 386e 3a61 7474          i18n:att
-000001d0: 7269 6275 7465 733d 2274 6974 6c65 220a  ributes="title".
-000001e0: 2020 3e0a 2020 2020 3c70 6572 6d69 7373    >.    <permiss
-000001f0: 696f 6e3e 4d61 6e61 6765 2070 6f72 7461  ion>Manage porta
-00000200: 6c3c 2f70 6572 6d69 7373 696f 6e3e 0a20  l</permission>. 
-00000210: 203c 2f63 6f6e 6669 676c 6574 3e0a 0a3c   </configlet>..<
-00000220: 2f6f 626a 6563 743e 0a0a                 /object>..
+00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
+00000020: 662d 3822 3f3e 0a3c 6f62 6a65 6374 2078  f-8"?>.<object x
+00000030: 6d6c 6e73 3a69 3138 6e3d 2268 7474 703a  mlns:i18n="http:
+00000040: 2f2f 786d 6c2e 7a6f 7065 2e6f 7267 2f6e  //xml.zope.org/n
+00000050: 616d 6573 7061 6365 732f 6931 386e 220a  amespaces/i18n".
+00000060: 2020 2020 2020 2020 6e61 6d65 3d22 706f          name="po
+00000070: 7274 616c 5f63 6f6e 7472 6f6c 7061 6e65  rtal_controlpane
+00000080: 6c22 0a20 2020 2020 2020 2070 7572 6765  l".        purge
+00000090: 3d22 4661 6c73 6522 0a20 2020 2020 2020  ="False".       
+000000a0: 2069 3138 6e3a 646f 6d61 696e 3d22 636f   i18n:domain="co
+000000b0: 6c6c 6563 7469 7665 2e61 7564 6974 6c6f  llective.auditlo
+000000c0: 6722 0a3e 0a0a 2020 3c63 6f6e 6669 676c  g".>..  <configl
+000000d0: 6574 2061 6374 696f 6e5f 6964 3d22 6175  et action_id="au
+000000e0: 6469 746c 6f67 220a 2020 2020 2020 2020  ditlog".        
+000000f0: 2020 2020 2061 7070 4964 3d22 636f 6c6c       appId="coll
+00000100: 6563 7469 7665 2e61 7564 6974 6c6f 6722  ective.auditlog"
+00000110: 0a20 2020 2020 2020 2020 2020 2020 6361  .             ca
+00000120: 7465 676f 7279 3d22 5072 6f64 7563 7473  tegory="Products
+00000130: 220a 2020 2020 2020 2020 2020 2020 2063  ".             c
+00000140: 6f6e 6469 7469 6f6e 5f65 7870 723d 2222  ondition_expr=""
+00000150: 0a20 2020 2020 2020 2020 2020 2020 7469  .             ti
+00000160: 746c 653d 2241 7564 6974 4c6f 6722 0a20  tle="AuditLog". 
+00000170: 2020 2020 2020 2020 2020 2020 7572 6c5f              url_
+00000180: 6578 7072 3d22 7374 7269 6e67 3a24 7b70  expr="string:${p
+00000190: 6f72 7461 6c5f 7572 6c7d 2f40 4061 7564  ortal_url}/@@aud
+000001a0: 6974 6c6f 672d 7365 7474 696e 6773 220a  itlog-settings".
+000001b0: 2020 2020 2020 2020 2020 2020 2076 6973               vis
+000001c0: 6962 6c65 3d22 5472 7565 220a 2020 2020  ible="True".    
+000001d0: 2020 2020 2020 2020 2069 3138 6e3a 6174           i18n:at
+000001e0: 7472 6962 7574 6573 3d22 7469 746c 6522  tributes="title"
+000001f0: 0a20 203e 0a20 2020 203c 7065 726d 6973  .  >.    <permis
+00000200: 7369 6f6e 3e4d 616e 6167 6520 706f 7274  sion>Manage port
+00000210: 616c 3c2f 7065 726d 6973 7369 6f6e 3e0a  al</permission>.
+00000220: 2020 3c2f 636f 6e66 6967 6c65 743e 0a0a    </configlet>..
+00000230: 3c2f 6f62 6a65 6374 3e0a                 </object>.
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/contentrules.xml` & `collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/contentrules.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 3% similar despite different names*

```diff
@@ -1,465 +1,458 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 223f 3e0a 3c63 6f6e 7465 6e74 7275  .0"?>.<contentru
-00000020: 6c65 733e 0a20 203c 7275 6c65 2064 6573  les>.  <rule des
-00000030: 6372 6970 7469 6f6e 3d22 5468 6973 2073  cription="This s
-00000040: 746f 7265 7320 616c 6c20 6163 7469 6f6e  tores all action
-00000050: 7320 6f66 2073 656e 6469 6e67 2063 6f6e  s of sending con
-00000060: 7465 6e74 2074 6872 6f75 6768 2077 6f72  tent through wor
-00000070: 6b66 6c6f 7720 696e 746f 2074 6865 2044  kflow into the D
-00000080: 6174 6120 5761 7265 686f 7573 6522 0a20  ata Warehouse". 
-00000090: 2020 2020 2020 2065 6e61 626c 6564 3d22         enabled="
-000000a0: 4661 6c73 6522 0a20 2020 2020 2020 2065  False".        e
-000000b0: 7665 6e74 3d22 5072 6f64 7563 7473 2e43  vent="Products.C
-000000c0: 4d46 436f 7265 2e69 6e74 6572 6661 6365  MFCore.interface
-000000d0: 732e 4941 6374 696f 6e53 7563 6365 6564  s.IActionSucceed
-000000e0: 6564 4576 656e 7422 0a20 2020 2020 2020  edEvent".       
-000000f0: 206e 616d 653d 2272 756c 652d 3130 3022   name="rule-100"
-00000100: 0a20 2020 2020 2020 2073 746f 702d 6166  .        stop-af
-00000110: 7465 723d 2246 616c 7365 220a 2020 2020  ter="False".    
-00000120: 2020 2020 7469 746c 653d 2253 746f 7265      title="Store
-00000130: 2057 6f72 6b66 6c6f 7720 5472 616e 7369   Workflow Transi
-00000140: 7469 6f6e 7322 0a20 203e 0a20 2020 203c  tions".  >.    <
-00000150: 636f 6e64 6974 696f 6e73 3e0a 2020 2020  conditions>.    
-00000160: 2020 3c63 6f6e 6469 7469 6f6e 2074 7970    <condition typ
-00000170: 653d 2270 6c6f 6e65 2e63 6f6e 6469 7469  e="plone.conditi
-00000180: 6f6e 732e 506f 7274 616c 5479 7065 223e  ons.PortalType">
-00000190: 0a20 2020 2020 2020 203c 7072 6f70 6572  .        <proper
-000001a0: 7479 206e 616d 653d 2263 6865 636b 5f74  ty name="check_t
-000001b0: 7970 6573 223e 0a0a 2020 2020 2020 2020  ypes">..        
-000001c0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-000001d0: 2020 3c2f 636f 6e64 6974 696f 6e3e 0a0a    </condition>..
-000001e0: 2020 2020 3c2f 636f 6e64 6974 696f 6e73      </conditions
-000001f0: 3e0a 2020 2020 3c61 6374 696f 6e73 3e0a  >.    <actions>.
-00000200: 2020 2020 2020 3c61 6374 696f 6e20 7479        <action ty
-00000210: 7065 3d22 706c 6f6e 652e 6163 7469 6f6e  pe="plone.action
-00000220: 732e 4175 6469 7422 3e0a 2020 2020 2020  s.Audit">.      
-00000230: 3c2f 6163 7469 6f6e 3e0a 2020 2020 3c2f  </action>.    </
-00000240: 6163 7469 6f6e 733e 0a20 203c 2f72 756c  actions>.  </rul
-00000250: 653e 0a20 203c 7275 6c65 2064 6573 6372  e>.  <rule descr
-00000260: 6970 7469 6f6e 3d22 5468 6973 2073 746f  iption="This sto
-00000270: 7265 7320 7468 6520 6163 7469 6f6e 206f  res the action o
-00000280: 6620 6368 6563 6b69 6e67 206f 7574 2061  f checking out a
-00000290: 6e79 2063 6f6e 7465 6e74 2069 6e74 6f20  ny content into 
-000002a0: 7468 6520 4461 7461 2057 6172 6568 6f75  the Data Warehou
-000002b0: 7365 220a 2020 2020 2020 2020 656e 6162  se".        enab
-000002c0: 6c65 643d 2246 616c 7365 220a 2020 2020  led="False".    
-000002d0: 2020 2020 6576 656e 743d 2270 6c6f 6e65      event="plone
-000002e0: 2e61 7070 2e69 7465 7261 7465 2e69 6e74  .app.iterate.int
-000002f0: 6572 6661 6365 732e 4942 6566 6f72 6543  erfaces.IBeforeC
-00000300: 6865 636b 6f75 7445 7665 6e74 220a 2020  heckoutEvent".  
-00000310: 2020 2020 2020 6e61 6d65 3d22 7275 6c65        name="rule
-00000320: 2d31 3031 220a 2020 2020 2020 2020 7374  -101".        st
-00000330: 6f70 2d61 6674 6572 3d22 4661 6c73 6522  op-after="False"
-00000340: 0a20 2020 2020 2020 2074 6974 6c65 3d22  .        title="
-00000350: 5374 6f72 6520 4368 6563 6b2d 6f75 7422  Store Check-out"
-00000360: 0a20 203e 0a20 2020 203c 636f 6e64 6974  .  >.    <condit
-00000370: 696f 6e73 3e0a 2020 2020 2020 3c63 6f6e  ions>.      <con
-00000380: 6469 7469 6f6e 2074 7970 653d 2270 6c6f  dition type="plo
-00000390: 6e65 2e63 6f6e 6469 7469 6f6e 732e 506f  ne.conditions.Po
-000003a0: 7274 616c 5479 7065 223e 0a20 2020 2020  rtalType">.     
-000003b0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000003c0: 653d 2263 6865 636b 5f74 7970 6573 223e  e="check_types">
-000003d0: 0a0a 2020 2020 2020 2020 3c2f 7072 6f70  ..        </prop
-000003e0: 6572 7479 3e0a 2020 2020 2020 3c2f 636f  erty>.      </co
-000003f0: 6e64 6974 696f 6e3e 0a20 2020 203c 2f63  ndition>.    </c
-00000400: 6f6e 6469 7469 6f6e 733e 0a20 2020 203c  onditions>.    <
-00000410: 6163 7469 6f6e 733e 0a20 2020 2020 203c  actions>.      <
-00000420: 6163 7469 6f6e 2074 7970 653d 2270 6c6f  action type="plo
-00000430: 6e65 2e61 6374 696f 6e73 2e41 7564 6974  ne.actions.Audit
-00000440: 223e 0a20 2020 2020 203c 2f61 6374 696f  ">.      </actio
-00000450: 6e3e 0a20 2020 203c 2f61 6374 696f 6e73  n>.    </actions
-00000460: 3e0a 2020 3c2f 7275 6c65 3e0a 2020 3c72  >.  </rule>.  <r
-00000470: 756c 6520 6465 7363 7269 7074 696f 6e3d  ule description=
-00000480: 2254 6869 7320 7374 6f72 6573 2074 6865  "This stores the
-00000490: 2061 6374 696f 6e20 6f66 2063 616e 6365   action of cance
-000004a0: 6c6c 696e 6720 6120 6368 6563 6b6f 7574  lling a checkout
-000004b0: 206f 6620 616e 7920 636f 6e74 656e 7420   of any content 
-000004c0: 696e 746f 2074 6865 2044 6174 6120 5761  into the Data Wa
-000004d0: 7265 686f 7573 6522 0a20 2020 2020 2020  rehouse".       
-000004e0: 2065 6e61 626c 6564 3d22 4661 6c73 6522   enabled="False"
-000004f0: 0a20 2020 2020 2020 2065 7665 6e74 3d22  .        event="
-00000500: 706c 6f6e 652e 6170 702e 6974 6572 6174  plone.app.iterat
-00000510: 652e 696e 7465 7266 6163 6573 2e49 4361  e.interfaces.ICa
-00000520: 6e63 656c 4368 6563 6b6f 7574 4576 656e  ncelCheckoutEven
-00000530: 7422 0a20 2020 2020 2020 206e 616d 653d  t".        name=
-00000540: 2272 756c 652d 3130 3222 0a20 2020 2020  "rule-102".     
-00000550: 2020 2073 746f 702d 6166 7465 723d 2246     stop-after="F
-00000560: 616c 7365 220a 2020 2020 2020 2020 7469  alse".        ti
-00000570: 746c 653d 2253 746f 7265 2043 616e 6365  tle="Store Cance
-00000580: 6c20 6368 6563 6b6f 7574 220a 2020 3e0a  l checkout".  >.
-00000590: 2020 2020 3c63 6f6e 6469 7469 6f6e 733e      <conditions>
-000005a0: 0a20 2020 2020 203c 636f 6e64 6974 696f  .      <conditio
-000005b0: 6e20 7479 7065 3d22 706c 6f6e 652e 636f  n type="plone.co
-000005c0: 6e64 6974 696f 6e73 2e50 6f72 7461 6c54  nditions.PortalT
-000005d0: 7970 6522 3e0a 2020 2020 2020 2020 3c70  ype">.        <p
-000005e0: 726f 7065 7274 7920 6e61 6d65 3d22 6368  roperty name="ch
-000005f0: 6563 6b5f 7479 7065 7322 3e0a 0a20 2020  eck_types">..   
-00000600: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000610: 0a20 2020 2020 203c 2f63 6f6e 6469 7469  .      </conditi
-00000620: 6f6e 3e0a 2020 2020 3c2f 636f 6e64 6974  on>.    </condit
-00000630: 696f 6e73 3e0a 2020 2020 3c61 6374 696f  ions>.    <actio
-00000640: 6e73 3e0a 2020 2020 2020 3c61 6374 696f  ns>.      <actio
-00000650: 6e20 7479 7065 3d22 706c 6f6e 652e 6163  n type="plone.ac
-00000660: 7469 6f6e 732e 4175 6469 7422 3e0a 2020  tions.Audit">.  
-00000670: 2020 2020 3c2f 6163 7469 6f6e 3e0a 2020      </action>.  
-00000680: 2020 3c2f 6163 7469 6f6e 733e 0a20 203c    </actions>.  <
-00000690: 2f72 756c 653e 0a20 203c 7275 6c65 2064  /rule>.  <rule d
-000006a0: 6573 6372 6970 7469 6f6e 3d22 5468 6973  escription="This
-000006b0: 2073 746f 7265 7320 7468 6520 6163 7469   stores the acti
-000006c0: 6f6e 206f 6620 6368 6563 6b69 6e67 2069  on of checking i
-000006d0: 6e20 616e 7920 636f 6e74 656e 7420 696e  n any content in
-000006e0: 746f 2074 6865 2044 6174 6120 5761 7265  to the Data Ware
-000006f0: 686f 7573 6522 0a20 2020 2020 2020 2065  house".        e
-00000700: 6e61 626c 6564 3d22 4661 6c73 6522 0a20  nabled="False". 
-00000710: 2020 2020 2020 2065 7665 6e74 3d22 706c         event="pl
-00000720: 6f6e 652e 6170 702e 6974 6572 6174 652e  one.app.iterate.
-00000730: 696e 7465 7266 6163 6573 2e49 4368 6563  interfaces.IChec
-00000740: 6b69 6e45 7665 6e74 220a 2020 2020 2020  kinEvent".      
-00000750: 2020 6e61 6d65 3d22 7275 6c65 2d31 3033    name="rule-103
-00000760: 220a 2020 2020 2020 2020 7374 6f70 2d61  ".        stop-a
-00000770: 6674 6572 3d22 4661 6c73 6522 0a20 2020  fter="False".   
-00000780: 2020 2020 2074 6974 6c65 3d22 5374 6f72       title="Stor
-00000790: 6520 4368 6563 6b2d 496e 220a 2020 3e0a  e Check-In".  >.
-000007a0: 2020 2020 3c63 6f6e 6469 7469 6f6e 733e      <conditions>
-000007b0: 0a20 2020 2020 203c 636f 6e64 6974 696f  .      <conditio
-000007c0: 6e20 7479 7065 3d22 706c 6f6e 652e 636f  n type="plone.co
-000007d0: 6e64 6974 696f 6e73 2e50 6f72 7461 6c54  nditions.PortalT
-000007e0: 7970 6522 3e0a 2020 2020 2020 2020 3c70  ype">.        <p
-000007f0: 726f 7065 7274 7920 6e61 6d65 3d22 6368  roperty name="ch
-00000800: 6563 6b5f 7479 7065 7322 3e0a 2020 2020  eck_types">.    
-00000810: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-00000820: 2020 2020 2020 3c2f 636f 6e64 6974 696f        </conditio
-00000830: 6e3e 0a20 2020 203c 2f63 6f6e 6469 7469  n>.    </conditi
-00000840: 6f6e 733e 0a20 2020 203c 6163 7469 6f6e  ons>.    <action
-00000850: 733e 0a20 2020 2020 203c 6163 7469 6f6e  s>.      <action
-00000860: 2074 7970 653d 2270 6c6f 6e65 2e61 6374   type="plone.act
-00000870: 696f 6e73 2e41 7564 6974 223e 0a20 2020  ions.Audit">.   
-00000880: 2020 203c 2f61 6374 696f 6e3e 0a20 2020     </action>.   
-00000890: 203c 2f61 6374 696f 6e73 3e0a 2020 3c2f   </actions>.  </
-000008a0: 7275 6c65 3e0a 2020 3c72 756c 6520 6465  rule>.  <rule de
-000008b0: 7363 7269 7074 696f 6e3d 2254 6869 7320  scription="This 
-000008c0: 7374 6f72 6573 2074 6865 2061 6374 696f  stores the actio
-000008d0: 6e20 6f66 2061 6e79 2063 6f6e 7465 6e74  n of any content
-000008e0: 2062 6569 6e67 206d 6f76 6564 2066 726f   being moved fro
-000008f0: 6d20 6f6e 6520 636f 6e74 6169 6e65 7220  m one container 
-00000900: 746f 2061 6e6f 7468 6572 2028 4375 742f  to another (Cut/
-00000910: 5061 7374 6529 2069 6e74 6f20 7468 6520  Paste) into the 
-00000920: 4461 7461 2057 6172 6568 6f75 7365 220a  Data Warehouse".
-00000930: 2020 2020 2020 2020 656e 6162 6c65 643d          enabled=
-00000940: 2246 616c 7365 220a 2020 2020 2020 2020  "False".        
-00000950: 6576 656e 743d 227a 6f70 652e 6c69 6665  event="zope.life
-00000960: 6379 636c 6565 7665 6e74 2e69 6e74 6572  cycleevent.inter
-00000970: 6661 6365 732e 494f 626a 6563 744d 6f76  faces.IObjectMov
-00000980: 6564 4576 656e 7422 0a20 2020 2020 2020  edEvent".       
-00000990: 206e 616d 653d 2272 756c 652d 3130 3422   name="rule-104"
-000009a0: 0a20 2020 2020 2020 2073 746f 702d 6166  .        stop-af
-000009b0: 7465 723d 2246 616c 7365 220a 2020 2020  ter="False".    
-000009c0: 2020 2020 7469 746c 653d 2253 746f 7265      title="Store
-000009d0: 204f 626a 6563 7420 4d6f 7665 6422 0a20   Object Moved". 
-000009e0: 203e 0a20 2020 203c 636f 6e64 6974 696f   >.    <conditio
-000009f0: 6e73 3e0a 2020 2020 2020 3c63 6f6e 6469  ns>.      <condi
-00000a00: 7469 6f6e 2074 7970 653d 2270 6c6f 6e65  tion type="plone
-00000a10: 2e63 6f6e 6469 7469 6f6e 732e 506f 7274  .conditions.Port
-00000a20: 616c 5479 7065 223e 0a20 2020 2020 2020  alType">.       
-00000a30: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00000a40: 2263 6865 636b 5f74 7970 6573 223e 0a20  "check_types">. 
-00000a50: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00000a60: 793e 0a20 2020 2020 203c 2f63 6f6e 6469  y>.      </condi
-00000a70: 7469 6f6e 3e0a 2020 2020 3c2f 636f 6e64  tion>.    </cond
-00000a80: 6974 696f 6e73 3e0a 2020 2020 3c61 6374  itions>.    <act
-00000a90: 696f 6e73 3e0a 2020 2020 2020 3c61 6374  ions>.      <act
-00000aa0: 696f 6e20 7479 7065 3d22 706c 6f6e 652e  ion type="plone.
-00000ab0: 6163 7469 6f6e 732e 4175 6469 7422 3e0a  actions.Audit">.
-00000ac0: 2020 2020 2020 3c2f 6163 7469 6f6e 3e0a        </action>.
-00000ad0: 2020 2020 3c2f 6163 7469 6f6e 733e 0a20      </actions>. 
-00000ae0: 203c 2f72 756c 653e 0a20 203c 7275 6c65   </rule>.  <rule
-00000af0: 2064 6573 6372 6970 7469 6f6e 3d22 5468   description="Th
-00000b00: 6973 2073 746f 7265 7320 7468 6520 6163  is stores the ac
-00000b10: 7469 6f6e 206f 6620 6465 6c65 7469 6e67  tion of deleting
-00000b20: 2061 6e79 2063 6f6e 7465 6e74 2066 726f   any content fro
-00000b30: 6d20 6120 636f 6e74 6169 6e65 722e 2054  m a container. T
-00000b40: 6869 7320 6973 206f 6e6c 7920 7472 6967  his is only trig
-00000b50: 6765 7265 6420 7768 656e 204c 696e 6b20  gered when Link 
-00000b60: 496e 7465 6772 6974 7920 6861 7320 6265  Integrity has be
-00000b70: 656e 2074 7269 6767 6572 6564 2061 6e64  en triggered and
-00000b80: 2063 6f6e 6669 726d 6564 2e22 0a20 2020   confirmed.".   
-00000b90: 2020 2020 2065 6e61 626c 6564 3d22 4661       enabled="Fa
-00000ba0: 6c73 6522 0a20 2020 2020 2020 2065 7665  lse".        eve
-00000bb0: 6e74 3d22 7a6f 7065 2e6c 6966 6563 7963  nt="zope.lifecyc
-00000bc0: 6c65 6576 656e 742e 696e 7465 7266 6163  leevent.interfac
-00000bd0: 6573 2e49 4f62 6a65 6374 5265 6d6f 7665  es.IObjectRemove
-00000be0: 6445 7665 6e74 220a 2020 2020 2020 2020  dEvent".        
-00000bf0: 6e61 6d65 3d22 7275 6c65 2d31 3035 220a  name="rule-105".
-00000c00: 2020 2020 2020 2020 7374 6f70 2d61 6674          stop-aft
-00000c10: 6572 3d22 4661 6c73 6522 0a20 2020 2020  er="False".     
-00000c20: 2020 2074 6974 6c65 3d22 5374 6f72 6520     title="Store 
-00000c30: 4f62 6a65 6374 2044 656c 6574 6564 220a  Object Deleted".
-00000c40: 2020 3e0a 2020 2020 3c63 6f6e 6469 7469    >.    <conditi
-00000c50: 6f6e 733e 0a20 2020 2020 203c 636f 6e64  ons>.      <cond
-00000c60: 6974 696f 6e20 7479 7065 3d22 706c 6f6e  ition type="plon
-00000c70: 652e 636f 6e64 6974 696f 6e73 2e50 6f72  e.conditions.Por
-00000c80: 7461 6c54 7970 6522 3e0a 2020 2020 2020  talType">.      
-00000c90: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000ca0: 3d22 6368 6563 6b5f 7479 7065 7322 3e0a  ="check_types">.
-00000cb0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00000cc0: 7479 3e0a 2020 2020 2020 3c2f 636f 6e64  ty>.      </cond
-00000cd0: 6974 696f 6e3e 0a20 2020 203c 2f63 6f6e  ition>.    </con
-00000ce0: 6469 7469 6f6e 733e 0a20 2020 203c 6163  ditions>.    <ac
-00000cf0: 7469 6f6e 733e 0a20 2020 2020 203c 6163  tions>.      <ac
-00000d00: 7469 6f6e 2074 7970 653d 2270 6c6f 6e65  tion type="plone
-00000d10: 2e61 6374 696f 6e73 2e41 7564 6974 223e  .actions.Audit">
-00000d20: 0a20 2020 2020 203c 2f61 6374 696f 6e3e  .      </action>
-00000d30: 0a20 2020 203c 2f61 6374 696f 6e73 3e0a  .    </actions>.
-00000d40: 2020 3c2f 7275 6c65 3e0a 2020 3c72 756c    </rule>.  <rul
-00000d50: 6520 6465 7363 7269 7074 696f 6e3d 2254  e description="T
-00000d60: 6869 7320 7374 6f72 6573 2074 6865 2061  his stores the a
-00000d70: 6374 696f 6e20 6f66 2065 6469 7469 6e67  ction of editing
-00000d80: 2061 6e79 2063 6f6e 7465 6e74 2069 6e74   any content int
-00000d90: 6f20 7468 6520 4461 7461 2057 6172 6568  o the Data Wareh
-00000da0: 6f75 7365 220a 2020 2020 2020 2020 656e  ouse".        en
-00000db0: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
-00000dc0: 2020 2020 2020 6576 656e 743d 227a 6f70        event="zop
-00000dd0: 652e 6c69 6665 6379 636c 6565 7665 6e74  e.lifecycleevent
-00000de0: 2e69 6e74 6572 6661 6365 732e 494f 626a  .interfaces.IObj
-00000df0: 6563 744d 6f64 6966 6965 6445 7665 6e74  ectModifiedEvent
-00000e00: 220a 2020 2020 2020 2020 6e61 6d65 3d22  ".        name="
-00000e10: 7275 6c65 2d31 3036 220a 2020 2020 2020  rule-106".      
-00000e20: 2020 7374 6f70 2d61 6674 6572 3d22 4661    stop-after="Fa
-00000e30: 6c73 6522 0a20 2020 2020 2020 2074 6974  lse".        tit
-00000e40: 6c65 3d22 5374 6f72 6520 4f62 6a65 6374  le="Store Object
-00000e50: 2045 6469 7473 220a 2020 3e0a 2020 2020   Edits".  >.    
-00000e60: 3c63 6f6e 6469 7469 6f6e 733e 0a20 2020  <conditions>.   
-00000e70: 2020 203c 636f 6e64 6974 696f 6e20 7479     <condition ty
-00000e80: 7065 3d22 706c 6f6e 652e 636f 6e64 6974  pe="plone.condit
-00000e90: 696f 6e73 2e50 6f72 7461 6c54 7970 6522  ions.PortalType"
-00000ea0: 3e0a 2020 2020 2020 2020 3c70 726f 7065  >.        <prope
-00000eb0: 7274 7920 6e61 6d65 3d22 6368 6563 6b5f  rty name="check_
-00000ec0: 7479 7065 7322 3e0a 2020 2020 2020 2020  types">.        
-00000ed0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00000ee0: 2020 3c2f 636f 6e64 6974 696f 6e3e 0a20    </condition>. 
-00000ef0: 2020 203c 2f63 6f6e 6469 7469 6f6e 733e     </conditions>
-00000f00: 0a20 2020 203c 6163 7469 6f6e 733e 0a20  .    <actions>. 
-00000f10: 2020 2020 203c 6163 7469 6f6e 2074 7970       <action typ
-00000f20: 653d 2270 6c6f 6e65 2e61 6374 696f 6e73  e="plone.actions
-00000f30: 2e41 7564 6974 223e 0a20 2020 2020 203c  .Audit">.      <
-00000f40: 2f61 6374 696f 6e3e 0a20 2020 203c 2f61  /action>.    </a
-00000f50: 6374 696f 6e73 3e0a 2020 3c2f 7275 6c65  ctions>.  </rule
-00000f60: 3e0a 2020 3c72 756c 6520 6465 7363 7269  >.  <rule descri
-00000f70: 7074 696f 6e3d 2254 6869 7320 7374 6f72  ption="This stor
-00000f80: 6573 2074 6865 2061 6374 696f 6e20 6f66  es the action of
-00000f90: 2061 6464 696e 6720 616e 7920 6e65 7720   adding any new 
-00000fa0: 6f62 6a65 6374 7320 746f 2061 2063 6f6e  objects to a con
-00000fb0: 7461 696e 6572 2069 6e74 6f20 7468 6520  tainer into the 
-00000fc0: 4461 7461 2057 6172 6568 6f75 7365 220a  Data Warehouse".
-00000fd0: 2020 2020 2020 2020 656e 6162 6c65 643d          enabled=
-00000fe0: 2246 616c 7365 220a 2020 2020 2020 2020  "False".        
-00000ff0: 6576 656e 743d 227a 6f70 652e 6c69 6665  event="zope.life
-00001000: 6379 636c 6565 7665 6e74 2e69 6e74 6572  cycleevent.inter
-00001010: 6661 6365 732e 494f 626a 6563 7443 7265  faces.IObjectCre
-00001020: 6174 6564 4576 656e 7422 0a20 2020 2020  atedEvent".     
-00001030: 2020 206e 616d 653d 2272 756c 652d 3130     name="rule-10
-00001040: 3722 0a20 2020 2020 2020 2073 746f 702d  7".        stop-
-00001050: 6166 7465 723d 2246 616c 7365 220a 2020  after="False".  
-00001060: 2020 2020 2020 7469 746c 653d 2253 746f        title="Sto
-00001070: 7265 204f 626a 6563 7420 4164 6465 6422  re Object Added"
-00001080: 0a20 203e 0a20 2020 203c 636f 6e64 6974  .  >.    <condit
-00001090: 696f 6e73 3e0a 2020 2020 2020 3c63 6f6e  ions>.      <con
-000010a0: 6469 7469 6f6e 2074 7970 653d 2270 6c6f  dition type="plo
-000010b0: 6e65 2e63 6f6e 6469 7469 6f6e 732e 506f  ne.conditions.Po
-000010c0: 7274 616c 5479 7065 223e 0a20 2020 2020  rtalType">.     
-000010d0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000010e0: 653d 2263 6865 636b 5f74 7970 6573 223e  e="check_types">
-000010f0: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
-00001100: 7274 793e 0a20 2020 2020 203c 2f63 6f6e  rty>.      </con
-00001110: 6469 7469 6f6e 3e0a 2020 2020 3c2f 636f  dition>.    </co
-00001120: 6e64 6974 696f 6e73 3e0a 2020 2020 3c61  nditions>.    <a
-00001130: 6374 696f 6e73 3e0a 2020 2020 2020 3c61  ctions>.      <a
-00001140: 6374 696f 6e20 7479 7065 3d22 706c 6f6e  ction type="plon
-00001150: 652e 6163 7469 6f6e 732e 4175 6469 7422  e.actions.Audit"
-00001160: 3e0a 2020 2020 2020 3c2f 6163 7469 6f6e  >.      </action
-00001170: 3e0a 2020 2020 3c2f 6163 7469 6f6e 733e  >.    </actions>
-00001180: 0a20 203c 2f72 756c 653e 0a20 203c 7275  .  </rule>.  <ru
-00001190: 6c65 2064 6573 6372 6970 7469 6f6e 3d22  le description="
-000011a0: 5468 6973 2073 746f 7265 7320 7468 6520  This stores the 
-000011b0: 6163 7469 6f6e 206f 6620 7265 6e61 6d69  action of renami
-000011c0: 6e67 2061 6e79 2063 6f6e 7465 6e74 2069  ng any content i
-000011d0: 6e74 6f20 7468 6520 4461 7461 2057 6172  nto the Data War
-000011e0: 6568 6f75 7365 2e22 0a20 2020 2020 2020  ehouse.".       
-000011f0: 2065 6e61 626c 6564 3d22 4661 6c73 6522   enabled="False"
-00001200: 0a20 2020 2020 2020 2065 7665 6e74 3d22  .        event="
-00001210: 7a6f 7065 2e6c 6966 6563 7963 6c65 6576  zope.lifecycleev
-00001220: 656e 742e 696e 7465 7266 6163 6573 2e49  ent.interfaces.I
-00001230: 4f62 6a65 6374 4d6f 7665 6445 7665 6e74  ObjectMovedEvent
-00001240: 220a 2020 2020 2020 2020 6e61 6d65 3d22  ".        name="
-00001250: 7275 6c65 2d31 3038 220a 2020 2020 2020  rule-108".      
-00001260: 2020 7374 6f70 2d61 6674 6572 3d22 4661    stop-after="Fa
-00001270: 6c73 6522 0a20 2020 2020 2020 2074 6974  lse".        tit
-00001280: 6c65 3d22 5374 6f72 6520 4f62 6a65 6374  le="Store Object
-00001290: 2052 656e 616d 6564 220a 2020 3e0a 2020   Renamed".  >.  
-000012a0: 2020 3c63 6f6e 6469 7469 6f6e 733e 0a20    <conditions>. 
-000012b0: 2020 2020 203c 636f 6e64 6974 696f 6e20       <condition 
-000012c0: 7479 7065 3d22 706c 6f6e 652e 636f 6e64  type="plone.cond
-000012d0: 6974 696f 6e73 2e50 6f72 7461 6c54 7970  itions.PortalTyp
-000012e0: 6522 3e0a 2020 2020 2020 2020 3c70 726f  e">.        <pro
-000012f0: 7065 7274 7920 6e61 6d65 3d22 6368 6563  perty name="chec
-00001300: 6b5f 7479 7065 7322 3e0a 2020 2020 2020  k_types">.      
-00001310: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
-00001320: 2020 2020 3c2f 636f 6e64 6974 696f 6e3e      </condition>
-00001330: 0a20 2020 203c 2f63 6f6e 6469 7469 6f6e  .    </condition
-00001340: 733e 0a20 2020 203c 6163 7469 6f6e 733e  s>.    <actions>
-00001350: 0a20 2020 2020 203c 6163 7469 6f6e 2074  .      <action t
-00001360: 7970 653d 2270 6c6f 6e65 2e61 6374 696f  ype="plone.actio
-00001370: 6e73 2e41 7564 6974 223e 0a20 2020 2020  ns.Audit">.     
-00001380: 203c 2f61 6374 696f 6e3e 0a20 2020 203c   </action>.    <
-00001390: 2f61 6374 696f 6e73 3e0a 2020 3c2f 7275  /actions>.  </ru
-000013a0: 6c65 3e0a 2020 3c72 756c 6520 6465 7363  le>.  <rule desc
-000013b0: 7269 7074 696f 6e3d 2254 6869 7320 7374  ription="This st
-000013c0: 6f72 6573 2074 6865 2061 6374 696f 6e20  ores the action 
-000013d0: 6f66 2063 6f70 6965 6420 616e 7920 636f  of copied any co
-000013e0: 6e74 656e 7420 696e 746f 2074 6865 2044  ntent into the D
-000013f0: 6174 6120 5761 7265 686f 7573 652e 220a  ata Warehouse.".
-00001400: 2020 2020 2020 2020 656e 6162 6c65 643d          enabled=
-00001410: 2246 616c 7365 220a 2020 2020 2020 2020  "False".        
-00001420: 6576 656e 743d 224f 4653 2e69 6e74 6572  event="OFS.inter
-00001430: 6661 6365 732e 494f 626a 6563 7443 6c6f  faces.IObjectClo
-00001440: 6e65 6445 7665 6e74 220a 2020 2020 2020  nedEvent".      
-00001450: 2020 6e61 6d65 3d22 7275 6c65 2d31 3039    name="rule-109
-00001460: 220a 2020 2020 2020 2020 7374 6f70 2d61  ".        stop-a
-00001470: 6674 6572 3d22 4661 6c73 6522 0a20 2020  fter="False".   
-00001480: 2020 2020 2074 6974 6c65 3d22 5374 6f72       title="Stor
-00001490: 6520 4f62 6a65 6374 2043 6f70 6965 6422  e Object Copied"
-000014a0: 0a20 203e 0a20 2020 203c 636f 6e64 6974  .  >.    <condit
-000014b0: 696f 6e73 3e0a 2020 2020 2020 3c63 6f6e  ions>.      <con
-000014c0: 6469 7469 6f6e 2074 7970 653d 2270 6c6f  dition type="plo
-000014d0: 6e65 2e63 6f6e 6469 7469 6f6e 732e 506f  ne.conditions.Po
-000014e0: 7274 616c 5479 7065 223e 0a20 2020 2020  rtalType">.     
-000014f0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00001500: 653d 2263 6865 636b 5f74 7970 6573 223e  e="check_types">
-00001510: 0a20 2020 2020 2020 203c 2f70 726f 7065  .        </prope
-00001520: 7274 793e 0a20 2020 2020 203c 2f63 6f6e  rty>.      </con
-00001530: 6469 7469 6f6e 3e0a 2020 2020 3c2f 636f  dition>.    </co
-00001540: 6e64 6974 696f 6e73 3e0a 2020 2020 3c61  nditions>.    <a
-00001550: 6374 696f 6e73 3e0a 2020 2020 2020 3c61  ctions>.      <a
-00001560: 6374 696f 6e20 7479 7065 3d22 706c 6f6e  ction type="plon
-00001570: 652e 6163 7469 6f6e 732e 4175 6469 7422  e.actions.Audit"
-00001580: 3e0a 2020 2020 2020 3c2f 6163 7469 6f6e  >.      </action
-00001590: 3e0a 2020 2020 3c2f 6163 7469 6f6e 733e  >.    </actions>
-000015a0: 0a20 203c 2f72 756c 653e 0a20 203c 7275  .  </rule>.  <ru
-000015b0: 6c65 2064 6573 6372 6970 7469 6f6e 3d22  le description="
-000015c0: 5468 6973 2073 746f 7265 7320 7468 6520  This stores the 
-000015d0: 6163 7469 6f6e 206f 6620 6164 6469 6e67  action of adding
-000015e0: 2061 6e79 206e 6577 206f 626a 6563 7473   any new objects
-000015f0: 2074 6f20 6120 636f 6e74 6169 6e65 7220   to a container 
-00001600: 696e 746f 2074 6865 2044 6174 6120 5761  into the Data Wa
-00001610: 7265 686f 7573 6522 0a20 2020 2020 2020  rehouse".       
-00001620: 2065 6e61 626c 6564 3d22 4661 6c73 6522   enabled="False"
-00001630: 0a20 2020 2020 2020 2065 7665 6e74 3d22  .        event="
-00001640: 7a6f 7065 2e6c 6966 6563 7963 6c65 6576  zope.lifecycleev
-00001650: 656e 742e 696e 7465 7266 6163 6573 2e49  ent.interfaces.I
-00001660: 4f62 6a65 6374 4164 6465 6445 7665 6e74  ObjectAddedEvent
-00001670: 220a 2020 2020 2020 2020 6e61 6d65 3d22  ".        name="
-00001680: 7275 6c65 2d31 3130 220a 2020 2020 2020  rule-110".      
-00001690: 2020 7374 6f70 2d61 6674 6572 3d22 4661    stop-after="Fa
-000016a0: 6c73 6522 0a20 2020 2020 2020 2074 6974  lse".        tit
-000016b0: 6c65 3d22 5374 6f72 6520 4f62 6a65 6374  le="Store Object
-000016c0: 2041 6464 6564 220a 2020 3e0a 2020 2020   Added".  >.    
-000016d0: 3c63 6f6e 6469 7469 6f6e 733e 0a20 2020  <conditions>.   
-000016e0: 2020 203c 636f 6e64 6974 696f 6e20 7479     <condition ty
-000016f0: 7065 3d22 706c 6f6e 652e 636f 6e64 6974  pe="plone.condit
-00001700: 696f 6e73 2e50 6f72 7461 6c54 7970 6522  ions.PortalType"
-00001710: 3e0a 2020 2020 2020 2020 3c70 726f 7065  >.        <prope
-00001720: 7274 7920 6e61 6d65 3d22 6368 6563 6b5f  rty name="check_
-00001730: 7479 7065 7322 3e0a 2020 2020 2020 2020  types">.        
-00001740: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00001750: 2020 3c2f 636f 6e64 6974 696f 6e3e 0a20    </condition>. 
-00001760: 2020 203c 2f63 6f6e 6469 7469 6f6e 733e     </conditions>
-00001770: 0a20 2020 203c 6163 7469 6f6e 733e 0a20  .    <actions>. 
-00001780: 2020 2020 203c 6163 7469 6f6e 2074 7970       <action typ
-00001790: 653d 2270 6c6f 6e65 2e61 6374 696f 6e73  e="plone.actions
-000017a0: 2e41 7564 6974 223e 0a20 2020 2020 203c  .Audit">.      <
-000017b0: 2f61 6374 696f 6e3e 0a20 2020 203c 2f61  /action>.    </a
-000017c0: 6374 696f 6e73 3e0a 2020 3c2f 7275 6c65  ctions>.  </rule
-000017d0: 3e0a 0a20 203c 6173 7369 676e 6d65 6e74  >..  <assignment
-000017e0: 2062 7562 626c 6573 3d22 5472 7565 220a   bubbles="True".
-000017f0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00001800: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
-00001810: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001820: 7469 6f6e 3d22 220a 2020 2020 2020 2020  tion="".        
-00001830: 2020 2020 2020 6e61 6d65 3d22 7275 6c65        name="rule
-00001840: 2d31 3030 220a 2020 2f3e 0a20 203c 6173  -100".  />.  <as
-00001850: 7369 676e 6d65 6e74 2062 7562 626c 6573  signment bubbles
-00001860: 3d22 5472 7565 220a 2020 2020 2020 2020  ="True".        
-00001870: 2020 2020 2020 656e 6162 6c65 643d 2246        enabled="F
-00001880: 616c 7365 220a 2020 2020 2020 2020 2020  alse".          
-00001890: 2020 2020 6c6f 6361 7469 6f6e 3d22 220a      location="".
-000018a0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-000018b0: 6d65 3d22 7275 6c65 2d31 3031 220a 2020  me="rule-101".  
-000018c0: 2f3e 0a20 203c 6173 7369 676e 6d65 6e74  />.  <assignment
-000018d0: 2062 7562 626c 6573 3d22 5472 7565 220a   bubbles="True".
-000018e0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-000018f0: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
-00001900: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001910: 7469 6f6e 3d22 220a 2020 2020 2020 2020  tion="".        
-00001920: 2020 2020 2020 6e61 6d65 3d22 7275 6c65        name="rule
-00001930: 2d31 3032 220a 2020 2f3e 0a20 203c 6173  -102".  />.  <as
-00001940: 7369 676e 6d65 6e74 2062 7562 626c 6573  signment bubbles
-00001950: 3d22 5472 7565 220a 2020 2020 2020 2020  ="True".        
-00001960: 2020 2020 2020 656e 6162 6c65 643d 2246        enabled="F
-00001970: 616c 7365 220a 2020 2020 2020 2020 2020  alse".          
-00001980: 2020 2020 6c6f 6361 7469 6f6e 3d22 220a      location="".
-00001990: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-000019a0: 6d65 3d22 7275 6c65 2d31 3033 220a 2020  me="rule-103".  
-000019b0: 2f3e 0a20 203c 6173 7369 676e 6d65 6e74  />.  <assignment
-000019c0: 2062 7562 626c 6573 3d22 5472 7565 220a   bubbles="True".
-000019d0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-000019e0: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
-000019f0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001a00: 7469 6f6e 3d22 220a 2020 2020 2020 2020  tion="".        
-00001a10: 2020 2020 2020 6e61 6d65 3d22 7275 6c65        name="rule
-00001a20: 2d31 3034 220a 2020 2f3e 0a20 203c 6173  -104".  />.  <as
-00001a30: 7369 676e 6d65 6e74 2062 7562 626c 6573  signment bubbles
-00001a40: 3d22 5472 7565 220a 2020 2020 2020 2020  ="True".        
-00001a50: 2020 2020 2020 656e 6162 6c65 643d 2246        enabled="F
-00001a60: 616c 7365 220a 2020 2020 2020 2020 2020  alse".          
-00001a70: 2020 2020 6c6f 6361 7469 6f6e 3d22 220a      location="".
-00001a80: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00001a90: 6d65 3d22 7275 6c65 2d31 3035 220a 2020  me="rule-105".  
-00001aa0: 2f3e 0a20 203c 6173 7369 676e 6d65 6e74  />.  <assignment
-00001ab0: 2062 7562 626c 6573 3d22 5472 7565 220a   bubbles="True".
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00001ad0: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
-00001ae0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001af0: 7469 6f6e 3d22 220a 2020 2020 2020 2020  tion="".        
-00001b00: 2020 2020 2020 6e61 6d65 3d22 7275 6c65        name="rule
-00001b10: 2d31 3036 220a 2020 2f3e 0a20 203c 6173  -106".  />.  <as
-00001b20: 7369 676e 6d65 6e74 2062 7562 626c 6573  signment bubbles
-00001b30: 3d22 5472 7565 220a 2020 2020 2020 2020  ="True".        
-00001b40: 2020 2020 2020 656e 6162 6c65 643d 2246        enabled="F
-00001b50: 616c 7365 220a 2020 2020 2020 2020 2020  alse".          
-00001b60: 2020 2020 6c6f 6361 7469 6f6e 3d22 220a      location="".
-00001b70: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00001b80: 6d65 3d22 7275 6c65 2d31 3037 220a 2020  me="rule-107".  
-00001b90: 2f3e 0a20 203c 6173 7369 676e 6d65 6e74  />.  <assignment
-00001ba0: 2062 7562 626c 6573 3d22 5472 7565 220a   bubbles="True".
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00001bc0: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
-00001bd0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001be0: 7469 6f6e 3d22 220a 2020 2020 2020 2020  tion="".        
-00001bf0: 2020 2020 2020 6e61 6d65 3d22 7275 6c65        name="rule
-00001c00: 2d31 3038 220a 2020 2f3e 0a20 203c 6173  -108".  />.  <as
-00001c10: 7369 676e 6d65 6e74 2062 7562 626c 6573  signment bubbles
-00001c20: 3d22 5472 7565 220a 2020 2020 2020 2020  ="True".        
-00001c30: 2020 2020 2020 656e 6162 6c65 643d 2246        enabled="F
-00001c40: 616c 7365 220a 2020 2020 2020 2020 2020  alse".          
-00001c50: 2020 2020 6c6f 6361 7469 6f6e 3d22 220a      location="".
-00001c60: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00001c70: 6d65 3d22 7275 6c65 2d31 3039 220a 2020  me="rule-109".  
-00001c80: 2f3e 0a20 203c 6173 7369 676e 6d65 6e74  />.  <assignment
-00001c90: 2062 7562 626c 6573 3d22 5472 7565 220a   bubbles="True".
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00001cb0: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
-00001cc0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001cd0: 7469 6f6e 3d22 220a 2020 2020 2020 2020  tion="".        
-00001ce0: 2020 2020 2020 6e61 6d65 3d22 7275 6c65        name="rule
-00001cf0: 2d31 3130 220a 2020 2f3e 0a0a 3c2f 636f  -110".  />..</co
-00001d00: 6e74 656e 7472 756c 6573 3e0a            ntentrules>.
+00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
+00000020: 662d 3822 3f3e 0a3c 636f 6e74 656e 7472  f-8"?>.<contentr
+00000030: 756c 6573 3e0a 2020 3c72 756c 6520 6465  ules>.  <rule de
+00000040: 7363 7269 7074 696f 6e3d 2254 6869 7320  scription="This 
+00000050: 7374 6f72 6573 2061 6c6c 2061 6374 696f  stores all actio
+00000060: 6e73 206f 6620 7365 6e64 696e 6720 636f  ns of sending co
+00000070: 6e74 656e 7420 7468 726f 7567 6820 776f  ntent through wo
+00000080: 726b 666c 6f77 2069 6e74 6f20 7468 6520  rkflow into the 
+00000090: 4461 7461 2057 6172 6568 6f75 7365 220a  Data Warehouse".
+000000a0: 2020 2020 2020 2020 656e 6162 6c65 643d          enabled=
+000000b0: 2246 616c 7365 220a 2020 2020 2020 2020  "False".        
+000000c0: 6576 656e 743d 2250 726f 6475 6374 732e  event="Products.
+000000d0: 434d 4643 6f72 652e 696e 7465 7266 6163  CMFCore.interfac
+000000e0: 6573 2e49 4163 7469 6f6e 5375 6363 6565  es.IActionSuccee
+000000f0: 6465 6445 7665 6e74 220a 2020 2020 2020  dedEvent".      
+00000100: 2020 6e61 6d65 3d22 7275 6c65 2d31 3030    name="rule-100
+00000110: 220a 2020 2020 2020 2020 7374 6f70 2d61  ".        stop-a
+00000120: 6674 6572 3d22 4661 6c73 6522 0a20 2020  fter="False".   
+00000130: 2020 2020 2074 6974 6c65 3d22 5374 6f72       title="Stor
+00000140: 6520 576f 726b 666c 6f77 2054 7261 6e73  e Workflow Trans
+00000150: 6974 696f 6e73 220a 2020 3e0a 2020 2020  itions".  >.    
+00000160: 3c63 6f6e 6469 7469 6f6e 733e 0a20 2020  <conditions>.   
+00000170: 2020 203c 636f 6e64 6974 696f 6e20 7479     <condition ty
+00000180: 7065 3d22 706c 6f6e 652e 636f 6e64 6974  pe="plone.condit
+00000190: 696f 6e73 2e50 6f72 7461 6c54 7970 6522  ions.PortalType"
+000001a0: 3e0a 2020 2020 2020 2020 3c70 726f 7065  >.        <prope
+000001b0: 7274 7920 6e61 6d65 3d22 6368 6563 6b5f  rty name="check_
+000001c0: 7479 7065 7322 3e0a 0a20 2020 2020 2020  types">..       
+000001d0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+000001e0: 2020 203c 2f63 6f6e 6469 7469 6f6e 3e0a     </condition>.
+000001f0: 0a20 2020 203c 2f63 6f6e 6469 7469 6f6e  .    </condition
+00000200: 733e 0a20 2020 203c 6163 7469 6f6e 733e  s>.    <actions>
+00000210: 0a20 2020 2020 203c 6163 7469 6f6e 2074  .      <action t
+00000220: 7970 653d 2270 6c6f 6e65 2e61 6374 696f  ype="plone.actio
+00000230: 6e73 2e41 7564 6974 223e 0a3c 2f61 6374  ns.Audit">.</act
+00000240: 696f 6e3e 0a20 2020 203c 2f61 6374 696f  ion>.    </actio
+00000250: 6e73 3e0a 2020 3c2f 7275 6c65 3e0a 2020  ns>.  </rule>.  
+00000260: 3c72 756c 6520 6465 7363 7269 7074 696f  <rule descriptio
+00000270: 6e3d 2254 6869 7320 7374 6f72 6573 2074  n="This stores t
+00000280: 6865 2061 6374 696f 6e20 6f66 2063 6865  he action of che
+00000290: 636b 696e 6720 6f75 7420 616e 7920 636f  cking out any co
+000002a0: 6e74 656e 7420 696e 746f 2074 6865 2044  ntent into the D
+000002b0: 6174 6120 5761 7265 686f 7573 6522 0a20  ata Warehouse". 
+000002c0: 2020 2020 2020 2065 6e61 626c 6564 3d22         enabled="
+000002d0: 4661 6c73 6522 0a20 2020 2020 2020 2065  False".        e
+000002e0: 7665 6e74 3d22 706c 6f6e 652e 6170 702e  vent="plone.app.
+000002f0: 6974 6572 6174 652e 696e 7465 7266 6163  iterate.interfac
+00000300: 6573 2e49 4265 666f 7265 4368 6563 6b6f  es.IBeforeChecko
+00000310: 7574 4576 656e 7422 0a20 2020 2020 2020  utEvent".       
+00000320: 206e 616d 653d 2272 756c 652d 3130 3122   name="rule-101"
+00000330: 0a20 2020 2020 2020 2073 746f 702d 6166  .        stop-af
+00000340: 7465 723d 2246 616c 7365 220a 2020 2020  ter="False".    
+00000350: 2020 2020 7469 746c 653d 2253 746f 7265      title="Store
+00000360: 2043 6865 636b 2d6f 7574 220a 2020 3e0a   Check-out".  >.
+00000370: 2020 2020 3c63 6f6e 6469 7469 6f6e 733e      <conditions>
+00000380: 0a20 2020 2020 203c 636f 6e64 6974 696f  .      <conditio
+00000390: 6e20 7479 7065 3d22 706c 6f6e 652e 636f  n type="plone.co
+000003a0: 6e64 6974 696f 6e73 2e50 6f72 7461 6c54  nditions.PortalT
+000003b0: 7970 6522 3e0a 2020 2020 2020 2020 3c70  ype">.        <p
+000003c0: 726f 7065 7274 7920 6e61 6d65 3d22 6368  roperty name="ch
+000003d0: 6563 6b5f 7479 7065 7322 3e0a 0a20 2020  eck_types">..   
+000003e0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+000003f0: 0a20 2020 2020 203c 2f63 6f6e 6469 7469  .      </conditi
+00000400: 6f6e 3e0a 2020 2020 3c2f 636f 6e64 6974  on>.    </condit
+00000410: 696f 6e73 3e0a 2020 2020 3c61 6374 696f  ions>.    <actio
+00000420: 6e73 3e0a 2020 2020 2020 3c61 6374 696f  ns>.      <actio
+00000430: 6e20 7479 7065 3d22 706c 6f6e 652e 6163  n type="plone.ac
+00000440: 7469 6f6e 732e 4175 6469 7422 3e0a 3c2f  tions.Audit">.</
+00000450: 6163 7469 6f6e 3e0a 2020 2020 3c2f 6163  action>.    </ac
+00000460: 7469 6f6e 733e 0a20 203c 2f72 756c 653e  tions>.  </rule>
+00000470: 0a20 203c 7275 6c65 2064 6573 6372 6970  .  <rule descrip
+00000480: 7469 6f6e 3d22 5468 6973 2073 746f 7265  tion="This store
+00000490: 7320 7468 6520 6163 7469 6f6e 206f 6620  s the action of 
+000004a0: 6361 6e63 656c 6c69 6e67 2061 2063 6865  cancelling a che
+000004b0: 636b 6f75 7420 6f66 2061 6e79 2063 6f6e  ckout of any con
+000004c0: 7465 6e74 2069 6e74 6f20 7468 6520 4461  tent into the Da
+000004d0: 7461 2057 6172 6568 6f75 7365 220a 2020  ta Warehouse".  
+000004e0: 2020 2020 2020 656e 6162 6c65 643d 2246        enabled="F
+000004f0: 616c 7365 220a 2020 2020 2020 2020 6576  alse".        ev
+00000500: 656e 743d 2270 6c6f 6e65 2e61 7070 2e69  ent="plone.app.i
+00000510: 7465 7261 7465 2e69 6e74 6572 6661 6365  terate.interface
+00000520: 732e 4943 616e 6365 6c43 6865 636b 6f75  s.ICancelCheckou
+00000530: 7445 7665 6e74 220a 2020 2020 2020 2020  tEvent".        
+00000540: 6e61 6d65 3d22 7275 6c65 2d31 3032 220a  name="rule-102".
+00000550: 2020 2020 2020 2020 7374 6f70 2d61 6674          stop-aft
+00000560: 6572 3d22 4661 6c73 6522 0a20 2020 2020  er="False".     
+00000570: 2020 2074 6974 6c65 3d22 5374 6f72 6520     title="Store 
+00000580: 4361 6e63 656c 2063 6865 636b 6f75 7422  Cancel checkout"
+00000590: 0a20 203e 0a20 2020 203c 636f 6e64 6974  .  >.    <condit
+000005a0: 696f 6e73 3e0a 2020 2020 2020 3c63 6f6e  ions>.      <con
+000005b0: 6469 7469 6f6e 2074 7970 653d 2270 6c6f  dition type="plo
+000005c0: 6e65 2e63 6f6e 6469 7469 6f6e 732e 506f  ne.conditions.Po
+000005d0: 7274 616c 5479 7065 223e 0a20 2020 2020  rtalType">.     
+000005e0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+000005f0: 653d 2263 6865 636b 5f74 7970 6573 223e  e="check_types">
+00000600: 0a0a 2020 2020 2020 2020 3c2f 7072 6f70  ..        </prop
+00000610: 6572 7479 3e0a 2020 2020 2020 3c2f 636f  erty>.      </co
+00000620: 6e64 6974 696f 6e3e 0a20 2020 203c 2f63  ndition>.    </c
+00000630: 6f6e 6469 7469 6f6e 733e 0a20 2020 203c  onditions>.    <
+00000640: 6163 7469 6f6e 733e 0a20 2020 2020 203c  actions>.      <
+00000650: 6163 7469 6f6e 2074 7970 653d 2270 6c6f  action type="plo
+00000660: 6e65 2e61 6374 696f 6e73 2e41 7564 6974  ne.actions.Audit
+00000670: 223e 0a3c 2f61 6374 696f 6e3e 0a20 2020  ">.</action>.   
+00000680: 203c 2f61 6374 696f 6e73 3e0a 2020 3c2f   </actions>.  </
+00000690: 7275 6c65 3e0a 2020 3c72 756c 6520 6465  rule>.  <rule de
+000006a0: 7363 7269 7074 696f 6e3d 2254 6869 7320  scription="This 
+000006b0: 7374 6f72 6573 2074 6865 2061 6374 696f  stores the actio
+000006c0: 6e20 6f66 2063 6865 636b 696e 6720 696e  n of checking in
+000006d0: 2061 6e79 2063 6f6e 7465 6e74 2069 6e74   any content int
+000006e0: 6f20 7468 6520 4461 7461 2057 6172 6568  o the Data Wareh
+000006f0: 6f75 7365 220a 2020 2020 2020 2020 656e  ouse".        en
+00000700: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
+00000710: 2020 2020 2020 6576 656e 743d 2270 6c6f        event="plo
+00000720: 6e65 2e61 7070 2e69 7465 7261 7465 2e69  ne.app.iterate.i
+00000730: 6e74 6572 6661 6365 732e 4943 6865 636b  nterfaces.ICheck
+00000740: 696e 4576 656e 7422 0a20 2020 2020 2020  inEvent".       
+00000750: 206e 616d 653d 2272 756c 652d 3130 3322   name="rule-103"
+00000760: 0a20 2020 2020 2020 2073 746f 702d 6166  .        stop-af
+00000770: 7465 723d 2246 616c 7365 220a 2020 2020  ter="False".    
+00000780: 2020 2020 7469 746c 653d 2253 746f 7265      title="Store
+00000790: 2043 6865 636b 2d49 6e22 0a20 203e 0a20   Check-In".  >. 
+000007a0: 2020 203c 636f 6e64 6974 696f 6e73 3e0a     <conditions>.
+000007b0: 2020 2020 2020 3c63 6f6e 6469 7469 6f6e        <condition
+000007c0: 2074 7970 653d 2270 6c6f 6e65 2e63 6f6e   type="plone.con
+000007d0: 6469 7469 6f6e 732e 506f 7274 616c 5479  ditions.PortalTy
+000007e0: 7065 223e 0a20 2020 2020 2020 203c 7072  pe">.        <pr
+000007f0: 6f70 6572 7479 206e 616d 653d 2263 6865  operty name="che
+00000800: 636b 5f74 7970 6573 223e 0a3c 2f70 726f  ck_types">.</pro
+00000810: 7065 7274 793e 0a20 2020 2020 203c 2f63  perty>.      </c
+00000820: 6f6e 6469 7469 6f6e 3e0a 2020 2020 3c2f  ondition>.    </
+00000830: 636f 6e64 6974 696f 6e73 3e0a 2020 2020  conditions>.    
+00000840: 3c61 6374 696f 6e73 3e0a 2020 2020 2020  <actions>.      
+00000850: 3c61 6374 696f 6e20 7479 7065 3d22 706c  <action type="pl
+00000860: 6f6e 652e 6163 7469 6f6e 732e 4175 6469  one.actions.Audi
+00000870: 7422 3e0a 3c2f 6163 7469 6f6e 3e0a 2020  t">.</action>.  
+00000880: 2020 3c2f 6163 7469 6f6e 733e 0a20 203c    </actions>.  <
+00000890: 2f72 756c 653e 0a20 203c 7275 6c65 2064  /rule>.  <rule d
+000008a0: 6573 6372 6970 7469 6f6e 3d22 5468 6973  escription="This
+000008b0: 2073 746f 7265 7320 7468 6520 6163 7469   stores the acti
+000008c0: 6f6e 206f 6620 616e 7920 636f 6e74 656e  on of any conten
+000008d0: 7420 6265 696e 6720 6d6f 7665 6420 6672  t being moved fr
+000008e0: 6f6d 206f 6e65 2063 6f6e 7461 696e 6572  om one container
+000008f0: 2074 6f20 616e 6f74 6865 7220 2843 7574   to another (Cut
+00000900: 2f50 6173 7465 2920 696e 746f 2074 6865  /Paste) into the
+00000910: 2044 6174 6120 5761 7265 686f 7573 6522   Data Warehouse"
+00000920: 0a20 2020 2020 2020 2065 6e61 626c 6564  .        enabled
+00000930: 3d22 4661 6c73 6522 0a20 2020 2020 2020  ="False".       
+00000940: 2065 7665 6e74 3d22 7a6f 7065 2e6c 6966   event="zope.lif
+00000950: 6563 7963 6c65 6576 656e 742e 696e 7465  ecycleevent.inte
+00000960: 7266 6163 6573 2e49 4f62 6a65 6374 4d6f  rfaces.IObjectMo
+00000970: 7665 6445 7665 6e74 220a 2020 2020 2020  vedEvent".      
+00000980: 2020 6e61 6d65 3d22 7275 6c65 2d31 3034    name="rule-104
+00000990: 220a 2020 2020 2020 2020 7374 6f70 2d61  ".        stop-a
+000009a0: 6674 6572 3d22 4661 6c73 6522 0a20 2020  fter="False".   
+000009b0: 2020 2020 2074 6974 6c65 3d22 5374 6f72       title="Stor
+000009c0: 6520 4f62 6a65 6374 204d 6f76 6564 220a  e Object Moved".
+000009d0: 2020 3e0a 2020 2020 3c63 6f6e 6469 7469    >.    <conditi
+000009e0: 6f6e 733e 0a20 2020 2020 203c 636f 6e64  ons>.      <cond
+000009f0: 6974 696f 6e20 7479 7065 3d22 706c 6f6e  ition type="plon
+00000a00: 652e 636f 6e64 6974 696f 6e73 2e50 6f72  e.conditions.Por
+00000a10: 7461 6c54 7970 6522 3e0a 2020 2020 2020  talType">.      
+00000a20: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00000a30: 3d22 6368 6563 6b5f 7479 7065 7322 3e0a  ="check_types">.
+00000a40: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00000a50: 2020 3c2f 636f 6e64 6974 696f 6e3e 0a20    </condition>. 
+00000a60: 2020 203c 2f63 6f6e 6469 7469 6f6e 733e     </conditions>
+00000a70: 0a20 2020 203c 6163 7469 6f6e 733e 0a20  .    <actions>. 
+00000a80: 2020 2020 203c 6163 7469 6f6e 2074 7970       <action typ
+00000a90: 653d 2270 6c6f 6e65 2e61 6374 696f 6e73  e="plone.actions
+00000aa0: 2e41 7564 6974 223e 0a3c 2f61 6374 696f  .Audit">.</actio
+00000ab0: 6e3e 0a20 2020 203c 2f61 6374 696f 6e73  n>.    </actions
+00000ac0: 3e0a 2020 3c2f 7275 6c65 3e0a 2020 3c72  >.  </rule>.  <r
+00000ad0: 756c 6520 6465 7363 7269 7074 696f 6e3d  ule description=
+00000ae0: 2254 6869 7320 7374 6f72 6573 2074 6865  "This stores the
+00000af0: 2061 6374 696f 6e20 6f66 2064 656c 6574   action of delet
+00000b00: 696e 6720 616e 7920 636f 6e74 656e 7420  ing any content 
+00000b10: 6672 6f6d 2061 2063 6f6e 7461 696e 6572  from a container
+00000b20: 2e20 5468 6973 2069 7320 6f6e 6c79 2074  . This is only t
+00000b30: 7269 6767 6572 6564 2077 6865 6e20 4c69  riggered when Li
+00000b40: 6e6b 2049 6e74 6567 7269 7479 2068 6173  nk Integrity has
+00000b50: 2062 6565 6e20 7472 6967 6765 7265 6420   been triggered 
+00000b60: 616e 6420 636f 6e66 6972 6d65 642e 220a  and confirmed.".
+00000b70: 2020 2020 2020 2020 656e 6162 6c65 643d          enabled=
+00000b80: 2246 616c 7365 220a 2020 2020 2020 2020  "False".        
+00000b90: 6576 656e 743d 227a 6f70 652e 6c69 6665  event="zope.life
+00000ba0: 6379 636c 6565 7665 6e74 2e69 6e74 6572  cycleevent.inter
+00000bb0: 6661 6365 732e 494f 626a 6563 7452 656d  faces.IObjectRem
+00000bc0: 6f76 6564 4576 656e 7422 0a20 2020 2020  ovedEvent".     
+00000bd0: 2020 206e 616d 653d 2272 756c 652d 3130     name="rule-10
+00000be0: 3522 0a20 2020 2020 2020 2073 746f 702d  5".        stop-
+00000bf0: 6166 7465 723d 2246 616c 7365 220a 2020  after="False".  
+00000c00: 2020 2020 2020 7469 746c 653d 2253 746f        title="Sto
+00000c10: 7265 204f 626a 6563 7420 4465 6c65 7465  re Object Delete
+00000c20: 6422 0a20 203e 0a20 2020 203c 636f 6e64  d".  >.    <cond
+00000c30: 6974 696f 6e73 3e0a 2020 2020 2020 3c63  itions>.      <c
+00000c40: 6f6e 6469 7469 6f6e 2074 7970 653d 2270  ondition type="p
+00000c50: 6c6f 6e65 2e63 6f6e 6469 7469 6f6e 732e  lone.conditions.
+00000c60: 506f 7274 616c 5479 7065 223e 0a20 2020  PortalType">.   
+00000c70: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000c80: 616d 653d 2263 6865 636b 5f74 7970 6573  ame="check_types
+00000c90: 223e 0a3c 2f70 726f 7065 7274 793e 0a20  ">.</property>. 
+00000ca0: 2020 2020 203c 2f63 6f6e 6469 7469 6f6e       </condition
+00000cb0: 3e0a 2020 2020 3c2f 636f 6e64 6974 696f  >.    </conditio
+00000cc0: 6e73 3e0a 2020 2020 3c61 6374 696f 6e73  ns>.    <actions
+00000cd0: 3e0a 2020 2020 2020 3c61 6374 696f 6e20  >.      <action 
+00000ce0: 7479 7065 3d22 706c 6f6e 652e 6163 7469  type="plone.acti
+00000cf0: 6f6e 732e 4175 6469 7422 3e0a 3c2f 6163  ons.Audit">.</ac
+00000d00: 7469 6f6e 3e0a 2020 2020 3c2f 6163 7469  tion>.    </acti
+00000d10: 6f6e 733e 0a20 203c 2f72 756c 653e 0a20  ons>.  </rule>. 
+00000d20: 203c 7275 6c65 2064 6573 6372 6970 7469   <rule descripti
+00000d30: 6f6e 3d22 5468 6973 2073 746f 7265 7320  on="This stores 
+00000d40: 7468 6520 6163 7469 6f6e 206f 6620 6564  the action of ed
+00000d50: 6974 696e 6720 616e 7920 636f 6e74 656e  iting any conten
+00000d60: 7420 696e 746f 2074 6865 2044 6174 6120  t into the Data 
+00000d70: 5761 7265 686f 7573 6522 0a20 2020 2020  Warehouse".     
+00000d80: 2020 2065 6e61 626c 6564 3d22 4661 6c73     enabled="Fals
+00000d90: 6522 0a20 2020 2020 2020 2065 7665 6e74  e".        event
+00000da0: 3d22 7a6f 7065 2e6c 6966 6563 7963 6c65  ="zope.lifecycle
+00000db0: 6576 656e 742e 696e 7465 7266 6163 6573  event.interfaces
+00000dc0: 2e49 4f62 6a65 6374 4d6f 6469 6669 6564  .IObjectModified
+00000dd0: 4576 656e 7422 0a20 2020 2020 2020 206e  Event".        n
+00000de0: 616d 653d 2272 756c 652d 3130 3622 0a20  ame="rule-106". 
+00000df0: 2020 2020 2020 2073 746f 702d 6166 7465         stop-afte
+00000e00: 723d 2246 616c 7365 220a 2020 2020 2020  r="False".      
+00000e10: 2020 7469 746c 653d 2253 746f 7265 204f    title="Store O
+00000e20: 626a 6563 7420 4564 6974 7322 0a20 203e  bject Edits".  >
+00000e30: 0a20 2020 203c 636f 6e64 6974 696f 6e73  .    <conditions
+00000e40: 3e0a 2020 2020 2020 3c63 6f6e 6469 7469  >.      <conditi
+00000e50: 6f6e 2074 7970 653d 2270 6c6f 6e65 2e63  on type="plone.c
+00000e60: 6f6e 6469 7469 6f6e 732e 506f 7274 616c  onditions.Portal
+00000e70: 5479 7065 223e 0a20 2020 2020 2020 203c  Type">.        <
+00000e80: 7072 6f70 6572 7479 206e 616d 653d 2263  property name="c
+00000e90: 6865 636b 5f74 7970 6573 223e 0a3c 2f70  heck_types">.</p
+00000ea0: 726f 7065 7274 793e 0a20 2020 2020 203c  roperty>.      <
+00000eb0: 2f63 6f6e 6469 7469 6f6e 3e0a 2020 2020  /condition>.    
+00000ec0: 3c2f 636f 6e64 6974 696f 6e73 3e0a 2020  </conditions>.  
+00000ed0: 2020 3c61 6374 696f 6e73 3e0a 2020 2020    <actions>.    
+00000ee0: 2020 3c61 6374 696f 6e20 7479 7065 3d22    <action type="
+00000ef0: 706c 6f6e 652e 6163 7469 6f6e 732e 4175  plone.actions.Au
+00000f00: 6469 7422 3e0a 3c2f 6163 7469 6f6e 3e0a  dit">.</action>.
+00000f10: 2020 2020 3c2f 6163 7469 6f6e 733e 0a20      </actions>. 
+00000f20: 203c 2f72 756c 653e 0a20 203c 7275 6c65   </rule>.  <rule
+00000f30: 2064 6573 6372 6970 7469 6f6e 3d22 5468   description="Th
+00000f40: 6973 2073 746f 7265 7320 7468 6520 6163  is stores the ac
+00000f50: 7469 6f6e 206f 6620 6164 6469 6e67 2061  tion of adding a
+00000f60: 6e79 206e 6577 206f 626a 6563 7473 2074  ny new objects t
+00000f70: 6f20 6120 636f 6e74 6169 6e65 7220 696e  o a container in
+00000f80: 746f 2074 6865 2044 6174 6120 5761 7265  to the Data Ware
+00000f90: 686f 7573 6522 0a20 2020 2020 2020 2065  house".        e
+00000fa0: 6e61 626c 6564 3d22 4661 6c73 6522 0a20  nabled="False". 
+00000fb0: 2020 2020 2020 2065 7665 6e74 3d22 7a6f         event="zo
+00000fc0: 7065 2e6c 6966 6563 7963 6c65 6576 656e  pe.lifecycleeven
+00000fd0: 742e 696e 7465 7266 6163 6573 2e49 4f62  t.interfaces.IOb
+00000fe0: 6a65 6374 4372 6561 7465 6445 7665 6e74  jectCreatedEvent
+00000ff0: 220a 2020 2020 2020 2020 6e61 6d65 3d22  ".        name="
+00001000: 7275 6c65 2d31 3037 220a 2020 2020 2020  rule-107".      
+00001010: 2020 7374 6f70 2d61 6674 6572 3d22 4661    stop-after="Fa
+00001020: 6c73 6522 0a20 2020 2020 2020 2074 6974  lse".        tit
+00001030: 6c65 3d22 5374 6f72 6520 4f62 6a65 6374  le="Store Object
+00001040: 2041 6464 6564 220a 2020 3e0a 2020 2020   Added".  >.    
+00001050: 3c63 6f6e 6469 7469 6f6e 733e 0a20 2020  <conditions>.   
+00001060: 2020 203c 636f 6e64 6974 696f 6e20 7479     <condition ty
+00001070: 7065 3d22 706c 6f6e 652e 636f 6e64 6974  pe="plone.condit
+00001080: 696f 6e73 2e50 6f72 7461 6c54 7970 6522  ions.PortalType"
+00001090: 3e0a 2020 2020 2020 2020 3c70 726f 7065  >.        <prope
+000010a0: 7274 7920 6e61 6d65 3d22 6368 6563 6b5f  rty name="check_
+000010b0: 7479 7065 7322 3e0a 3c2f 7072 6f70 6572  types">.</proper
+000010c0: 7479 3e0a 2020 2020 2020 3c2f 636f 6e64  ty>.      </cond
+000010d0: 6974 696f 6e3e 0a20 2020 203c 2f63 6f6e  ition>.    </con
+000010e0: 6469 7469 6f6e 733e 0a20 2020 203c 6163  ditions>.    <ac
+000010f0: 7469 6f6e 733e 0a20 2020 2020 203c 6163  tions>.      <ac
+00001100: 7469 6f6e 2074 7970 653d 2270 6c6f 6e65  tion type="plone
+00001110: 2e61 6374 696f 6e73 2e41 7564 6974 223e  .actions.Audit">
+00001120: 0a3c 2f61 6374 696f 6e3e 0a20 2020 203c  .</action>.    <
+00001130: 2f61 6374 696f 6e73 3e0a 2020 3c2f 7275  /actions>.  </ru
+00001140: 6c65 3e0a 2020 3c72 756c 6520 6465 7363  le>.  <rule desc
+00001150: 7269 7074 696f 6e3d 2254 6869 7320 7374  ription="This st
+00001160: 6f72 6573 2074 6865 2061 6374 696f 6e20  ores the action 
+00001170: 6f66 2072 656e 616d 696e 6720 616e 7920  of renaming any 
+00001180: 636f 6e74 656e 7420 696e 746f 2074 6865  content into the
+00001190: 2044 6174 6120 5761 7265 686f 7573 652e   Data Warehouse.
+000011a0: 220a 2020 2020 2020 2020 656e 6162 6c65  ".        enable
+000011b0: 643d 2246 616c 7365 220a 2020 2020 2020  d="False".      
+000011c0: 2020 6576 656e 743d 227a 6f70 652e 6c69    event="zope.li
+000011d0: 6665 6379 636c 6565 7665 6e74 2e69 6e74  fecycleevent.int
+000011e0: 6572 6661 6365 732e 494f 626a 6563 744d  erfaces.IObjectM
+000011f0: 6f76 6564 4576 656e 7422 0a20 2020 2020  ovedEvent".     
+00001200: 2020 206e 616d 653d 2272 756c 652d 3130     name="rule-10
+00001210: 3822 0a20 2020 2020 2020 2073 746f 702d  8".        stop-
+00001220: 6166 7465 723d 2246 616c 7365 220a 2020  after="False".  
+00001230: 2020 2020 2020 7469 746c 653d 2253 746f        title="Sto
+00001240: 7265 204f 626a 6563 7420 5265 6e61 6d65  re Object Rename
+00001250: 6422 0a20 203e 0a20 2020 203c 636f 6e64  d".  >.    <cond
+00001260: 6974 696f 6e73 3e0a 2020 2020 2020 3c63  itions>.      <c
+00001270: 6f6e 6469 7469 6f6e 2074 7970 653d 2270  ondition type="p
+00001280: 6c6f 6e65 2e63 6f6e 6469 7469 6f6e 732e  lone.conditions.
+00001290: 506f 7274 616c 5479 7065 223e 0a20 2020  PortalType">.   
+000012a0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+000012b0: 616d 653d 2263 6865 636b 5f74 7970 6573  ame="check_types
+000012c0: 223e 0a3c 2f70 726f 7065 7274 793e 0a20  ">.</property>. 
+000012d0: 2020 2020 203c 2f63 6f6e 6469 7469 6f6e       </condition
+000012e0: 3e0a 2020 2020 3c2f 636f 6e64 6974 696f  >.    </conditio
+000012f0: 6e73 3e0a 2020 2020 3c61 6374 696f 6e73  ns>.    <actions
+00001300: 3e0a 2020 2020 2020 3c61 6374 696f 6e20  >.      <action 
+00001310: 7479 7065 3d22 706c 6f6e 652e 6163 7469  type="plone.acti
+00001320: 6f6e 732e 4175 6469 7422 3e0a 3c2f 6163  ons.Audit">.</ac
+00001330: 7469 6f6e 3e0a 2020 2020 3c2f 6163 7469  tion>.    </acti
+00001340: 6f6e 733e 0a20 203c 2f72 756c 653e 0a20  ons>.  </rule>. 
+00001350: 203c 7275 6c65 2064 6573 6372 6970 7469   <rule descripti
+00001360: 6f6e 3d22 5468 6973 2073 746f 7265 7320  on="This stores 
+00001370: 7468 6520 6163 7469 6f6e 206f 6620 636f  the action of co
+00001380: 7069 6564 2061 6e79 2063 6f6e 7465 6e74  pied any content
+00001390: 2069 6e74 6f20 7468 6520 4461 7461 2057   into the Data W
+000013a0: 6172 6568 6f75 7365 2e22 0a20 2020 2020  arehouse.".     
+000013b0: 2020 2065 6e61 626c 6564 3d22 4661 6c73     enabled="Fals
+000013c0: 6522 0a20 2020 2020 2020 2065 7665 6e74  e".        event
+000013d0: 3d22 4f46 532e 696e 7465 7266 6163 6573  ="OFS.interfaces
+000013e0: 2e49 4f62 6a65 6374 436c 6f6e 6564 4576  .IObjectClonedEv
+000013f0: 656e 7422 0a20 2020 2020 2020 206e 616d  ent".        nam
+00001400: 653d 2272 756c 652d 3130 3922 0a20 2020  e="rule-109".   
+00001410: 2020 2020 2073 746f 702d 6166 7465 723d       stop-after=
+00001420: 2246 616c 7365 220a 2020 2020 2020 2020  "False".        
+00001430: 7469 746c 653d 2253 746f 7265 204f 626a  title="Store Obj
+00001440: 6563 7420 436f 7069 6564 220a 2020 3e0a  ect Copied".  >.
+00001450: 2020 2020 3c63 6f6e 6469 7469 6f6e 733e      <conditions>
+00001460: 0a20 2020 2020 203c 636f 6e64 6974 696f  .      <conditio
+00001470: 6e20 7479 7065 3d22 706c 6f6e 652e 636f  n type="plone.co
+00001480: 6e64 6974 696f 6e73 2e50 6f72 7461 6c54  nditions.PortalT
+00001490: 7970 6522 3e0a 2020 2020 2020 2020 3c70  ype">.        <p
+000014a0: 726f 7065 7274 7920 6e61 6d65 3d22 6368  roperty name="ch
+000014b0: 6563 6b5f 7479 7065 7322 3e0a 3c2f 7072  eck_types">.</pr
+000014c0: 6f70 6572 7479 3e0a 2020 2020 2020 3c2f  operty>.      </
+000014d0: 636f 6e64 6974 696f 6e3e 0a20 2020 203c  condition>.    <
+000014e0: 2f63 6f6e 6469 7469 6f6e 733e 0a20 2020  /conditions>.   
+000014f0: 203c 6163 7469 6f6e 733e 0a20 2020 2020   <actions>.     
+00001500: 203c 6163 7469 6f6e 2074 7970 653d 2270   <action type="p
+00001510: 6c6f 6e65 2e61 6374 696f 6e73 2e41 7564  lone.actions.Aud
+00001520: 6974 223e 0a3c 2f61 6374 696f 6e3e 0a20  it">.</action>. 
+00001530: 2020 203c 2f61 6374 696f 6e73 3e0a 2020     </actions>.  
+00001540: 3c2f 7275 6c65 3e0a 2020 3c72 756c 6520  </rule>.  <rule 
+00001550: 6465 7363 7269 7074 696f 6e3d 2254 6869  description="Thi
+00001560: 7320 7374 6f72 6573 2074 6865 2061 6374  s stores the act
+00001570: 696f 6e20 6f66 2061 6464 696e 6720 616e  ion of adding an
+00001580: 7920 6e65 7720 6f62 6a65 6374 7320 746f  y new objects to
+00001590: 2061 2063 6f6e 7461 696e 6572 2069 6e74   a container int
+000015a0: 6f20 7468 6520 4461 7461 2057 6172 6568  o the Data Wareh
+000015b0: 6f75 7365 220a 2020 2020 2020 2020 656e  ouse".        en
+000015c0: 6162 6c65 643d 2246 616c 7365 220a 2020  abled="False".  
+000015d0: 2020 2020 2020 6576 656e 743d 227a 6f70        event="zop
+000015e0: 652e 6c69 6665 6379 636c 6565 7665 6e74  e.lifecycleevent
+000015f0: 2e69 6e74 6572 6661 6365 732e 494f 626a  .interfaces.IObj
+00001600: 6563 7441 6464 6564 4576 656e 7422 0a20  ectAddedEvent". 
+00001610: 2020 2020 2020 206e 616d 653d 2272 756c         name="rul
+00001620: 652d 3131 3022 0a20 2020 2020 2020 2073  e-110".        s
+00001630: 746f 702d 6166 7465 723d 2246 616c 7365  top-after="False
+00001640: 220a 2020 2020 2020 2020 7469 746c 653d  ".        title=
+00001650: 2253 746f 7265 204f 626a 6563 7420 4164  "Store Object Ad
+00001660: 6465 6422 0a20 203e 0a20 2020 203c 636f  ded".  >.    <co
+00001670: 6e64 6974 696f 6e73 3e0a 2020 2020 2020  nditions>.      
+00001680: 3c63 6f6e 6469 7469 6f6e 2074 7970 653d  <condition type=
+00001690: 2270 6c6f 6e65 2e63 6f6e 6469 7469 6f6e  "plone.condition
+000016a0: 732e 506f 7274 616c 5479 7065 223e 0a20  s.PortalType">. 
+000016b0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000016c0: 206e 616d 653d 2263 6865 636b 5f74 7970   name="check_typ
+000016d0: 6573 223e 0a3c 2f70 726f 7065 7274 793e  es">.</property>
+000016e0: 0a20 2020 2020 203c 2f63 6f6e 6469 7469  .      </conditi
+000016f0: 6f6e 3e0a 2020 2020 3c2f 636f 6e64 6974  on>.    </condit
+00001700: 696f 6e73 3e0a 2020 2020 3c61 6374 696f  ions>.    <actio
+00001710: 6e73 3e0a 2020 2020 2020 3c61 6374 696f  ns>.      <actio
+00001720: 6e20 7479 7065 3d22 706c 6f6e 652e 6163  n type="plone.ac
+00001730: 7469 6f6e 732e 4175 6469 7422 3e0a 3c2f  tions.Audit">.</
+00001740: 6163 7469 6f6e 3e0a 2020 2020 3c2f 6163  action>.    </ac
+00001750: 7469 6f6e 733e 0a20 203c 2f72 756c 653e  tions>.  </rule>
+00001760: 0a0a 2020 3c61 7373 6967 6e6d 656e 7420  ..  <assignment 
+00001770: 6275 6262 6c65 733d 2254 7275 6522 0a20  bubbles="True". 
+00001780: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
+00001790: 626c 6564 3d22 4661 6c73 6522 0a20 2020  bled="False".   
+000017a0: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+000017b0: 696f 6e3d 2222 0a20 2020 2020 2020 2020  ion="".         
+000017c0: 2020 2020 206e 616d 653d 2272 756c 652d       name="rule-
+000017d0: 3130 3022 0a20 202f 3e0a 2020 3c61 7373  100".  />.  <ass
+000017e0: 6967 6e6d 656e 7420 6275 6262 6c65 733d  ignment bubbles=
+000017f0: 2254 7275 6522 0a20 2020 2020 2020 2020  "True".         
+00001800: 2020 2020 2065 6e61 626c 6564 3d22 4661       enabled="Fa
+00001810: 6c73 6522 0a20 2020 2020 2020 2020 2020  lse".           
+00001820: 2020 206c 6f63 6174 696f 6e3d 2222 0a20     location="". 
+00001830: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00001840: 653d 2272 756c 652d 3130 3122 0a20 202f  e="rule-101".  /
+00001850: 3e0a 2020 3c61 7373 6967 6e6d 656e 7420  >.  <assignment 
+00001860: 6275 6262 6c65 733d 2254 7275 6522 0a20  bubbles="True". 
+00001870: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
+00001880: 626c 6564 3d22 4661 6c73 6522 0a20 2020  bled="False".   
+00001890: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+000018a0: 696f 6e3d 2222 0a20 2020 2020 2020 2020  ion="".         
+000018b0: 2020 2020 206e 616d 653d 2272 756c 652d       name="rule-
+000018c0: 3130 3222 0a20 202f 3e0a 2020 3c61 7373  102".  />.  <ass
+000018d0: 6967 6e6d 656e 7420 6275 6262 6c65 733d  ignment bubbles=
+000018e0: 2254 7275 6522 0a20 2020 2020 2020 2020  "True".         
+000018f0: 2020 2020 2065 6e61 626c 6564 3d22 4661       enabled="Fa
+00001900: 6c73 6522 0a20 2020 2020 2020 2020 2020  lse".           
+00001910: 2020 206c 6f63 6174 696f 6e3d 2222 0a20     location="". 
+00001920: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00001930: 653d 2272 756c 652d 3130 3322 0a20 202f  e="rule-103".  /
+00001940: 3e0a 2020 3c61 7373 6967 6e6d 656e 7420  >.  <assignment 
+00001950: 6275 6262 6c65 733d 2254 7275 6522 0a20  bubbles="True". 
+00001960: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
+00001970: 626c 6564 3d22 4661 6c73 6522 0a20 2020  bled="False".   
+00001980: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+00001990: 696f 6e3d 2222 0a20 2020 2020 2020 2020  ion="".         
+000019a0: 2020 2020 206e 616d 653d 2272 756c 652d       name="rule-
+000019b0: 3130 3422 0a20 202f 3e0a 2020 3c61 7373  104".  />.  <ass
+000019c0: 6967 6e6d 656e 7420 6275 6262 6c65 733d  ignment bubbles=
+000019d0: 2254 7275 6522 0a20 2020 2020 2020 2020  "True".         
+000019e0: 2020 2020 2065 6e61 626c 6564 3d22 4661       enabled="Fa
+000019f0: 6c73 6522 0a20 2020 2020 2020 2020 2020  lse".           
+00001a00: 2020 206c 6f63 6174 696f 6e3d 2222 0a20     location="". 
+00001a10: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00001a20: 653d 2272 756c 652d 3130 3522 0a20 202f  e="rule-105".  /
+00001a30: 3e0a 2020 3c61 7373 6967 6e6d 656e 7420  >.  <assignment 
+00001a40: 6275 6262 6c65 733d 2254 7275 6522 0a20  bubbles="True". 
+00001a50: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
+00001a60: 626c 6564 3d22 4661 6c73 6522 0a20 2020  bled="False".   
+00001a70: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+00001a80: 696f 6e3d 2222 0a20 2020 2020 2020 2020  ion="".         
+00001a90: 2020 2020 206e 616d 653d 2272 756c 652d       name="rule-
+00001aa0: 3130 3622 0a20 202f 3e0a 2020 3c61 7373  106".  />.  <ass
+00001ab0: 6967 6e6d 656e 7420 6275 6262 6c65 733d  ignment bubbles=
+00001ac0: 2254 7275 6522 0a20 2020 2020 2020 2020  "True".         
+00001ad0: 2020 2020 2065 6e61 626c 6564 3d22 4661       enabled="Fa
+00001ae0: 6c73 6522 0a20 2020 2020 2020 2020 2020  lse".           
+00001af0: 2020 206c 6f63 6174 696f 6e3d 2222 0a20     location="". 
+00001b00: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00001b10: 653d 2272 756c 652d 3130 3722 0a20 202f  e="rule-107".  /
+00001b20: 3e0a 2020 3c61 7373 6967 6e6d 656e 7420  >.  <assignment 
+00001b30: 6275 6262 6c65 733d 2254 7275 6522 0a20  bubbles="True". 
+00001b40: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
+00001b50: 626c 6564 3d22 4661 6c73 6522 0a20 2020  bled="False".   
+00001b60: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+00001b70: 696f 6e3d 2222 0a20 2020 2020 2020 2020  ion="".         
+00001b80: 2020 2020 206e 616d 653d 2272 756c 652d       name="rule-
+00001b90: 3130 3822 0a20 202f 3e0a 2020 3c61 7373  108".  />.  <ass
+00001ba0: 6967 6e6d 656e 7420 6275 6262 6c65 733d  ignment bubbles=
+00001bb0: 2254 7275 6522 0a20 2020 2020 2020 2020  "True".         
+00001bc0: 2020 2020 2065 6e61 626c 6564 3d22 4661       enabled="Fa
+00001bd0: 6c73 6522 0a20 2020 2020 2020 2020 2020  lse".           
+00001be0: 2020 206c 6f63 6174 696f 6e3d 2222 0a20     location="". 
+00001bf0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00001c00: 653d 2272 756c 652d 3130 3922 0a20 202f  e="rule-109".  /
+00001c10: 3e0a 2020 3c61 7373 6967 6e6d 656e 7420  >.  <assignment 
+00001c20: 6275 6262 6c65 733d 2254 7275 6522 0a20  bubbles="True". 
+00001c30: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
+00001c40: 626c 6564 3d22 4661 6c73 6522 0a20 2020  bled="False".   
+00001c50: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+00001c60: 696f 6e3d 2222 0a20 2020 2020 2020 2020  ion="".         
+00001c70: 2020 2020 206e 616d 653d 2272 756c 652d       name="rule-
+00001c80: 3131 3022 0a20 202f 3e0a 0a3c 2f63 6f6e  110".  />..</con
+00001c90: 7465 6e74 7275 6c65 733e 0a              tentrules>.
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/profiles/default/actions.xml` & `collective.auditlog-3.0.0a1/collective/auditlog/profiles/default/actions.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 223f 3e0a 3c6f 626a 6563 7420 786d  .0"?>.<object xm
-00000020: 6c6e 733a 6931 386e 3d22 6874 7470 3a2f  lns:i18n="http:/
-00000030: 2f78 6d6c 2e7a 6f70 652e 6f72 672f 6e61  /xml.zope.org/na
-00000040: 6d65 7370 6163 6573 2f69 3138 6e22 0a20  mespaces/i18n". 
-00000050: 2020 2020 2020 206d 6574 615f 7479 7065         meta_type
-00000060: 3d22 506c 6f6e 6520 4163 7469 6f6e 7320  ="Plone Actions 
-00000070: 546f 6f6c 220a 2020 2020 2020 2020 6e61  Tool".        na
-00000080: 6d65 3d22 706f 7274 616c 5f61 6374 696f  me="portal_actio
-00000090: 6e73 220a 3e0a 2020 3c6f 626a 6563 7420  ns".>.  <object 
-000000a0: 6d65 7461 5f74 7970 653d 2243 4d46 2041  meta_type="CMF A
-000000b0: 6374 696f 6e20 4361 7465 676f 7279 220a  ction Category".
-000000c0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-000000d0: 7573 6572 220a 2020 3e0a 2020 2020 3c6f  user".  >.    <o
-000000e0: 626a 6563 7420 6d65 7461 5f74 7970 653d  bject meta_type=
-000000f0: 2243 4d46 2041 6374 696f 6e22 0a20 2020  "CMF Action".   
-00000100: 2020 2020 2020 2020 206e 616d 653d 2261           name="a
-00000110: 7564 6974 6c6f 6722 0a20 2020 203e 0a20  uditlog".    >. 
-00000120: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00000130: 616d 653d 2274 6974 6c65 223e 4175 6469  ame="title">Audi
-00000140: 7420 4c6f 673c 2f70 726f 7065 7274 793e  t Log</property>
-00000150: 0a20 2020 2020 203c 7072 6f70 6572 7479  .      <property
-00000160: 206e 616d 653d 2264 6573 6372 6970 7469   name="descripti
-00000170: 6f6e 2220 2f3e 0a20 2020 2020 203c 7072  on" />.      <pr
-00000180: 6f70 6572 7479 206e 616d 653d 2275 726c  operty name="url
-00000190: 5f65 7870 7222 3e73 7472 696e 673a 247b  _expr">string:${
-000001a0: 676c 6f62 616c 735f 7669 6577 2f6e 6176  globals_view/nav
-000001b0: 6967 6174 696f 6e52 6f6f 7455 726c 7d2f  igationRootUrl}/
-000001c0: 4040 6175 6469 746c 6f67 2d76 6965 773f  @@auditlog-view?
-000001d0: 6f72 6465 723d 7065 7266 6f72 6d65 645f  order=performed_
-000001e0: 6f6e 6469 7265 6374 696f 6e3d 6465 7363  ondirection=desc
-000001f0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00000200: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000210: 3d22 6963 6f6e 5f65 7870 7222 202f 3e0a  ="icon_expr" />.
-00000220: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00000230: 6e61 6d65 3d22 6176 6169 6c61 626c 655f  name="available_
-00000240: 6578 7072 223e 7079 7468 6f6e 3a6d 656d  expr">python:mem
-00000250: 6265 7220 6973 206e 6f74 204e 6f6e 653c  ber is not None<
-00000260: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00000270: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00000280: 2270 6572 6d69 7373 696f 6e73 223e 0a20  "permissions">. 
-00000290: 2020 2020 2020 203c 656c 656d 656e 7420         <element 
-000002a0: 7661 6c75 653d 2263 6f6c 6c65 6374 6976  value="collectiv
-000002b0: 652e 6175 6469 746c 6f67 3a20 5669 6577  e.auditlog: View
-000002c0: 2041 7564 6974 6c6f 6722 202f 3e0a 2020   Auditlog" />.  
-000002d0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
-000002e0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-000002f0: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
-00000300: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00000310: 2020 203c 2f6f 626a 6563 743e 0a20 203c     </object>.  <
-00000320: 2f6f 626a 6563 743e 0a3c 2f6f 626a 6563  /object>.</objec
-00000330: 743e 0a                                  t>.
+00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
+00000020: 662d 3822 3f3e 0a3c 6f62 6a65 6374 2078  f-8"?>.<object x
+00000030: 6d6c 6e73 3a69 3138 6e3d 2268 7474 703a  mlns:i18n="http:
+00000040: 2f2f 786d 6c2e 7a6f 7065 2e6f 7267 2f6e  //xml.zope.org/n
+00000050: 616d 6573 7061 6365 732f 6931 386e 220a  amespaces/i18n".
+00000060: 2020 2020 2020 2020 6d65 7461 5f74 7970          meta_typ
+00000070: 653d 2250 6c6f 6e65 2041 6374 696f 6e73  e="Plone Actions
+00000080: 2054 6f6f 6c22 0a20 2020 2020 2020 206e   Tool".        n
+00000090: 616d 653d 2270 6f72 7461 6c5f 6163 7469  ame="portal_acti
+000000a0: 6f6e 7322 0a3e 0a20 203c 6f62 6a65 6374  ons".>.  <object
+000000b0: 206d 6574 615f 7479 7065 3d22 434d 4620   meta_type="CMF 
+000000c0: 4163 7469 6f6e 2043 6174 6567 6f72 7922  Action Category"
+000000d0: 0a20 2020 2020 2020 2020 206e 616d 653d  .          name=
+000000e0: 2275 7365 7222 0a20 203e 0a20 2020 203c  "user".  >.    <
+000000f0: 6f62 6a65 6374 206d 6574 615f 7479 7065  object meta_type
+00000100: 3d22 434d 4620 4163 7469 6f6e 220a 2020  ="CMF Action".  
+00000110: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+00000120: 6175 6469 746c 6f67 220a 2020 2020 3e0a  auditlog".    >.
+00000130: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000140: 6e61 6d65 3d22 7469 746c 6522 3e41 7564  name="title">Aud
+00000150: 6974 204c 6f67 3c2f 7072 6f70 6572 7479  it Log</property
+00000160: 3e0a 2020 2020 2020 3c70 726f 7065 7274  >.      <propert
+00000170: 7920 6e61 6d65 3d22 6465 7363 7269 7074  y name="descript
+00000180: 696f 6e22 202f 3e0a 2020 2020 2020 3c70  ion" />.      <p
+00000190: 726f 7065 7274 7920 6e61 6d65 3d22 7572  roperty name="ur
+000001a0: 6c5f 6578 7072 223e 7374 7269 6e67 3a24  l_expr">string:$
+000001b0: 7b67 6c6f 6261 6c73 5f76 6965 772f 6e61  {globals_view/na
+000001c0: 7669 6761 7469 6f6e 526f 6f74 5572 6c7d  vigationRootUrl}
+000001d0: 2f40 4061 7564 6974 6c6f 672d 7669 6577  /@@auditlog-view
+000001e0: 3f6f 7264 6572 3d70 6572 666f 726d 6564  ?order=performed
+000001f0: 5f6f 6e64 6972 6563 7469 6f6e 3d64 6573  _ondirection=des
+00000200: 633c 2f70 726f 7065 7274 793e 0a20 2020  c</property>.   
+00000210: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000220: 653d 2269 636f 6e5f 6578 7072 2220 2f3e  e="icon_expr" />
+00000230: 0a20 2020 2020 203c 7072 6f70 6572 7479  .      <property
+00000240: 206e 616d 653d 2261 7661 696c 6162 6c65   name="available
+00000250: 5f65 7870 7222 3e70 7974 686f 6e3a 6d65  _expr">python:me
+00000260: 6d62 6572 2069 7320 6e6f 7420 4e6f 6e65  mber is not None
+00000270: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00000280: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00000290: 3d22 7065 726d 6973 7369 6f6e 7322 3e0a  ="permissions">.
+000002a0: 2020 2020 2020 2020 3c65 6c65 6d65 6e74          <element
+000002b0: 2076 616c 7565 3d22 636f 6c6c 6563 7469   value="collecti
+000002c0: 7665 2e61 7564 6974 6c6f 673a 2056 6965  ve.auditlog: Vie
+000002d0: 7720 4175 6469 746c 6f67 2220 2f3e 0a20  w Auditlog" />. 
+000002e0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+000002f0: 0a20 2020 2020 203c 7072 6f70 6572 7479  .      <property
+00000300: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
+00000310: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+00000320: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
+00000330: 3c2f 6f62 6a65 6374 3e0a 3c2f 6f62 6a65  </object>.</obje
+00000340: 6374 3e0a                                ct>.
```

### Comparing `collective.auditlog-2.0.0a2/collective/auditlog/action.py` & `collective.auditlog-3.0.0a1/collective/auditlog/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 from collective.auditlog.utils import addLogEntry
 from collective.auditlog.utils import getObjectInfo
 from OFS.interfaces import IObjectClonedEvent
 from OFS.SimpleItem import SimpleItem
 from plone.app.contentrules.browser.formhelper import AddForm
 from plone.app.contentrules.browser.formhelper import EditForm
 from plone.app.iterate.interfaces import IBeforeCheckoutEvent
@@ -46,36 +45,34 @@
 class IAuditAction(Interface):
     pass
 
 
 @implementer(IAuditAction, IRuleElementData)
 class AuditAction(SimpleItem):
     element = "plone.actions.Audit"
-    summary = u"Audit"
+    summary = "Audit"
 
 
 @implementer(IExecutable)
 @adapter(Interface, IAuditAction, Interface)
-class AuditActionExecutor(object):
+class AuditActionExecutor:
     def __init__(self, context, element, event):
         self.context = context
         self.element = element
         self.event = event
 
     @property
     def request(self):
-        """Try to get a request
-        """
+        """Try to get a request"""
         return getRequest()
 
     @property
     @memoize
     def rule(self):
-        """ Check up the stack the rule that invoked this action
-        """
+        """Check up the stack the rule that invoked this action"""
         # start higher in the stack
         frame = inspect.currentframe().f_back.f_back
         while frame:
             rule = frame.f_locals.get("self", None)
             if isinstance(rule, RuleExecutable):
                 return rule
             frame = frame.f_back
@@ -93,15 +90,15 @@
         rule = self.rule
         if rule and event_iface != rule.rule.event:
             return False
 
         return True
 
     def get_history_comment(self):
-        """ Given an object and a IActionSucceededEvent,
+        """Given an object and a IActionSucceededEvent,
         extract the comment of the transition.
         """
         action = self.event.action
         if not action:
             return ""
         history = self.event.object.workflow_history
         for transition in reversed(history[self.event.workflow.id]):
@@ -118,16 +115,15 @@
         ]  # noqa
 
     def _getObjectInfo(self, obj):
         return getObjectInfo(obj)
 
     @memoize
     def getLogEntry(self):
-        """ Get's a log entry for your action
-        """
+        """Gets a log entry for your action"""
         event = self.event
         obj = event.object
         data = {"info": ""}
         environ = getattr(self.request, "environ", {})
 
         # the order of those interface checks matters since some interfaces
         # inherit from others
@@ -148,15 +144,15 @@
                     action = "rename"
                 else:
                     # cut out here, double action for this event
                     return True
             else:
                 if self.rule is None or "Moved" in self.rule.rule.title:
                     parent_path = "/".join(event.oldParent.getPhysicalPath())
-                    previous_location = u"{0}/{1}".format(parent_path, event.oldName)
+                    previous_location = f"{parent_path}/{event.oldName}"
                     info = {"previous_location": previous_location}
                     data["info"] = json.dumps(info)
                     action = "moved"
                 else:
                     # step out immediately since this could be a double action
                     return True
         elif IObjectModifiedEvent.providedBy(event):
@@ -222,22 +218,20 @@
     def __call__(self):
         if self.can_execute:
             self._addLogEntry(self.getLogEntry())
         return True
 
 
 class AuditAddForm(AddForm):
-
     schema = IAuditAction
-    label = u"Add Audit Action"
-    form_name = u"Configure element"
+    label = "Add Audit Action"
+    form_name = "Configure element"
 
     def create(self, data):
         a = AuditAction()
         return a
 
 
 class AuditEditForm(EditForm):
-
     schema = IAuditAction
-    label = u"Edit Audit Action"
-    form_name = u"Configure element"
+    label = "Edit Audit Action"
+    form_name = "Configure element"
```

### Comparing `collective.auditlog-2.0.0a2/docs/LICENSE.txt` & `collective.auditlog-3.0.0a1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a2/docs/INSTALL.txt` & `collective.auditlog-3.0.0a1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a2/docs/LICENSE.GPL` & `collective.auditlog-3.0.0a1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.auditlog-2.0.0a2/README.rst` & `collective.auditlog-3.0.0a1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 "bin/pcelery worker" from the buildout directory. Note that the script is
 now named 'pcelery' and it needs a path to the zope configuration. Example::
 
     $ bin/pcelery worker parts/client1/etc/zope.conf
 
 Flower is included in this setup. Run "bin/flower" from the buildout
 directory and consult the dashboard at http://localhost:5555 using a
-browser. Note that the broker is now a requried parameter::
+browser. Note that the broker is now a required parameter::
 
     $ bin/flower --broker redis://127.0.0.1:6379
 
 Dependencies
 ============
 
 All dependencies are installed automatically
```

