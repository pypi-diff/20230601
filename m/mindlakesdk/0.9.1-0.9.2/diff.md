# Comparing `tmp/mindlakesdk-0.9.1.tar.gz` & `tmp/mindlakesdk-0.9.2.tar.gz`

## Comparing `mindlakesdk-0.9.1.tar` & `mindlakesdk-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/requirements.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/README.md
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/__init__.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/cryptor.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/datalake.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/keyhelper.py
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/message.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/permission.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/settings.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/mindlakesdk/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/LICENSE
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mindlakesdk-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/README.md
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/__init__.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/cryptor.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/datalake.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/keyhelper.py
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/message.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/permission.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/settings.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/PKG-INFO
```

### Comparing `mindlakesdk-0.9.1/mindlakesdk/LICENSE` & `mindlakesdk-0.9.2/mindlakesdk/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/mindlakesdk/__init__.py` & `mindlakesdk-0.9.2/mindlakesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/mindlakesdk/cryptor.py` & `mindlakesdk-0.9.2/mindlakesdk/cryptor.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/mindlakesdk/datalake.py` & `mindlakesdk-0.9.2/mindlakesdk/datalake.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/mindlakesdk/keyhelper.py` & `mindlakesdk-0.9.2/mindlakesdk/keyhelper.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/mindlakesdk/message.py` & `mindlakesdk-0.9.2/mindlakesdk/message.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/mindlakesdk/permission.py` & `mindlakesdk-0.9.2/mindlakesdk/permission.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/mindlakesdk/settings.py` & `mindlakesdk-0.9.2/mindlakesdk/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# GATEWAY = 'http://121.40.82.244:18801/node'
-# GATEWAY = 'http://sdk.mindnetwork.xyz/node'
-GATEWAY = 'http://sdk.mindnetwork.io/node'
-# GATEWAY = 'http://localhost:18802/node'
+GATEWAY = 'http://sdk.mindnetwork.xyz/node'
 WEB3API = 'https://goerli.infura.io/v3/744c0ade89464e4b867ca1b002a10231'
 CONTRACT_ADDRESS = '0xF5932e67e84F08965DC6D62C2B67f47a6826E5a7'
 CONTRACT_ABI = [
         {
                 "anonymous": False,
                 "inputs": [
                         {
```

### Comparing `mindlakesdk-0.9.1/mindlakesdk/utils.py` & `mindlakesdk-0.9.2/mindlakesdk/utils.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/LICENSE` & `mindlakesdk-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/README.md` & `mindlakesdk-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.1/pyproject.toml` & `mindlakesdk-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mindlakesdk"
-version = "v0.9.1"
+version = "v0.9.2"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to connect to Mind Lake"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mindlakesdk-0.9.1/PKG-INFO` & `mindlakesdk-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindlakesdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python SDK to connect to Mind Lake
 Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
 Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
```

