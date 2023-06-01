# Comparing `tmp/UEVaultManager-1.6.2.tar.gz` & `tmp/UEVaultManager-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.6.2.tar", last modified: Wed May 31 17:18:08 2023, max compression
+gzip compressed data, was "UEVaultManager-1.6.3.tar", last modified: Thu Jun  1 08:13:24 2023, max compression
```

## Comparing `UEVaultManager-1.6.2.tar` & `UEVaultManager-1.6.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.983884 UEVaultManager-1.6.2/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     6127 2023-05-31 17:18:08.983884 UEVaultManager-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.946884 UEVaultManager-1.6.2/UEVaultManager/
--rw-rw-rw-   0        0        0      778 2023-05-31 17:17:25.000000 UEVaultManager-1.6.2/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.952884 UEVaultManager-1.6.2/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-25 16:36:39.000000 UEVaultManager-1.6.2/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.2/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.955885 UEVaultManager-1.6.2/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.2/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.6.2/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.2/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.6.2/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    72442 2023-05-31 17:11:25.000000 UEVaultManager-1.6.2/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47592 2023-05-31 17:11:24.000000 UEVaultManager-1.6.2/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.956884 UEVaultManager-1.6.2/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.957883 UEVaultManager-1.6.2/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.6.2/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.2/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.961884 UEVaultManager-1.6.2/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.2/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.2/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23585 2023-05-26 09:04:11.000000 UEVaultManager-1.6.2/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.2/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.6.2/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.967884 UEVaultManager-1.6.2/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-25 16:35:27.000000 UEVaultManager-1.6.2/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.6.2/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.2/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.2/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.2/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.2/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.2/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30505 2023-05-25 16:36:21.000000 UEVaultManager-1.6.2/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.968883 UEVaultManager-1.6.2/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1694 2023-05-26 08:33:52.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.978884 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    33931 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0    13334 2023-05-31 17:11:24.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    43221 2023-05-31 15:30:23.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0     9697 2023-05-31 17:11:24.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     6036 2023-05-31 16:57:38.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/functions_no_deps.py
--rw-rw-rw-   0        0        0     2631 2023-05-31 15:29:53.000000 UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.982884 UEVaultManager-1.6.2/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3478 2023-05-25 16:35:05.000000 UEVaultManager-1.6.2/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.6.2/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.2/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.6.2/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.2/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.2/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.2/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:08.950885 UEVaultManager-1.6.2/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6127 2023-05-31 17:18:08.000000 UEVaultManager-1.6.2/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-05-31 17:18:08.000000 UEVaultManager-1.6.2/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:18:08.000000 UEVaultManager-1.6.2/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-31 17:18:08.000000 UEVaultManager-1.6.2/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      300 2023-05-31 17:18:08.000000 UEVaultManager-1.6.2/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 17:18:08.000000 UEVaultManager-1.6.2/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 17:18:08.983884 UEVaultManager-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.454998 UEVaultManager-1.6.3/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0     6127 2023-06-01 08:13:24.454998 UEVaultManager-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.417992 UEVaultManager-1.6.3/UEVaultManager/
+-rw-rw-rw-   0        0        0      778 2023-06-01 08:10:45.000000 UEVaultManager-1.6.3/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.422992 UEVaultManager-1.6.3/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.3/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-25 16:36:39.000000 UEVaultManager-1.6.3/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.3/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.425992 UEVaultManager-1.6.3/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.3/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.6.3/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.3/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.6.3/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    72972 2023-06-01 08:08:08.000000 UEVaultManager-1.6.3/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    46806 2023-06-01 06:50:17.000000 UEVaultManager-1.6.3/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.425992 UEVaultManager-1.6.3/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.3/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.427993 UEVaultManager-1.6.3/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.3/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.6.3/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.3/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.430992 UEVaultManager-1.6.3/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.3/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.3/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.3/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23585 2023-05-26 09:04:11.000000 UEVaultManager-1.6.3/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.3/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3927 2023-06-01 07:37:43.000000 UEVaultManager-1.6.3/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.436992 UEVaultManager-1.6.3/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.3/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     5942 2023-06-01 07:24:48.000000 UEVaultManager-1.6.3/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.6.3/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.3/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.3/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.3/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.6.3/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.3/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.3/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30610 2023-06-01 07:29:35.000000 UEVaultManager-1.6.3/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.438993 UEVaultManager-1.6.3/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1694 2023-05-26 08:33:52.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.449992 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    32497 2023-06-01 06:46:43.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0    12723 2023-06-01 07:08:05.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    43199 2023-06-01 07:25:24.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0     9697 2023-05-31 17:11:24.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     6344 2023-06-01 07:39:35.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/functions_no_deps.py
+-rw-rw-rw-   0        0        0     2631 2023-05-31 15:29:53.000000 UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.453997 UEVaultManager-1.6.3/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.3/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3691 2023-06-01 07:18:12.000000 UEVaultManager-1.6.3/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.6.3/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.3/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.6.3/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.3/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.3/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.3/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:13:24.421992 UEVaultManager-1.6.3/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6127 2023-06-01 08:13:24.000000 UEVaultManager-1.6.3/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-06-01 08:13:24.000000 UEVaultManager-1.6.3/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:13:24.000000 UEVaultManager-1.6.3/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-01 08:13:24.000000 UEVaultManager-1.6.3/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      300 2023-06-01 08:13:24.000000 UEVaultManager-1.6.3/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 08:13:24.000000 UEVaultManager-1.6.3/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:13:24.455996 UEVaultManager-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.3/setup.py
```

### Comparing `UEVaultManager-1.6.2/LICENSE` & `UEVaultManager-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/PKG-INFO` & `UEVaultManager-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.2
+Version: 1.6.3
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.6.2 ## codename: Virgo+2
+ UEVaultManager ## version:1.6.3 ## codename: Virgo+3
```

### Comparing `UEVaultManager-1.6.2/README.md` & `UEVaultManager-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/__init__.py` & `UEVaultManager-1.6.3/UEVaultManager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.6.2'
+__version__ = '1.6.3'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
 # 5 Virgo Shaka
-__codename__ = 'Virgo+2'
+__codename__ = 'Virgo+3'
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/api/egs.py` & `UEVaultManager-1.6.3/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/api/uevm.py` & `UEVaultManager-1.6.3/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.6.3/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/assets/main.ico` & `UEVaultManager-1.6.3/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/cli.py` & `UEVaultManager-1.6.3/UEVaultManager/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1139,27 +1139,28 @@
             file=input_filename,
             rebuild_data=rebuild
         )
         gui_g.UEVM_gui_ref.mainloop()
         # gui_g.UEVM_gui_ref.quit()
 
     @staticmethod
-    def print_help(args, parser=None) -> None:
+    def print_help(args, parser=None, forced=False) -> None:
         """
         Prints the help for the command
         :param args:
         :param parser: command line parser. If not provided, gui_g.UEVM_parser_ref will be used
+        :param forced: if True, the help will be printed even if the --help option is not present
         """
         if parser is None:
             parser = gui_g.UEVM_parser_ref
         if parser is None:
             return
         uewm_gui_exists = False
 
-        if args.full_help:
+        if args.full_help or forced:
             if args.gui:
                 uewm_gui_exists, _ = init_display_window()
             custom_print(keep_mode=False, text=parser.format_help())
 
             # Commands that should not be shown in full help/list of commands (e.g. aliases)
             _hidden_commands = {'download', 'update', 'repair', 'get-token', 'verify-asset', 'list-assets'}
             # Print the help for all the subparsers. Thanks stackoverflow!
@@ -1176,30 +1177,43 @@
             from UEVaultManager.lfs.windows_helpers import double_clicked
             if double_clicked():
                 custom_print(text='Please note that this is not the intended way to run UEVaultManager.')
                 custom_print(text='If you want to start it without arguments, you can start it in edit mode by default.')
                 custom_print(text='For that, you must set the line start_in_edit_mode=true in the configuration file.')
                 custom_print(text='More info on usage and configuration can be found in https://github.com/LaurentOngaro/UEVaultManager#readme')
                 subprocess.Popen(['cmd', '/K', 'echo>nul'])
-        custom_print(keep_mode=False)  # as it, next print will not keep the content
+        else:
+            # on non-windows systems
+            # UEVaultManagerCLI.print_help(args, parser=parser, forced=True)
+            UEVaultManagerCLI.print_version()
+            return
 
         if args.gui and not uewm_gui_exists:
             gui_g.UEVM_gui_ref.mainloop()
 
+    @staticmethod
+    def print_version():
+        """
+        Prints the version of UEVaultManager and exit
+        """
+        print(f'UEVaultManager version "{UEVM_version}", codename "{UEVM_codename}"')
+        sys.exit(0)
+
 
 def main():
     """
     Main function
     """
     parser = argparse.ArgumentParser(description=f'UEVaultManager v{UEVM_version} - "{UEVM_codename}"')
     parser.register('action', 'parsers', HiddenAliasSubparsersAction)
 
     # general arguments
     parser.add_argument('-H', '--full-help', dest='full_help', action='store_true', help='Show full help (including individual command help)')
     parser.add_argument('-d', '--debug', dest='debug', action='store_true', help='Set loglevel to debug')
+    # noinspection DuplicatedCode
     parser.add_argument('-y', '--yes', dest='yes', action='store_true', help='Default to yes for all prompts')
     parser.add_argument('-V', '--version', dest='version', action='store_true', help='Print version and exit')
     parser.add_argument(
         '-c', '--config-file', dest='config_file', action='store', metavar='<path/name>', help='Overwrite the default configuration file name to use'
     )
     parser.add_argument('-J', '--pretty-json', dest='pretty_json', action='store_true', help='Pretty-print JSON. Improve readability')
     parser.add_argument(
@@ -1261,14 +1275,15 @@
     )
     auth_parser.add_argument('--delete', dest='auth_delete', action='store_true', help='Remove existing authentication (log out)')
     auth_parser.add_argument('--disable-webview', dest='no_webview', action='store_true', help='Do not use embedded browser for login')
 
     list_parser.add_argument(
         '-T', '--third-party', dest='include_non_asset', action='store_true', default=False, help='Include assets that are not installable.'
     )
+    # noinspection DuplicatedCode
     list_parser.add_argument('--csv', dest='csv', action='store_true', help='Output in in CSV format')
     list_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Output in in TSV format')
     list_parser.add_argument('--json', dest='json', action='store_true', help='Output in in JSON format')
     list_parser.add_argument(
         '-f',
         '--force-refresh',
         dest='force_refresh',
@@ -1294,14 +1309,15 @@
     )
 
     list_files_parser.add_argument(
         '--manifest', dest='override_manifest', action='store', metavar='<uri>', help='Manifest URL or path to use instead of the CDN one'
     )
     list_files_parser.add_argument('--csv', dest='csv', action='store_true', help='Output in CSV format')
     list_files_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Output in TSV format')
+    # noinspection DuplicatedCode
     list_files_parser.add_argument('--json', dest='json', action='store_true', help='Output in JSON format')
     list_files_parser.add_argument(
         '--hashlist', dest='hashlist', action='store_true', help='Output file hash list in hashCheck/sha1sum -c compatible format'
     )
     list_files_parser.add_argument(
         '-f',
         '--force-refresh',
@@ -1328,15 +1344,15 @@
         '-m,'
         '--delete-metadata', dest='delete_metadata', action='store_true', help='Also delete metadata files. They are kept by default'
     )
     clean_parser.add_argument(
         '-e,'
         '--delete-extras-data', dest='delete_extras_data', action='store_true', help='Also delete extras data files. They are kept by default'
     )
-
+    # noinspection DuplicatedCode
     info_parser.add_argument('--offline', dest='offline', action='store_true', help='Only print info available offline')
     info_parser.add_argument('--json', dest='json', action='store_true', help='Output information in JSON format')
     info_parser.add_argument(
         '-f',
         '--force-refresh',
         dest='force_refresh',
         action='store_true',
@@ -1355,16 +1371,15 @@
     # edit_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Input file is in TSV format')
     # edit_parser.add_argument('--json', dest='json', action='store_true', help='Input file is in JSON format')
 
     # Note: this line prints the full help and quit if not other command is available
     args, extra = parser.parse_known_args()
 
     if args.version:
-        print(f'UEVaultManager version "{UEVM_version}", codename "{UEVM_codename}"')
-        sys.exit(0)
+        cli.print_version()
 
     cli = UEVaultManagerCLI(override_config=args.config_file, api_timeout=args.api_timeout)
 
     start_in_edit_mode = str_to_bool(cli.core.uevmlfs.config.get('UEVaultManager', 'start_in_edit_mode', fallback=False))
 
     if not start_in_edit_mode and (not args.subparser_name or args.full_help):
         cli.print_help(args=args, parser=parser)
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/core.py` & `UEVaultManager-1.6.3/UEVaultManager/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from UEVaultManager.models.json_manifest import JSONManifest
 from UEVaultManager.models.manifest import Manifest
 from UEVaultManager.tkgui.modules.functions import box_message
 from UEVaultManager.utils.cli import check_and_create_path
 from UEVaultManager.utils.egl_crypt import decrypt_epic_data
 from UEVaultManager.utils.env import is_windows_mac_or_pyi
 
-
 # The heading dict contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
 
 # ToDo: instead of true/false return values for success/failure actually raise an exception that the CLI/GUI
 #  can handle to give the user more details. (Not required yet since there's no GUI so log output is fine)
 
 
 class AppCore:
@@ -117,43 +116,39 @@
         self.thread_executor_must_stop = False
         self.engine_version_for_obsolete_assets = '4.26'
 
     def setup_assets_logging(self) -> None:
         """
         Setup logging for ignored, not found and bad data assets
         """
+
+        def create_logger(logger_name: str, filename_log: str) -> None:
+            """
+            Create a logger for ignored, not found and bad data assets
+            :param logger_name:   
+            :param filename_log: 
+            :return: 
+            """
+            filename_log = filename_log.replace('~/.config', self.uevmlfs.path)
+            if check_and_create_path(filename_log):
+                handler = logging.FileHandler(filename_log, mode='w')
+                handler.setFormatter(formatter)
+                logger = logging.Logger(logger_name, 'INFO')
+                logger.addHandler(handler)
+                logger.info(message)
+
         formatter = logging.Formatter('%(message)s')
         message = f"-----\n{datetime.now().strftime(self.default_datetime_format)} Log Started\n-----\n"
 
-        if self.ignored_assets_filename_log != '':
-            ignored_assets_filename_log = self.ignored_assets_filename_log.replace('~/.config', self.uevmlfs.path)
-            if check_and_create_path(ignored_assets_filename_log):
-                ignored_assets_handler = logging.FileHandler(ignored_assets_filename_log, mode='w')
-                ignored_assets_handler.setFormatter(formatter)
-                self.ignored_logger = logging.Logger('IgnoredAssets', 'INFO')
-                self.ignored_logger.addHandler(ignored_assets_handler)
-                self.ignored_logger.info(message)
-
-        if self.notfound_assets_filename_log != '':
-            notfound_assets_filename_log = self.notfound_assets_filename_log.replace('~/.config', self.uevmlfs.path)
-            if check_and_create_path(notfound_assets_filename_log):
-                notfound_assets_handler = logging.FileHandler(notfound_assets_filename_log, mode='w')
-                notfound_assets_handler.setFormatter(formatter)
-                self.notfound_logger = logging.Logger('NotFoundAssets', 'INFO')
-                self.notfound_logger.addHandler(notfound_assets_handler)
-                self.notfound_logger.info(message)
-
-        if self.bad_data_assets_filename_log != '':
-            bad_data_assets_filename_log = self.bad_data_assets_filename_log.replace('~/.config', self.uevmlfs.path)
-            if check_and_create_path(bad_data_assets_filename_log):
-                bad_data_assets_handler = logging.FileHandler(bad_data_assets_filename_log, mode='w')
-                bad_data_assets_handler.setFormatter(formatter)
-                self.bad_data_logger = logging.Logger('BadDataAssets', 'INFO')
-                self.bad_data_logger.addHandler(bad_data_assets_handler)
-                self.bad_data_logger.info(message)
+        if self.ignored_assets_filename_log:
+            create_logger('IgnoredAssets', self.ignored_assets_filename_log)
+        if self.notfound_assets_filename_log:
+            create_logger('NotFoundAssets', self.notfound_assets_filename_log)
+        if self.bad_data_assets_filename_log:
+            create_logger('BadDataAssets', self.bad_data_assets_filename_log)
 
     def auth_sid(self, sid) -> str:
         """
         Handles getting an exchange code from an id
         :param sid: session id
         :return: exchange code
         """
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.6.3/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.6.3/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.6.3/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.6.3/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.6.3/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.6.3/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.6.3/UEVaultManager/lfs/windows_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 # coding=utf-8
 """
 Windows specific helper functions for registry access.
 """
 import ctypes
 import logging
+# noinspection PyCompatibility
+# will be added in the future 3.12 release
 import winreg
 
 _logger = logging.getLogger('WindowsHelpers')
 
 HKEY_CURRENT_USER = winreg.HKEY_CURRENT_USER
 HKEY_LOCAL_MACHINE = winreg.HKEY_LOCAL_MACHINE
 TYPE_STRING = winreg.REG_SZ
 TYPE_DWORD = winreg.REG_DWORD
 
 
-def query_registry_value(hive, key, value):
+def query_registry_value(hive, key, value) -> str:
+    """
+    Query a registry value.
+    :param hive:
+    :param key:
+    :param value:
+    :return: value data as string
+    """
     ret = None
     try:
         k = winreg.OpenKey(hive, key, reserved=0, access=winreg.KEY_READ)
     except FileNotFoundError:
         _logger.debug(f'Registry key "{key}" not found')
     else:
         try:
@@ -26,15 +35,22 @@
         except FileNotFoundError:
             _logger.debug(f'Registry value "{key}":"{value}" not found')
         winreg.CloseKey(k)
 
     return ret
 
 
-def list_registry_values(hive, key, use_32bit_view=False):
+def list_registry_values(hive, key, use_32bit_view=False) -> list:
+    """
+    List all values in a registry key.
+    :param hive:
+    :param key:
+    :param use_32bit_view:
+    :return: list of tuples (value_name, value_data, value_type)
+    """
     ret = []
 
     access = winreg.KEY_READ
     if use_32bit_view:
         access |= winreg.KEY_WOW64_32KEY
 
     try:
@@ -49,15 +65,22 @@
             except OSError:
                 break
             idx += 1
 
     return ret
 
 
-def remove_registry_value(hive, key, value, use_32bit_view=False):
+def remove_registry_value(hive, key, value, use_32bit_view=False) -> None:
+    """
+    Remove a registry value.
+    :param hive:
+    :param key:
+    :param value:
+    :param use_32bit_view:
+    """
     access = winreg.KEY_ALL_ACCESS
     if use_32bit_view:
         access |= winreg.KEY_WOW64_32KEY
 
     try:
         k = winreg.OpenKey(hive, key, reserved=0, access=access)
     except FileNotFoundError:
@@ -66,15 +89,24 @@
         try:
             winreg.DeleteValue(k, value)
         except Exception as error:
             _logger.debug(f'Deleting "{key}":"{value}" failed with {repr(error)}')
         winreg.CloseKey(k)
 
 
-def set_registry_value(hive, key, value, data, reg_type=winreg.REG_SZ, use_32bit_view=False):
+def set_registry_value(hive, key, value, data, reg_type=winreg.REG_SZ, use_32bit_view=False) -> None:
+    """
+    Set a registry value.
+    :param hive:
+    :param key:
+    :param value:
+    :param data:
+    :param reg_type:
+    :param use_32bit_view:
+    """
     access = winreg.KEY_ALL_ACCESS
     if use_32bit_view:
         access |= winreg.KEY_WOW64_32KEY
 
     try:
         k = winreg.CreateKeyEx(hive, key, reserved=0, access=access)
     except Exception as error:
@@ -84,14 +116,17 @@
             winreg.SetValueEx(k, value, 0, reg_type, data)
         except Exception as error:
             _logger.debug(f'Setting "{key}":"{value}" to "{data}" failed with {repr(error)}')
         winreg.CloseKey(k)
 
 
 def double_clicked() -> bool:
+    """
+    Check if the application was started by a double click
+    """
     # Thanks https://stackoverflow.com/a/55476145
 
     # Load kernel32.dll
     kernel32 = ctypes.WinDLL('kernel32', use_last_error=True)
     # Create an array to store the processes in.  This doesn't actually need to
     # be large enough to store the whole process list since GetConsoleProcessList()
     # just returns the number of processes if the array is too small.
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/models/chunk.py` & `UEVaultManager-1.6.3/UEVaultManager/models/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         return self.stored_as & 0x1
 
     @classmethod
     def read_buffer(cls, data):
         _sio = BytesIO(data)
         return cls.read(_sio)
 
+    # noinspection DuplicatedCode
     @classmethod
     def read(cls, bio):
         head_start = bio.tell()
 
         if struct.unpack('<I', bio.read(4))[0] != cls.header_magic:
             raise ValueError('Chunk magic doesn\'t match!')
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/models/config.py` & `UEVaultManager-1.6.3/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/models/csv.py` & `UEVaultManager-1.6.3/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/models/downloading.py` & `UEVaultManager-1.6.3/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/models/egl.py` & `UEVaultManager-1.6.3/UEVaultManager/models/egl.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 # coding=utf-8
+"""
+implementation for:
+- EGLManifest: EGL Manifest 
+"""
 from copy import deepcopy
 
 from UEVaultManager.utils.cli import str_to_bool
 
 _template = {
-    'AppCategories'         : ['public', 'games', 'applications'],
-    'AppName'               : '',
-    'AppVersionString'      : '',
-    'BaseURLs'              : [],
-    'BuildLabel'            : '',
-    'CatalogItemId'         : '',
-    'CatalogNamespace'      : '',
-    'ChunkDbs'              : [],
-    'CompatibleApps'        : [],
-    'DisplayName'           : '',
-    'FormatVersion'         : 0,
-    'FullAppName'           : '',
-    'HostInstallationGuid'  : '',
-    'InstallComponents'     : [],
-    'InstallLocation'       : '',
-    'InstallSessionId'      : '',
-    'InstallSize'           : 0,
-    'InstallTags'           : [],
-    'InstallationGuid'      : '',
-    'LaunchCommand'         : '',
-    'LaunchExecutable'      : '',
-    'MainGameAppName'       : '',
-    'MainWindowProcessName' : '',
+    'AppCategories': ['public', 'games', 'applications'],
+    'AppName': '',
+    'AppVersionString': '',
+    'BaseURLs': [],
+    'BuildLabel': '',
+    'CatalogItemId': '',
+    'CatalogNamespace': '',
+    'ChunkDbs': [],
+    'CompatibleApps': [],
+    'DisplayName': '',
+    'FormatVersion': 0,
+    'FullAppName': '',
+    'HostInstallationGuid': '',
+    'InstallComponents': [],
+    'InstallLocation': '',
+    'InstallSessionId': '',
+    'InstallSize': 0,
+    'InstallTags': [],
+    'InstallationGuid': '',
+    'LaunchCommand': '',
+    'LaunchExecutable': '',
+    'MainGameAppName': '',
+    'MainWindowProcessName': '',
     'MandatoryAppFolderName': '',
-    'ManifestLocation'      : '',
-    'OwnershipToken'        : '',
-    'PrereqIds'             : [],
-    'ProcessNames'          : [],
-    'StagingLocation'       : '',
-    'TechnicalType'         : '',
-    'VaultThumbnailUrl'     : '',
-    'VaultTitleText'        : '',
-    'bCanRunOffline'        : True,
-    'bIsApplication'        : True,
-    'bIsExecutable'         : True,
-    'bIsIncompleteInstall'  : False,
-    'bIsManaged'            : False,
-    'bNeedsValidation'      : False,
-    'bRequiresAuth'         : True
+    'ManifestLocation': '',
+    'OwnershipToken': '',
+    'PrereqIds': [],
+    'ProcessNames': [],
+    'StagingLocation': '',
+    'TechnicalType': '',
+    'VaultThumbnailUrl': '',
+    'VaultTitleText': '',
+    'bCanRunOffline': True,
+    'bIsApplication': True,
+    'bIsExecutable': True,
+    'bIsIncompleteInstall': False,
+    'bIsManaged': False,
+    'bNeedsValidation': False,
+    'bRequiresAuth': True
 }
 
 
 class EGLManifest:
+    """
+    EGL Manifest
+    """
+
     def __init__(self):
         self.app_name = None
         self.app_version_string = None
         self.base_urls = None
         self.build_label = None
         self.catalog_item_id = None
         self.namespace = None
@@ -69,27 +77,33 @@
         self.can_run_offline = None
         self.is_incomplete_install = None
         self.needs_validation = None
 
         self.remainder = dict()
 
     @classmethod
-    def from_json(cls, json: dict):
+    def from_json(cls, json: dict) -> 'EGLManifest':
+        """
+        Create EGLManifest from json
+        :param json: json data
+        :return: EGLManifest
+        """
         json = deepcopy(json)
         tmp = cls()
         tmp.app_name = json.pop('AppName')
         tmp.app_version_string = json.pop('AppVersionString', None)
         tmp.base_urls = json.pop('BaseURLs', list())
         tmp.build_label = json.pop('BuildLabel', '')
         tmp.catalog_item_id = json.pop('CatalogItemId', '')
         tmp.namespace = json.pop('CatalogNamespace', '')
         tmp.display_name = json.pop('DisplayName', '')
         tmp.install_location = json.pop('InstallLocation', '')
         tmp.install_size = json.pop('InstallSize', 0)
         tmp.install_tags = json.pop('InstallTags', [])
+        # noinspection DuplicatedCode
         tmp.installation_guid = json.pop('InstallationGuid', '')
         tmp.launch_command = json.pop('LaunchCommand', '')
         tmp.executable = json.pop('LaunchExecutable', '')
         tmp.main_game_appname = json.pop('MainGameAppName', '')
         tmp.app_folder_name = json.pop('MandatoryAppFolderName', '')
         tmp.manifest_location = json.pop('ManifestLocation', '')
         tmp.ownership_token = str_to_bool(json.pop('OwnershipToken', 'False'))
@@ -97,24 +111,30 @@
         tmp.can_run_offline = json.pop('bCanRunOffline', True)
         tmp.is_incomplete_install = json.pop('bIsIncompleteInstall', False)
         tmp.needs_validation = json.pop('bNeedsValidation', False)
         tmp.remainder = json.copy()
         return tmp
 
     def to_json(self) -> dict:
+        """
+        Convert EGLManifest to json
+        :return: json data
+        """
         out = _template.copy()
         out.update(self.remainder)
+        # noinspection DuplicatedCode
         out['AppName'] = self.app_name
         out['AppVersionString'] = self.app_version_string
         out['BaseURLs'] = self.base_urls
         out['BuildLabel'] = self.build_label
         out['CatalogItemId'] = self.catalog_item_id
         out['CatalogNamespace'] = self.namespace
         out['DisplayName'] = self.display_name
         out['InstallLocation'] = self.install_location
+        # noinspection DuplicatedCode
         out['InstallSize'] = self.install_size
         out['InstallTags'] = self.install_tags
         out['InstallationGuid'] = self.installation_guid
         out['LaunchCommand'] = self.launch_command
         out['LaunchExecutable'] = self.executable
         out['MainGameAppName'] = self.main_game_appname
         out['MandatoryAppFolderName'] = self.app_folder_name
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.6.3/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/models/manifest.py` & `UEVaultManager-1.6.3/UEVaultManager/models/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,14 +257,15 @@
         s.update(self.app_name.encode('utf-8'))
         s.update(self.build_version.encode('utf-8'))
         s.update(self.launch_exe.encode('utf-8'))
         s.update(self.launch_command.encode('utf-8'))
         self._build_id = b64encode(s.digest()).decode('ascii').replace('+', '-').replace('/', '_').replace('=', '')
         return self._build_id
 
+    # noinspection DuplicatedCode
     @classmethod
     def read(cls, bio):
         _meta = cls()
 
         _meta.meta_size = struct.unpack('<I', bio.read(4))[0]
         _meta.data_version = struct.unpack('B', bio.read(1))[0]
         # Usually same as manifest version, but can be different
@@ -396,14 +397,15 @@
                 self.guid_int_map[chunk.guid_num] = index
 
         index = self.guid_int_map.get(guid_int, None)
         if index is None:
             raise ValueError(f'Invalid GUID! {hex(guid_int)}')
         return self.elements[index]
 
+    # noinspection DuplicatedCode
     @classmethod
     def read(cls, bio, manifest_version=18):
         cdl_start = bio.tell()
         _cdl = cls()
         _cdl._manifest_version = manifest_version
 
         _cdl.size = struct.unpack('<I', bio.read(4))[0]
@@ -546,14 +548,15 @@
                 self._path_map[fm.filename] = index
 
         index = self._path_map.get(path, None)
         if index is None:
             raise ValueError(f'Invalid path! {path}')
         return self.elements[index]
 
+    # noinspection DuplicatedCode
     @classmethod
     def read(cls, bio):
         fml_start = bio.tell()
         _fml = cls()
         _fml.size = struct.unpack('<I', bio.read(4))[0]
         _fml.version = struct.unpack('B', bio.read(1))[0]
         _fml.count = struct.unpack('<I', bio.read(4))[0]
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files 6% similar despite different names*

```diff
@@ -691,46 +691,20 @@
         """
         Quick edit the content some cells of the selected row.
         :param quick_edit_frame: The frame to display the cell content preview in.
         :param row: The row index of the selected cell.
         """
         if row is None or row >= len(self.model.df) or quick_edit_frame is None:
             return
-        # Url
-        col = self.model.df.columns.get_loc('Url')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Url', content=value, row=row, col=col)
-        # Comment
-        col = self.model.df.columns.get_loc('Comment')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Comment', content=value, row=row, col=col)
-        # Stars
-        col = self.model.df.columns.get_loc('Stars')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Stars', content=value, row=row, col=col)
-        # Test
-        col = self.model.df.columns.get_loc('Test result')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Test result', content=value, row=row, col=col)
-        # Must buy
-        col = self.model.df.columns.get_loc('Must buy')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Must buy', label='', content=value, row=row, col=col)
-        # Alternative
-        col = self.model.df.columns.get_loc('Alternative')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Alternative', content=value, row=row, col=col)
-        # Installed
-        col = self.model.df.columns.get_loc('Installed folder')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Installed folder', content=value, row=row, col=col)
-        # Origin
-        col = self.model.df.columns.get_loc('Origin')
-        value = self.model.getValueAt(row=row, col=col)
-        quick_edit_frame.set_child_values(tag='Origin', content=value, row=row, col=col)
+
+        column_names = ['Url', 'Comment', 'Stars', 'Test result', 'Must buy', 'Alternative', 'Installed folder', 'Origin']
+        for col_name in column_names:
+            col = self.model.df.columns.get_loc(col_name)
+            value = self.model.getValueAt(row=row, col=col)
+            quick_edit_frame.set_child_values(tag=col_name, content=value, row=row, col=col)
 
     @staticmethod
     def quick_edit(quick_edit_frame: TaggedLabelFrame = None) -> None:
         """
         Resets the cell content preview.
         :param quick_edit_frame: The frame to reset the cell content preview in.
         """
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from termcolor import colored
 
 import UEVaultManager.tkgui.modules.functions_no_deps as gui_fn
 from UEVaultManager.lfs.utils import clean_filename
 from UEVaultManager.models.config import AppConf
 
-
 # NOTE : we can't import the following modules here because of circular dependencies
 # UEVaultManager.tkgui.modules.functions_no_deps
 
 
 def log(msg: str) -> None:
     """
     Print a message to the console
@@ -170,28 +169,31 @@
     # use properties for keeping transparent access to these properties
     debug_mode = property(get_debug_mode, set_debug_mode)
     never_update_data_files = property(get_never_update_data_files, set_never_update_data_files)
     reopen_last_file = property(get_reopen_last_file, set_reopen_last_file)
     use_colors_for_data = property(get_use_colors_for_data, set_use_colors_for_data)
     image_cache_max_time = property(get_image_cache_max_time, set_image_cache_max_time)
     last_opened_file = property(get_last_opened_file, set_last_opened_file)
+
     # following vars are not set as properties to avoid storing absolute paths in the config file
     # getter and setter could be used to store relative paths
     # cache_folder = property(get_cache_folder, set_cache_folder)
     # results_folder = property(get_results_folder, set_results_folder)
 
     def init_gui_config_file(self, config_file: str = '') -> None:
         """
         Initialize the config file for the gui
         :param config_file: the path to the config file to use
         """
         if config_path := os.environ.get('XDG_CONFIG_HOME'):
             self.path = os.path.join(config_path, 'UEVaultManager')
         else:
             self.path = os.path.expanduser('~/.config/UEVaultManager')
+        if not os.path.isdir(self.path):
+            os.makedirs(self.path)
         if config_file:
             if os.path.exists(config_file):
                 self.config_path = os.path.abspath(config_file)
             else:
                 self.config_path = os.path.join(self.path, clean_filename(config_file))
             log(f'UEVMGui is using non-default config file "{self.config_path}"')
         else:
@@ -202,53 +204,60 @@
             self.config.read(self.config_path)
         except Exception as error:
             log('Unable to read configuration file, please ensure that file is valid! '
                 f'(Error: {repr(error)})')
             log('Continuing with blank config in safe-mode...')
             self.config.read_only = True
 
-        # make sure "UEVaultManager" section exists
+        config_defaults = {
+            'debug_mode': {
+                'comment': 'Set to True to print debug information (GUI related only',
+                'value': 'False'
+            },
+            'never_update_data_files': {
+                'comment': 'Set to True to speed the update process by not updating the metadata files. FOR TESTING ONLY',
+                'value': 'False'
+            },
+            'reopen_last_file': {
+                'comment': 'Set to True to re-open the last file at startup if no input file is given',
+                'value': 'True'
+            },
+            'use_colors_for_data': {
+                'comment': 'Set to True to enable cell coloring depending on its content.It could slow down data and display refreshing',
+                'value': 'True'
+            },
+            'last_opened_file': {
+                'comment': 'File name of the last opened file',
+                'value': ''
+            },
+            'image_cache_max_time': {
+                'comment': 'Delay in seconds when image cache will be invalidated. Default value represent 15 days',
+                'value': str(60 * 60 * 24 * 15)
+            },
+            'cache_folder': {
+                'comment': 'Folder (relative or absolute) to store cached data for assets (mainly preview images)',
+                'value': '../../../cache'
+            },
+            'results_folder': {
+                'comment': 'Folder (relative or absolute) to store result files to read and save data from',
+                'value': '../../../results'
+            },
+        }
+
         has_changed = False
         if 'UEVaultManager' not in self.config:
             self.config.add_section('UEVaultManager')
             has_changed = True
-        if not self.config.has_option('UEVaultManager', 'debug_mode'):
-            self.config.set('UEVaultManager', '; Set to True to print debug information (GUI related only)')
-            self.config.set('UEVaultManager', 'debug_mode', 'False')
-            has_changed = True
-        if not self.config.has_option('UEVaultManager', 'never_update_data_files'):
-            self.config.set('UEVaultManager', '; Set to True to speed the update process by not updating the metadata files. FOR TESTING ONLY')
-            self.config.set('UEVaultManager', 'never_update_data_files', 'False')
-            has_changed = True
-        if not self.config.has_option('UEVaultManager', 'reopen_last_file'):
-            self.config.set('UEVaultManager', '; Set to True to re-open the last file at startup if no input file is given')
-            self.config.set('UEVaultManager', 'reopen_last_file', 'True')
-            has_changed = True
-        if not self.config.has_option('UEVaultManager', 'use_colors_for_data'):
-            self.config.set(
-                'UEVaultManager', '; Set to True to enable cell coloring depending on its content.It could slow down data and display refreshing'
-            )
-            self.config.set('UEVaultManager', 'use_colors_for_data', 'True')
-            has_changed = True
-        if not self.config.has_option('UEVaultManager', 'last_opened_file'):
-            self.config.set('UEVaultManager', '; Last opened file name')
-            self.config.set('UEVaultManager', 'last_opened_file', '')
-            has_changed = True
-        if not self.config.has_option('UEVaultManager', 'image_cache_max_time'):
-            self.config.set('UEVaultManager', '; Delay in seconds when image cache will be invalidated. Default value represent 15 days')
-            self.config.set('UEVaultManager', 'image_cache_max_time', str(60 * 60 * 24 * 15))
-            has_changed = True
-        if not self.config.has_option('UEVaultManager', 'cache_folder'):
-            self.config.set('UEVaultManager', '; Folder (relative or absolute) to store cached data for assets (mainly preview images)')
-            self.config.set('UEVaultManager', 'cache_folder', '../../../cache')
-            has_changed = True
-        if not self.config.has_option('UEVaultManager', 'results_folder'):
-            self.config.set('UEVaultManager', '; Folder (relative or absolute) to store result files to read and save data from')
-            self.config.set('UEVaultManager', 'results_folder', '../../../results')
-            has_changed = True
+
+        for option, content in config_defaults.items():
+            if not self.config.has_option('UEVaultManager', option):
+                self.config.set('UEVaultManager', f';{content["comment"]}')
+                self.config.set('UEVaultManager', option, content['value'])
+                has_changed = True
+
         if has_changed:
             self.save_config_file(save_config_var=False)
 
     def store_config_properties(self) -> None:
         """
         store the properties in the config file
         """
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -722,34 +722,36 @@
 
     def next_asset(self) -> None:
         """
         Move to the next asset in the table
         """
         self.editable_table.move_to_next_record()
 
+    # noinspection DuplicatedCode
     def toggle_controls_pane(self) -> None:
         """
-        Toggle the visibility of the controls pane on the right side of the table
+        Toggle the visibility of the controls pane
         """
-        # Toggle visibility of filter controls frame
+        # noinspection DuplicatedCode
         if self.control_frame.winfo_ismapped():
             self.control_frame.pack_forget()
             self.toolbar_frame.btn_toggle_controls.config(text='Show Control')
             self.toolbar_frame.btn_toggle_options.config(state=tk.NORMAL)
 
         else:
             self.control_frame.pack(side=tk.RIGHT, fill=tk.BOTH)
             self.toolbar_frame.btn_toggle_controls.config(text='Hide Control')
             self.toolbar_frame.btn_toggle_options.config(state=tk.DISABLED)
 
+    # noinspection DuplicatedCode
     def toggle_options_pane(self) -> None:
         """
-        Toggle the visibility of the Options pane on the right side of the table
+        Toggle the visibility of the Options pane
         """
-        # Toggle visibility of filter controls frame
+        # noinspection DuplicatedCode
         if self.options_frame.winfo_ismapped():
             self.options_frame.pack_forget()
             self.toolbar_frame.btn_toggle_options.config(text='Show Options')
             self.toolbar_frame.btn_toggle_controls.config(state=tk.NORMAL)
         else:
             self.options_frame.pack(side=tk.RIGHT, fill=tk.BOTH)
             self.toolbar_frame.btn_toggle_options.config(text='Hide Options')
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/functions_no_deps.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/functions_no_deps.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,18 +85,23 @@
 def set_toolbar_style(tk_window) -> None:
     """
     Remove the minimize and maximize buttons from a tkinter window.
     This version is compatible with Windows AND Non-windows OS
     # see https://stackoverflow.com/questions/2969870/removing-minimize-maximize-buttons-in-tkinter
     :param tk_window: the tkinter window
     """
-    set_window_pos = ct.windll.user32.SetWindowPos
-    set_window_long = ct.windll.user32.SetWindowLongPtrW
-    get_window_long = ct.windll.user32.GetWindowLongPtrW
-    get_parent = ct.windll.user32.GetParent
+    try:
+        set_window_pos = ct.windll.user32.SetWindowPos
+        set_window_long = ct.windll.user32.SetWindowLongPtrW
+        get_window_long = ct.windll.user32.GetWindowLongPtrW
+        get_parent = ct.windll.user32.GetParent
+    except AttributeError:
+        # Non-windows OS
+        print('Non-windows OS detected. No need to remove the minimize and maximize buttons from the window.')
+        return
     # Identifiers
     gwl_style = -16
     ws_minimizebox = 131072
     ws_maximizebox = 65536
     swp_nozorder = 4
     swp_nomove = 2
     swp_nosize = 1
@@ -127,14 +132,17 @@
 
 
 def create_empty_file(file_path: str) -> None:
     """
     Create an empty file
     :param file_path: the path of the file to create
     """
+    path = os.path.dirname(file_path)
+    if not os.path.exists(path):
+        os.makedirs(path)
     open(file_path, 'a').close()
 
 
 def convert_to_bool(value) -> bool:
     """
     Convert a value to a boolean
     :param value: the value to convert. If the value is not a boolean, it will be converted to a string and then to a boolean.
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.6.3/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.6.3/UEVaultManager/utils/aliasing.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,22 @@
 
 
 def _filter(local_input):
     return ''.join(char for char in local_input if char in allowed_characters)
 
 
 def generate_aliases(game_name, item_folder=None, split_words=True, app_name=None):
+    """
+    Generate aliases for a game name.
+    :param game_name:
+    :param item_folder:
+    :param split_words:
+    :param app_name:
+    :return:
+    """
     # normalise and split name, then filter for legal characters
     game_parts = [_filter(p) for p in game_name.lower().split()]
     # filter out empty parts
     game_parts = [p for p in game_parts if p]
 
     _aliases = [game_name.lower().strip(), ' '.join(game_parts), ''.join(game_parts), ''.join(roman.get(p, p) for p in game_parts)]
 
@@ -70,15 +78,15 @@
         _aliases.extend(generate_aliases(game_name.replace('-', ' ')))
     # include folder name for alternative short forms
     if item_folder:
         _aliases.extend(generate_aliases(item_folder, split_words=False))
     # include lowercase version of app name in aliases
     if app_name:
         _aliases.append(app_name.lower())
-    # include initialisms
+    # noinspection DuplicatedCode
     if len(game_parts) > 1:
         _aliases.append(''.join(p[0] for p in game_parts))
         _aliases.append(''.join(p[0] if p not in roman else p for p in game_parts))
         _aliases.append(''.join(roman.get(p, p[0]) for p in game_parts))
     # Attempt to address cases like "Battlefront" being shortened to "BF"
     if split_words:
         new_game_parts = []
@@ -87,14 +95,15 @@
                 word_middle = word[3:-3]
                 word_split = ' f'.join(word_middle.split('f'))
                 word = word[0:3] + word_split + word[-3:]
                 new_game_parts.extend(word.split())
             else:
                 new_game_parts.append(word)
 
+        # noinspection DuplicatedCode
         if len(new_game_parts) > 1:
             _aliases.append(''.join(p[0] for p in new_game_parts))
             _aliases.append(''.join(p[0] if p not in roman else p for p in new_game_parts))
             _aliases.append(''.join(roman.get(p, p[0]) for p in new_game_parts))
 
     # return sorted uniques
     return sorted(set(_aliases))
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/utils/cli.py` & `UEVaultManager-1.6.3/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.6.3/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.6.3/UEVaultManager/utils/egl_crypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 You should practically never roll your own crypto like this.
 In this case it's just unimportant enough since all it needs to do is decrypt some data from the EGL config file.
 """
 
 import locale
 
+# noinspection DuplicatedCode
 s_box = (
     0x63, 0x7C, 0x77, 0x7B, 0xF2, 0x6B, 0x6F, 0xC5, 0x30, 0x01, 0x67, 0x2B, 0xFE, 0xD7, 0xAB, 0x76,
     0xCA, 0x82, 0xC9, 0x7D, 0xFA, 0x59, 0x47, 0xF0, 0xAD, 0xD4, 0xA2, 0xAF, 0x9C, 0xA4, 0x72, 0xC0,
     0xB7, 0xFD, 0x93, 0x26, 0x36, 0x3F, 0xF7, 0xCC, 0x34, 0xA5, 0xE5, 0xF1, 0x71, 0xD8, 0x31, 0x15,
     0x04, 0xC7, 0x23, 0xC3, 0x18, 0x96, 0x05, 0x9A, 0x07, 0x12, 0x80, 0xE2, 0xEB, 0x27, 0xB2, 0x75,
     0x09, 0x83, 0x2C, 0x1A, 0x1B, 0x6E, 0x5A, 0xA0, 0x52, 0x3B, 0xD6, 0xB3, 0x29, 0xE3, 0x2F, 0x84,
     0x53, 0xD1, 0x00, 0xED, 0x20, 0xFC, 0xB1, 0x5B, 0x6A, 0xCB, 0xBE, 0x39, 0x4A, 0x4C, 0x58, 0xCF,
@@ -24,14 +25,15 @@
     0xE7, 0xC8, 0x37, 0x6D, 0x8D, 0xD5, 0x4E, 0xA9, 0x6C, 0x56, 0xF4, 0xEA, 0x65, 0x7A, 0xAE, 0x08,
     0xBA, 0x78, 0x25, 0x2E, 0x1C, 0xA6, 0xB4, 0xC6, 0xE8, 0xDD, 0x74, 0x1F, 0x4B, 0xBD, 0x8B, 0x8A,
     0x70, 0x3E, 0xB5, 0x66, 0x48, 0x03, 0xF6, 0x0E, 0x61, 0x35, 0x57, 0xB9, 0x86, 0xC1, 0x1D, 0x9E,
     0xE1, 0xF8, 0x98, 0x11, 0x69, 0xD9, 0x8E, 0x94, 0x9B, 0x1E, 0x87, 0xE9, 0xCE, 0x55, 0x28, 0xDF,
     0x8C, 0xA1, 0x89, 0x0D, 0xBF, 0xE6, 0x42, 0x68, 0x41, 0x99, 0x2D, 0x0F, 0xB0, 0x54, 0xBB, 0x16,
 )
 
+# noinspection DuplicatedCode
 inv_s_box = (
     0x52, 0x09, 0x6A, 0xD5, 0x30, 0x36, 0xA5, 0x38, 0xBF, 0x40, 0xA3, 0x9E, 0x81, 0xF3, 0xD7, 0xFB,
     0x7C, 0xE3, 0x39, 0x82, 0x9B, 0x2F, 0xFF, 0x87, 0x34, 0x8E, 0x43, 0x44, 0xC4, 0xDE, 0xE9, 0xCB,
     0x54, 0x7B, 0x94, 0x32, 0xA6, 0xC2, 0x23, 0x3D, 0xEE, 0x4C, 0x95, 0x0B, 0x42, 0xFA, 0xC3, 0x4E,
     0x08, 0x2E, 0xA1, 0x66, 0x28, 0xD9, 0x24, 0xB2, 0x76, 0x5B, 0xA2, 0x49, 0x6D, 0x8B, 0xD1, 0x25,
     0x72, 0xF8, 0xF6, 0x64, 0x86, 0x68, 0x98, 0x16, 0xD4, 0xA4, 0x5C, 0xCC, 0x5D, 0x65, 0xB6, 0x92,
     0x6C, 0x70, 0x48, 0x50, 0xFD, 0xED, 0xB9, 0xDA, 0x5E, 0x15, 0x46, 0x57, 0xA7, 0x8D, 0x9D, 0x84,
@@ -56,20 +58,22 @@
 
 def inv_sub_bytes(s):
     for i in range(4):
         for j in range(4):
             s[i][j] = inv_s_box[s[i][j]]
 
 
+# noinspection DuplicatedCode
 def shift_rows(s):
     s[0][1], s[1][1], s[2][1], s[3][1] = s[1][1], s[2][1], s[3][1], s[0][1]
     s[0][2], s[1][2], s[2][2], s[3][2] = s[2][2], s[3][2], s[0][2], s[1][2]
     s[0][3], s[1][3], s[2][3], s[3][3] = s[3][3], s[0][3], s[1][3], s[2][3]
 
 
+# noinspection DuplicatedCode
 def inv_shift_rows(s):
     s[0][1], s[1][1], s[2][1], s[3][1] = s[3][1], s[0][1], s[1][1], s[2][1]
     s[0][2], s[1][2], s[2][2], s[3][2] = s[2][2], s[3][2], s[0][2], s[1][2]
     s[0][3], s[1][3], s[2][3], s[3][3] = s[1][3], s[2][3], s[3][3], s[0][3]
 
 
 def add_round_key(s, k):
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.6.3/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.6.3/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.6.3/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.2
+Version: 1.6.3
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.6.2 ## codename: Virgo+2
+ UEVaultManager ## version:1.6.3 ## codename: Virgo+3
```

### Comparing `UEVaultManager-1.6.2/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.6.3/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.2/setup.py` & `UEVaultManager-1.6.3/setup.py`

 * *Files identical despite different names*

