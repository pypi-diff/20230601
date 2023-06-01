# Comparing `tmp/stabilityai-1.0.2.tar.gz` & `tmp/stabilityai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilityai-1.0.2.tar", last modified: Thu Jun  1 14:32:04 2023, max compression
+gzip compressed data, was "stabilityai-1.0.3.tar", last modified: Thu Jun  1 14:38:49 2023, max compression
```

## Comparing `stabilityai-1.0.2.tar` & `stabilityai-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.107526 stabilityai-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.103526 stabilityai-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.103526 stabilityai-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 14:31:47.000000 stabilityai-1.0.2/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-01 14:31:47.000000 stabilityai-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 14:31:47.000000 stabilityai-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 14:32:04.107526 stabilityai-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-01 14:31:47.000000 stabilityai-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-01 14:31:47.000000 stabilityai-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 14:31:47.000000 stabilityai-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:32:04.107526 stabilityai-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.107526 stabilityai-1.0.2/stabilityai/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 14:31:47.000000 stabilityai-1.0.2/stabilityai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:04.107526 stabilityai-1.0.2/stabilityai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 14:32:04.000000 stabilityai-1.0.2/stabilityai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:38:49.757239 stabilityai-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:38:49.749239 stabilityai-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:38:49.753239 stabilityai-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 14:38:36.000000 stabilityai-1.0.3/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-01 14:38:36.000000 stabilityai-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 14:38:36.000000 stabilityai-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 14:38:49.757239 stabilityai-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-01 14:38:36.000000 stabilityai-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-01 14:38:36.000000 stabilityai-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 14:38:36.000000 stabilityai-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:38:49.757239 stabilityai-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:38:49.753239 stabilityai-1.0.3/stabilityai/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 14:38:36.000000 stabilityai-1.0.3/stabilityai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-01 14:38:36.000000 stabilityai-1.0.3/stabilityai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 14:38:36.000000 stabilityai-1.0.3/stabilityai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 14:38:36.000000 stabilityai-1.0.3/stabilityai/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-06-01 14:38:36.000000 stabilityai-1.0.3/stabilityai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 14:38:36.000000 stabilityai-1.0.3/stabilityai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:38:49.757239 stabilityai-1.0.3/stabilityai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 14:38:49.000000 stabilityai-1.0.3/stabilityai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 14:38:49.000000 stabilityai-1.0.3/stabilityai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:38:49.000000 stabilityai-1.0.3/stabilityai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 14:38:49.000000 stabilityai-1.0.3/stabilityai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 14:38:49.000000 stabilityai-1.0.3/stabilityai.egg-info/top_level.txt
```

### Comparing `stabilityai-1.0.2/.github/workflows/build-and-publish.yml` & `stabilityai-1.0.3/.github/workflows/build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.2/.gitignore` & `stabilityai-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.2/LICENSE` & `stabilityai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.2/PKG-INFO` & `stabilityai-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilityai
-Version: 1.0.2
+Version: 1.0.3
 Summary: *Unofficial* client for the Stability REST API
 Author-email: Estelle Poulin <dev@inspiredby.es>
 License: GPLv3
 Project-URL: homepage, https://github.com/estheruary/stabilityai
 Project-URL: repository, https://github.com/estheruary/stabilityai
 Project-URL: changelog, https://github.com/estheruary/stabilityai/-/blob/main/CHANGELOG.md
 Keywords: stabilityai,bot
```

### Comparing `stabilityai-1.0.2/README.md` & `stabilityai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.2/pyproject.toml` & `stabilityai-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.2/stabilityai/client.py` & `stabilityai-1.0.3/stabilityai/client.py`

 * *Files identical despite different names*

### Comparing `stabilityai-1.0.2/stabilityai/models.py` & `stabilityai-1.0.3/stabilityai/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,16 +183,16 @@
     height: Optional[DiffuseImageHeight] = None
     width: Optional[DiffuseImageWidth] = None
     text_prompts: TextPrompts
 
 
 class ImageToImageUpscaleRequestBody(BaseModel):
     image: InitImage
-    width: Optional[UpscaleImageWidth]
-    height: Optional[UpscaleImageHeight]
+    width: Optional[UpscaleImageWidth] = None
+    height: Optional[UpscaleImageHeight] = None
 
     @validator("width", always=True)
     def mutually_exclusive(cls, v, values):
         if values["height"] is not None and v:
             raise ValueError("You can only specify one of width and height.")
         return v
```

### Comparing `stabilityai-1.0.2/stabilityai.egg-info/PKG-INFO` & `stabilityai-1.0.3/stabilityai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilityai
-Version: 1.0.2
+Version: 1.0.3
 Summary: *Unofficial* client for the Stability REST API
 Author-email: Estelle Poulin <dev@inspiredby.es>
 License: GPLv3
 Project-URL: homepage, https://github.com/estheruary/stabilityai
 Project-URL: repository, https://github.com/estheruary/stabilityai
 Project-URL: changelog, https://github.com/estheruary/stabilityai/-/blob/main/CHANGELOG.md
 Keywords: stabilityai,bot
```

