# Comparing `tmp/cardboard.py-0.0.6.tar.gz` & `tmp/cardboard.py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardboard.py-0.0.6.tar", last modified: Thu Jun  1 00:51:01 2023, max compression
+gzip compressed data, was "cardboard.py-0.0.7.tar", last modified: Thu Jun  1 01:09:48 2023, max compression
```

## Comparing `cardboard.py-0.0.6.tar` & `cardboard.py-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 00:51:01.477054 cardboard.py-0.0.6/
--rw-rw-rw-   0        0        0     4267 2023-06-01 00:51:01.475055 cardboard.py-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3338 2023-06-01 00:33:53.000000 cardboard.py-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 00:51:01.455052 cardboard.py-0.0.6/cardboard/
--rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.6/cardboard/Exceptions.py
--rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.6/cardboard/__init__.py
--rw-rw-rw-   0        0        0    10992 2023-06-01 00:32:48.000000 cardboard.py-0.0.6/cardboard/cardboard.py
--rw-rw-rw-   0        0        0    11857 2023-06-01 00:50:19.000000 cardboard.py-0.0.6/cardboard/cardboard_async.py
-drwxrwxrwx   0        0        0        0 2023-06-01 00:51:01.471057 cardboard.py-0.0.6/cardboard.py.egg-info/
--rw-rw-rw-   0        0        0     4267 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 00:51:01.000000 cardboard.py-0.0.6/cardboard.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 00:51:01.477054 cardboard.py-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-06-01 00:50:56.000000 cardboard.py-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:09:48.207774 cardboard.py-0.0.7/
+-rw-rw-rw-   0        0        0     4360 2023-06-01 01:09:48.206777 cardboard.py-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3427 2023-06-01 00:53:19.000000 cardboard.py-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 01:09:48.192774 cardboard.py-0.0.7/cardboard/
+-rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.7/cardboard/Exceptions.py
+-rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.7/cardboard/__init__.py
+-rw-rw-rw-   0        0        0    11004 2023-06-01 00:55:29.000000 cardboard.py-0.0.7/cardboard/cardboard.py
+-rw-rw-rw-   0        0        0    11869 2023-06-01 00:55:46.000000 cardboard.py-0.0.7/cardboard/cardboard_async.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:09:48.203781 cardboard.py-0.0.7/cardboard.py.egg-info/
+-rw-rw-rw-   0        0        0     4360 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-01 01:09:48.000000 cardboard.py-0.0.7/cardboard.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 01:09:48.207774 cardboard.py-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-06-01 01:09:43.000000 cardboard.py-0.0.7/setup.py
```

### Comparing `cardboard.py-0.0.6/PKG-INFO` & `cardboard.py-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.6
+Version: 0.0.7
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -80,15 +80,19 @@
 
 # Documentation
 For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
 
 For detailed documentation on how to use the cardboard.py library, please wait while we write it lol.
 
 ### Methods
-A list of methods you can call with either Cardboard or CardboardAsync.
+A list of methods/attributes you can call with either Cardboard or CardboardAsync.
+- `.app_url` (str)
+- `.app_name` (str)
+- `.secret` (str)
+- `.client_id` (str)
 - `.revoke_token(token:str)` (bool)
 - `.get_token(code:str)` (class AuthToken)
     - `.token` (str)
     - `.token_type` (str)
     - `.refresh_token` (str)
     - `.expires_in` (int)
     - `._raw` (dict)
```

### Comparing `cardboard.py-0.0.6/README.md` & `cardboard.py-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,19 @@
 
 # Documentation
 For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
 
 For detailed documentation on how to use the cardboard.py library, please wait while we write it lol.
 
 ### Methods
-A list of methods you can call with either Cardboard or CardboardAsync.
+A list of methods/attributes you can call with either Cardboard or CardboardAsync.
+- `.app_url` (str)
+- `.app_name` (str)
+- `.secret` (str)
+- `.client_id` (str)
 - `.revoke_token(token:str)` (bool)
 - `.get_token(code:str)` (class AuthToken)
     - `.token` (str)
     - `.token_type` (str)
     - `.refresh_token` (str)
     - `.expires_in` (int)
     - `._raw` (dict)
```

### Comparing `cardboard.py-0.0.6/cardboard/Exceptions.py` & `cardboard.py-0.0.7/cardboard/Exceptions.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.6/cardboard/cardboard.py` & `cardboard.py-0.0.7/cardboard/cardboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self._session.headers.update({"Content-Type": "application/x-www-form-urlencoded"})
 
         def __check_verify(self) -> bool|list:
             """
             Verifies authentication data. ID and Secret.
 
             Returns:
-                bool|list: [True, app_name] if everything is valid, else False.
+                bool|list: [True, app_name, app_vanity] if everything is valid, else False.
             """
             resp = requests.post(self._baseurl+'/check', headers={'Content-Type': 'application/x-www-form-urlencoded'}, data={'client_id': self.client_id, 'client_secret': self.secret})
             if resp.status_code != 200:
                 return False
             return [True, resp.json()['name'], resp.json()['vanity']]
     
         self.__check_verify = lambda: __check_verify(self)
```

### Comparing `cardboard.py-0.0.6/cardboard/cardboard_async.py` & `cardboard.py-0.0.7/cardboard/cardboard_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self._session = aiohttp.ClientSession(headers={"Content-Type": "application/x-www-form-urlencoded"})
 
         async def __check_verify(self) -> bool|list:
             """
             Verifies authentication data. ID and Secret.
 
             Returns:
-                bool|list: [True, app_name] if everything is valid, else False.
+                bool|list: [True, app_name, app_vanity] if everything is valid, else False.
             """
             url = self._baseurl + '/check'
             async with aiohttp.ClientSession() as session:
                 async with session.post(
                     url,
                     data={'client_id': self.client_id, 'client_secret': self.secret},
                     headers={'Content-Type': 'application/x-www-form-urlencoded'}
```

### Comparing `cardboard.py-0.0.6/cardboard.py.egg-info/PKG-INFO` & `cardboard.py-0.0.7/cardboard.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.6
+Version: 0.0.7
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -80,15 +80,19 @@
 
 # Documentation
 For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
 
 For detailed documentation on how to use the cardboard.py library, please wait while we write it lol.
 
 ### Methods
-A list of methods you can call with either Cardboard or CardboardAsync.
+A list of methods/attributes you can call with either Cardboard or CardboardAsync.
+- `.app_url` (str)
+- `.app_name` (str)
+- `.secret` (str)
+- `.client_id` (str)
 - `.revoke_token(token:str)` (bool)
 - `.get_token(code:str)` (class AuthToken)
     - `.token` (str)
     - `.token_type` (str)
     - `.refresh_token` (str)
     - `.expires_in` (int)
     - `._raw` (dict)
```

### Comparing `cardboard.py-0.0.6/setup.py` & `cardboard.py-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cardboard.py',
-    version='0.0.6',
+    version='0.0.7',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://cardboard.ink/api/v1/',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cardboard-ink/cardboard.py/',
     packages=find_packages(),
```

