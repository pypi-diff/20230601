# Comparing `tmp/honeybee-idaice-0.3.3.tar.gz` & `tmp/honeybee-idaice-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.3.3.tar", last modified: Wed May 31 19:14:10 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.3.4.tar", last modified: Thu Jun  1 19:32:29 2023, max compression
```

## Comparing `honeybee-idaice-0.3.3.tar` & `honeybee-idaice-0.3.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 19:14:10.000000 honeybee-idaice-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 19:12:44.000000 honeybee-idaice-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 19:32:29.000000 honeybee-idaice-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-01 19:31:23.000000 honeybee-idaice-0.3.4/setup.py
```

### Comparing `honeybee-idaice-0.3.3/LICENSE` & `honeybee-idaice-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/PKG-INFO` & `honeybee-idaice-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.3
+Version: 0.3.4
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.3/README.md` & `honeybee-idaice-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/archive.py` & `honeybee-idaice-0.3.4/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.3.4/honeybee_idaice/bldgbody.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.3.4/honeybee_idaice/cli/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         model_json: Full path to a Model JSON file (HBJSON) or a Model pkl (HBpkl) file.
 
     """
     try:
         model = Model.from_file(model_json)
         folder = pathlib.Path(folder)
         folder.mkdir(parents=True, exist_ok=True)
-        model.to_idm(folder.as_posix(), name=name)
+        model.to_idm(folder.as_posix(), name=name, debug=False)
     except Exception as e:
         _logger.exception('Model translation failed.\n{}'.format(e))
         sys.exit(1)
     else:
         sys.exit(0)
```

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/face.py` & `honeybee-idaice-0.3.4/honeybee_idaice/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.3.4/honeybee_idaice/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/shade.py` & `honeybee-idaice-0.3.4/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.3.4/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.3.4/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.3.4/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.3.4/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.3.4/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.3.4/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/writer.py` & `honeybee-idaice-0.3.4/honeybee_idaice/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,14 +213,18 @@
 
 def model_to_idm(model: Model, out_folder: pathlib.Path, name: str = None,
                  debug: bool = True):
     """Translate a Honeybee model to an IDM file."""
 
     model = prepare_model(model)
 
+    # make sure names don't have subfolder or extension
+    original_name = name or model.display_name
+    name = pathlib.Path(original_name).stem
+
     __here__ = pathlib.Path(__file__).parent
     templates_folder = __here__.joinpath('templates')
     bldg_name = name or model.display_name
     base_folder = pathlib.Path(out_folder)
     model_folder = base_folder.joinpath(bldg_name)
     if model_folder.exists():
         shutil.rmtree(model_folder.as_posix())
@@ -276,15 +280,17 @@
         shutil.copy(template_room, room_file.as_posix())
         with room_file.open('a') as rm:
             geometry = room_to_idm(room)
             rm.write(geometry)
             footer = f'\n;[end of {bldg_name}\\{room_name}.idm]\n'
             rm.write(footer)
 
-    idm_file = base_folder.joinpath(f'{bldg_name}.idm')
+    if not original_name.endswith('.idm'):
+        original_name = f'{original_name}.idm'
+    idm_file = base_folder.joinpath(original_name)
     zip_folder_to_idm(model_folder, idm_file)
 
     # clean up the folder
     if not debug:
-        shutil.rmtree(model_folder)
+        shutil.rmtree(model_folder, ignore_errors=True)
 
     return idm_file
```

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.3.4/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.3.4/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.3
+Version: 0.3.4
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.3/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.3.4/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.3/setup.py` & `honeybee-idaice-0.3.4/setup.py`

 * *Files identical despite different names*

