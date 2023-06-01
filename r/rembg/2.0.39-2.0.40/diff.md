# Comparing `tmp/rembg-2.0.39.tar.gz` & `tmp/rembg-2.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.39.tar", last modified: Tue May 30 04:51:08 2023, max compression
+gzip compressed data, was "rembg-2.0.40.tar", last modified: Thu Jun  1 05:58:31 2023, max compression
```

## Comparing `rembg-2.0.39.tar` & `rembg-2.0.40.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.814818 rembg-2.0.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 04:50:54.000000 rembg-2.0.39/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-30 04:50:54.000000 rembg-2.0.39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-05-30 04:51:08.814818 rembg-2.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-05-30 04:50:54.000000 rembg-2.0.39/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-30 04:50:54.000000 rembg-2.0.39/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.814818 rembg-2.0.39/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-30 04:51:08.814818 rembg-2.0.39/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.810818 rembg-2.0.39/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.814818 rembg-2.0.39/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.810818 rembg-2.0.39/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 04:50:54.000000 rembg-2.0.39/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-30 04:50:54.000000 rembg-2.0.39/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 04:51:08.814818 rembg-2.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-30 04:50:54.000000 rembg-2.0.39/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-30 04:50:54.000000 rembg-2.0.39/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:58:31.312757 rembg-2.0.40/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 05:58:20.000000 rembg-2.0.40/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 05:58:20.000000 rembg-2.0.40/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-06-01 05:58:31.312757 rembg-2.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-06-01 05:58:20.000000 rembg-2.0.40/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 05:58:21.000000 rembg-2.0.40/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:58:31.312757 rembg-2.0.40/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 05:58:31.312757 rembg-2.0.40/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:58:31.308757 rembg-2.0.40/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:58:31.312757 rembg-2.0.40/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-01 05:58:21.000000 rembg-2.0.40/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:58:31.308757 rembg-2.0.40/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-06-01 05:58:31.000000 rembg-2.0.40/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-01 05:58:31.000000 rembg-2.0.40/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 05:58:31.000000 rembg-2.0.40/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 05:58:31.000000 rembg-2.0.40/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 05:58:31.000000 rembg-2.0.40/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 05:58:31.000000 rembg-2.0.40/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 05:58:21.000000 rembg-2.0.40/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 05:58:21.000000 rembg-2.0.40/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 05:58:31.312757 rembg-2.0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-01 05:58:21.000000 rembg-2.0.40/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-01 05:58:21.000000 rembg-2.0.40/versioneer.py
```

### Comparing `rembg-2.0.39/LICENSE.txt` & `rembg-2.0.40/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/PKG-INFO` & `rembg-2.0.40/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.39
+Version: 2.0.40
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
```

### Comparing `rembg-2.0.39/README.md` & `rembg-2.0.40/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/bg.py` & `rembg-2.0.40/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/commands/b_command.py` & `rembg-2.0.40/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/commands/i_command.py` & `rembg-2.0.40/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/commands/p_command.py` & `rembg-2.0.40/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/commands/s_command.py` & `rembg-2.0.40/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/session_factory.py` & `rembg-2.0.40/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/__init__.py` & `rembg-2.0.40/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/base.py` & `rembg-2.0.40/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/dis_anime.py` & `rembg-2.0.40/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/dis_general_use.py` & `rembg-2.0.40/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/sam.py` & `rembg-2.0.40/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/silueta.py` & `rembg-2.0.40/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/u2net.py` & `rembg-2.0.40/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.40/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.40/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg/sessions/u2netp.py` & `rembg-2.0.40/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/rembg.egg-info/PKG-INFO` & `rembg-2.0.40/rembg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.39
+Version: 2.0.40
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
```

### Comparing `rembg-2.0.39/rembg.egg-info/SOURCES.txt` & `rembg-2.0.40/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.39/setup.py` & `rembg-2.0.40/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,38 +33,38 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="remove, background, u2net",
     packages=["rembg", "rembg.sessions", "rembg.commands"],
     python_requires=">3.7, <3.11",
     install_requires=[
-        "aiohttp>=3.8.1",
-        "asyncer>=0.0.2",
-        "click>=8.1.3",
-        "fastapi>=0.92.0",
-        "filetype>=1.2.0",
-        "gradio>=3.32.0",
-        "imagehash>=4.3.1",
-        "numpy>=1.23.5",
-        "onnxruntime>=1.14.1",
-        "opencv-python-headless>=4.6.0.66",
-        "pillow>=9.3.0",
-        "pooch>=1.6.0",
-        "pymatting>=1.1.8",
-        "python-multipart>=0.0.5",
-        "scikit-image>=0.19.3",
-        "scipy>=1.9.3",
-        "tqdm>=4.64.1",
-        "uvicorn>=0.20.0",
-        "watchdog>=2.1.9",
+        "aiohttp",
+        "asyncer",
+        "click",
+        "fastapi",
+        "filetype",
+        "gradio",
+        "imagehash",
+        "numpy",
+        "onnxruntime",
+        "opencv-python-headless",
+        "pillow",
+        "pooch",
+        "pymatting",
+        "python-multipart",
+        "scikit-image",
+        "scipy",
+        "tqdm",
+        "uvicorn",
+        "watchdog",
     ],
     entry_points={
         "console_scripts": [
             "rembg=rembg.cli:main",
         ],
     },
     extras_require={
-        "gpu": ["onnxruntime-gpu>=1.14.1"],
+        "gpu": ["onnxruntime-gpu"],
     },
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `rembg-2.0.39/versioneer.py` & `rembg-2.0.40/versioneer.py`

 * *Files identical despite different names*

