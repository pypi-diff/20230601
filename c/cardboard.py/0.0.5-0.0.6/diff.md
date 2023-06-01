# Comparing `tmp/cardboard.py-0.0.5.tar.gz` & `tmp/cardboard.py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardboard.py-0.0.5.tar", last modified: Thu Jun  1 00:47:42 2023, max compression
+gzip compressed data, was "cardboard.py-0.0.6.tar", last modified: Thu Jun  1 00:51:01 2023, max compression
```

## Comparing `cardboard.py-0.0.5.tar` & `cardboard.py-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 00:47:42.603383 cardboard.py-0.0.5/
--rw-rw-rw-   0        0        0     4267 2023-06-01 00:47:42.602378 cardboard.py-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3338 2023-06-01 00:33:53.000000 cardboard.py-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 00:47:42.585382 cardboard.py-0.0.5/cardboard/
--rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.5/cardboard/Exceptions.py
--rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.5/cardboard/__init__.py
--rw-rw-rw-   0        0        0    10992 2023-06-01 00:32:48.000000 cardboard.py-0.0.5/cardboard/cardboard.py
--rw-rw-rw-   0        0        0    11814 2023-06-01 00:47:34.000000 cardboard.py-0.0.5/cardboard/cardboard_async.py
-drwxrwxrwx   0        0        0        0 2023-06-01 00:47:42.598381 cardboard.py-0.0.5/cardboard.py.egg-info/
--rw-rw-rw-   0        0        0     4267 2023-06-01 00:47:42.000000 cardboard.py-0.0.5/cardboard.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-01 00:47:42.000000 cardboard.py-0.0.5/cardboard.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 00:47:42.000000 cardboard.py-0.0.5/cardboard.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-01 00:47:42.000000 cardboard.py-0.0.5/cardboard.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 00:47:42.000000 cardboard.py-0.0.5/cardboard.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 00:47:42.603383 cardboard.py-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-06-01 00:34:55.000000 cardboard.py-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 00:51:01.477054 cardboard.py-0.0.6/
+-rw-rw-rw-   0        0        0     4267 2023-06-01 00:51:01.475055 cardboard.py-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3338 2023-06-01 00:33:53.000000 cardboard.py-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 00:51:01.455052 cardboard.py-0.0.6/cardboard/
+-rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.6/cardboard/Exceptions.py
+-rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.6/cardboard/__init__.py
+-rw-rw-rw-   0        0        0    10992 2023-06-01 00:32:48.000000 cardboard.py-0.0.6/cardboard/cardboard.py
+-rw-rw-rw-   0        0        0    11857 2023-06-01 00:50:19.000000 cardboard.py-0.0.6/cardboard/cardboard_async.py
+drwxrwxrwx   0        0        0        0 2023-06-01 00:51:01.471057 cardboard.py-0.0.6/cardboard.py.egg-info/
+-rw-rw-rw-   0        0        0     4267 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 00:51:01.477054 cardboard.py-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-06-01 00:50:56.000000 cardboard.py-0.0.6/setup.py
```

### Comparing `cardboard.py-0.0.5/PKG-INFO` & `cardboard.py-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.5
+Version: 0.0.6
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardboard.py-0.0.5/README.md` & `cardboard.py-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.5/cardboard/Exceptions.py` & `cardboard.py-0.0.6/cardboard/Exceptions.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.5/cardboard/cardboard.py` & `cardboard.py-0.0.6/cardboard/cardboard.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.5/cardboard/cardboard_async.py` & `cardboard.py-0.0.6/cardboard/cardboard_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     elif response.status == 429:
         raise RateLimited(await response.text())
     elif 200 <= response.status < 300:
         return False
     else:
         raise CardboardException(await response.text())
 
-class Cardboard:
+class CardboardAsync:
     """
-    Base Cardboard class for interacting with the Cardboard API.
+    Base asynchronous Cardboard class for interacting with the Cardboard API.
 
     Args:
         client_id (str): Your app's id.
         
         secret (str): Your app's secret.
     """
 
@@ -171,20 +171,20 @@
             userTransientStatus (str|None): The user's current transient status if applicable.
             _raw (dict): The raw data returned from the API.
         """
         def __init__(self, data):
             self.name:str = data["name"]
             self.id:str = data["id"]
             self.subdomain:str = data["subdomain"]
-            self.aliases:list = [Cardboard.UserAlias(data) for data in data["aliases"]]
+            self.aliases:list = [CardboardAsync.UserAlias(data) for data in data["aliases"]]
             self.avatar:str = data["avatar"]
             self.banner:str = data["banner"]
-            self.status:Cardboard.UserStatus = Cardboard.UserStatus(data["userStatus"])
+            self.status:CardboardAsync.UserStatus = CardboardAsync.UserStatus(data["userStatus"])
             self.moderationStatus:str|None = data["moderationStatus"]
-            self.aboutInfo:Cardboard.UserAbout = Cardboard.UserAbout(data["aboutInfo"])
+            self.aboutInfo:CardboardAsync.UserAbout = CardboardAsync.UserAbout(data["aboutInfo"])
             self.userTransientStatus:str|None = data["userTransientStatus"]
             self._raw:dict = data
 
     class AuthToken:
         """
         AuthToken object.
```

### Comparing `cardboard.py-0.0.5/cardboard.py.egg-info/PKG-INFO` & `cardboard.py-0.0.6/cardboard.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.5
+Version: 0.0.6
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardboard.py-0.0.5/setup.py` & `cardboard.py-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cardboard.py',
-    version='0.0.5',
+    version='0.0.6',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://cardboard.ink/api/v1/',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cardboard-ink/cardboard.py/',
     packages=find_packages(),
```

