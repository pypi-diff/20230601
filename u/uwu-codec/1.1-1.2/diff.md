# Comparing `tmp/uwu_codec-1.1.tar.gz` & `tmp/uwu_codec-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwu_codec-1.1.tar", last modified: Fri May 19 22:36:56 2023, max compression
+gzip compressed data, was "uwu_codec-1.2.tar", last modified: Thu Jun  1 13:52:26 2023, max compression
```

## Comparing `uwu_codec-1.1.tar` & `uwu_codec-1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-19 22:36:56.191754 uwu_codec-1.1/
--rw-r--r--   0 goldy     (1001) goldy     (1001)       66 2023-05-16 23:04:32.000000 uwu_codec-1.1/.gitattributes
--rw-r--r--   0 goldy     (1001) goldy     (1001)       52 2023-05-16 22:47:20.000000 uwu_codec-1.1/.gitignore
--rwxr-xr-x   0 goldy     (1001) goldy     (1001)       74 2023-05-16 21:46:14.000000 uwu_codec-1.1/Makefile
--rw-r--r--   0 goldy     (1001) goldy     (1001)     3638 2023-05-19 22:36:56.191754 uwu_codec-1.1/PKG-INFO
--rw-r--r--   0 goldy     (1001) goldy     (1001)     2719 2023-05-16 22:47:26.000000 uwu_codec-1.1/README.md
--rw-r--r--   0 goldy     (1001) goldy     (1001)     2633 2023-05-16 23:08:12.000000 uwu_codec-1.1/pyproject.toml
--rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-05-19 22:36:56.191754 uwu_codec-1.1/setup.cfg
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-19 22:36:56.190754 uwu_codec-1.1/uwu_codec/
--rw-r--r--   0 goldy     (1001) goldy     (1001)      517 2023-05-19 22:36:45.000000 uwu_codec-1.1/uwu_codec/__init__.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1387 2023-05-19 22:21:52.000000 uwu_codec-1.1/uwu_codec/codec.py
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-19 22:36:56.191754 uwu_codec-1.1/uwu_codec.egg-info/
--rw-r--r--   0 goldy     (1001) goldy     (1001)     3638 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1001) goldy     (1001)      264 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)      106 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/requires.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)       10 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/top_level.txt
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-06-01 13:52:26.421333 uwu_codec-1.2/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       66 2023-05-16 23:04:32.000000 uwu_codec-1.2/.gitattributes
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       52 2023-05-16 22:47:20.000000 uwu_codec-1.2/.gitignore
+-rwxr-xr-x   0 goldy     (1001) goldy     (1001)       74 2023-05-16 21:46:14.000000 uwu_codec-1.2/Makefile
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3638 2023-06-01 13:52:26.421333 uwu_codec-1.2/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2719 2023-05-16 22:47:26.000000 uwu_codec-1.2/README.md
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2633 2023-05-16 23:08:12.000000 uwu_codec-1.2/pyproject.toml
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-06-01 13:52:26.421333 uwu_codec-1.2/setup.cfg
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-06-01 13:52:26.420333 uwu_codec-1.2/uwu_codec/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      909 2023-06-01 13:51:20.000000 uwu_codec-1.2/uwu_codec/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1387 2023-05-31 13:16:20.000000 uwu_codec-1.2/uwu_codec/codec.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     9236 2023-05-31 13:17:28.000000 uwu_codec-1.2/uwu_codec/stream_reader.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1335 2023-05-31 13:17:35.000000 uwu_codec-1.2/uwu_codec/stream_writer.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-06-01 13:52:26.421333 uwu_codec-1.2/uwu_codec.egg-info/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3638 2023-06-01 13:52:26.000000 uwu_codec-1.2/uwu_codec.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      318 2023-06-01 13:52:26.000000 uwu_codec-1.2/uwu_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-06-01 13:52:26.000000 uwu_codec-1.2/uwu_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      106 2023-06-01 13:52:26.000000 uwu_codec-1.2/uwu_codec.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       10 2023-06-01 13:52:26.000000 uwu_codec-1.2/uwu_codec.egg-info/top_level.txt
```

### Comparing `uwu_codec-1.1/PKG-INFO` & `uwu_codec-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwu_codec
-Version: 1.1
+Version: 1.2
 Summary: Yep, your eyes are not deceiving you. An UwU codec. 😳 Currently WIP...
 Author-email: Goldy <goldy@devgoldy.xyz>
 Project-URL: GitHub, https://github.com/THEGOLDENPRO/uwu-codec
 Project-URL: BugTracker, https://github.com/THEGOLDENPRO/uwu-codec/issues
 Keywords: uwu,UwU,UwU Codec,uwu-codec,uwu encoder,uwu decoder
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `uwu_codec-1.1/README.md` & `uwu_codec-1.2/README.md`

 * *Files identical despite different names*

### Comparing `uwu_codec-1.1/pyproject.toml` & `uwu_codec-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uwu_codec-1.1/uwu_codec/codec.py` & `uwu_codec-1.2/uwu_codec/codec.py`

 * *Files identical despite different names*

### Comparing `uwu_codec-1.1/uwu_codec.egg-info/PKG-INFO` & `uwu_codec-1.2/uwu_codec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwu-codec
-Version: 1.1
+Version: 1.2
 Summary: Yep, your eyes are not deceiving you. An UwU codec. 😳 Currently WIP...
 Author-email: Goldy <goldy@devgoldy.xyz>
 Project-URL: GitHub, https://github.com/THEGOLDENPRO/uwu-codec
 Project-URL: BugTracker, https://github.com/THEGOLDENPRO/uwu-codec/issues
 Keywords: uwu,UwU,UwU Codec,uwu-codec,uwu encoder,uwu decoder
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

