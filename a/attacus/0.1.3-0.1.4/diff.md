# Comparing `tmp/attacus-0.1.3-cp310-cp310-win_amd64.whl.zip` & `tmp/attacus-0.1.4-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 900391 bytes, number of entries: 16
+Zip file size: 901853 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 10:35 attacus/__about__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-27 06:52 attacus/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-26 08:44 attacus/app.py
--rw-rw-rw-  2.0 fat     2771 b- defN 23-May-28 16:10 attacus/artifacts.py
--rw-rw-rw-  2.0 fat  2275328 b- defN 23-May-28 07:29 attacus/attacus.pyd
--rw-rw-rw-  2.0 fat      412 b- defN 23-May-28 06:53 attacus/build.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-May-28 18:19 attacus/artifacts.py
+-rw-rw-rw-  2.0 fat  2277376 b- defN 23-May-31 13:06 attacus/attacus.pyd
+-rw-rw-rw-  2.0 fat      397 b- defN 23-May-28 18:02 attacus/build.py
 -rw-rw-rw-  2.0 fat      429 b- defN 23-May-28 01:20 attacus/flutter_config.py
 -rw-rw-rw-  2.0 fat      355 b- defN 23-May-27 08:23 attacus/flutter_view.py
 -rw-rw-rw-  2.0 fat      480 b- defN 23-May-28 06:31 attacus/install.py
 -rw-rw-rw-  2.0 fat      636 b- defN 23-May-28 12:49 attacus/post_build.py
+-rw-rw-rw-  2.0 fat      686 b- defN 23-Jun-01 07:55 attacus/project.py
+-rw-rw-rw-  2.0 fat      668 b- defN 23-Jun-01 07:47 attacus/pyproject.py
 -rw-rw-rw-  2.0 fat      186 b- defN 23-May-28 06:30 attacus/uninstall.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4271 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1221 b- defN 23-May-28 17:17 attacus-0.1.3.dist-info/RECORD
-16 files, 2287667 bytes uncompressed, 898405 bytes compressed:  60.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4221 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1371 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/RECORD
+18 files, 2291551 bytes uncompressed, 899639 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -24,26 +24,32 @@
 
 Filename: attacus/install.py
 Comment: 
 
 Filename: attacus/post_build.py
 Comment: 
 
+Filename: attacus/project.py
+Comment: 
+
+Filename: attacus/pyproject.py
+Comment: 
+
 Filename: attacus/uninstall.py
 Comment: 
 
-Filename: attacus-0.1.3.dist-info/LICENSE
+Filename: attacus-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: attacus-0.1.3.dist-info/METADATA
+Filename: attacus-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: attacus-0.1.3.dist-info/WHEEL
+Filename: attacus-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: attacus-0.1.3.dist-info/top_level.txt
+Filename: attacus-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: attacus-0.1.3.dist-info/RECORD
+Filename: attacus-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attacus/artifacts.py

```diff
@@ -1,23 +1,24 @@
 import os
 import requests
 import tempfile
 import zipfile
 import json
-
+import __main__
 from loguru import logger
 
 from pathlib import Path
 from platformdirs import user_cache_dir
 
 appname = "Attacus"
 appauthor = "CrungeLab"
 
 
 def ensure() -> None:
+    logger.debug('ensure')
     version = get_engine_version()
     if not version:
         raise RuntimeError('Flutter Engine Version not found')
     ensure_engine(version)
     ensure_artifacts(version)
 
 def ensure_engine(version: str) -> None:
@@ -35,33 +36,50 @@
     path = Path(user_cache_dir(appname, appauthor)) / 'flutter' / version / 'artifacts'
     #logger.debug(path)
     if not path.exists():
         url = f'https://storage.googleapis.com/flutter_infra_release/flutter/{version}/windows-x64/artifacts.zip'
         zip_file = download_file(url)
         extract_zip(zip_file, path)
 
+_engine_version: str = None
+
 def get_engine_version() -> str:
-    #version = '90fa3ae28fe6ddaee1af2c120f01e50201c1401b'
+    global _engine_version
+    if _engine_version:
+        return _engine_version
+
     version = None
     flutter_assets = os.environ.get('FLUTTER_ASSETS')
     if flutter_assets:
-        logger.debug(f'loading engine version from {flutter_assets}')
-        engine_data_path = Path(flutter_assets) / 'Engine.json'
-        with open(engine_data_path, 'r') as f:
-            engine_data = json.load(f)
-            version = engine_data['version']
+        version = get_app_engine_version()
     else:
-        flutter_root = os.environ.get('FLUTTER_ROOT')
-        if not flutter_root:
-            return None
-        logger.debug(f'loading engine version from sdk')
-        version_path = flutter_root / Path('bin/internal/engine.version')
-        with open(version_path, 'r') as file:
-            version = file.readline().rstrip()
+        version = get_sdk_engine_version()
     logger.debug(version)
+    _engine_version = version
+    return version
+
+def get_app_engine_version() -> str:
+    flutter_assets = os.environ.get('FLUTTER_ASSETS')
+    if not flutter_assets:
+        return None
+    logger.debug(f'loading engine version from {flutter_assets}')
+    engine_data_path = Path(flutter_assets) / 'Engine.json'
+    with open(engine_data_path, 'r') as f:
+        engine_data = json.load(f)
+        version = engine_data['version']
+    return version
+
+def get_sdk_engine_version() -> str:
+    flutter_root = os.environ.get('FLUTTER_ROOT')
+    if not flutter_root:
+        return None
+    logger.debug(f'loading engine version from sdk')
+    version_path = flutter_root / Path('bin/internal/engine.version')
+    with open(version_path, 'r') as file:
+        version = file.readline().rstrip()
     return version
 
 def download_file(url: str):
     response = requests.get(url, stream=True)
     temp_file = tempfile.TemporaryFile()
     for chunk in response.iter_content(chunk_size=128):
         temp_file.write(chunk)
```

## attacus/build.py

```diff
@@ -1,9 +1,8 @@
 import sys
-import shutil
 from pathlib import Path
 import subprocess
 
 from .post_build import post_build
 from .install import install
 
 FLUTTER = 'flutter.bat' if sys.platform == 'win32' else 'flutter'
```

## Comparing `attacus-0.1.3.dist-info/LICENSE` & `attacus-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attacus-0.1.3.dist-info/METADATA` & `attacus-0.1.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attacus
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Flutter Extension
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License        
         Copyright (c) 2023 Kurtis Fields        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,15 +36,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru (~=0.7.0)
 Requires-Dist: platformdirs (~=3.5.1)
 Requires-Dist: requests (~=2.31.0)
 Requires-Dist: rich (~=13.3.5)
 Provides-Extra: dev
-Requires-Dist: cxbuild (==0.1.0) ; extra == 'dev'
 Requires-Dist: black (~=22.12.0) ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest (~=7.2.1) ; extra == 'test'
 
 # Attacus :snake: :butterfly:
 
 Flutter Python Extension
```

