# Comparing `tmp/murloc-0.0.4.tar.gz` & `tmp/murloc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murloc-0.0.4.tar", last modified: Sat May 27 21:58:27 2023, max compression
+gzip compressed data, was "murloc-0.0.5.tar", last modified: Thu Jun  1 02:41:24 2023, max compression
```

## Comparing `murloc-0.0.4.tar` & `murloc-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 21:58:27.618814 murloc-0.0.4/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.4/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 21:58:27.618814 murloc-0.0.4/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     2818 2023-05-27 20:48:16.000000 murloc-0.0.4/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 21:58:27.618814 murloc-0.0.4/murloc/
--rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.4/murloc/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4505 2023-05-27 21:57:01.000000 murloc-0.0.4/murloc/murloc.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 21:58:27.618814 murloc-0.0.4/murloc.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-27 21:58:27.618814 murloc-0.0.4/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-05-27 21:57:50.000000 murloc-0.0.4/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 02:41:24.564990 murloc-0.0.5/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.5/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4086 2023-06-01 02:41:24.564990 murloc-0.0.5/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3722 2023-06-01 02:38:30.000000 murloc-0.0.5/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 02:41:24.563990 murloc-0.0.5/murloc/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.5/murloc/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5058 2023-06-01 02:19:05.000000 murloc-0.0.5/murloc/murloc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 02:41:24.564990 murloc-0.0.5/murloc.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4086 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-06-01 02:41:24.564990 murloc-0.0.5/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-06-01 01:31:57.000000 murloc-0.0.5/setup.py
```

### Comparing `murloc-0.0.4/LICENSE` & `murloc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `murloc-0.0.4/PKG-INFO` & `murloc-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: murloc
-Version: 0.0.4
-Summary: extensible api server
-Home-page: 
-Author: Chris Varga
-Author-email: 
-Keywords: extensible api server
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Murloc
 Extensible api server
 
 ## Example usage
 ```python
 import murloc
 
@@ -26,20 +12,20 @@
     print("hello, world!")
     return f"params={params}"
 
 def command_set(self, params):
     return '{"err":0,"data":"configuration successful"}'
 
 
-# Then add the methods to murloc using a `dict` like so.
-myroutes = {
+# Then add the methods to murloc by setting the methods `dict`.
+dispatch = {
     "hello": hello,
     "set": command_set,
 }
-m = murloc.init(methods=myroutes)
+m = murloc.init(methods=dispatch)
 
 # And start the server.
 m.listen()
 ```
 
 ## Syntax
 Murloc uses the following api conventions.
@@ -66,14 +52,16 @@
 ```javascript
 {
     "err": 1,
     "data": // any valid json
 }
 ```
 
+Of course, you can have your own methods return anything you like.
+
 ## Examples
 ```bash
 hero@azeroth:~$ cat hero.py
 import murloc
 
 def new_character(self, params):
     self.log(f"setting class to {params['class']}")
@@ -97,37 +85,79 @@
 \:\  \ /:/  /    Port: 8048
  \:\  /:/  /     PID:  3139
   \:\/:/  /
    \::/  /             Aaaaaughibbrgubugbugrguburgle!
     \/__/
 
 [2023-05-27 20:35:19] [3139] Listening at 127.0.0.1:8048
-[2023-05-27 20:35:33] [3142] Connection from ('127.0.0.1', 43668)
-[2023-05-27 20:35:47] [3146] Connection from ('127.0.0.1', 45626)
 [2023-05-27 20:35:47] [3146] setting class to warrior
 [2023-05-27 20:35:47] [3146] equiping weapons: ['worn shortsword', 'worn buckler']
 ```
 
 ```bash
 hero@azeroth:~$ echo '{"method":"new","params":{"class":"warrior","weapons":["worn shortsword","worn buckler"]}}' | nc -q 0 localhost 8048
-{"err":0,"data":null}
+{"err": 0, "data": null}
 hero@azeroth:~$ echo '{"method":"dwarf","params":{"variable":"class","value":"warrior"}}' | nc -q 0 localhost 8048
-{"err":1,"data":"method not defined"}
+{"err": 1, "data": "method not defined"}
 hero@azeroth:~$ echo '{"params":{"variable":"class","value":"warrior"}}' | nc -q 0 localhost 8048
-{"err":1,"data":"request lacks method"}
+{"err": 1, "data": "request lacks method"}
 hero@azeroth:~$ echo '{"method":"dwarf"}' | nc -q 0 localhost 8048
-{"err":1,"data":"request lacks params"}
+# params are optional, but note that new_character() above will raise an exception since params will be None
+# e.g., TypeError: 'NoneType' object is not subscriptable
 hero@azeroth:~$
 ```
 
 ## Customizing murloc
 The following default parameters can be changed by setting them in the murloc `init()` function.
 ```python
+def init(
     version="1.0.0",
     host="127.0.0.1",
     port=8048,
     name="murloc",
     mode="default",
     url="Aaaaaughibbrgubugbugrguburgle!",
     methods=dict(),
     logfile=None,
+    verbose=False,
+):
+```
+
+Here's an example.
+```python
+import murloc
+
+m = murloc.init(
+    version="2.1.0",
+    port=8080,
+    name="gandalf",
+    mode="grey",
+    url="https://example.com/gandalf",
+    verbose=True,
+)
+m.methods["fly"] = lambda self, params : "Fly, you fools!"
+m.listen()
+```
+
+```bash
+frodo@hobbiton:~$ python3 gandalf.py
+[2023-06-01 02:35:23] [murloc.py:148] [4129]
+     ___
+    /\  \
+   /::\  \       gandalf 2.1.0
+  /:/\:\  \
+ /:/  \:\  \
+/:/__/ \:\__\    Running in grey mode
+\:\  \ /:/  /    Port: 8080
+ \:\  /:/  /     PID:  4129
+  \:\/:/  /
+   \::/  /             https://example.com/gandalf
+    \/__/
+
+[2023-06-01 02:35:23] [murloc.py:155] [4129] Listening at 127.0.0.1:8080
+```
+
+```bash
+frodo@hobbiton:~$ echo '{"method":"fly"}' | nc -q 0 localhost 8080
+Fly, you fools!
+frodo@hobbiton:~$
 ```
```

### Comparing `murloc-0.0.4/murloc/murloc.py` & `murloc-0.0.5/murloc/murloc.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,25 @@
         host=socket.inet_ntoa(struct.pack("!L", socket.INADDR_LOOPBACK)),
         port=8048,
         name="murloc",
         mode="default",
         url="Aaaaaughibbrgubugbugrguburgle!",
         methods=dict(),
         logfile=None,
+        verbose=False,
     ):
         self.version = version
         self.host = host
         self.port = port
         self.name = name
         self.mode = mode
         self.url = url
         self.methods = methods
         self.logfile = logfile
+        self.verbose = verbose
         self.pid = os.getpid()
         self.boot = inspect.cleandoc(
             f"""\n
                     
                  ___
                 /\  \ 
                /::\  \       {self.name} {self.version}
@@ -50,48 +52,67 @@
                \::/  /             {self.url}
                 \/__/ 
                     """
         )
 
     def log(self, s):
         date = time.strftime("%Y-%m-%d %H:%M:%S")
-        if self.mode == "debug":
+        if self.verbose:
             n = inspect.currentframe().f_back.f_lineno
-            msg = f"[{date}] [{__file__}:{n}] [{os.getpid()}] {s}"
+            msg = f"[{date}] [{os.path.basename(__file__)}:{n}] [{os.getpid()}] {s}"
         else:
             msg = f"[{date}] [{os.getpid()}] {s}"
         if not self.logfile:
             print(msg)
         else:
             try:
                 with open(self.logfile, "a") as f:
                     f.write(f"{msg}\n")
             except:
                 print(msg)
 
+    def debug(self, s):
+        if not self.verbose:
+            return
+        date = time.strftime("%Y-%m-%d %H:%M:%S")
+        n = inspect.currentframe().f_back.f_lineno
+        msg = f"[{date}] [{os.path.basename(__file__)}:{n}] [{os.getpid()}] {s}"
+        if not self.logfile:
+            print(msg)
+        else:
+            try:
+                with open(self.logfile, "a") as f:
+                    f.write(f"{msg}\n")
+            except:
+                print(msg)
+
     def handle(self, method, params):
+        err = {"err": 1, "data": "method not defined"}
         if method not in self.methods:
-            return '{"err":1,"data":"method not defined"}'
+            self.debug(f"method {method} not defined")
+            return json.dumps(err)
         return self.methods[method](self, params)
 
     def parse(self, req):
+        err = {"err": 1, "data": None}
         try:
             js = json.loads(req)
         except Exception as e:
-            if self.mode == "debug":
-                self.log(f"json.loads: {req}: {e}")
-            return '{"err":1,"data":"invalid json request"}'
+            self.debug(f"json.loads: {req}: {e}")
+            err["data"] = "invalid json request"
+            return json.dumps(err)
         try:
             method = js["method"]
         except:
-            return '{"err":1,"data":"request lacks method"}'
+            err["data"] = "request lacks method"
+            return json.dumps(err)
         try:
             params = js["params"]
         except:
-            return '{"err":1,"data":"request lacks params"}'
+            params = None
         return self.handle(method, params)
 
     def recvall(self, conn):
         data = b""
         while True:
             packet = conn.recv(1024)
             data += packet
@@ -100,16 +121,15 @@
         return data
 
     def handle_connection(self, conn, addr):
         while True:
             try:
                 data = self.recvall(conn)
             except Exception as e:
-                if self.mode == "debug":
-                    self.log(f"recv: {e}")
+                self.debug(f"recv: {e}")
                 conn.shutdown(socket.SHUT_RDWR)
                 conn.close()
                 break
             if not data:
                 conn.shutdown(socket.SHUT_RDWR)
                 conn.close()
                 break
@@ -133,20 +153,19 @@
         sock.bind((self.host, self.port))
         sock.listen()
         self.log(f"Listening at {self.host}:{self.port}")
         while True:
             try:
                 conn, addr = sock.accept()
             except Exception as e:
-                if self.mode == "debug":
-                    self.log(f"accept: {e}")
+                self.debug(f"accept: {e}")
                 break
             conn.settimeout(10)
             # Fork to handle the new connection; this allows us to use
             # os.system() etc, which is problematic within a thread.
             pid = os.fork()
             if pid == 0:
-                self.log(f"Connection from {addr}")
+                self.debug(f"Connection from {addr}")
                 self.handle_connection(conn, addr)
                 sys.exit(0)
             else:
                 continue
```

### Comparing `murloc-0.0.4/setup.py` & `murloc-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="murloc",
-    version="0.0.4",
+    version="0.0.5",
     author="Chris Varga",
     author_email="",
     description="extensible api server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
```

