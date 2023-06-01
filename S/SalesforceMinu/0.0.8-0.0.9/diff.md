# Comparing `tmp/SalesforceMinu-0.0.8.tar.gz` & `tmp/SalesforceMinu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalesforceMinu-0.0.8.tar", last modified: Tue May 30 15:28:33 2023, max compression
+gzip compressed data, was "SalesforceMinu-0.0.9.tar", last modified: Thu Jun  1 16:33:25 2023, max compression
```

## Comparing `SalesforceMinu-0.0.8.tar` & `SalesforceMinu-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:28:33.714981 SalesforceMinu-0.0.8/
--rw-rw-rw-   0        0        0      610 2023-05-30 15:28:33.713983 SalesforceMinu-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-30 15:16:29.000000 SalesforceMinu-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 15:28:33.694036 SalesforceMinu-0.0.8/SalesforceMinu/
--rw-rw-rw-   0        0        0     4813 2023-05-30 15:15:35.000000 SalesforceMinu-0.0.8/SalesforceMinu/Funciones.py
--rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.8/SalesforceMinu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:28:33.713017 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 15:28:33.714981 SalesforceMinu-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-05-30 15:16:19.000000 SalesforceMinu-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:33:25.051892 SalesforceMinu-0.0.9/
+-rw-rw-rw-   0        0        0      610 2023-06-01 16:33:25.051892 SalesforceMinu-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-30 15:16:29.000000 SalesforceMinu-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 16:33:25.027958 SalesforceMinu-0.0.9/SalesforceMinu/
+-rw-rw-rw-   0        0        0     4818 2023-06-01 16:29:47.000000 SalesforceMinu-0.0.9/SalesforceMinu/Funciones.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.9/SalesforceMinu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:33:25.049896 SalesforceMinu-0.0.9/SalesforceMinu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-06-01 16:33:24.000000 SalesforceMinu-0.0.9/SalesforceMinu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-01 16:33:24.000000 SalesforceMinu-0.0.9/SalesforceMinu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 16:33:24.000000 SalesforceMinu-0.0.9/SalesforceMinu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 16:33:24.000000 SalesforceMinu-0.0.9/SalesforceMinu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 16:33:24.000000 SalesforceMinu-0.0.9/SalesforceMinu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 16:33:25.052889 SalesforceMinu-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-06-01 16:29:56.000000 SalesforceMinu-0.0.9/setup.py
```

### Comparing `SalesforceMinu-0.0.8/PKG-INFO` & `SalesforceMinu-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.8
+Version: 0.0.9
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `SalesforceMinu-0.0.8/SalesforceMinu/Funciones.py` & `SalesforceMinu-0.0.9/SalesforceMinu/Funciones.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,27 @@
     # Convertimos a lista
     names = names.split(',')
     return names
 
 # OBTENER LOS IDS DE ACCOUNT Y EL ORDEN DE SUS NOMBRE
 # Si no encuentra el nombre que mande mensaje de error o algo
 def get_account_id_names(names,sf):
-    from unicodedata import normalize
+    #from unicodedata import normalize
 
     # Puede ser un nombre o varios
     case = 0
     if type(names) == str:
         name = str(names)[1:-1]
-        trans_tab = dict.fromkeys(map(ord, u'\u0301\u0308'), None)
-        name = normalize('NFKC', normalize('NFKD', name).translate(trans_tab))
+        #trans_tab = dict.fromkeys(map(ord, u'\u0301\u0308'), None)
+        #name = normalize('NFKC', normalize('NFKD', name).translate(trans_tab))
         where = f"Name = '{name}'"
     else:
         name = str(names)[1:-1]
-        trans_tab = dict.fromkeys(map(ord, u'\u0301\u0308'), None)
-        name = normalize('NFKC', normalize('NFKD', name).translate(trans_tab))
+        #trans_tab = dict.fromkeys(map(ord, u'\u0301\u0308'), None)
+        #name = normalize('NFKC', normalize('NFKD', name).translate(trans_tab))
         where = f"Name IN ({name})"
         case = 1
     
     query = f"""SELECT Id, Name, NumberOfEmployees
     FROM Account
     WHERE {where}
     AND Etapa_de_Oportunidad__c LIKE '%TyC firmado%'"""
```

### Comparing `SalesforceMinu-0.0.8/SalesforceMinu.egg-info/PKG-INFO` & `SalesforceMinu-0.0.9/SalesforceMinu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.8
+Version: 0.0.9
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `SalesforceMinu-0.0.8/setup.py` & `SalesforceMinu-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 PACKAGE_NAME = 'SalesforceMinu' 
 AUTHOR = 'Corchado Ramos Itzae Balam' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'g7_corc18@ens.cnyn.unam.mx' 
 URL = 'https://github.com/BalamCor?tab=repositories' 
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para extraer datos de minu en salesforce'
```

