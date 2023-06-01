# Comparing `tmp/Magma-Indonesia-API-1.0.1.tar.gz` & `tmp/Magma-Indonesia-API-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Magma-Indonesia-API-1.0.1.tar", last modified: Sat Feb  4 06:51:06 2023, max compression
+gzip compressed data, was "Magma-Indonesia-API-2.0.0.tar", last modified: Thu Jun  1 09:05:04 2023, max compression
```

## Comparing `Magma-Indonesia-API-1.0.1.tar` & `Magma-Indonesia-API-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-04 06:51:06.087176 Magma-Indonesia-API-1.0.1/
--rw-rw-rw-   0        0        0     1086 2023-02-04 06:40:25.000000 Magma-Indonesia-API-1.0.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-02-04 06:51:06.064854 Magma-Indonesia-API-1.0.1/Magma/
--rw-rw-rw-   0        0        0     3041 2023-02-04 06:50:09.000000 Magma-Indonesia-API-1.0.1/Magma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-04 06:51:06.082683 Magma-Indonesia-API-1.0.1/Magma_Indonesia_API.egg-info/
--rw-rw-rw-   0        0        0      706 2023-02-04 06:51:05.000000 Magma-Indonesia-API-1.0.1/Magma_Indonesia_API.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-02-04 06:51:05.000000 Magma-Indonesia-API-1.0.1/Magma_Indonesia_API.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-04 06:51:05.000000 Magma-Indonesia-API-1.0.1/Magma_Indonesia_API.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-04 06:51:05.000000 Magma-Indonesia-API-1.0.1/Magma_Indonesia_API.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      706 2023-02-04 06:51:06.087176 Magma-Indonesia-API-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-02-04 06:39:44.000000 Magma-Indonesia-API-1.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-02-04 06:51:06.087176 Magma-Indonesia-API-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      947 2023-02-04 06:50:58.000000 Magma-Indonesia-API-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:05:04.808390 Magma-Indonesia-API-2.0.0/
+-rw-rw-rw-   0        0        0     1086 2023-02-04 06:40:25.000000 Magma-Indonesia-API-2.0.0/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 09:05:04.796684 Magma-Indonesia-API-2.0.0/Magma/
+-rw-rw-rw-   0        0        0     5875 2023-06-01 08:46:19.000000 Magma-Indonesia-API-2.0.0/Magma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:05:04.806376 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/
+-rw-rw-rw-   0        0        0      706 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 09:05:04.000000 Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      706 2023-06-01 09:05:04.808390 Magma-Indonesia-API-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-02-04 06:39:44.000000 Magma-Indonesia-API-2.0.0/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:05:04.809390 Magma-Indonesia-API-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      947 2023-06-01 08:48:18.000000 Magma-Indonesia-API-2.0.0/setup.py
```

### Comparing `Magma-Indonesia-API-1.0.1/LICENSE.txt` & `Magma-Indonesia-API-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Magma-Indonesia-API-1.0.1/Magma_Indonesia_API.egg-info/PKG-INFO` & `Magma-Indonesia-API-2.0.0/Magma_Indonesia_API.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Magma-Indonesia-API
-Version: 1.0.1
+Version: 2.0.0
 Summary: Magma-Indonesia-API is an unofficial API made with Python language!
 Home-page: https://github.com/Gabrielbjb/Magma-Indonesia-API
 Author: Gabrielbjb
 Author-email: gabrielbjb@protonmail.com
 License: MIT
 Keywords: Python,Indonesia,Magma Indonesia,Volcano,Magma,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Magma-Indonesia-API-1.0.1/PKG-INFO` & `Magma-Indonesia-API-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Magma-Indonesia-API
-Version: 1.0.1
+Version: 2.0.0
 Summary: Magma-Indonesia-API is an unofficial API made with Python language!
 Home-page: https://github.com/Gabrielbjb/Magma-Indonesia-API
 Author: Gabrielbjb
 Author-email: gabrielbjb@protonmail.com
 License: MIT
 Keywords: Python,Indonesia,Magma Indonesia,Volcano,Magma,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Magma-Indonesia-API-1.0.1/setup.py` & `Magma-Indonesia-API-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
  
 setup(
     name="Magma-Indonesia-API",
-    version="1.0.1",
+    version="2.0.0",
     description="Magma-Indonesia-API is an unofficial API made with Python language!",
     long_description=readme(),
     long_description_content_type="",
     url="https://github.com/Gabrielbjb/Magma-Indonesia-API",
     author="Gabrielbjb",
     author_email="gabrielbjb@protonmail.com",
     license="MIT",
```

