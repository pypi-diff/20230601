# Comparing `tmp/heaven-0.0.1.tar.gz` & `tmp/heaven-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.1.tar", max compression
+gzip compressed data, was "heaven-0.0.2.tar", max compression
```

## Comparing `heaven-0.0.1.tar` & `heaven-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.1/LICENSE
--rw-r--r--   0        0        0     1312 2023-05-03 15:13:50.357871 heaven-0.0.1/README.md
--rw-r--r--   0        0        0      150 2023-05-03 15:19:47.360667 heaven-0.0.1/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-04-04 16:11:34.731647 heaven-0.0.1/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-04-04 16:11:34.731908 heaven-0.0.1/heaven/context.py
--rw-r--r--   0        0        0      141 2023-04-04 16:11:34.732086 heaven-0.0.1/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-05-03 15:18:16.753088 heaven-0.0.1/heaven/form.py
--rw-r--r--   0        0        0     2920 2023-05-03 15:18:08.445234 heaven-0.0.1/heaven/mocks.py
--rw-r--r--   0        0        0     3188 2023-05-03 15:14:18.988470 heaven-0.0.1/heaven/request.py
--rw-r--r--   0        0        0     2830 2023-05-03 15:15:09.488292 heaven-0.0.1/heaven/response.py
--rw-r--r--   0        0        0    19341 2023-05-03 15:17:31.053754 heaven-0.0.1/heaven/router.py
--rw-r--r--   0        0        0        0 2023-04-04 16:11:34.733604 heaven-0.0.1/heaven/server.py
--rw-r--r--   0        0        0      926 2023-04-04 16:11:34.734047 heaven-0.0.1/heaven/utils.py
--rw-r--r--   0        0        0      467 2023-05-03 15:11:27.649325 heaven-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 heaven-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1312 2023-05-03 15:13:50.357871 heaven-0.0.2/README.md
+-rw-r--r--   0        0        0      216 2023-06-01 15:02:47.533018 heaven-0.0.2/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-04 16:11:34.731647 heaven-0.0.2/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-04-04 16:11:34.731908 heaven-0.0.2/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-04-04 16:11:34.732086 heaven-0.0.2/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-05-03 15:18:16.753088 heaven-0.0.2/heaven/form.py
+-rw-r--r--   0        0        0     2920 2023-05-03 15:18:08.445234 heaven-0.0.2/heaven/mocks.py
+-rw-r--r--   0        0        0     3188 2023-05-04 09:15:57.271144 heaven-0.0.2/heaven/request.py
+-rw-r--r--   0        0        0     2830 2023-05-03 15:15:09.488292 heaven-0.0.2/heaven/response.py
+-rw-r--r--   0        0        0    19425 2023-06-01 15:02:38.459653 heaven-0.0.2/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-04-04 16:11:34.733604 heaven-0.0.2/heaven/server.py
+-rw-r--r--   0        0        0      926 2023-04-04 16:11:34.734047 heaven-0.0.2/heaven/utils.py
+-rw-r--r--   0        0        0      467 2023-06-01 15:03:12.819675 heaven-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 heaven-0.0.2/PKG-INFO
```

### Comparing `heaven-0.0.1/LICENSE` & `heaven-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/README.md` & `heaven-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/heaven/constants.py` & `heaven-0.0.2/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/heaven/form.py` & `heaven-0.0.2/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/heaven/mocks.py` & `heaven-0.0.2/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/heaven/request.py` & `heaven-0.0.2/heaven/request.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/heaven/response.py` & `heaven-0.0.2/heaven/response.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/heaven/router.py` & `heaven-0.0.2/heaven/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,7 +493,12 @@
                     handler = cache[route]
                     self.subdomain(subdomain)
                     self.abettor(method, route, handler, subdomain=subdomain, router=router if isolated else self)
             for after in engine.afters:
                 self.subdomains[subdomain].afters[after] = [*engine.afters[after], *self.subdomains[subdomain].afters.get(after, [])]
             for before in engine.befores:
                 self.subdomains[subdomain].befores[before] = [*engine.befores[before], *self.subdomains[subdomain].befores.get(before, [])]
+
+
+class Application(Router):...
+class App(Router):...
+class Server(Router):...
```

### Comparing `heaven-0.0.1/heaven/utils.py` & `heaven-0.0.2/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.1/PKG-INFO` & `heaven-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

