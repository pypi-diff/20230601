# Comparing `tmp/ccdt-2.1.1.tar.gz` & `tmp/ccdt-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.1.tar", last modified: Thu Jun  1 09:11:49 2023, max compression
+gzip compressed data, was "ccdt-2.1.2.tar", last modified: Thu Jun  1 09:25:37 2023, max compression
```

## Comparing `ccdt-2.1.1.tar` & `ccdt-2.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:11:49.303460 ccdt-2.1.1/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     4309 2023-06-01 09:11:49.303460 ccdt-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:11:49.301466 ccdt-2.1.1/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4309 2023-06-01 09:11:49.000000 ccdt-2.1.1/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-06-01 09:11:49.000000 ccdt-2.1.1/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:11:49.000000 ccdt-2.1.1/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-01 09:11:49.000000 ccdt-2.1.1/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-06-01 09:11:49.000000 ccdt-2.1.1/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:11:49.000000 ccdt-2.1.1/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:11:49.303460 ccdt-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2336 2023-06-01 09:09:21.000000 ccdt-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:25:37.146888 ccdt-2.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4309 2023-06-01 09:25:37.145870 ccdt-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 09:25:37.143875 ccdt-2.1.2/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4309 2023-06-01 09:25:37.000000 ccdt-2.1.2/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-01 09:25:37.000000 ccdt-2.1.2/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:25:37.000000 ccdt-2.1.2/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-01 09:25:37.000000 ccdt-2.1.2/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-06-01 09:25:37.000000 ccdt-2.1.2/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:25:37.000000 ccdt-2.1.2/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:25:37.146888 ccdt-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2336 2023-06-01 09:25:07.000000 ccdt-2.1.2/setup.py
```

### Comparing `ccdt-2.1.1/LICENSE` & `ccdt-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.1/PKG-INFO` & `ccdt-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.1
+Version: 2.1.2
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.1/README.md` & `ccdt-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.1/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.2/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.1
+Version: 2.1.2
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.1/setup.py` & `ccdt-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.1',
+    version='2.1.2',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

