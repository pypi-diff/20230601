# Comparing `tmp/UEVaultManager-1.6.5.tar.gz` & `tmp/UEVaultManager-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.6.5.tar", last modified: Thu Jun  1 09:33:13 2023, max compression
+gzip compressed data, was "UEVaultManager-1.6.6.tar", last modified: Thu Jun  1 11:22:23 2023, max compression
```

## Comparing `UEVaultManager-1.6.5.tar` & `UEVaultManager-1.6.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.942972 UEVaultManager-1.6.5/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.5/LICENSE
--rw-rw-rw-   0        0        0     6127 2023-06-01 09:33:13.942972 UEVaultManager-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.906973 UEVaultManager-1.6.5/UEVaultManager/
--rw-rw-rw-   0        0        0      778 2023-06-01 09:31:58.000000 UEVaultManager-1.6.5/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.911974 UEVaultManager-1.6.5/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.5/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-25 16:36:39.000000 UEVaultManager-1.6.5/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.5/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.914974 UEVaultManager-1.6.5/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.5/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.6.5/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.5/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.6.5/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    73048 2023-06-01 09:13:57.000000 UEVaultManager-1.6.5/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    46806 2023-06-01 06:50:17.000000 UEVaultManager-1.6.5/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.914974 UEVaultManager-1.6.5/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.5/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.916973 UEVaultManager-1.6.5/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.5/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.6.5/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.5/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.919973 UEVaultManager-1.6.5/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.5/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.5/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.5/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23585 2023-05-26 09:04:11.000000 UEVaultManager-1.6.5/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.5/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3927 2023-06-01 07:37:43.000000 UEVaultManager-1.6.5/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.925972 UEVaultManager-1.6.5/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.5/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     5942 2023-06-01 07:24:48.000000 UEVaultManager-1.6.5/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.6.5/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.5/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.5/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.5/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.6.5/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.5/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.5/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30610 2023-06-01 07:29:35.000000 UEVaultManager-1.6.5/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.926972 UEVaultManager-1.6.5/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1709 2023-06-01 09:11:19.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.937972 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    32497 2023-06-01 06:46:43.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0    12788 2023-06-01 09:12:21.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    43199 2023-06-01 07:25:24.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0     9697 2023-05-31 17:11:24.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     7214 2023-06-01 09:29:41.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/functions_no_deps.py
--rw-rw-rw-   0        0        0     2631 2023-05-31 15:29:53.000000 UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.941972 UEVaultManager-1.6.5/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.5/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3691 2023-06-01 07:18:12.000000 UEVaultManager-1.6.5/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.6.5/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.5/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.6.5/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.5/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.5/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.5/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:33:13.910975 UEVaultManager-1.6.5/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6127 2023-06-01 09:33:13.000000 UEVaultManager-1.6.5/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-06-01 09:33:13.000000 UEVaultManager-1.6.5/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:33:13.000000 UEVaultManager-1.6.5/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-01 09:33:13.000000 UEVaultManager-1.6.5/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      300 2023-06-01 09:33:13.000000 UEVaultManager-1.6.5/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-01 09:33:13.000000 UEVaultManager-1.6.5/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:33:13.943972 UEVaultManager-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.836544 UEVaultManager-1.6.6/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0     6127 2023-06-01 11:22:23.836544 UEVaultManager-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.795542 UEVaultManager-1.6.6/UEVaultManager/
+-rw-rw-rw-   0        0        0      778 2023-06-01 11:22:08.000000 UEVaultManager-1.6.6/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.801543 UEVaultManager-1.6.6/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-25 16:36:39.000000 UEVaultManager-1.6.6/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.6/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.804544 UEVaultManager-1.6.6/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.6.6/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.6.6/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    73092 2023-06-01 11:05:19.000000 UEVaultManager-1.6.6/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    46806 2023-06-01 06:50:17.000000 UEVaultManager-1.6.6/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.804544 UEVaultManager-1.6.6/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.806545 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.810542 UEVaultManager-1.6.6/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23585 2023-05-26 09:04:11.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3927 2023-06-01 07:37:43.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.817546 UEVaultManager-1.6.6/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     5942 2023-06-01 07:24:48.000000 UEVaultManager-1.6.6/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.6.6/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.6/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.6/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.6.6/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.6/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.6/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30610 2023-06-01 07:29:35.000000 UEVaultManager-1.6.6/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.818542 UEVaultManager-1.6.6/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1709 2023-06-01 09:11:19.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.828546 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    32497 2023-06-01 06:46:43.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0    12788 2023-06-01 09:12:21.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    43199 2023-06-01 07:25:24.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0     9697 2023-05-31 17:11:24.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     7590 2023-06-01 11:21:26.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions_no_deps.py
+-rw-rw-rw-   0        0        0     2631 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.835544 UEVaultManager-1.6.6/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3691 2023-06-01 07:18:12.000000 UEVaultManager-1.6.6/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-06-01 11:15:05.000000 UEVaultManager-1.6.6/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.6/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.6.6/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.6/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.6/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.6/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.799544 UEVaultManager-1.6.6/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6127 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      300 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 11:22:23.837544 UEVaultManager-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.6/setup.py
```

### Comparing `UEVaultManager-1.6.5/LICENSE` & `UEVaultManager-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/PKG-INFO` & `UEVaultManager-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.5
+Version: 1.6.6
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
 
 
- UEVaultManager ## version:1.6.5 ## codename: Virgo+5
+ UEVaultManager ## version:1.6.6 ## codename: Virgo+6
```

### Comparing `UEVaultManager-1.6.5/README.md` & `UEVaultManager-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/__init__.py` & `UEVaultManager-1.6.6/UEVaultManager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.6.5'
+__version__ = '1.6.6'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
 # 5 Virgo Shaka
-__codename__ = 'Virgo+5'
+__codename__ = 'Virgo+6'
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
```

### Comparing `UEVaultManager-1.6.5/UEVaultManager/api/egs.py` & `UEVaultManager-1.6.6/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/api/uevm.py` & `UEVaultManager-1.6.6/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.6.6/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/assets/main.ico` & `UEVaultManager-1.6.6/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/cli.py` & `UEVaultManager-1.6.6/UEVaultManager/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1372,22 +1372,23 @@
     # edit_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Input file is in TSV format')
     # edit_parser.add_argument('--json', dest='json', action='store_true', help='Input file is in JSON format')
 
     # Note: this line prints the full help and quit if not other command is available
     args, extra = parser.parse_known_args()
 
     if args.version:
-        cli.print_version()
+        UEVaultManagerCLI.print_version()
+        return
 
     cli = UEVaultManagerCLI(override_config=args.config_file, api_timeout=args.api_timeout)
 
     start_in_edit_mode = str_to_bool(cli.core.uevmlfs.config.get('UEVaultManager', 'start_in_edit_mode', fallback=False))
 
     if not start_in_edit_mode and (not args.subparser_name or args.full_help):
-        cli.print_help(args=args, parser=parser)
+        UEVaultManagerCLI.print_help(args=args, parser=parser)
         return
 
     ql = cli.setup_threaded_logging()
 
     conf_log_level = cli.core.uevmlfs.config.get('UEVaultManager', 'log_level', fallback='info')
     if conf_log_level == 'debug' or args.debug:
         cli.core.verbose_mode = True
```

### Comparing `UEVaultManager-1.6.5/UEVaultManager/core.py` & `UEVaultManager-1.6.6/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.6.6/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.6.6/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.6.6/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.6.6/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.6.6/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.6.6/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.6.6/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/app.py` & `UEVaultManager-1.6.6/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/chunk.py` & `UEVaultManager-1.6.6/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/config.py` & `UEVaultManager-1.6.6/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/csv.py` & `UEVaultManager-1.6.6/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/downloading.py` & `UEVaultManager-1.6.6/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/egl.py` & `UEVaultManager-1.6.6/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.6.6/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/models/manifest.py` & `UEVaultManager-1.6.6/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/functions_no_deps.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions_no_deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,31 +137,44 @@
 
 def create_empty_file(file_path: str) -> str:
     """
     Create an empty file
     :param file_path: the path of the file to create
     :return: the path of the file
     """
-    path = os.path.dirname(file_path)
-    file = os.path.basename(file_path)
+    path, file = os.path.split(file_path)
+    path = check_and_get_folder(os.path.dirname(path))
+    file_path = os.path.normpath(os.path.join(path, file))
+    open(file_path, 'a').close()
+    return file_path
+
+
+def check_and_get_folder(folder_path: str) -> str:
+    """
+    Check if the folder exists. If not, create it or use the default one
+    :param folder_path: the path of the folder to check
+    :return: the path of the folder
+    """
+    path = folder_path
     if not os.path.exists(path):
         try:
             os.makedirs(path)
         except (OSError, PermissionError) as e:
             print(f'Error while creating the directory {path}: {e}')
             if home_dir := os.environ.get('XDG_CONFIG_HOME'):
                 path = os.path.join(home_dir, 'UEVaultManager')
             else:
                 path = os.path.expanduser('~/.config/UEVaultManager')
             if not os.path.exists(path):
                 os.makedirs(path)
-            file_path = os.path.normpath(os.path.join(path, file))
-            print(f'The following file {file_path} will be used as default')
-    open(file_path, 'a').close()
-    return file_path
+                path = os.path.normpath(path)
+            print(f'The following folder {path} will be used as default')
+
+    path = os.path.normpath(path)
+    return path
 
 
 def convert_to_bool(value) -> bool:
     """
     Convert a value to a boolean
     :param value: the value to convert. If the value is not a boolean, it will be converted to a string and then to a boolean.
     :return:
```

### Comparing `UEVaultManager-1.6.5/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.6.6/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/utils/cli.py` & `UEVaultManager-1.6.6/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.6.6/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.6.6/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.6.6/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.6.6/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.6.6/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.5
+Version: 1.6.6
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
 
 
- UEVaultManager ## version:1.6.5 ## codename: Virgo+5
+ UEVaultManager ## version:1.6.6 ## codename: Virgo+6
```

### Comparing `UEVaultManager-1.6.5/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.6.6/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.5/setup.py` & `UEVaultManager-1.6.6/setup.py`

 * *Files identical despite different names*

