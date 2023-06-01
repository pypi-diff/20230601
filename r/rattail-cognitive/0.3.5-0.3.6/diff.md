# Comparing `tmp/rattail_cognitive-0.3.5.tar.gz` & `tmp/rattail_cognitive-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rattail_cognitive-0.3.5.tar", last modified: Mon Jan 21 23:29:18 2019, max compression
+gzip compressed data, was "dist/rattail_cognitive-0.3.6.tar", last modified: Thu Jun  1 19:20:08 2023, max compression
```

## Comparing `rattail_cognitive-0.3.5.tar` & `rattail_cognitive-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-01-21 23:29:18.000000 rattail_cognitive-0.3.5/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-01-21 23:29:18.000000 rattail_cognitive-0.3.5/rattail_cognitive.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     2518 2019-01-21 23:29:17.000000 rattail_cognitive-0.3.5/rattail_cognitive.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2019-01-21 23:29:17.000000 rattail_cognitive-0.3.5/rattail_cognitive.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       18 2019-01-21 23:29:17.000000 rattail_cognitive-0.3.5/rattail_cognitive.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2019-01-21 23:29:17.000000 rattail_cognitive-0.3.5/rattail_cognitive.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       15 2019-01-21 23:29:17.000000 rattail_cognitive-0.3.5/rattail_cognitive.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      387 2019-01-21 23:29:17.000000 rattail_cognitive-0.3.5/rattail_cognitive.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2019-01-21 23:29:18.000000 rattail_cognitive-0.3.5/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     2518 2019-01-21 23:29:18.000000 rattail_cognitive-0.3.5/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      646 2019-01-21 23:28:23.000000 rattail_cognitive-0.3.5/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)       28 2014-01-28 16:55:26.000000 rattail_cognitive-0.3.5/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)      336 2017-07-07 15:18:40.000000 rattail_cognitive-0.3.5/README.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     3902 2017-07-07 15:18:57.000000 rattail_cognitive-0.3.5/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:17:22.000000 rattail_cognitive-0.3.5/COPYING.txt
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2019-01-21 23:29:18.000000 rattail_cognitive-0.3.5/rattail_cognitive/
--rw-r--r--   0 lance     (1000) lance     (1000)     1025 2017-07-07 15:18:05.000000 rattail_cognitive-0.3.5/rattail_cognitive/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3119 2018-12-05 00:51:08.000000 rattail_cognitive-0.3.5/rattail_cognitive/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2019-01-21 23:28:30.000000 rattail_cognitive-0.3.5/rattail_cognitive/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:20:08.000000 rattail_cognitive-0.3.6/
+-rw-r--r--   0 lance     (1000) lance     (1000)       28 2014-01-28 16:55:26.000000 rattail_cognitive-0.3.6/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)      975 2023-05-16 19:19:56.000000 rattail_cognitive-0.3.6/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1016 2023-06-01 19:20:08.000000 rattail_cognitive-0.3.6/setup.cfg
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:20:08.000000 rattail_cognitive-0.3.6/rattail_cognitive.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-01 19:20:07.000000 rattail_cognitive-0.3.6/rattail_cognitive.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-01 19:20:07.000000 rattail_cognitive-0.3.6/rattail_cognitive.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)      397 2023-06-01 19:20:07.000000 rattail_cognitive-0.3.6/rattail_cognitive.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       15 2023-06-01 19:20:07.000000 rattail_cognitive-0.3.6/rattail_cognitive.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       18 2023-06-01 19:20:07.000000 rattail_cognitive-0.3.6/rattail_cognitive.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1341 2023-06-01 19:20:07.000000 rattail_cognitive-0.3.6/rattail_cognitive.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:17:22.000000 rattail_cognitive-0.3.6/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      739 2023-06-01 19:19:52.000000 rattail_cognitive-0.3.6/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)      336 2017-07-07 15:18:40.000000 rattail_cognitive-0.3.6/README.txt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:20:08.000000 rattail_cognitive-0.3.6/rattail_cognitive/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3119 2018-12-05 00:51:08.000000 rattail_cognitive-0.3.6/rattail_cognitive/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-06-01 19:19:55.000000 rattail_cognitive-0.3.6/rattail_cognitive/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1025 2017-07-07 15:18:05.000000 rattail_cognitive-0.3.6/rattail_cognitive/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1341 2023-06-01 19:20:08.000000 rattail_cognitive-0.3.6/PKG-INFO
```

### Comparing `rattail_cognitive-0.3.5/CHANGES.rst` & `rattail_cognitive-0.3.6/CHANGES.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 CHANGELOG
 =========
 
+0.3.6 (2023-06-01)
+------------------
+
+* Replace ``setup.py`` contents with ``setup.cfg``.
+
+
 0.3.5 (2019-01-21)
 ------------------
 
 * Remove unused reference to ``cStringIO``.
 
 
 0.3.4 (2017-07-07)
```

### Comparing `rattail_cognitive-0.3.5/COPYING.txt` & `rattail_cognitive-0.3.6/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail_cognitive-0.3.5/rattail_cognitive/__init__.py` & `rattail_cognitive-0.3.6/rattail_cognitive/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_cognitive-0.3.5/rattail_cognitive/labels.py` & `rattail_cognitive-0.3.6/rattail_cognitive/labels.py`

 * *Files identical despite different names*

