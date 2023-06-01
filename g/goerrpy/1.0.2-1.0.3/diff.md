# Comparing `tmp/goerrpy-1.0.2.tar.gz` & `tmp/goerrpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goerrpy-1.0.2.tar", last modified: Thu Jun  1 21:30:09 2023, max compression
+gzip compressed data, was "goerrpy-1.0.3.tar", last modified: Thu Jun  1 21:40:48 2023, max compression
```

## Comparing `goerrpy-1.0.2.tar` & `goerrpy-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:30:09.402290 goerrpy-1.0.2/
--rw-r--r--   0 mbozhilov   (505) staff       (20)      433 2023-06-01 21:30:09.402154 goerrpy-1.0.2/PKG-INFO
--rw-r--r--   0 mbozhilov   (505) staff       (20)       67 2023-06-01 21:07:37.000000 goerrpy-1.0.2/README.md
-drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:30:09.401174 goerrpy-1.0.2/goerrpy/
--rw-r--r--   0 mbozhilov   (505) staff       (20)       63 2023-06-01 21:29:57.000000 goerrpy-1.0.2/goerrpy/__init__.py
--rw-r--r--   0 mbozhilov   (505) staff       (20)      457 2023-06-01 09:14:30.000000 goerrpy-1.0.2/goerrpy/decorators.py
-drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:30:09.401945 goerrpy-1.0.2/goerrpy.egg-info/
--rw-r--r--   0 mbozhilov   (505) staff       (20)      433 2023-06-01 21:30:09.000000 goerrpy-1.0.2/goerrpy.egg-info/PKG-INFO
--rw-r--r--   0 mbozhilov   (505) staff       (20)      184 2023-06-01 21:30:09.000000 goerrpy-1.0.2/goerrpy.egg-info/SOURCES.txt
--rw-r--r--   0 mbozhilov   (505) staff       (20)        1 2023-06-01 21:30:09.000000 goerrpy-1.0.2/goerrpy.egg-info/dependency_links.txt
--rw-r--r--   0 mbozhilov   (505) staff       (20)        8 2023-06-01 21:30:09.000000 goerrpy-1.0.2/goerrpy.egg-info/top_level.txt
--rw-r--r--   0 mbozhilov   (505) staff       (20)       38 2023-06-01 21:30:09.402336 goerrpy-1.0.2/setup.cfg
--rw-r--r--   0 mbozhilov   (505) staff       (20)      522 2023-06-01 21:29:12.000000 goerrpy-1.0.2/setup.py
+drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:40:48.046304 goerrpy-1.0.3/
+-rw-r--r--   0 mbozhilov   (505) staff       (20)     1595 2023-06-01 21:40:48.046156 goerrpy-1.0.3/PKG-INFO
+-rw-r--r--   0 mbozhilov   (505) staff       (20)     1228 2023-06-01 21:40:33.000000 goerrpy-1.0.3/README.md
+drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:40:48.045339 goerrpy-1.0.3/goerrpy/
+-rw-r--r--   0 mbozhilov   (505) staff       (20)       63 2023-06-01 21:29:57.000000 goerrpy-1.0.3/goerrpy/__init__.py
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      457 2023-06-01 09:14:30.000000 goerrpy-1.0.3/goerrpy/decorators.py
+drwxr-xr-x   0 mbozhilov   (505) staff       (20)        0 2023-06-01 21:40:48.045962 goerrpy-1.0.3/goerrpy.egg-info/
+-rw-r--r--   0 mbozhilov   (505) staff       (20)     1595 2023-06-01 21:40:48.000000 goerrpy-1.0.3/goerrpy.egg-info/PKG-INFO
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      184 2023-06-01 21:40:48.000000 goerrpy-1.0.3/goerrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mbozhilov   (505) staff       (20)        1 2023-06-01 21:40:48.000000 goerrpy-1.0.3/goerrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mbozhilov   (505) staff       (20)        8 2023-06-01 21:40:48.000000 goerrpy-1.0.3/goerrpy.egg-info/top_level.txt
+-rw-r--r--   0 mbozhilov   (505) staff       (20)       38 2023-06-01 21:40:48.046355 goerrpy-1.0.3/setup.cfg
+-rw-r--r--   0 mbozhilov   (505) staff       (20)      522 2023-06-01 21:40:22.000000 goerrpy-1.0.3/setup.py
```

### Comparing `goerrpy-1.0.2/setup.py` & `goerrpy-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='goerrpy',
-    version='1.0.2',
+    version='1.0.3',
     author='Michael Bozhilov',
     author_email='michaelbozhilov@gmail.com',
     description="Decorator for simulating Golang's error handling in Python",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/asynchroza/goerrpy',
     packages=["goerrpy"],
```

