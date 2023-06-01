# Comparing `tmp/nopaths-5.tar.gz` & `tmp/nopaths-6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopaths-5.tar", last modified: Thu Jun  1 00:14:07 2023, max compression
+gzip compressed data, was "nopaths-6.tar", last modified: Thu Jun  1 02:16:28 2023, max compression
```

## Comparing `nopaths-5.tar` & `nopaths-6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.096813 nopaths-5/
--rw-r--r--   0 nop       (1000) nop       (1000)     4839 2023-06-01 00:14:07.096813 nopaths-5/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     3053 2023-05-31 23:12:25.000000 nopaths-5/README.rst
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.088813 nopaths-5/bin/
--rwxr-xr-x   0 nop       (1000) nop       (1000)       24 2023-05-31 22:10:03.000000 nopaths-5/bin/nopaths
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/nopaths/
--rw-r--r--   0 nop       (1000) nop       (1000)     1350 2023-05-31 22:58:00.000000 nopaths-5/nopaths/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2284 2023-06-01 00:10:58.000000 nopaths-5/nopaths/__main__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      568 2023-05-31 18:48:29.000000 nopaths-5/nopaths/clients.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1086 2023-05-31 18:48:44.000000 nopaths-5/nopaths/clocked.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2603 2023-05-31 19:48:57.000000 nopaths-5/nopaths/command.py
--rw-r--r--   0 nop       (1000) nop       (1000)      159 2023-05-31 17:48:19.000000 nopaths-5/nopaths/configs.py
--rw-r--r--   0 nop       (1000) nop       (1000)      796 2023-05-31 17:48:47.000000 nopaths-5/nopaths/decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-31 18:53:59.000000 nopaths-5/nopaths/default.py
--rw-r--r--   0 nop       (1000) nop       (1000)      299 2023-05-31 20:02:22.000000 nopaths-5/nopaths/defines.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1322 2023-05-31 19:50:08.000000 nopaths-5/nopaths/encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      348 2023-05-31 19:52:08.000000 nopaths-5/nopaths/errored.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1968 2023-05-31 19:51:30.000000 nopaths-5/nopaths/handler.py
--rw-r--r--   0 nop       (1000) nop       (1000)      939 2023-05-31 18:49:17.000000 nopaths-5/nopaths/listens.py
--rw-r--r--   0 nop       (1000) nop       (1000)      441 2023-05-31 18:41:00.000000 nopaths-5/nopaths/logging.py
--rw-r--r--   0 nop       (1000) nop       (1000)      940 2023-05-31 18:47:45.000000 nopaths-5/nopaths/message.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/nopaths/modules/
--rw-r--r--   0 nop       (1000) nop       (1000)     1786 2023-05-31 19:59:21.000000 nopaths-5/nopaths/modules/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      576 2023-05-31 23:58:48.000000 nopaths-5/nopaths/modules/cfg.py
--rw-r--r--   0 nop       (1000) nop       (1000)      211 2023-05-31 17:40:41.000000 nopaths-5/nopaths/modules/cmd.py
--rw-r--r--   0 nop       (1000) nop       (1000)      704 2023-05-31 23:52:18.000000 nopaths-5/nopaths/modules/err.py
--rw-r--r--   0 nop       (1000) nop       (1000)      418 2023-05-31 18:50:47.000000 nopaths-5/nopaths/modules/flt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      964 2023-05-31 19:54:01.000000 nopaths-5/nopaths/modules/fnd.py
--rw-r--r--   0 nop       (1000) nop       (1000)    20506 2023-05-31 23:56:50.000000 nopaths-5/nopaths/modules/irc.py
--rw-r--r--   0 nop       (1000) nop       (1000)      705 2023-05-31 19:44:53.000000 nopaths-5/nopaths/modules/log.py
--rw-r--r--   0 nop       (1000) nop       (1000)      176 2023-05-31 17:36:44.000000 nopaths-5/nopaths/modules/mod.py
--rw-r--r--   0 nop       (1000) nop       (1000)     7710 2023-05-31 23:56:18.000000 nopaths-5/nopaths/modules/rss.py
--rw-r--r--   0 nop       (1000) nop       (1000)      346 2023-05-31 17:33:36.000000 nopaths-5/nopaths/modules/sts.py
--rw-r--r--   0 nop       (1000) nop       (1000)      939 2023-05-31 19:43:02.000000 nopaths-5/nopaths/modules/tdo.py
--rw-r--r--   0 nop       (1000) nop       (1000)      987 2023-05-31 19:45:11.000000 nopaths-5/nopaths/modules/thr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      218 2023-05-31 17:35:13.000000 nopaths-5/nopaths/modules/upt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      173 2023-05-31 17:38:42.000000 nopaths-5/nopaths/modules/ver.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2011 2023-05-31 23:55:17.000000 nopaths-5/nopaths/objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2133 2023-05-31 20:04:26.000000 nopaths-5/nopaths/objfunc.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1810 2023-05-31 20:05:12.000000 nopaths-5/nopaths/parsers.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4719 2023-05-31 19:51:41.000000 nopaths-5/nopaths/persist.py
--rw-r--r--   0 nop       (1000) nop       (1000)      355 2023-05-31 18:48:57.000000 nopaths-5/nopaths/repeats.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2684 2023-05-31 19:51:04.000000 nopaths-5/nopaths/runtime.py
--rw-r--r--   0 nop       (1000) nop       (1000)      894 2023-05-31 18:43:38.000000 nopaths-5/nopaths/threads.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2933 2023-05-31 23:54:10.000000 nopaths-5/nopaths/utility.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/nopaths.egg-info/
--rw-r--r--   0 nop       (1000) nop       (1000)     4839 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     1121 2023-06-01 00:14:07.000000 nopaths-5/nopaths.egg-info/SOURCES.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/dependency_links.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/top_level.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/zip-safe
--rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-06-01 00:14:07.096813 nopaths-5/setup.cfg
--rw-r--r--   0 nop       (1000) nop       (1000)      852 2023-05-31 23:45:37.000000 nopaths-5/setup.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/test/
--rw-r--r--   0 nop       (1000) nop       (1000)      718 2023-06-01 00:04:43.000000 nopaths-5/test/test_composite.py
--rw-r--r--   0 nop       (1000) nop       (1000)      553 2023-06-01 00:10:34.000000 nopaths-5/test/test_decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      448 2023-06-01 00:12:25.000000 nopaths-5/test/test_encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      969 2023-06-01 00:02:56.000000 nopaths-5/test/test_inherit.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4657 2023-06-01 00:08:52.000000 nopaths-5/test/test_objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)      687 2023-05-31 23:51:14.000000 nopaths-5/test/test_recursive.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1159 2023-06-01 00:01:11.000000 nopaths-5/test/test_storage.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 02:16:28.224628 nopaths-6/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4831 2023-06-01 02:16:28.224628 nopaths-6/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     3045 2023-06-01 00:23:53.000000 nopaths-6/README.rst
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 02:16:28.220628 nopaths-6/bin/
+-rwxr-xr-x   0 nop       (1000) nop       (1000)       24 2023-05-31 22:10:03.000000 nopaths-6/bin/nopaths
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 02:16:28.224628 nopaths-6/nopaths/
+-rw-r--r--   0 nop       (1000) nop       (1000)     1350 2023-05-31 22:58:00.000000 nopaths-6/nopaths/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2284 2023-06-01 00:10:58.000000 nopaths-6/nopaths/__main__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      568 2023-05-31 18:48:29.000000 nopaths-6/nopaths/clients.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1086 2023-05-31 18:48:44.000000 nopaths-6/nopaths/clocked.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2603 2023-05-31 19:48:57.000000 nopaths-6/nopaths/command.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      159 2023-05-31 17:48:19.000000 nopaths-6/nopaths/configs.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      796 2023-05-31 17:48:47.000000 nopaths-6/nopaths/decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-31 18:53:59.000000 nopaths-6/nopaths/default.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      299 2023-05-31 20:02:22.000000 nopaths-6/nopaths/defines.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1322 2023-05-31 19:50:08.000000 nopaths-6/nopaths/encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      348 2023-05-31 19:52:08.000000 nopaths-6/nopaths/errored.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1968 2023-05-31 19:51:30.000000 nopaths-6/nopaths/handler.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      939 2023-05-31 18:49:17.000000 nopaths-6/nopaths/listens.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      441 2023-05-31 18:41:00.000000 nopaths-6/nopaths/logging.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      940 2023-05-31 18:47:45.000000 nopaths-6/nopaths/message.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 02:16:28.224628 nopaths-6/nopaths/modules/
+-rw-r--r--   0 nop       (1000) nop       (1000)     1786 2023-05-31 19:59:21.000000 nopaths-6/nopaths/modules/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      576 2023-05-31 23:58:48.000000 nopaths-6/nopaths/modules/cfg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      211 2023-05-31 17:40:41.000000 nopaths-6/nopaths/modules/cmd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      704 2023-05-31 23:52:18.000000 nopaths-6/nopaths/modules/err.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      418 2023-05-31 18:50:47.000000 nopaths-6/nopaths/modules/flt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      964 2023-05-31 19:54:01.000000 nopaths-6/nopaths/modules/fnd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    20719 2023-06-01 02:08:00.000000 nopaths-6/nopaths/modules/irc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      705 2023-05-31 19:44:53.000000 nopaths-6/nopaths/modules/log.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      176 2023-05-31 17:36:44.000000 nopaths-6/nopaths/modules/mod.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     7710 2023-05-31 23:56:18.000000 nopaths-6/nopaths/modules/rss.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      346 2023-05-31 17:33:36.000000 nopaths-6/nopaths/modules/sts.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      939 2023-05-31 19:43:02.000000 nopaths-6/nopaths/modules/tdo.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      987 2023-05-31 19:45:11.000000 nopaths-6/nopaths/modules/thr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      218 2023-05-31 17:35:13.000000 nopaths-6/nopaths/modules/upt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      173 2023-05-31 17:38:42.000000 nopaths-6/nopaths/modules/ver.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2011 2023-05-31 23:55:17.000000 nopaths-6/nopaths/objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2133 2023-05-31 20:04:26.000000 nopaths-6/nopaths/objfunc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1810 2023-05-31 20:05:12.000000 nopaths-6/nopaths/parsers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4719 2023-05-31 19:51:41.000000 nopaths-6/nopaths/persist.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      355 2023-05-31 18:48:57.000000 nopaths-6/nopaths/repeats.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2684 2023-06-01 02:16:10.000000 nopaths-6/nopaths/runtime.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      894 2023-05-31 18:43:38.000000 nopaths-6/nopaths/threads.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2933 2023-05-31 23:54:10.000000 nopaths-6/nopaths/utility.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 02:16:28.224628 nopaths-6/nopaths.egg-info/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4831 2023-06-01 02:16:28.000000 nopaths-6/nopaths.egg-info/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     1121 2023-06-01 02:16:28.000000 nopaths-6/nopaths.egg-info/SOURCES.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-01 02:16:28.000000 nopaths-6/nopaths.egg-info/dependency_links.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-06-01 02:16:28.000000 nopaths-6/nopaths.egg-info/top_level.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-01 02:16:28.000000 nopaths-6/nopaths.egg-info/zip-safe
+-rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-06-01 02:16:28.224628 nopaths-6/setup.cfg
+-rw-r--r--   0 nop       (1000) nop       (1000)      852 2023-06-01 02:15:59.000000 nopaths-6/setup.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 02:16:28.224628 nopaths-6/test/
+-rw-r--r--   0 nop       (1000) nop       (1000)      718 2023-06-01 00:04:43.000000 nopaths-6/test/test_composite.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      553 2023-06-01 00:10:34.000000 nopaths-6/test/test_decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      448 2023-06-01 00:12:25.000000 nopaths-6/test/test_encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      969 2023-06-01 00:02:56.000000 nopaths-6/test/test_inherit.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4657 2023-06-01 00:08:52.000000 nopaths-6/test/test_objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      687 2023-05-31 23:51:14.000000 nopaths-6/test/test_recursive.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1159 2023-06-01 00:01:11.000000 nopaths-6/test/test_storage.py
```

### Comparing `nopaths-5/PKG-INFO` & `nopaths-6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 5
+Version: 6
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -58,15 +58,15 @@
         
         **INSTALL**
         
         
         ::
         
         
-            install from pypi::
+            install from pypi
         
                 $ sudo python3 -m pip install nopaths
         
         
         **USAGE**
         
         
@@ -101,26 +101,26 @@
         
         **CONFIGURATION**
         
         
         ::
         
         
-            *irc*
+            irc
         
                 $ nopaths cfg server=<server>
                 $ nopaths cfg channel=<channel>
                 $ nopaths cfg nick=<nick>
         
-            *sasl*
+            sasl
         
                 $ nopaths pwd <nsnick> <nspass>
                 $ nopaths cfg password=<frompwd>
         
-            *rss*
+            rss
          
                 $ nopaths rss <url>
                 $ nopaths dpl <str_in_url> <i1,i2>
                 $ nopaths rem <str_in_url>
                 $ nopaths nme <str_in_url> <name>
```

### Comparing `nopaths-5/README.rst` & `nopaths-6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 **INSTALL**
 
 
 ::
 
 
-    install from pypi::
+    install from pypi
 
         $ sudo python3 -m pip install nopaths
 
 
 **USAGE**
 
 
@@ -93,26 +93,26 @@
 
 **CONFIGURATION**
 
 
 ::
 
 
-    *irc*
+    irc
 
         $ nopaths cfg server=<server>
         $ nopaths cfg channel=<channel>
         $ nopaths cfg nick=<nick>
 
-    *sasl*
+    sasl
 
         $ nopaths pwd <nsnick> <nspass>
         $ nopaths cfg password=<frompwd>
 
-    *rss*
+    rss
  
         $ nopaths rss <url>
         $ nopaths dpl <str_in_url> <i1,i2>
         $ nopaths rem <str_in_url>
         $ nopaths nme <str_in_url> <name>
```

### Comparing `nopaths-5/nopaths/__init__.py` & `nopaths-6/nopaths/__init__.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/__main__.py` & `nopaths-6/nopaths/__main__.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/clients.py` & `nopaths-6/nopaths/clients.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/clocked.py` & `nopaths-6/nopaths/clocked.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/command.py` & `nopaths-6/nopaths/command.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/decoder.py` & `nopaths-6/nopaths/decoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/encoder.py` & `nopaths-6/nopaths/encoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/handler.py` & `nopaths-6/nopaths/handler.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/listens.py` & `nopaths-6/nopaths/listens.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/message.py` & `nopaths-6/nopaths/message.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/__init__.py` & `nopaths-6/nopaths/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/cfg.py` & `nopaths-6/nopaths/modules/cfg.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/err.py` & `nopaths-6/nopaths/modules/err.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/fnd.py` & `nopaths-6/nopaths/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/irc.py` & `nopaths-6/nopaths/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,15 @@
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
             self.state.errors = []
             self.joined.set()
         elif cmd == '433':
-            self.state.errors.append(txt)
+            self.state.errors = txt
             nck = self.cfg.nick + '_' + str(random.randint(1, 10))
             self.command('NICK', nck)
         return evt
 
     def fileno(self):
         return self.sock.fileno()
 
@@ -475,23 +475,30 @@
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
             except (
+                    OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 Errors.errors.append(ex)
-                return self.event(str(ex))
-        return self.event(self.buffer.pop(0))
+                self.stop()
+                Logging.debug("handler stopped")
+                #return self.event(str(ex))
+        try:
+            txt = self.buffer.pop(0)
+        except IndexError:
+            txt = ""
+        return self.event(txt)
 
     def privmsg(self, event):
         if event.txt:
             if event.txt[0] in [self.cfg.control, '!']:
                 event.txt = event.txt[1:]
             elif event.txt.startswith('%s:' % self.cfg.nick):
                 event.txt = event.txt[len(self.cfg.nick)+1:]
@@ -519,14 +526,15 @@
         txt = txt[:512]
         txt += '\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
+                    OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 Errors.errors.append(ex)
                 self.stop()
```

### Comparing `nopaths-5/nopaths/modules/log.py` & `nopaths-6/nopaths/modules/log.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/rss.py` & `nopaths-6/nopaths/modules/rss.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/tdo.py` & `nopaths-6/nopaths/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/modules/thr.py` & `nopaths-6/nopaths/modules/thr.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/objects.py` & `nopaths-6/nopaths/objects.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/objfunc.py` & `nopaths-6/nopaths/objfunc.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/parsers.py` & `nopaths-6/nopaths/parsers.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/persist.py` & `nopaths-6/nopaths/persist.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/runtime.py` & `nopaths-6/nopaths/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 Cfg.debug = False
 Cfg.mod = "cmd,err,flt,mod,sts,thr,upt,ver"
 Cfg.name = "nopaths"
 Cfg.skip = "PING,PONG,PRIVMSG"
 Cfg.threaded = False
-Cfg.version = "4"
+Cfg.version = "6"
 
 
 # FUNCTIONS
 
 
 def banner():
     Logging.debug(f"{Cfg.name.upper()} started at {DATE}")
```

### Comparing `nopaths-5/nopaths/threads.py` & `nopaths-6/nopaths/threads.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths/utility.py` & `nopaths-6/nopaths/utility.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/nopaths.egg-info/PKG-INFO` & `nopaths-6/nopaths.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 5
+Version: 6
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -58,15 +58,15 @@
         
         **INSTALL**
         
         
         ::
         
         
-            install from pypi::
+            install from pypi
         
                 $ sudo python3 -m pip install nopaths
         
         
         **USAGE**
         
         
@@ -101,26 +101,26 @@
         
         **CONFIGURATION**
         
         
         ::
         
         
-            *irc*
+            irc
         
                 $ nopaths cfg server=<server>
                 $ nopaths cfg channel=<channel>
                 $ nopaths cfg nick=<nick>
         
-            *sasl*
+            sasl
         
                 $ nopaths pwd <nsnick> <nspass>
                 $ nopaths cfg password=<frompwd>
         
-            *rss*
+            rss
          
                 $ nopaths rss <url>
                 $ nopaths dpl <str_in_url> <i1,i2>
                 $ nopaths rem <str_in_url>
                 $ nopaths nme <str_in_url> <name>
```

### Comparing `nopaths-5/nopaths.egg-info/SOURCES.txt` & `nopaths-6/nopaths.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nopaths-5/setup.py` & `nopaths-6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="nopaths",
-    version="5",
+    version="6",
     author="No Paths <nopaths@proton.me>",
     author_email="nopaths@proton.me",
     url="http://github.com/nopaths/nopaths",
     zip_safe=True,
     description="there are no paths",
     long_description=read(),
     long_description_content_type="text/x-rst",
```

### Comparing `nopaths-5/test/test_composite.py` & `nopaths-6/test/test_composite.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/test/test_decoder.py` & `nopaths-6/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/test/test_inherit.py` & `nopaths-6/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/test/test_objects.py` & `nopaths-6/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/test/test_recursive.py` & `nopaths-6/test/test_recursive.py`

 * *Files identical despite different names*

### Comparing `nopaths-5/test/test_storage.py` & `nopaths-6/test/test_storage.py`

 * *Files identical despite different names*

