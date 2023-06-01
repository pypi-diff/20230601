# Comparing `tmp/nopaths-4.tar.gz` & `tmp/nopaths-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopaths-4.tar", last modified: Wed May 31 09:18:13 2023, max compression
+gzip compressed data, was "nopaths-5.tar", last modified: Thu Jun  1 00:14:07 2023, max compression
```

## Comparing `nopaths-4.tar` & `nopaths-5.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/
--rw-r--r--   0 nop       (1000) nop       (1000)     4524 2023-05-31 09:18:13.138167 nopaths-4/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     2890 2023-05-30 21:25:56.000000 nopaths-4/README.rst
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.134167 nopaths-4/nopaths/
--rw-r--r--   0 nop       (1000) nop       (1000)     1253 2023-05-30 22:47:54.000000 nopaths-4/nopaths/__init__.py
--rwxr-xr-x   0 nop       (1000) nop       (1000)     2205 2023-05-30 20:37:42.000000 nopaths-4/nopaths/__main__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-29 13:03:22.000000 nopaths-4/nopaths/clients.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-29 13:03:22.000000 nopaths-4/nopaths/clocked.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2484 2023-05-31 09:08:04.000000 nopaths-4/nopaths/command.py
--rw-r--r--   0 nop       (1000) nop       (1000)      127 2023-05-29 13:34:01.000000 nopaths-4/nopaths/configs.py
--rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-29 13:03:22.000000 nopaths-4/nopaths/decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-29 13:03:22.000000 nopaths-4/nopaths/default.py
--rw-r--r--   0 nop       (1000) nop       (1000)      226 2023-05-30 08:05:54.000000 nopaths-4/nopaths/defines.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1156 2023-05-30 20:10:02.000000 nopaths-4/nopaths/encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      311 2023-05-30 08:03:46.000000 nopaths-4/nopaths/errored.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-29 13:03:22.000000 nopaths-4/nopaths/handler.py
--rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-29 13:03:22.000000 nopaths-4/nopaths/listens.py
--rw-r--r--   0 nop       (1000) nop       (1000)      410 2023-05-30 13:33:23.000000 nopaths-4/nopaths/logging.py
--rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-29 13:03:22.000000 nopaths-4/nopaths/message.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/nopaths/modules/
--rw-r--r--   0 nop       (1000) nop       (1000)     1746 2023-05-30 22:54:09.000000 nopaths-4/nopaths/modules/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      537 2023-05-30 17:33:08.000000 nopaths-4/nopaths/modules/cfg.py
--rw-r--r--   0 nop       (1000) nop       (1000)      195 2023-05-30 18:18:56.000000 nopaths-4/nopaths/modules/cmd.py
--rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/err.py
--rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/flt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/fnd.py
--rw-r--r--   0 nop       (1000) nop       (1000)    19811 2023-05-30 11:53:49.000000 nopaths-4/nopaths/modules/irc.py
--rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/log.py
--rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/mod.py
--rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/rss.py
--rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/sts.py
--rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/tdo.py
--rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/thr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/upt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-29 13:03:28.000000 nopaths-4/nopaths/modules/ver.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1638 2023-05-30 19:25:22.000000 nopaths-4/nopaths/objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2082 2023-05-30 19:02:10.000000 nopaths-4/nopaths/objfunc.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-29 13:03:22.000000 nopaths-4/nopaths/parsers.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4149 2023-05-30 19:27:37.000000 nopaths-4/nopaths/persist.py
--rw-r--r--   0 nop       (1000) nop       (1000)      325 2023-05-29 13:03:22.000000 nopaths-4/nopaths/repeats.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2439 2023-05-30 13:31:53.000000 nopaths-4/nopaths/runtime.py
--rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-29 13:03:22.000000 nopaths-4/nopaths/threads.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2891 2023-05-29 13:03:22.000000 nopaths-4/nopaths/utility.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/nopaths.egg-info/
--rw-r--r--   0 nop       (1000) nop       (1000)     4524 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     1086 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/SOURCES.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/dependency_links.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/top_level.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-31 09:18:13.000000 nopaths-4/nopaths.egg-info/zip-safe
--rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-31 09:18:13.138167 nopaths-4/setup.cfg
--rw-r--r--   0 nop       (1000) nop       (1000)      787 2023-05-30 21:34:37.000000 nopaths-4/setup.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-31 09:18:13.138167 nopaths-4/test/
--rw-r--r--   0 nop       (1000) nop       (1000)      661 2023-05-31 09:17:18.000000 nopaths-4/test/test_composite.py
--rw-r--r--   0 nop       (1000) nop       (1000)      483 2023-05-29 12:59:16.000000 nopaths-4/test/test_decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-29 12:59:16.000000 nopaths-4/test/test_encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      887 2023-05-29 12:59:16.000000 nopaths-4/test/test_inherit.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4580 2023-05-29 12:59:16.000000 nopaths-4/test/test_objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1051 2023-05-29 12:59:16.000000 nopaths-4/test/test_storage.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.096813 nopaths-5/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4839 2023-06-01 00:14:07.096813 nopaths-5/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     3053 2023-05-31 23:12:25.000000 nopaths-5/README.rst
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.088813 nopaths-5/bin/
+-rwxr-xr-x   0 nop       (1000) nop       (1000)       24 2023-05-31 22:10:03.000000 nopaths-5/bin/nopaths
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/nopaths/
+-rw-r--r--   0 nop       (1000) nop       (1000)     1350 2023-05-31 22:58:00.000000 nopaths-5/nopaths/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2284 2023-06-01 00:10:58.000000 nopaths-5/nopaths/__main__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      568 2023-05-31 18:48:29.000000 nopaths-5/nopaths/clients.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1086 2023-05-31 18:48:44.000000 nopaths-5/nopaths/clocked.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2603 2023-05-31 19:48:57.000000 nopaths-5/nopaths/command.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      159 2023-05-31 17:48:19.000000 nopaths-5/nopaths/configs.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      796 2023-05-31 17:48:47.000000 nopaths-5/nopaths/decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-31 18:53:59.000000 nopaths-5/nopaths/default.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      299 2023-05-31 20:02:22.000000 nopaths-5/nopaths/defines.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1322 2023-05-31 19:50:08.000000 nopaths-5/nopaths/encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      348 2023-05-31 19:52:08.000000 nopaths-5/nopaths/errored.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1968 2023-05-31 19:51:30.000000 nopaths-5/nopaths/handler.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      939 2023-05-31 18:49:17.000000 nopaths-5/nopaths/listens.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      441 2023-05-31 18:41:00.000000 nopaths-5/nopaths/logging.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      940 2023-05-31 18:47:45.000000 nopaths-5/nopaths/message.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/nopaths/modules/
+-rw-r--r--   0 nop       (1000) nop       (1000)     1786 2023-05-31 19:59:21.000000 nopaths-5/nopaths/modules/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      576 2023-05-31 23:58:48.000000 nopaths-5/nopaths/modules/cfg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      211 2023-05-31 17:40:41.000000 nopaths-5/nopaths/modules/cmd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      704 2023-05-31 23:52:18.000000 nopaths-5/nopaths/modules/err.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      418 2023-05-31 18:50:47.000000 nopaths-5/nopaths/modules/flt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      964 2023-05-31 19:54:01.000000 nopaths-5/nopaths/modules/fnd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    20506 2023-05-31 23:56:50.000000 nopaths-5/nopaths/modules/irc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      705 2023-05-31 19:44:53.000000 nopaths-5/nopaths/modules/log.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      176 2023-05-31 17:36:44.000000 nopaths-5/nopaths/modules/mod.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     7710 2023-05-31 23:56:18.000000 nopaths-5/nopaths/modules/rss.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      346 2023-05-31 17:33:36.000000 nopaths-5/nopaths/modules/sts.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      939 2023-05-31 19:43:02.000000 nopaths-5/nopaths/modules/tdo.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      987 2023-05-31 19:45:11.000000 nopaths-5/nopaths/modules/thr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      218 2023-05-31 17:35:13.000000 nopaths-5/nopaths/modules/upt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      173 2023-05-31 17:38:42.000000 nopaths-5/nopaths/modules/ver.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2011 2023-05-31 23:55:17.000000 nopaths-5/nopaths/objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2133 2023-05-31 20:04:26.000000 nopaths-5/nopaths/objfunc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1810 2023-05-31 20:05:12.000000 nopaths-5/nopaths/parsers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4719 2023-05-31 19:51:41.000000 nopaths-5/nopaths/persist.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      355 2023-05-31 18:48:57.000000 nopaths-5/nopaths/repeats.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2684 2023-05-31 19:51:04.000000 nopaths-5/nopaths/runtime.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      894 2023-05-31 18:43:38.000000 nopaths-5/nopaths/threads.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2933 2023-05-31 23:54:10.000000 nopaths-5/nopaths/utility.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/nopaths.egg-info/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4839 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     1121 2023-06-01 00:14:07.000000 nopaths-5/nopaths.egg-info/SOURCES.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/dependency_links.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/top_level.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-06-01 00:14:06.000000 nopaths-5/nopaths.egg-info/zip-safe
+-rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-06-01 00:14:07.096813 nopaths-5/setup.cfg
+-rw-r--r--   0 nop       (1000) nop       (1000)      852 2023-05-31 23:45:37.000000 nopaths-5/setup.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-06-01 00:14:07.092813 nopaths-5/test/
+-rw-r--r--   0 nop       (1000) nop       (1000)      718 2023-06-01 00:04:43.000000 nopaths-5/test/test_composite.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      553 2023-06-01 00:10:34.000000 nopaths-5/test/test_decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      448 2023-06-01 00:12:25.000000 nopaths-5/test/test_encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      969 2023-06-01 00:02:56.000000 nopaths-5/test/test_inherit.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4657 2023-06-01 00:08:52.000000 nopaths-5/test/test_objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      687 2023-05-31 23:51:14.000000 nopaths-5/test/test_recursive.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1159 2023-06-01 00:01:11.000000 nopaths-5/test/test_storage.py
```

### Comparing `nopaths-4/PKG-INFO` & `nopaths-5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,124 +1,139 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 4
+Version: 5
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
         ::
         
-            nopaths - there are no paths
+        
+            NOPATHS - there are no paths
+        
         
         **SYNOPSIS**
         
         ::
         
+        
             nopaths <cmd> [key=val] [key==val]
-            nopaths [-c] [-d] [-v]
+            nopaths [-a] [-c] [-d] [-t] [-v]
+        
         
         **DESCRIPTION**
         
-        ``nopaths`` is a python3 bot, it connects to irc and provides a select sets of
-        commands. It doesn't use os.popen, does no external imports, can be run in client
-        or daemon mode and has batteries included. 
-        
-        ``nopaths`` is intended to be programmable, it provides object persistence, an
-        event handler and some basic code to load modules that can provide additional
-        functionality.
-        
-        ``nopaths`` uses object programming, programming where the methods are seperated
-        out into functions that use the object as the first argument of that funcion.
-        This gives base class definitions a clean namespace to inherit from and to load
-        json data into the object's __dict__. A clean namespace prevents a json loaded
-        attribute to overwrite any methods.
-        
-        ``nopaths`` stores it's data on disk where objects are time versioned and the
-        last version saved on disk is served to the user layer. Files are JSON dumps
-        and paths carry the type in the path name what makes reconstruction from
-        filename easier then reading type from the object.
         
-        ``nopaths`` has some functionality builtin, it can take notes, add todo, maintain a
-        shopping list and display rss feeds. 
+        ::
         
         
-        **INSTALL**
+            NOPATHS is a python3 bot, it connects to irc and provides a select sets of
+            commands. It doesn't use os.popen, does no external imports, can be run in client
+            or daemon mode and has batteries included. 
+        
+            NOPATHS is intended to be programmable, it provides object persistence, an
+            event handler and some basic code to load modules that can provide additional
+            functionality.
+        
+            NOPATHS uses object programming, programming where the methods are seperated
+            out into functions that use the object as the first argument of that funcion.
+            This gives base class definitions a clean namespace to inherit from and to load
+            json data into the object's __dict__. A clean namespace prevents a json loaded
+            attribute to overwrite any methods.
+        
+            NOPATHS stores it's data on disk where objects are time versioned and the
+            last version saved on disk is served to the user layer. Files are JSON dumps
+            and paths carry the type in the path name what makes reconstruction from
+            filename easier then reading type from the object.
         
-        install from pypi::
+            NOPATHS has some functionality builtin, it can take notes, add todo, maintain a
+            shopping list and display rss feeds. 
         
-            $ sudo python3 -m pip install nopaths
+            NOPATHS has its roots in "no other options available" e.g. no choices left.
         
-        or download the tarball from https://github.com/nopaths/nopaths/releases/
+            NOPATHS is placed in the Public Domain.
         
-        **USAGE**
         
-        use an alias for easier typing::
+        **INSTALL**
         
-            $ alias nopaths="python3 -m nopaths"
         
-        list of commands::
+        ::
         
-            $ nopaths cmd
-            cmd,err,flt,sts,thr,upt
         
-        start a console::
+            install from pypi::
         
-            $ nopaths -c
-            >
+                $ sudo python3 -m pip install nopaths
         
-        start additional modules::
         
-            $ nopaths mod=<mod1,mod2> -c
-            >
+        **USAGE**
         
-        list of modules::
         
-            $ nopaths mod
-            cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
+        ::
         
-        start as daemon::
         
-            $ nopaths mod=cmd,irc,rss -d
-            $ 
+            list of commands
         
-        **CONFIGURATION**
+                $ nopaths cmd
+                cmd,err,flt,sts,thr,upt
         
-        *irc*
+            start a console
         
+                $ nopaths -c
+                >
         
-        ::
+            start additional modules
         
-            $ nopaths cfg server=<server>
-            $ nopaths cfg channel=<channel>
-            $ nopaths cfg nick=<nick>
+                $ nopaths mod=<mod1,mod2> -c
+                >
         
-        *sasl*
+            list of modules
         
-        ::
+                $ nopaths mod
+                cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
+        
+            start as daemon
         
-            $ nopaths pwd <nsnick> <nspass>
-            $ nopaths cfg password=<frompwd>
+                $ nopaths mod=cmd,irc,rss -d
+                $ 
+        
+        
+        **CONFIGURATION**
         
-        *rss*
         
         ::
         
-            $ nopaths rss <url>
-            $ nopaths dpl <str_in_url> <i1,i2>
-            $ nopaths rem <str_in_url>
-            $ nopaths nme <str_in_url> <name>
+        
+            *irc*
+        
+                $ nopaths cfg server=<server>
+                $ nopaths cfg channel=<channel>
+                $ nopaths cfg nick=<nick>
+        
+            *sasl*
+        
+                $ nopaths pwd <nsnick> <nspass>
+                $ nopaths cfg password=<frompwd>
+        
+            *rss*
+         
+                $ nopaths rss <url>
+                $ nopaths dpl <str_in_url> <i1,i2>
+                $ nopaths rem <str_in_url>
+                $ nopaths nme <str_in_url> <name>
         
         
         **COMMANDS**
         
+        
         ::
         
+        
             cmd - commands
             cfg - irc configuration
             dlt - remove a user
             dpl - sets display items
             ftc - runs a fetching batch
             fnd - find objects 
             flt - instances registered
@@ -135,24 +150,28 @@
             slg - slogan
             thr - show the running threads
             tpc - genocide stats into topic
         
         
         **AUTHOR**
         
+        
         ::
         
+        
             No Paths <nopaths@proton.me>
         
         
         **COPYRIGHT**
         
+        
         ::
         
-            nopaths is placed in the Public Domain.
+        
+            NOPATHS is placed in the Public Domain.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
```

### Comparing `nopaths-4/nopaths/__init__.py` & `nopaths-5/nopaths/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is placed in the Public Domain
+# pylama: ignore=E402
 
-"""
-there are no paths
+"""there are no paths
 
 
 NOPATHS is a python3 bot, it connects to irc and provides a select sets of
-commands. It doesn't use os.popen, does no external imports, can be run in client
-or daemon mode and has batteries included. 
+commands. It doesn't use os.popen, does no external imports, can be run in
+client or daemon mode and has batteries included.
 
 MOPATHS is intended to be programmable, it provides object persistence, an
 event handler and some basic code to load modules that can provide additional
 functionality.
 
 NOPATHS uses object programming, programming where the methods are seperated
 out into functions that use the object as the first argument of that funcion.
@@ -20,13 +20,16 @@
 
 NOPATHS stores it's data on disk where objects are time versioned and the
 last version saved on disk is served to the user layer. Files are JSON dumps
 and paths carry the type in the path name what makes reconstruction from
 filename easier then reading type from the object.
 
 NOPATHS has some functionality builtin, it can take notes, add todo, maintain a
-shopping list and display rss feeds. 
+shopping list and display rss feeds.
+
+
+NOPATHS has its roots in "no other options available" e.g. no choices left.
 
 """
 
 __author__ = "No Paths <nopaths@proton.me>"
-__version__ = "4"
+__version__ = "5"
```

### Comparing `nopaths-4/nopaths/__main__.py` & `nopaths-5/nopaths/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0401,W0212,W0611
+# pylint: disable=E0012,C0115,C0116,C0413,E0401,W0212,W0611,W1514,R1732
+# flake8: noqa: E402
+# pylama: ignore=W0611,E402
 
 
 "there are no paths"
 
 
 import os
 import readline
@@ -20,17 +22,17 @@
 from nopaths.logging import Logging
 from nopaths.persist import Persist
 from nopaths.runtime import Cfg, banner, command, parse_cli
 from nopaths.runtime import scanstr, waiter
 
 
 import nopaths.modules
+Commands.modules = nopaths.modules
 
 
-Commands.modules = nopaths.modules
 Persist.workdir = os.path.expanduser(f"~/.{Cfg.name}")
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
```

### Comparing `nopaths-4/nopaths/clients.py` & `nopaths-5/nopaths/clients.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0115,C0116,W0613
 
 
 from .command import Commands
 from .handler import Handler
 from .listens import Listens
 
 
 def __dir__():
-    return ( 
+    return (
             'Client',
            )
 
 
 class Client(Handler):
 
     def __init__(self):
```

### Comparing `nopaths-4/nopaths/clocked.py` & `nopaths-5/nopaths/clocked.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0115,C0116
 
 
 import threading
 import time
 
 
 from .objects import Object
```

### Comparing `nopaths-4/nopaths/command.py` & `nopaths-5/nopaths/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0115,C0116,W0703
 
 
 import inspect
 import sys
 
 
 from .errored import Errors
 from .logging import Logging
 from .message import Message
 from .objects import Object, copy
-from .persist import last, write
-from .utility import spl
 
 
 def __dir__():
     return (
             'Commands',
            )
 
@@ -47,15 +46,14 @@
 class Commands(Object):
 
     cmds = Object()
     modnames = copy(Object(), MODNAMES)
     modules = None
     ondemand = True
 
- 
     @staticmethod
     def add(cmd, func) -> None:
         setattr(Commands.cmds, cmd, func)
         setattr(Commands.modnames, cmd, func.__module__)
 
     @staticmethod
     def handle(evt) -> Message:
@@ -64,15 +62,19 @@
         if Commands.ondemand and not func:
             modname = getattr(Commands.modnames, evt.cmd, None)
             if modname:
                 if modname in sys.modules:
                     mod = sys.modules[modname]
                 if not mod:
                     Logging.debug(f"load {modname}")
-                    mod = getattr(Commands.modules, modname.split(".")[-1], None)
+                    mod = getattr(
+                                  Commands.modules,
+                                  modname.split(".")[-1],
+                                  None
+                                 )
                 func = getattr(mod, evt.cmd, None)
         if func:
             try:
                 func(evt)
                 evt.show()
             except Exception as ex:
                 Errors.handle(ex)
```

### Comparing `nopaths-4/nopaths/decoder.py` & `nopaths-5/nopaths/decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0115,C0116
 
 
 import json
 
 
 from .objects import Object, copy
```

### Comparing `nopaths-4/nopaths/encoder.py` & `nopaths-5/nopaths/encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # This file is placed in the Public Domain.
-
+# pylint: disable=C0114,C0115,C0116
 
 import json
 
 
-from .objects import Object, items
+from .objects import Object
 
 
 def __dir__():
     return (
             'ObjectEncoder',
             'dump',
             'dumps'
            )
 
 
 class ObjectEncoder(json.JSONEncoder):
 
-
     def default(self, o) -> str:
         if isinstance(o, dict):
             return o.items()
         if isinstance(o, Object):
             return vars(o)
         if isinstance(o, list):
             return iter(o)
-        if isinstance(o,
-                      (type(str), type(True), type(False),
-                       type(int), type(float))
+        if isinstance(
+                      o,
+                      (
+                       type(str),
+                       type(True),
+                       type(False),
+                       type(int),
+                       type(float)
+                      )
                      ):
             return str(o)
         try:
             return json.JSONEncoder.default(self, o)
         except TypeError:
             return str(o)
```

### Comparing `nopaths-4/nopaths/handler.py` & `nopaths-5/nopaths/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This file is placed in the Public Domain.
+# pylint: disable=R,C0114,C0115,C0116,W0613,W0212,W0703
 
 
 import queue
 import ssl
 import threading
 
 
@@ -71,15 +72,15 @@
         launch(self.loop)
 
     def stop(self) -> None:
         self.stopped.set()
         self.queue.put_nowait(None)
 
 
-## HANDLERS
+# HANDLERS
 
 
 def dispatch(func, evt) -> None:
     try:
         func(evt)
     except Exception as ex:
         exc = ex.with_traceback(ex.__traceback__)
```

### Comparing `nopaths-4/nopaths/listens.py` & `nopaths-5/nopaths/listens.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0115,C0116
 
 
 from .objects import Object
 
 
 def __dir__():
     return (
```

### Comparing `nopaths-4/nopaths/message.py` & `nopaths-5/nopaths/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0115,C0116
 
 
 import threading
 
 
 from .default import Default
 from .listens import Listens
 from .parsers import parse as evtparse
-from .utility import spl
 
 
 def __dir__():
     return (
             'Message',
            )
```

### Comparing `nopaths-4/nopaths/modules/__init__.py` & `nopaths-5/nopaths/modules/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # This file is placed in the Public Domain.
+# flake8: noqa: F401
+# pylama:ignore=W0611
+
 
 """there are no paths modules
 
 
 use an alias for easier typing::
 
     $ alias np="python3 -m nopaths"
@@ -26,15 +29,15 @@
 
     $ np mod
     cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
 
 start as daemon::
 
     $ np mod=cmd,irc,rss -d
-    $ 
+    $
 
 *irc*
 
     $ np cfg server=<server>
     $ np cfg channel=<channel>
     $ np cfg nick=<nick>
 
@@ -54,15 +57,15 @@
 **COMMANDS**
 
     cmd - commands
     cfg - irc configuration
     dlt - remove a user
     dpl - sets display items
     ftc - runs a fetching batch
-    fnd - find objects 
+    fnd - find objects
     flt - instances registered
     log - log some text
     mdl - genocide model
     met - add a user
     mre - displays cached output
     nck - changes nick on irc
     now - genocide stats
@@ -99,9 +102,7 @@
             "thr",
             "upt",
             'ver'
            )
 
 
 __all__ = __dir__()
-
-
```

### Comparing `nopaths-4/nopaths/modules/fnd.py` & `nopaths-5/nopaths/modules/fnd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0116
 
 
 import time
 
 
 from ..objects import keys
 from ..objfunc import prt
 from ..persist import Persist
 from ..utility import elapsed, fntime
 
 
-## COMMANDS
-
-
 def fnd(event):
     if not event.args:
-        res = ','.join(sorted([x.split('.')[-1].lower() for x in Persist.files()]))
+        res = sorted([x.split('.')[-1].lower() for x in Persist.files()])
         if res:
-            event.reply(res)
+            event.reply(",".join(res))
         else:
             event.reply('no types yet.')
         return
     otype = event.args[0]
     nmr = 0
     keyz = None
     if event.gets:
```

### Comparing `nopaths-4/nopaths/modules/irc.py` & `nopaths-5/nopaths/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file is placed in the Public Domain.
-# pylint: disable=E1101
+# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
+# flake8:
+# pylama: ignore=C901
 
 
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
-import sys
 import time
 import textwrap
 import threading
 import _thread
 
 
 from ..clients import Client
@@ -40,15 +41,15 @@
 
 
 class NoUser(Exception):
 
     pass
 
 
-## CONFIG
+# CONFIG
 
 
 class Config(Default):
 
     channel = '#%s' % Cfg.name
     control = '!'
     nick = Cfg.name
@@ -79,15 +80,15 @@
         self.users = Config.users
         self.verbose = Config.verbose
 
 
 Persist.add(Config)
 
 
-## OUTPUT
+# OUTPUT
 
 
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
@@ -142,15 +143,18 @@
             wrapper = TextWrap()
             try:
                 txtlist = wrapper.wrap(txt)
             except AttributeError:
                 continue
             if len(txtlist) > 3:
                 self.extend(channel, txtlist)
-                self.dosay(channel, '%s put in cache, use !mre to show more' % len(txtlist))
+                self.dosay(
+                           channel,
+                           'use !mre to show more (+%s)' % len(txtlist)
+                          )
                 continue
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     def size(self, chan):
@@ -164,15 +168,15 @@
         return self
 
     def stop(self):
         self.dostop.set()
         self.oqueue.put_nowait((None, None))
 
 
-## IRC
+# IRC
 
 
 class IRC(Client, Output):
 
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
@@ -227,15 +231,21 @@
     def command(self, cmd, *args):
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw('%s %s' % (cmd.upper(), args[0]))
             elif len(args) == 2:
-                self.raw('%s %s :%s' % (cmd.upper(), args[0], ' '.join(args[1:])))
+                self.raw(
+                         '%s %s :%s' % (
+                                        cmd.upper(),
+                                        args[0],
+                                        ' '.join(args[1:])
+                                       )
+                        )
             elif len(args) >= 3:
                 self.raw(
                          '%s %s %s :%s' % (
                                            cmd.upper(),
                                            args[0],
                                            args[1],
                                            ' '.join(args[2:])
@@ -265,15 +275,14 @@
             os.set_inheritable(self.fileno(), os.O_RDWR)
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.connected.set()
             return True
         return False
 
-
     def direct(self, txt):
         Logging.debug(txt)
         self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
         try:
             self.sock.shutdown(2)
@@ -309,38 +318,42 @@
         txt = txt.replace('  ', ' ')
         self.command('PRIVMSG', channel, txt)
 
     def error(self, event):
         self.state.nrerror += 1
         self.state.errors.append(event.txt)
         Logging.debug(event.txt)
-        #self.stop()
 
     def event(self, txt):
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.command('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
         if cmd == '001':
             self.state.needconnect = False
             if self.cfg.servermodes:
-                self.command('MODE %s %s' % (self.cfg.nick, self.cfg.servermodes))
+                self.command(
+                             'MODE %s %s' % (
+                                             self.cfg.nick,
+                                             self.cfg.servermodes
+                                            )
+                            )
             self.zelf = evt.args[-1]
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
             self.state.errors = []
             self.joined.set()
         elif cmd == '433':
             self.state.errors.append(txt)
-            nck = self.cfg.nick + '_' + str(random.randint(1,10))
+            nck = self.cfg.nick + '_' + str(random.randint(1, 10))
             self.command('NICK', nck)
         return evt
 
     def fileno(self):
         return self.sock.fileno()
 
     def h903(self, event):
@@ -372,19 +385,21 @@
                 break
 
     def logon(self, server, nck):
         self.connected.wait()
         self.authed.wait()
         self.direct('NICK %s' % nck)
         self.direct(
-                 'USER %s %s %s :%s' % (self.cfg.username or Cfg.name,
-                 server,
-                 server,
-                 self.cfg.realname or Cfg.name)
-                )
+                    'USER %s %s %s :%s' % (
+                                           self.cfg.username or Cfg.name,
+                                           server,
+                                           server,
+                                           self.cfg.realname or Cfg.name
+                                          )
+                   )
 
     def kill(self, event):
         pass
 
     def log(self, event):
         pass
 
@@ -467,15 +482,14 @@
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 Errors.errors.append(ex)
-                #self.stop()
                 return self.event(str(ex))
         return self.event(self.buffer.pop(0))
 
     def privmsg(self, event):
         if event.txt:
             if event.txt[0] in [self.cfg.control, '!']:
                 event.txt = event.txt[1:]
@@ -567,15 +581,15 @@
     def stop(self):
         Listens.remove(self)
         Client.stop(self)
         Output.stop(self)
         self.disconnect()
 
 
-## USERS
+# USERS
 
 
 class User(Object):
 
     def __init__(self, val=None):
         Object.__init__(self)
         self.user = ''
@@ -630,26 +644,28 @@
             raise NoUser(origin)
         if permission.upper() not in user.perms:
             user.perms.append(permission.upper())
             write(user)
         return user
 
 
-## COMMANDS
+# COMMANDS
 
 
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
-        event.reply(prt(
+        event.reply(
+                    prt(
                         config,
                         keys(config),
-                        skip='control,password,realname,sleep,username')
+                        skip='control,password,realname,sleep,username'
                        )
+                   )
     else:
         edit(config, event.sets)
         write(config)
         event.reply('ok')
 
 
 def dlt(event):
@@ -676,14 +692,15 @@
         return
     user = User()
     user.user = event.rest
     user.perms = ['USER']
     write(user)
     event.reply('ok')
 
+
 def mre(event):
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = event.bot()
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
```

### Comparing `nopaths-4/nopaths/modules/log.py` & `nopaths-5/nopaths/modules/tdo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 # This file is placed in the Public Domain.
+# pylint: disable=R,C0114,C0115,C0116
 
 
 import time
 
 
 from ..objects import Object
 from ..persist import Persist, write
 from ..utility import elapsed, fntime
 
 
-class Log(Object):
+class Todo(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
-Persist.add(Log)
+Persist.add(Todo)
 
 
-## COMMANDS
+# COMMANDS
 
 
-def log(event):
+def dne(event):
+    if not event.args:
+        return
+    selector = {'txt': event.args[0]}
+    for obj in Persist.find('todo', selector):
+        obj.__deleted__ = True
+        write(obj)
+        event.reply('ok')
+        break
+
+
+def tdo(event):
     if not event.rest:
         nmr = 0
-        for obj in Persist.find('log'):
-            lap = elapsed(time.time() - fntime(obj.__oid__))
+        for obj in Persist.find('todo'):
+            lap = elapsed(time.time()-fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
-            event.reply('no log')
+            event.reply("no todo")
         return
-    obj = Log()
+    obj = Todo()
     obj.txt = event.rest
     write(obj)
     event.reply('ok')
```

### Comparing `nopaths-4/nopaths/modules/rss.py` & `nopaths-5/nopaths/modules/rss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=E1101
+# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
 
 
 import html.parser
 import re
 import threading
 import time
 import urllib
@@ -155,28 +155,27 @@
                 lne = lne.replace('![CDATA[', '')
                 lne = lne.replace(']]', '')
                 lne = lne[1:-1]
         except ValueError:
             lne = None
         return lne
 
-
     @staticmethod
     def parse(txt, item='title,link'):
         res = []
         for line in txt.split('<item>'):
             line = line.strip()
             obj = Object()
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
-## UTILITIES
+# UTILITIES
 
 
 def getfeed(url, item):
     if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
@@ -224,15 +223,15 @@
     return html.unescape(txt)
 
 
 def useragent(txt):
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-## COMMANDS
+# COMMANDS
 
 
 def dpl(event):
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
@@ -281,19 +280,20 @@
     event.reply('ok')
 
 
 def rss(event):
     if not event.rest:
         nrs = 0
         for feed in Persist.find('rss'):
-            event.reply('%s %s %s' % (
-                                   nrs,
-                                   prt(feed),
-                                   elapsed(time.time()-fntime(feed.__oid__))
-                                  )
+            event.reply(
+                        '%s %s %s' % (
+                                      nrs,
+                                      prt(feed),
+                                      elapsed(time.time()-fntime(feed.__oid__))
+                                     )
                        )
             nrs += 1
         if not nrs:
             event.reply('no rss feed found.')
         return
     url = event.args[0]
     if 'http' not in url:
```

### Comparing `nopaths-4/nopaths/modules/thr.py` & `nopaths-5/nopaths/modules/thr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # This file is placed in the Public Domain.
-# pylint: disable=E1101
+# pylint: disable=C0114,C0116,E1101
 
 
 import threading
 import time
 
 
 from ..objects import Object, update
 from ..runtime import STARTTIME
 from ..utility import elapsed
 
 
-## COMMANDS
-
-
 def thr(event):
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
```

### Comparing `nopaths-4/nopaths/objects.py` & `nopaths-5/nopaths/objects.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file is placed in the Public Domain.
+# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
 
 
 import datetime
 import os
 import uuid
 
 
 def __dir__():
     return (
             'Object',
             'copy',
+            'dumprec',
             'ident',
             'items',
             'keys',
             'kind',
             'update',
             'values'
            )
@@ -29,29 +31,40 @@
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
-        return str(self.__dict__)
+        return dumprec(self)
 
 
 def copy(obj, val) -> None:
     if isinstance(val, list):
         update(obj, dict(val))
     elif isinstance(val, zip):
         update(obj, dict(val))
     elif isinstance(val, dict):
         update(obj, val)
     elif isinstance(val, Object):
         update(obj, vars(val))
     return obj
 
 
+def dumprec(obj, ooo="{"):
+    for key, value in items(obj):
+        if issubclass(type(value), Object):
+            ooo += "'%s': %s" % (str(key), dumprec(value, ooo))
+            continue
+        else:
+            ooo += "'%s': '%s'" % (str(key), str(value))
+    ooo += "}"
+    return ooo
+
+
 def ident(obj) -> str:
     return os.path.join(
                         kind(obj),
                         str(uuid.uuid4().hex),
                         os.sep.join(str(datetime.datetime.now()).split())
                        )
```

### Comparing `nopaths-4/nopaths/objfunc.py` & `nopaths-5/nopaths/objfunc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file is placed in the Public Domain.
-
+# pylint: disable=C0114,C0116
+# pylama: ignore=C901
 
 from .objects import Object, copy, items, keys
 
 
 def __dir__():
     return (
             'edit',
```

### Comparing `nopaths-4/nopaths/parsers.py` & `nopaths-5/nopaths/parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # This file is placed in the Public Domain.
+# pylint: disable=R,C0114,C0116
+# pylama: ignore=C901
 
 
 from .default import Default
 from .utility import spl
 
 
 def __dir__():
```

### Comparing `nopaths-4/nopaths/persist.py` & `nopaths-5/nopaths/persist.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # This file is placed in the Public Domain.
+# pylint: disable=R,C0114,C0115,C0116,W0613,E1101
 
 
-import json
 import os
-import pathlib
-import time
 import _thread
 
 
-from .decoder import ObjectDecoder, load
+from .decoder import load
 from .default import Default
 from .encoder import dump
-from .objects import Object, ident, kind, update
+from .objects import Object, ident, items, kind, update
 from .objfunc import search
 from .utility import cdir, fnclass, fntime, strip
 
 
 def __dir__():
     return (
             'Persist',
             'last',
             'read',
-            'write'
+            'write',
+            'writerec'
            )
 
 
 disklock = _thread.allocate_lock()
 
 
 class Persist(Object):
@@ -119,15 +118,15 @@
         delattr(Persist.cls, f"{clz.__module__}.{clz.__name__}")
 
     @staticmethod
     def storedir() -> str:
         return os.path.join(Persist.workdir, "store")
 
 
-## FUNCTIONS
+# FUNCTIONS
 
 
 def last(obj, selector=None) -> None:
     if selector is None:
         selector = {}
     result = sorted(
                     Persist.find(kind(obj), selector),
@@ -136,34 +135,53 @@
     if result:
         inp = result[-1]
         update(obj, inp)
         obj.__oid__ = inp.__oid__
     return obj.__oid__
 
 
-def read(obj, pth) -> None:
+def read(obj, pth) -> str:
     pth = Persist.path(pth)
     with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             data = load(ofile)
             update(obj, data)
     obj.__oid__ = strip(pth)
     return obj.__oid__
 
 
+def readrec(obj, pth=None) -> type:
+    ooo = type(obj)()
+    if pth:
+        read(ooo, pth)
+    else:
+        update(ooo, obj)
+    oooo = type(obj)()
+    for key, value in items(ooo):
+        if issubclass(type(value), Object):
+            setattr(oooo, key, readrec(value))
+            continue
+        else:
+            setattr(oooo, key, value)
+    return oooo
+
+
 def write(obj) -> str:
     try:
         pth = Persist.path(obj.__oid__)
     except TypeError:
         pth = Persist.path(ident(obj))
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
 
-"""
-def recursive(obj):
-    
-    for k, v in items(obj):
-"""
-      
+
+def writerec(obj):
+    ooo = type(obj)()
+    for key, value in items(obj):
+        if issubclass(type(value), Object):
+            setattr(ooo, key, writerec(value))
+        else:
+            setattr(ooo, key, str(value))
+    return write(ooo)
```

### Comparing `nopaths-4/nopaths/runtime.py` & `nopaths-5/nopaths/runtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,82 @@
 # This file is placed in the Pubic Domain.
+# pylint: disable=C0114,C0115,C0116,W0613,W0212
 
 
 import functools
 import io
 import time
 import traceback
 
 
-from .default import Default
-from .objects import Object, kind, update
+from .objects import update
 from .logging import Logging
 from .command import Commands
 from .configs import Cfg
 from .errored import Errors
 from .message import Message
-from .persist import Persist
 from .threads import Thread
-from .utility import fntime, spl
+from .utility import spl
 
 
 def __dir__():
     return (
             'DATE',
             'STARTTIME',
             'Config',
             'Cfg',
             'command',
             'launch',
             'parse_cli',
             'threaded'
-           ) 
+           )
 
 
 DATE = time.ctime(time.time()).replace("  ", " ")
 STARTTIME = time.time()
 
 
 Cfg.debug = False
 Cfg.mod = "cmd,err,flt,mod,sts,thr,upt,ver"
 Cfg.name = "nopaths"
 Cfg.skip = "PING,PONG,PRIVMSG"
 Cfg.threaded = False
 Cfg.version = "4"
 
 
-## FUNCTIONS
+# FUNCTIONS
 
 
 def banner():
     Logging.debug(f"{Cfg.name.upper()} started at {DATE}")
 
 
 def command(cli, txt) -> Message:
     evt = cli.event(txt)
     Commands.handle(evt)
     evt.ready()
     return evt
 
-    
+
 def scanstr(pkg, mods, init=None, doall=False, wait=False) -> None:
     res = []
     if doall:
         mods = ",".join(pkg.__all__)
     for modname in spl(mods):
         mod = getattr(pkg, modname)
         if not mod:
             continue
         Commands.scan(mod)
         if init and "start" in dir(mod):
             mod._thr = launch(mod.start)
         res.append(mod)
     if wait:
-       for module in res:
-           if "_thr" in dir(module):
-               module._thr.join()
+        for module in res:
+            if "_thr" in dir(module):
+                module._thr.join()
     return res
 
 
 def launch(func, *args, **kwargs) -> Thread:
     thrname = kwargs.get('name', '')
     thr = Thread(func, thrname, *args)
     thr.start()
@@ -103,14 +102,20 @@
 
     return threadedfunc
 
 
 def waiter(clear=True):
     got = []
     for ex in Errors.errors:
-        stream = io.StringIO(traceback.print_exception(type(ex), ex, ex.__traceback__))
+        stream = io.StringIO(
+                             traceback.print_exception(
+                                                       type(ex),
+                                                       ex,
+                                                       ex.__traceback__
+                                                      )
+                            )
         for line in stream.readlines():
             Logging.debug(line)
         got.append(ex)
     if clear:
         for exc in got:
             Errors.errors.remove(exc)
```

### Comparing `nopaths-4/nopaths/threads.py` & `nopaths-5/nopaths/threads.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0115
 
 
 import queue
 import threading
 import time
-import types
 
 
 from .utility import name
 
 
 def __dir__():
     return (
             'Thread',
            )
 
- 
+
 class Thread(threading.Thread):
 
     def __init__(self, func, thrname, *args, daemon=True):
         super().__init__(None, self.run, thrname, (), {}, daemon=daemon)
         self._result = None
         self.name = thrname or name(func)
         self.queue = queue.Queue()
```

### Comparing `nopaths-4/nopaths/utility.py` & `nopaths-5/nopaths/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This file is placed in the Public Domain.
+# pylint: disable=E0012,C0114,C0116,C0209
 
 
 import os
 import pathlib
 import time
 import types
```

### Comparing `nopaths-4/nopaths.egg-info/PKG-INFO` & `nopaths-5/nopaths.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,124 +1,139 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 4
+Version: 5
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
         ::
         
-            nopaths - there are no paths
+        
+            NOPATHS - there are no paths
+        
         
         **SYNOPSIS**
         
         ::
         
+        
             nopaths <cmd> [key=val] [key==val]
-            nopaths [-c] [-d] [-v]
+            nopaths [-a] [-c] [-d] [-t] [-v]
+        
         
         **DESCRIPTION**
         
-        ``nopaths`` is a python3 bot, it connects to irc and provides a select sets of
-        commands. It doesn't use os.popen, does no external imports, can be run in client
-        or daemon mode and has batteries included. 
-        
-        ``nopaths`` is intended to be programmable, it provides object persistence, an
-        event handler and some basic code to load modules that can provide additional
-        functionality.
-        
-        ``nopaths`` uses object programming, programming where the methods are seperated
-        out into functions that use the object as the first argument of that funcion.
-        This gives base class definitions a clean namespace to inherit from and to load
-        json data into the object's __dict__. A clean namespace prevents a json loaded
-        attribute to overwrite any methods.
-        
-        ``nopaths`` stores it's data on disk where objects are time versioned and the
-        last version saved on disk is served to the user layer. Files are JSON dumps
-        and paths carry the type in the path name what makes reconstruction from
-        filename easier then reading type from the object.
         
-        ``nopaths`` has some functionality builtin, it can take notes, add todo, maintain a
-        shopping list and display rss feeds. 
+        ::
         
         
-        **INSTALL**
+            NOPATHS is a python3 bot, it connects to irc and provides a select sets of
+            commands. It doesn't use os.popen, does no external imports, can be run in client
+            or daemon mode and has batteries included. 
+        
+            NOPATHS is intended to be programmable, it provides object persistence, an
+            event handler and some basic code to load modules that can provide additional
+            functionality.
+        
+            NOPATHS uses object programming, programming where the methods are seperated
+            out into functions that use the object as the first argument of that funcion.
+            This gives base class definitions a clean namespace to inherit from and to load
+            json data into the object's __dict__. A clean namespace prevents a json loaded
+            attribute to overwrite any methods.
+        
+            NOPATHS stores it's data on disk where objects are time versioned and the
+            last version saved on disk is served to the user layer. Files are JSON dumps
+            and paths carry the type in the path name what makes reconstruction from
+            filename easier then reading type from the object.
         
-        install from pypi::
+            NOPATHS has some functionality builtin, it can take notes, add todo, maintain a
+            shopping list and display rss feeds. 
         
-            $ sudo python3 -m pip install nopaths
+            NOPATHS has its roots in "no other options available" e.g. no choices left.
         
-        or download the tarball from https://github.com/nopaths/nopaths/releases/
+            NOPATHS is placed in the Public Domain.
         
-        **USAGE**
         
-        use an alias for easier typing::
+        **INSTALL**
         
-            $ alias nopaths="python3 -m nopaths"
         
-        list of commands::
+        ::
         
-            $ nopaths cmd
-            cmd,err,flt,sts,thr,upt
         
-        start a console::
+            install from pypi::
         
-            $ nopaths -c
-            >
+                $ sudo python3 -m pip install nopaths
         
-        start additional modules::
         
-            $ nopaths mod=<mod1,mod2> -c
-            >
+        **USAGE**
         
-        list of modules::
         
-            $ nopaths mod
-            cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
+        ::
         
-        start as daemon::
         
-            $ nopaths mod=cmd,irc,rss -d
-            $ 
+            list of commands
         
-        **CONFIGURATION**
+                $ nopaths cmd
+                cmd,err,flt,sts,thr,upt
         
-        *irc*
+            start a console
         
+                $ nopaths -c
+                >
         
-        ::
+            start additional modules
         
-            $ nopaths cfg server=<server>
-            $ nopaths cfg channel=<channel>
-            $ nopaths cfg nick=<nick>
+                $ nopaths mod=<mod1,mod2> -c
+                >
         
-        *sasl*
+            list of modules
         
-        ::
+                $ nopaths mod
+                cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
+        
+            start as daemon
         
-            $ nopaths pwd <nsnick> <nspass>
-            $ nopaths cfg password=<frompwd>
+                $ nopaths mod=cmd,irc,rss -d
+                $ 
+        
+        
+        **CONFIGURATION**
         
-        *rss*
         
         ::
         
-            $ nopaths rss <url>
-            $ nopaths dpl <str_in_url> <i1,i2>
-            $ nopaths rem <str_in_url>
-            $ nopaths nme <str_in_url> <name>
+        
+            *irc*
+        
+                $ nopaths cfg server=<server>
+                $ nopaths cfg channel=<channel>
+                $ nopaths cfg nick=<nick>
+        
+            *sasl*
+        
+                $ nopaths pwd <nsnick> <nspass>
+                $ nopaths cfg password=<frompwd>
+        
+            *rss*
+         
+                $ nopaths rss <url>
+                $ nopaths dpl <str_in_url> <i1,i2>
+                $ nopaths rem <str_in_url>
+                $ nopaths nme <str_in_url> <name>
         
         
         **COMMANDS**
         
+        
         ::
         
+        
             cmd - commands
             cfg - irc configuration
             dlt - remove a user
             dpl - sets display items
             ftc - runs a fetching batch
             fnd - find objects 
             flt - instances registered
@@ -135,24 +150,28 @@
             slg - slogan
             thr - show the running threads
             tpc - genocide stats into topic
         
         
         **AUTHOR**
         
+        
         ::
         
+        
             No Paths <nopaths@proton.me>
         
         
         **COPYRIGHT**
         
+        
         ::
         
-            nopaths is placed in the Public Domain.
+        
+            NOPATHS is placed in the Public Domain.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
```

### Comparing `nopaths-4/nopaths.egg-info/SOURCES.txt` & `nopaths-5/nopaths.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.rst
 setup.py
+bin/nopaths
 nopaths/__init__.py
 nopaths/__main__.py
 nopaths/clients.py
 nopaths/clocked.py
 nopaths/command.py
 nopaths/configs.py
 nopaths/decoder.py
@@ -44,8 +45,9 @@
 nopaths/modules/upt.py
 nopaths/modules/ver.py
 test/test_composite.py
 test/test_decoder.py
 test/test_encoder.py
 test/test_inherit.py
 test/test_objects.py
+test/test_recursive.py
 test/test_storage.py
```

### Comparing `nopaths-4/setup.py` & `nopaths-5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0114,C0116,W1514
 
 
 from setuptools import setup
 
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="nopaths",
-    version="4",
+    version="5",
     author="No Paths <nopaths@proton.me>",
     author_email="nopaths@proton.me",
     url="http://github.com/nopaths/nopaths",
     zip_safe=True,
     description="there are no paths",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
     packages=[
               "nopaths",
               'nopaths.modules'
              ],
+    scripts=["bin/nopaths"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: Public Domain",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
      ],
 )
```

### Comparing `nopaths-4/test/test_composite.py` & `nopaths-5/test/test_composite.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is placed in the Public Domain.
-# pylint: disable=E1101
+# pylint: disable=C0114,C0115,C0116,C0413,E1101,R1732
+# pylama: ignore=W0611,E265,E402
 
 
-import os
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
 
 
@@ -23,11 +23,11 @@
         self.assertEqual(obj.obj.a, "test")
 
     def testcompositeprint(self):
         obj = Object()
         obj.obj = Object()
         obj.obj.a = "test"
         pth = write(obj)
-        oo = Object()
-        read(oo, pth)
-        #self.assertEqual(oo.obj.a, "test")
-        self.assertTrue(oo.obj)
+        ooo = Object()
+        read(ooo, pth)
+        #self.assertEqual(ooo.obj.a, "test")
+        self.assertTrue(ooo.obj)
```

### Comparing `nopaths-4/test/test_inherit.py` & `nopaths-5/test/test_inherit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0103,C0114,C0115,C0413,C0116,R0903
+# pylama: ignore=W0611,E302,E265,E402
 
 
-import os
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
```

### Comparing `nopaths-4/test/test_objects.py` & `nopaths-5/test/test_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is placed in the Public Domain.
-# pylint: disable=E1101
+# pylint: disable=W0012,C0103,C0114,C0115,C0116,C0413,C2801,R0903,R0904,E1101
+# pylama: ignore=W0611,E303,E402
 
 
-import os
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
```

### Comparing `nopaths-4/test/test_storage.py` & `nopaths-5/test/test_storage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0413,C0103,C0114,C0115,C0116,R0903
+# pylama: ignore=W0611,E303,E402
 
 
 import os
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
 
 
-
 from nopaths.objects import Object
 from nopaths.persist import Persist, write
 
 
 import nopaths.persist
 
 
 Persist.workdir = '.test'
 
 
 ATTRS1 = (
           'Persist',
           'last',
           'read',
-          'write'
+          'write',
+          'writerec'
          )
 
 
 class TestStorage(unittest.TestCase):
 
     def test_constructor(self):
         obj = Persist()
```

