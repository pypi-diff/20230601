# Comparing `tmp/minidevice-1.0.1.tar.gz` & `tmp/minidevice-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.1.tar", last modified: Thu Jun  1 01:41:03 2023, max compression
+gzip compressed data, was "minidevice-1.0.2.tar", last modified: Thu Jun  1 03:24:43 2023, max compression
```

## Comparing `minidevice-1.0.1.tar` & `minidevice-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 01:41:03.344519 minidevice-1.0.1/
--rw-rw-rw-   0        0        0     1205 2023-06-01 01:41:03.343521 minidevice-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-06-01 01:33:14.000000 minidevice-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 01:41:03.333548 minidevice-1.0.1/minidevice/
--rw-rw-rw-   0        0        0       29 2023-05-31 10:12:15.000000 minidevice-1.0.1/minidevice/__init__.py
--rw-rw-rw-   0        0        0     2040 2023-06-01 01:14:31.000000 minidevice-1.0.1/minidevice/adb.py
--rw-rw-rw-   0        0        0      269 2023-05-31 10:26:49.000000 minidevice-1.0.1/minidevice/config.py
--rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.1/minidevice/device.py
--rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.1/minidevice/minicap.py
--rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.1/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.1/minidevice/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:41:03.342524 minidevice-1.0.1/minidevice.egg-info/
--rw-rw-rw-   0        0        0     1205 2023-06-01 01:41:02.000000 minidevice-1.0.1/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-06-01 01:41:03.000000 minidevice-1.0.1/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 01:41:02.000000 minidevice-1.0.1/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-01 01:41:03.000000 minidevice-1.0.1/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 01:41:03.000000 minidevice-1.0.1/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 01:41:03.344519 minidevice-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      644 2023-06-01 01:40:04.000000 minidevice-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:24:43.873790 minidevice-1.0.2/
+-rw-rw-rw-   0        0        0     1205 2023-06-01 03:24:43.872809 minidevice-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-06-01 01:33:14.000000 minidevice-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 03:24:43.842845 minidevice-1.0.2/minidevice/
+-rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.2/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     2040 2023-06-01 01:14:31.000000 minidevice-1.0.2/minidevice/adb.py
+-rw-rw-rw-   0        0        0      269 2023-05-31 10:26:49.000000 minidevice-1.0.2/minidevice/config.py
+-rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.2/minidevice/device.py
+-rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.2/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.2/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.2/minidevice/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:24:43.871810 minidevice-1.0.2/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1205 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 03:24:43.873790 minidevice-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-06-01 03:24:08.000000 minidevice-1.0.2/setup.py
```

### Comparing `minidevice-1.0.1/PKG-INFO` & `minidevice-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.1
+Version: 1.0.2
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
```

### Comparing `minidevice-1.0.1/README.md` & `minidevice-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.1/minidevice/adb.py` & `minidevice-1.0.2/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.1/minidevice/device.py` & `minidevice-1.0.2/minidevice/device.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.1/minidevice/minicap.py` & `minidevice-1.0.2/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.1/minidevice.egg-info/PKG-INFO` & `minidevice-1.0.2/minidevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.1
+Version: 1.0.2
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
```

### Comparing `minidevice-1.0.1/setup.py` & `minidevice-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.0.1',
+      version='1.0.2',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku',
       license='MIT',
       keywords='game',
       project_urls={},
       packages=['minidevice'],
-      install_requires=['opencv-python>=4.7.0.72', 'uiautomator2>=2.16.23'],
+      install_requires=['opencv-python>=4.7.0.72', 'uiautomator2>=2.16.23','pyminitouch>=0.3.3'],
       python_requires='>=3'
      )
```

