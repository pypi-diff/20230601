# Comparing `tmp/MS_visualizer_lite-0.0.1.tar.gz` & `tmp/MS_visualizer_lite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MS_visualizer_lite-0.0.1.tar", last modified: Wed May 31 22:03:02 2023, max compression
+gzip compressed data, was "MS_visualizer_lite-0.0.2.tar", last modified: Wed May 31 22:05:06 2023, max compression
```

## Comparing `MS_visualizer_lite-0.0.1.tar` & `MS_visualizer_lite-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.683963 MS_visualizer_lite-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.633869 MS_visualizer_lite-0.0.1/MS_visualizer_lite/
--rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.662140 MS_visualizer_lite-0.0.1/MS_visualizer_lite/assets/
--rw-rw-rw-   0        0        0        0 2023-05-30 11:21:18.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/assets/__init__.py
--rw-rw-rw-   0        0        0     2553 2022-03-31 11:56:33.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/assets/plotly_colors.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.664620 MS_visualizer_lite-0.0.1/MS_visualizer_lite/components/
--rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/components/__init__.py
--rw-rw-rw-   0        0        0     5619 2023-05-31 21:53:33.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/components/components.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.667596 MS_visualizer_lite-0.0.1/MS_visualizer_lite/controller/
--rw-rw-rw-   0        0        0        0 2022-03-31 11:56:33.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/controller/__init__.py
--rw-rw-rw-   0        0        0     3027 2023-05-31 21:47:28.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/controller/func.py
--rw-rw-rw-   0        0        0      679 2023-05-31 21:12:43.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/server.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.670571 MS_visualizer_lite-0.0.1/MS_visualizer_lite/utils/
--rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/utils/__init__.py
--rw-rw-rw-   0        0        0      226 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/utils/toml.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.675035 MS_visualizer_lite-0.0.1/MS_visualizer_lite/view/
--rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/view/__init__.py
--rw-rw-rw-   0        0        0       68 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/view/home.py
--rw-rw-rw-   0        0        0    18399 2023-05-31 21:49:12.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite/view/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.658668 MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/
--rw-rw-rw-   0        0        0      615 2023-05-31 22:03:02.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      855 2023-05-31 22:03:02.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:03:02.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-31 22:03:02.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      122 2023-05-31 22:03:02.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-31 22:03:02.000000 MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      615 2023-05-31 22:03:02.684459 MS_visualizer_lite-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       18 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.678011 MS_visualizer_lite-0.0.1/bin/
--rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.1/bin/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-05-31 21:50:19.000000 MS_visualizer_lite-0.0.1/bin/run.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:02.682475 MS_visualizer_lite-0.0.1/examples/
--rw-rw-rw-   0        0        0        0 2022-03-31 11:56:33.000000 MS_visualizer_lite-0.0.1/examples/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-31 21:12:43.000000 MS_visualizer_lite-0.0.1/examples/forthilo.py
--rw-rw-rw-   0        0        0     4922 2023-05-31 21:15:44.000000 MS_visualizer_lite-0.0.1/examples/get_data.py
--rw-rw-rw-   0        0        0       86 2023-05-31 22:03:02.688426 MS_visualizer_lite-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1279 2023-05-31 22:02:12.000000 MS_visualizer_lite-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.248616 MS_visualizer_lite-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.201992 MS_visualizer_lite-0.0.2/MS_visualizer_lite/
+-rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.228279 MS_visualizer_lite-0.0.2/MS_visualizer_lite/assets/
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:21:18.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/assets/__init__.py
+-rw-rw-rw-   0        0        0     2553 2022-03-31 11:56:33.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/assets/plotly_colors.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.231256 MS_visualizer_lite-0.0.2/MS_visualizer_lite/components/
+-rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/components/__init__.py
+-rw-rw-rw-   0        0        0     5619 2023-05-31 21:53:33.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/components/components.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.233734 MS_visualizer_lite-0.0.2/MS_visualizer_lite/controller/
+-rw-rw-rw-   0        0        0        0 2022-03-31 11:56:33.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/controller/__init__.py
+-rw-rw-rw-   0        0        0     3027 2023-05-31 21:47:28.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/controller/func.py
+-rw-rw-rw-   0        0        0      679 2023-05-31 21:12:43.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.236215 MS_visualizer_lite-0.0.2/MS_visualizer_lite/utils/
+-rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/utils/__init__.py
+-rw-rw-rw-   0        0        0      226 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/utils/toml.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.240183 MS_visualizer_lite-0.0.2/MS_visualizer_lite/view/
+-rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/view/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/view/home.py
+-rw-rw-rw-   0        0        0    18336 2023-05-31 22:04:52.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite/view/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.225303 MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-05-31 22:05:06.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      855 2023-05-31 22:05:06.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:05:06.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-31 22:05:06.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      122 2023-05-31 22:05:06.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-31 22:05:06.000000 MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      615 2023-05-31 22:05:06.248616 MS_visualizer_lite-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.243159 MS_visualizer_lite-0.0.2/bin/
+-rw-rw-rw-   0        0        0        0 2022-02-22 09:22:04.000000 MS_visualizer_lite-0.0.2/bin/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-05-31 21:50:19.000000 MS_visualizer_lite-0.0.2/bin/run.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:05:06.247128 MS_visualizer_lite-0.0.2/examples/
+-rw-rw-rw-   0        0        0        0 2022-03-31 11:56:33.000000 MS_visualizer_lite-0.0.2/examples/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-31 21:12:43.000000 MS_visualizer_lite-0.0.2/examples/forthilo.py
+-rw-rw-rw-   0        0        0     4922 2023-05-31 21:15:44.000000 MS_visualizer_lite-0.0.2/examples/get_data.py
+-rw-rw-rw-   0        0        0       86 2023-05-31 22:05:06.253080 MS_visualizer_lite-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1279 2023-05-31 22:05:00.000000 MS_visualizer_lite-0.0.2/setup.py
```

### Comparing `MS_visualizer_lite-0.0.1/MS_visualizer_lite/assets/plotly_colors.py` & `MS_visualizer_lite-0.0.2/MS_visualizer_lite/assets/plotly_colors.py`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/MS_visualizer_lite/components/components.py` & `MS_visualizer_lite-0.0.2/MS_visualizer_lite/components/components.py`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/MS_visualizer_lite/controller/func.py` & `MS_visualizer_lite-0.0.2/MS_visualizer_lite/controller/func.py`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/MS_visualizer_lite/server.py` & `MS_visualizer_lite-0.0.2/MS_visualizer_lite/server.py`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/MS_visualizer_lite/view/visualizer.py` & `MS_visualizer_lite-0.0.2/MS_visualizer_lite/view/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,16 @@
 TRANSFORMED_MZ_MAX = 200
 SCAN_MIN = 1
 SCAN_MAX = 450
 INV_ION_M_MIN = 0.6
 INV_ION_M_MAX = 1.5
 MIN_INTENSITY = 10
 
-DEFAULT_PATH = "data/data.d"
-BASE_PATH = "data/"
-
-# DEFAULT_PATH = "/data/rawdata/gutamine/G2112/G211202_004_Slot1-1_1_3342.d"
-# BASE_PATH = "/data/rawdata/gutamine/"
+DEFAULT_PATH = "/data/rawdata/gutamine/G2112/G211202_004_Slot1-1_1_3342.d"
+BASE_PATH = "/data/rawdata/"
 
 
 # Layout
 visualizer = html.Div([
 
     # store if the graph shows the raw or clustered data
     dcc.Store(id="last_button_id"),
```

### Comparing `MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/PKG-INFO` & `MS_visualizer_lite-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MS-visualizer-lite
-Version: 0.0.1
+Name: MS_visualizer_lite
+Version: 0.0.2
 Summary: Description.
 Home-page: https://github.com/MatteoLacki/MS_visualizer2.git
 Author: ['ThiloSchild', 'David Teschner', 'MatteoLacki']
 Author-email: matteo.lacki@gmail.com
 Keywords: Great module,Devel Inside
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `MS_visualizer_lite-0.0.1/MS_visualizer_lite.egg-info/SOURCES.txt` & `MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/PKG-INFO` & `MS_visualizer_lite-0.0.2/MS_visualizer_lite.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MS_visualizer_lite
-Version: 0.0.1
+Name: MS-visualizer-lite
+Version: 0.0.2
 Summary: Description.
 Home-page: https://github.com/MatteoLacki/MS_visualizer2.git
 Author: ['ThiloSchild', 'David Teschner', 'MatteoLacki']
 Author-email: matteo.lacki@gmail.com
 Keywords: Great module,Devel Inside
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `MS_visualizer_lite-0.0.1/bin/run.py` & `MS_visualizer_lite-0.0.2/bin/run.py`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/examples/forthilo.py` & `MS_visualizer_lite-0.0.2/examples/forthilo.py`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/examples/get_data.py` & `MS_visualizer_lite-0.0.2/examples/get_data.py`

 * *Files identical despite different names*

### Comparing `MS_visualizer_lite-0.0.1/setup.py` & `MS_visualizer_lite-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This Python file uses the following encoding: utf-8
 from setuptools import setup, find_packages
 
 setup(name='MS_visualizer_lite',
       packages=find_packages(),
-      version='0.0.1',
+      version='0.0.2',
       description='Description.',
       long_description='Long description.',
       author=['ThiloSchild', 'David Teschner', 'MatteoLacki'],
       author_email='matteo.lacki@gmail.com',
       url='https://github.com/MatteoLacki/MS_visualizer2.git',
       keywords=['Great module', 'Devel Inside'],
       classifiers=['Development Status :: 1 - Planning',
```

