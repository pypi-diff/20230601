# Comparing `tmp/neon_phal_plugin_core_updater-1.0.1a1-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_core_updater-1.0.1a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6574 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7869 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2327 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      726 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD
-7 files, 12776 bytes uncompressed, 5246 bytes compressed:  58.9%
+Zip file size: 6577 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7869 b- defN 23-Jun-01 00:33 neon_phal_plugin_core_updater/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-01 00:33 neon_phal_plugin_core_updater-1.0.1a2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2333 b- defN 23-Jun-01 00:33 neon_phal_plugin_core_updater-1.0.1a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 00:33 neon_phal_plugin_core_updater-1.0.1a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-01 00:33 neon_phal_plugin_core_updater-1.0.1a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-01 00:33 neon_phal_plugin_core_updater-1.0.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      726 b- defN 23-Jun-01 00:33 neon_phal_plugin_core_updater-1.0.1a2.dist-info/RECORD
+7 files, 12783 bytes uncompressed, 5249 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_core_updater/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md
+Filename: neon_phal_plugin_core_updater-1.0.1a2.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA
+Filename: neon_phal_plugin_core_updater-1.0.1a2.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/WHEEL
+Filename: neon_phal_plugin_core_updater-1.0.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/entry_points.txt
+Filename: neon_phal_plugin_core_updater-1.0.1a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/top_level.txt
+Filename: neon_phal_plugin_core_updater-1.0.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD
+Filename: neon_phal_plugin_core_updater-1.0.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md` & `neon_phal_plugin_core_updater-1.0.1a2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA` & `neon_phal_plugin_core_updater-1.0.1a2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: neon-utils (~=1.1)
 Requires-Dist: ovos-plugin-manager (~=0.0.20)
 
 # Core Updater Plugin
 Exposes a messagebus API to check for and initiate core module updates. Update
 checks use GitHub releases or PyPI indices, depending on plugin configuration.
@@ -66,8 +66,7 @@
 msg_type: neon.core_updater.start_update
 data:
   version: <new_version>
 ```
 will start the configured update command in a shell with `version` passed as the
 first and only argument. If `version` is omitted, the configured update command
 will be called with no commands.
-
```

## Comparing `neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD` & `neon_phal_plugin_core_updater-1.0.1a2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 neon_phal_plugin_core_updater/__init__.py,sha256=wRzyxoFnSGqIg7x_kjqGz8aAqTE0fYpuW4TxeD7_v64,7869
-neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA,sha256=r8XCQqM3CJxetThX586Edq0vOuXRy6V90cbHID0Yvcs,2327
-neon_phal_plugin_core_updater-1.0.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_core_updater-1.0.1a1.dist-info/entry_points.txt,sha256=3UhJ0b7cF_TxJwAPWiEGnlMncHuI8nOvh9dzyeokMf0,98
-neon_phal_plugin_core_updater-1.0.1a1.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
-neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD,,
+neon_phal_plugin_core_updater-1.0.1a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_core_updater-1.0.1a2.dist-info/METADATA,sha256=5nDP1MlosHZ2u3JkWJU5Ydkdua0QTkWJKKMfNDdsb7A,2333
+neon_phal_plugin_core_updater-1.0.1a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_core_updater-1.0.1a2.dist-info/entry_points.txt,sha256=VNgr7F2h4e9YHmu7kYdA3YQRnayDrsBKBnaUMW_YkpM,99
+neon_phal_plugin_core_updater-1.0.1a2.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
+neon_phal_plugin_core_updater-1.0.1a2.dist-info/RECORD,,
```

