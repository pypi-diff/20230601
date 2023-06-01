# Comparing `tmp/mindlakesdk-0.9.2.tar.gz` & `tmp/mindlakesdk-0.9.3.tar.gz`

## Comparing `mindlakesdk-0.9.2.tar` & `mindlakesdk-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/requirements.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/README.md
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/__init__.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/cryptor.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/datalake.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/keyhelper.py
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/message.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/permission.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/settings.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/mindlakesdk/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/LICENSE
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mindlakesdk-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/__init__.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/cryptor.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/datalake.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/keyhelper.py
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/message.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/permission.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/settings.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/PKG-INFO
```

### Comparing `mindlakesdk-0.9.2/mindlakesdk/LICENSE` & `mindlakesdk-0.9.3/mindlakesdk/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/mindlakesdk/__init__.py` & `mindlakesdk-0.9.3/mindlakesdk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         
         session.walletAddress = walletAccount.address
         session.appKey = appKey
         if gateway:
             session.gateway = gateway
         else:
             session.gateway = settings.GATEWAY
+        logging.debug('gateway: %s'%session.gateway)
         logging.debug('walletAddress: %s'%session.walletAddress)
 
         result = mindlakesdk.message.getNounce(session)
         if not result:
             self.code = result.code
             self.message = result.message
             self.data = result.data
```

### Comparing `mindlakesdk-0.9.2/mindlakesdk/cryptor.py` & `mindlakesdk-0.9.3/mindlakesdk/cryptor.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/mindlakesdk/datalake.py` & `mindlakesdk-0.9.3/mindlakesdk/datalake.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/mindlakesdk/keyhelper.py` & `mindlakesdk-0.9.3/mindlakesdk/keyhelper.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/mindlakesdk/message.py` & `mindlakesdk-0.9.3/mindlakesdk/message.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/mindlakesdk/permission.py` & `mindlakesdk-0.9.3/mindlakesdk/permission.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/mindlakesdk/settings.py` & `mindlakesdk-0.9.3/mindlakesdk/settings.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/mindlakesdk/utils.py` & `mindlakesdk-0.9.3/mindlakesdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     headers = {}
     headers['Content-Type'] = 'application/json'
     headers['wa'] = session.walletAddress
     headers['ver'] = settings.VERSION
     headers['app'] = session.appKey
     if session.token:
         headers['token'] = session.token
-    response = requests.post(settings.GATEWAY, json=data, headers=headers)
+    response = requests.post(session.gateway, json=data, headers=headers)
     logging.debug("============== Mind SDK request ==============")
     logging.debug('MindSDKHeaders: %s'%headers)
     logging.debug("MindSDKData: %s"%data)
     logging.debug('MindSDKRequest: %s'%response.request.body.decode('utf-8'))
     logging.debug('MindSDKResponse: %s'%response.text)
     if response and response.status_code == 200:
         return json.loads(response.text)
```

### Comparing `mindlakesdk-0.9.2/LICENSE` & `mindlakesdk-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/README.md` & `mindlakesdk-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.2/pyproject.toml` & `mindlakesdk-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mindlakesdk"
-version = "v0.9.2"
+version = "v0.9.3"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to connect to Mind Lake"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mindlakesdk-0.9.2/PKG-INFO` & `mindlakesdk-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindlakesdk
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python SDK to connect to Mind Lake
 Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
 Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
```

