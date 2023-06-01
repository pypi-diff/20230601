# Comparing `tmp/id4eo-scim-client-1.0.2.tar.gz` & `tmp/id4eo-scim-client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/id4eo-scim-client-1.0.2.tar", last modified: Thu Jun  1 16:21:07 2023, max compression
+gzip compressed data, was "dist/id4eo-scim-client-1.0.3.tar", last modified: Thu Jun  1 18:07:51 2023, max compression
```

## Comparing `id4eo-scim-client-1.0.2.tar` & `id4eo-scim-client-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/
-drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim/
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)      338 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.2/id4eo_scim/__init__.py
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)    28837 2023-06-01 16:18:56.000000 id4eo-scim-client-1.0.2/id4eo_scim/id4eo_scim.py
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)     3147 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.2/id4eo_scim/main.py
-drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)      532 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/PKG-INFO
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)      259 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/SOURCES.txt
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)        1 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/dependency_links.txt
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)       11 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/top_level.txt
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)     2842 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.2/README.md
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)       79 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/setup.cfg
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)      738 2023-06-01 16:21:06.000000 id4eo-scim-client-1.0.2/setup.py
--rw-r--r--   0 alvl       (508) gsc4eo    (1001)      532 2023-06-01 16:21:07.000000 id4eo-scim-client-1.0.2/PKG-INFO
+drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/
+drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/id4eo_scim/
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      338 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.3/id4eo_scim/__init__.py
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)    28842 2023-06-01 18:06:37.000000 id4eo-scim-client-1.0.3/id4eo_scim/id4eo_scim.py
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)     3147 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.3/id4eo_scim/main.py
+drwxr-xr-x   0 alvl       (508) gsc4eo    (1001)        0 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/id4eo_scim_client.egg-info/
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      532 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/id4eo_scim_client.egg-info/PKG-INFO
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      259 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/id4eo_scim_client.egg-info/SOURCES.txt
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)        1 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/id4eo_scim_client.egg-info/dependency_links.txt
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)       11 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/id4eo_scim_client.egg-info/top_level.txt
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)     2842 2023-05-24 15:13:31.000000 id4eo-scim-client-1.0.3/README.md
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)       79 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/setup.cfg
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      738 2023-06-01 18:07:40.000000 id4eo-scim-client-1.0.3/setup.py
+-rw-r--r--   0 alvl       (508) gsc4eo    (1001)      532 2023-06-01 18:07:51.000000 id4eo-scim-client-1.0.3/PKG-INFO
```

### Comparing `id4eo-scim-client-1.0.2/id4eo_scim/id4eo_scim.py` & `id4eo-scim-client-1.0.3/id4eo_scim/id4eo_scim.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             self.access_token = None
             return self.getUserAttributes(userID)
         logging.info("User attributes found, returning.")
         self.authRetries = 3
         return res.json()
 
     def addUserAttribute(self, userID, attributePath, newValue):
-        logging.info("Adding attribute " + attributePath + ", with value " + newValue + " to user " + userID)
+        logging.info("Adding attribute " + attributePath + ", with value " + str(newValue) + " to user " + userID)
         if self.client_id == None:
             logging.info("No client id found, please register first.")
             return None
         url = self.__SCIM_USERS_ENDPOINT + "/" + self.__getUserInum(userID)
         headers = {
             'content-type': "application/scim+json",
             'Authorization': self.createBearerToken(self.access_token if self.access_token is not None else '0')
```

### Comparing `id4eo-scim-client-1.0.2/id4eo_scim/main.py` & `id4eo-scim-client-1.0.3/id4eo_scim/main.py`

 * *Files identical despite different names*

### Comparing `id4eo-scim-client-1.0.2/id4eo_scim_client.egg-info/PKG-INFO` & `id4eo-scim-client-1.0.3/id4eo_scim_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: id4eo-scim-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library to interact with SCIM protocol
 Home-page: https://stash.elecnor-deimos.com/projects/GSC4EO/repos/id4eo/browse/src/scim-client
 Author: ID4EO
 Author-email: joao.matos@elecnor.es
 License: apache-2.0
 Description: UNKNOWN
 Keywords: SCIM,Client,ID4EO,user,management
```

### Comparing `id4eo-scim-client-1.0.2/README.md` & `id4eo-scim-client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `id4eo-scim-client-1.0.2/setup.py` & `id4eo-scim-client-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
   name = 'id4eo-scim-client',
-  version = '1.0.2',
+  version = '1.0.3',
   author = 'ID4EO',
   author_email = 'joao.matos@elecnor.es',
   description = 'Python library to interact with SCIM protocol',
   url = 'https://stash.elecnor-deimos.com/projects/GSC4EO/repos/id4eo/browse/src/scim-client',
   packages=setuptools.find_packages(),
   license='apache-2.0',
   keywords = ['SCIM', 'Client', 'ID4EO','user','management'],
```

### Comparing `id4eo-scim-client-1.0.2/PKG-INFO` & `id4eo-scim-client-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: id4eo-scim-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library to interact with SCIM protocol
 Home-page: https://stash.elecnor-deimos.com/projects/GSC4EO/repos/id4eo/browse/src/scim-client
 Author: ID4EO
 Author-email: joao.matos@elecnor.es
 License: apache-2.0
 Description: UNKNOWN
 Keywords: SCIM,Client,ID4EO,user,management
```

