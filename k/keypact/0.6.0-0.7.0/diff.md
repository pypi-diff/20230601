# Comparing `tmp/keypact-0.6.0.tar.gz` & `tmp/keypact-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.6.0.tar", last modified: Wed May 31 15:46:23 2023, max compression
+gzip compressed data, was "keypact-0.7.0.tar", last modified: Thu Jun  1 10:59:09 2023, max compression
```

## Comparing `keypact-0.6.0.tar` & `keypact-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 15:46:09.000000 keypact-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 15:46:23.406116 keypact-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-31 15:46:09.000000 keypact-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:46:23.406116 keypact-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 15:46:09.000000 keypact-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 15:46:09.000000 keypact-0.6.0/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-31 15:46:09.000000 keypact-0.6.0/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 10:58:59.000000 keypact-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-01 10:59:09.550456 keypact-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-01 10:58:59.000000 keypact-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 10:59:09.554456 keypact-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 10:58:59.000000 keypact-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 10:58:59.000000 keypact-0.7.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-01 10:58:59.000000 keypact-0.7.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.6.0/LICENSE` & `keypact-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.6.0/PKG-INFO` & `keypact-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.6.0
+Version: 0.7.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -14,14 +14,15 @@
         - Simultaneous Writing
         - Easy to use
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
+        - Able to encryption
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

### Comparing `keypact-0.6.0/README.md` & `keypact-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - Simultaneous Writing
 - Easy to use
 - Easy to integrate
 - Easy to deploy
 - Able to saving files
 - Able to compressing datas
 - Able to storing pyton objects (Pickle)
+- Able to encryption
 
 
 ## Installation
 You can install KeyPact by pip3:
 
 ```console
 pip3 install keypact
```

### Comparing `keypact-0.6.0/setup.py` & `keypact-0.7.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.6.0',
+version='0.7.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
 packages=["keypact"],
 package_dir={'':'src'},
 install_requires=[
     "fire==0.5.0",
-    "mgzip==0.2.1"
+    "mgzip==0.2.1",
+    "pycryptodome==3.18.0"
 ],
 entry_points = {
     'console_scripts': ['keypact=keypact.keypact:main'],
 },
 python_requires=">= 3",
 zip_safe=False)
```

### Comparing `keypact-0.6.0/src/keypact/keypact.py` & `keypact-0.7.0/src/keypact/keypact.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,40 @@
 
 import time
 from shutil import move, copy
 
 import mgzip
 
 
+
+import base64
+import hashlib
+from Crypto import Random
+from Crypto.Cipher import AES
+
+
+
+
+def encrypt(key, message):
+    def pad(s):
+        return s + (16 - len(s) % 16) * chr(16 - len(s) % 16)
+    padded_message = pad(message)
+    iv = Random.new().read(AES.block_size)
+    cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
+    return base64.b64encode(iv + cipher.encrypt(padded_message.encode())).decode()
+
+def decrypt(key, message):
+    def unpad(s):
+        return s[:-ord(s[len(s)-1:])]
+    message = base64.b64decode(message.encode())
+    iv = message[:AES.block_size]
+    cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
+    return unpad(cipher.decrypt(message[AES.block_size:])).decode()
+
+
 class KeyPact:
 
     def __init__(self, name):
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "kp-" + self.hashed_name)
 
@@ -28,15 +54,33 @@
     def initialize(self):
         try: 
             os.makedirs(self.location)
         except OSError:
             if not os.path.isdir(self.location):
                 raise
 
-    def set(self, key: str, value, type_of_value: str ="str", compress: bool=False) -> str:
+
+
+    def encrypt(self, key, message):
+        def pad(s):
+            return s + (16 - len(s) % 16) * chr(16 - len(s) % 16)
+        padded_message = pad(message)
+        iv = Random.new().read(AES.block_size)
+        cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
+        return base64.b64encode(iv + cipher.encrypt(padded_message.encode())).decode()
+
+    def decrypt(self, key, message):
+        def unpad(s):
+            return s[:-ord(s[len(s)-1:])]
+        message = base64.b64decode(message.encode())
+        iv = message[:AES.block_size]
+        cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
+        return unpad(cipher.decrypt(message[AES.block_size:])).decode()
+
+    def set(self, key: str, value, type_of_value: str ="str", compress: bool=False, encryption_key:str="None") -> str:
         self.counter += 1
         
         
 
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
@@ -44,15 +88,16 @@
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
         key_location_loading = os.path.join(self.location, key_location+".l")
         key_location_loading_indicator = os.path.join(self.location, key_location+".li")
 
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
-        
+        if encryption_key != "None":
+            value = encrypt(encryption_key, value)
 
         if compress:
             # create key_location_compress_indicator
             with open(key_location_compress_indicator, "wb") as f:
                 f.write(b"1")
 
             with mgzip.open(key_location_loading, "wb") as f:
@@ -105,15 +150,15 @@
     def get_file(self, key: str, custom_key_location: str = None):
         the_key = self.get(key,custom_key_location)
         return the_key+the_key.split("/")[-1]
 
 
 
 
-    def get(self, key: str, custom_key_location: str = None):
+    def get(self, key: str, custom_key_location: str = None, encryption_key:str="None"):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
 
         key_location_loading_indicator = os.path.join(self.location, key_location+".li")
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         while os.path.exists(key_location_loading_indicator):
@@ -146,14 +191,17 @@
                         total_result = result
         except EOFError or FileNotFoundError:
             pass
 
         if os.path.isfile(key_location_reading_indicator):
             os.remove(key_location_reading_indicator)
 
+        if encryption_key != "None":
+            total_result = decrypt(encryption_key, total_result)
+
         return total_result
 
     def get_key(self, key_location: str):
        
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
@@ -205,22 +253,22 @@
         self.delete(key)
         
 
     def delete_all(self):
         for key in self.dict():
             self.delete(key)
 
-    def dict(self):
+    def dict(self, encryption_key:str="None"):
         result ={}
         for key in os.listdir(self.location):
             if not "." in key:
                 the_key = self.get_key(key)
                 if not the_key is None:
                     if the_key != False:
-                        result_of_key = self.get(the_key)
+                        result_of_key = self.get(the_key, encryption_key=encryption_key)
                         if not result_of_key is None:
                             result[the_key] = result_of_key
         return result
 
     def size_all(self):
         #Calculate self.location size
         total_size = 0
```

### Comparing `keypact-0.6.0/src/keypact.egg-info/PKG-INFO` & `keypact-0.7.0/src/keypact.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.6.0
+Version: 0.7.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -14,14 +14,15 @@
         - Simultaneous Writing
         - Easy to use
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
+        - Able to encryption
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

