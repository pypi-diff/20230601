# Comparing `tmp/easyport-0.1.0.tar.gz` & `tmp/easyport-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyport-0.1.0.tar", last modified: Thu Jan 12 13:50:40 2023, max compression
+gzip compressed data, was "easyport-0.1.3.tar", last modified: Thu Jun  1 13:45:41 2023, max compression
```

## Comparing `easyport-0.1.0.tar` & `easyport-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-12 13:50:40.388507 easyport-0.1.0/
--rw-rw-r--   0 life      (1000) life      (1000)     1070 2022-11-28 14:30:49.000000 easyport-0.1.0/LICENSE
--rw-rw-r--   0 life      (1000) life      (1000)      879 2023-01-12 13:50:40.388507 easyport-0.1.0/PKG-INFO
--rw-rw-r--   0 life      (1000) life      (1000)      480 2022-12-12 16:10:37.000000 easyport-0.1.0/README.md
-drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-12 13:50:40.384507 easyport-0.1.0/easyport/
--rw-rw-r--   0 life      (1000) life      (1000)        0 2022-11-28 14:15:45.000000 easyport-0.1.0/easyport/__init__.py
--rw-rw-r--   0 life      (1000) life      (1000)     8029 2023-01-12 13:50:25.000000 easyport-0.1.0/easyport/epconnector.py
-drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-12 13:50:40.384507 easyport-0.1.0/easyport.egg-info/
--rw-rw-r--   0 life      (1000) life      (1000)      879 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/PKG-INFO
--rw-rw-r--   0 life      (1000) life      (1000)      246 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/SOURCES.txt
--rw-rw-r--   0 life      (1000) life      (1000)        1 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/dependency_links.txt
--rw-rw-r--   0 life      (1000) life      (1000)       12 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/requires.txt
--rw-rw-r--   0 life      (1000) life      (1000)        9 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/top_level.txt
--rw-rw-r--   0 life      (1000) life      (1000)      103 2022-11-28 14:25:53.000000 easyport-0.1.0/pyproject.toml
--rw-rw-r--   0 life      (1000) life      (1000)      527 2023-01-12 13:50:40.388507 easyport-0.1.0/setup.cfg
+drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-06-01 13:45:41.181161 easyport-0.1.3/
+-rw-rw-r--   0 life      (1000) life      (1000)     1070 2022-11-28 14:30:49.000000 easyport-0.1.3/LICENSE
+-rw-rw-r--   0 life      (1000) life      (1000)      879 2023-06-01 13:45:41.181161 easyport-0.1.3/PKG-INFO
+-rw-rw-r--   0 life      (1000) life      (1000)      480 2022-12-12 16:10:37.000000 easyport-0.1.3/README.md
+drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-06-01 13:45:41.177161 easyport-0.1.3/easyport/
+-rw-rw-r--   0 life      (1000) life      (1000)        0 2022-11-28 14:15:45.000000 easyport-0.1.3/easyport/__init__.py
+-rw-rw-r--   0 life      (1000) life      (1000)     8041 2023-01-12 14:03:09.000000 easyport-0.1.3/easyport/epconnector.py
+drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-06-01 13:45:41.181161 easyport-0.1.3/easyport.egg-info/
+-rw-rw-r--   0 life      (1000) life      (1000)      879 2023-06-01 13:45:41.000000 easyport-0.1.3/easyport.egg-info/PKG-INFO
+-rw-rw-r--   0 life      (1000) life      (1000)      246 2023-06-01 13:45:41.000000 easyport-0.1.3/easyport.egg-info/SOURCES.txt
+-rw-rw-r--   0 life      (1000) life      (1000)        1 2023-06-01 13:45:41.000000 easyport-0.1.3/easyport.egg-info/dependency_links.txt
+-rw-rw-r--   0 life      (1000) life      (1000)       12 2023-06-01 13:45:41.000000 easyport-0.1.3/easyport.egg-info/requires.txt
+-rw-rw-r--   0 life      (1000) life      (1000)        9 2023-06-01 13:45:41.000000 easyport-0.1.3/easyport.egg-info/top_level.txt
+-rw-rw-r--   0 life      (1000) life      (1000)      103 2022-11-28 14:25:53.000000 easyport-0.1.3/pyproject.toml
+-rw-rw-r--   0 life      (1000) life      (1000)      527 2023-06-01 13:45:41.181161 easyport-0.1.3/setup.cfg
```

### Comparing `easyport-0.1.0/LICENSE` & `easyport-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easyport-0.1.0/PKG-INFO` & `easyport-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyport
-Version: 0.1.0
+Version: 0.1.3
 Summary: Connect to EasyPort Module from Festo Didactic
 Author: Ferdinand List
 Author-email: easyport@list.bayern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
```

### Comparing `easyport-0.1.0/easyport/epconnector.py` & `easyport-0.1.3/easyport/epconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,34 +127,34 @@
 
     def write(self, data, receive=True):
         super(BasicEasyport, self).write_ftdi(data)
         if receive:
             sleep(0.01)
             return self.read(reversed=False)
 
-    def send_from_memory(self, name, value=0, modify=2, intformat=True):
+    def send_from_memory(self, name, value=0, modify=2, check=True, intformat=True):
         if name not in self.memory:
             raise ValueError("No item named " + name)
         x = self.memory[name]
         self.flush()
 
         if modify != 2:
             m = modify
         else:
             m = x[3]
         if m == 1:
             m = True
         else:
             m = False
         self.flush()
-        y = self.send(m, x[0], x[1], x[2], True, value)
+        y = self.send(m, x[0], x[1], x[2], check, value)
         if not intformat:
             return y
         z = self.convert(y)
-        if x[4] is None or z < -1:
+        if x[4] is None or z < 0:
             return z
         z=(z*10)/0x7fff
         return x[4](z)
 
 
 
     def send(self, modify=True, inout=1, bbw=0, addr=0, check=True, value=0):
```

### Comparing `easyport-0.1.0/easyport.egg-info/PKG-INFO` & `easyport-0.1.3/easyport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyport
-Version: 0.1.0
+Version: 0.1.3
 Summary: Connect to EasyPort Module from Festo Didactic
 Author: Ferdinand List
 Author-email: easyport@list.bayern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
```

### Comparing `easyport-0.1.0/setup.cfg` & `easyport-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyport
-version = 0.1.0
+version = 0.1.3
 author = Ferdinand List
 author_email = easyport@list.bayern
 description = Connect to EasyPort Module from Festo Didactic
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

