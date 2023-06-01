# Comparing `tmp/TAFPD-0.0.1.tar.gz` & `tmp/TAFPD-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TAFPD-0.0.1.tar", last modified: Thu Jun  1 09:43:53 2023, max compression
+gzip compressed data, was "TAFPD-0.0.2.tar", last modified: Thu Jun  1 17:43:47 2023, max compression
```

## Comparing `TAFPD-0.0.1.tar` & `TAFPD-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:43:53.516848 TAFPD-0.0.1/
--rw-rw-rw-   0        0        0      421 2023-06-01 09:43:53.512847 TAFPD-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 09:43:53.236784 TAFPD-0.0.1/TAFPD/
--rw-rw-rw-   0        0        0        0 2023-06-01 09:21:26.000000 TAFPD-0.0.1/TAFPD/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-01 09:21:51.000000 TAFPD-0.0.1/TAFPD/tafpd.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:43:53.508845 TAFPD-0.0.1/TAFPD.egg-info/
--rw-rw-rw-   0        0        0      421 2023-06-01 09:43:52.000000 TAFPD-0.0.1/TAFPD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-06-01 09:43:53.000000 TAFPD-0.0.1/TAFPD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:43:52.000000 TAFPD-0.0.1/TAFPD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-01 09:43:52.000000 TAFPD-0.0.1/TAFPD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:43:53.516848 TAFPD-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-06-01 09:24:35.000000 TAFPD-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:43:47.618974 TAFPD-0.0.2/
+-rw-rw-rw-   0        0        0      418 2023-06-01 17:43:47.609973 TAFPD-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 17:43:47.526968 TAFPD-0.0.2/TAFPD new nersion/
+-rw-rw-rw-   0        0        0       47 2023-06-01 17:35:29.000000 TAFPD-0.0.2/TAFPD new nersion/__init__.py
+-rw-rw-rw-   0        0        0     1082 2023-06-01 17:35:32.000000 TAFPD-0.0.2/TAFPD new nersion/tafpd.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:43:47.604970 TAFPD-0.0.2/TAFPD.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-06-01 17:43:47.000000 TAFPD-0.0.2/TAFPD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-06-01 17:43:47.000000 TAFPD-0.0.2/TAFPD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 17:43:47.000000 TAFPD-0.0.2/TAFPD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 17:43:47.000000 TAFPD-0.0.2/TAFPD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 17:43:47.619973 TAFPD-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      682 2023-06-01 15:01:04.000000 TAFPD-0.0.2/setup.py
```

### Comparing `TAFPD-0.0.1/setup.py` & `TAFPD-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'command analythor'
 
 # Setting up
 setup(
     name="TAFPD",
     version=VERSION,
     author="TAFPD team",
     author_email="<giokhvichia69@gmail.com>",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/plain",
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'data', 'analyse', 'information'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

