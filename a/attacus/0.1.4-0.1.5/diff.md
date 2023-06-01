# Comparing `tmp/attacus-0.1.4-cp310-cp310-win_amd64.whl.zip` & `tmp/attacus-0.1.5-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,23 @@
-Zip file size: 901853 bytes, number of entries: 18
+Zip file size: 902751 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 10:35 attacus/__about__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-27 06:52 attacus/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-26 08:44 attacus/app.py
 -rw-rw-rw-  2.0 fat     3168 b- defN 23-May-28 18:19 attacus/artifacts.py
+-rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-01 08:36 attacus/assets.py
 -rw-rw-rw-  2.0 fat  2277376 b- defN 23-May-31 13:06 attacus/attacus.pyd
 -rw-rw-rw-  2.0 fat      397 b- defN 23-May-28 18:02 attacus/build.py
--rw-rw-rw-  2.0 fat      429 b- defN 23-May-28 01:20 attacus/flutter_config.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-01 09:42 attacus/cli.py
+-rw-rw-rw-  2.0 fat      518 b- defN 23-Jun-01 08:36 attacus/flutter_config.py
 -rw-rw-rw-  2.0 fat      355 b- defN 23-May-27 08:23 attacus/flutter_view.py
--rw-rw-rw-  2.0 fat      480 b- defN 23-May-28 06:31 attacus/install.py
+-rw-rw-rw-  2.0 fat      590 b- defN 23-Jun-01 09:05 attacus/install.py
 -rw-rw-rw-  2.0 fat      636 b- defN 23-May-28 12:49 attacus/post_build.py
--rw-rw-rw-  2.0 fat      686 b- defN 23-Jun-01 07:55 attacus/project.py
+-rw-rw-rw-  2.0 fat      829 b- defN 23-Jun-01 09:07 attacus/project.py
 -rw-rw-rw-  2.0 fat      668 b- defN 23-Jun-01 07:47 attacus/pyproject.py
 -rw-rw-rw-  2.0 fat      186 b- defN 23-May-28 06:30 attacus/uninstall.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4221 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1371 b- defN 23-Jun-01 08:25 attacus-0.1.4.dist-info/RECORD
-18 files, 2291551 bytes uncompressed, 899639 bytes compressed:  60.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4252 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       44 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/RECORD
+21 files, 2292612 bytes uncompressed, 900167 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -6,20 +6,26 @@
 
 Filename: attacus/app.py
 Comment: 
 
 Filename: attacus/artifacts.py
 Comment: 
 
+Filename: attacus/assets.py
+Comment: 
+
 Filename: attacus/attacus.pyd
 Comment: 
 
 Filename: attacus/build.py
 Comment: 
 
+Filename: attacus/cli.py
+Comment: 
+
 Filename: attacus/flutter_config.py
 Comment: 
 
 Filename: attacus/flutter_view.py
 Comment: 
 
 Filename: attacus/install.py
@@ -33,23 +39,26 @@
 
 Filename: attacus/pyproject.py
 Comment: 
 
 Filename: attacus/uninstall.py
 Comment: 
 
-Filename: attacus-0.1.4.dist-info/LICENSE
+Filename: attacus-0.1.5.dist-info/LICENSE
+Comment: 
+
+Filename: attacus-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: attacus-0.1.4.dist-info/METADATA
+Filename: attacus-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: attacus-0.1.4.dist-info/WHEEL
+Filename: attacus-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: attacus-0.1.4.dist-info/top_level.txt
+Filename: attacus-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: attacus-0.1.4.dist-info/RECORD
+Filename: attacus-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attacus/flutter_config.py

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 from importlib import resources
 
 from loguru import logger
 
 from . import attacus as core
+from .assets import get_assets_path
 from .artifacts import get_icu_data_path
 
 class FlutterConfig(core.FlutterConfig):
     def __init__(self) -> None:
         super().__init__()
-        self.assets_path = str(Path.cwd() / 'flutter_assets')
+        #self.assets_path = str(Path.cwd() / 'flutter_assets')
+        self.assets_path = str(get_assets_path())
         self.icu_data_path = str(get_icu_data_path())
         #logger.debug(self.icu_data_path)
```

## attacus/install.py

```diff
@@ -1,16 +1,22 @@
 import shutil
 from pathlib import Path
 
 from rich import print
 
+from .project import get_project
+
+
 def install():
-    from_path = Path.cwd() / 'build' / 'flutter_assets'
-    to_path = Path.cwd() / 'flutter_assets'
-    #print('[green]Installing :thumbs_up:') # This will bomb with F5 in vscode
-    print(f'[green]Installing flutter_assets to {to_path}[/green]')
+    from_path = Path.cwd() / "build" / "flutter_assets"
+    # to_path = Path.cwd() / "flutter_assets"
+    project = get_project()
+    to_path = project.flutter_assets
+    # print('[green]Installing :thumbs_up:') # This will bomb with F5 in vscode
+    print(f"[green]Installing flutter_assets to {to_path}[/green]")
     if to_path.exists():
         shutil.rmtree(to_path)
     shutil.copytree(from_path, to_path)
 
+
 if __name__ == "__main__":
     install()
```

## attacus/project.py

```diff
@@ -13,11 +13,17 @@
         self.path: Path = path
         self.pyproject:PyProject = PyProject.load(path)
         self.name: str = self.pyproject.name
 
     @property
     def flutter_assets(self):
         if hasattr(self.pyproject.tool.attacus, 'flutter_assets'):
-            return self.pyproject.tool.attacus.flutter_assets
+            return Path(self.pyproject.tool.attacus.flutter_assets)
         return Path.cwd() / 'flutter_assets'
 
-_project: Project = None
+_project: Project = None
+
+def get_project() -> Project:
+    global _project
+    if not _project:
+        _project = Project(Path.cwd())
+    return _project
```

## Comparing `attacus-0.1.4.dist-info/LICENSE` & `attacus-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attacus-0.1.4.dist-info/METADATA` & `attacus-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attacus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Flutter Extension
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License        
         Copyright (c) 2023 Kurtis Fields        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,14 +35,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru (~=0.7.0)
 Requires-Dist: platformdirs (~=3.5.1)
 Requires-Dist: requests (~=2.31.0)
 Requires-Dist: rich (~=13.3.5)
+Requires-Dist: click (~=8.1.3)
 Provides-Extra: dev
 Requires-Dist: black (~=22.12.0) ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest (~=7.2.1) ; extra == 'test'
 
 # Attacus :snake: :butterfly:
```

