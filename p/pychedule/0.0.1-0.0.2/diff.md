# Comparing `tmp/pychedule-0.0.1-py3-none-any.whl.zip` & `tmp/pychedule-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,11 @@
-Zip file size: 1584 bytes, number of entries: 6
+Zip file size: 2626 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       47 b- defN 23-Jun-01 14:12 packageTest/__init__.py
--rw-r--r--  2.0 unx       53 b- defN 23-Jun-01 14:12 packageTest/packageTest.py
--rw-r--r--  2.0 unx      590 b- defN 23-Jun-01 14:13 pychedule-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 14:13 pychedule-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-01 14:13 pychedule-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      464 b- defN 23-Jun-01 14:13 pychedule-0.0.1.dist-info/RECORD
-6 files, 1258 bytes uncompressed, 736 bytes compressed:  41.5%
+-rw-r--r--  2.0 unx      459 b- defN 23-Jun-01 16:31 packageTest/packageTest.py
+-rwxr-xr-x  2.0 unx      459 b- defN 23-Jun-01 16:30 pychedule-0.0.2.data/scripts/test.py
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-01 16:33 test/__init__.py
+-rw-r--r--  2.0 unx      459 b- defN 23-Jun-01 16:30 test/test.py
+-rw-r--r--  2.0 unx      590 b- defN 23-Jun-01 16:34 pychedule-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 16:34 pychedule-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-01 16:34 pychedule-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      695 b- defN 23-Jun-01 16:34 pychedule-0.0.2.dist-info/RECORD
+9 files, 2846 bytes uncompressed, 1422 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -1,19 +1,28 @@
 Filename: packageTest/__init__.py
 Comment: 
 
 Filename: packageTest/packageTest.py
 Comment: 
 
-Filename: pychedule-0.0.1.dist-info/METADATA
+Filename: pychedule-0.0.2.data/scripts/test.py
 Comment: 
 
-Filename: pychedule-0.0.1.dist-info/WHEEL
+Filename: test/__init__.py
 Comment: 
 
-Filename: pychedule-0.0.1.dist-info/top_level.txt
+Filename: test/test.py
 Comment: 
 
-Filename: pychedule-0.0.1.dist-info/RECORD
+Filename: pychedule-0.0.2.dist-info/METADATA
+Comment: 
+
+Filename: pychedule-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: pychedule-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: pychedule-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## packageTest/packageTest.py

```diff
@@ -1,2 +1,17 @@
-def test_package():
-    print("This is package test")
+import os
+import subprocess
+import argparse
+
+def load_python_files(directory):
+    file_paths = []
+    for root, dirs, files in os.walk(directory):
+        for file in files:
+            if file.endswith(".py"):
+                file_path = os.path.join(root, file)
+                file_paths.append(file_path)
+    return file_paths
+
+def execute_python_files(file_paths):
+    for file_path in file_paths:
+        subprocess.run(["python", file_path])
+
```

## Comparing `pychedule-0.0.1.dist-info/METADATA` & `pychedule-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychedule
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scheduler for Python
 Home-page: https://github.com/wklee610/pychedule
 Author: wklee610
 Author-email: wklee610@gmail.com
 License: UNKNOWN
 Keywords: scheduler,wklee610,python
 Platform: UNKNOWN
```

