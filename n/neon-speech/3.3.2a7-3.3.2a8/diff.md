# Comparing `tmp/neon_speech-3.3.2a7-py3-none-any.whl.zip` & `tmp/neon_speech-3.3.2a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17841 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1831 b- defN 23-May-26 22:25 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2784 b- defN 23-May-26 22:25 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5171 b- defN 23-May-26 22:25 neon_speech/cli.py
--rw-r--r--  2.0 unx    21078 b- defN 23-May-26 22:25 neon_speech/service.py
--rw-r--r--  2.0 unx     4459 b- defN 23-May-26 22:25 neon_speech/stt.py
--rw-r--r--  2.0 unx     4395 b- defN 23-May-26 22:25 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2451 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      988 b- defN 23-May-26 22:25 neon_speech-3.3.2a7.dist-info/RECORD
-12 files, 45006 bytes uncompressed, 16183 bytes compressed:  64.0%
+Zip file size: 17817 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-31 22:15 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2784 b- defN 23-May-31 22:15 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5171 b- defN 23-May-31 22:15 neon_speech/cli.py
+-rw-r--r--  2.0 unx    20934 b- defN 23-May-31 22:15 neon_speech/service.py
+-rw-r--r--  2.0 unx     4459 b- defN 23-May-31 22:15 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4395 b- defN 23-May-31 22:15 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-31 22:15 neon_speech-3.3.2a8.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2451 b- defN 23-May-31 22:15 neon_speech-3.3.2a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 22:15 neon_speech-3.3.2a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-May-31 22:15 neon_speech-3.3.2a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-31 22:15 neon_speech-3.3.2a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      988 b- defN 23-May-31 22:15 neon_speech-3.3.2a8.dist-info/RECORD
+12 files, 44862 bytes uncompressed, 16159 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.3.2a7.dist-info/LICENSE.md
+Filename: neon_speech-3.3.2a8.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.3.2a7.dist-info/METADATA
+Filename: neon_speech-3.3.2a8.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.3.2a7.dist-info/WHEEL
+Filename: neon_speech-3.3.2a8.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.3.2a7.dist-info/entry_points.txt
+Filename: neon_speech-3.3.2a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a7.dist-info/top_level.txt
+Filename: neon_speech-3.3.2a8.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a7.dist-info/RECORD
+Filename: neon_speech-3.3.2a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/service.py

```diff
@@ -178,15 +178,14 @@
                                      "wake_word": requested_ww})
         else:
             try:
                 LOG.info(f"Disabling wake word: {requested_ww}")
                 config_patch = {"hotwords": {requested_ww: {"active": False}}}
                 _SERVICE_READY.clear()
                 update_mycroft_config(config_patch, bus=self.bus)
-                self.reload_configuration()  # TODO Not auto-reloading?
                 if not _SERVICE_READY.wait(15):
                     raise TimeoutError("Timed out waiting for config reload")
                 resp = message.response({"error": False,
                                          "active": False,
                                          "wake_word": requested_ww})
             except Exception as e:
                 LOG.exception(e)
@@ -219,15 +218,14 @@
                                      "wake_word": requested_ww})
         else:
             try:
                 LOG.info(f"Enabling wake word: {requested_ww}")
                 config_patch = {"hotwords": {requested_ww: {"active": True}}}
                 _SERVICE_READY.clear()
                 update_mycroft_config(config_patch, bus=self.bus)
-                self.reload_configuration()  # TODO Not auto-reloading?
                 if not _SERVICE_READY.wait(30):
                     raise TimeoutError("Timed out waiting for config reload")
                 resp = message.response({"error": False,
                                          "active": True,
                                          "wake_word": requested_ww})
             except Exception as e:
                 LOG.exception(e)
```

## Comparing `neon_speech-3.3.2a7.dist-info/LICENSE.md` & `neon_speech-3.3.2a8.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.3.2a7.dist-info/METADATA` & `neon_speech-3.3.2a8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.3.2a7
+Version: 3.3.2a8
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ovos-dinkum-listener (>=0.0.2a24,~=0.0.1)
+Requires-Dist: ovos-dinkum-listener (>=0.0.2a32,~=0.0.1)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-utils (~=0.0.30)
 Requires-Dist: ovos-plugin-manager (>=0.0.23a17,~=0.0.19)
 Requires-Dist: click (~=8.0)
 Requires-Dist: click-default-group (~=1.2)
 Requires-Dist: neon-utils[audio,network] (>=1.5.0a5,~=1.3)
 Requires-Dist: ovos-config (~=0.0.7)
```

