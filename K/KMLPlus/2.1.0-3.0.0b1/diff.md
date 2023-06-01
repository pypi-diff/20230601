# Comparing `tmp/KMLPlus-2.1.0.tar.gz` & `tmp/KMLPlus-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMLPlus-2.1.0.tar", last modified: Wed Jan 27 12:18:08 2021, max compression
+gzip compressed data, was "KMLPlus-3.0.0b1.tar", last modified: Thu Jun  1 17:55:21 2023, max compression
```

## Comparing `KMLPlus-2.1.0.tar` & `KMLPlus-3.0.0b1.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-01-27 12:18:08.589393 KMLPlus-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-01-27 12:18:08.585393 KMLPlus-2.1.0/KMLPlus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15924 2021-01-27 12:18:08.000000 KMLPlus-2.1.0/KMLPlus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      263 2021-01-27 12:18:08.000000 KMLPlus-2.1.0/KMLPlus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2021-01-27 12:18:08.000000 KMLPlus-2.1.0/KMLPlus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2021-01-27 12:18:08.000000 KMLPlus-2.1.0/KMLPlus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    15924 2021-01-27 12:18:08.589393 KMLPlus-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12222 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-01-27 12:18:08.585393 KMLPlus-2.1.0/kmlplus/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/kmlplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12329 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/kmlplus/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15502 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/kmlplus/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2021-01-27 12:18:08.589393 KMLPlus-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      750 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-01-27 12:18:08.589393 KMLPlus-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5320 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/test/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (122)    11885 2021-01-27 12:17:59.000000 KMLPlus-2.1.0/test/test_paths.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.798368 KMLPlus-3.0.0b1/
+drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.789357 KMLPlus-3.0.0b1/KMLPlus.egg-info/
+-rw-rw-rw-   0        0        0    11555 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2022-08-16 13:56:01.000000 KMLPlus-3.0.0b1/LICENSE
+-rw-rw-rw-   0        0        0    11555 2023-06-01 17:55:21.797367 KMLPlus-3.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0    10998 2023-06-01 17:11:25.000000 KMLPlus-3.0.0b1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.793363 KMLPlus-3.0.0b1/kmlplus/
+-rw-rw-rw-   0        0        0        0 2023-05-26 14:38:48.000000 KMLPlus-3.0.0b1/kmlplus/__init__.py
+-rw-rw-rw-   0        0        0    23313 2023-06-01 17:02:09.000000 KMLPlus-3.0.0b1/kmlplus/geo.py
+-rw-rw-rw-   0        0        0     3157 2023-06-01 16:07:02.000000 KMLPlus-3.0.0b1/kmlplus/interface.py
+-rw-rw-rw-   0        0        0    10477 2023-06-01 17:55:14.000000 KMLPlus-3.0.0b1/kmlplus/kml.py
+-rw-rw-rw-   0        0        0    21374 2023-06-01 16:07:02.000000 KMLPlus-3.0.0b1/kmlplus/shapes.py
+-rw-rw-rw-   0        0        0     3924 2023-05-26 10:58:29.000000 KMLPlus-3.0.0b1/kmlplus/util.py
+-rw-rw-rw-   0        0        0       42 2023-06-01 17:55:21.798368 KMLPlus-3.0.0b1/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-06-01 17:55:14.000000 KMLPlus-3.0.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.796367 KMLPlus-3.0.0b1/test/
+-rw-rw-rw-   0        0        0        0 2022-08-16 13:56:01.000000 KMLPlus-3.0.0b1/test/__init__.py
+-rw-rw-rw-   0        0        0     9603 2023-06-01 17:00:43.000000 KMLPlus-3.0.0b1/test/test_geo.py
+-rw-rw-rw-   0        0        0     5365 2023-06-01 17:02:31.000000 KMLPlus-3.0.0b1/test/test_shapes.py
+-rw-rw-rw-   0        0        0     4161 2023-06-01 15:57:55.000000 KMLPlus-3.0.0b1/test/test_util.py
```

### Comparing `KMLPlus-2.1.0/setup.py` & `KMLPlus-3.0.0b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="KMLPlus",  # Replace with your own username
-    version="2.1.0",
-    author="Mark Henderson",
-    author_email="mark.henderson1988@gmail.com",
-    description="A Python library for creating 3d floating polygons and circles in .kml for Google Earth.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/MHenderson1988/kmlplus",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.8',
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="KMLPlus",  # Replace with your own username
+    version="3.0.0-beta.1",
+    author="Mark Henderson",
+    author_email="mark.henderson1988@gmail.com",
+    description="A Python library for creating 3d floating polygons and circles in .kml for Google Earth.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/MHenderson1988/kmlplus",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.8',
+)
```

