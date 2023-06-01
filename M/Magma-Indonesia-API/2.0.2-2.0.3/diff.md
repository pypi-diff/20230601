# Comparing `tmp/Magma-Indonesia-API-2.0.2.tar.gz` & `tmp/Magma-Indonesia-API-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Magma-Indonesia-API-2.0.2.tar", last modified: Thu Jun  1 09:51:57 2023, max compression
+gzip compressed data, was "Magma-Indonesia-API-2.0.3.tar", last modified: Thu Jun  1 10:00:43 2023, max compression
```

## Comparing `Magma-Indonesia-API-2.0.2.tar` & `Magma-Indonesia-API-2.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:51:57.261935 Magma-Indonesia-API-2.0.2/
--rw-rw-rw-   0        0        0     1086 2023-02-04 06:40:25.000000 Magma-Indonesia-API-2.0.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 09:51:57.257966 Magma-Indonesia-API-2.0.2/Magma/
--rw-rw-rw-   0        0        0     5847 2023-06-01 09:50:59.000000 Magma-Indonesia-API-2.0.2/Magma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:51:57.261157 Magma-Indonesia-API-2.0.2/Magma_Indonesia_API.egg-info/
--rw-rw-rw-   0        0        0      706 2023-06-01 09:51:57.000000 Magma-Indonesia-API-2.0.2/Magma_Indonesia_API.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-01 09:51:57.000000 Magma-Indonesia-API-2.0.2/Magma_Indonesia_API.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:51:57.000000 Magma-Indonesia-API-2.0.2/Magma_Indonesia_API.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-01 09:51:57.000000 Magma-Indonesia-API-2.0.2/Magma_Indonesia_API.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      706 2023-06-01 09:51:57.261935 Magma-Indonesia-API-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-02-04 06:39:44.000000 Magma-Indonesia-API-2.0.2/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:51:57.262936 Magma-Indonesia-API-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      947 2023-06-01 09:51:33.000000 Magma-Indonesia-API-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:00:43.489693 Magma-Indonesia-API-2.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-02-04 06:40:25.000000 Magma-Indonesia-API-2.0.3/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 10:00:43.480124 Magma-Indonesia-API-2.0.3/Magma/
+-rw-rw-rw-   0        0        0     5849 2023-06-01 10:00:07.000000 Magma-Indonesia-API-2.0.3/Magma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:00:43.489592 Magma-Indonesia-API-2.0.3/Magma_Indonesia_API.egg-info/
+-rw-rw-rw-   0        0        0      706 2023-06-01 10:00:43.000000 Magma-Indonesia-API-2.0.3/Magma_Indonesia_API.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-01 10:00:43.000000 Magma-Indonesia-API-2.0.3/Magma_Indonesia_API.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 10:00:43.000000 Magma-Indonesia-API-2.0.3/Magma_Indonesia_API.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 10:00:43.000000 Magma-Indonesia-API-2.0.3/Magma_Indonesia_API.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      706 2023-06-01 10:00:43.490189 Magma-Indonesia-API-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-02-04 06:39:44.000000 Magma-Indonesia-API-2.0.3/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 10:00:43.491449 Magma-Indonesia-API-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      947 2023-06-01 10:00:38.000000 Magma-Indonesia-API-2.0.3/setup.py
```

### Comparing `Magma-Indonesia-API-2.0.2/LICENSE.txt` & `Magma-Indonesia-API-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Magma-Indonesia-API-2.0.2/Magma/__init__.py` & `Magma-Indonesia-API-2.0.3/Magma/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     else:
         totalpage = 1
     month = {"Januari":"January","Februari":"February","Maret":"March","April":"April","Mei":"May","Juni":"June","Juli":"July","Agustus":"August","September":"September","Oktober":"October","November":"November","Desember":"December"}
     day = {"Senin":"Monday","Selasa":"Tuesday","Rabu":"Wednesday","Kamis":"Thursday","Jumat":"Friday","Sabtu":"Saturday","Minggu":"Sunday"}
     judul = ""
     checking = 0
     while checking < totalpage:
-        web = asyncio.run(link(f"https://magma.esdm.go.id/v1/gunung-api/informasi-letusan?page={checking}"))
+        web = asyncio.run(link(f"https://magma.esdm.go.id/v1/gunung-api/informasi-letusan?page={checking+1}"))
         HTMLResult = BeautifulSoup(web, "html.parser") 
         content = HTMLResult.find_all('div', class_="timeline-item")
         for i in content:
             if len(i.attrs['class']) >= 2:
                 date = ((i.find('p', class_="timeline-date")).get_text(strip=True).split(", "))[1].split(" ")
                 if date[0] in list(day.keys()):
                     date = (i.get_text(strip=True).split(", ")[2]).split(" ")
```

### Comparing `Magma-Indonesia-API-2.0.2/Magma_Indonesia_API.egg-info/PKG-INFO` & `Magma-Indonesia-API-2.0.3/Magma_Indonesia_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Magma-Indonesia-API
-Version: 2.0.2
+Version: 2.0.3
 Summary: Magma-Indonesia-API is an unofficial API made with Python language!
 Home-page: https://github.com/Gabrielbjb/Magma-Indonesia-API
 Author: Gabrielbjb
 Author-email: gabrielbjb@protonmail.com
 License: MIT
 Keywords: Python,Indonesia,Magma Indonesia,Volcano,Magma,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Magma-Indonesia-API-2.0.2/PKG-INFO` & `Magma-Indonesia-API-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Magma-Indonesia-API
-Version: 2.0.2
+Version: 2.0.3
 Summary: Magma-Indonesia-API is an unofficial API made with Python language!
 Home-page: https://github.com/Gabrielbjb/Magma-Indonesia-API
 Author: Gabrielbjb
 Author-email: gabrielbjb@protonmail.com
 License: MIT
 Keywords: Python,Indonesia,Magma Indonesia,Volcano,Magma,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Magma-Indonesia-API-2.0.2/setup.py` & `Magma-Indonesia-API-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
  
 setup(
     name="Magma-Indonesia-API",
-    version="2.0.2",
+    version="2.0.3",
     description="Magma-Indonesia-API is an unofficial API made with Python language!",
     long_description=readme(),
     long_description_content_type="",
     url="https://github.com/Gabrielbjb/Magma-Indonesia-API",
     author="Gabrielbjb",
     author_email="gabrielbjb@protonmail.com",
     license="MIT",
```

