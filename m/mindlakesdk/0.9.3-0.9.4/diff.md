# Comparing `tmp/mindlakesdk-0.9.3.tar.gz` & `tmp/mindlakesdk-0.9.4.tar.gz`

## Comparing `mindlakesdk-0.9.3.tar` & `mindlakesdk-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,33 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/requirements.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/__init__.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/cryptor.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/datalake.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/keyhelper.py
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/message.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/permission.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/settings.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/mindlakesdk/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/LICENSE
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mindlakesdk-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/requirements.txt
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/examples/env_template.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/examples/quickstart.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/examples/use_case_1.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/examples/use_case_2.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/examples/use_case_3.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/__init__.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/cryptor.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/datalake.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/keyhelper.py
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/message.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/permission.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/settings.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/mindlakesdk/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/env_template.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_all.py
+-rw-r--r--   0        0        0    12613 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_base.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_create.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_delete.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_drop.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_encryption.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_insert.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_link.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_sharing.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/tests/test_update.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mindlakesdk-0.9.4/PKG-INFO
```

### Comparing `mindlakesdk-0.9.3/mindlakesdk/LICENSE` & `mindlakesdk-0.9.4/mindlakesdk/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/__init__.py` & `mindlakesdk-0.9.4/mindlakesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/cryptor.py` & `mindlakesdk-0.9.4/mindlakesdk/cryptor.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/datalake.py` & `mindlakesdk-0.9.4/mindlakesdk/datalake.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/keyhelper.py` & `mindlakesdk-0.9.4/mindlakesdk/keyhelper.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/message.py` & `mindlakesdk-0.9.4/mindlakesdk/message.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/permission.py` & `mindlakesdk-0.9.4/mindlakesdk/permission.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/settings.py` & `mindlakesdk-0.9.4/mindlakesdk/settings.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/mindlakesdk/utils.py` & `mindlakesdk-0.9.4/mindlakesdk/utils.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/LICENSE` & `mindlakesdk-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/README.md` & `mindlakesdk-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `mindlakesdk-0.9.3/pyproject.toml` & `mindlakesdk-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mindlakesdk"
-version = "v0.9.3"
+version = "v0.9.4"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to connect to Mind Lake"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mindlakesdk-0.9.3/PKG-INFO` & `mindlakesdk-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindlakesdk
-Version: 0.9.3
+Version: 0.9.4
 Summary: A Python SDK to connect to Mind Lake
 Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
 Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
```

