# Comparing `tmp/tello_solectric_pl-0.0.2.tar.gz` & `tmp/tello_solectric_pl-0.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello_solectric_pl-0.0.2.tar", last modified: Thu Jun  1 12:02:37 2023, max compression
+gzip compressed data, was "tello_solectric_pl-0.0.2b0.tar", last modified: Thu Jun  1 12:05:27 2023, max compression
```

## Comparing `tello_solectric_pl-0.0.2.tar` & `tello_solectric_pl-0.0.2b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.2/README.md
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/setup.cfg
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-06-01 11:53:26.000000 tello_solectric_pl-0.0.2/setup.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/tello_solectric_pl/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.2/tello_solectric_pl/__init__.py
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3011 2023-06-01 08:30:40.000000 tello_solectric_pl-0.0.2/tello_solectric_pl/tello_solectric_pl.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/SOURCES.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/dependency_links.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/requires.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/top_level.txt
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3178 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.2b0/README.md
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/setup.cfg
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      891 2023-06-01 12:05:16.000000 tello_solectric_pl-0.0.2b0/setup.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/tello_solectric_pl/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl/__init__.py
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3044 2023-06-01 12:05:06.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl/tello_solectric_pl.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3178 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/SOURCES.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/dependency_links.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/requires.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/top_level.txt
```

### Comparing `tello_solectric_pl-0.0.2/PKG-INFO` & `tello_solectric_pl-0.0.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello_solectric_pl
-Version: 0.0.2
+Version: 0.0.2b0
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

### Comparing `tello_solectric_pl-0.0.2/README.md` & `tello_solectric_pl-0.0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `tello_solectric_pl-0.0.2/setup.py` & `tello_solectric_pl-0.0.2b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tello_solectric_pl",
-    version="0.0.2",
+    version="0.0.2b",
     author="Adam Jurkiewicz",
     python_requires='>=3.8',
     author_email="adam@jurkiewicz.tech",
     description="Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://solectric.pl",
```

### Comparing `tello_solectric_pl-0.0.2/tello_solectric_pl/tello_solectric_pl.py` & `tello_solectric_pl-0.0.2b0/tello_solectric_pl/tello_solectric_pl.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,16 +76,17 @@
             return False
 
         hardware_probe = self.query_hardware()
         if self.hardware_type == hardware_probe:
             hardware_ok = True
             print(f"Połączono z dronem typu {self.hardware_type}")
             battery_level = self.get_battery()
+	    print(f"Poziom baterii == ({battery_level} %)")
             if battery_level < self.min_battery_level:
-                print(f"Poziom baterii zbyt niski ({battery_level} %) - wymagane minimum to {self.min_battery_level} %.")
+                print(f"Poziom baterii zbyt niski - wymagane minimum to {self.min_battery_level} %.")
                 return False
         else:
             print(f"Otrzymano: {repr(hardware_probe)} -> nie pasuje do {self.hardware_type}")
 
         return connection_success and hardware_ok
```

### Comparing `tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/PKG-INFO` & `tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello-solectric-pl
-Version: 0.0.2
+Version: 0.0.2b0
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

