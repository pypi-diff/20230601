# Comparing `tmp/jdFlatpakSnapshot-2.0.tar.gz` & `tmp/jdFlatpakSnapshot-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdFlatpakSnapshot-2.0.tar", last modified: Tue Apr 18 16:24:17 2023, max compression
+gzip compressed data, was "jdFlatpakSnapshot-2.1.tar", last modified: Thu Jun  1 06:20:53 2023, max compression
```

## Comparing `jdFlatpakSnapshot-2.0.tar` & `jdFlatpakSnapshot-2.1.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/
--rw-r--r--   0 root         (0) root         (0)     2879 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35075 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5358 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4277 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/
--rw-r--r--   0 root         (0) root         (0)     1595 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/AboutDialog.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Constants.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Environment.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/FlatpakHandler.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Functions.py
--rw-r--r--   0 root         (0) root         (0)     5509 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ImportExport.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Languages.py
--rw-r--r--   0 root         (0) root         (0)    17027 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/MainWindow.py
--rw-r--r--   0 root         (0) root         (0)     4940 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ProgressDialog.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Settings.py
--rw-r--r--   0 root         (0) root         (0)     3721 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/SettingsDialog.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4013 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/SnapshotCollection.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Types.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/WelcomeDialog.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/
--rw-r--r--   0 root         (0) root         (0)     3101 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/app-icon.svg
--rw-r--r--   0 root         (0) root         (0)     1181 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/default-icon.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/
--rw-r--r--   0 root         (0) root         (0)    27319 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
--rw-r--r--   0 root         (0) root         (0)    27635 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts
--rw-r--r--   0 root         (0) root         (0)    25664 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/AboutDialog.ui
--rw-r--r--   0 root         (0) root         (0)     6240 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/MainWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2265 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/ProgressDialog.ui
--rw-r--r--   0 root         (0) root         (0)     5587 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/SettingsDialog.ui
--rw-r--r--   0 root         (0) root         (0)     4097 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/WelcomeDialog.ui
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5358 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1323 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1413 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35075 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5440 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4277 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Constants.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/FlatpakHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     5509 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ImportExport.py
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Languages.py
+-rw-r--r--   0 root         (0) root         (0)    17027 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ProgressDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/SnapshotCollection.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Types.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/WelcomeDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/icons/
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/icons/app-icon.svg
+-rw-r--r--   0 root         (0) root         (0)     1181 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/icons/default-icon.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/
+-rw-r--r--   0 root         (0) root         (0)    28285 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
+-rw-r--r--   0 root         (0) root         (0)    27965 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts
+-rw-r--r--   0 root         (0) root         (0)    30606 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_ru.ts
+-rw-r--r--   0 root         (0) root         (0)    25978 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts
+-rw-r--r--   0 root         (0) root         (0)    30226 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_uk.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     6240 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/ProgressDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/WelcomeDialog.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5440 2023-06-01 06:20:53.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-06-01 06:20:53.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 06:20:53.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-01 06:20:53.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-01 06:20:53.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 06:20:53.000000 jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-06-01 06:20:01.000000 jdFlatpakSnapshot-2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 06:20:53.134429 jdFlatpakSnapshot-2.1/setup.cfg
```

### Comparing `jdFlatpakSnapshot-2.0/BuildBackend.py` & `jdFlatpakSnapshot-2.1/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/LICENSE` & `jdFlatpakSnapshot-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/PKG-INFO` & `jdFlatpakSnapshot-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jdFlatpakSnapshot
-Version: 2.0
+Version: 2.1
 Summary: A Program to create Snapshots of Flatpak Apps
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdFlatpakSnaphot
 Project-URL: Issues, https://codeberg.org/JakobDev/jdFlatpakSnapshot/issues
+Project-URL: Translate, https://translate.codeberg.org/projects/jdFlatpakSnapshot
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Linux,Flatpak
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `jdFlatpakSnapshot-2.0/README.md` & `jdFlatpakSnapshot-2.1/README.md`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/AboutDialog.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Constants.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Constants.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Environment.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Environment.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/FlatpakHandler.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/FlatpakHandler.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Functions.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Functions.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ImportExport.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ImportExport.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/MainWindow.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/MainWindow.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ProgressDialog.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ProgressDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Settings.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Settings.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/SettingsDialog.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Snapshot.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/Snapshot.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/SnapshotCollection.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/SnapshotCollection.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/WelcomeDialog.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/WelcomeDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/__init__.py` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/app-icon.svg` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/icons/app-icon.svg`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/default-icon.svg` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/icons/default-icon.svg`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts`

 * *Files 4% similar despite different names*

#### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts`

```diff
@@ -1,650 +1,660 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="de">
+<TS version="2.1" language="nl">
   <context>
     <name>AboutDialog</name>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>About</source>
-      <translation>Über</translation>
+      <translation>Over</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>A Program to create Snapshots of Flatpak Apps</source>
-      <translation>Ein Programm zum erstellen von Snapshots von Flatpak Apps</translation>
+      <translation>Een programma om momentopnamen van flatpakapps te maken</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
-      <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
+      <translation>Dit programma is uitgebracht onder de GPL3-licentie</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Translators</source>
-      <translation>Übersetzer</translation>
+      <translation>Vertalers</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>The following people translated jdFlatpakSnapshot:</source>
-      <translation>Die folgenden Personen haben jdFlatpakSnapshot übersetzt:</translation>
+      <translation>Deze mensen hebben jdFlatpakSnapshot vertaald:</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Changelog</source>
-      <translation>Änderungsprotokoll</translation>
+      <translation>Wijzigingslog</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Close</source>
-      <translation>Schließen</translation>
+      <translation>Sluiten</translation>
     </message>
   </context>
   <context>
     <name>Constants</name>
     <message>
       <location filename="../Constants.py" line="12"/>
       <source>None</source>
-      <translation>Keine</translation>
+      <translation>Geen</translation>
     </message>
   </context>
   <context>
     <name>ImportExport</name>
     <message>
       <location filename="../ImportExport.py" line="29"/>
       <source>This includes the following Snapshot:</source>
-      <translation>Dies enthält den folgenden Snapshot:</translation>
+      <translation>Dit bevat de volgende momentopname:</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="30"/>
       <source>App: {{app}}</source>
       <translation>App: {{app}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="31"/>
       <source>Name: {{name}}</source>
-      <translation>Name: {{name}}</translation>
+      <translation>Naam: {{name}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="32"/>
       <source>Compression: {{compression}}</source>
-      <translation>Komprimierungsverfahren: {{compression}}</translation>
+      <translation>Compressie: {{compression}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="33"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Größe auf dem Datenträger: {{size}}</translation>
+      <translation>Grootte op schijf: {{size}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="34"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Erstellt am: {{datetime}}</translation>
+      <translation>Gemaakt op: {{datetime}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="35"/>
       <source>Do you want to import it?</source>
-      <translation>Möchtest du ihn importieren?</translation>
+      <translation>Wilt u deze momentopname importeren?</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="37"/>
       <source>Import</source>
-      <translation>Importieren</translation>
+      <translation>Importeren</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="41"/>
       <source>App not installed</source>
-      <translation>App nicht installiert</translation>
+      <translation>App niet geïnstalleerd</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="41"/>
       <source>It looks like {{app}} is not installed. Are you really want to import the data?</source>
-      <translation>Es sieht so aus, als sei {{app}} nicht intstalliert. Mächtest du die Daten trotzdem importieren?</translation>
+      <translation>Het lijkt er op dan {{app}} niet geïnstalleerd is. Weet u zeker dat u de gegevens wilt importeren?</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="46"/>
       <source>New name</source>
-      <translation>Neuer Name</translation>
+      <translation>Nieuwe naam</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="46"/>
       <source>There is already a Snapshot with this Name for this App. Please enter a new one.</source>
-      <translation>Es existiert bereits ein Snapshot mt diesem Namen für diese App. Bitte gib einen neuen ein.</translation>
+      <translation>Er is al een momentopname van deze app onder deze naam. Kies een andere naam.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="52"/>
       <source>Name exists</source>
-      <translation>Name existiert</translation>
+      <translation>Naam in gebruik</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="52"/>
       <source>This Name also exists. Please enter a new one.</source>
-      <translation>Diser Name existiert auch. Bitte gib einen neuen ein.</translation>
+      <translation>Deze naam is ook in gebruik. Kies een andere naam.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="77"/>
       <source>Error</source>
-      <translation>Fehler</translation>
+      <translation>Foutmelding</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="77"/>
       <source>An error occurred during import. Maybe the File is not valid.</source>
-      <translation>Während des Importierens ist ein Fehler aufgetreten. Möglicherweise ist die Datei ungültig.</translation>
+      <translation>Er is een fout opgetreden tijdens het importeren. Mogelijk is het bestand beschadigd.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Export failed</source>
-      <translation>Export fehlgeschlagen</translation>
+      <translation>Exporteren mislukt</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Cound not export {{name}}</source>
-      <translation>Konnte {{name}} nicht exportieren</translation>
+      <translation>{{name}} kan niet worden geëxporteerd</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
       <location filename="../Languages.py" line="6"/>
       <source>English</source>
-      <translation>Englisch</translation>
+      <translation>Engels</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="7"/>
       <source>German</source>
-      <translation>Deutsch</translation>
+      <translation>Duits</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="8"/>
       <source>Dutch</source>
-      <translation>Niederländisch</translation>
+      <translation>Nederlands</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="9"/>
       <source>Turkish</source>
-      <translation>Türkisch</translation>
+      <translation>Turks</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="10"/>
+      <source>Ukrainian</source>
+      <translation>Oekraïens</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="11"/>
+      <source>Russian</source>
+      <translation>Russisch</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
       <location filename="../MainWindow.py" line="87"/>
       <source>No Flatpaks found</source>
-      <translation>Keine Flatpaks gefunden</translation>
+      <translation>Geen flatpaks aangetroffen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="87"/>
       <source>No flatpaks were found on your system. Make sure that some are installed and jdFlatpakSnapshot has the necessary permissions. If the problem persists, please report it. You can access the bug reporting page from the ? menu.</source>
-      <translation>Es wurden keine Flatpaks auf deinem System gefunden. Stelle sicher, dass welche installiert sind und jdFlatpakSnapshot die notwendigen Berechtigungen hat. Sollte der Fehler bestehen bleiben, melde ihn bitte. Du kannst die Seite zum Melden von Fehlern über das ? Menü aufrufen.</translation>
+      <translation>Er zijn geen flatpaks aangetroffen op uw systeem. Zorg dat er flatplaks geïnstalleerd zijn en dat jdFlatpakSnapshot over de juiste rechten beschikt. Als het probleem blijft optreden, maak hier dan melding van. U kunt de meldingspagina openen via het ?-menu.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="317"/>
       <location filename="../MainWindow.py" line="186"/>
       <source>Exported Snapshots</source>
-      <translation>Exportierte Snapshots</translation>
+      <translation>Geëxporteerde momentopnamen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="317"/>
       <location filename="../MainWindow.py" line="186"/>
       <source>All Files</source>
-      <translation>Alle Dateien</translation>
+      <translation>Alle bestanden</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="197"/>
       <source>Delete Snapshot of uninstalled Apps</source>
-      <translation>Snapshots von deinstallierten Apps löschen</translation>
+      <translation>Momentopname van verwijderde apps wissen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="197"/>
       <source>This will delete all Snapshots of apps that are no longer installed. Do you want to continue?</source>
-      <translation>Dies wird alle Snapshots von Apps löschen, die nicht mehr installiert sind. Möchtest du fortfahren?</translation>
+      <translation>Hierdoor worden alle momentopnamen van verwijderde apps gewist. Weet u zeker dat u wilt doorgaan?</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="216"/>
       <location filename="../MainWindow.py" line="205"/>
       <source>Snapshots deleted</source>
-      <translation>Snapshots gelöscht</translation>
+      <translation>Momentopnamen gewist</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="216"/>
       <location filename="../MainWindow.py" line="205"/>
       <source>The Snapshots were successfully deleted</source>
-      <translation>Die Snapshots wurden erfolgreich gelöscht</translation>
+      <translation>De momentopnamen zijn gewist</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../MainWindow.py" line="208"/>
       <source>Delete broken Snapshots</source>
-      <translation>Kaputte Snapshots löschen</translation>
+      <translation>Beschadigde momentopnamen wissen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="208"/>
       <source>This will delete all broken Snaphots. This might be needed, when a Bug occurs during the creation of a Snaphot or the data is messed up. Do you want to continue?</source>
-      <translation>Dies wird alle kaputten Snapshots löschen.Das wird eventuell benötigt, wenn während des Erstellens eines Snapshots ein Bug aufgetreten ist oder Dateien zerstört sind. Möchtest du fortfahren?</translation>
+      <translation>Hierdoor worden alle beschadigde momentopnamen gewist. Dit kan nodig zijn als er bijvoorbeeld een bug optreedt tijdens het maken van een momentopname of als de gegevens niet kloppen. Weet u zeker dat u wilt doorgaan?</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="222"/>
       <source>No data</source>
-      <translation>Keine Daten</translation>
+      <translation>Geen gegevens</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="222"/>
       <source>This Flatpak has no Data</source>
-      <translation>Dieses Flatpak hat keine Daten</translation>
+      <translation>Deze flatpak bevat geen gegevens</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="269"/>
       <location filename="../MainWindow.py" line="226"/>
       <source>Flatpak running</source>
-      <translation>Flatpak läuft</translation>
+      <translation>Flatpak in gebruik</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="269"/>
       <location filename="../MainWindow.py" line="226"/>
       <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
-      <translation>Dieses Flatpak wird gerade ausgeführt. Du kannst keinen Snapshot wiederherstellen, während das Flatpak gerade ausgeführt wird.</translation>
+      <translation>Deze flatpak is momenteel in gebruik. U kunt de momentopname van een flatpak niet herstellen zolang deze in gebruik is.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="231"/>
       <source>Could not get Commit</source>
-      <translation>Kontte Commit nicht auslesen</translation>
+      <translation>Kan commit niet opvragen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="231"/>
       <source>Could not get the commit for this Flatpak. You still can craete a Snapshot, but you will not know, to which Version it belongs.</source>
-      <translation>Der Commit dieses Flatpaks konnte nicht ausgelesen werden. Du kannst trotzdem einen Snapshot erstellen, weisst aber nacher nicht mehr, zu welcher Version er gehört.</translation>
+      <translation>De commit van deze flatpak kan niet worden opgevraagd. U kunt wel een momentopname maken, maar er wordt geen versienummer toegekend.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="233"/>
       <source>Enter Name</source>
-      <translation>Namen eingeben</translation>
+      <translation>Naam invoeren</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="233"/>
       <source>Please enter a Name for your Snapshot</source>
-      <translation>Bitte gib einen Namen für diesen Snapshot ein</translation>
+      <translation>Geef de momentopname een naam</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="296"/>
       <location filename="../MainWindow.py" line="239"/>
       <source>Name exists</source>
-      <translation>Name existiert</translation>
+      <translation>Naam in gebruik</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="239"/>
       <source>This Name already exists</source>
-      <translation>Dieser Name existiert bereits</translation>
+      <translation>Deze naam is al in gebruik</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="246"/>
       <source>Compression method</source>
-      <translation>Komprimierungsverfahren</translation>
+      <translation>Compressiemethode</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="246"/>
       <source>Please choose a compression method</source>
-      <translation>Bitte wähle ein Komprimierungsverfahren aus</translation>
+      <translation>Kies een compressiemethode</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="272"/>
       <source>Restore Snapshot</source>
-      <translation>Snapshot wiederherstellen</translation>
+      <translation>Momentopname herstellen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="272"/>
       <source>Are you sure you want to restore this Snapshot? This will overwrite all Data of this Flatpak.</source>
-      <translation>Bist du sicher, dass du diesen Snapshot wiederherstellen möchtest? Vorhandene Daten werden dabei überschrieben.</translation>
+      <translation>Weet u zeker dat u deze momentopname wilt herstellen? Hierdoor worden alle flatpakgegevens overschreven.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="282"/>
       <source>Error</source>
-      <translation>fehler</translation>
+      <translation>Foutmelding</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="282"/>
       <source>An error occurred while deleting {{path}}</source>
-      <translation>Während des Löschens von {{path}} ist ein Fehler aufgetreten</translation>
+      <translation>Er is een fout opgetreden tijdens het verwijderen van {{path}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="288"/>
       <source>New name</source>
-      <translation>Neuer Name</translation>
+      <translation>Nieuwe naam</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="288"/>
       <source>Please enter a new name</source>
-      <translation>Bitte gib einen neuen Namen ein</translation>
+      <translation>Voer een nieuwe naam in</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="296"/>
       <source>This name already exists</source>
-      <translation>Dieser Name existiert bereits</translation>
+      <translation>Deze naam is al in gebruik</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="304"/>
       <source>Delete snapshot</source>
-      <translation>Snapshot löschen</translation>
+      <translation>Momentopname verwijderen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="304"/>
       <source>Are you sure you want to delete this snapshot?</source>
-      <translation>Bist du sicher, dass du diesen Snapshot löschen willst?</translation>
+      <translation>Weet u zeker dat u deze momentopname wilt verwijderen?</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="314"/>
       <source>Snapshot deleted</source>
-      <translation>Snapshot gelöscht</translation>
+      <translation>Momentopname verwijderd</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="314"/>
       <source>The snapshot was successfully deleted</source>
-      <translation>Der Snapshot wurde erfolgreich gelöscht</translation>
+      <translation>De momentopname is verwijderd</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="328"/>
       <source>Compression: {{compression}}</source>
-      <translation>Komprimierungsverfahren: {{compression}}</translation>
+      <translation>Compressie: {{compression}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="329"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Größe auf dem Datenträger: {{size}}</translation>
+      <translation>Grootte op schijf: {{size}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="330"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Erstellt am: {{datetime}}</translation>
+      <translation>Gemaakt op: {{datetime}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="331"/>
       <source>Commit: {{commit}}</source>
       <translation>Commit: {{commit}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="331"/>
       <source>Unknown</source>
-      <translation>Unbekannt</translation>
+      <translation>Onbekend</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="333"/>
       <source>About {{name}}</source>
-      <translation>Über {{name}}</translation>
+      <translation>Over {{name}}</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Flatpaks</source>
       <translation>Flatpaks</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Create Snapshot</source>
-      <translation>Snapshot erstellen</translation>
+      <translation>Momentopname maken</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Snapshots</source>
-      <translation>Snapshots</translation>
+      <translation>Momentopnamen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Restore</source>
-      <translation>Wiederherstellen</translation>
+      <translation>Herstellen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Rename</source>
-      <translation>Umbennenen</translation>
+      <translation>Naam wijzigen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Delete</source>
-      <translation>Löschen</translation>
+      <translation>Verwijderen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Export</source>
-      <translation>Exportieren</translation>
+      <translation>Exporteren</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About</source>
-      <translation>Über</translation>
+      <translation>Over</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
-      <translation>Datei</translation>
+      <translation>Bestand</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Settings</source>
-      <translation>Einstellungen</translation>
+      <translation>Instellingen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Maintenance</source>
-      <translation>Wartung</translation>
+      <translation>Onderhoud</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About Qt</source>
-      <translation>Über Qt</translation>
+      <translation>Over Qt</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Exit</source>
-      <translation>Beenden</translation>
+      <translation>Afsluiten</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Import</source>
-      <translation>Import</translation>
+      <translation>Importeren</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Show welcome dialog</source>
-      <translation>Willkommensdialog zeigen</translation>
+      <translation>Welkomstvenster tonen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>View Source</source>
-      <translation>Quelltext ansehen</translation>
+      <translation>Broncode bekijken</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Report Bug</source>
-      <translation>Fehler melden</translation>
+      <translation>Bug melden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Translate</source>
-      <translation>Übersetzen</translation>
+      <translation>Vertalen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Donate</source>
-      <translation>Spenden</translation>
+      <translation>Doneren</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Delete Snapshots of uninstalled Apps</source>
-      <translation>Snapshots von deinstallierten Apps löschen</translation>
+      <translation>Momentopnamen van verwijderde apps wissen</translation>
     </message>
   </context>
   <context>
     <name>ProgressDialog</name>
     <message>
       <location filename="../ProgressDialog.py" line="32"/>
       <source>Scanning files. Please wait...</source>
-      <translation>Durchsuche Dateien. bite warten...</translation>
+      <translation>Bezig met doorzoeken van bestanden…</translation>
     </message>
     <message>
       <location filename="../ProgressDialog.py" line="42"/>
       <source>Compressing {{path}}</source>
-      <translation>Komprimiere {{path}}</translation>
+      <translation>Bezig met comprimeren van {{path}}…</translation>
     </message>
     <message>
       <location filename="../ProgressDialog.py" line="58"/>
       <source>Extracting {{path}}</source>
-      <translation>Extrahiere {{path}}</translation>
+      <translation>Bezig met extraheren van {{path}}…</translation>
     </message>
     <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>Progress</source>
-      <translation>Fortschritt</translation>
+      <translation>Voortgang</translation>
     </message>
     <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>The progress bar only shows how many files have been processed. It does not show the progress within a single file, so if a larger file is being processed, it may look like the program is hanging.</source>
-      <translation>Der Fortschrittsbalken zeigt nur an, wie viele Dateien bereits verarbeitet wurden. Er zeigt nicht an, den Fortschritt innerhalb einer einzigen Datei an, Wenn gerade eine größere Datei verarbeitet wird, kann es also so aussehen, als würde das Programm gerade hängen.</translation>
+      <translation>Let op: de voortgangsbalk toont alléén hoeveel bestanden er verwerkt zijn, dus níet de voortgang van losse bestanden. Bij het verwerken van grotere bestanden kan het daardoor lijken of het programma bevroren is.</translation>
     </message>
     <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
       <location filename="../SettingsDialog.py" line="27"/>
       <source>System language</source>
-      <translation>Systemsprache</translation>
+      <translation>Systeemtaal</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.py" line="57"/>
       <source>(Preview: {{preview}})</source>
-      <translation>(Vorschau: {{preview}})</translation>
+      <translation>(Voorbeeld: {{preview}})</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.py" line="59"/>
       <source>(Invalid)</source>
-      <translation>(Ungültig)</translation>
+      <translation>(Ongeldig)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
-      <translation>Einstellungen</translation>
+      <translation>Instellingen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>General</source>
-      <translation>Allgemein</translation>
+      <translation>Algemeen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>(needs restart)</source>
-      <translation>(benötigt Neustart)</translation>
+      <translation>(herstart vereist)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Datetime Format:</source>
-      <translation>Datumszeitformat:</translation>
+      <translation>Datum- en tijdopmaak:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
-      <translation>Sprache:</translation>
+      <translation>Taal:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Show system Apps</source>
-      <translation>Systemapps anzeigen</translation>
+      <translation>Systeemapps tonen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Show Apps with no Data</source>
-      <translation>Apps ohne Daten anzeigen</translation>
+      <translation>Gegevensloze apps tonen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Allow creating Snapshots while the App is running</source>
-      <translation>Erstellen von Snapshots während die App läuft erlauben</translation>
+      <translation>Ook momentopnamen maken terwijl apps actief zijn</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Allow restoring Snapshots while the App is running</source>
-      <translation>Wiederherstellen von Snapshots während die App läuft erlauben</translation>
+      <translation>Ook momentopnamen herstellen terwijl apps actief zijn</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Advanced</source>
-      <translation>Erweitert</translation>
+      <translation>Geavanceerd</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Flatpak Command</source>
-      <translation>Flatpakbefehl</translation>
+      <translation>Flatpakopdracht</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>You can specify the command to call Flatpak here. This is only needed if Flatpak is not present in the PATH due to an own installation.</source>
       <comment>Don't translate PATH, as it's the name of a Environment Variable</comment>
-      <translation>Du kannst hier den Befehl zum aufrufen von Flatpak festlegen. Dies wird nur benötigt, wenn Flatpak aufgrund eine eigenen Installation nicht im PATH vorhanden sein sollte.</translation>
+      <translation>Hier kunt u aangeven welke flatpakopdracht er dient te worden aangeroepen. Dit is alléén nodig als Flatpak niet op een door PATH opgenomen locatie geïnstalleerd is.</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Flatpak Command:</source>
-      <translation>Flatpakbefehl:</translation>
+      <translation>Flatpakopdracht:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Reset</source>
-      <translation>Zurücksetzen</translation>
+      <translation>Standaardwaarden</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Ok</translation>
+      <translation>Oké</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
-      <translation>Willkommen</translation>
+      <translation>Welkom</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome to jdFlatpakSnapshot!</source>
-      <translation>Willkommen bei jdFlatpakSnapshot!</translation>
+      <translation>Welkom in jdFlatpakSnapshot!</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program allows you to create a Snapshot of the Data of a Flatpak.</source>
-      <translation>Dieses Programm erlaubt dir, Snapshots von den Daten eines Flatpaks zu erstellen.</translation>
+      <translation>Met dit programma kunt u een momentopname van de gegevens van een flatpak maken.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>You can use this e.g. to play a with the Settings of a Program and when something doesn't work, restore the Snapshot.</source>
-      <translation>Du kannst das z.B. nutzen um mit den Einstellungen eines Programms herumzuspielen und falls etwas nicht funktioniert, einfach den alten Stand wiederherstellen.</translation>
+      <translation>Dit is bijvoorbeeld handig als u met de instellingen van een programma wilt spelen en ze nadien wilt herstellen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program only saves the Data of a Flatpak and the Version of the Flatpak, but not the Flatpak itself.</source>
-      <translation>Dieses Programm speichert nur die Daten eines Flatpaks sowie die Version, aber nicht das Flatpak selber.</translation>
+      <translation>Let op: dit programma maakt alleen een momentopname van de gegevens en versie van een flatpak, maar niet van de flatpak zelf.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>If you encounter a bug, please report it. You can access the Bug Tracker via ?&gt;Report Bug. Suggestions for improvement are also welcome.</source>
-      <translation>Solltest du auf einen Fehler stoßen, melde ihn bitte. Du kannst den Bugtracker über ?&gt;Fehler melden aufrufen. Verbesserungsvorschläge sind auch willkommen.</translation>
+      <translation>Als u een bug tegenkomt, meld deze dan. U kunt de bugpagina openen via ? → Bug melden. U kunt op die manier tevens ideeën delen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>To get started, select a Flatpak and click &quot;Create Snapshot&quot;.</source>
-      <translation>Um loszulegen, wähle ein Flatpak aus und klicke auf &quot;Snapshot erstellen&quot;.</translation>
+      <translation>Kies een flatpak en klik op ‘Momentopname maken’ om aan de slag te gaan.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Show this Dialog on Startup</source>
-      <translation>Diesen Dialog beim Programmstart anzeigen</translation>
+      <translation>Venster altijd tonen na opstarten</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts`

 * *Files 13% similar despite different names*

#### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts`

```diff
@@ -1,650 +1,660 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="nl">
+<TS version="2.1" language="de">
   <context>
     <name>AboutDialog</name>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Über</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>A Program to create Snapshots of Flatpak Apps</source>
-      <translation>Een programma om momentopnamen van flatpakapps te maken</translation>
+      <translation>Ein Programm zum erstellen von Snapshots von Flatpak Apps</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
-      <translation>Dit programma is uitgebracht onder de GPL3-licentie</translation>
+      <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Translators</source>
-      <translation>Vertalers</translation>
+      <translation>Übersetzer</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>The following people translated jdFlatpakSnapshot:</source>
-      <translation>Deze mensen hebben jdFlatpakSnapshot vertaald:</translation>
+      <translation>Die folgenden Personen haben jdFlatpakSnapshot übersetzt:</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Changelog</source>
-      <translation>Wijzigingslog</translation>
+      <translation>Änderungsprotokoll</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Close</source>
-      <translation>Sluiten</translation>
+      <translation>Schließen</translation>
     </message>
   </context>
   <context>
     <name>Constants</name>
     <message>
       <location filename="../Constants.py" line="12"/>
       <source>None</source>
-      <translation>Geen</translation>
+      <translation>Keine</translation>
     </message>
   </context>
   <context>
     <name>ImportExport</name>
     <message>
       <location filename="../ImportExport.py" line="29"/>
       <source>This includes the following Snapshot:</source>
-      <translation>Dit bevat de volgende momentopname:</translation>
+      <translation>Dies enthält den folgenden Snapshot:</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="30"/>
       <source>App: {{app}}</source>
       <translation>App: {{app}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="31"/>
       <source>Name: {{name}}</source>
-      <translation>Naam: {{name}}</translation>
+      <translation>Name: {{name}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="32"/>
       <source>Compression: {{compression}}</source>
-      <translation>Compressie: {{compression}}</translation>
+      <translation>Komprimierungsverfahren: {{compression}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="33"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Grootte op schijf: {{size}}</translation>
+      <translation>Größe auf dem Datenträger: {{size}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="34"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Gemaakt op: {{datetime}}</translation>
+      <translation>Erstellt am: {{datetime}}</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="35"/>
       <source>Do you want to import it?</source>
-      <translation>Wilt u deze momentopname importeren?</translation>
+      <translation>Möchtest du ihn importieren?</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="37"/>
       <source>Import</source>
-      <translation>Importeren</translation>
+      <translation>Importieren</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="41"/>
       <source>App not installed</source>
-      <translation>App niet geïnstalleerd</translation>
+      <translation>App nicht installiert</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="41"/>
       <source>It looks like {{app}} is not installed. Are you really want to import the data?</source>
-      <translation>Het lijkt er op dan {{app}} niet geïnstalleerd is. Weet u zeker dat u de gegevens wilt importeren?</translation>
+      <translation>Es sieht so aus, als sei {{app}} nicht intstalliert. Mächtest du die Daten trotzdem importieren?</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="46"/>
       <source>New name</source>
-      <translation>Nieuwe naam</translation>
+      <translation>Neuer Name</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="46"/>
       <source>There is already a Snapshot with this Name for this App. Please enter a new one.</source>
-      <translation>Er is al een momentopname van deze app onder deze naam. Kies een andere naam.</translation>
+      <translation>Es existiert bereits ein Snapshot mt diesem Namen für diese App. Bitte gib einen neuen ein.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="52"/>
       <source>Name exists</source>
-      <translation>Naam in gebruik</translation>
+      <translation>Name existiert</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="52"/>
       <source>This Name also exists. Please enter a new one.</source>
-      <translation>Deze naam is ook in gebruik. Kies een andere naam.</translation>
+      <translation>Diser Name existiert auch. Bitte gib einen neuen ein.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="77"/>
       <source>Error</source>
-      <translation>Foutmelding</translation>
+      <translation>Fehler</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="77"/>
       <source>An error occurred during import. Maybe the File is not valid.</source>
-      <translation>Er is een fout opgetreden tijdens het importeren. Mogelijk is het bestand beschadigd.</translation>
+      <translation>Während des Importierens ist ein Fehler aufgetreten. Möglicherweise ist die Datei ungültig.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Export failed</source>
-      <translation>Exporteren mislukt</translation>
+      <translation>Export fehlgeschlagen</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Cound not export {{name}}</source>
-      <translation>{{name}} kan niet worden geëxporteerd</translation>
+      <translation>Konnte {{name}} nicht exportieren</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
       <location filename="../Languages.py" line="6"/>
       <source>English</source>
-      <translation>Engels</translation>
+      <translation>Englisch</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="7"/>
       <source>German</source>
-      <translation>Duits</translation>
+      <translation>Deutsch</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="8"/>
       <source>Dutch</source>
-      <translation>Nederlands</translation>
+      <translation>Niederländisch</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="9"/>
       <source>Turkish</source>
-      <translation>Turks</translation>
+      <translation>Türkisch</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="10"/>
+      <source>Ukrainian</source>
+      <translation>Ukrainisch</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="11"/>
+      <source>Russian</source>
+      <translation>Russisch</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
       <location filename="../MainWindow.py" line="87"/>
       <source>No Flatpaks found</source>
-      <translation>Geen flatpaks aangetroffen</translation>
+      <translation>Keine Flatpaks gefunden</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="87"/>
       <source>No flatpaks were found on your system. Make sure that some are installed and jdFlatpakSnapshot has the necessary permissions. If the problem persists, please report it. You can access the bug reporting page from the ? menu.</source>
-      <translation>Er zijn geen flatpaks aangetroffen op uw systeem. Zorg dat er flatplaks geïnstalleerd zijn en dat jdFlatpakSnapshot over de juiste rechten beschikt. Als het probleem blijft optreden, maak hier dan melding van. U kunt de meldingspagina openen via het ?-menu.</translation>
+      <translation>Es wurden keine Flatpaks auf deinem System gefunden. Stelle sicher, dass welche installiert sind und jdFlatpakSnapshot die notwendigen Berechtigungen hat. Sollte der Fehler bestehen bleiben, melde ihn bitte. Du kannst die Seite zum Melden von Fehlern über das ? Menü aufrufen.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="317"/>
       <location filename="../MainWindow.py" line="186"/>
       <source>Exported Snapshots</source>
-      <translation>Geëxporteerde momentopnamen</translation>
+      <translation>Exportierte Snapshots</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="317"/>
       <location filename="../MainWindow.py" line="186"/>
       <source>All Files</source>
-      <translation>Alle bestanden</translation>
+      <translation>Alle Dateien</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="197"/>
       <source>Delete Snapshot of uninstalled Apps</source>
-      <translation>Momentopname van verwijderde apps wissen</translation>
+      <translation>Snapshots von deinstallierten Apps löschen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="197"/>
       <source>This will delete all Snapshots of apps that are no longer installed. Do you want to continue?</source>
-      <translation>Hierdoor worden alle momentopnamen van verwijderde apps gewist. Weet u zeker dat u wilt doorgaan?</translation>
+      <translation>Dies wird alle Snapshots von Apps löschen, die nicht mehr installiert sind. Möchtest du fortfahren?</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="216"/>
       <location filename="../MainWindow.py" line="205"/>
       <source>Snapshots deleted</source>
-      <translation>Momentopnamen gewist</translation>
+      <translation>Snapshots gelöscht</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="216"/>
       <location filename="../MainWindow.py" line="205"/>
       <source>The Snapshots were successfully deleted</source>
-      <translation>De momentopnamen zijn gewist</translation>
+      <translation>Die Snapshots wurden erfolgreich gelöscht</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../MainWindow.py" line="208"/>
       <source>Delete broken Snapshots</source>
-      <translation>Beschadigde momentopnamen wissen</translation>
+      <translation>Kaputte Snapshots löschen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="208"/>
       <source>This will delete all broken Snaphots. This might be needed, when a Bug occurs during the creation of a Snaphot or the data is messed up. Do you want to continue?</source>
-      <translation>Hierdoor worden alle beschadigde momentopnamen gewist. Dit kan nodig zijn als er bijvoorbeeld een bug optreedt tijdens het maken van een momentopname of als de gegevens niet kloppen. Weet u zeker dat u wilt doorgaan?</translation>
+      <translation>Dies wird alle kaputten Snapshots löschen.Das wird eventuell benötigt, wenn während des Erstellens eines Snapshots ein Bug aufgetreten ist oder Dateien zerstört sind. Möchtest du fortfahren?</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="222"/>
       <source>No data</source>
-      <translation>Geen gegevens</translation>
+      <translation>Keine Daten</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="222"/>
       <source>This Flatpak has no Data</source>
-      <translation>Deze flatpak bevat geen gegevens</translation>
+      <translation>Dieses Flatpak hat keine Daten</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="269"/>
       <location filename="../MainWindow.py" line="226"/>
       <source>Flatpak running</source>
-      <translation>Flatpak in gebruik</translation>
+      <translation>Flatpak läuft</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="269"/>
       <location filename="../MainWindow.py" line="226"/>
       <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
-      <translation>Deze flatpak is momenteel in gebruik. U kunt de momentopname van een flatpak niet herstellen zolang deze in gebruik is.</translation>
+      <translation>Dieses Flatpak wird gerade ausgeführt. Du kannst keinen Snapshot wiederherstellen, während das Flatpak gerade ausgeführt wird.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="231"/>
       <source>Could not get Commit</source>
-      <translation>Kan commit niet opvragen</translation>
+      <translation>Kontte Commit nicht auslesen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="231"/>
       <source>Could not get the commit for this Flatpak. You still can craete a Snapshot, but you will not know, to which Version it belongs.</source>
-      <translation>De commit van deze flatpak kan niet worden opgevraagd. U kunt wel een momentopname maken, maar er wordt geen versienummer toegekend.</translation>
+      <translation>Der Commit dieses Flatpaks konnte nicht ausgelesen werden. Du kannst trotzdem einen Snapshot erstellen, weisst aber nacher nicht mehr, zu welcher Version er gehört.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="233"/>
       <source>Enter Name</source>
-      <translation>Naam invoeren</translation>
+      <translation>Namen eingeben</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="233"/>
       <source>Please enter a Name for your Snapshot</source>
-      <translation>Geef de momentopname een naam</translation>
+      <translation>Bitte gib einen Namen für diesen Snapshot ein</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="296"/>
       <location filename="../MainWindow.py" line="239"/>
       <source>Name exists</source>
-      <translation>Naam in gebruik</translation>
+      <translation>Name existiert</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="239"/>
       <source>This Name already exists</source>
-      <translation>Deze naam is al in gebruik</translation>
+      <translation>Dieser Name existiert bereits</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="246"/>
       <source>Compression method</source>
-      <translation>Compressiemethode</translation>
+      <translation>Komprimierungsverfahren</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="246"/>
       <source>Please choose a compression method</source>
-      <translation>Kies een compressiemethode</translation>
+      <translation>Bitte wähle ein Komprimierungsverfahren aus</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="272"/>
       <source>Restore Snapshot</source>
-      <translation>Momentopname herstellen</translation>
+      <translation>Snapshot wiederherstellen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="272"/>
       <source>Are you sure you want to restore this Snapshot? This will overwrite all Data of this Flatpak.</source>
-      <translation>Weet u zeker dat u deze momentopname wilt herstellen? Hierdoor worden alle flatpakgegevens overschreven.</translation>
+      <translation>Bist du sicher, dass du diesen Snapshot wiederherstellen möchtest? Vorhandene Daten werden dabei überschrieben.</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="282"/>
       <source>Error</source>
-      <translation>Foutmelding</translation>
+      <translation>fehler</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="282"/>
       <source>An error occurred while deleting {{path}}</source>
-      <translation>Er is een fout opgetreden tijdens het verwijderen van {{path}}</translation>
+      <translation>Während des Löschens von {{path}} ist ein Fehler aufgetreten</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="288"/>
       <source>New name</source>
-      <translation>Nieuwe naam</translation>
+      <translation>Neuer Name</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="288"/>
       <source>Please enter a new name</source>
-      <translation>Voer een nieuwe naam in</translation>
+      <translation>Bitte gib einen neuen Namen ein</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="296"/>
       <source>This name already exists</source>
-      <translation>Deze naam is al in gebruik</translation>
+      <translation>Dieser Name existiert bereits</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="304"/>
       <source>Delete snapshot</source>
-      <translation>Momentopname verwijderen</translation>
+      <translation>Snapshot löschen</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="304"/>
       <source>Are you sure you want to delete this snapshot?</source>
-      <translation>Weet u zeker dat u deze momentopname wilt verwijderen?</translation>
+      <translation>Bist du sicher, dass du diesen Snapshot löschen willst?</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="314"/>
       <source>Snapshot deleted</source>
-      <translation>Momentopname verwijderd</translation>
+      <translation>Snapshot gelöscht</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="314"/>
       <source>The snapshot was successfully deleted</source>
-      <translation>De momentopname is verwijderd</translation>
+      <translation>Der Snapshot wurde erfolgreich gelöscht</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="328"/>
       <source>Compression: {{compression}}</source>
-      <translation>Compressie: {{compression}}</translation>
+      <translation>Komprimierungsverfahren: {{compression}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="329"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Grootte op schijf: {{size}}</translation>
+      <translation>Größe auf dem Datenträger: {{size}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="330"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Gemaakt op: {{datetime}}</translation>
+      <translation>Erstellt am: {{datetime}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="331"/>
       <source>Commit: {{commit}}</source>
       <translation>Commit: {{commit}}</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="331"/>
       <source>Unknown</source>
-      <translation>Onbekend</translation>
+      <translation>Unbekannt</translation>
     </message>
     <message>
       <location filename="../MainWindow.py" line="333"/>
       <source>About {{name}}</source>
-      <translation>Over {{name}}</translation>
+      <translation>Über {{name}}</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Flatpaks</source>
       <translation>Flatpaks</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Create Snapshot</source>
-      <translation>Momentopname maken</translation>
+      <translation>Snapshot erstellen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Snapshots</source>
-      <translation>Momentopnamen</translation>
+      <translation>Snapshots</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Restore</source>
-      <translation>Herstellen</translation>
+      <translation>Wiederherstellen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Rename</source>
-      <translation>Naam wijzigen</translation>
+      <translation>Umbennenen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Delete</source>
-      <translation>Verwijderen</translation>
+      <translation>Löschen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Export</source>
-      <translation>Exporteren</translation>
+      <translation>Exportieren</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Über</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
-      <translation>Bestand</translation>
+      <translation>Datei</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Settings</source>
-      <translation>Instellingen</translation>
+      <translation>Einstellungen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Maintenance</source>
-      <translation>Onderhoud</translation>
+      <translation>Wartung</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About Qt</source>
-      <translation>Over Qt</translation>
+      <translation>Über Qt</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Exit</source>
-      <translation>Afsluiten</translation>
+      <translation>Beenden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Import</source>
-      <translation>Importeren</translation>
+      <translation>Import</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Show welcome dialog</source>
-      <translation>Welkomstvenster tonen</translation>
+      <translation>Willkommensdialog zeigen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>View Source</source>
-      <translation>Broncode bekijken</translation>
+      <translation>Quelltext ansehen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Report Bug</source>
-      <translation>Bug melden</translation>
+      <translation>Fehler melden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Translate</source>
-      <translation>Vertalen</translation>
+      <translation>Übersetzen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Donate</source>
-      <translation>Doneren</translation>
+      <translation>Spenden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Delete Snapshots of uninstalled Apps</source>
-      <translation>Momentopnamen van verwijderde apps wissen</translation>
+      <translation>Snapshots von deinstallierten Apps löschen</translation>
     </message>
   </context>
   <context>
     <name>ProgressDialog</name>
     <message>
       <location filename="../ProgressDialog.py" line="32"/>
       <source>Scanning files. Please wait...</source>
-      <translation>Bezig met doorzoeken van bestanden…</translation>
+      <translation>Durchsuche Dateien. bite warten...</translation>
     </message>
     <message>
       <location filename="../ProgressDialog.py" line="42"/>
       <source>Compressing {{path}}</source>
-      <translation>Bezig met comprimeren van {{path}}…</translation>
+      <translation>Komprimiere {{path}}</translation>
     </message>
     <message>
       <location filename="../ProgressDialog.py" line="58"/>
       <source>Extracting {{path}}</source>
-      <translation>Bezig met extraheren van {{path}}…</translation>
+      <translation>Extrahiere {{path}}</translation>
     </message>
     <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>Progress</source>
-      <translation>Voortgang</translation>
+      <translation>Fortschritt</translation>
     </message>
     <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>The progress bar only shows how many files have been processed. It does not show the progress within a single file, so if a larger file is being processed, it may look like the program is hanging.</source>
-      <translation>Let op: de voortgangsbalk toont alléén hoeveel bestanden er verwerkt zijn, dus níet de voortgang van losse bestanden. Bij het verwerken van grotere bestanden kan het daardoor lijken of het programma bevroren is.</translation>
+      <translation>Der Fortschrittsbalken zeigt nur an, wie viele Dateien bereits verarbeitet wurden. Er zeigt nicht an, den Fortschritt innerhalb einer einzigen Datei an, Wenn gerade eine größere Datei verarbeitet wird, kann es also so aussehen, als würde das Programm gerade hängen.</translation>
     </message>
     <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
       <location filename="../SettingsDialog.py" line="27"/>
       <source>System language</source>
-      <translation>Systeemtaal</translation>
+      <translation>Systemsprache</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.py" line="57"/>
       <source>(Preview: {{preview}})</source>
-      <translation>(Voorbeeld: {{preview}})</translation>
+      <translation>(Vorschau: {{preview}})</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.py" line="59"/>
       <source>(Invalid)</source>
-      <translation>(Ongeldig)</translation>
+      <translation>(Ungültig)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
-      <translation>Instellingen</translation>
+      <translation>Einstellungen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>General</source>
-      <translation>Algemeen</translation>
+      <translation>Allgemein</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>(needs restart)</source>
-      <translation>(herstart vereist)</translation>
+      <translation>(benötigt Neustart)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Datetime Format:</source>
-      <translation>Datum- en tijdopmaak:</translation>
+      <translation>Datumszeitformat:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
-      <translation>Taal:</translation>
+      <translation>Sprache:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Show system Apps</source>
-      <translation>Systeemapps tonen</translation>
+      <translation>Systemapps anzeigen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Show Apps with no Data</source>
-      <translation>Gegevensloze apps tonen</translation>
+      <translation>Apps ohne Daten anzeigen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Allow creating Snapshots while the App is running</source>
-      <translation>Ook momentopnamen maken terwijl apps actief zijn</translation>
+      <translation>Erstellen von Snapshots während die App läuft erlauben</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Allow restoring Snapshots while the App is running</source>
-      <translation>Ook momentopnamen herstellen terwijl apps actief zijn</translation>
+      <translation>Wiederherstellen von Snapshots während die App läuft erlauben</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Advanced</source>
-      <translation>Geavanceerd</translation>
+      <translation>Erweitert</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Flatpak Command</source>
-      <translation>Flatpakopdracht</translation>
+      <translation>Flatpakbefehl</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>You can specify the command to call Flatpak here. This is only needed if Flatpak is not present in the PATH due to an own installation.</source>
       <comment>Don't translate PATH, as it's the name of a Environment Variable</comment>
-      <translation>Hier kunt u aangeven welke flatpakopdracht er dient te worden aangeroepen. Dit is alléén nodig als Flatpak niet op een door PATH opgenomen locatie geïnstalleerd is.</translation>
+      <translation>Du kannst hier den Befehl zum aufrufen von Flatpak festlegen. Dies wird nur benötigt, wenn Flatpak aufgrund eine eigenen Installation nicht im PATH vorhanden sein sollte.</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Flatpak Command:</source>
-      <translation>Flatpakopdracht:</translation>
+      <translation>Flatpakbefehl:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Reset</source>
-      <translation>Standaardwaarden</translation>
+      <translation>Zurücksetzen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>Ok</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
-      <translation>Welkom</translation>
+      <translation>Willkommen</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome to jdFlatpakSnapshot!</source>
-      <translation>Welkom in jdFlatpakSnapshot!</translation>
+      <translation>Willkommen bei jdFlatpakSnapshot!</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program allows you to create a Snapshot of the Data of a Flatpak.</source>
-      <translation>Met dit programma kunt u een momentopname van de gegevens van een flatpak maken.</translation>
+      <translation>Dieses Programm erlaubt dir, Snapshots von den Daten eines Flatpaks zu erstellen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>You can use this e.g. to play a with the Settings of a Program and when something doesn't work, restore the Snapshot.</source>
-      <translation>Dit is bijvoorbeeld handig als u met de instellingen van een programma wilt spelen en ze nadien wilt herstellen.</translation>
+      <translation>Du kannst das z.B. nutzen um mit den Einstellungen eines Programms herumzuspielen und falls etwas nicht funktioniert, einfach den alten Stand wiederherstellen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program only saves the Data of a Flatpak and the Version of the Flatpak, but not the Flatpak itself.</source>
-      <translation>Let op: dit programma maakt alleen een momentopname van de gegevens en versie van een flatpak, maar niet van de flatpak zelf.</translation>
+      <translation>Dieses Programm speichert nur die Daten eines Flatpaks sowie die Version, aber nicht das Flatpak selber.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>If you encounter a bug, please report it. You can access the Bug Tracker via ?&gt;Report Bug. Suggestions for improvement are also welcome.</source>
-      <translation>Als u een bug tegenkomt, meld deze dan. U kunt de bugpagina openen via ? → Bug melden. U kunt op die manier tevens ideeën delen.</translation>
+      <translation>Solltest du auf einen Fehler stoßen, melde ihn bitte. Du kannst den Bugtracker über ?&gt;Fehler melden aufrufen. Verbesserungsvorschläge sind auch willkommen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>To get started, select a Flatpak and click &quot;Create Snapshot&quot;.</source>
-      <translation>Kies een flatpak en klik op ‘Momentopname maken’ om aan de slag te gaan.</translation>
+      <translation>Um loszulegen, wähle ein Flatpak aus und klicke auf &quot;Snapshot erstellen&quot;.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Show this Dialog on Startup</source>
-      <translation>Venster altijd tonen na opstarten</translation>
+      <translation>Diesen Dialog beim Programmstart anzeigen</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts`

 * *Files 1% similar despite different names*

#### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts`

```diff
@@ -159,14 +159,24 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../Languages.py" line="9"/>
       <source>Turkish</source>
       <translation type="unfinished"/>
     </message>
+    <message>
+      <location filename="../Languages.py" line="10"/>
+      <source>Ukrainian</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="11"/>
+      <source>Russian</source>
+      <translation type="unfinished"/>
+    </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
       <location filename="../MainWindow.py" line="87"/>
       <source>No Flatpaks found</source>
       <translation type="unfinished"/>
```

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/AboutDialog.ui` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/AboutDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/MainWindow.ui` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/ProgressDialog.ui` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/ProgressDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/SettingsDialog.ui` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/SettingsDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/WelcomeDialog.ui` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot/ui/WelcomeDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/PKG-INFO` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jdFlatpakSnapshot
-Version: 2.0
+Version: 2.1
 Summary: A Program to create Snapshots of Flatpak Apps
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdFlatpakSnaphot
 Project-URL: Issues, https://codeberg.org/JakobDev/jdFlatpakSnapshot/issues
+Project-URL: Translate, https://translate.codeberg.org/projects/jdFlatpakSnapshot
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Linux,Flatpak
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/SOURCES.txt` & `jdFlatpakSnapshot-2.1/jdFlatpakSnapshot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,13 +27,15 @@
 jdFlatpakSnapshot.egg-info/entry_points.txt
 jdFlatpakSnapshot.egg-info/requires.txt
 jdFlatpakSnapshot.egg-info/top_level.txt
 jdFlatpakSnapshot/icons/app-icon.svg
 jdFlatpakSnapshot/icons/default-icon.svg
 jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
 jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts
+jdFlatpakSnapshot/translations/jdFlatpakSnapshot_ru.ts
 jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts
+jdFlatpakSnapshot/translations/jdFlatpakSnapshot_uk.ts
 jdFlatpakSnapshot/ui/AboutDialog.ui
 jdFlatpakSnapshot/ui/MainWindow.ui
 jdFlatpakSnapshot/ui/ProgressDialog.ui
 jdFlatpakSnapshot/ui/SettingsDialog.ui
 jdFlatpakSnapshot/ui/WelcomeDialog.ui
```

### Comparing `jdFlatpakSnapshot-2.0/pyproject.toml` & `jdFlatpakSnapshot-2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "PyQt6", "wheel"]
 build-backend = "BuildBackend"
 backend-path = ["."]
 
 [project]
 name = "jdFlatpakSnapshot"
 description = "A Program to create Snapshots of Flatpak Apps"
 readme = "README.md"
@@ -31,14 +31,15 @@
   "desktop-entry-lib"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://codeberg.org/JakobDev/jdFlatpakSnaphot"
 Issues = "https://codeberg.org/JakobDev/jdFlatpakSnapshot/issues"
+Translate = "https://translate.codeberg.org/projects/jdFlatpakSnapshot"
 Donation = "https://ko-fi.com/jakobdev"
 
 [project.gui-scripts]
 jdflatpaksnapshot = "jdFlatpakSnapshot:main"
 
 [tool.setuptools.package-dir]
 jdFlatpakSnapshot = "jdFlatpakSnapshot"
```

