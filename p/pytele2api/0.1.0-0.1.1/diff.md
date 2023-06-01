# Comparing `tmp/pytele2api-0.1.0.tar.gz` & `tmp/pytele2api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytele2api-0.1.0.tar", last modified: Thu Jun  1 07:35:32 2023, max compression
+gzip compressed data, was "pytele2api-0.1.1.tar", last modified: Thu Jun  1 09:00:38 2023, max compression
```

## Comparing `pytele2api-0.1.0.tar` & `pytele2api-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 07:35:32.840767 pytele2api-0.1.0/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.0/LICENSE
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.0/MANIFEST.in
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 07:35:32.840812 pytele2api-0.1.0/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.0/README.md
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 07:35:32.839866 pytele2api-0.1.0/pytele2api/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     3780 2023-06-01 07:20:36.000000 pytele2api-0.1.0/pytele2api/Tele2Api.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.0/pytele2api/__init__.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      484 2023-06-01 07:19:00.000000 pytele2api-0.1.0/pytele2api/const.py
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 07:35:32.840655 pytele2api-0.1.0/pytele2api.egg-info/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 07:35:32.000000 pytele2api-0.1.0/pytele2api.egg-info/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-01 07:35:32.000000 pytele2api-0.1.0/pytele2api.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-01 07:35:32.000000 pytele2api-0.1.0/pytele2api.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-01 07:35:32.000000 pytele2api-0.1.0/pytele2api.egg-info/requires.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-01 07:35:32.000000 pytele2api-0.1.0/pytele2api.egg-info/top_level.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-01 07:35:32.840983 pytele2api-0.1.0/setup.cfg
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-01 07:34:50.000000 pytele2api-0.1.0/setup.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:00:38.817501 pytele2api-0.1.1/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.1/LICENSE
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.1/MANIFEST.in
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 09:00:38.817563 pytele2api-0.1.1/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.1/README.md
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:00:38.816460 pytele2api-0.1.1/pytele2api/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     4034 2023-06-01 08:31:35.000000 pytele2api-0.1.1/pytele2api/Tele2Api.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.1/pytele2api/__init__.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      484 2023-06-01 07:19:00.000000 pytele2api-0.1.1/pytele2api/const.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 09:00:38.817390 pytele2api-0.1.1/pytele2api.egg-info/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/requires.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-01 09:00:38.000000 pytele2api-0.1.1/pytele2api.egg-info/top_level.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-01 09:00:38.817763 pytele2api-0.1.1/setup.cfg
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-01 08:40:20.000000 pytele2api-0.1.1/setup.py
```

### Comparing `pytele2api-0.1.0/LICENSE` & `pytele2api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytele2api-0.1.0/PKG-INFO` & `pytele2api-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.1.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.0/pytele2api/Tele2Api.py` & `pytele2api-0.1.1/pytele2api/Tele2Api.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
     def getSubscription(self) -> dict:
         self.session.post(self.AUTH_URL, data=self.CREDENTIALS)
         resp = self.session.get(self.SUBSCRIPTION_URL)
 
         if resp.status_code == 200:
             data = json.loads(resp.content)
+            self.log("Got subscription info: ", str(data))
             if len(data) > 0 and "subsId" in data[0]:
                 return {
                     CONF_SUBSCRIPTION: str(data[0]["subsId"]),
                     CONF_SUBSCRIPTIONMODEL: data[0]["name"],
                 }
 
         return {}
@@ -77,14 +78,22 @@
             return {}
         elif resp.status_code == 200:
             data = json.loads(resp.content)
             limit = data[Tele2ApiResult.packageLimit]
             usage = data["usage"]
             remaining = data[Tele2ApiResult.remaining]
 
+            self.log(
+                "Got result. Limit: %s, usage: %s, remaining: %s, unlimited: %s",
+                limit,
+                usage,
+                remaining,
+                data[Tele2ApiResult.unlimitedData],
+            )
+
             if Tele2ApiResult.unlimitedData in data:
                 self._data[RES_UNLIMITED] = data[Tele2ApiResult.unlimitedData]
 
             if Tele2ApiResult.buckets in data and len(data["buckets"]) > 0:
                 bucket = data["buckets"][0]
                 if Tele2ApiResult.startDate in bucket:
                     startDate = datetime.datetime.strptime(
@@ -93,24 +102,23 @@
                     self._data[RES_PERIOD_START] = startDate
                 if Tele2ApiResult.endDate in bucket:
                     endDate = datetime.datetime.strptime(
                         bucket[Tele2ApiResult.endDate], "%Y-%m-%d"
                     ).date()
                     self._data[RES_PERIOD_END] = endDate
 
-            if limit is not None and remaining is not None:
-                dataLeft = remaining
-                self.tries = 0
-                self._data[RES_LIMIT] = limit
-                self._data[RES_USAGE] = usage
-                self._data[RES_DATA_LEFT] = dataLeft
-                self.isUpdating = False
-                return self._data
+            self.tries = 0
+            self._data[RES_LIMIT] = limit
+            self._data[RES_USAGE] = usage
+            self._data[RES_DATA_LEFT] = remaining
+            self.log("Setting native value to: %d", remaining)
+            return self._data
 
         return {}
 
     def updateAuth(self) -> None:
+        self.log("Updating authentication")
         self.session.post(self.AUTH_URL, data=self.CREDENTIALS)
 
     def log(self, msg, *args, **kwargs):
         if self._LOGGER is not None:
             self._LOGGER.debug(msg, args)
```

### Comparing `pytele2api-0.1.0/pytele2api.egg-info/PKG-INFO` & `pytele2api-0.1.1/pytele2api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.1.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.0/setup.py` & `pytele2api-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytele2api",
-    version="0.1.0",
+    version="0.1.1",
     author="Fredrik Häggbom",
     author_email="fredrik.haggbom@gmail.com",
     description="Python library for communication with Tele2 My TSO",
-    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.0.tar.gz",
+    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.1.tar.gz",
     keywords=["tele2"],
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredrikhaggbom/pytele2",
     packages=setuptools.find_packages(),
     install_requires=["requests", "datetime"],
```

