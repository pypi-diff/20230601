# Comparing `tmp/ehzahumming-0.1.tar.gz` & `tmp/ehzahumming-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehzahumming-0.1.tar", last modified: Thu Jun  1 09:02:14 2023, max compression
+gzip compressed data, was "ehzahumming-0.2.tar", last modified: Thu Jun  1 10:54:44 2023, max compression
```

## Comparing `ehzahumming-0.1.tar` & `ehzahumming-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 09:02:14.242097 ehzahumming-0.1/
--rw-rw-r--   0 ehz       (1000) ehz       (1000)      661 2023-06-01 09:02:14.242097 ehzahumming-0.1/PKG-INFO
--rw-rw-r--   0 ehz       (1000) ehz       (1000)       62 2023-06-01 09:02:06.000000 ehzahumming-0.1/README.md
-drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 09:02:14.242097 ehzahumming-0.1/ehzahumming/
--rw-rw-r--   0 ehz       (1000) ehz       (1000)       34 2023-06-01 09:02:06.000000 ehzahumming-0.1/ehzahumming/__init__.py
--rw-rw-r--   0 ehz       (1000) ehz       (1000)      124 2023-06-01 09:02:06.000000 ehzahumming-0.1/ehzahumming/humming.py
-drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 09:02:14.242097 ehzahumming-0.1/ehzahumming.egg-info/
--rw-rw-r--   0 ehz       (1000) ehz       (1000)      661 2023-06-01 09:02:14.000000 ehzahumming-0.1/ehzahumming.egg-info/PKG-INFO
--rw-rw-r--   0 ehz       (1000) ehz       (1000)      242 2023-06-01 09:02:14.000000 ehzahumming-0.1/ehzahumming.egg-info/SOURCES.txt
--rw-rw-r--   0 ehz       (1000) ehz       (1000)        1 2023-06-01 09:02:14.000000 ehzahumming-0.1/ehzahumming.egg-info/dependency_links.txt
--rw-rw-r--   0 ehz       (1000) ehz       (1000)       12 2023-06-01 09:02:14.000000 ehzahumming-0.1/ehzahumming.egg-info/top_level.txt
--rw-rw-r--   0 ehz       (1000) ehz       (1000)       90 2023-06-01 09:02:06.000000 ehzahumming-0.1/pyproject.toml
--rw-rw-r--   0 ehz       (1000) ehz       (1000)       38 2023-06-01 09:02:14.242097 ehzahumming-0.1/setup.cfg
--rw-rw-r--   0 ehz       (1000) ehz       (1000)      770 2023-06-01 09:02:06.000000 ehzahumming-0.1/setup.py
-drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 09:02:14.242097 ehzahumming-0.1/tests/
--rw-rw-r--   0 ehz       (1000) ehz       (1000)      121 2023-06-01 09:02:06.000000 ehzahumming-0.1/tests/test_humming.py
+drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 10:54:44.296465 ehzahumming-0.2/
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)      649 2023-06-01 10:54:44.296465 ehzahumming-0.2/PKG-INFO
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)       62 2023-06-01 09:02:06.000000 ehzahumming-0.2/README.md
+drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 10:54:44.296465 ehzahumming-0.2/ehzahumming/
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)       34 2023-06-01 09:02:06.000000 ehzahumming-0.2/ehzahumming/__init__.py
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)      124 2023-06-01 09:02:06.000000 ehzahumming-0.2/ehzahumming/humming.py
+drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 10:54:44.296465 ehzahumming-0.2/ehzahumming.egg-info/
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)      649 2023-06-01 10:54:44.000000 ehzahumming-0.2/ehzahumming.egg-info/PKG-INFO
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)      242 2023-06-01 10:54:44.000000 ehzahumming-0.2/ehzahumming.egg-info/SOURCES.txt
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)        1 2023-06-01 10:54:44.000000 ehzahumming-0.2/ehzahumming.egg-info/dependency_links.txt
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)       12 2023-06-01 10:54:44.000000 ehzahumming-0.2/ehzahumming.egg-info/top_level.txt
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)       90 2023-06-01 09:02:06.000000 ehzahumming-0.2/pyproject.toml
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)       38 2023-06-01 10:54:44.296465 ehzahumming-0.2/setup.cfg
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)      758 2023-06-01 10:53:47.000000 ehzahumming-0.2/setup.py
+drwxrwxr-x   0 ehz       (1000) ehz       (1000)        0 2023-06-01 10:54:44.296465 ehzahumming-0.2/tests/
+-rw-rw-r--   0 ehz       (1000) ehz       (1000)      121 2023-06-01 09:02:06.000000 ehzahumming-0.2/tests/test_humming.py
```

### Comparing `ehzahumming-0.1/PKG-INFO` & `ehzahumming-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ehzahumming
-Version: 0.1
+Version: 0.2
 Summary: A simple utility to generate humming sounds
-Home-page: https://github.com/yourusername/ehzahumming
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/ehzawad/ehzahumming
+Author: ehzawad
+Author-email: ehzawad@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ehzahumming-0.1/ehzahumming.egg-info/PKG-INFO` & `ehzahumming-0.2/ehzahumming.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ehzahumming
-Version: 0.1
+Version: 0.2
 Summary: A simple utility to generate humming sounds
-Home-page: https://github.com/yourusername/ehzahumming
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/ehzawad/ehzahumming
+Author: ehzawad
+Author-email: ehzawad@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ehzahumming-0.1/setup.py` & `ehzahumming-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ehzahumming",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     description="A simple utility to generate humming sounds",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    author="Your Name",
-    author_email="your.email@example.com",
-    url="https://github.com/yourusername/ehzahumming",
+    author="ehzawad",
+    author_email="ehzawad@gmail.com",
+    url="https://github.com/ehzawad/ehzahumming",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

