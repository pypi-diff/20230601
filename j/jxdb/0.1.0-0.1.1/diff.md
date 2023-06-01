# Comparing `tmp/jxdb-0.1.0.tar.gz` & `tmp/jxdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jxdb-0.1.0.tar", last modified: Tue May 30 05:17:45 2023, max compression
+gzip compressed data, was "jxdb-0.1.1.tar", last modified: Thu Jun  1 19:45:44 2023, max compression
```

## Comparing `jxdb-0.1.0.tar` & `jxdb-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 05:17:45.082498 jxdb-0.1.0/
--rw-rw-rw-   0        0        0     1351 2023-05-30 04:54:06.000000 jxdb-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3264 2023-05-30 05:17:45.081501 jxdb-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1252 2023-05-30 05:17:08.000000 jxdb-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 05:17:45.062453 jxdb-0.1.0/jxdb/
--rw-rw-rw-   0        0        0     2834 2023-05-30 05:08:42.000000 jxdb-0.1.0/jxdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:17:45.080504 jxdb-0.1.0/jxdb.egg-info/
--rw-rw-rw-   0        0        0     3264 2023-05-30 05:17:45.000000 jxdb-0.1.0/jxdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-30 05:17:45.000000 jxdb-0.1.0/jxdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 05:17:45.000000 jxdb-0.1.0/jxdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-30 05:17:45.000000 jxdb-0.1.0/jxdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-30 05:17:45.000000 jxdb-0.1.0/jxdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 05:17:45.082498 jxdb-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      882 2023-05-30 05:17:35.000000 jxdb-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:45:44.912036 jxdb-0.1.1/
+-rw-rw-rw-   0        0        0     1366 2023-06-01 19:44:31.000000 jxdb-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5157 2023-06-01 19:45:44.911038 jxdb-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2023-06-01 19:45:34.000000 jxdb-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:45:44.884141 jxdb-0.1.1/jxdb/
+-rw-rw-rw-   0        0        0     2811 2023-06-01 19:45:07.000000 jxdb-0.1.1/jxdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:45:44.910072 jxdb-0.1.1/jxdb.egg-info/
+-rw-rw-rw-   0        0        0     5157 2023-06-01 19:45:44.000000 jxdb-0.1.1/jxdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-01 19:45:44.000000 jxdb-0.1.1/jxdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:45:44.000000 jxdb-0.1.1/jxdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 19:45:44.000000 jxdb-0.1.1/jxdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-01 19:45:44.000000 jxdb-0.1.1/jxdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:45:44.912036 jxdb-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      882 2023-06-01 19:44:53.000000 jxdb-0.1.1/setup.py
```

### Comparing `jxdb-0.1.0/LICENSE` & `jxdb-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-OpenSociety License
-
-Copyright (c) 2023 xinyc
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-1. Non-Commercial Use: In non-commercial use of the Software, there is no requirement to attribute the author.
-
-2. Commercial Use: In commercial use of the Software, proper attribution of the author is required.
-
-3. Modification: Any person may modify the Software based on the aforementioned conditions and distribute their modifications.
-
-4. Grant of License: This license allows any person to apply this license to their own software products, subject to the terms and conditions herein.
-
-5. No Warranty: The Software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. The author of the Software shall not be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the Software or the use or other dealings in the Software.
+OpenSociety License
+
+Copyright (c) 2023 xinyc
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+1. Non-Commercial Use: In non-commercial use of the Software, there is no requirement to attribute the author.
+
+2. Commercial Use: In commercial use of the Software, proper attribution of the author is required.
+
+3. Modification: Any person may modify the Software based on the aforementioned conditions and distribute their modifications.
+
+4. Grant of License: This license allows any person to apply this license to their own software products, subject to the terms and conditions herein.
+
+5. No Warranty: The Software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. The author of the Software shall not be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the Software or the use or other dealings in the Software.
```

### Comparing `jxdb-0.1.0/jxdb/__init__.py` & `jxdb-0.1.1/jxdb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 from Crypto.Random import get_random_bytes
 from Crypto.Protocol.KDF import PBKDF2
 
+
 class JsonDB:
     def __init__(self):
         self.data = {}
 
     def open(self, filename, password):
         with open(filename, 'rb') as file:
             encrypted_data = file.read()
@@ -48,20 +49,20 @@
 
     def concept(self, data):
         result = []
         for key, value in self.data.items():
             if data in key:
                 result.append(value)
         return result
-    
+
     def keyconcept(self, data):
         result = []
         for key in self.data.keys():
             if data in key:
-                result.append(self.data[key])
+                result.append(key)
         return result
 
     def keys(self):
         return list(self.data.keys())
 
     def values(self):
         return list(self.data.values())
@@ -86,9 +87,7 @@
     def delete_by_key(self, key):
         keys_to_delete = []
         for k in self.data.keys():
             if key in k:
                 keys_to_delete.append(k)
         for k in keys_to_delete:
             del self.data[k]
-    
-
```

### Comparing `jxdb-0.1.0/setup.py` & `jxdb-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     license_text = file.read()
 
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='jxdb',
-    version='0.1.0',
+    version='0.1.1',
     description='Secured Python Json Database',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='xinyc',
     author_email='csecinside@proton.me',
     url='https://github.com/ent1tydev/jxdb',
     license=license_text,
```

