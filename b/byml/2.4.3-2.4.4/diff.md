# Comparing `tmp/byml-2.4.3-py3-none-any.whl.zip` & `tmp/byml-2.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 16351 bytes, number of entries: 12
+Zip file size: 16352 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      113 b- defN 19-Jun-23 10:34 byml/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 23-May-15 11:22 byml/_version.py
--rw-r--r--  2.0 unx    18041 b- defN 20-Mar-21 13:40 byml/byml.py
+-rw-r--r--  2.0 unx      498 b- defN 23-Jun-01 01:12 byml/_version.py
+-rw-r--r--  2.0 unx    18041 b- defN 23-May-31 23:19 byml/byml.py
 -rw-r--r--  2.0 unx     1522 b- defN 20-Aug-11 15:45 byml/byml_to_yml.py
 -rw-r--r--  2.0 unx     1379 b- defN 20-Mar-21 13:16 byml/yaml_util.py
 -rw-r--r--  2.0 unx     1615 b- defN 23-May-15 11:20 byml/yml_to_byml.py
--rw-r--r--  2.0 unx    17879 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3015 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       90 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      903 b- defN 23-May-15 11:22 byml-2.4.3.dist-info/RECORD
-12 files, 45152 bytes uncompressed, 14857 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx    17879 b- defN 23-Jun-01 01:12 byml-2.4.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3015 b- defN 23-Jun-01 01:12 byml-2.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 01:12 byml-2.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-01 01:12 byml-2.4.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-01 01:12 byml-2.4.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      903 b- defN 23-Jun-01 01:12 byml-2.4.4.dist-info/RECORD
+12 files, 45152 bytes uncompressed, 14858 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: byml/yaml_util.py
 Comment: 
 
 Filename: byml/yml_to_byml.py
 Comment: 
 
-Filename: byml-2.4.3.dist-info/LICENSE
+Filename: byml-2.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: byml-2.4.3.dist-info/METADATA
+Filename: byml-2.4.4.dist-info/METADATA
 Comment: 
 
-Filename: byml-2.4.3.dist-info/WHEEL
+Filename: byml-2.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: byml-2.4.3.dist-info/entry_points.txt
+Filename: byml-2.4.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: byml-2.4.3.dist-info/top_level.txt
+Filename: byml-2.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: byml-2.4.3.dist-info/RECORD
+Filename: byml-2.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## byml/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-05-15T12:18:44+0100",
+ "date": "2023-06-01T02:12:06+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "17770f9d34f09a3d8f9e982120537c4d287c2e43",
- "version": "v2.4.3"
+ "full-revisionid": "f79c6b7cf45cb5f8da4e2f841e7ae17eb56d6ccc",
+ "version": "v2.4.4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## byml/byml.py

```diff
@@ -63,16 +63,16 @@
             self._be = True
         elif magic == b'YB':
             self._be = False
         else:
             raise ValueError("Invalid magic: %s (expected 'BY' or 'YB')" % magic)
 
         version = self._read_u16(2)
-        if not (1 <= version <= 4):
-            raise ValueError("Invalid version: %u (expected 1-4)" % version)
+        if not (1 <= version <= 7):
+            raise ValueError("Invalid version: %u (expected 1-7)" % version)
         if version == 1 and self._be:
             raise ValueError("Invalid version: %u-wiiu (expected 1-3)" % version)
 
         self._hash_key_table_offset = self._read_u32(4)
         self._string_table_offset = self._read_u32(8)
 
         if self._hash_key_table_offset != 0:
@@ -227,16 +227,16 @@
         self._data = data
         self._be = be
         self._version = version
 
         if not isinstance(data, list) and not isinstance(data, dict):
             raise ValueError("Data should be a dict or a list")
 
-        if not (1 <= version <= 4):
-            raise ValueError("Invalid version: %u (expected 1-4)" % version)
+        if not (1 <= version <= 7):
+            raise ValueError("Invalid version: %u (expected 1-7)" % version)
         if version == 1 and be:
             raise ValueError("Invalid version: %u-wiiu (expected 1-3)" % version)
 
         self._hash_key_table: SortedDict[str, int] = SortedDict()
         self._string_table: SortedDict[str, int] = SortedDict()
         self._make_string_table(self._data, self._hash_key_table, self._string_table)
         # Nintendo seems to sort entries in alphabetical order.
```

## Comparing `byml-2.4.3.dist-info/LICENSE` & `byml-2.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `byml-2.4.3.dist-info/METADATA` & `byml-2.4.4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: byml
-Version: 2.4.3
+Version: 2.4.4
 Summary: A simple Nintendo BYML or BYAML v2/v3 parser and writer
 Home-page: https://github.com/leoetlino/byml-v2
 Author: leoetlino
 Author-email: leo@leolam.fr
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYAML (~=5.1)
+Requires-Dist: PyYAML (~=6.0)
 Requires-Dist: oead (~=1.1)
 Requires-Dist: sortedcontainers (~=2.0)
 
 ## Simple bymlv2 parser + writer + converters
 
 Features:
```

## Comparing `byml-2.4.3.dist-info/RECORD` & `byml-2.4.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 byml/__init__.py,sha256=WUcmRBw7EMVmZrUeC9isKi-KJAvrMFsDAp0tVK34M3Y,113
-byml/_version.py,sha256=PD2uX6K45zijbZbGB9LEfiPSWpvNvwsH0hyHuHAGyrU,498
-byml/byml.py,sha256=orUPUP3opb2qvSMTlxPZuYt-w6laAx7zkL4fkOh7ZC4,18041
+byml/_version.py,sha256=h59YuxaIM9DaRhUKMHDuOUK0kkXk4vB8d_p9lMNXCV8,498
+byml/byml.py,sha256=l0KwJWVXiENWxn0vi7DL10zeglNUoTahkuryQpVj1bk,18041
 byml/byml_to_yml.py,sha256=V0BXl26w4Pa-655FRwDIG6_zIOZ2xEEYvU2RT79ZznM,1522
 byml/yaml_util.py,sha256=xB3Z4hGZCPm1y4qFCK3ZyVLY75UAUZWrqn7InyAbv-0,1379
 byml/yml_to_byml.py,sha256=NozXJ7pf6dmOJpyqba-aAw5A-aMbC09B-SAtqVvwXRA,1615
-byml-2.4.3.dist-info/LICENSE,sha256=MVVce6oSrBFQvJpI-22FtV2c6hM2rjr6k9ZT9o_km7I,17879
-byml-2.4.3.dist-info/METADATA,sha256=IV_sS-39fZ5RFYzh1y55aod_7cTuYjGiO-6PErwMcLg,3015
-byml-2.4.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-byml-2.4.3.dist-info/entry_points.txt,sha256=5tQRomryYvz8yPbY5gMWEaeRopSXiLniNJNfVBaUsnA,90
-byml-2.4.3.dist-info/top_level.txt,sha256=DZ9pR2xSDQetNBG3oI8GsBwnfG2ohwFsMojhWdWwqbs,5
-byml-2.4.3.dist-info/RECORD,,
+byml-2.4.4.dist-info/LICENSE,sha256=MVVce6oSrBFQvJpI-22FtV2c6hM2rjr6k9ZT9o_km7I,17879
+byml-2.4.4.dist-info/METADATA,sha256=aNtwW7tYviEjESawDIPYR-CMrPuAv8qnp8c0pjtsOlw,3015
+byml-2.4.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+byml-2.4.4.dist-info/entry_points.txt,sha256=5tQRomryYvz8yPbY5gMWEaeRopSXiLniNJNfVBaUsnA,90
+byml-2.4.4.dist-info/top_level.txt,sha256=DZ9pR2xSDQetNBG3oI8GsBwnfG2ohwFsMojhWdWwqbs,5
+byml-2.4.4.dist-info/RECORD,,
```

