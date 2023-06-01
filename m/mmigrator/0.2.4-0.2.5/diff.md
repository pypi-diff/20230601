# Comparing `tmp/mmigrator-0.2.4.tar.gz` & `tmp/mmigrator-0.2.5.tar.gz`

## Comparing `mmigrator-0.2.4.tar` & `mmigrator-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.2.4/package.sh
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.2.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/cli.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/constants.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/db.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/migration.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/migration_manager.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/config_manager/__init__.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/config_manager/config_manager.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/config_manager/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.4/src/mmigrator/types/__init__.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.2.4/tests/helpers.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.2.4/tests/test_migration_manager.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.2.4/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mmigrator-0.2.4/LICENSE
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 mmigrator-0.2.4/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 mmigrator-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.2.5/package.sh
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.2.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/cli.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/constants.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/db.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/migration.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/migration_manager.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/config_manager/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/config_manager/config_manager.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/config_manager/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.5/src/mmigrator/types/__init__.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.2.5/tests/helpers.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.2.5/tests/test_migration_manager.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mmigrator-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 mmigrator-0.2.5/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 mmigrator-0.2.5/PKG-INFO
```

### Comparing `mmigrator-0.2.4/src/mmigrator/cli.py` & `mmigrator-0.2.5/src/mmigrator/cli.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/src/mmigrator/constants.py` & `mmigrator-0.2.5/src/mmigrator/constants.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/src/mmigrator/db.py` & `mmigrator-0.2.5/src/mmigrator/db.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/src/mmigrator/migration.py` & `mmigrator-0.2.5/src/mmigrator/migration.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/src/mmigrator/migration_manager.py` & `mmigrator-0.2.5/src/mmigrator/migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/src/mmigrator/config_manager/config_manager.py` & `mmigrator-0.2.5/src/mmigrator/config_manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/src/mmigrator/config_manager/helpers.py` & `mmigrator-0.2.5/src/mmigrator/config_manager/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 def try_load_from_dotenv(varname, data):
     m = re.search(fr'{varname}\s?=\s?(.*)', data)
 
     return m[1] if m else None
 
 
 def load_var(filename, varname):
-    var_value = None
-
-    with open(filename, 'r') as f:
-        data = f.read()
-
-    if re.match(r'^.*\.json$', filename):
-        var_value = try_load_from_json(varname, data)
-    else:
-        var_value = try_load_from_dotenv(varname, data)
-
-    if not var_value:
+    try:
+        var_value = None
+    
+        with open(filename, 'r') as f:
+            data = f.read()
+    
+        if re.match(r'^.*\.json$', filename):
+            var_value = try_load_from_json(varname, data)
+        else:
+            var_value = try_load_from_dotenv(varname, data)
+        
+        return var_value
+    except Exception:
         raise Exception(f'Cannot parse {varname} variable from file {filename}')
-
-    return var_value
```

### Comparing `mmigrator-0.2.4/tests/helpers.py` & `mmigrator-0.2.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/tests/test_migration_manager.py` & `mmigrator-0.2.5/tests/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/LICENSE` & `mmigrator-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/README.md` & `mmigrator-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mmigrator-0.2.4/pyproject.toml` & `mmigrator-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mmigrator"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Serhii Kovalov", email="moiserge.k@gmail.com" },
 ]
 description = "Migration engine for MongoDB"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `mmigrator-0.2.4/PKG-INFO` & `mmigrator-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmigrator
-Version: 0.2.4
+Version: 0.2.5
 Summary: Migration engine for MongoDB
 Project-URL: Homepage, https://github.com/sergekovalev/mmigrator
 Project-URL: Bug Tracker, https://github.com/sergekovalev/mmigrator/issues
 Author-email: Serhii Kovalov <moiserge.k@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

