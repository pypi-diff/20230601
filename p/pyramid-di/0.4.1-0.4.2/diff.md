# Comparing `tmp/pyramid_di-0.4.1.tar.gz` & `tmp/pyramid_di-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_di-0.4.1.tar", last modified: Fri Mar 19 13:01:25 2021, max compression
+gzip compressed data, was "pyramid_di-0.4.2.tar", last modified: Thu Jun  1 20:29:32 2023, max compression
```

## Comparing `pyramid_di-0.4.1.tar` & `pyramid_di-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 13:01:25.407446 pyramid_di-0.4.1/
--rw-r--r--   0 ztane     (1000) ztane     (1000)      568 2021-03-19 13:00:46.000000 pyramid_di-0.4.1/CHANGES.md
--rw-r--r--   0 ztane     (1000) ztane     (1000)       56 2020-11-25 08:55:18.000000 pyramid_di-0.4.1/MANIFEST.in
--rw-r--r--   0 ztane     (1000) ztane     (1000)     4817 2021-03-19 13:01:25.407446 pyramid_di-0.4.1/PKG-INFO
--rw-r--r--   0 ztane     (1000) ztane     (1000)     2063 2020-11-25 08:59:21.000000 pyramid_di-0.4.1/README.md
--rw-r--r--   0 ztane     (1000) ztane     (1000)      113 2020-11-14 08:43:08.000000 pyramid_di-0.4.1/coveragerc-python3
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 13:01:25.407446 pyramid_di-0.4.1/pyramid_di/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     7255 2021-03-19 12:58:01.000000 pyramid_di-0.4.1/pyramid_di/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 13:01:25.407446 pyramid_di-0.4.1/pyramid_di.egg-info/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     4817 2021-03-19 13:01:25.000000 pyramid_di-0.4.1/pyramid_di.egg-info/PKG-INFO
--rw-r--r--   0 ztane     (1000) ztane     (1000)      321 2021-03-19 13:01:25.000000 pyramid_di-0.4.1/pyramid_di.egg-info/SOURCES.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)        1 2021-03-19 13:01:25.000000 pyramid_di-0.4.1/pyramid_di.egg-info/dependency_links.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)        1 2020-11-13 18:46:18.000000 pyramid_di-0.4.1/pyramid_di.egg-info/not-zip-safe
--rw-r--r--   0 ztane     (1000) ztane     (1000)       59 2021-03-19 13:01:25.000000 pyramid_di-0.4.1/pyramid_di.egg-info/requires.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)       11 2021-03-19 13:01:25.000000 pyramid_di-0.4.1/pyramid_di.egg-info/top_level.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)      191 2021-03-19 13:01:25.407446 pyramid_di-0.4.1/setup.cfg
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1575 2021-03-19 12:59:13.000000 pyramid_di-0.4.1/setup.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 13:01:25.407446 pyramid_di-0.4.1/tests/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     3205 2020-11-19 09:01:12.000000 pyramid_di-0.4.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 20:29:32.428998 pyramid_di-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-01 20:29:21.000000 pyramid_di-0.4.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-01 20:29:21.000000 pyramid_di-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-01 20:29:32.428998 pyramid_di-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2063 2023-06-01 20:29:21.000000 pyramid_di-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-01 20:29:21.000000 pyramid_di-0.4.2/coveragerc-python3
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 20:29:32.428998 pyramid_di-0.4.2/pyramid_di/
+-rw-r--r--   0 runner    (1001) docker     (122)     7255 2023-06-01 20:29:21.000000 pyramid_di-0.4.2/pyramid_di/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 20:29:32.428998 pyramid_di-0.4.2/pyramid_di.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-01 20:29:32.000000 pyramid_di-0.4.2/pyramid_di.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-01 20:29:32.000000 pyramid_di-0.4.2/pyramid_di.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 20:29:32.000000 pyramid_di-0.4.2/pyramid_di.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 20:29:32.000000 pyramid_di-0.4.2/pyramid_di.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-01 20:29:32.000000 pyramid_di-0.4.2/pyramid_di.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-01 20:29:32.000000 pyramid_di-0.4.2/pyramid_di.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-01 20:29:32.428998 pyramid_di-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-06-01 20:29:21.000000 pyramid_di-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 20:29:32.428998 pyramid_di-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-01 20:29:21.000000 pyramid_di-0.4.2/tests/test_integration.py
```

### Comparing `pyramid_di-0.4.1/README.md` & `pyramid_di-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyramid_di-0.4.1/pyramid_di/__init__.py` & `pyramid_di-0.4.2/pyramid_di/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from zope.interface import Interface
 from zope.interface.interface import InterfaceClass
 from functools import update_wrapper
 from pyramid_services import _resolve_iface
 import warnings
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 _to_underscores = re.compile("((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))")
 
 
 class reify_attr(object):
     """
```

### Comparing `pyramid_di-0.4.1/setup.py` & `pyramid_di-0.4.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-import os, sys
+from pathlib import Path
 
 from setuptools import setup, find_packages
 
-here = os.path.abspath(os.path.dirname(__file__))
-README = open(os.path.join(here, "README.md")).read()
-CHANGES = open(os.path.join(here, "CHANGES.md")).read()
+here = Path(__file__).parent
+README = (here / "README.md").read_text()
+CHANGES = (here / "CHANGES.md").read_text()
 
-requires = ["pyramid>=1.7,<2.0", "pyramid_services>=1.1,<2.0"]
-dev_requires = ["pytest"]
+requires = ["pyramid>=1.7,<3.0", "pyramid_services>=1.1,<2.0"]
+dev_requires = ["pytest>=3.0", "pytest-cov"]
 
 setup(
     name="pyramid_di",
-    version="0.4.1",
+    version="0.4.2",
     description="Dependency injection stuff for Pyramid",
     long_description=README + "\n\n" + CHANGES,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: Pyramid",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Python Software Foundation License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Internet :: WWW/HTTP :: WSGI",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
     author="Antti Haapala",
```

### Comparing `pyramid_di-0.4.1/tests/test_integration.py` & `pyramid_di-0.4.2/tests/test_integration.py`

 * *Files identical despite different names*

