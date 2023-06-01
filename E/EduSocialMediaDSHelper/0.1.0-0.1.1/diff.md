# Comparing `tmp/EduSocialMediaDSHelper-0.1.0.tar.gz` & `tmp/EduSocialMediaDSHelper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EduSocialMediaDSHelper-0.1.0.tar", last modified: Thu Jun  1 00:47:45 2023, max compression
+gzip compressed data, was "dist\EduSocialMediaDSHelper-0.1.1.tar", last modified: Thu Jun  1 01:16:25 2023, max compression
```

## Comparing `EduSocialMediaDSHelper-0.1.0.tar` & `EduSocialMediaDSHelper-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/
--rw-rw-rw-   0        0        0        0 2023-01-02 21:56:20.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/__init__.py
--rw-rw-rw-   0        0        0      622 2023-03-06 00:34:43.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_cars_dataset.py
--rw-rw-rw-   0        0        0     3578 2023-03-03 19:31:04.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_sphinx_data.py
--rw-rw-rw-   0        0        0     1862 2023-03-15 18:31:49.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_twitter_dataset.py
--rw-rw-rw-   0        0        0     1340 2023-03-05 20:44:32.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_uci_census_data.py
--rw-rw-rw-   0        0        0     1075 2023-03-09 02:12:23.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_video_games_dataset.py
--rw-rw-rw-   0        0        0     2632 2023-03-19 23:46:27.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/element_answer_checks.py
--rw-rw-rw-   0        0        0     3068 2023-03-19 23:46:31.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/list_answer_checks.py
--rw-rw-rw-   0        0        0      327 2023-06-01 00:42:56.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/load_legos.py
--rw-rw-rw-   0        0        0     6333 2023-06-01 00:27:35.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/misc_helpers.py
--rw-rw-rw-   0        0        0    11673 2023-03-19 23:45:54.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/recommender_support.py
-drwxrwxrwx   0        0        0        0 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper.egg-info/
--rw-rw-rw-   0        0        0      569 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-01-02 22:05:40.000000 EduSocialMediaDSHelper-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0       54 2023-06-01 00:25:52.000000 EduSocialMediaDSHelper-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      569 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-01-02 20:27:04.000000 EduSocialMediaDSHelper-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 00:47:45.000000 EduSocialMediaDSHelper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      772 2023-06-01 00:26:45.000000 EduSocialMediaDSHelper-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/
+-rw-rw-rw-   0        0        0        0 2023-01-02 21:56:20.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-03-06 00:34:43.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_cars_dataset.py
+-rw-rw-rw-   0        0        0     3578 2023-03-03 19:31:04.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_sphinx_data.py
+-rw-rw-rw-   0        0        0     1862 2023-03-15 18:31:49.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_twitter_dataset.py
+-rw-rw-rw-   0        0        0     1340 2023-03-05 20:44:32.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_uci_census_data.py
+-rw-rw-rw-   0        0        0     1075 2023-03-09 02:12:23.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_video_games_dataset.py
+-rw-rw-rw-   0        0        0     2632 2023-03-19 23:46:27.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/element_answer_checks.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/legos/
+-rw-rw-rw-   0        0        0     3836 2023-06-01 00:22:11.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/legos/color_counts.csv
+-rw-rw-rw-   0        0        0   507514 2019-09-20 23:25:20.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/legos/sets.csv
+-rw-rw-rw-   0        0        0     3068 2023-03-19 23:46:31.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/list_answer_checks.py
+-rw-rw-rw-   0        0        0      700 2023-06-01 01:15:32.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/load_legos.py
+-rw-rw-rw-   0        0        0     6333 2023-06-01 00:27:35.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/misc_helpers.py
+-rw-rw-rw-   0        0        0    11673 2023-03-19 23:45:54.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/recommender_support.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-01-02 22:05:40.000000 EduSocialMediaDSHelper-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      100 2023-06-01 01:10:57.000000 EduSocialMediaDSHelper-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      569 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2023-01-02 20:27:04.000000 EduSocialMediaDSHelper-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 01:16:25.000000 EduSocialMediaDSHelper-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      772 2023-06-01 01:11:13.000000 EduSocialMediaDSHelper-0.1.1/setup.py
```

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_cars_dataset.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_cars_dataset.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_sphinx_data.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_sphinx_data.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_twitter_dataset.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_twitter_dataset.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_uci_census_data.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_uci_census_data.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/create_video_games_dataset.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/create_video_games_dataset.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/element_answer_checks.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/element_answer_checks.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/list_answer_checks.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/list_answer_checks.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/misc_helpers.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/misc_helpers.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper/recommender_support.py` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper/recommender_support.py`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper.egg-info/PKG-INFO` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduSocialMediaDSHelper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Helper for DS Social Media learning material
 Home-page: https://github.com/Joshkking/EduSocialMediaDSHelper
 Author: Josh King
 Author-email: joshkking@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EduSocialMediaDSHelper-0.1.0/EduSocialMediaDSHelper.egg-info/SOURCES.txt` & `EduSocialMediaDSHelper-0.1.1/EduSocialMediaDSHelper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 EduSocialMediaDSHelper/list_answer_checks.py
 EduSocialMediaDSHelper/load_legos.py
 EduSocialMediaDSHelper/misc_helpers.py
 EduSocialMediaDSHelper/recommender_support.py
 EduSocialMediaDSHelper.egg-info/PKG-INFO
 EduSocialMediaDSHelper.egg-info/SOURCES.txt
 EduSocialMediaDSHelper.egg-info/dependency_links.txt
-EduSocialMediaDSHelper.egg-info/top_level.txt
+EduSocialMediaDSHelper.egg-info/top_level.txt
+EduSocialMediaDSHelper/legos/color_counts.csv
+EduSocialMediaDSHelper/legos/sets.csv
```

### Comparing `EduSocialMediaDSHelper-0.1.0/LICENSE.md` & `EduSocialMediaDSHelper-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EduSocialMediaDSHelper-0.1.0/PKG-INFO` & `EduSocialMediaDSHelper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduSocialMediaDSHelper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Helper for DS Social Media learning material
 Home-page: https://github.com/Joshkking/EduSocialMediaDSHelper
 Author: Josh King
 Author-email: joshkking@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EduSocialMediaDSHelper-0.1.0/setup.py` & `EduSocialMediaDSHelper-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="EduSocialMediaDSHelper", # Replace with your own username
-    version="0.1.0",
+    version="0.1.1",
     author="Josh King",
     author_email="joshkking@gmail.com",
     description="Helper for DS Social Media learning material",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Joshkking/EduSocialMediaDSHelper",
     packages=setuptools.find_packages(),
```

