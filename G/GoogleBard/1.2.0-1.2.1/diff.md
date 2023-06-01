# Comparing `tmp/GoogleBard-1.2.0.tar.gz` & `tmp/GoogleBard-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.2.0.tar", last modified: Sun May 28 12:52:56 2023, max compression
+gzip compressed data, was "GoogleBard-1.2.1.tar", last modified: Thu Jun  1 04:34:53 2023, max compression
```

## Comparing `GoogleBard-1.2.0.tar` & `GoogleBard-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-28 12:52:31.000000 GoogleBard-1.2.0/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:56.610354 GoogleBard-1.2.0/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 12:52:56.000000 GoogleBard-1.2.0/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:34:53.831040 GoogleBard-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 04:34:53.827041 GoogleBard-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 04:34:53.831040 GoogleBard-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:34:53.827041 GoogleBard-1.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:34:53.827041 GoogleBard-1.2.1/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.2.0/LICENSE` & `GoogleBard-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.2.0/PKG-INFO` & `GoogleBard-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.2.0
+Version: 1.2.1
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.2.0/README.md` & `GoogleBard-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.2.0/setup.py` & `GoogleBard-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.2.0",
+    version="1.2.1",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.2.0/src/Bard.py` & `GoogleBard-1.2.1/src/Bard.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
         # url params
         params = {
-            "bl": "boq_assistant-bard-web-server_20230523.13_p0",
+            "bl": "boq_assistant-bard-web-server_20230530.14_p0",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
 
         # message arr -> data["f.req"]. Message is double json stringified
         message_struct = [
             [message],
```

### Comparing `GoogleBard-1.2.0/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.2.1/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.2.0
+Version: 1.2.1
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

