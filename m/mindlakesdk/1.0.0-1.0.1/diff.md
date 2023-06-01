# Comparing `tmp/mindlakesdk-1.0.0.tar.gz` & `tmp/mindlakesdk-1.0.1.tar.gz`

## Comparing `mindlakesdk-1.0.0.tar` & `mindlakesdk-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/requirements.txt
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/examples/env_template.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/examples/quickstart.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/examples/use_case_1.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/examples/use_case_2.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/examples/use_case_3.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/__init__.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/cryptor.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/datalake.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/keyhelper.py
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/message.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/permission.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/settings.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/mindlakesdk/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/env_template.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_all.py
--rw-r--r--   0        0        0    12613 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_base.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_create.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_delete.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_drop.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_encryption.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_insert.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_link.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_sharing.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/tests/test_update.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/LICENSE
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mindlakesdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/env_template.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/quickstart.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/use_case_1.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/use_case_2.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/use_case_3.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/__init__.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/cryptor.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/datalake.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/keyhelper.py
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/message.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/permission.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/settings.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/env_template.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_all.py
+-rw-r--r--   0        0        0    12613 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_base.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_create.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_delete.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_drop.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_encryption.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_insert.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_link.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_sharing.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_update.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/PKG-INFO
```

### Comparing `mindlakesdk-1.0.0/examples/quickstart.py` & `mindlakesdk-1.0.1/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/examples/use_case_1.py` & `mindlakesdk-1.0.1/examples/use_case_1.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/examples/use_case_2.py` & `mindlakesdk-1.0.1/examples/use_case_2.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/examples/use_case_3.py` & `mindlakesdk-1.0.1/examples/use_case_3.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/LICENSE` & `mindlakesdk-1.0.1/mindlakesdk/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/__init__.py` & `mindlakesdk-1.0.1/mindlakesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/cryptor.py` & `mindlakesdk-1.0.1/mindlakesdk/cryptor.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/datalake.py` & `mindlakesdk-1.0.1/mindlakesdk/datalake.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/keyhelper.py` & `mindlakesdk-1.0.1/mindlakesdk/keyhelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         mk = __decryptWithWalletKey(walletAccount, mkCipher)
         skIV, skCipher = skCipher[:16], skCipher[16:]
         skBytes = mindlakesdk.utils.aesDecrypt(mk, skIV, skCipher)
         sk = RSA.import_key(skBytes)
     else:
         mk = mindlakesdk.utils.genAESKey()
         sk = mindlakesdk.utils.genRSAKey()
-        skBytes = sk.exportKey('DER')
+        skBytes = sk.exportKey('DER', pkcs=8)
         skIV = mindlakesdk.utils.get_random_bytes(16)
         skCipher = mindlakesdk.utils.aesEncrypt(mk, skIV, skBytes)
         skCipher = skIV + skCipher
         mkCipher = __encryptWithWalletKey(walletAccount, mk)
         __saveKeysToChain(web3, walletAccount, mkCipher, skCipher)
     logging.debug('mk: %s'%mk)
     logging.debug('sk: %s'%sk)
```

### Comparing `mindlakesdk-1.0.0/mindlakesdk/message.py` & `mindlakesdk-1.0.1/mindlakesdk/message.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/permission.py` & `mindlakesdk-1.0.1/mindlakesdk/permission.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/settings.py` & `mindlakesdk-1.0.1/mindlakesdk/settings.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/mindlakesdk/utils.py` & `mindlakesdk-1.0.1/mindlakesdk/utils.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_all.py` & `mindlakesdk-1.0.1/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_base.py` & `mindlakesdk-1.0.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_create.py` & `mindlakesdk-1.0.1/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_delete.py` & `mindlakesdk-1.0.1/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_drop.py` & `mindlakesdk-1.0.1/tests/test_drop.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_encryption.py` & `mindlakesdk-1.0.1/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_insert.py` & `mindlakesdk-1.0.1/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_link.py` & `mindlakesdk-1.0.1/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_sharing.py` & `mindlakesdk-1.0.1/tests/test_sharing.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/tests/test_update.py` & `mindlakesdk-1.0.1/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/LICENSE` & `mindlakesdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.0/README.md` & `mindlakesdk-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: mindlakesdk
+Version: 1.0.1
+Summary: A Python SDK to connect to Mind Lake
+Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
+Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
+Author-email: Mind Labs <biz@mindnetwork.xyz>
+License-File: LICENSE
+Keywords: datalake,encryption,web3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: eth-account
+Requires-Dist: pynacl
+Requires-Dist: web3
+Description-Content-Type: text/markdown
+
 # Mind Lake Python SDK
 
 An Python implementation for Mind Lake
 
 ## Description
 
 The Mind Lake SDK utilizes Mind Lake's encryption storage and privacy computing capabilities to provide secure data management. 
@@ -58,11 +76,13 @@
 * Dennis [@yuhaos](https://twitter.com/yuhaos)
 * George [@georgemindnet](https://twitter.com/georgemindnet)
 
 ## Version History
 
 * v1.0
     * Initial Release
+* v1.0.1
+    * Fix bug
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

### Comparing `mindlakesdk-1.0.0/pyproject.toml` & `mindlakesdk-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mindlakesdk"
-version = "v1.0.0"
+version = "v1.0.1"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to connect to Mind Lake"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mindlakesdk-1.0.0/PKG-INFO` & `mindlakesdk-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: mindlakesdk
-Version: 1.0.0
-Summary: A Python SDK to connect to Mind Lake
-Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
-Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
-Author-email: Mind Labs <biz@mindnetwork.xyz>
-License-File: LICENSE
-Keywords: datalake,encryption,web3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: eth-account
-Requires-Dist: pynacl
-Requires-Dist: web3
-Description-Content-Type: text/markdown
-
 # Mind Lake Python SDK
 
 An Python implementation for Mind Lake
 
 ## Description
 
 The Mind Lake SDK utilizes Mind Lake's encryption storage and privacy computing capabilities to provide secure data management. 
@@ -76,11 +58,13 @@
 * Dennis [@yuhaos](https://twitter.com/yuhaos)
 * George [@georgemindnet](https://twitter.com/georgemindnet)
 
 ## Version History
 
 * v1.0
     * Initial Release
+* v1.0.1
+    * Fix bug
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

