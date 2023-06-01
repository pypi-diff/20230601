# Comparing `tmp/fdlogger-23.5.30.tar.gz` & `tmp/fdlogger-23.5.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdlogger-23.5.30.tar", last modified: Tue May 30 16:02:19 2023, max compression
+gzip compressed data, was "fdlogger-23.5.31.tar", last modified: Thu Jun  1 02:58:09 2023, max compression
```

## Comparing `fdlogger-23.5.30.tar` & `fdlogger-23.5.31.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:02:19.332498 fdlogger-23.5.30/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-07-24 04:24:05.000000 fdlogger-23.5.30/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20839 2023-05-30 16:02:19.332498 fdlogger-23.5.30/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20049 2023-05-30 15:47:32.000000 fdlogger-23.5.30/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:02:19.324498 fdlogger-23.5.30/fdlogger/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   105318 2023-05-30 15:44:18.000000 fdlogger-23.5.30/fdlogger/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:02:19.327498 fdlogger-23.5.30/fdlogger/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2972 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/data/arrl_sect.dat
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2023-02-01 18:15:34.000000 fdlogger-23.5.30/fdlogger/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2023-02-01 14:59:00.000000 fdlogger-23.5.30/fdlogger/data/k6gte-fieldday.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   104172 2023-02-02 21:16:39.000000 fdlogger-23.5.30/fdlogger/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30785 2023-02-02 20:14:22.000000 fdlogger-23.5.30/fdlogger/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2023-02-01 18:15:34.000000 fdlogger-23.5.30/fdlogger/data/startup.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:02:19.329498 fdlogger-23.5.30/fdlogger/icon/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/cloud_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/cloud_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/cloud_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/gear16x16.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/k6gte-fdlogger.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2023-02-19 21:29:22.000000 fdlogger-23.5.30/fdlogger/icon/logo.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/radio.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/icon/radio_red.png
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:02:19.331498 fdlogger-23.5.30/fdlogger/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.5.30/fdlogger/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10234 2023-02-02 20:57:22.000000 fdlogger-23.5.30/fdlogger/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2023-02-02 20:57:35.000000 fdlogger-23.5.30/fdlogger/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13592 2023-02-02 20:58:22.000000 fdlogger-23.5.30/fdlogger/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2023-02-03 16:08:03.000000 fdlogger-23.5.30/fdlogger/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4626 2023-02-02 20:59:29.000000 fdlogger-23.5.30/fdlogger/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6707 2023-04-08 23:33:07.000000 fdlogger-23.5.30/fdlogger/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-30 15:44:35.000000 fdlogger-23.5.30/fdlogger/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2023-02-02 20:14:22.000000 fdlogger-23.5.30/fdlogger/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:02:19.325498 fdlogger-23.5.30/fdlogger.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20839 2023-05-30 16:02:19.000000 fdlogger-23.5.30/fdlogger.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1106 2023-05-30 16:02:19.000000 fdlogger-23.5.30/fdlogger.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-30 16:02:19.000000 fdlogger-23.5.30/fdlogger.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-30 16:02:19.000000 fdlogger-23.5.30/fdlogger.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2023-05-30 16:02:19.000000 fdlogger-23.5.30/fdlogger.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-30 16:02:19.000000 fdlogger-23.5.30/fdlogger.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1181 2023-05-30 15:44:49.000000 fdlogger-23.5.30/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-30 16:02:19.332498 fdlogger-23.5.30/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:02:19.331498 fdlogger-23.5.30/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2022-09-14 17:33:52.000000 fdlogger-23.5.30/testing/inject_multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2022-07-24 04:24:05.000000 fdlogger-23.5.30/testing/inject_udp.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 fdlogger-23.5.30/testing/multicast_listener.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-03-01 19:35:42.000000 fdlogger-23.5.30/testing/simulant.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-01 02:58:09.903069 fdlogger-23.5.31/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-07-24 04:24:05.000000 fdlogger-23.5.31/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20911 2023-06-01 02:58:09.903069 fdlogger-23.5.31/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20121 2023-06-01 02:56:25.000000 fdlogger-23.5.31/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-01 02:58:09.878069 fdlogger-23.5.31/fdlogger/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   105318 2023-05-30 15:44:18.000000 fdlogger-23.5.31/fdlogger/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-01 02:58:09.887069 fdlogger-23.5.31/fdlogger/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2972 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/data/arrl_sect.dat
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-06-01 02:37:05.000000 fdlogger-23.5.31/fdlogger/data/cwmacros_fd.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2023-02-01 18:15:34.000000 fdlogger-23.5.31/fdlogger/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2023-06-01 02:37:17.000000 fdlogger-23.5.31/fdlogger/data/fd_preferences.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2023-02-01 14:59:00.000000 fdlogger-23.5.31/fdlogger/data/k6gte-fieldday.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   104172 2023-02-02 21:16:39.000000 fdlogger-23.5.31/fdlogger/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30785 2023-02-02 20:14:22.000000 fdlogger-23.5.31/fdlogger/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2023-02-01 18:15:34.000000 fdlogger-23.5.31/fdlogger/data/startup.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-01 02:58:09.891069 fdlogger-23.5.31/fdlogger/icon/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/cloud_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/cloud_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/cloud_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/gear16x16.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/k6gte-fdlogger.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2023-02-19 21:29:22.000000 fdlogger-23.5.31/fdlogger/icon/logo.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/radio.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/icon/radio_red.png
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-01 02:58:09.897069 fdlogger-23.5.31/fdlogger/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.5.31/fdlogger/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10234 2023-02-02 20:57:22.000000 fdlogger-23.5.31/fdlogger/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2023-02-02 20:57:35.000000 fdlogger-23.5.31/fdlogger/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13592 2023-02-02 20:58:22.000000 fdlogger-23.5.31/fdlogger/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2023-02-03 16:08:03.000000 fdlogger-23.5.31/fdlogger/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4626 2023-02-02 20:59:29.000000 fdlogger-23.5.31/fdlogger/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6707 2023-04-08 23:33:07.000000 fdlogger-23.5.31/fdlogger/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-01 02:49:17.000000 fdlogger-23.5.31/fdlogger/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2023-02-02 20:14:22.000000 fdlogger-23.5.31/fdlogger/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-01 02:58:09.881069 fdlogger-23.5.31/fdlogger.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20911 2023-06-01 02:58:09.000000 fdlogger-23.5.31/fdlogger.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1170 2023-06-01 02:58:09.000000 fdlogger-23.5.31/fdlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-01 02:58:09.000000 fdlogger-23.5.31/fdlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-06-01 02:58:09.000000 fdlogger-23.5.31/fdlogger.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2023-06-01 02:58:09.000000 fdlogger-23.5.31/fdlogger.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-01 02:58:09.000000 fdlogger-23.5.31/fdlogger.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1181 2023-06-01 02:49:18.000000 fdlogger-23.5.31/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-01 02:58:09.903069 fdlogger-23.5.31/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-01 02:58:09.902069 fdlogger-23.5.31/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2022-09-14 17:33:52.000000 fdlogger-23.5.31/testing/inject_multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2022-07-24 04:24:05.000000 fdlogger-23.5.31/testing/inject_udp.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 fdlogger-23.5.31/testing/multicast_listener.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-03-01 19:35:42.000000 fdlogger-23.5.31/testing/simulant.py
```

### Comparing `fdlogger-23.5.30/LICENSE` & `fdlogger-23.5.31/LICENSE`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/PKG-INFO` & `fdlogger-23.5.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 23.5.30
+Version: 23.5.31
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -92,14 +92,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.5.31] Replaced some deleted stuff. Thanks @ATCUSA for finding it!
 - [23.5.30] Changed default multicast address from 224.1.1.1 to 239.1.1.1
 - [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
```

### Comparing `fdlogger-23.5.30/README.md` & `fdlogger-23.5.31/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.5.31] Replaced some deleted stuff. Thanks @ATCUSA for finding it!
 - [23.5.30] Changed default multicast address from 224.1.1.1 to 239.1.1.1
 - [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
```

### Comparing `fdlogger-23.5.30/fdlogger/__main__.py` & `fdlogger-23.5.31/fdlogger/__main__.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/data/JetBrainsMono-Regular.ttf` & `fdlogger-23.5.31/fdlogger/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/data/MASTER.SCP` & `fdlogger-23.5.31/fdlogger/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/data/arrl_sect.dat` & `fdlogger-23.5.31/fdlogger/data/arrl_sect.dat`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/data/dialog.ui` & `fdlogger-23.5.31/fdlogger/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/data/main.ui` & `fdlogger-23.5.31/fdlogger/data/main.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/data/settings.ui` & `fdlogger-23.5.31/fdlogger/data/settings.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/data/startup.ui` & `fdlogger-23.5.31/fdlogger/data/startup.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/cloud_green.png` & `fdlogger-23.5.31/fdlogger/icon/cloud_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/cloud_grey.png` & `fdlogger-23.5.31/fdlogger/icon/cloud_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/gear16x16.png` & `fdlogger-23.5.31/fdlogger/icon/gear16x16.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/k6gte-fdlogger.png` & `fdlogger-23.5.31/fdlogger/icon/k6gte-fdlogger.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/logo.png` & `fdlogger-23.5.31/fdlogger/icon/logo.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/radio.svg` & `fdlogger-23.5.31/fdlogger/icon/radio.svg`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/radio_green.png` & `fdlogger-23.5.31/fdlogger/icon/radio_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/radio_grey.png` & `fdlogger-23.5.31/fdlogger/icon/radio_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/icon/radio_red.png` & `fdlogger-23.5.31/fdlogger/icon/radio_red.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/lib/cat_interface.py` & `fdlogger-23.5.31/fdlogger/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/lib/cwinterface.py` & `fdlogger-23.5.31/fdlogger/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/lib/database.py` & `fdlogger-23.5.31/fdlogger/lib/database.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/lib/lookup.py` & `fdlogger-23.5.31/fdlogger/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/lib/n1mm.py` & `fdlogger-23.5.31/fdlogger/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/lib/settings.py` & `fdlogger-23.5.31/fdlogger/lib/settings.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger/lib/versiontest.py` & `fdlogger-23.5.31/fdlogger/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/fdlogger.egg-info/PKG-INFO` & `fdlogger-23.5.31/fdlogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 23.5.30
+Version: 23.5.31
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -92,14 +92,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.5.31] Replaced some deleted stuff. Thanks @ATCUSA for finding it!
 - [23.5.30] Changed default multicast address from 224.1.1.1 to 239.1.1.1
 - [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
```

### Comparing `fdlogger-23.5.30/fdlogger.egg-info/SOURCES.txt` & `fdlogger-23.5.31/fdlogger.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 fdlogger.egg-info/dependency_links.txt
 fdlogger.egg-info/entry_points.txt
 fdlogger.egg-info/requires.txt
 fdlogger.egg-info/top_level.txt
 fdlogger/data/JetBrainsMono-Regular.ttf
 fdlogger/data/MASTER.SCP
 fdlogger/data/arrl_sect.dat
+fdlogger/data/cwmacros_fd.txt
 fdlogger/data/dialog.ui
+fdlogger/data/fd_preferences.json
 fdlogger/data/k6gte-fieldday.desktop
 fdlogger/data/main.ui
 fdlogger/data/settings.ui
 fdlogger/data/startup.ui
 fdlogger/icon/cloud_green.png
 fdlogger/icon/cloud_grey.png
 fdlogger/icon/cloud_red.png
```

### Comparing `fdlogger-23.5.30/pyproject.toml` & `fdlogger-23.5.31/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdlogger" 
-version = "23.5.30"
+version = "23.5.31"
 description = "ARRL Field Day logger GUI"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `fdlogger-23.5.30/testing/inject_multicast.py` & `fdlogger-23.5.31/testing/inject_multicast.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/testing/inject_udp.py` & `fdlogger-23.5.31/testing/inject_udp.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/testing/multicast_listener.py` & `fdlogger-23.5.31/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.5.30/testing/simulant.py` & `fdlogger-23.5.31/testing/simulant.py`

 * *Files identical despite different names*

