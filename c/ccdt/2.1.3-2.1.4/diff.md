# Comparing `tmp/ccdt-2.1.3.tar.gz` & `tmp/ccdt-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.3.tar", last modified: Thu Jun  1 09:40:39 2023, max compression
+gzip compressed data, was "ccdt-2.1.4.tar", last modified: Thu Jun  1 09:49:56 2023, max compression
```

## Comparing `ccdt-2.1.3.tar` & `ccdt-2.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.838509 ccdt-2.1.3/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.3/LICENSE
--rw-rw-rw-   0        0        0     4309 2023-06-01 09:40:39.837538 ccdt-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.716133 ccdt-2.1.3/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.3/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.752278 ccdt-2.1.3/ccdt/dataset/
--rw-rw-rw-   0        0        0      216 2023-05-17 01:52:32.000000 ccdt-2.1.3/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.766241 ccdt-2.1.3/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.3/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22572 2023-05-25 05:57:25.000000 ccdt-2.1.3/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.797223 ccdt-2.1.3/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.3/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7401 2023-05-25 01:56:24.000000 ccdt-2.1.3/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    63498 2023-05-25 02:57:06.000000 ccdt-2.1.3/ccdt/dataset/base_labelme/base_labelme.py
--rw-rw-rw-   0        0        0    14420 2023-05-25 03:24:49.000000 ccdt-2.1.3/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.808845 ccdt-2.1.3/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-05-17 01:56:42.000000 ccdt-2.1.3/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.3/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    17029 2023-05-25 06:27:22.000000 ccdt-2.1.3/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.824229 ccdt-2.1.3/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.3/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-05-25 06:23:23.000000 ccdt-2.1.3/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4845 2023-05-25 06:30:32.000000 ccdt-2.1.3/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:40:39.727105 ccdt-2.1.3/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4309 2023-06-01 09:40:39.000000 ccdt-2.1.3/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-06-01 09:40:39.000000 ccdt-2.1.3/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:40:39.000000 ccdt-2.1.3/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-01 09:40:39.000000 ccdt-2.1.3/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-06-01 09:40:39.000000 ccdt-2.1.3/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-01 09:40:39.000000 ccdt-2.1.3/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:40:39.838509 ccdt-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2336 2023-06-01 09:39:39.000000 ccdt-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.356750 ccdt-2.1.4/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4309 2023-06-01 09:49:56.355753 ccdt-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.322820 ccdt-2.1.4/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.4/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.335785 ccdt-2.1.4/ccdt/dataset/
+-rw-rw-rw-   0        0        0      216 2023-05-17 01:52:32.000000 ccdt-2.1.4/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.338778 ccdt-2.1.4/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.4/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22572 2023-05-25 05:57:25.000000 ccdt-2.1.4/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.343789 ccdt-2.1.4/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.4/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7401 2023-05-25 01:56:24.000000 ccdt-2.1.4/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    63498 2023-05-25 02:57:06.000000 ccdt-2.1.4/ccdt/dataset/base_labelme/base_labelme.py
+-rw-rw-rw-   0        0        0    14420 2023-05-25 03:24:49.000000 ccdt-2.1.4/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.348771 ccdt-2.1.4/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-05-17 01:56:42.000000 ccdt-2.1.4/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.4/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    17029 2023-05-25 06:27:22.000000 ccdt-2.1.4/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.353738 ccdt-2.1.4/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.4/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-25 06:23:23.000000 ccdt-2.1.4/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4845 2023-05-25 06:30:32.000000 ccdt-2.1.4/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:49:56.332794 ccdt-2.1.4/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4309 2023-06-01 09:49:56.000000 ccdt-2.1.4/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-06-01 09:49:56.000000 ccdt-2.1.4/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:49:56.000000 ccdt-2.1.4/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-01 09:49:56.000000 ccdt-2.1.4/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2023-06-01 09:49:56.000000 ccdt-2.1.4/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-01 09:49:56.000000 ccdt-2.1.4/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:49:56.357728 ccdt-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2344 2023-06-01 09:48:54.000000 ccdt-2.1.4/setup.py
```

### Comparing `ccdt-2.1.3/LICENSE` & `ccdt-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/PKG-INFO` & `ccdt-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.3
+Version: 2.1.4
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.3/README.md` & `ccdt-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.4/ccdt/dataset/base_coco/base_coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.4/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.4/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/dataset/main.py` & `ccdt-2.1.4/ccdt/dataset/main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.4/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.4/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/video_tool/split.py` & `ccdt-2.1.4/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt/video_tool/video_main.py` & `ccdt-2.1.4/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.4/ccdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.3
+Version: 2.1.4
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.3/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.4/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.3/setup.py` & `ccdt-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 def get_install_requires():
     install_requires = [
-        'tqdm',
+        'tqdm==4.65.0',
         'opencv_python',  # for PyInstaller
         'numpy',
         'pycocotools',
         'prettytable',
         'shapely',
         'psutil',
         'pypinyin',
@@ -23,15 +23,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.3',
+    version='2.1.4',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

