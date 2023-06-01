# Comparing `tmp/vaksms-0.2.tar.gz` & `tmp/vaksms-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaksms-0.2.tar", last modified: Mon May 29 07:16:12 2023, max compression
+gzip compressed data, was "vaksms-0.3.tar", last modified: Thu Jun  1 19:51:04 2023, max compression
```

## Comparing `vaksms-0.2.tar` & `vaksms-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:16:12.936362 vaksms-0.2/
--rw-rw-rw-   0        0        0     2256 2023-05-29 07:16:12.936362 vaksms-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1508 2023-05-28 21:34:42.000000 vaksms-0.2/README.md
--rw-rw-rw-   0        0        0      486 2023-05-29 07:16:12.936362 vaksms-0.2/setup.cfg
--rw-rw-rw-   0        0        0      910 2023-05-29 07:15:52.000000 vaksms-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:16:12.920743 vaksms-0.2/vaksms/
--rw-rw-rw-   0        0        0     6625 2023-05-28 21:38:06.000000 vaksms-0.2/vaksms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:16:12.936362 vaksms-0.2/vaksms.egg-info/
--rw-rw-rw-   0        0        0     2256 2023-05-29 07:16:12.000000 vaksms-0.2/vaksms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-29 07:16:12.000000 vaksms-0.2/vaksms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:16:12.000000 vaksms-0.2/vaksms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-29 07:16:12.000000 vaksms-0.2/vaksms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 07:16:12.000000 vaksms-0.2/vaksms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 19:51:04.398624 vaksms-0.3/
+-rw-rw-rw-   0        0        0     2256 2023-06-01 19:51:04.398624 vaksms-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1508 2023-05-28 21:34:42.000000 vaksms-0.3/README.md
+-rw-rw-rw-   0        0        0      486 2023-06-01 19:51:04.398624 vaksms-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      910 2023-06-01 19:50:54.000000 vaksms-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:51:04.398624 vaksms-0.3/vaksms/
+-rw-rw-rw-   0        0        0     6586 2023-06-01 19:49:59.000000 vaksms-0.3/vaksms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:51:04.398624 vaksms-0.3/vaksms.egg-info/
+-rw-rw-rw-   0        0        0     2256 2023-06-01 19:51:04.000000 vaksms-0.3/vaksms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-01 19:51:04.000000 vaksms-0.3/vaksms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:51:04.000000 vaksms-0.3/vaksms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-01 19:51:04.000000 vaksms-0.3/vaksms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 19:51:04.000000 vaksms-0.3/vaksms.egg-info/top_level.txt
```

### Comparing `vaksms-0.2/PKG-INFO` & `vaksms-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaksms
-Version: 0.2
+Version: 0.3
 Summary: VakSms API library
 Home-page: https://github.com/Pr0n1xGH/vaksms
 Author: PrOn1x
 Author-email: prosto.nechyvak@yahoo.com
 License: AGPL-3.0
 Keywords: vak-sms sms api library
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vaksms-0.2/README.md` & `vaksms-0.3/README.md`

 * *Files identical despite different names*

### Comparing `vaksms-0.2/setup.py` & `vaksms-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
     name='vaksms',
-    version='0.2',
+    version='0.3',
     description='VakSms API library',
     long_description=readme(),
     url='https://github.com/Pr0n1xGH/vaksms',
     author='PrOn1x',
     author_email='prosto.nechyvak@yahoo.com',
     license='AGPL-3.0',
     classifiers=[
```

### Comparing `vaksms-0.2/vaksms/__init__.py` & `vaksms-0.3/vaksms/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
     def getCountNumber(
             self, 
             service: str, 
             country: str = "ru", 
             operator: str = None, 
-            price: str = None,
+            price: bool = False,
             numList: bool = False
     ):
         """Gives the number of available numbers
 
         -----------------------------------------------------
 
         `Args`:
@@ -69,25 +69,25 @@
 
         `Countres and operators`: https://vak-sms.com/api/vak/#countryOperatorList1
         
         """
 
         if numList == True: ...
 
-        url = f"https://vak-sms.com/api/getCountNumber/?apiKey={self.ApiKey}&service={service}&country={country}&operator={operator}&price={price}"
+        url = f"https://vak-sms.com/api/getCountNumber/?apiKey={self.ApiKey}&service={service}&country={country}&operator={operator}&price"
 
         if operator is None:
             url = re.sub(f"&operator={operator}", "", url)
         
-        if price is None:
-            url = re.sub(f"&price={price}", "", url)
+        if price is False:
+            url = re.sub(f"&price", "", url)
 
         getCountNumber = requests.get(url).text
 
-        return json.loads(getCountNumber)[f'{service}']
+        return getCountNumber
     
     
     def getNumber(
             self,
             service: str,
             rent: bool = False,
             country: str = "ru",
```

### Comparing `vaksms-0.2/vaksms.egg-info/PKG-INFO` & `vaksms-0.3/vaksms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaksms
-Version: 0.2
+Version: 0.3
 Summary: VakSms API library
 Home-page: https://github.com/Pr0n1xGH/vaksms
 Author: PrOn1x
 Author-email: prosto.nechyvak@yahoo.com
 License: AGPL-3.0
 Keywords: vak-sms sms api library
 Classifier: Development Status :: 3 - Alpha
```

