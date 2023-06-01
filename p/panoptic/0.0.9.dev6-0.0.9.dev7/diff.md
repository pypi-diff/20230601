# Comparing `tmp/panoptic-0.0.9.dev6.tar.gz` & `tmp/panoptic-0.0.9.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptic-0.0.9.dev6.tar", last modified: Tue May 30 20:50:54 2023, max compression
+gzip compressed data, was "panoptic-0.0.9.dev7.tar", last modified: Thu Jun  1 06:55:11 2023, max compression
```

## Comparing `panoptic-0.0.9.dev6.tar` & `panoptic-0.0.9.dev7.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.191613 panoptic-0.0.9.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-30 20:50:54.191613 panoptic-0.0.9.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/build_commans.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.183613 panoptic-0.0.9.dev6/panoptic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.187613 panoptic-0.0.9.dev6/panoptic/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/compute/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/compute/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/compute/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.187613 panoptic-0.0.9.dev6/panoptic/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/core/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/core/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/core/image_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.187613 panoptic-0.0.9.dev6/panoptic/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.187613 panoptic-0.0.9.dev6/panoptic/html/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/html/assets/bootstrap-icons-966620f9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/html/assets/bootstrap-icons-c6569d46.woff
--rw-r--r--   0 runner    (1001) docker     (123)   262280 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/html/assets/index-26ce049e.js
--rw-r--r--   0 runner    (1001) docker     (123)   430321 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/html/assets/index-66fe5260.css
--rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/html/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.191613 panoptic-0.0.9.dev6/panoptic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/models/payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.191613 panoptic-0.0.9.dev6/panoptic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/scripts/create_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/scripts/populate_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/panoptic/scripts/to_pca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:50:54.183613 panoptic-0.0.9.dev6/panoptic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-30 20:50:54.000000 panoptic-0.0.9.dev6/panoptic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-30 20:50:54.000000 panoptic-0.0.9.dev6/panoptic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:50:54.000000 panoptic-0.0.9.dev6/panoptic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 20:50:54.000000 panoptic-0.0.9.dev6/panoptic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 20:50:54.000000 panoptic-0.0.9.dev6/panoptic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 20:50:54.000000 panoptic-0.0.9.dev6/panoptic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:50:54.191613 panoptic-0.0.9.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-30 20:50:40.000000 panoptic-0.0.9.dev6/thunder-collection_Panoptic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.457470 panoptic-0.0.9.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 06:55:11.457470 panoptic-0.0.9.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/build_commans.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.453469 panoptic-0.0.9.dev7/panoptic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.453469 panoptic-0.0.9.dev7/panoptic/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/compute/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/compute/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/compute/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.453469 panoptic-0.0.9.dev7/panoptic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/core/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/core/image_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.453469 panoptic-0.0.9.dev7/panoptic/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.453469 panoptic-0.0.9.dev7/panoptic/html/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/html/assets/bootstrap-icons-966620f9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/html/assets/bootstrap-icons-c6569d46.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   430321 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/html/assets/index-66fe5260.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/html/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.457470 panoptic-0.0.9.dev7/panoptic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/models/payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.457470 panoptic-0.0.9.dev7/panoptic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/scripts/create_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/scripts/populate_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/panoptic/scripts/to_pca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:11.453469 panoptic-0.0.9.dev7/panoptic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 06:55:11.000000 panoptic-0.0.9.dev7/panoptic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-01 06:55:11.000000 panoptic-0.0.9.dev7/panoptic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 06:55:11.000000 panoptic-0.0.9.dev7/panoptic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 06:55:11.000000 panoptic-0.0.9.dev7/panoptic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 06:55:11.000000 panoptic-0.0.9.dev7/panoptic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 06:55:11.000000 panoptic-0.0.9.dev7/panoptic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 06:55:11.457470 panoptic-0.0.9.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-01 06:54:59.000000 panoptic-0.0.9.dev7/thunder-collection_Panoptic.json
```

### Comparing `panoptic-0.0.9.dev6/PKG-INFO` & `panoptic-0.0.9.dev7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.9.dev6
+Version: 0.0.9.dev7
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.9.dev6/description.md` & `panoptic-0.0.9.dev7/description.md`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/api.py` & `panoptic-0.0.9.dev7/panoptic/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 from sys import platform
 from typing import Optional
 
 import aiofiles as aiofiles
-from fastapi import FastAPI, Query
+from fastapi import FastAPI, Query, UploadFile
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 from starlette.responses import Response
 from starlette.staticfiles import StaticFiles
+import pandas as pd
 
 from panoptic import core
 from panoptic.scripts.to_pca import compute_all_pca
-from panoptic.core import create_property, add_property_to_image, get_images, create_tag, \
+from panoptic.core import create_property, add_property_to_images, get_images, create_tag, \
     delete_image_property, \
     update_tag, get_tags, get_properties, delete_property, update_property, delete_tag, delete_tag_parent, add_folder, \
-    db_utils, make_clusters, get_similar_images, get_full_image
+    db_utils, make_clusters, get_similar_images, get_full_image, read_properties_file
 from panoptic.core import db
 from panoptic.models import Property, Images, Tag, Tags, Properties, PropertyPayload, \
     AddImagePropertyPayload, AddTagPayload, DeleteImagePropertyPayload, \
     UpdateTagPayload, UpdatePropertyPayload, Tab, MakeClusterPayload
 
 app = FastAPI()
 app.add_middleware(
@@ -49,24 +50,28 @@
     return await get_properties()
 
 
 @app.patch("/property")
 async def update_property_route(payload: UpdatePropertyPayload) -> Property:
     return await update_property(payload)
 
+@app.post('/property/file')
+async def properties_by_file(file: UploadFile):
+    data = pd.read_csv(file.file, sep=";")
+    return await read_properties_file(data)
 
 @app.delete('/property/{property_id}')
 async def delete_property_route(property_id: str):
     await delete_property(property_id)
     return f"Property {property_id} correctly deleted"
 
 
 # Route pour récupérer la liste de toutes les images
 @app.get("/images")
-async def get_images_route() -> Images:
+async def get_images_route():
     images = await get_images()
     return images
 
 
 @app.get('/images/{file_path:path}')
 async def get_image(file_path: str):
     if platform == "linux" or platform == "linux2" or platform == "darwin":
@@ -82,15 +87,15 @@
     return Response(content=data, media_type="image/" + ext)
 
 
 # Route pour ajouter une property à une image dans la table de jointure entre image et property
 # On retourne le payload pour pouvoir valider l'update côté front
 @app.post("/image_property")
 async def add_image_property(payload: AddImagePropertyPayload) -> AddImagePropertyPayload:
-    await add_property_to_image(payload.property_id, payload.sha1_list, payload.value)
+    await add_property_to_images(payload.property_id, payload.sha1_list, payload.value)
     return payload
 
 
 # Route pour supprimer une property d'une image dans la table de jointure entre image et property
 @app.delete("/image_property")
 async def delete_property_route(payload: DeleteImagePropertyPayload) -> DeleteImagePropertyPayload:
     await delete_image_property(payload.property_id, payload.sha1)
```

### Comparing `panoptic-0.0.9.dev6/panoptic/compute/ocr.py` & `panoptic-0.0.9.dev7/panoptic/compute/ocr.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/compute/similarity.py` & `panoptic-0.0.9.dev7/panoptic/compute/similarity.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/compute/transform.py` & `panoptic-0.0.9.dev7/panoptic/compute/transform.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/compute/utils.py` & `panoptic-0.0.9.dev7/panoptic/compute/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/core/__init__.py` & `panoptic-0.0.9.dev7/panoptic/core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import atexit
 import json
 from concurrent.futures import ProcessPoolExecutor
+import random
 from typing import List
 
+import pandas
 from fastapi import HTTPException
 
 from panoptic import compute
 import panoptic.core.db
 from panoptic.models import PropertyType, JSON, Image, Tag, Images, PropertyValue, Property, Tags, Properties, \
     UpdateTagPayload, UpdatePropertyPayload, Folder, ImageVector
 from .image_importer import ImageImporter
@@ -35,28 +37,27 @@
     return {prop.id: prop for prop in properties}
 
 
 async def delete_property(property_id: str):
     await db.delete_property(property_id)
 
 
-async def get_images() -> Images:
+async def get_images():
     """
     Get all images from database
     """
     rows = await db.get_images()
     result = {}
     for row in rows:
         sha1, paths, height, width, url, extension, name, property_id, value, ahash = row
         if sha1 not in result:
-            result[sha1] = Image(sha1=sha1, paths=json.loads(paths), width=width, height=height, url=url, name=name,
-                                 extension=extension, ahash=ahash)
+            result[sha1] = {'sha1':sha1, 'paths':json.loads(paths), 'width':width, 'height': height, 'url':url, 'name':name,
+                                 'extension':extension, 'ahash':ahash, 'properties': {}}
         if property_id:
-            result[sha1].properties[property_id] = PropertyValue(
-                **{'property_id': property_id, 'value': db.decode_if_json(value)})
+            result[sha1]['properties'][property_id] = {'property_id': property_id, 'value': db.decode_if_json(value)}
     return result
 
 
 async def get_full_image(sha1: str) -> Image:
     """
     Get all images from database
     """
@@ -84,28 +85,56 @@
 
 async def get_similar_images(sha1_list: list[str]):
     vectors = [i.vector for i in await db.get_images_with_vectors(sha1_list)]
     res = compute.get_similar_images(vectors)
     return [img for img in res if img['sha1'] not in sha1_list]
 
 
-async def add_property_to_image(property_id: int, sha1_list: list[str], value: JSON) -> str:
+async def add_property_to_images(property_id: int, sha1_list: list[str], value: JSON) -> str:
     # first check that the property and the image exist:
     if await db.get_property_by_id(property_id) and await db.get_images_by_sha1s(sha1_list):
         await db.add_or_update_images_properties(sha1_list, property_id, value)
         # check if a value already exists
         # if await db.get_image_property(sha1, property_id):
         #     await db.update_image_property(sha1, property_id, value)
         # else:
         #     await db.add_image_property(sha1, property_id, value)
         return value
     else:
         raise HTTPException(status_code=400, detail="Trying to set a value on a non existent property or sha1")
 
 
+async def read_properties_file(data: pandas.DataFrame):
+    filenames, sha1s = zip(*[(i.name, i.sha1) for i in await db.get_images(as_image=True)])
+    data = data[data.key.isin(filenames)]
+    data = data.drop_duplicates(subset='key', keep='first')
+    for f, s in zip(filenames, sha1s):
+        data.loc[data.key == f, 'sha1'] = s
+
+    properties_to_create = data.columns.tolist()
+
+    for prop in properties_to_create:
+        if prop == "key" or prop == "sha1":
+            continue
+        prop_name, prop_type = prop.split('[')
+        prop_type = PropertyType(prop_type.split(']')[0])
+        property = await create_property(prop_name, prop_type)
+        prop_values = list(data[prop].unique())
+        for value in prop_values:
+            real_value = value
+            if property.type == PropertyType.tag.value or property.type == PropertyType.multi_tags.value:
+                colors = ["7c1314", "c31d20", "f94144", "f3722c", "f8961e", "f9c74f", "90be6d", "43aa8b", "577590",
+                           "9daebe"]
+                color = colors[random.randint(0, len(colors) - 1)]
+                tag = await create_tag(property.id, value, 0, color)
+                real_value = [tag.id]
+            sub_data = data[data[prop] == value]
+            await add_property_to_images(property.id, sub_data.sha1.tolist(), real_value)
+
+
 async def delete_image_property(property_id: int, sha1: str):
     await db.delete_image_property(property_id, sha1)
 
 
 # TODO: confirm lock efficacity
 add_image_lock = asyncio.Lock()
```

### Comparing `panoptic-0.0.9.dev6/panoptic/core/db.py` & `panoptic-0.0.9.dev7/panoptic/core/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from panoptic.core.db_utils import execute_query, decode_if_json, execute_query_many
 from panoptic.models import ImageVector
 from panoptic.models import Tag, Image, Property, ImageProperty, JSON, Folder, Tab
 
 
 async def add_property(name: str, property_type: str) -> Property:
-    query = 'INSERT INTO properties (name, type) VALUES (?, ?)'
+    query = 'INSERT INTO properties (name, type) VALUES (?, ?) on conflict do nothing'
     cursor = await execute_query(query, (name, property_type))
     prop = Property(id=cursor.lastrowid, name=name, type=property_type)
     return prop
 
 
 async def add_tag(property_id: int, value: str, parents: str, color: str):
     query = "INSERT INTO tags (property_id, value, parents, color) VALUES (?, ?, ?, ?)"
@@ -60,21 +60,24 @@
             LEFT JOIN images_properties i_d ON i.sha1 = i_d.sha1
             WHERE i.sha1 = ?
             """
     cursor = await execute_query(query, (sha1,))
     return await cursor.fetchall()
 
 
-async def get_images():
+async def get_images(as_image=False):
     query = """
             SELECT DISTINCT i.sha1, i.paths, i.height, i.width,  i.url, i.extension, i.name, i_d.property_id, i_d.value, i.ahash
             FROM images i
             LEFT JOIN images_properties i_d ON i.sha1 = i_d.sha1
+            ORDER BY i.name
             """
     cursor = await execute_query(query)
+    if as_image:
+        return [Image(**auto_dict(row, cursor)) for row in await cursor.fetchall()]
     return await cursor.fetchall()
 
 
 async def update_image_paths(sha1, new_paths) -> list[str]:
     query = """
                UPDATE images
                SET paths = ?
@@ -285,8 +288,14 @@
 
 
 async def add_or_update_images_properties(sha1_list: list[str], property_id: int, value):
     query = "INSERT into images_properties (sha1, property_id, value) " \
             "VALUES (?, ?, ?)" \
             "ON conflict (sha1, property_id) do update set value=excluded.value"
     svalue = json.dumps(value)
-    return await execute_query_many(query, [(sha1, property_id, svalue) for sha1 in sha1_list])
+    return await execute_query_many(query, [(sha1, property_id, svalue) for sha1 in sha1_list])
+
+
+async def get_sha1s_by_filenames(filenames: list[str]) -> list[str]:
+    query = "SELECT sha1 from images where name in " + "(" + ','.join('?' * len(filenames)) + ') order by name'
+    cursor = await execute_query(query, tuple(filenames))
+    return await cursor.fetchall()
```

### Comparing `panoptic-0.0.9.dev6/panoptic/core/db_utils.py` & `panoptic-0.0.9.dev7/panoptic/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/core/image_importer.py` & `panoptic-0.0.9.dev7/panoptic/core/image_importer.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/html/assets/bootstrap-icons-966620f9.woff2` & `panoptic-0.0.9.dev7/panoptic/html/assets/bootstrap-icons-966620f9.woff2`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/html/assets/bootstrap-icons-c6569d46.woff` & `panoptic-0.0.9.dev7/panoptic/html/assets/bootstrap-icons-c6569d46.woff`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/html/assets/index-66fe5260.css` & `panoptic-0.0.9.dev7/panoptic/html/assets/index-66fe5260.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/html/favicon.ico` & `panoptic-0.0.9.dev7/panoptic/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/main.py` & `panoptic-0.0.9.dev7/panoptic/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,18 @@
     # while True:
     #     print("running")
     #     sleep(2)
 
 
 def start():
     root = tk.Tk()
-    root.iconbitmap(os.path.join(os.path.dirname(__file__), "html/favicon.ico"))
+    try:
+        root.iconbitmap(os.path.join(os.path.dirname(__file__), "html/favicon.ico"))
+    except:
+        pass
     thread = Thread(target=launch_uvicorn)
     thread.daemon = True
     thread.start()
     global ui
     ui = MiniUI(root)
 
     root.mainloop()
```

### Comparing `panoptic-0.0.9.dev6/panoptic/models/models.py` & `panoptic-0.0.9.dev7/panoptic/models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     width: int
     height: int
     paths: list[str]
     extension: str
     properties: Optional[dict[int, PropertyValue]] = {}
     vector: Any
     ahash: str|None
+    name: str
 
 
 class ImageVector(BaseModel):
     sha1: str
     vector: numpy.ndarray
     ahash: str
```

### Comparing `panoptic-0.0.9.dev6/panoptic/models/payloads.py` & `panoptic-0.0.9.dev7/panoptic/models/payloads.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/scripts/create_db.sql` & `panoptic-0.0.9.dev7/panoptic/scripts/create_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/scripts/populate_db.sql` & `panoptic-0.0.9.dev7/panoptic/scripts/populate_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic/scripts/to_pca.py` & `panoptic-0.0.9.dev7/panoptic/scripts/to_pca.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev6/panoptic.egg-info/PKG-INFO` & `panoptic-0.0.9.dev7/panoptic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.9.dev6
+Version: 0.0.9.dev7
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.9.dev6/panoptic.egg-info/SOURCES.txt` & `panoptic-0.0.9.dev7/panoptic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 panoptic/core/db.py
 panoptic/core/db_utils.py
 panoptic/core/image_importer.py
 panoptic/html/favicon.ico
 panoptic/html/index.html
 panoptic/html/assets/bootstrap-icons-966620f9.woff2
 panoptic/html/assets/bootstrap-icons-c6569d46.woff
-panoptic/html/assets/index-26ce049e.js
 panoptic/html/assets/index-66fe5260.css
 panoptic/models/__init__.py
 panoptic/models/models.py
 panoptic/models/payloads.py
 panoptic/scripts/__init__.py
 panoptic/scripts/create_db.sql
 panoptic/scripts/populate_db.sql
```

### Comparing `panoptic-0.0.9.dev6/setup.py` & `panoptic-0.0.9.dev7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "panoptic"
-VERSION = "0.0.9.dev6"
+VERSION = "0.0.9.dev7"
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `panoptic-0.0.9.dev6/thunder-collection_Panoptic.json` & `panoptic-0.0.9.dev7/thunder-collection_Panoptic.json`

 * *Files identical despite different names*

