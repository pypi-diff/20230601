# Comparing `tmp/Magma-Indonesia-API-2.0.0.tar.gz` & `tmp/Magma-Indonesia-API-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Magma-Indonesia-API-2.0.0.tar", last modified: Thu Jun  1 09:05:04 2023, max compression
+gzip compressed data, was "Magma-Indonesia-API-2.0.1.tar", last modified: Thu Jun  1 09:14:41 2023, max compression
```

## Comparing `Magma-Indonesia-API-2.0.0.tar` & `Magma-Indonesia-API-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:05:04.808390 Magma-Indonesia-API-2.0.0/
--rw-rw-rw-   0        0        0     1086 2023-02-04 06:40:25.000000 Magma-Indonesia-API-2.0.0/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 09:05:04.796684 Magma-Indonesia-API-2.0.0/Magma/
--rw-rw-rw-   0        0        0     5875 2023-06-01 08:46:19.000000 Magma-Indonesia-API-2.0.0/Magma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:05:04.806376 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/
--rw-rw-rw-   0        0        0      706 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      706 2023-06-01 09:05:04.808390 Magma-Indonesia-API-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-02-04 06:39:44.000000 Magma-Indonesia-API-2.0.0/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:05:04.809390 Magma-Indonesia-API-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      947 2023-06-01 08:48:18.000000 Magma-Indonesia-API-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:14:41.129981 Magma-Indonesia-API-2.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-02-04 06:40:25.000000 Magma-Indonesia-API-2.0.1/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 09:14:41.125481 Magma-Indonesia-API-2.0.1/Magma/
+-rw-rw-rw-   0        0        0     5847 2023-06-01 09:13:43.000000 Magma-Indonesia-API-2.0.1/Magma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:14:41.129981 Magma-Indonesia-API-2.0.1/Magma_Indonesia_API.egg-info/
+-rw-rw-rw-   0        0        0      706 2023-06-01 09:14:41.000000 Magma-Indonesia-API-2.0.1/Magma_Indonesia_API.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-01 09:14:41.000000 Magma-Indonesia-API-2.0.1/Magma_Indonesia_API.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:14:41.000000 Magma-Indonesia-API-2.0.1/Magma_Indonesia_API.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 09:14:41.000000 Magma-Indonesia-API-2.0.1/Magma_Indonesia_API.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      706 2023-06-01 09:14:41.129981 Magma-Indonesia-API-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-02-04 06:39:44.000000 Magma-Indonesia-API-2.0.1/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:14:41.131975 Magma-Indonesia-API-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      947 2023-06-01 09:14:07.000000 Magma-Indonesia-API-2.0.1/setup.py
```

### Comparing `Magma-Indonesia-API-2.0.0/LICENSE.txt` & `Magma-Indonesia-API-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Magma-Indonesia-API-2.0.0/Magma/__init__.py` & `Magma-Indonesia-API-2.0.1/Magma/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 gunung = (j.get_text(strip=True)).replace("Lihat laporan","").split(" - ")
                 result[judul2][gunung[0]] = {"location":gunung[1],"link":url[linkcheck]}
                 linkcheck += 1
             elif tes == False:
                 result[judul2] = {}
     return result
 
-def magmaeruption(page = "all"):
+def magmaeruption(page = 1):
     result = {}
     web = asyncio.run(link("https://magma.esdm.go.id/v1/gunung-api/informasi-letusan"))
     HTMLResult = BeautifulSoup(web, "html.parser") 
     pageHTML = int(HTMLResult.find('div', class_="ui pagination menu").find_all('a')[7].get_text(strip=True))+1
     if page == "all":
         totalpage = pageHTML
     elif isinstance(page, int):
@@ -52,15 +52,14 @@
     else:
         totalpage = 1
     month = {"Januari":"January","Februari":"February","Maret":"March","April":"April","Mei":"May","Juni":"June","Juli":"July","Agustus":"August","September":"September","Oktober":"October","November":"November","Desember":"December"}
     day = {"Senin":"Monday","Selasa":"Tuesday","Rabu":"Wednesday","Kamis":"Thursday","Jumat":"Friday","Sabtu":"Saturday","Minggu":"Sunday"}
     judul = ""
     checking = 1
     while checking < totalpage:
-        print("wow")
         web = asyncio.run(link(f"https://magma.esdm.go.id/v1/gunung-api/informasi-letusan?page={checking}"))
         HTMLResult = BeautifulSoup(web, "html.parser") 
         content = HTMLResult.find_all('div', class_="timeline-item")
         for i in content:
             if len(i.attrs['class']) >= 2:
                 date = ((i.find('p', class_="timeline-date")).get_text(strip=True).split(", "))[1].split(" ")
                 if date[0] in list(day.keys()):
@@ -72,15 +71,14 @@
             else:
                 clock = i.find('div', class_="timeline-time").get_text().split(" ")
 
                 if clock[1] in result[judul].keys():
                     result[judul][clock[1]].update({clock[0]: {"volcano_name": i.find('p', class_="timeline-title").get_text()}})
                 else:
                     result[judul][clock[1]] = {clock[0]:{"volcano_name": i.find('p', class_="timeline-title").get_text()}}
-
                 result[judul][clock[1]][clock[0]].update({"author": i.find_next(class_="timeline-author").get_text().replace("Dibuat oleh ","")})
                 result[judul][clock[1]][clock[0]].update({"information": i.find('p', class_="timeline-text").get_text(strip=True).replace("  ","")})
                 result[judul][clock[1]][clock[0]].update({"image": i.find('img', class_="bd img-fluid")['src']})
                 result[judul][clock[1]][clock[0]].update({"detail": i.find('a', class_="btn btn-sm btn-outline-primary")['href']})
         checking += 1
     return result
```

### Comparing `Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/PKG-INFO` & `Magma-Indonesia-API-2.0.1/Magma_Indonesia_API.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Magma-Indonesia-API
-Version: 2.0.0
+Version: 2.0.1
 Summary: Magma-Indonesia-API is an unofficial API made with Python language!
 Home-page: https://github.com/Gabrielbjb/Magma-Indonesia-API
 Author: Gabrielbjb
 Author-email: gabrielbjb@protonmail.com
 License: MIT
 Keywords: Python,Indonesia,Magma Indonesia,Volcano,Magma,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Magma-Indonesia-API-2.0.0/PKG-INFO` & `Magma-Indonesia-API-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Magma-Indonesia-API
-Version: 2.0.0
+Version: 2.0.1
 Summary: Magma-Indonesia-API is an unofficial API made with Python language!
 Home-page: https://github.com/Gabrielbjb/Magma-Indonesia-API
 Author: Gabrielbjb
 Author-email: gabrielbjb@protonmail.com
 License: MIT
 Keywords: Python,Indonesia,Magma Indonesia,Volcano,Magma,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Magma-Indonesia-API-2.0.0/setup.py` & `Magma-Indonesia-API-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
  
 setup(
     name="Magma-Indonesia-API",
-    version="2.0.0",
+    version="2.0.1",
     description="Magma-Indonesia-API is an unofficial API made with Python language!",
     long_description=readme(),
     long_description_content_type="",
     url="https://github.com/Gabrielbjb/Magma-Indonesia-API",
     author="Gabrielbjb",
     author_email="gabrielbjb@protonmail.com",
     license="MIT",
```

