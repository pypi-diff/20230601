# Comparing `tmp/tello_solectric_pl-0.0.1.tar.gz` & `tmp/tello_solectric_pl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello_solectric_pl-0.0.1.tar", last modified: Sat Apr  8 09:56:25 2023, max compression
+gzip compressed data, was "tello_solectric_pl-0.0.2.tar", last modified: Thu Jun  1 12:02:37 2023, max compression
```

## Comparing `tello_solectric_pl-0.0.1.tar` & `tello_solectric_pl-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-04-08 09:56:25.419290 tello_solectric_pl-0.0.1/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3139 2023-04-08 09:56:25.415957 tello_solectric_pl-0.0.1/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.1/README.md
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       38 2023-04-08 09:56:25.419290 tello_solectric_pl-0.0.1/setup.cfg
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.1/setup.py
-drwxr-xr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-04-08 09:56:25.415957 tello_solectric_pl-0.0.1/tello_solectric_pl/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.1/tello_solectric_pl/__init__.py
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2669 2023-04-08 09:34:48.000000 tello_solectric_pl-0.0.1/tello_solectric_pl/tello_solectric_pl.py
-drwxr-xr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-04-08 09:56:25.415957 tello_solectric_pl-0.0.1/tello_solectric_pl.egg-info/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3139 2023-04-08 09:56:25.000000 tello_solectric_pl-0.0.1/tello_solectric_pl.egg-info/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-04-08 09:56:25.000000 tello_solectric_pl-0.0.1/tello_solectric_pl.egg-info/SOURCES.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-04-08 09:56:25.000000 tello_solectric_pl-0.0.1/tello_solectric_pl.egg-info/dependency_links.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-04-08 09:56:25.000000 tello_solectric_pl-0.0.1/tello_solectric_pl.egg-info/requires.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-04-08 09:56:25.000000 tello_solectric_pl-0.0.1/tello_solectric_pl.egg-info/top_level.txt
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.2/README.md
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/setup.cfg
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-06-01 11:53:26.000000 tello_solectric_pl-0.0.2/setup.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/tello_solectric_pl/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.2/tello_solectric_pl/__init__.py
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3011 2023-06-01 08:30:40.000000 tello_solectric_pl-0.0.2/tello_solectric_pl/tello_solectric_pl.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:02:37.056845 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/SOURCES.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/dependency_links.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/requires.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-01 12:02:37.000000 tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/top_level.txt
```

### Comparing `tello_solectric_pl-0.0.1/PKG-INFO` & `tello_solectric_pl-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: tello_solectric_pl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
+License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -52,7 +54,9 @@
 
 ```
 
 ---
 Zmiany w stosunku do oryginalnych metod biblioteki `djitellopy`:
 
 * metoda `connect()` zwraca wartość `True` lub `False` - i w ten sposób kontrolujemy, czy połączenie się powiodło oraz czy używamy odpowiedniego drona.
+
+
```

### Comparing `tello_solectric_pl-0.0.1/README.md` & `tello_solectric_pl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tello_solectric_pl-0.0.1/setup.py` & `tello_solectric_pl-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tello_solectric_pl",
-    version="0.0.1",
+    version="0.0.2",
     author="Adam Jurkiewicz",
     python_requires='>=3.8',
     author_email="adam@jurkiewicz.tech",
     description="Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://solectric.pl",
```

### Comparing `tello_solectric_pl-0.0.1/tello_solectric_pl/tello_solectric_pl.py` & `tello_solectric_pl-0.0.2/tello_solectric_pl/tello_solectric_pl.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         :return: "RMTT" if using the Controller on top of the RMTT, or "TELLO", if using a Tello or RMTT without
         the controller.
         :rtype:
         """
         try:
             hardware = self.send_read_command('hardware?')
-            if hardware == 'unknown command: hardware?':
+            if hardware in ('ok', 'unknown command: hardware?'):
                 hardware = "TelloEDU"
         except Exception as exc:
             hardware = "TelloEDU"
 
         return hardware
 
     def get_speed(self) -> int:
@@ -46,41 +46,47 @@
         return speed_value
 
 
 class TelloEDU(TelloMain):
     """
 
     Klasa przeznaczona dla dronów Tello-EDU (czarny)
-    W metodzie D.connect() sprawdza, czy to taki dron
+    W metodzie D.connect() sprawdza, czy to taki dron, czy poziom naładowania baterii jest wystarczający
     """
     hardware_type = "TelloEDU"
+    min_battery_level = 25
 
     def __init__(self, info_all=False):
         """
 
         :param info_all: Czy ysyłać wszystkie informacje na ekran, True lub False (default)
         """
         super().__init__(info_all=info_all)
 
     def connect(self, wait_for_state=True) -> bool:
         connection_success = False
         hardware_ok = False
         hardware_probe = "xxxx"
 
+
         try:
             super().connect(wait_for_state=wait_for_state)
             connection_success = True
         except Exception as e:
             print(f"Błąd przy wywołaniu CONNECT: {e}")
             return False
 
         hardware_probe = self.query_hardware()
         if self.hardware_type == hardware_probe:
             hardware_ok = True
             print(f"Połączono z dronem typu {self.hardware_type}")
+            battery_level = self.get_battery()
+            if battery_level < self.min_battery_level:
+                print(f"Poziom baterii zbyt niski ({battery_level} %) - wymagane minimum to {self.min_battery_level} %.")
+                return False
         else:
             print(f"Otrzymano: {repr(hardware_probe)} -> nie pasuje do {self.hardware_type}")
 
         return connection_success and hardware_ok
 
 
 class RyzenTT(TelloMain):
```

### Comparing `tello_solectric_pl-0.0.1/tello_solectric_pl.egg-info/PKG-INFO` & `tello_solectric_pl-0.0.2/tello_solectric_pl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: tello-solectric-pl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
+License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -52,7 +54,9 @@
 
 ```
 
 ---
 Zmiany w stosunku do oryginalnych metod biblioteki `djitellopy`:
 
 * metoda `connect()` zwraca wartość `True` lub `False` - i w ten sposób kontrolujemy, czy połączenie się powiodło oraz czy używamy odpowiedniego drona.
+
+
```

