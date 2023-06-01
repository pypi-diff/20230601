# Comparing `tmp/pytele2api-0.1.1.tar.gz` & `tmp/pytele2api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytele2api-0.1.1.tar", last modified: Thu Jun  1 09:00:38 2023, max compression
+gzip compressed data, was "pytele2api-0.1.3.tar", last modified: Thu Jun  1 09:21:50 2023, max compression
```

## Comparing `pytele2api-0.1.1.tar` & `pytele2api-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:00:38.817501 pytele2api-0.1.1/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.1/LICENSE
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.1/MANIFEST.in
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 09:00:38.817563 pytele2api-0.1.1/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.1/README.md
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:00:38.816460 pytele2api-0.1.1/pytele2api/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     4034 2023-06-01 08:31:35.000000 pytele2api-0.1.1/pytele2api/Tele2Api.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.1/pytele2api/__init__.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      484 2023-06-01 07:19:00.000000 pytele2api-0.1.1/pytele2api/const.py
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:00:38.817390 pytele2api-0.1.1/pytele2api.egg-info/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/requires.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/top_level.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-01 09:00:38.817763 pytele2api-0.1.1/setup.cfg
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-01 08:40:20.000000 pytele2api-0.1.1/setup.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:21:50.718857 pytele2api-0.1.3/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.3/LICENSE
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.3/MANIFEST.in
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 09:21:50.718927 pytele2api-0.1.3/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.3/README.md
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:21:50.717860 pytele2api-0.1.3/pytele2api/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     4019 2023-06-01 09:16:55.000000 pytele2api-0.1.3/pytele2api/Tele2Api.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.3/pytele2api/__init__.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      484 2023-06-01 07:19:00.000000 pytele2api-0.1.3/pytele2api/const.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:21:50.718697 pytele2api-0.1.3/pytele2api.egg-info/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 09:21:50.000000 pytele2api-0.1.3/pytele2api.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-01 09:21:50.000000 pytele2api-0.1.3/pytele2api.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-01 09:21:50.000000 pytele2api-0.1.3/pytele2api.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-01 09:21:50.000000 pytele2api-0.1.3/pytele2api.egg-info/requires.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-01 09:21:50.000000 pytele2api-0.1.3/pytele2api.egg-info/top_level.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-01 09:21:50.719154 pytele2api-0.1.3/setup.cfg
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-01 09:20:40.000000 pytele2api-0.1.3/setup.py
```

### Comparing `pytele2api-0.1.1/LICENSE` & `pytele2api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytele2api-0.1.1/PKG-INFO` & `pytele2api-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.3.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.1/pytele2api/Tele2Api.py` & `pytele2api-0.1.3/pytele2api/Tele2Api.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,15 @@
         return {}
 
     def getDataUsage(self) -> dict:
         resp = self.session.get(self.DATA_USAGE_URL)
         if (resp.status_code == 401 or resp.status_code == 403) and self.tries < 1:
             self.tries += 1
             self.updateAuth()
-            self.getDataUsage()
-            return {}
+            return self.getDataUsage()
         elif resp.status_code == 200:
             data = json.loads(resp.content)
             limit = data[Tele2ApiResult.packageLimit]
             usage = data["usage"]
             remaining = data[Tele2ApiResult.remaining]
 
             self.log(
```

### Comparing `pytele2api-0.1.1/pytele2api.egg-info/PKG-INFO` & `pytele2api-0.1.3/pytele2api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.3.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.1/setup.py` & `pytele2api-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytele2api",
-    version="0.1.1",
+    version="0.1.3",
     author="Fredrik Häggbom",
     author_email="fredrik.haggbom@gmail.com",
     description="Python library for communication with Tele2 My TSO",
-    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.1.tar.gz",
+    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.3.tar.gz",
     keywords=["tele2"],
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredrikhaggbom/pytele2",
     packages=setuptools.find_packages(),
     install_requires=["requests", "datetime"],
```

