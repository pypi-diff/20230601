# Comparing `tmp/gmcapsule-0.3.2.tar.gz` & `tmp/gmcapsule-0.4.0.tar.gz`

## Comparing `gmcapsule-0.3.2.tar` & `gmcapsule-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/example.ini
--rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/__init__.py
--rw-r--r--   0        0        0    24276 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/gemini.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/markdown.py
--rwxr-xr-x   0        0        0    18589 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/modules/80_gitview.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/modules/90_cgi.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/gmcapsule/modules/99_static.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/.gitignore
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 gmcapsule-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/example.ini
+-rw-r--r--   0        0        0    25496 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/gmcapsule/__init__.py
+-rw-r--r--   0        0        0    24608 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/gmcapsule/gemini.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/gmcapsule/markdown.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/gmcapsule/modules/10_rewrite.py
+-rwxr-xr-x   0        0        0    18589 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/gmcapsule/modules/80_gitview.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/gmcapsule/modules/90_cgi.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/gmcapsule/modules/99_static.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 gmcapsule-0.4.0/PKG-INFO
```

### Comparing `gmcapsule-0.3.2/example.ini` & `gmcapsule-0.4.0/example.ini`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.2/gmcapsule/__init__.py` & `gmcapsule-0.4.0/gmcapsule/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,17 @@
 *************
 
 The GmCapsule configuration file is in `INI format
 <https://en.wikipedia.org/wiki/INI_file>`_. The following sections are
 defined:
 
 - :ref:`server` — server settings
-- :ref:`static` — serving static files
 - :ref:`titan` — Titan upload settings
+- :ref:`static` — serving static files
+- :ref:`rewrite.*` — URL rewriting rules
 - :ref:`cgi` — General CGI settings
 - :ref:`cgi.*` — CGI programs
 - :ref:`gitview` — Git repository viewer settings
 - :ref:`gitview.*` — Git repository settings
 
 Example of a minimal configuration file for serving static files from
 `/var/gemini/example.com/`:
@@ -128,14 +129,58 @@
 
         [static]
         root = /home/user/gemini
 
     files will be served from `/home/user/gemini/example.com/`.
 
 
+rewrite.*
+---------
+
+Settings for the `rewrite` module that checks regular expressions against
+the request path and can rewrite the path or return a custom status. You can
+use this for internal remapping of directories and files, redirections,
+"Gone" statuses, or other exceptional situations.
+
+Each rewriting rule is a section that begins with ``rewrite.``.
+
+.. code-block:: ini
+
+    [rewrite.rename]
+    path    = ^/old-path/
+    repl    = /new-location/
+
+    [rewrite.elsewhere]
+    path    = .*\\.gmi$
+    status  = 31 gemini://mygemlog.space/\\1.gmi
+
+protocol : string
+    Protocol for the rewrite rule. If omitted, the rule applies to both
+    ``gemini`` and ``titan``.
+
+host : string
+    Hostname for the rewrite rule. If omitted, defaults to the first
+    hostname defined in the :ref:`server` section.
+
+path : string
+    Regular expression that is matched against the request path. You may use
+    capture groups and refer to them in the replacement text. Note that the
+    request path always begins with a slash.
+
+repl : string
+    Replacement path. The part of the request path that matches the "path"
+    pattern is replaced with this. You can use backslashes to refer to
+    capture groups (``\\1``).
+
+status : string
+    Custom status to respond with. Must begin with the status code followed
+    by the meta line. You can use backslashes to refer to capture groups
+    (``\\1``).
+
+
 cgi
 ---
 
 General settings for CGI programs.
 
 bin_root : path
     CGI root directory. If set, all executables under the root are made
@@ -436,15 +481,15 @@
 import subprocess
 from pathlib import Path
 
 from .gemini import Server, Cache
 from .markdown import to_gemtext as markdown_to_gemtext
 
 
-__version__ = '0.3.2'
+__version__ = '0.4.0'
 __all__ = [
     'Config', 'Capsule', 'Cache',
     'get_mime_type', 'markdown_to_gemtext'
 ]
 
 
 class Config:
@@ -625,42 +670,72 @@
 
         Args:
             cache (Cache): Cache instance.
         """
         self.sv.add_cache(cache)
 
     def load_modules(self):
-        name_pattern = re.compile(r'[0-9][0-9]_(.*)\.py')
+        # The configuration can override default priorities.
+        mod_priority = {}
+        if 'priority' in self.cfg.ini:
+            for name, priority in self.cfg.section('priority').items():
+                mod_priority[name] = int(priority)
+
+        # We will load all recognized modules.
+        name_pattern = re.compile(r'([0-9][0-9])_(.*)\.py')
         dirs = []
         for user_dir in self.cfg.mod_dirs():
             if user_dir not in dirs:
                 dirs.append(user_dir)
         dirs += [Path(__file__).parent.resolve() / 'modules']
+        mods = []
         for mdir in dirs:
             for mod_file in sorted(os.listdir(mdir)):
                 m = name_pattern.match(mod_file)
                 if m:
                     path = (mdir / mod_file).resolve()
-                    name = m.group(1)
+                    name = m.group(2)
                     loader = importlib.machinery.SourceFileLoader(name, str(path))
                     spec = importlib.util.spec_from_loader(name, loader)
                     mod = importlib.util.module_from_spec(spec)
                     loader.exec_module(mod)
-                    print('MODULE:', mod.__doc__)
-                    mod.init(self)
+                    if name in mod_priority:
+                        priority = mod_priority[name]
+                    else:
+                        priority = int(m.group(1))
+                    mods.append((priority, name, mod))
+
+        # Initialize in priority order.
+        for _, _, mod in sorted(mods):
+            print(f'Init:', mod.__doc__)
+            mod.init(self)
 
     def shutdown_event(self):
         """
         Returns:
             threading.Event: Event that is set when the server is
             shutting down. Background workers must wait on this and stop
             when the event is set.
         """
         return self.sv.shutdown_event
 
+    def call_entrypoint(self, request):
+        """
+        Calls the registered entry point for a request.
+
+        Args:
+            request (Request): Request object.
+
+        Returns:
+            Tuple with (response, cache). The response can be binary data, text,
+            tuple with status and meta string, or tuple with status, meta, and body.
+            The cache is None if the data was not read from a cache.
+        """
+        return self.sv.call_entrypoint(request)
+
     def run(self):
         """
         Start worker threads and begin accepting incoming connections. The
         server will run until stopped with a KeyboardInterrupt (^C).
         """
         self.sv.run(memtrace=self.cfg.debug_memtrace)
```

### Comparing `gmcapsule-0.3.2/gmcapsule/gemini.py` & `gmcapsule-0.4.0/gmcapsule/gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 import time
 from urllib.parse import urlparse
 
 import OpenSSL.crypto
 from OpenSSL import SSL, crypto
 
 
+class GeminiError(Exception):
+    def __init__(self, status, msg):
+        Exception.__init__(self, msg)
+        self.status = status
+
+
 class AbortedIOError(Exception):
     def __init__(self, msg):
         Exception.__init__(self, msg)
 
 
 def wait_for_read(stream, timeout):
     fno = stream._socket.fileno()
@@ -267,14 +273,17 @@
         self.hostname = hostname
         self.path = path
         self.query = query
         self.content_token = content_token
         self.content_mime = content_mime
         self.content = content
 
+    def url(self):
+        return f'{self.scheme}://{self.hostname}{self.path}{"?" + self.query if self.query else ""}'
+
 
 def verify_callback(connection, cert, err_num, err_depth, ret_code):
     #print("verify_callback:", connection, cert, ret_code)
     return True
 
 
 class Cache:
@@ -441,80 +450,50 @@
                 report_error(stream, 59, "Gemini disallows request content")
                 return
 
         self.log(request)
 
         url = urlparse(request)
         path = url.path
-        if url.port != None and url.port != self.server.port:
-            report_error(stream, 59, "Invalid port number")
-            return
         if path == '':
             path = '/'
         hostname = url.hostname
-        entrypoint = self.server.find_entrypoint(url.scheme, hostname, path)
 
-        # Server name indication is required.
+        if url.port != None and url.port != self.server.port:
+            report_error(stream, 59, "Invalid port number")
+            return
         if not stream.get_servername():
+            # Server name indication is required.
             report_error(stream, 59, "Missing TLS server name indication")
             return
-        if stream.get_servername().decode() != url.hostname:
+        if stream.get_servername().decode() != hostname:
             report_error(stream, 53, "Proxy request refused")
             return
 
-        caches = [] if (url.scheme != 'gemini' or identity or len(url.query) > 0) \
-            else self.server.caches
-        from_cache = None
-
-        # print(f'Request : {request}')
-        # print(f'Cert    : {cl_cert}')
-
-        if entrypoint:
-            # Check the caches first.
-            for cache in caches:
-                media, content = cache.try_load(hostname + path)
-                if not media is None:
-                    response = 20, media, content
-                    from_cache = cache
-                    if hasattr(content, '__len__'):
-                        print('%d bytes from cache, %s' % (len(content), media))
-                    else:
-                        print('stream from cache,', media)
-                    break
-
-            # Process the request normally if there is nothing cached.
-            if not from_cache:
-                try:
-                    response = entrypoint(Request(
-                        identity,
-                        remote_address=from_addr,
-                        scheme=url.scheme,
-                        hostname=hostname,
-                        path=path,
-                        query=url.query if '?' in request else None,
-                        content_token=req_token,
-                        content_mime=req_mime,
-                        content=data if len(data) else None
-                    ))
-                except Exception as x:
-                    import traceback
-                    traceback.print_exception(x)
-                    report_error(stream, 40, 'Temporary failure')
-                    return
+        try:
+            request = Request(
+                identity,
+                remote_address=from_addr,
+                scheme=url.scheme,
+                hostname=hostname,
+                path=path,
+                query=url.query if '?' in request else None,
+                content_token=req_token,
+                content_mime=req_mime,
+                content=data if len(data) else None
+            )
+            response, from_cache = self.server.call_entrypoint(request)
 
             # Determine status code, meta line, and body content.
             if type(response) == tuple:
                 if len(response) == 2:
-                    status = response[0]
-                    meta = response[1]
+                    status, meta = response
                     response = ''
                 else:
-                    status = response[0]
-                    meta = response[1]
-                    response = response[2]
+                    status, meta, response = response
             else:
                 status = 20
                 meta = 'text/gemini; charset=utf-8'
 
             if response == None:
                 response_data = b''
             elif type(response) == str:
@@ -524,24 +503,25 @@
 
             safe_sendall(stream, f'{status} {meta}\r\n'.encode('utf-8'))
             safe_sendall(stream, response_data)
 
             # Save to cache.
             if not from_cache and status == 20 and \
                     (type(response_data) == bytes or type(response_data) == bytearray):
-                for cache in caches:
+                for cache in self.server.caches:
                     if cache.save(hostname + path, meta, response_data):
                         break
 
             # Close handles.
             if hasattr(response_data, 'close'):
                 response_data.close()
 
-        else:
-            report_error(stream, 50, 'Permanent failure')
+        except GeminiError as error:
+            report_error(stream, error.status, str(error))
+            return
 
 
 class Server:
     def __init__(self, hostname_or_hostnames, cert_path, key_path,
                  address='localhost', port=1965,
                  cache=None, session_id=None, max_upload_size=0, num_threads=1,
                  require_upload_identity=True):
@@ -689,11 +669,43 @@
                     if len(path_pattern) == 0 or fnmatch.fnmatch(path, path_pattern):
                         return handler
                 else:
                     # A callable generic path matcher.
                     handler = path_pattern(path)
                     if handler:
                         return handler
-        except:
+        except Exception as x:
+            print(x)
             return None
 
         return None
+
+    def call_entrypoint(self, request):
+        entrypoint = self.find_entrypoint(request.scheme, request.hostname, request.path)
+
+        caches = self.caches if (request.scheme == 'gemini' and
+                                 not request.identity and
+                                 not request.query) else []
+        from_cache = None
+
+        if entrypoint:
+            # Check the caches first.
+            for cache in caches:
+                media, content = cache.try_load(request.hostname + request.path)
+                if not media is None:
+                    response = 20, media, content
+                    if hasattr(content, '__len__'):
+                        print('%d bytes from cache, %s' % (len(content), media))
+                    else:
+                        print('stream from cache,', media)
+                    return response, cache
+
+            # Process the request normally if there is nothing cached.
+            if not from_cache:
+                try:
+                    return entrypoint(request), None
+                except Exception as x:
+                    import traceback
+                    traceback.print_exception(x)
+                    raise GeminiError(40, 'Temporary failure')
+
+        raise GeminiError(50, 'Permanent failure')
```

### Comparing `gmcapsule-0.3.2/gmcapsule/markdown.py` & `gmcapsule-0.4.0/gmcapsule/markdown.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.2/gmcapsule/modules/80_gitview.py` & `gmcapsule-0.4.0/gmcapsule/modules/80_gitview.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.2/gmcapsule/modules/90_cgi.py` & `gmcapsule-0.4.0/gmcapsule/modules/90_cgi.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.2/gmcapsule/modules/99_static.py` & `gmcapsule-0.4.0/gmcapsule/modules/99_static.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.2/README.md` & `gmcapsule-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -33,23 +33,29 @@
     WantedBy=default.target
 
 Replace `<YOUR-INSTALL-PATH>` with the actual path of `gmcapsuled`. `pip` will install it in a directory on your PATH.
 
 Then you can do the usual:
 
     systemctl --user daemon-reload
-    systemctl --user enable gmcapsule.service
+    systemctl --user enable gmcapsule
     systemctl --user start gmcapsule
 
 The log can be viewed via journalctl (or syslog):
 
     journalctl -xe --user-unit=gmcapsule
 
 ## Change log
 
+### v0.4
+
+* Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
+* Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
+* Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
+
 ### v0.3
 
 * Added a shutdown event for custom background workers.
 * `Request.query` is None if there is no query string present. Previously, the query string was an empty string in this case. This allows making a distinction between empty and absent query strings.
 
 v0.3.1:
```

### Comparing `gmcapsule-0.3.2/pyproject.toml` & `gmcapsule-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.3.2/PKG-INFO` & `gmcapsule-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmcapsule
-Version: 0.3.2
+Version: 0.4.0
 Summary: Extensible Gemini/Titan server
 Project-URL: Home-page, https://geminispace.org/gmcapsule/
 Project-URL: Documentation, https://geminispace.org/gmcapsule/gmcapsule.html
 Project-URL: Source, https://codeberg.org/skyjake/gmcapsule
 Project-URL: Issues, https://codeberg.org/skyjake/gmcapsule/issues
 Author-email: Jaakko Keränen <jaakko.keranen@iki.fi>
 Keywords: gemini,internet,server,titan
@@ -55,23 +55,29 @@
     WantedBy=default.target
 
 Replace `<YOUR-INSTALL-PATH>` with the actual path of `gmcapsuled`. `pip` will install it in a directory on your PATH.
 
 Then you can do the usual:
 
     systemctl --user daemon-reload
-    systemctl --user enable gmcapsule.service
+    systemctl --user enable gmcapsule
     systemctl --user start gmcapsule
 
 The log can be viewed via journalctl (or syslog):
 
     journalctl -xe --user-unit=gmcapsule
 
 ## Change log
 
+### v0.4
+
+* Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
+* Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
+* Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
+
 ### v0.3
 
 * Added a shutdown event for custom background workers.
 * `Request.query` is None if there is no query string present. Previously, the query string was an empty string in this case. This allows making a distinction between empty and absent query strings.
 
 v0.3.1:
```

