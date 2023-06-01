# Comparing `tmp/keypact-0.8.0.tar.gz` & `tmp/keypact-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.8.0.tar", last modified: Thu Jun  1 13:11:34 2023, max compression
+gzip compressed data, was "keypact-0.9.0.tar", last modified: Thu Jun  1 13:36:32 2023, max compression
```

## Comparing `keypact-0.8.0.tar` & `keypact-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.287673 keypact-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 13:11:24.000000 keypact-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-01 13:11:34.283672 keypact-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-01 13:11:24.000000 keypact-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:11:34.287673 keypact-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 13:11:24.000000 keypact-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.283672 keypact-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.283672 keypact-0.8.0/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 13:11:24.000000 keypact-0.8.0/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-01 13:11:24.000000 keypact-0.8.0/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.283672 keypact-0.8.0/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:36:32.674611 keypact-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 13:36:20.000000 keypact-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-01 13:36:32.674611 keypact-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-01 13:36:20.000000 keypact-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:36:32.674611 keypact-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 13:36:20.000000 keypact-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:36:32.674611 keypact-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:36:32.674611 keypact-0.9.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 13:36:20.000000 keypact-0.9.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-01 13:36:20.000000 keypact-0.9.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:36:32.674611 keypact-0.9.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-01 13:36:32.000000 keypact-0.9.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 13:36:32.000000 keypact-0.9.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:36:32.000000 keypact-0.9.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 13:36:32.000000 keypact-0.9.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:36:32.000000 keypact-0.9.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 13:36:32.000000 keypact-0.9.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 13:36:32.000000 keypact-0.9.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.8.0/LICENSE` & `keypact-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.8.0/PKG-INFO` & `keypact-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.8.0
+Version: 0.9.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -16,14 +16,15 @@
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
         - Able to encryption
         - Able to caching
+        - Able to backup and restore
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

### Comparing `keypact-0.8.0/README.md` & `keypact-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 - Easy to integrate
 - Easy to deploy
 - Able to saving files
 - Able to compressing datas
 - Able to storing pyton objects (Pickle)
 - Able to encryption
 - Able to caching
+- Able to backup and restore
 
 
 ## Installation
 You can install KeyPact by pip3:
 
 ```console
 pip3 install keypact
```

### Comparing `keypact-0.8.0/setup.py` & `keypact-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.8.0',
+version='0.9.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.8.0/src/keypact/keypact.py` & `keypact-0.9.0/src/keypact/keypact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,30 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+from datetime import datetime
 import os
 from hashlib import sha256
 import pickle
 
 import fire
 
 import time
-from shutil import move, copy
+from shutil import move, copy, make_archive, unpack_archive
 
 import mgzip
 
 
 
 import base64
 import hashlib
 from Crypto import Random
 from Crypto.Cipher import AES
 
-
-
-
-def encrypt(key, message):
-    def pad(s):
-        return s + (16 - len(s) % 16) * chr(16 - len(s) % 16)
-    padded_message = pad(message)
-    iv = Random.new().read(AES.block_size)
-    cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
-    return base64.b64encode(iv + cipher.encrypt(padded_message.encode())).decode()
-
-def decrypt(key, message):
-    def unpad(s):
-        return s[:-ord(s[len(s)-1:])]
-    message = base64.b64decode(message.encode())
-    iv = message[:AES.block_size]
-    cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
-    return unpad(cipher.decrypt(message[AES.block_size:])).decode()
-
+import traceback
 
 class KeyPact:
 
     def __init__(self, name):
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "kp-" + self.hashed_name)
@@ -91,15 +74,15 @@
         key_location_loading = os.path.join(self.location, key_location+".l")
         key_location_loading_indicator = os.path.join(self.location, key_location+".li")
 
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         if encryption_key != "None":
-            value = encrypt(encryption_key, value)
+            value = self.encrypt(encryption_key, value)
 
         the_dict = {"key":key,"value":value, "type":type}
 
         if cache_policy != 0:
             the_dict["cache_time"] = time.time()
             the_dict["cache_policy"] = cache_policy
         else:
@@ -155,36 +138,36 @@
 
 
     def set_file_withrkey(self, file, dont_remove: bool = False) -> str:
         key = str(self.counter) + str(time.time())
         return self.set_file(key, file, dont_remove)
 
 
-    def get_file(self, key: str, custom_key_location: str = None):
+    def get_file(self, key: str, custom_key_location: str = ""):
         the_key = self.get(key,custom_key_location)
         return the_key+the_key.split("/")[-1]
 
 
 
 
-    def get(self, key: str, custom_key_location: str = None, encryption_key:str="None", no_cache: bool = False):
+    def get(self, key: str, custom_key_location: str = "", encryption_key:str="None", no_cache: bool = False):
 
         if key in self.cache and not no_cache:
             cache_control = False
             currently = time.time()
             last_time = self.cache[key]["cache_time"]
             cache_policy = self.cache[key]["cache_policy"]
 
             if currently - last_time < cache_policy:
                 cache_control = True
             
             if cache_control:
                 return self.cache[key]["value"]
 
-        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
+        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == "" else custom_key_location
 
         key_location_loading_indicator = os.path.join(self.location, key_location+".li")
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         while os.path.exists(key_location_loading_indicator):
             time.sleep(0.1)
@@ -216,15 +199,15 @@
                     total_result_standart = result
                     try:
                         total_result = result["value"]
                     except TypeError:
                         total_result = result
 
             if encryption_key != "None":
-                total_result = decrypt(encryption_key, total_result)
+                total_result = self.decrypt(encryption_key, total_result)
 
             if "cache_time" in total_result_standart:
                 self.cache[key] = total_result_standart
 
         except EOFError or FileNotFoundError:
             pass
 
@@ -324,10 +307,29 @@
     def size(self, key: str):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         return os.path.getsize(os.path.join(self.location, key_location))
 
+    def backup(self, backup_location: str) -> str:
+        # create a name for backup that a date
+        name = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
+        location = os.path.join(backup_location, name)
+        make_archive(location, 'zip', self.location)
+        move(location+".zip", location+".kp")
+        return location+".kp"
+
+    def restore(self, backup_location: str) -> bool:
+        try:
+            move(backup_location, backup_location.replace(".kp", ".zip"))
+            backup_location = backup_location.replace(".kp", ".zip")
+            unpack_archive(backup_location, self.location)
+            return True
+        except:
+            traceback.print_exc()
+            return False
+
+
 
 def main():
     fire.Fire(KeyPact)
```

### Comparing `keypact-0.8.0/src/keypact.egg-info/PKG-INFO` & `keypact-0.9.0/src/keypact.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.8.0
+Version: 0.9.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -16,14 +16,15 @@
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
         - Able to encryption
         - Able to caching
+        - Able to backup and restore
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

