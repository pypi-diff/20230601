# Comparing `tmp/purdy-1.9.0.tar.gz` & `tmp/purdy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purdy-1.9.0.tar", last modified: Tue May 11 19:37:40 2021, max compression
+gzip compressed data, was "purdy-1.9.1.tar", last modified: Sun May 16 16:03:14 2021, max compression
```

## Comparing `purdy-1.9.0.tar` & `purdy-1.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.028066 purdy-1.9.0/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2019-09-22 14:42:38.000000 purdy-1.9.0/LICENSE
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5122 2021-05-11 19:37:40.027366 purdy-1.9.0/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3378 2021-03-21 18:53:09.000000 purdy-1.9.0/README.rst
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.014161 purdy-1.9.0/bin/
--rwxr-xr-x   0 ctrudeau   (501) staff       (20)     1278 2020-05-22 20:43:49.000000 purdy-1.9.0/bin/pat
--rwxr-xr-x   0 ctrudeau   (501) staff       (20)     1365 2020-05-22 20:43:49.000000 purdy-1.9.0/bin/prat
--rwxr-xr-x   0 ctrudeau   (501) staff       (20)     2815 2020-07-15 15:18:31.000000 purdy-1.9.0/bin/purdy
--rwxr-xr-x   0 ctrudeau   (501) staff       (20)     6637 2020-05-11 22:55:48.000000 purdy-1.9.0/bin/subpurdy
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.017289 purdy-1.9.0/purdy/
--rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2021-05-11 19:09:22.000000 purdy-1.9.0/purdy/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    21052 2021-03-21 18:53:09.000000 purdy-1.9.0/purdy/actions.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.020209 purdy-1.9.0/purdy/animation/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-06 18:12:08.000000 purdy-1.9.0/purdy/animation/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     8207 2021-03-21 18:53:09.000000 purdy-1.9.0/purdy/animation/cell.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3923 2021-03-21 18:53:09.000000 purdy-1.9.0/purdy/animation/manager.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    12285 2021-03-21 18:53:09.000000 purdy-1.9.0/purdy/animation/steps.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    13205 2021-03-21 18:53:09.000000 purdy-1.9.0/purdy/builder.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2636 2020-11-01 21:29:41.000000 purdy-1.9.0/purdy/cmd.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.022046 purdy-1.9.0/purdy/colour/
--rw-r--r--   0 ctrudeau   (501) staff       (20)      421 2020-11-01 18:24:19.000000 purdy-1.9.0/purdy/colour/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3191 2020-11-01 22:24:53.000000 purdy-1.9.0/purdy/colour/ansico.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3260 2020-11-01 22:29:12.000000 purdy-1.9.0/purdy/colour/htmlco.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      905 2020-11-01 22:28:53.000000 purdy-1.9.0/purdy/colour/plainco.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6868 2020-11-01 22:28:45.000000 purdy-1.9.0/purdy/colour/rtfco.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5007 2021-03-11 01:00:19.000000 purdy-1.9.0/purdy/colour/urwidco.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    16305 2021-05-11 19:31:15.000000 purdy-1.9.0/purdy/content.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.022406 purdy-1.9.0/purdy/iscreen/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-17 19:35:21.000000 purdy-1.9.0/purdy/iscreen/__init__.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.022897 purdy-1.9.0/purdy/iscreen/exercise/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-22 20:43:49.000000 purdy-1.9.0/purdy/iscreen/exercise/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     4148 2020-05-22 20:43:49.000000 purdy-1.9.0/purdy/iscreen/exercise/iscreen.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.023725 purdy-1.9.0/purdy/iscreen/tui/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-17 19:35:21.000000 purdy-1.9.0/purdy/iscreen/tui/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    12316 2021-03-21 18:53:09.000000 purdy-1.9.0/purdy/iscreen/tui/iscreen.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6205 2021-03-10 23:40:16.000000 purdy-1.9.0/purdy/iscreen/tui/widgets.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.024191 purdy-1.9.0/purdy/iscreen/virtual/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-17 19:35:21.000000 purdy-1.9.0/purdy/iscreen/virtual/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2646 2020-11-01 22:34:37.000000 purdy-1.9.0/purdy/iscreen/virtual/iscreen.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1842 2021-05-11 19:01:40.000000 purdy-1.9.0/purdy/lexers.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     8061 2021-05-11 19:18:18.000000 purdy-1.9.0/purdy/parser.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3908 2020-11-01 19:22:37.000000 purdy-1.9.0/purdy/scribe.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      903 2020-07-15 15:14:08.000000 purdy-1.9.0/purdy/settings.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    17138 2021-05-11 19:34:22.000000 purdy-1.9.0/purdy/ui.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.019000 purdy-1.9.0/purdy.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5122 2021-05-11 19:37:39.000000 purdy-1.9.0/purdy.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1059 2021-05-11 19:37:39.000000 purdy-1.9.0/purdy.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2021-05-11 19:37:39.000000 purdy-1.9.0/purdy.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       61 2021-05-11 19:37:39.000000 purdy-1.9.0/purdy.egg-info/requires.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       12 2021-05-11 19:37:39.000000 purdy-1.9.0/purdy.egg-info/top_level.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2021-05-11 19:37:40.028342 purdy-1.9.0/setup.cfg
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1556 2021-05-11 15:17:37.000000 purdy-1.9.0/setup.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-11 19:37:40.026833 purdy-1.9.0/tests/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-01 17:16:57.000000 purdy-1.9.0/tests/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2651 2021-03-10 21:55:12.000000 purdy-1.9.0/tests/base.py
--rwxr-xr-x   0 ctrudeau   (501) staff       (20)     2135 2021-03-21 18:53:09.000000 purdy-1.9.0/tests/capture_exercise.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1198 2021-03-10 21:55:12.000000 purdy-1.9.0/tests/test_builder.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3700 2020-11-02 14:17:48.000000 purdy-1.9.0/tests/test_cmds.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    13097 2020-07-04 20:14:29.000000 purdy-1.9.0/tests/test_content.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1291 2021-03-21 18:53:09.000000 purdy-1.9.0/tests/test_exercises.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2465 2021-05-11 19:11:32.000000 purdy-1.9.0/tests/test_parser.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3978 2020-11-01 21:32:03.000000 purdy-1.9.0/tests/test_scribe.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.860120 purdy-1.9.1/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2019-09-22 14:42:38.000000 purdy-1.9.1/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5122 2021-05-16 16:03:14.859828 purdy-1.9.1/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3378 2021-03-21 18:53:09.000000 purdy-1.9.1/README.rst
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.846205 purdy-1.9.1/bin/
+-rwxr-xr-x   0 ctrudeau   (501) staff       (20)     1278 2020-05-22 20:43:49.000000 purdy-1.9.1/bin/pat
+-rwxr-xr-x   0 ctrudeau   (501) staff       (20)     1365 2020-05-22 20:43:49.000000 purdy-1.9.1/bin/prat
+-rwxr-xr-x   0 ctrudeau   (501) staff       (20)     2815 2020-07-15 15:18:31.000000 purdy-1.9.1/bin/purdy
+-rwxr-xr-x   0 ctrudeau   (501) staff       (20)     6637 2020-05-11 22:55:48.000000 purdy-1.9.1/bin/subpurdy
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.850079 purdy-1.9.1/purdy/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2021-05-16 15:58:08.000000 purdy-1.9.1/purdy/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    21052 2021-03-21 18:53:09.000000 purdy-1.9.1/purdy/actions.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.852868 purdy-1.9.1/purdy/animation/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-06 18:12:08.000000 purdy-1.9.1/purdy/animation/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     8207 2021-03-21 18:53:09.000000 purdy-1.9.1/purdy/animation/cell.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3923 2021-03-21 18:53:09.000000 purdy-1.9.1/purdy/animation/manager.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    12285 2021-03-21 18:53:09.000000 purdy-1.9.1/purdy/animation/steps.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    13205 2021-03-21 18:53:09.000000 purdy-1.9.1/purdy/builder.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2636 2020-11-01 21:29:41.000000 purdy-1.9.1/purdy/cmd.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.854640 purdy-1.9.1/purdy/colour/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      421 2020-11-01 18:24:19.000000 purdy-1.9.1/purdy/colour/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3191 2020-11-01 22:24:53.000000 purdy-1.9.1/purdy/colour/ansico.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3260 2020-11-01 22:29:12.000000 purdy-1.9.1/purdy/colour/htmlco.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      905 2020-11-01 22:28:53.000000 purdy-1.9.1/purdy/colour/plainco.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     6938 2021-05-16 15:25:00.000000 purdy-1.9.1/purdy/colour/rtfco.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5007 2021-03-11 01:00:19.000000 purdy-1.9.1/purdy/colour/urwidco.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    16305 2021-05-11 19:31:15.000000 purdy-1.9.1/purdy/content.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.854901 purdy-1.9.1/purdy/iscreen/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-17 19:35:21.000000 purdy-1.9.1/purdy/iscreen/__init__.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.855252 purdy-1.9.1/purdy/iscreen/exercise/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-22 20:43:49.000000 purdy-1.9.1/purdy/iscreen/exercise/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     4148 2020-05-22 20:43:49.000000 purdy-1.9.1/purdy/iscreen/exercise/iscreen.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.856172 purdy-1.9.1/purdy/iscreen/tui/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-17 19:35:21.000000 purdy-1.9.1/purdy/iscreen/tui/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    12316 2021-03-21 18:53:09.000000 purdy-1.9.1/purdy/iscreen/tui/iscreen.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     6205 2021-03-10 23:40:16.000000 purdy-1.9.1/purdy/iscreen/tui/widgets.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.856633 purdy-1.9.1/purdy/iscreen/virtual/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-17 19:35:21.000000 purdy-1.9.1/purdy/iscreen/virtual/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2646 2020-11-01 22:34:37.000000 purdy-1.9.1/purdy/iscreen/virtual/iscreen.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2120 2021-05-16 14:58:47.000000 purdy-1.9.1/purdy/lexers.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     8061 2021-05-11 19:18:18.000000 purdy-1.9.1/purdy/parser.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3908 2020-11-01 19:22:37.000000 purdy-1.9.1/purdy/scribe.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      903 2020-07-15 15:14:08.000000 purdy-1.9.1/purdy/settings.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    17138 2021-05-11 19:34:22.000000 purdy-1.9.1/purdy/ui.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.851704 purdy-1.9.1/purdy.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5122 2021-05-16 16:03:14.000000 purdy-1.9.1/purdy.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1059 2021-05-16 16:03:14.000000 purdy-1.9.1/purdy.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2021-05-16 16:03:14.000000 purdy-1.9.1/purdy.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       61 2021-05-16 16:03:14.000000 purdy-1.9.1/purdy.egg-info/requires.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       12 2021-05-16 16:03:14.000000 purdy-1.9.1/purdy.egg-info/top_level.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2021-05-16 16:03:14.860192 purdy-1.9.1/setup.cfg
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1556 2021-05-11 15:17:37.000000 purdy-1.9.1/setup.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2021-05-16 16:03:14.859284 purdy-1.9.1/tests/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2020-05-01 17:16:57.000000 purdy-1.9.1/tests/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2651 2021-03-10 21:55:12.000000 purdy-1.9.1/tests/base.py
+-rwxr-xr-x   0 ctrudeau   (501) staff       (20)     2135 2021-03-21 18:53:09.000000 purdy-1.9.1/tests/capture_exercise.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1198 2021-03-10 21:55:12.000000 purdy-1.9.1/tests/test_builder.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3700 2020-11-02 14:17:48.000000 purdy-1.9.1/tests/test_cmds.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    13097 2020-07-04 20:14:29.000000 purdy-1.9.1/tests/test_content.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1291 2021-03-21 18:53:09.000000 purdy-1.9.1/tests/test_exercises.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2465 2021-05-11 19:11:32.000000 purdy-1.9.1/tests/test_parser.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3978 2020-11-01 21:32:03.000000 purdy-1.9.1/tests/test_scribe.py
```

### Comparing `purdy-1.9.0/LICENSE` & `purdy-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/PKG-INFO` & `purdy-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: purdy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Terminal based code snippet display tool 
 Home-page: https://github.com/cltrudeau/purdy
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
 Description: *****
         Purdy
```

### Comparing `purdy-1.9.0/README.rst` & `purdy-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/bin/pat` & `purdy-1.9.1/bin/pat`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/bin/prat` & `purdy-1.9.1/bin/prat`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/bin/purdy` & `purdy-1.9.1/bin/purdy`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/bin/subpurdy` & `purdy-1.9.1/bin/subpurdy`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/actions.py` & `purdy-1.9.1/purdy/actions.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/animation/cell.py` & `purdy-1.9.1/purdy/animation/cell.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/animation/manager.py` & `purdy-1.9.1/purdy/animation/manager.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/animation/steps.py` & `purdy-1.9.1/purdy/animation/steps.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/builder.py` & `purdy-1.9.1/purdy/builder.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/cmd.py` & `purdy-1.9.1/purdy/cmd.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/colour/ansico.py` & `purdy-1.9.1/purdy/colour/ansico.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/colour/htmlco.py` & `purdy-1.9.1/purdy/colour/htmlco.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/colour/plainco.py` & `purdy-1.9.1/purdy/colour/plainco.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/colour/rtfco.py` & `purdy-1.9.1/purdy/colour/rtfco.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,19 @@
     while index < size:
         num = parts[index]
 
         if num <= 127:
             # regular ascii
             letter = chr(num)
 
-            # RTF uses backslash, so it needs to be escaped
+            # Escape characters that are used by RTF 
             if letter == '\\':
                 output.append('\\\\')
+            elif letter in '{}':
+                output.append('\\' + letter)
             else:
                 output.append(letter)
         elif num <= 256:
             # extended ascii, use hex notation
             output.append(f"\\'{num:2x}" )
         elif num < 55296:
             # 0xD800 (55296) is the the boundary for two-word encoding, less
@@ -88,16 +90,16 @@
     Name.Decorator:     '\\b \\cf8 %s\n\\b0\n', 
     Name.Variable:      '\\cf0 %s\n',
     Name.Constant:      '\\cf0 %s\n',
     Name.Attribute:     '\\cf0 %s\n',
     Name.Tag:           '\\cf0 %s\n',
     Punctuation:        '\\b \\cf5 %s\n\\b0\n', 
     String:             '\\cf9 %s\n', 
-    String.Doc:         '\\i \\cf2 %s\n \\i0', 
-    Number:             '\\b \cf10 %s\n \\b0', 
+    String.Doc:         '\\i \\cf2 %s\n\\i0', 
+    Number:             '\\b \cf10 %s\n\\b0', 
     Generic.Prompt:     '\\cf2 %s\n',
     Generic.Error:      '\\cf11 %s\n',
     Generic.Traceback:  '\\b \cf12 %s\n\\b0\n', 
     Error:              '\\cf11 %s\n',
 }
 
 _xml_palette = dict(_code_palette)
```

### Comparing `purdy-1.9.0/purdy/colour/urwidco.py` & `purdy-1.9.1/purdy/colour/urwidco.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/content.py` & `purdy-1.9.1/purdy/content.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/iscreen/exercise/iscreen.py` & `purdy-1.9.1/purdy/iscreen/exercise/iscreen.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/iscreen/tui/iscreen.py` & `purdy-1.9.1/purdy/iscreen/tui/iscreen.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/iscreen/tui/widgets.py` & `purdy-1.9.1/purdy/iscreen/tui/widgets.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/iscreen/virtual/iscreen.py` & `purdy-1.9.1/purdy/iscreen/virtual/iscreen.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/lexers.py` & `purdy-1.9.1/purdy/lexers.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,22 +49,30 @@
         for match in line_re.finditer(text):
             line = match.group()
             if line.startswith('> '):
                 insertions.append((len(curcode), 
                     [(0, Generic.Prompt, line[:2])]))
 
                 curcode += line[2:]
-            elif line.startswith('... '):
+            elif line.startswith('...'):
+                # node does a nested ... thing depending on depth
+                code = line.lstrip('.')
+                lead = len(line) - len(code)
+
                 insertions.append((len(curcode), 
-                    [(0, Generic.Prompt, line[:4])]))
+                    [(0, Generic.Prompt, line[:lead])]))
 
-                curcode += line[4:]
+                curcode += code
             else:
                 if curcode:
                     yield from do_insertions(insertions, 
                         jslexer.get_tokens_unprocessed(curcode))
 
                     curcode = ''
                     insertions = []
 
                 yield from do_insertions([], 
                     jslexer.get_tokens_unprocessed(line))
+
+        if curcode:
+            yield from do_insertions(insertions, 
+                jslexer.get_tokens_unprocessed(curcode))
```

### Comparing `purdy-1.9.0/purdy/parser.py` & `purdy-1.9.1/purdy/parser.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/scribe.py` & `purdy-1.9.1/purdy/scribe.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/settings.py` & `purdy-1.9.1/purdy/settings.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy/ui.py` & `purdy-1.9.1/purdy/ui.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/purdy.egg-info/PKG-INFO` & `purdy-1.9.1/purdy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: purdy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Terminal based code snippet display tool 
 Home-page: https://github.com/cltrudeau/purdy
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
 Description: *****
         Purdy
```

### Comparing `purdy-1.9.0/purdy.egg-info/SOURCES.txt` & `purdy-1.9.1/purdy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/setup.py` & `purdy-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/base.py` & `purdy-1.9.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/capture_exercise.py` & `purdy-1.9.1/tests/capture_exercise.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/test_builder.py` & `purdy-1.9.1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/test_cmds.py` & `purdy-1.9.1/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/test_content.py` & `purdy-1.9.1/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/test_exercises.py` & `purdy-1.9.1/tests/test_exercises.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/test_parser.py` & `purdy-1.9.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `purdy-1.9.0/tests/test_scribe.py` & `purdy-1.9.1/tests/test_scribe.py`

 * *Files identical despite different names*

