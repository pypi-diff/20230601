# Comparing `tmp/collective.casestudy-1.0.0a2.tar.gz` & `tmp/collective.casestudy-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.casestudy-1.0.0a2.tar", last modified: Mon May 15 08:44:57 2023, max compression
+gzip compressed data, was "collective.casestudy-1.0.0a3.tar", last modified: Thu Jun  1 19:40:40 2023, max compression
```

## Comparing `collective.casestudy-1.0.0a2.tar` & `collective.casestudy-1.0.0a3.tar`

### file list

```diff
@@ -1,74 +1,121 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.334089 collective.casestudy-1.0.0a2/
--rw-r--r--   0 ericof     (501) staff       (20)      174 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/CHANGELOG.md
--rw-r--r--   0 ericof     (501) staff       (20)       49 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/CONTRIBUTORS.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/LICENSE.md
--rw-r--r--   0 ericof     (501) staff       (20)       66 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     4643 2023-05-15 08:44:57.333955 collective.casestudy-1.0.0a2/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     3279 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/README.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.327446 collective.casestudy-1.0.0a2/docs/
--rw-r--r--   0 ericof     (501) staff       (20)     8072 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/docs/icon.svg
--rw-r--r--   0 ericof     (501) staff       (20)      800 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-15 08:44:57.334130 collective.casestudy-1.0.0a2/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2207 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.325105 collective.casestudy-1.0.0a2/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.327590 collective.casestudy-1.0.0a2/src/collective/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.329677 collective.casestudy-1.0.0a2/src/collective/casestudy/
--rw-r--r--   0 ericof     (501) staff       (20)      201 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.330149 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      667 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1009 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/browser/controlpanel.py
--rw-r--r--   0 ericof     (501) staff       (20)      670 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.330446 collective.casestudy-1.0.0a2/src/collective/casestudy/content/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/content/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1096 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/content/case_study.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.330846 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      245 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/case_study.py
--rw-r--r--   0 ericof     (501) staff       (20)      271 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/indexers/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1013 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/interfaces.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.331118 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/
--rw-r--r--   0 ericof     (501) staff       (20)     3133 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/collective.casestudy.pot
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.325623 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/es/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.331272 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/es/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     3793 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/es/LC_MESSAGES/collective.casestudy.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.325752 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/pt_BR/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.331419 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     3438 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/collective.casestudy.po
--rw-r--r--   0 ericof     (501) staff       (20)     1946 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/locales/update.py
--rw-r--r--   0 ericof     (501) staff       (20)      287 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/permissions.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.326122 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332185 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/
--rw-r--r--   0 ericof     (501) staff       (20)      169 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/browserlayer.xml
--rw-r--r--   0 ericof     (501) staff       (20)      503 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/catalog.xml
--rw-r--r--   0 ericof     (501) staff       (20)      458 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/controlpanel.xml
--rw-r--r--   0 ericof     (501) staff       (20)      107 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/metadata.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332457 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/
--rw-r--r--   0 ericof     (501) staff       (20)     1080 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/main.xml
--rw-r--r--   0 ericof     (501) staff       (20)     2359 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/registry/querystring.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332619 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types/
--rw-r--r--   0 ericof     (501) staff       (20)     2866 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types/CaseStudy.xml
--rw-r--r--   0 ericof     (501) staff       (20)      184 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.332779 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/uninstall/
--rw-r--r--   0 ericof     (501) staff       (20)      123 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 ericof     (501) staff       (20)      742 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/profiles.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      671 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.333048 collective.casestudy-1.0.0a2/src/collective/casestudy/upgrades/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/upgrades/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      140 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/upgrades/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.333738 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      435 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      519 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/industries.py
--rw-r--r--   0 ericof     (501) staff       (20)      505 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/usages.py
--rw-r--r--   0 ericof     (501) staff       (20)      548 2023-05-15 08:44:56.000000 collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/versions.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-15 08:44:57.328738 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     4643 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     2251 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)      125 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)      147 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/top_level.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-15 08:44:57.000000 collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/zip-safe
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.414175 collective.casestudy-1.0.0a3/
+-rw-r--r--   0 ericof     (501) staff       (20)       21 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/.coveragerc
+-rw-r--r--   0 ericof     (501) staff       (20)      972 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      381 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/CHANGELOG.md
+-rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/CONTRIBUTORS.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/LICENSE.md
+-rw-r--r--   0 ericof     (501) staff       (20)      151 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     3001 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)     4963 2023-06-01 19:40:40.414033 collective.casestudy-1.0.0a3/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     3392 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/README.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.403300 collective.casestudy-1.0.0a3/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     8072 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/docs/icon.svg
+-rw-r--r--   0 ericof     (501) staff       (20)      800 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-01 19:40:40.414212 collective.casestudy-1.0.0a3/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2189 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.399792 collective.casestudy-1.0.0a3/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.403423 collective.casestudy-1.0.0a3/src/collective/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.405169 collective.casestudy-1.0.0a3/src/collective/casestudy/
+-rw-r--r--   0 ericof     (501) staff       (20)      201 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.405775 collective.casestudy-1.0.0a3/src/collective/casestudy/behaviors/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/behaviors/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1421 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/behaviors/address_info.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1162 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/behaviors/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1281 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/behaviors/contact_info.py
+-rw-r--r--   0 ericof     (501) staff       (20)      926 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/behaviors/providers.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.406126 collective.casestudy-1.0.0a3/src/collective/casestudy/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      667 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1009 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/browser/controlpanel.py
+-rw-r--r--   0 ericof     (501) staff       (20)      705 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.406494 collective.casestudy-1.0.0a3/src/collective/casestudy/content/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/content/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1096 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/content/case_study.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1570 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/content/provider.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.406977 collective.casestudy-1.0.0a3/src/collective/casestudy/indexers/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/indexers/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      245 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/indexers/case_study.py
+-rw-r--r--   0 ericof     (501) staff       (20)      360 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/indexers/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      320 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/indexers/providers.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1521 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/interfaces.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.407236 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/
+-rw-r--r--   0 ericof     (501) staff       (20)     8479 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/collective.casestudy.pot
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.400422 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/es/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.407366 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/es/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)     9055 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/es/LC_MESSAGES/collective.casestudy.po
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.400573 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/pt_BR/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.407504 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)     9879 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/pt_BR/LC_MESSAGES/collective.casestudy.po
+-rw-r--r--   0 ericof     (501) staff       (20)     1946 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/locales/update.py
+-rw-r--r--   0 ericof     (501) staff       (20)      795 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/permissions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.401096 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.408759 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/
+-rw-r--r--   0 ericof     (501) staff       (20)      169 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/browserlayer.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      899 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/catalog.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/controlpanel.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      362 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/diff_tool.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      107 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/metadata.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.409069 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/registry/
+-rw-r--r--   0 ericof     (501) staff       (20)     1543 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/registry/main.xml
+-rw-r--r--   0 ericof     (501) staff       (20)     4589 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/registry/querystring.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      354 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/repositorytool.xml
+-rw-r--r--   0 ericof     (501) staff       (20)     1101 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/rolemap.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.409376 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/types/
+-rw-r--r--   0 ericof     (501) staff       (20)     2921 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/types/CaseStudy.xml
+-rw-r--r--   0 ericof     (501) staff       (20)     2899 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/types/Provider.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      251 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/types.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.401015 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/workflows/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.409537 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/workflows/provider_workflow/
+-rw-r--r--   0 ericof     (501) staff       (20)    12163 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/workflows/provider_workflow/definition.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      401 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/workflows.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.409706 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/uninstall/
+-rw-r--r--   0 ericof     (501) staff       (20)      123 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      742 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/profiles.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      906 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.410132 collective.casestudy-1.0.0a3/src/collective/casestudy/upgrades/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/upgrades/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1562 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/upgrades/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1788 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/upgrades/vocabulary.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.411412 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1088 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      991 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/countries.py
+-rw-r--r--   0 ericof     (501) staff       (20)      588 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/industries.py
+-rw-r--r--   0 ericof     (501) staff       (20)      627 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/organization.py
+-rw-r--r--   0 ericof     (501) staff       (20)      509 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/providers.py
+-rw-r--r--   0 ericof     (501) staff       (20)      587 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/services.py
+-rw-r--r--   0 ericof     (501) staff       (20)      596 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/usages.py
+-rw-r--r--   0 ericof     (501) staff       (20)      548 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/versions.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.404431 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     4963 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     3838 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      125 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      157 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/top_level.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-01 19:40:40.000000 collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/zip-safe
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.411679 collective.casestudy-1.0.0a3/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.411825 collective.casestudy-1.0.0a3/tests/behaviors/
+-rw-r--r--   0 ericof     (501) staff       (20)     1995 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/behaviors/test_providers.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3396 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.412122 collective.casestudy-1.0.0a3/tests/content/
+-rw-r--r--   0 ericof     (501) staff       (20)     1879 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/content/test_case_study.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1457 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/content/test_provider.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.412419 collective.casestudy-1.0.0a3/tests/restapi/
+-rw-r--r--   0 ericof     (501) staff       (20)     2767 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/restapi/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3542 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/restapi/test_restapi_provider.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.412747 collective.casestudy-1.0.0a3/tests/setup/
+-rw-r--r--   0 ericof     (501) staff       (20)      595 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/setup/test_setup_install.py
+-rw-r--r--   0 ericof     (501) staff       (20)      631 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/setup/test_setup_uninstall.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-01 19:40:40.413809 collective.casestudy-1.0.0a3/tests/vocabularies/
+-rw-r--r--   0 ericof     (501) staff       (20)     2433 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/vocabularies/test_vocab_countries.py
+-rw-r--r--   0 ericof     (501) staff       (20)      724 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/vocabularies/test_vocab_industries.py
+-rw-r--r--   0 ericof     (501) staff       (20)      716 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/vocabularies/test_vocab_organization.py
+-rw-r--r--   0 ericof     (501) staff       (20)      892 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/vocabularies/test_vocab_providers.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1077 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/vocabularies/test_vocab_services.py
+-rw-r--r--   0 ericof     (501) staff       (20)      698 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/vocabularies/test_vocab_usages.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1120 2023-06-01 19:40:39.000000 collective.casestudy-1.0.0a3/tests/vocabularies/test_vocab_versions.py
```

### Comparing `collective.casestudy-1.0.0a2/LICENSE.md` & `collective.casestudy-1.0.0a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/PKG-INFO` & `collective.casestudy-1.0.0a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.casestudy
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Case Study content type for Plone.
 Home-page: https://github.com/collective/collective.casestudy
 Author: Plone Community
 Author-email: ericof@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.casestudy
 Project-URL: Source, https://github.com/collective/collective.casestudy
@@ -48,27 +48,39 @@
 ![Code Style](https://img.shields.io/badge/Code%20Style-Black-000000)
 
 [![GitHub contributors](https://img.shields.io/github/contributors/collective/collective.casestudy)](https://github.com/collective/collective.casestudy)
 [![GitHub Repo stars](https://img.shields.io/github/stars/collective/collective.casestudy?style=social)](https://github.com/collective/collective.casestudy)
 
 </div>
 
-Features
---------
+## Features
 
-**collective.casestudy** provides a Case Study content type to be used in Plone sites.
+`collective.casestudy` provides two new content types to be used in Plone sites, Case Study and Provider.
 
-Documentation
--------------
+### Case Study
 
-This package supports Plone sites using Volto, but each project should provide their own view for this content type.
+A case study of a Plone deployment, which has attributes to track the Plone version used, the industry, and the type of usage of Plone.
 
+### Provider
 
-Installation
-------------
+A company providing Plone services and solutions.
+
+## See it in action
+
+**collective.casestudy** is being used in the following sites:
+
+* [Plone.org](https://plone.org)
+* [Plone Brasil](https://plone.org.br)
+
+## Documentation
+
+This package supports Plone sites using Volto, but each project should provide its view for this content type.
+
+
+### Installation
 
 Add **collective.casestudy** to the Plone installation using `pip`:
 
 ```bash
 pip install collective.casestudy
 ```
 or add it as a dependency on your package's `setup.py`
@@ -81,53 +93,55 @@
         "setuptools",
     ],
 ```
 
 Start Plone and activate the plugin in the addons control-panel.
 
 
-Source Code and Contributions
------------------------------
+## Source Code and Contributions
 
-If you want to help with the development (improvement, update, bug-fixing, ...) of `collective.casestudy` this is a great idea!
+We welcome contributions to `collective.casestudy`.
+You can create an issue in the issue tracker, or contact a maintainer.
 
 - [Issue Tracker](https://github.com/collective/collective.casestudy/issues)
 - [Source Code](https://github.com/collective/collective.casestudy/)
 
 
-We appreciate any contribution and if a release is needed to be done on PyPI, please just contact one of us.
 
-Development
------------
+### Development
 
-You need a working `python` environment (system, virtualenv, pyenv, etc) version 3.7 or superior.
+You need a working Python environment version 3.7 or later.
 
 Then install the dependencies and a development instance using:
 
 ```bash
 make build
 ```
 
-To run tests for this package:
+By default, we use the latest Plone version in the 6.x series.
 
-```bash
-make test
-```
+## License
+
+The project is licensed under GPLv2.
 
-By default we use the latest Plone version in the 6.x series.
 
-License
--------
+# Changelog
 
-The project is licensed under the GPLv2.
+## 1.0.0a3 (2023-06-01)
 
+- Add Provider content type #2 [ericof]
+
+- Add Providers behavior [ericof]
+
+- Add catalog indexes for providers, country, services [ericof]
+
+- Update pt_BR translation [ericof]
 
-# Changelog
 
-1.0.0a2 (2023-05-15)
+## 1.0.0a2 (2023-05-15)
 
 - Added Spanish translation [macagua]
 
 - Use `pytest-plone` for testing.
   [ericof]
```

### Comparing `collective.casestudy-1.0.0a2/README.md` & `collective.casestudy-1.0.0a3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,27 +18,39 @@
 ![Code Style](https://img.shields.io/badge/Code%20Style-Black-000000)
 
 [![GitHub contributors](https://img.shields.io/github/contributors/collective/collective.casestudy)](https://github.com/collective/collective.casestudy)
 [![GitHub Repo stars](https://img.shields.io/github/stars/collective/collective.casestudy?style=social)](https://github.com/collective/collective.casestudy)
 
 </div>
 
-Features
---------
+## Features
 
-**collective.casestudy** provides a Case Study content type to be used in Plone sites.
+`collective.casestudy` provides two new content types to be used in Plone sites, Case Study and Provider.
 
-Documentation
--------------
+### Case Study
 
-This package supports Plone sites using Volto, but each project should provide their own view for this content type.
+A case study of a Plone deployment, which has attributes to track the Plone version used, the industry, and the type of usage of Plone.
 
+### Provider
 
-Installation
-------------
+A company providing Plone services and solutions.
+
+## See it in action
+
+**collective.casestudy** is being used in the following sites:
+
+* [Plone.org](https://plone.org)
+* [Plone Brasil](https://plone.org.br)
+
+## Documentation
+
+This package supports Plone sites using Volto, but each project should provide its view for this content type.
+
+
+### Installation
 
 Add **collective.casestudy** to the Plone installation using `pip`:
 
 ```bash
 pip install collective.casestudy
 ```
 or add it as a dependency on your package's `setup.py`
@@ -51,41 +63,32 @@
         "setuptools",
     ],
 ```
 
 Start Plone and activate the plugin in the addons control-panel.
 
 
-Source Code and Contributions
------------------------------
+## Source Code and Contributions
 
-If you want to help with the development (improvement, update, bug-fixing, ...) of `collective.casestudy` this is a great idea!
+We welcome contributions to `collective.casestudy`.
+You can create an issue in the issue tracker, or contact a maintainer.
 
 - [Issue Tracker](https://github.com/collective/collective.casestudy/issues)
 - [Source Code](https://github.com/collective/collective.casestudy/)
 
 
-We appreciate any contribution and if a release is needed to be done on PyPI, please just contact one of us.
 
-Development
------------
+### Development
 
-You need a working `python` environment (system, virtualenv, pyenv, etc) version 3.7 or superior.
+You need a working Python environment version 3.7 or later.
 
 Then install the dependencies and a development instance using:
 
 ```bash
 make build
 ```
 
-To run tests for this package:
-
-```bash
-make test
-```
-
-By default we use the latest Plone version in the 6.x series.
+By default, we use the latest Plone version in the 6.x series.
 
-License
--------
+## License
 
-The project is licensed under the GPLv2.
+The project is licensed under GPLv2.
```

### Comparing `collective.casestudy-1.0.0a2/docs/icon.svg` & `collective.casestudy-1.0.0a3/docs/icon.svg`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/pyproject.toml` & `collective.casestudy-1.0.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/setup.py` & `collective.casestudy-1.0.0a3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGELOG.md").read_text()}\n
 """
 
 setup(
     name="collective.casestudy",
-    version="1.0.0a2",
+    version="1.0.0a3",
     description="Case Study content type for Plone.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -41,19 +41,15 @@
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["collective"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=True,
     python_requires=">=3.8",
-    install_requires=[
-        "setuptools",
-        "Plone",
-        "plone.api",
-    ],
+    install_requires=["setuptools", "Plone", "plone.api", "pycountry"],
     extras_require={
         "test": [
             "zest.releaser[recommended]",
             "plone.app.testing>=7.0.0a3",
             "plone.restapi[test]",
             "pytest",
             "pytest-cov",
```

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/browser/configure.zcml` & `collective.casestudy-1.0.0a3/src/collective/casestudy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/browser/controlpanel.py` & `collective.casestudy-1.0.0a3/src/collective/casestudy/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/configure.zcml` & `collective.casestudy-1.0.0a3/src/collective/casestudy/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -18,12 +18,13 @@
   <include package="plone.restapi" />
 
   <include file="permissions.zcml" />
   <include file="profiles.zcml" />
 
   <!-- -*- extra stuff goes here -*- -->
 
+  <include package=".behaviors" />
   <include package=".browser" />
   <include package=".indexers" />
   <include package=".vocabularies" />
 
 </configure>
```

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/content/case_study.py` & `collective.casestudy-1.0.0a3/src/collective/casestudy/content/case_study.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/locales/update.py` & `collective.casestudy-1.0.0a3/src/collective/casestudy/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types/CaseStudy.xml` & `collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/types/CaseStudy.xml`

 * *Files 2% similar despite different names*

#### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/profiles/default/types/CaseStudy.xml` & `collective.casestudy-1.0.0a3/src/collective/casestudy/profiles/default/types/CaseStudy.xml`

```diff
@@ -18,14 +18,15 @@
   <property name="add_permission">cmf.AddPortalContent</property>
   <property name="klass">collective.casestudy.content.case_study.CaseStudy</property>
   <property name="model_file"/>
   <property name="model_source"/>
   <property name="schema">collective.casestudy.content.case_study.ICaseStudy</property>
   <!-- Enabled behaviors -->
   <property name="behaviors" purge="false">
+    <element value="collective.casestudy.providers"/>
     <element value="plone.dublincore"/>
     <element value="plone.namefromtitle"/>
     <element value="plone.shortname"/>
     <element value="plone.excludefromnavigation"/>
     <element value="plone.relateditems"/>
     <element value="plone.versioning"/>
     <element value="volto.blocks"/>
```

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/profiles.zcml` & `collective.casestudy-1.0.0a3/src/collective/casestudy/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/industries.py` & `collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/industries.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,9 +7,11 @@
 
 @provider(IVocabularyFactory)
 def industries_vocabulary(context):
     """Vocabulary of industries."""
     terms = []
     industries = api.portal.get_registry_record("casestudy.industries")
     for title in industries:
-        terms.append(SimpleTerm(title, title, title))
+        if "|" in title:
+            token, title = title.split("|")
+        terms.append(SimpleTerm(token, token, title))
     return SimpleVocabulary(terms)
```

### Comparing `collective.casestudy-1.0.0a2/src/collective/casestudy/vocabularies/versions.py` & `collective.casestudy-1.0.0a3/src/collective/casestudy/vocabularies/versions.py`

 * *Files identical despite different names*

### Comparing `collective.casestudy-1.0.0a2/src/collective.casestudy.egg-info/PKG-INFO` & `collective.casestudy-1.0.0a3/src/collective.casestudy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.casestudy
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Case Study content type for Plone.
 Home-page: https://github.com/collective/collective.casestudy
 Author: Plone Community
 Author-email: ericof@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.casestudy
 Project-URL: Source, https://github.com/collective/collective.casestudy
@@ -48,27 +48,39 @@
 ![Code Style](https://img.shields.io/badge/Code%20Style-Black-000000)
 
 [![GitHub contributors](https://img.shields.io/github/contributors/collective/collective.casestudy)](https://github.com/collective/collective.casestudy)
 [![GitHub Repo stars](https://img.shields.io/github/stars/collective/collective.casestudy?style=social)](https://github.com/collective/collective.casestudy)
 
 </div>
 
-Features
---------
+## Features
 
-**collective.casestudy** provides a Case Study content type to be used in Plone sites.
+`collective.casestudy` provides two new content types to be used in Plone sites, Case Study and Provider.
 
-Documentation
--------------
+### Case Study
 
-This package supports Plone sites using Volto, but each project should provide their own view for this content type.
+A case study of a Plone deployment, which has attributes to track the Plone version used, the industry, and the type of usage of Plone.
 
+### Provider
 
-Installation
-------------
+A company providing Plone services and solutions.
+
+## See it in action
+
+**collective.casestudy** is being used in the following sites:
+
+* [Plone.org](https://plone.org)
+* [Plone Brasil](https://plone.org.br)
+
+## Documentation
+
+This package supports Plone sites using Volto, but each project should provide its view for this content type.
+
+
+### Installation
 
 Add **collective.casestudy** to the Plone installation using `pip`:
 
 ```bash
 pip install collective.casestudy
 ```
 or add it as a dependency on your package's `setup.py`
@@ -81,53 +93,55 @@
         "setuptools",
     ],
 ```
 
 Start Plone and activate the plugin in the addons control-panel.
 
 
-Source Code and Contributions
------------------------------
+## Source Code and Contributions
 
-If you want to help with the development (improvement, update, bug-fixing, ...) of `collective.casestudy` this is a great idea!
+We welcome contributions to `collective.casestudy`.
+You can create an issue in the issue tracker, or contact a maintainer.
 
 - [Issue Tracker](https://github.com/collective/collective.casestudy/issues)
 - [Source Code](https://github.com/collective/collective.casestudy/)
 
 
-We appreciate any contribution and if a release is needed to be done on PyPI, please just contact one of us.
 
-Development
------------
+### Development
 
-You need a working `python` environment (system, virtualenv, pyenv, etc) version 3.7 or superior.
+You need a working Python environment version 3.7 or later.
 
 Then install the dependencies and a development instance using:
 
 ```bash
 make build
 ```
 
-To run tests for this package:
+By default, we use the latest Plone version in the 6.x series.
 
-```bash
-make test
-```
+## License
+
+The project is licensed under GPLv2.
 
-By default we use the latest Plone version in the 6.x series.
 
-License
--------
+# Changelog
 
-The project is licensed under the GPLv2.
+## 1.0.0a3 (2023-06-01)
 
+- Add Provider content type #2 [ericof]
+
+- Add Providers behavior [ericof]
+
+- Add catalog indexes for providers, country, services [ericof]
+
+- Update pt_BR translation [ericof]
 
-# Changelog
 
-1.0.0a2 (2023-05-15)
+## 1.0.0a2 (2023-05-15)
 
 - Added Spanish translation [macagua]
 
 - Use `pytest-plone` for testing.
   [ericof]
```

