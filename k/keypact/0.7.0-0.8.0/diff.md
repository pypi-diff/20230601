# Comparing `tmp/keypact-0.7.0.tar.gz` & `tmp/keypact-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.7.0.tar", last modified: Thu Jun  1 10:59:09 2023, max compression
+gzip compressed data, was "keypact-0.8.0.tar", last modified: Thu Jun  1 13:11:34 2023, max compression
```

## Comparing `keypact-0.7.0.tar` & `keypact-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 10:58:59.000000 keypact-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-01 10:59:09.550456 keypact-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-01 10:58:59.000000 keypact-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 10:59:09.554456 keypact-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 10:58:59.000000 keypact-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 10:58:59.000000 keypact-0.7.0/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-01 10:58:59.000000 keypact-0.7.0/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:59:09.550456 keypact-0.7.0/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 10:59:09.000000 keypact-0.7.0/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.287673 keypact-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 13:11:24.000000 keypact-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-01 13:11:34.283672 keypact-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-01 13:11:24.000000 keypact-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:11:34.287673 keypact-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 13:11:24.000000 keypact-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.283672 keypact-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.283672 keypact-0.8.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 13:11:24.000000 keypact-0.8.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-01 13:11:24.000000 keypact-0.8.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:34.283672 keypact-0.8.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 13:11:34.000000 keypact-0.8.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.7.0/LICENSE` & `keypact-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.7.0/PKG-INFO` & `keypact-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.7.0
+Version: 0.8.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -15,14 +15,15 @@
         - Easy to use
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
         - Able to encryption
+        - Able to caching
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

### Comparing `keypact-0.7.0/README.md` & `keypact-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 - Easy to use
 - Easy to integrate
 - Easy to deploy
 - Able to saving files
 - Able to compressing datas
 - Able to storing pyton objects (Pickle)
 - Able to encryption
+- Able to caching
 
 
 ## Installation
 You can install KeyPact by pip3:
 
 ```console
 pip3 install keypact
```

### Comparing `keypact-0.7.0/setup.py` & `keypact-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.7.0',
+version='0.8.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.7.0/src/keypact/keypact.py` & `keypact-0.8.0/src/keypact/keypact.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "kp-" + self.hashed_name)
 
 
         self.counter = 0
 
+        self.cache = {}
+
         self.initialize()
 
     def initialize(self):
         try: 
             os.makedirs(self.location)
         except OSError:
             if not os.path.isdir(self.location):
@@ -72,15 +74,15 @@
         def unpad(s):
             return s[:-ord(s[len(s)-1:])]
         message = base64.b64decode(message.encode())
         iv = message[:AES.block_size]
         cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
         return unpad(cipher.decrypt(message[AES.block_size:])).decode()
 
-    def set(self, key: str, value, type_of_value: str ="str", compress: bool=False, encryption_key:str="None") -> str:
+    def set(self, key: str, value, type_of_value: str ="str", compress: bool=False, encryption_key:str="None", cache_policy: int = 0, dont_delete_cache: bool=False) -> str:
         self.counter += 1
         
         
 
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
@@ -91,25 +93,35 @@
 
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         if encryption_key != "None":
             value = encrypt(encryption_key, value)
 
+        the_dict = {"key":key,"value":value, "type":type}
+
+        if cache_policy != 0:
+            the_dict["cache_time"] = time.time()
+            the_dict["cache_policy"] = cache_policy
+        else:
+            if key in self.cache and not dont_delete_cache:
+                del self.cache[key]
+
+
         if compress:
             # create key_location_compress_indicator
             with open(key_location_compress_indicator, "wb") as f:
                 f.write(b"1")
 
             with mgzip.open(key_location_loading, "wb") as f:
-                pickle.dump({"key":key,"value":value, "type":type}, f)
+                pickle.dump(the_dict, f)
         
         else:
             with open(key_location_loading, "wb") as f:
-                pickle.dump({"key":key,"value":value, "type":type}, f)
+                pickle.dump(the_dict, f)
 
 
 
 
         #Create a file that inform is loading
         with open(key_location_loading_indicator, "wb") as f:
             f.write(b"1")
@@ -150,15 +162,28 @@
     def get_file(self, key: str, custom_key_location: str = None):
         the_key = self.get(key,custom_key_location)
         return the_key+the_key.split("/")[-1]
 
 
 
 
-    def get(self, key: str, custom_key_location: str = None, encryption_key:str="None"):
+    def get(self, key: str, custom_key_location: str = None, encryption_key:str="None", no_cache: bool = False):
+
+        if key in self.cache and not no_cache:
+            cache_control = False
+            currently = time.time()
+            last_time = self.cache[key]["cache_time"]
+            cache_policy = self.cache[key]["cache_policy"]
+
+            if currently - last_time < cache_policy:
+                cache_control = True
+            
+            if cache_control:
+                return self.cache[key]["value"]
+
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
 
         key_location_loading_indicator = os.path.join(self.location, key_location+".li")
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         while os.path.exists(key_location_loading_indicator):
@@ -167,41 +192,49 @@
 
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
 
         total_result = None
 
+        total_result_standart = None
+
         try:
             
             with open(key_location_reading_indicator, "wb") as f:
                 f.write(b"1")
             if os.path.exists(key_location_compress_indicator):
                 with mgzip.open(os.path.join(self.location, key_location), "rb") as f:
                     result = pickle.load(f)
+                    total_result_standart = result
                     try:
                         total_result = result["value"]
                     except TypeError:
                         total_result = result
             else:
                 with open(os.path.join(self.location, key_location), "rb") as f:
                     result = pickle.load(f)
+                    total_result_standart = result
                     try:
                         total_result = result["value"]
                     except TypeError:
                         total_result = result
+
+            if encryption_key != "None":
+                total_result = decrypt(encryption_key, total_result)
+
+            if "cache_time" in total_result_standart:
+                self.cache[key] = total_result_standart
+
         except EOFError or FileNotFoundError:
             pass
 
         if os.path.isfile(key_location_reading_indicator):
             os.remove(key_location_reading_indicator)
 
-        if encryption_key != "None":
-            total_result = decrypt(encryption_key, total_result)
-
         return total_result
 
     def get_key(self, key_location: str):
        
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
@@ -209,23 +242,31 @@
 
         try:
             if os.path.exists(key_location_compress_indicator):
                 with mgzip.open(os.path.join(self.location, key_location), "rb") as f:
                     result = pickle.load(f)
                     if not "type" in result:
                         result["type"] = "str"
+                    if not "cache_time" in result:
+                        result["cache_time"] = 0
+                    if not "cache_policy" in result:
+                        result["cache_policy"] = 0
                     try:
                         total_result = result["key"]
                     except TypeError:
                         total_result = False            
             else:
                 with open(os.path.join(self.location, key_location), "rb") as f:
                     result = pickle.load(f)
                     if not "type" in result:
                         result["type"] = "str"
+                    if not "cache_time" in result:
+                        result["cache_time"] = 0
+                    if not "cache_policy" in result:
+                        result["cache_policy"] = 0
                     try:
                         total_result = result["key"]
                     except TypeError:
                         total_result = False
         except EOFError or FileNotFoundError:
             pass            
         return total_result
```

### Comparing `keypact-0.7.0/src/keypact.egg-info/PKG-INFO` & `keypact-0.8.0/src/keypact.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.7.0
+Version: 0.8.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -15,14 +15,15 @@
         - Easy to use
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
         - Able to encryption
+        - Able to caching
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

