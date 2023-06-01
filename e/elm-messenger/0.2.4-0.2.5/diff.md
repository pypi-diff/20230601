# Comparing `tmp/elm-messenger-0.2.4.tar.gz` & `tmp/elm-messenger-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.2.4.tar", last modified: Tue May 30 02:10:57 2023, max compression
+gzip compressed data, was "elm-messenger-0.2.5.tar", last modified: Thu Jun  1 03:52:17 2023, max compression
```

## Comparing `elm-messenger-0.2.4.tar` & `elm-messenger-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18770 2023-05-30 02:08:02.000000 elm-messenger-0.2.4/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.4/messengercli/patcher.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.4/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7109 2023-05-31 16:29:21.000000 elm-messenger-0.2.5/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-01 03:52:17.277209 elm-messenger-0.2.5/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    19438 2023-06-01 03:45:19.000000 elm-messenger-0.2.5/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.5/messengercli/patcher.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.5/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/setup.py
```

### Comparing `elm-messenger-0.2.4/messengercli/messenger.py` & `elm-messenger-0.2.5/messengercli/messenger.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import shutil
 import json
 from .updater import Updater
 from .patcher import patch
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.2.4"
+API_VERSION = "0.2.5"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -25,24 +25,25 @@
         """
         if os.path.exists("messenger.json"):
             with open("messenger.json", "r") as f:
                 self.config = json.load(f)
             if "version" not in self.config:
                 raise Exception("Messenger API version not found in the config file.")
             if self.config["version"] != API_VERSION:
-                raise Exception(f"Messenger API version not matched. I'm using v{API_VERSION}. You can edit messenger.json manually to upgrade.")
+                raise Exception(
+                    f"Messenger API version not matched. I'm using v{API_VERSION}. You can edit messenger.json manually to upgrade."
+                )
         else:
             raise Exception(
                 "messenger.json not found. Are you in the project initialized by the Messenger? Try `messenger init <your-project-name>`."
             )
         if not os.path.exists(".messenger"):
             print("Messenger files not found. Initializing...")
             os.system(f"git clone {self.config['template_repo']} .messenger --depth=1")
 
-
     def dump_config(self):
         with open("messenger.json", "w") as f:
             json.dump(self.config, f, indent=4, ensure_ascii=False)
 
     def add_scene(self, scene: str):
         if scene in self.config["scenes"] or scene in self.config["sceneprotos"]:
             raise Exception("Scene already exists.")
@@ -254,26 +255,37 @@
         self.config["sceneprotos"][sceneproto]["levels"].append(level)
         self.dump_config()
         os.mkdir(f"src/Scenes/{level}")
         Updater(
             [".messenger/sceneproto/Export.elm"], [f"src/Scenes/{level}/Export.elm"]
         ).rep(level).rep(sceneproto)
 
-    def add_component(self, name: str):
+    def add_component(self, name: str, dir=""):
         """
         Add a component
         """
-        os.mkdir(f"src/Components/{name}")
+        from os.path import join
+
+        if not os.path.exists(join("src/Components", dir)):
+            raise Exception("Directory doesn't exist.")
+        if os.path.exists(join("src/Components", dir, name)):
+            raise Exception("Component already exists.")
+        dir = join(dir, name)
+        os.mkdir(join("src/Components", dir))
+        modPath = dir.replace("/", ".")
         Updater(
             [
                 ".messenger/component/Sample/Sample.elm",
                 ".messenger/component/Sample/Export.elm",
             ],
-            [f"src/Components/{name}/{name}.elm", f"src/Components/{name}/Export.elm"],
-        ).rep(name)
+            [
+                join("src/Components", dir, f"{name}.elm"),
+                join("src/Components", dir, "Export.elm"),
+            ],
+        ).rep(modPath).rep(name)
 
     def add_gamecomponent(self, sceneproto: str, gc: str):
         """
         Add a GameComponent to a SceneProto
         """
         if sceneproto not in self.config["sceneprotos"]:
             raise Exception("SceneProto doesn't exist.")
@@ -414,37 +426,54 @@
 
     os.makedirs("src/Scenes", exist_ok=True)
     os.makedirs("assets", exist_ok=True)
     os.makedirs("src/Components", exist_ok=True)
     os.makedirs("src/SceneProtos", exist_ok=True)
 
     print("Creating elm.json...")
-    initObject = {"version": API_VERSION, "template_repo" : template_repo, "scenes": {}, "sceneprotos": {}}
+    initObject = {
+        "version": API_VERSION,
+        "template_repo": template_repo,
+        "scenes": {},
+        "sceneprotos": {},
+    }
     with open("messenger.json", "w") as f:
         json.dump(initObject, f, indent=4, ensure_ascii=False)
     print("Installing dependencies...")
     os.system("elm make")
     print("Done!")
     print(f"Now please go to {name} and add scenes and components.")
 
 
 @app.command()
-def component(name: str):
+def component(
+    name: str,
+    dir=typer.Option(
+        "", "--dir", "-d", help="Component module to create component in."
+    ),
+):
     msg = Messenger()
     input(f"You are going to create a component named {name}, continue?")
-    msg.add_component(name)
+    msg.add_component(name, dir)
     msg.format()
     print("Done!")
 
 
 @app.command()
 def update(
     scene=typer.Option(False, "--scene", "-s", help="Update scenes."),
-    scenelayer=typer.Option(None, "--scenelayer", "-sl", help="Update layers in that scene."),
-    sceneprotolayer=typer.Option(None, "--sceneprotolayer", "-spl", help="Update sceneproto layers in that sceneproto."),
+    scenelayer=typer.Option(
+        None, "--scenelayer", "-sl", help="Update layers in that scene."
+    ),
+    sceneprotolayer=typer.Option(
+        None,
+        "--sceneprotolayer",
+        "-spl",
+        help="Update sceneproto layers in that sceneproto.",
+    ),
 ):
     msg = Messenger()
     input(
         f"You are going to regenerate settings (including scenes, layers, sceneproto layers), continue?"
     )
     if scene:
         msg.update_scenes()
@@ -532,9 +561,10 @@
 def updatelib():
     msg = Messenger()
     input(f"You are going to update the core library of Messenger, continue?")
     patch()
     msg.format()
     print("Done!")
 
+
 if __name__ == "__main__":
     app()
```

### Comparing `elm-messenger-0.2.4/messengercli/patcher.py` & `elm-messenger-0.2.5/messengercli/patcher.py`

 * *Files identical despite different names*

### Comparing `elm-messenger-0.2.4/messengercli/updater.py` & `elm-messenger-0.2.5/messengercli/updater.py`

 * *Files identical despite different names*

