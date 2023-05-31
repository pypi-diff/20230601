# Comparing `tmp/emb_ser_protocol-1.1.20.tar.gz` & `tmp/emb_ser_protocol-1.1.21.tar.gz`

## Comparing `emb_ser_protocol-1.1.20.tar` & `emb_ser_protocol-1.1.21.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/src/emb_ser_protocol/__init__.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/src/emb_ser_protocol/protocol.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/src/emb_ser_protocol/version.py
--rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/tests/emb_ser_protocol/protocol_tests.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/LICENSE
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/README.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/pyproject.toml
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.20/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/src/emb_ser_protocol/__init__.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/src/emb_ser_protocol/protocol.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/src/emb_ser_protocol/version.py
+-rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/tests/emb_ser_protocol/protocol_tests.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/LICENSE
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/pyproject.toml
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 emb_ser_protocol-1.1.21/PKG-INFO
```

### Comparing `emb_ser_protocol-1.1.20/src/emb_ser_protocol/protocol.py` & `emb_ser_protocol-1.1.21/src/emb_ser_protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `emb_ser_protocol-1.1.20/tests/emb_ser_protocol/protocol_tests.py` & `emb_ser_protocol-1.1.21/tests/emb_ser_protocol/protocol_tests.py`

 * *Files identical despite different names*

### Comparing `emb_ser_protocol-1.1.20/.gitignore` & `emb_ser_protocol-1.1.21/.gitignore`

 * *Files identical despite different names*

### Comparing `emb_ser_protocol-1.1.20/LICENSE` & `emb_ser_protocol-1.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `emb_ser_protocol-1.1.20/README.md` & `emb_ser_protocol-1.1.21/README.md`

 * *Files identical despite different names*

### Comparing `emb_ser_protocol-1.1.20/pyproject.toml` & `emb_ser_protocol-1.1.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "emb_ser_protocol"
-version = "1.1.20"
+version = "1.1.21"
 authors = [
   { name="Warren Woolsey", email="budgettsfrog@protonmail.com" },
 ]
 description = "A simple serial protocol for communicating with embedded devices."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `emb_ser_protocol-1.1.20/PKG-INFO` & `emb_ser_protocol-1.1.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emb_ser_protocol
-Version: 1.1.20
+Version: 1.1.21
 Summary: A simple serial protocol for communicating with embedded devices.
 Project-URL: Homepage, https://github.com/pypa/emb_ser_protocol
 Project-URL: Bug Tracker, https://github.com/pypa/emb_ser_protocol/issues
 Author-email: Warren Woolsey <budgettsfrog@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

