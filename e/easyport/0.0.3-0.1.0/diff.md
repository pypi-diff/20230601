# Comparing `tmp/easyport-0.0.3.tar.gz` & `tmp/easyport-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyport-0.0.3.tar", last modified: Wed Jan  4 09:47:48 2023, max compression
+gzip compressed data, was "easyport-0.1.0.tar", last modified: Thu Jan 12 13:50:40 2023, max compression
```

## Comparing `easyport-0.0.3.tar` & `easyport-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-04 09:47:48.761544 easyport-0.0.3/
--rw-rw-r--   0 life      (1000) life      (1000)     1070 2022-11-28 14:30:49.000000 easyport-0.0.3/LICENSE
--rw-rw-r--   0 life      (1000) life      (1000)      876 2023-01-04 09:47:48.761544 easyport-0.0.3/PKG-INFO
--rw-rw-r--   0 life      (1000) life      (1000)      480 2022-12-12 16:10:37.000000 easyport-0.0.3/README.md
-drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-04 09:47:48.761544 easyport-0.0.3/easyport/
--rw-rw-r--   0 life      (1000) life      (1000)        0 2022-11-28 14:15:45.000000 easyport-0.0.3/easyport/__init__.py
--rw-rw-r--   0 life      (1000) life      (1000)     6350 2023-01-04 09:47:18.000000 easyport-0.0.3/easyport/epconnector.py
-drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-04 09:47:48.761544 easyport-0.0.3/easyport.egg-info/
--rw-rw-r--   0 life      (1000) life      (1000)      876 2023-01-04 09:47:48.000000 easyport-0.0.3/easyport.egg-info/PKG-INFO
--rw-rw-r--   0 life      (1000) life      (1000)      246 2023-01-04 09:47:48.000000 easyport-0.0.3/easyport.egg-info/SOURCES.txt
--rw-rw-r--   0 life      (1000) life      (1000)        1 2023-01-04 09:47:48.000000 easyport-0.0.3/easyport.egg-info/dependency_links.txt
--rw-rw-r--   0 life      (1000) life      (1000)        7 2023-01-04 09:47:48.000000 easyport-0.0.3/easyport.egg-info/requires.txt
--rw-rw-r--   0 life      (1000) life      (1000)        9 2023-01-04 09:47:48.000000 easyport-0.0.3/easyport.egg-info/top_level.txt
--rw-rw-r--   0 life      (1000) life      (1000)      103 2022-11-28 14:25:53.000000 easyport-0.0.3/pyproject.toml
--rw-rw-r--   0 life      (1000) life      (1000)      518 2023-01-04 09:47:48.761544 easyport-0.0.3/setup.cfg
+drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-12 13:50:40.388507 easyport-0.1.0/
+-rw-rw-r--   0 life      (1000) life      (1000)     1070 2022-11-28 14:30:49.000000 easyport-0.1.0/LICENSE
+-rw-rw-r--   0 life      (1000) life      (1000)      879 2023-01-12 13:50:40.388507 easyport-0.1.0/PKG-INFO
+-rw-rw-r--   0 life      (1000) life      (1000)      480 2022-12-12 16:10:37.000000 easyport-0.1.0/README.md
+drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-12 13:50:40.384507 easyport-0.1.0/easyport/
+-rw-rw-r--   0 life      (1000) life      (1000)        0 2022-11-28 14:15:45.000000 easyport-0.1.0/easyport/__init__.py
+-rw-rw-r--   0 life      (1000) life      (1000)     8029 2023-01-12 13:50:25.000000 easyport-0.1.0/easyport/epconnector.py
+drwxrwxr-x   0 life      (1000) life      (1000)        0 2023-01-12 13:50:40.384507 easyport-0.1.0/easyport.egg-info/
+-rw-rw-r--   0 life      (1000) life      (1000)      879 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/PKG-INFO
+-rw-rw-r--   0 life      (1000) life      (1000)      246 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/SOURCES.txt
+-rw-rw-r--   0 life      (1000) life      (1000)        1 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/dependency_links.txt
+-rw-rw-r--   0 life      (1000) life      (1000)       12 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/requires.txt
+-rw-rw-r--   0 life      (1000) life      (1000)        9 2023-01-12 13:50:40.000000 easyport-0.1.0/easyport.egg-info/top_level.txt
+-rw-rw-r--   0 life      (1000) life      (1000)      103 2022-11-28 14:25:53.000000 easyport-0.1.0/pyproject.toml
+-rw-rw-r--   0 life      (1000) life      (1000)      527 2023-01-12 13:50:40.388507 easyport-0.1.0/setup.cfg
```

### Comparing `easyport-0.0.3/LICENSE` & `easyport-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyport-0.0.3/PKG-INFO` & `easyport-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: easyport
-Version: 0.0.3
+Version: 0.1.0
 Summary: Connect to EasyPort Module from Festo Didactic
 Author: Ferdinand List
-Author-email: ferdi.list@tum.de
+Author-email: easyport@list.bayern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easyport-0.0.3/easyport/epconnector.py` & `easyport-0.1.0/easyport/epconnector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from time import sleep
 
 from pyftdi.ftdi import Ftdi
 
-import pickle
+import dill
 
 
 class FtdiConnector:
     # Connect to the USB-Ftdi interface
     _count = 0
 
     def __init__(self, setup=True):
@@ -41,99 +41,127 @@
             Ftdi.add_custom_product(self.vendor, self.product)
         except ValueError:
             # if product exists everything is fine
             pass
         self.device = Ftdi.create_from_url("ftdi://" + hex(self.vendor) + ":" + hex(self.product) + "/" + str(self.id))
         self.device.set_baudrate(self.baudrate)
         self.is_setup = True
-        self.write(b'setup0')
+        self.write_ftdi(b'setup0')
         sleep(0.01)
-        tmp = self.read()
-        if len(tmp) != 1:
-            raise ValueError("Unknown response of device")
-        if tmp[1] != b'setup1':
-            raise ValueError("Unknown response of device")
-            
+        tmp = self.read_ftdi()
+        if len(tmp) > 1:
+            raise ValueError("Unknown response of device: " + str(tmp))
+        if len(tmp) == 0:
+            print("Easyport already configured or error with Setup routine. Continuing...")
+            return
+        if tmp[0] != b'setup1':
+            raise ValueError("Unknown response of device: " + str(tmp))
 
-    def write(self, data):
+    def write_ftdi(self, data):
         self.check_connect(False)
         self.device.write_data(data + b'\r')
 
-    def read(self):
+    def read_ftdi(self):
         self.check_connect(False)
         x = b'1'
+        y = 0
         while x[-1] != b'\r':
-            tmp = self.device.read_data(256)
-            if len(tmp) == 0 and len(x) == 1:
-                return []
+            tmp = self.device.read_data(1024)
+            y += 1
+            if len(tmp) != 0:
+                y = 0
+            if y > 1:
+                break
             x += tmp
         return x[1:].split(b'\r')[:-1]
 
     def check_connect(self, already):
         if already and self.is_setup:
             raise AlreadyConnectedException("No changes can be made to connection parameters after connection")
         if not already and not self.is_setup:
             raise NotConnectedException("You need an active connection to send or receive. Use setup()")
 
 
 class BasicEasyport(FtdiConnector):
+    buffer = []
 
-    def __init__(self, filepath=None):
-        super().__init__()
+    def __init__(self, filepath=None, setup=True):
+        super().__init__(setup)
         self.buffer = []
         self.module = 1
         self.memory = {}
         self.set_filepath(filepath)
         if self.filepath != None:
-            self.load()
+            try:
+                self.load()
+            except FileNotFoundError:
+                print("Could not find specified save-file")
+        if(setup):
+            x = self.write(b'DV')
+            sleep(0.1)
+            print("Setup comlete! Easyport version " + x[2:].decode('ascii'))
+        self.flush()
+
 
     def set_filepath(self, filepath):
         if filepath is None:
             self.filepath = None
         if filepath[-4:] != '.pkl':
             raise ValueError("Configuration file must be .pkl")
 
         self.filepath = filepath
 
     def set_module(self, id):
         self.module = id
 
     def read(self, reversed=False):
-        self.buffer += super(BasicEasyport, self).read()
+        self.buffer.extend(super(BasicEasyport, self).read_ftdi())
         try:
             if reversed:
                 return self.buffer.pop()
             return self.buffer.pop(0)
         except IndexError:
-            return []
+            return None
 
     def flush(self):
         self.buffer = []
 
     def write(self, data, receive=True):
-        super(BasicEasyport, self).write(data)
+        super(BasicEasyport, self).write_ftdi(data)
         if receive:
             sleep(0.01)
             return self.read(reversed=False)
 
-    def send_from_memory(self, name, value=0, modify=2):
+    def send_from_memory(self, name, value=0, modify=2, intformat=True):
         if name not in self.memory:
             raise ValueError("No item named " + name)
-        x=self.memory[name]
+        x = self.memory[name]
+        self.flush()
+
         if modify != 2:
             m = modify
         else:
             m = x[3]
         if m == 1:
             m = True
         else:
             m = False
-        return self.send(m,x[0],x[1],x[2], value)
+        self.flush()
+        y = self.send(m, x[0], x[1], x[2], True, value)
+        if not intformat:
+            return y
+        z = self.convert(y)
+        if x[4] is None or z < -1:
+            return z
+        z=(z*10)/0x7fff
+        return x[4](z)
+
 
-    def send(self, modify=True, inout=1, bbw=0, addr=0, value=0):
+
+    def send(self, modify=True, inout=1, bbw=0, addr=0, check=True, value=0):
         if modify:
             send = b'M'
             if inout != 2:
                 raise ValueError("Only Outputs can be modified")
         else:
             send = b'D'
         # inout = 0: add nothing
@@ -172,41 +200,62 @@
         if modify:
             send += b'='
             tmp = hex(value)[2:]
             if len(tmp) > 4 or value < 0:
                 raise ValueError("value to modify fust be positive and not greater than 0xFFFF")
             send += tmp.upper().encode('ascii')
 
-        tmp = self.write(send)
-        if (not modify and tmp[:tmp.find(b'=')] != send[1:tmp.find(b'=') + 1]) or (modify and tmp != send[1:]):
-            print("Unexpected output of Easyport: " + str(tmp) + "\n Send it: " + str(send))
+        tmp = self.write(send , check)
+        if check:
+            return self.check_output(send,tmp,modify,bbw)
         return tmp
 
+
+    def check_output(self,input,out, modify,bbw):
+        if out is None or (not modify and out[:out.find(b'=')] != input[1:out.find(b'=') + 1]) or (
+                modify and ((bbw > 0 and out != input[1:]) or (bbw == 0 and out[:-1] != input[1:]))):
+            print("Unexpected output of Easyport: " + str(out) + "\n Send it: " + str(input))
+        elif not out is None and modify and bbw == 0:
+            a = out.find(b'=')
+            if len(out) > 1 and len(out) - a == 3 and out[-1] == out[-2]:
+                out = out[:-1]
+        return out
     def save(self):
         if self.filepath is None:
             raise FileNotFoundError("Please specify a filepath on init or with set_filepath()")
-        with open(self.filepath,'wb') as f:
-            pickle.dump(self.memory, f)
+        with open(self.filepath, 'wb') as f:
+            dill.dump(self.memory, f)
 
     def load(self):
         if self.filepath is None:
             raise FileNotFoundError("Please specify a filepath on init or with set_filepath()")
         with open(self.filepath, 'rb') as f:
-            self.memory = pickle.load(f)
+            self.memory = dill.load(f)
 
-    def set(self, name, inout=1, bbw=0, addr=0, modify=2):
-        self.memory[name] = (inout, bbw, addr, modify)
+    def set(self, name, inout=1, bbw=0, addr=0, modify=2, calc=None):
+        self.memory[name] = (inout, bbw, addr, modify, calc)
 
     def delete(self, name):
         if name not in self.memory:
-            raise ValueError("No item named "+ name)
+            raise ValueError("No item named " + name)
         del self.memory[name]
 
-    def version(self):
-        return self.write("DV")
+    def list(self):
+        for x, y in self.memory.items():
+            print(x + ":\tInput/Output(1/2):" + str(y[0]) + "\tBit(0),Byte(1),Word(2):" + str(y[1]) + "\tAddress:"
+                  + hex(y[2]) + "\tdefaultModify:" + str(y[3]))
+
+    def convert(self, x):
+        try:
+            z = x.index(b'=')
+            if z + 1 < len(x):
+                return int(x[z + 1:], base=16)
+        except ValueError:
+            return -1
+        return -1
 
 
 class AlreadyConnectedException(Exception):
     # After connection no change can be made to connection parameters
     pass
```

### Comparing `easyport-0.0.3/easyport.egg-info/PKG-INFO` & `easyport-0.1.0/easyport.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: easyport
-Version: 0.0.3
+Version: 0.1.0
 Summary: Connect to EasyPort Module from Festo Didactic
 Author: Ferdinand List
-Author-email: ferdi.list@tum.de
+Author-email: easyport@list.bayern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easyport-0.0.3/setup.cfg` & `easyport-0.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [metadata]
 name = easyport
-version = 0.0.3
+version = 0.1.0
 author = Ferdinand List
-author_email = ferdi.list@tum.de
+author_email = easyport@list.bayern
 description = Connect to EasyPort Module from Festo Didactic
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 
 [options]
 install_requires = 
 	pyftdi
+	dill
 packages = find:
 python_requires = >=3.7
 include_package_data = False
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

