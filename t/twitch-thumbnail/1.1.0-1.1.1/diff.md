# Comparing `tmp/twitch-thumbnail-1.1.0.tar.gz` & `tmp/twitch-thumbnail-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-thumbnail-1.1.0.tar", last modified: Wed Jan 11 15:39:36 2023, max compression
+gzip compressed data, was "twitch-thumbnail-1.1.1.tar", last modified: Thu Jun  1 06:39:41 2023, max compression
```

## Comparing `twitch-thumbnail-1.1.0.tar` & `twitch-thumbnail-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 15:39:36.334658 twitch-thumbnail-1.1.0/
--rw-rw-rw-   0        0        0     1067 2023-01-11 15:39:36.333660 twitch-thumbnail-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      782 2023-01-11 15:39:14.000000 twitch-thumbnail-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-01-11 15:39:36.334658 twitch-thumbnail-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-01-11 15:39:24.000000 twitch-thumbnail-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:39:36.314658 twitch-thumbnail-1.1.0/twitch_thumbnail/
--rw-rw-rw-   0        0        0      325 2023-01-09 17:08:12.000000 twitch-thumbnail-1.1.0/twitch_thumbnail/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-01-11 15:30:41.000000 twitch-thumbnail-1.1.0/twitch_thumbnail/asynchronous.py
--rw-rw-rw-   0        0        0      429 2023-01-11 15:35:19.000000 twitch-thumbnail-1.1.0/twitch_thumbnail/exceptions.py
--rw-rw-rw-   0        0        0      333 2023-01-09 17:11:26.000000 twitch-thumbnail-1.1.0/twitch_thumbnail/ffmpeg.py
--rw-rw-rw-   0        0        0     1942 2023-01-11 15:35:31.000000 twitch-thumbnail-1.1.0/twitch_thumbnail/streamlink.py
--rw-rw-rw-   0        0        0     1325 2023-01-11 15:30:52.000000 twitch-thumbnail-1.1.0/twitch_thumbnail/synchronous.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:39:36.332658 twitch-thumbnail-1.1.0/twitch_thumbnail.egg-info/
--rw-rw-rw-   0        0        0     1067 2023-01-11 15:39:36.000000 twitch-thumbnail-1.1.0/twitch_thumbnail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-01-11 15:39:36.000000 twitch-thumbnail-1.1.0/twitch_thumbnail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 15:39:36.000000 twitch-thumbnail-1.1.0/twitch_thumbnail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-01-11 15:39:36.000000 twitch-thumbnail-1.1.0/twitch_thumbnail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-01-11 15:39:36.000000 twitch-thumbnail-1.1.0/twitch_thumbnail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 06:39:41.767441 twitch-thumbnail-1.1.1/
+-rw-rw-rw-   0        0        0     1067 2023-06-01 06:39:41.765396 twitch-thumbnail-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-01-11 15:39:14.000000 twitch-thumbnail-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 06:39:41.767441 twitch-thumbnail-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-06-01 06:38:29.000000 twitch-thumbnail-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:39:41.735838 twitch-thumbnail-1.1.1/twitch_thumbnail/
+-rw-rw-rw-   0        0        0      325 2023-01-09 17:08:12.000000 twitch-thumbnail-1.1.1/twitch_thumbnail/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-01-11 15:30:41.000000 twitch-thumbnail-1.1.1/twitch_thumbnail/asynchronous.py
+-rw-rw-rw-   0        0        0      429 2023-01-11 15:35:19.000000 twitch-thumbnail-1.1.1/twitch_thumbnail/exceptions.py
+-rw-rw-rw-   0        0        0      333 2023-01-09 17:11:26.000000 twitch-thumbnail-1.1.1/twitch_thumbnail/ffmpeg.py
+-rw-rw-rw-   0        0        0     1942 2023-01-11 15:35:31.000000 twitch-thumbnail-1.1.1/twitch_thumbnail/streamlink.py
+-rw-rw-rw-   0        0        0     1325 2023-01-11 15:30:52.000000 twitch-thumbnail-1.1.1/twitch_thumbnail/synchronous.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:39:41.761268 twitch-thumbnail-1.1.1/twitch_thumbnail.egg-info/
+-rw-rw-rw-   0        0        0     1067 2023-06-01 06:39:41.000000 twitch-thumbnail-1.1.1/twitch_thumbnail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-06-01 06:39:41.000000 twitch-thumbnail-1.1.1/twitch_thumbnail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 06:39:41.000000 twitch-thumbnail-1.1.1/twitch_thumbnail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-01 06:39:41.000000 twitch-thumbnail-1.1.1/twitch_thumbnail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-01 06:39:41.000000 twitch-thumbnail-1.1.1/twitch_thumbnail.egg-info/top_level.txt
```

### Comparing `twitch-thumbnail-1.1.0/PKG-INFO` & `twitch-thumbnail-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-thumbnail
-Version: 1.1.0
+Version: 1.1.1
 Summary: Download Twitch channel thumbnail
 Home-page: https://github.com/minibox24/twitch-thumbnail
 Author: Minibox
 Author-email: minibox724@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `twitch-thumbnail-1.1.0/README.md` & `twitch-thumbnail-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `twitch-thumbnail-1.1.0/setup.py` & `twitch-thumbnail-1.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 readme = ""
 with open(f"README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name="twitch-thumbnail",
-    version="1.1.0",
+    version="1.1.1",
     description="Download Twitch channel thumbnail",
     author="Minibox",
     author_email="minibox724@gmail.com",
     url="https://github.com/minibox24/twitch-thumbnail",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
```

### Comparing `twitch-thumbnail-1.1.0/twitch_thumbnail/asynchronous.py` & `twitch-thumbnail-1.1.1/twitch_thumbnail/asynchronous.py`

 * *Files identical despite different names*

### Comparing `twitch-thumbnail-1.1.0/twitch_thumbnail/streamlink.py` & `twitch-thumbnail-1.1.1/twitch_thumbnail/streamlink.py`

 * *Files identical despite different names*

### Comparing `twitch-thumbnail-1.1.0/twitch_thumbnail/synchronous.py` & `twitch-thumbnail-1.1.1/twitch_thumbnail/synchronous.py`

 * *Files identical despite different names*

### Comparing `twitch-thumbnail-1.1.0/twitch_thumbnail.egg-info/PKG-INFO` & `twitch-thumbnail-1.1.1/twitch_thumbnail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-thumbnail
-Version: 1.1.0
+Version: 1.1.1
 Summary: Download Twitch channel thumbnail
 Home-page: https://github.com/minibox24/twitch-thumbnail
 Author: Minibox
 Author-email: minibox724@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

