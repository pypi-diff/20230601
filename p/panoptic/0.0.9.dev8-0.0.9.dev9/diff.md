# Comparing `tmp/panoptic-0.0.9.dev8.tar.gz` & `tmp/panoptic-0.0.9.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptic-0.0.9.dev8.tar", last modified: Thu Jun  1 09:34:32 2023, max compression
+gzip compressed data, was "panoptic-0.0.9.dev9.tar", last modified: Thu Jun  1 15:50:05 2023, max compression
```

## Comparing `panoptic-0.0.9.dev8.tar` & `panoptic-0.0.9.dev9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.448303 panoptic-0.0.9.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 09:34:32.448303 panoptic-0.0.9.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/build_commans.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.444303 panoptic-0.0.9.dev8/panoptic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.444303 panoptic-0.0.9.dev8/panoptic/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/compute/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/compute/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/compute/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.444303 panoptic-0.0.9.dev8/panoptic/core/
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/core/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/core/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/core/image_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.448303 panoptic-0.0.9.dev8/panoptic/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.448303 panoptic-0.0.9.dev8/panoptic/html/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/html/assets/bootstrap-icons-966620f9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/html/assets/bootstrap-icons-c6569d46.woff
--rw-r--r--   0 runner    (1001) docker     (123)   323661 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/html/assets/index-43ae5eb5.js
--rw-r--r--   0 runner    (1001) docker     (123)   430321 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/html/assets/index-66fe5260.css
--rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/html/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.448303 panoptic-0.0.9.dev8/panoptic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/models/payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.448303 panoptic-0.0.9.dev8/panoptic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/scripts/create_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/scripts/populate_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/panoptic/scripts/to_pca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:34:32.444303 panoptic-0.0.9.dev8/panoptic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 09:34:32.000000 panoptic-0.0.9.dev8/panoptic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 09:34:32.000000 panoptic-0.0.9.dev8/panoptic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:34:32.000000 panoptic-0.0.9.dev8/panoptic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 09:34:32.000000 panoptic-0.0.9.dev8/panoptic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 09:34:32.000000 panoptic-0.0.9.dev8/panoptic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 09:34:32.000000 panoptic-0.0.9.dev8/panoptic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:34:32.448303 panoptic-0.0.9.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-01 09:34:20.000000 panoptic-0.0.9.dev8/thunder-collection_Panoptic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.904106 panoptic-0.0.9.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 15:50:05.904106 panoptic-0.0.9.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/build_commans.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.900106 panoptic-0.0.9.dev9/panoptic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.900106 panoptic-0.0.9.dev9/panoptic/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/compute/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/compute/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/compute/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.900106 panoptic-0.0.9.dev9/panoptic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/core/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/core/image_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.900106 panoptic-0.0.9.dev9/panoptic/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.904106 panoptic-0.0.9.dev9/panoptic/html/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/html/assets/bootstrap-icons-966620f9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/html/assets/bootstrap-icons-c6569d46.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   430321 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/html/assets/index-66fe5260.css
+-rw-r--r--   0 runner    (1001) docker     (123)   323652 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/html/assets/index-7472937f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/html/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.904106 panoptic-0.0.9.dev9/panoptic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/models/payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.904106 panoptic-0.0.9.dev9/panoptic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/scripts/create_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/scripts/populate_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/panoptic/scripts/to_pca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:05.900106 panoptic-0.0.9.dev9/panoptic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 15:50:05.000000 panoptic-0.0.9.dev9/panoptic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 15:50:05.000000 panoptic-0.0.9.dev9/panoptic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:50:05.000000 panoptic-0.0.9.dev9/panoptic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 15:50:05.000000 panoptic-0.0.9.dev9/panoptic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 15:50:05.000000 panoptic-0.0.9.dev9/panoptic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 15:50:05.000000 panoptic-0.0.9.dev9/panoptic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:50:05.904106 panoptic-0.0.9.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-01 15:49:52.000000 panoptic-0.0.9.dev9/thunder-collection_Panoptic.json
```

### Comparing `panoptic-0.0.9.dev8/PKG-INFO` & `panoptic-0.0.9.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.9.dev8
+Version: 0.0.9.dev9
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.9.dev8/description.md` & `panoptic-0.0.9.dev9/description.md`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/api.py` & `panoptic-0.0.9.dev9/panoptic/api.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/compute/ocr.py` & `panoptic-0.0.9.dev9/panoptic/compute/ocr.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/compute/similarity.py` & `panoptic-0.0.9.dev9/panoptic/compute/similarity.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/compute/transform.py` & `panoptic-0.0.9.dev9/panoptic/compute/transform.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/compute/utils.py` & `panoptic-0.0.9.dev9/panoptic/compute/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/core/__init__.py` & `panoptic-0.0.9.dev9/panoptic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/core/db.py` & `panoptic-0.0.9.dev9/panoptic/core/db.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/core/db_utils.py` & `panoptic-0.0.9.dev9/panoptic/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/core/image_importer.py` & `panoptic-0.0.9.dev9/panoptic/core/image_importer.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/html/assets/bootstrap-icons-966620f9.woff2` & `panoptic-0.0.9.dev9/panoptic/html/assets/bootstrap-icons-966620f9.woff2`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/html/assets/bootstrap-icons-c6569d46.woff` & `panoptic-0.0.9.dev9/panoptic/html/assets/bootstrap-icons-c6569d46.woff`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/html/assets/index-43ae5eb5.js` & `panoptic-0.0.9.dev9/panoptic/html/assets/index-7472937f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -15048,15 +15048,15 @@
                 function p(_, b) {
                     let w = _.images,
                         S = b[0],
                         D = new SO(Array),
                         M = T.properties[S].type;
                     for (let H of w) {
                         let z = S in H.properties ? H.properties[S].value : "undefined";
-                        (z == null || z == "") && (z = void 0), M == B.checkbox && z != !0 && (z = !1), Array.isArray(z) && z.forEach(U => D[U].push(H)), M == B.date ? D[G(z).format("YYYY/MM")].push(H) : D[z].push(H)
+                        z == null || z == "" ? z = void 0 : M == B.checkbox && z != !0 ? z = !1 : Array.isArray(z) ? z.forEach(U => D[U].push(H)) : M == B.date ? D[G(z).format("YYYY/MM")].push(H) : D[z].push(H)
                     }
                     let L = [];
                     for (let H of Object.keys(D).sort()) L.push({
                         name: H,
                         images: D[H],
                         groups: void 0,
                         count: D[H].length,
```

### Comparing `panoptic-0.0.9.dev8/panoptic/html/assets/index-66fe5260.css` & `panoptic-0.0.9.dev9/panoptic/html/assets/index-66fe5260.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/html/favicon.ico` & `panoptic-0.0.9.dev9/panoptic/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/main.py` & `panoptic-0.0.9.dev9/panoptic/main.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/models/models.py` & `panoptic-0.0.9.dev9/panoptic/models/models.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/models/payloads.py` & `panoptic-0.0.9.dev9/panoptic/models/payloads.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/scripts/create_db.sql` & `panoptic-0.0.9.dev9/panoptic/scripts/create_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/scripts/populate_db.sql` & `panoptic-0.0.9.dev9/panoptic/scripts/populate_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic/scripts/to_pca.py` & `panoptic-0.0.9.dev9/panoptic/scripts/to_pca.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.9.dev8/panoptic.egg-info/PKG-INFO` & `panoptic-0.0.9.dev9/panoptic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.9.dev8
+Version: 0.0.9.dev9
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.9.dev8/panoptic.egg-info/SOURCES.txt` & `panoptic-0.0.9.dev9/panoptic.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 panoptic/core/db.py
 panoptic/core/db_utils.py
 panoptic/core/image_importer.py
 panoptic/html/favicon.ico
 panoptic/html/index.html
 panoptic/html/assets/bootstrap-icons-966620f9.woff2
 panoptic/html/assets/bootstrap-icons-c6569d46.woff
-panoptic/html/assets/index-43ae5eb5.js
 panoptic/html/assets/index-66fe5260.css
+panoptic/html/assets/index-7472937f.js
 panoptic/models/__init__.py
 panoptic/models/models.py
 panoptic/models/payloads.py
 panoptic/scripts/__init__.py
 panoptic/scripts/create_db.sql
 panoptic/scripts/populate_db.sql
 panoptic/scripts/to_pca.py
```

### Comparing `panoptic-0.0.9.dev8/setup.py` & `panoptic-0.0.9.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "panoptic"
-VERSION = "0.0.9.dev8"
+VERSION = "0.0.9.dev9"
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `panoptic-0.0.9.dev8/thunder-collection_Panoptic.json` & `panoptic-0.0.9.dev9/thunder-collection_Panoptic.json`

 * *Files identical despite different names*

