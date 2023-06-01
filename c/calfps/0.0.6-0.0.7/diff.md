# Comparing `tmp/calfps-0.0.6.tar.gz` & `tmp/calfps-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfps-0.0.6.tar", last modified: Thu Jun  1 08:30:44 2023, max compression
+gzip compressed data, was "calfps-0.0.7.tar", last modified: Thu Jun  1 08:33:01 2023, max compression
```

## Comparing `calfps-0.0.6.tar` & `calfps-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:30:44.315559 calfps-0.0.6/
--rw-rw-r--   0 alyce     (1000) alyce     (1000)     1065 2023-05-11 02:13:38.000000 calfps-0.0.6/LICENSE.txt
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-06-01 08:30:44.315559 calfps-0.0.6/PKG-INFO
--rw-rw-r--   0 alyce     (1000) alyce     (1000)       73 2023-05-11 02:14:48.000000 calfps-0.0.6/README.md
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      103 2023-05-11 02:12:02.000000 calfps-0.0.6/pyproject.toml
--rw-rw-r--   0 alyce     (1000) alyce     (1000)       38 2023-06-01 08:30:44.315559 calfps-0.0.6/setup.cfg
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      792 2023-06-01 08:30:36.000000 calfps-0.0.6/setup.py
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:30:44.311559 calfps-0.0.6/src/
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:30:44.315559 calfps-0.0.6/src/calculate/
--rw-rw-r--   0 alyce     (1000) alyce     (1000)        0 2023-05-11 01:50:42.000000 calfps-0.0.6/src/calculate/__init__.py
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      522 2023-06-01 08:30:30.000000 calfps-0.0.6/src/calculate/fps.py
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:30:44.315559 calfps-0.0.6/src/calfps.egg-info/
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-06-01 08:30:44.000000 calfps-0.0.6/src/calfps.egg-info/PKG-INFO
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      228 2023-06-01 08:30:44.000000 calfps-0.0.6/src/calfps.egg-info/SOURCES.txt
--rw-rw-r--   0 alyce     (1000) alyce     (1000)        1 2023-06-01 08:30:44.000000 calfps-0.0.6/src/calfps.egg-info/dependency_links.txt
--rw-rw-r--   0 alyce     (1000) alyce     (1000)       10 2023-06-01 08:30:44.000000 calfps-0.0.6/src/calfps.egg-info/top_level.txt
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:33:01.183606 calfps-0.0.7/
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)     1065 2023-05-11 02:13:38.000000 calfps-0.0.7/LICENSE.txt
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-06-01 08:33:01.183606 calfps-0.0.7/PKG-INFO
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)       73 2023-05-11 02:14:48.000000 calfps-0.0.7/README.md
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      103 2023-05-11 02:12:02.000000 calfps-0.0.7/pyproject.toml
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)       38 2023-06-01 08:33:01.183606 calfps-0.0.7/setup.cfg
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      792 2023-06-01 08:32:54.000000 calfps-0.0.7/setup.py
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:33:01.179606 calfps-0.0.7/src/
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:33:01.183606 calfps-0.0.7/src/calculate/
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)        0 2023-05-11 01:50:42.000000 calfps-0.0.7/src/calculate/__init__.py
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      527 2023-06-01 08:32:31.000000 calfps-0.0.7/src/calculate/fps.py
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-06-01 08:33:01.183606 calfps-0.0.7/src/calfps.egg-info/
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-06-01 08:33:01.000000 calfps-0.0.7/src/calfps.egg-info/PKG-INFO
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      228 2023-06-01 08:33:01.000000 calfps-0.0.7/src/calfps.egg-info/SOURCES.txt
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)        1 2023-06-01 08:33:01.000000 calfps-0.0.7/src/calfps.egg-info/dependency_links.txt
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)       10 2023-06-01 08:33:01.000000 calfps-0.0.7/src/calfps.egg-info/top_level.txt
```

### Comparing `calfps-0.0.6/LICENSE.txt` & `calfps-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `calfps-0.0.6/PKG-INFO` & `calfps-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfps
-Version: 0.0.6
+Version: 0.0.7
 Summary: calculating fps as simple
 Home-page: https://github.com/Junhojuno/test-fps
 Author: Junhojuno
 Author-email: rlawnsgh2245@gmail.com
 Project-URL: Bug Tracker, https://github.com/Junhojuno/test-fps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calfps-0.0.6/setup.py` & `calfps-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="calfps",
-    version="0.0.6",
+    version="0.0.7",
     author="Junhojuno",
     author_email="rlawnsgh2245@gmail.com",
     description="calculating fps as simple",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Junhojuno/test-fps",
     project_urls={
```

### Comparing `calfps-0.0.6/src/calculate/fps.py` & `calfps-0.0.7/src/calculate/fps.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         f"{time_info.tm_sec}.{sec_decimal}"
     )
 
 
 def calculate_fps(start_time, fps_avg_frame_count) -> Tuple[str, str]:
     fps = 15.0 + random.uniform(0.0, 1.5)
     end_time = 1 / fps + start_time
-    return get_time_string(start_time), get_time_string(end_time)
+    return fps, get_time_string(start_time), get_time_string(end_time)
```

### Comparing `calfps-0.0.6/src/calfps.egg-info/PKG-INFO` & `calfps-0.0.7/src/calfps.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfps
-Version: 0.0.6
+Version: 0.0.7
 Summary: calculating fps as simple
 Home-page: https://github.com/Junhojuno/test-fps
 Author: Junhojuno
 Author-email: rlawnsgh2245@gmail.com
 Project-URL: Bug Tracker, https://github.com/Junhojuno/test-fps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

