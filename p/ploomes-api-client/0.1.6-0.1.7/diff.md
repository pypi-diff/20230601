# Comparing `tmp/ploomes-api-client-0.1.6.tar.gz` & `tmp/ploomes-api-client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.1.6.tar", last modified: Wed May 31 19:43:53 2023, max compression
+gzip compressed data, was "ploomes-api-client-0.1.7.tar", last modified: Thu Jun  1 21:49:44 2023, max compression
```

## Comparing `ploomes-api-client-0.1.6.tar` & `ploomes-api-client-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:43:53.115454 ploomes-api-client-0.1.6/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.6/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:43:53.115316 ploomes-api-client-0.1.6/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.6/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:43:53.114442 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-31 19:43:53.000000 ploomes-api-client-0.1.6/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:43:53.114661 ploomes-api-client-0.1.6/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.6/ploomes_client/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    24697 2023-05-31 19:43:22.000000 ploomes-api-client-0.1.6/ploomes_client/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-31 19:43:53.115505 ploomes-api-client-0.1.6/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-31 19:43:50.000000 ploomes-api-client-0.1.6/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 21:49:44.501585 ploomes-api-client-0.1.7/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.7/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-06-01 21:49:44.501431 ploomes-api-client-0.1.7/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.7/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 21:49:44.500456 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 21:49:44.500889 ploomes-api-client-0.1.7/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.7/ploomes_client/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    24693 2023-06-01 21:46:49.000000 ploomes-api-client-0.1.7/ploomes_client/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-01 21:49:44.501637 ploomes-api-client-0.1.7/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-01 21:49:43.000000 ploomes-api-client-0.1.7/setup.py
```

### Comparing `ploomes-api-client-0.1.6/LICENSE` & `ploomes-api-client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.6/PKG-INFO` & `ploomes-api-client-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.6/README.md` & `ploomes-api-client-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.6/ploomes_api_client.egg-info/PKG-INFO` & `ploomes-api-client-0.1.7/ploomes_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.6/ploomes_client/ploomes_client.py` & `ploomes-api-client-0.1.7/ploomes_client/ploomes_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,17 +318,17 @@
         response = r.json()
         print(response)
         return response
 
     @retry
     @sleep_and_retry
     @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
-    def get_field(self, name):
+    def get_field(self, _filter):
         r = requests.get(
-            f"{self.host}/Fields?$filter=Name+eq+'{name}'&$expand=Type,OptionsTable($expand=Options)",
+            f"{self.host}/Fields?$filter={_filter}&$expand=Type,OptionsTable($expand=Options)",
             headers=self.headers,
         )
         response = r.json().get("value")
         if response:
             item = next(iter(response))
             return item
         return None
```

### Comparing `ploomes-api-client-0.1.6/setup.py` & `ploomes-api-client-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

