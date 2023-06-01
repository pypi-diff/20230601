# Comparing `tmp/wafpd-0.0.2.tar.gz` & `tmp/wafpd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafpd-0.0.2.tar", last modified: Thu Jun  1 18:04:02 2023, max compression
+gzip compressed data, was "wafpd-0.0.3.tar", last modified: Thu Jun  1 18:39:58 2023, max compression
```

## Comparing `wafpd-0.0.2.tar` & `wafpd-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:04:02.852284 wafpd-0.0.2/
--rw-rw-rw-   0        0        0      426 2023-06-01 18:04:02.848284 wafpd-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 18:04:02.853284 wafpd-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-06-01 18:03:21.000000 wafpd-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:04:02.751274 wafpd-0.0.2/wafpd/
--rw-rw-rw-   0        0        0       34 2023-06-01 18:03:38.000000 wafpd-0.0.2/wafpd/__init__.py
--rw-rw-rw-   0        0        0      976 2023-06-01 18:03:36.000000 wafpd-0.0.2/wafpd/wafpd.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:04:02.844285 wafpd-0.0.2/wafpd.egg-info/
--rw-rw-rw-   0        0        0      426 2023-06-01 18:04:02.000000 wafpd-0.0.2/wafpd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-01 18:04:02.000000 wafpd-0.0.2/wafpd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:04:02.000000 wafpd-0.0.2/wafpd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-01 18:04:02.000000 wafpd-0.0.2/wafpd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-01 18:04:02.000000 wafpd-0.0.2/wafpd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 18:39:58.333487 wafpd-0.0.3/
+-rw-rw-rw-   0        0        0      437 2023-06-01 18:39:58.330488 wafpd-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:39:58.334487 wafpd-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      747 2023-06-01 18:39:24.000000 wafpd-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:39:58.172473 wafpd-0.0.3/wafpd/
+-rw-rw-rw-   0        0        0       65 2023-06-01 18:33:31.000000 wafpd-0.0.3/wafpd/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-06-01 18:32:59.000000 wafpd-0.0.3/wafpd/wafpd.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:39:58.322486 wafpd-0.0.3/wafpd.egg-info/
+-rw-rw-rw-   0        0        0      437 2023-06-01 18:39:57.000000 wafpd-0.0.3/wafpd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-01 18:39:58.000000 wafpd-0.0.3/wafpd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:39:57.000000 wafpd-0.0.3/wafpd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 18:39:57.000000 wafpd-0.0.3/wafpd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 18:39:57.000000 wafpd-0.0.3/wafpd.egg-info/top_level.txt
```

### Comparing `wafpd-0.0.2/setup.py` & `wafpd-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
-DESCRIPTION = 'Command analyzer for pandas'
+VERSION = '0.0.3'
+DESCRIPTION = 'Command analyzer for pandas new versin'
 
 # Setting up
 setup(
     name="wafpd",
     version=VERSION,
-    author="TAFPD team",
+    author="WAFPD team",
     author_email="giokhvichia69@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/plain",
     packages=find_packages(),
     install_requires=[
-        "nltk"  # Add any additional dependencies here
+        "nltk" , "pandas" # Add any additional dependencies here
     ],
     keywords=['python', 'data', 'analyze', 'information'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

