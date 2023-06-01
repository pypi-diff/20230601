# Comparing `tmp/hukudo-ingress-1.1.0.tar.gz` & `tmp/hukudo-ingress-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hukudo-ingress-1.1.0.tar", last modified: Thu Nov  3 12:07:02 2022, max compression
+gzip compressed data, was "hukudo-ingress-2.0.0.tar", last modified: Thu Jun  1 14:04:11 2023, max compression
```

## Comparing `hukudo-ingress-1.1.0.tar` & `hukudo-ingress-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2022-11-03 12:07:02.693671 hukudo-ingress-1.1.0/
--rw-rw-r--   0 felix     (1337) felix     (1337)      637 2022-11-03 12:07:02.693671 hukudo-ingress-1.1.0/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      329 2022-10-21 10:31:18.000000 hukudo-ingress-1.1.0/README.md
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2022-11-03 12:07:02.693671 hukudo-ingress-1.1.0/hukudo_ingress.egg-info/
--rw-rw-r--   0 felix     (1337) felix     (1337)      637 2022-11-03 12:07:02.000000 hukudo-ingress-1.1.0/hukudo_ingress.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      417 2022-11-03 12:07:02.000000 hukudo-ingress-1.1.0/hukudo_ingress.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        1 2022-11-03 12:07:02.000000 hukudo-ingress-1.1.0/hukudo_ingress.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)       45 2022-11-03 12:07:02.000000 hukudo-ingress-1.1.0/hukudo_ingress.egg-info/entry_points.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)      163 2022-11-03 12:07:02.000000 hukudo-ingress-1.1.0/hukudo_ingress.egg-info/requires.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        8 2022-11-03 12:07:02.000000 hukudo-ingress-1.1.0/hukudo_ingress.egg-info/top_level.txt
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2022-11-03 12:07:02.693671 hukudo-ingress-1.1.0/ingress/
--rw-rw-r--   0 felix     (1337) felix     (1337)       22 2022-10-21 10:31:18.000000 hukudo-ingress-1.1.0/ingress/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1258 2022-09-09 11:32:56.000000 hukudo-ingress-1.1.0/ingress/caddy.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2137 2022-10-21 11:24:45.000000 hukudo-ingress-1.1.0/ingress/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2116 2022-09-09 11:32:56.000000 hukudo-ingress-1.1.0/ingress/config.py
--rw-rw-r--   0 felix     (1337) felix     (1337)       38 2022-09-09 11:32:56.000000 hukudo-ingress-1.1.0/ingress/exceptions.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     3888 2022-10-20 15:08:23.000000 hukudo-ingress-1.1.0/ingress/main.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1991 2022-10-21 10:31:08.000000 hukudo-ingress-1.1.0/ingress/models.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      659 2022-09-09 11:32:56.000000 hukudo-ingress-1.1.0/ingress/repo.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      511 2022-09-09 16:28:41.000000 hukudo-ingress-1.1.0/ingress/utils.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      707 2022-11-03 12:07:02.693671 hukudo-ingress-1.1.0/setup.cfg
--rw-rw-r--   0 felix     (1337) felix     (1337)      348 2022-09-09 11:32:56.000000 hukudo-ingress-1.1.0/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-01 14:04:11.399649 hukudo-ingress-2.0.0/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      637 2023-06-01 14:04:11.399649 hukudo-ingress-2.0.0/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      329 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/README.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-01 14:04:11.399649 hukudo-ingress-2.0.0/hukudo_ingress.egg-info/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      637 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/hukudo_ingress.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      499 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/hukudo_ingress.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/hukudo_ingress.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       45 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/hukudo_ingress.egg-info/entry_points.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)      163 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/hukudo_ingress.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        8 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/hukudo_ingress.egg-info/top_level.txt
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-01 14:04:11.399649 hukudo-ingress-2.0.0/ingress/
+-rw-rw-r--   0 felix     (1000) felix     (1000)       22 2023-06-01 14:04:11.000000 hukudo-ingress-2.0.0/ingress/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1258 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/ingress/caddy.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2137 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/ingress/cli.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2116 2023-06-01 13:53:02.000000 hukudo-ingress-2.0.0/ingress/config.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/ingress/exceptions.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     3888 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/ingress/main.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1991 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/ingress/models.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      659 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/ingress/repo.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      511 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/ingress/utils.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      707 2023-06-01 14:04:11.399649 hukudo-ingress-2.0.0/setup.cfg
+-rw-rw-r--   0 felix     (1000) felix     (1000)      348 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-01 14:04:11.399649 hukudo-ingress-2.0.0/tests/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      317 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/tests/test_caddy.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      319 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/tests/test_logging.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      594 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/tests/test_models.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      317 2023-06-01 13:48:21.000000 hukudo-ingress-2.0.0/tests/test_repo.py
```

### Comparing `hukudo-ingress-1.1.0/PKG-INFO` & `hukudo-ingress-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hukudo-ingress
-Version: 1.1.0
+Version: 2.0.0
 Home-page: https://gitlab.com/hukudo/ingress
 Author: hukudo GmbH
 Author-email: hukudo-ingress@hukudo.de
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: include_package_data
 
 # Ingress
 Configure Caddy as an ingress for your Docker containers.
 
 ## Usage
 ```
-pip install hukudo-ingress==1.1.0
+pip install hukudo-ingress==2.0.0
 ingress --help
 ```
 
 ## Development
 Initial
 ```
 make dev-setup
```

### Comparing `hukudo-ingress-1.1.0/hukudo_ingress.egg-info/PKG-INFO` & `hukudo-ingress-2.0.0/hukudo_ingress.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hukudo-ingress
-Version: 1.1.0
+Version: 2.0.0
 Home-page: https://gitlab.com/hukudo/ingress
 Author: hukudo GmbH
 Author-email: hukudo-ingress@hukudo.de
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: include_package_data
 
 # Ingress
 Configure Caddy as an ingress for your Docker containers.
 
 ## Usage
 ```
-pip install hukudo-ingress==1.1.0
+pip install hukudo-ingress==2.0.0
 ingress --help
 ```
 
 ## Development
 Initial
 ```
 make dev-setup
```

### Comparing `hukudo-ingress-1.1.0/ingress/caddy.py` & `hukudo-ingress-2.0.0/ingress/caddy.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-1.1.0/ingress/cli.py` & `hukudo-ingress-2.0.0/ingress/cli.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-1.1.0/ingress/config.py` & `hukudo-ingress-2.0.0/ingress/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
 def get_caddyfile() -> Path:
     return Path('Caddyfile')
 
 
 def get_caddy_container_name() -> str:
-    return 'ingress_caddy_1'
+    return 'ingress-caddy-1'
 
 
 def get_caddy_hostname():
     result = 'localhost'
     if socket.gethostname() == 'controller.ingress':
         result = 'caddy.ingress'
     return result
```

### Comparing `hukudo-ingress-1.1.0/ingress/main.py` & `hukudo-ingress-2.0.0/ingress/main.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-1.1.0/ingress/models.py` & `hukudo-ingress-2.0.0/ingress/models.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-1.1.0/ingress/repo.py` & `hukudo-ingress-2.0.0/ingress/repo.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-1.1.0/setup.cfg` & `hukudo-ingress-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hukudo-ingress
-version = 1.1.0
+version = 2.0.0
 url = https://gitlab.com/hukudo/ingress
 author = hukudo GmbH
 author_email = hukudo-ingress@hukudo.de
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
```

