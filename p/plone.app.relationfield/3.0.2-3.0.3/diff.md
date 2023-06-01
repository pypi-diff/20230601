# Comparing `tmp/plone.app.relationfield-3.0.2.tar.gz` & `tmp/plone.app.relationfield-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.relationfield-3.0.2.tar", last modified: Sat Apr 15 08:03:23 2023, max compression
+gzip compressed data, was "plone.app.relationfield-3.0.3.tar", last modified: Thu Jun  1 08:06:35 2023, max compression
```

## Comparing `plone.app.relationfield-3.0.2.tar` & `plone.app.relationfield-3.0.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/
--rw-r--r--   0 gil       (1000) gil       (1000)     5376 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      150 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)     6978 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      714 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.651490 plone.app.relationfield-3.0.2/docs/
--rw-r--r--   0 gil       (1000) gil       (1000)      703 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/docs/INSTALL.txt
--rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/docs/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      752 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.651490 plone.app.relationfield-3.0.2/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.652490 plone.app.relationfield-3.0.2/plone/app/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/plone/app/relationfield/
--rw-r--r--   0 gil       (1000) gil       (1000)      257 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      524 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/adapter.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1165 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/behavior.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2768 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      731 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/demo.py
--rw-r--r--   0 gil       (1000) gil       (1000)      457 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/demo.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     1378 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/event.py
--rw-r--r--   0 gil       (1000) gil       (1000)      114 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)      779 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2376 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      393 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      743 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/monkey.py
--rw-r--r--   0 gil       (1000) gil       (1000)      806 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/path.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.650490 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/default/
--rw-r--r--   0 gil       (1000) gil       (1000)       23 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/default/install_relations.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      181 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/default/metadata.xml
--rw-r--r--   0 gil       (1000) gil       (1000)     2786 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6006 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1205 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     5812 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor_contenttree.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1092 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/setuphandlers.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1362 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/source.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1921 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5860 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      406 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     5985 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel_contenttree.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     3670 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/testing.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      659 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_marshall.py
--rw-r--r--   0 gil       (1000) gil       (1000)      321 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_marshall.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      647 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_schemaeditor.py
--rw-r--r--   0 gil       (1000) gil       (1000)      651 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_supermodel.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2254 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_widget.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5571 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/widget.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1141 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/widget.zcml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.652490 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)     6978 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     1899 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      512 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1694 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 08:03:23.656490 plone.app.relationfield-3.0.2/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     2292 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.246438 plone.app.relationfield-3.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     5610 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      150 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     7212 2023-06-01 08:06:35.246155 plone.app.relationfield-3.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      714 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.232990 plone.app.relationfield-3.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      703 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      752 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.233295 plone.app.relationfield-3.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.235716 plone.app.relationfield-3.0.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.243547 plone.app.relationfield-3.0.3/plone/app/relationfield/
+-rw-r--r--   0 maurits    (501) staff       (20)      257 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      524 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1179 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2768 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      731 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/demo.py
+-rw-r--r--   0 maurits    (501) staff       (20)      457 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/demo.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1378 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/event.py
+-rw-r--r--   0 maurits    (501) staff       (20)      114 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      779 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/marshaler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2376 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/marshaler.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/marshaler.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      743 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/monkey.py
+-rw-r--r--   0 maurits    (501) staff       (20)      806 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/path.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.229911 plone.app.relationfield-3.0.3/plone/app/relationfield/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.244125 plone.app.relationfield-3.0.3/plone/app/relationfield/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)       23 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/profiles/default/install_relations.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      181 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2767 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6006 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1205 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5812 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor_contenttree.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1092 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1362 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/source.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1921 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/supermodel.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      406 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/supermodel.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5985 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/supermodel_contenttree.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3670 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.245788 plone.app.relationfield-3.0.3/plone/app/relationfield/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      659 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_marshall.py
+-rw-r--r--   0 maurits    (501) staff       (20)      321 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_marshall.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      647 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)      651 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2254 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5571 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1141 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/plone/app/relationfield/widget.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-01 08:06:35.235418 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     7212 2023-06-01 08:06:35.000000 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-06-01 08:06:35.000000 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-01 08:06:35.000000 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-06-01 08:06:35.000000 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-01 08:06:35.000000 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      403 2023-06-01 08:06:35.000000 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-01 08:06:35.000000 plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3900 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-06-01 08:06:35.246522 plone.app.relationfield-3.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-06-01 08:06:34.000000 plone.app.relationfield-3.0.3/setup.py
```

### Comparing `plone.app.relationfield-3.0.2/CHANGES.rst` & `plone.app.relationfield-3.0.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-06-01)
+------------------
+
+Bug fixes:
+
+
+- Removed unneeded dependency on plone.app.dexterity.
+  It remains a test dependency though.
+  [maurits] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c)
+
+
 3.0.2 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.relationfield-3.0.2/PKG-INFO` & `plone.app.relationfield-3.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.relationfield
-Version: 3.0.2
+Version: 3.0.3
 Summary: Plone support for z3c.relationfield
 Home-page: https://pypi.org/project/plone.app.relationfield
 Author: Alec Mitchell
 Author-email: apm13@columbia.edu
 License: GPL
 Keywords: dexterity relations plone zc.relation
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-06-01)
+------------------
+
+Bug fixes:
+
+
+- Removed unneeded dependency on plone.app.dexterity.
+  It remains a test dependency though.
+  [maurits] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c)
+
+
 3.0.2 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.relationfield-3.0.2/README.rst` & `plone.app.relationfield-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/docs/INSTALL.txt` & `plone.app.relationfield-3.0.3/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/docs/LICENSE.GPL` & `plone.app.relationfield-3.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/docs/LICENSE.txt` & `plone.app.relationfield-3.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/adapter.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/adapter.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/behavior.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/behavior.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from plone.app.dexterity import _
 from plone.app.z3cform.widget import RelatedItemsFieldWidget
 from plone.autoform import directives as form
 from plone.autoform.interfaces import IFormFieldProvider
+from plone.base import PloneMessageFactory as _
 from plone.supermodel import model
 from plone.supermodel.directives import fieldset
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope.interface import provider
```

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/configure.zcml` & `plone.app.relationfield-3.0.3/plone/app/relationfield/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/demo.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/demo.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/event.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/event.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/marshaler.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.rst` & `plone.app.relationfield-3.0.3/plone/app/relationfield/marshaler.rst`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/monkey.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/monkey.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/path.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/path.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from plone.app.vocabularies.catalog import CatalogSource
+from plone.base import PloneMessageFactory as _
 from plone.schemaeditor.fields import FieldFactory
 from plone.schemaeditor.interfaces import IFieldEditFormSchema
 from plone.schemaeditor.interfaces import IFieldFactory
 from z3c.relationfield import interfaces
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope import schema
 from zope.component import adapter
 from zope.component import queryUtility
-from zope.i18n import MessageFactory
 from zope.interface import implementer
 from zope.intid.interfaces import IIntIds
 
 
-_ = MessageFactory("plone")
-
-
 @implementer(IFieldFactory)
 class RelationFieldFactory(FieldFactory):
     def available(self):
         return queryUtility(IIntIds) is not None
 
 
 class IRelationFieldSettings(schema.interfaces.IField):
```

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.txt` & `plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.zcml` & `plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor_contenttree.txt` & `plone.app.relationfield-3.0.3/plone/app/relationfield/schemaeditor_contenttree.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/setuphandlers.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/source.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/source.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.txt` & `plone.app.relationfield-3.0.3/plone/app/relationfield/supermodel.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel_contenttree.txt` & `plone.app.relationfield-3.0.3/plone/app/relationfield/supermodel_contenttree.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/testing.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_marshall.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_marshall.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_schemaeditor.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_supermodel.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_widget.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/widget.py` & `plone.app.relationfield-3.0.3/plone/app/relationfield/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone/app/relationfield/widget.zcml` & `plone.app.relationfield-3.0.3/plone/app/relationfield/widget.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/PKG-INFO` & `plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.relationfield
-Version: 3.0.2
+Version: 3.0.3
 Summary: Plone support for z3c.relationfield
 Home-page: https://pypi.org/project/plone.app.relationfield
 Author: Alec Mitchell
 Author-email: apm13@columbia.edu
 License: GPL
 Keywords: dexterity relations plone zc.relation
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-06-01)
+------------------
+
+Bug fixes:
+
+
+- Removed unneeded dependency on plone.app.dexterity.
+  It remains a test dependency though.
+  [maurits] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c)
+
+
 3.0.2 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/SOURCES.txt` & `plone.app.relationfield-3.0.3/plone.app.relationfield.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.app.relationfield.egg-info/PKG-INFO
 plone.app.relationfield.egg-info/SOURCES.txt
```

### Comparing `plone.app.relationfield-3.0.2/setup.py` & `plone.app.relationfield-3.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.2"
+version = "3.0.3"
 
 setup(
     name="plone.app.relationfield",
     version=version,
     description="Plone support for z3c.relationfield",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     # Get more strings from
@@ -32,46 +32,38 @@
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "setuptools",
-        "zope.interface",
-        "zope.component",
-        "zope.schema",
-        "zope.intid",
+        "plone.base",
+        # Keep Products.CMFCore because z3c.dependencychecker does not yet
+        # check transitive dependencies in our config.
+        "Products.CMFCore",
         "five.intid",
         "plone.app.intid",
-        "z3c.form",
-        "z3c.relationfield>0.7.999",
-        "z3c.formwidget.query",
-        "plone.autoform",
-        "plone.supermodel",
         "plone.app.vocabularies",
-        "plone.schemaeditor>=1.3.5",
-        "Products.CMFCore",
-        "plone.rfc822",
-        "plone.app.z3cform>=1.1.0",
-        "BTrees",
-        "Products.GenericSetup",
-        "plone.app.dexterity",
+        "plone.app.z3cform",
+        "plone.autoform",
         "plone.behavior",
         "plone.dexterity",
+        "plone.rfc822",
+        "plone.schemaeditor",
+        "plone.supermodel",
         "plone.uuid",
-        "plone.z3cform",
+        "z3c.form",
         "z3c.objpath",
+        "z3c.formwidget.query",
+        "z3c.relationfield",
         "zc.relation",
     ],
     extras_require={
         "test": [
-            "persistent",
             "plone.app.contenttypes[test]",
             "plone.app.testing",
             "plone.app.dexterity",
+            "plone.formwidget.contenttree",
             "plone.testing",
         ]
     },
-    entry_points="""
-    # -*- Entry points: -*-
-    """,
 )
```

