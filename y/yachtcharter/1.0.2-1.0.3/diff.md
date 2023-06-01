# Comparing `tmp/yachtcharter-1.0.2.tar.gz` & `tmp/yachtcharter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yachtcharter-1.0.2.tar", last modified: Tue Sep 20 04:51:56 2022, max compression
+gzip compressed data, was "yachtcharter-1.0.3.tar", last modified: Thu Jun  1 05:35:15 2023, max compression
```

## Comparing `yachtcharter-1.0.2.tar` & `yachtcharter-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nick_evershed   (503) staff       (20)        0 2022-09-20 04:51:56.405121 yachtcharter-1.0.2/
--rw-r--r--   0 nick_evershed   (503) staff       (20)      519 2022-09-20 04:51:56.404673 yachtcharter-1.0.2/PKG-INFO
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)       40 2021-09-22 01:52:14.000000 yachtcharter-1.0.2/README.md
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)      103 2021-09-22 03:27:24.000000 yachtcharter-1.0.2/pyproject.toml
--rw-r--r--   0 nick_evershed   (503) staff       (20)       38 2022-09-20 04:51:56.405211 yachtcharter-1.0.2/setup.cfg
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)      869 2022-09-20 04:50:06.000000 yachtcharter-1.0.2/setup.py
-drwxr-xr-x   0 nick_evershed   (503) staff       (20)        0 2022-09-20 04:51:56.399734 yachtcharter-1.0.2/yachtcharter/
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)     2074 2022-09-20 04:50:30.000000 yachtcharter-1.0.2/yachtcharter/__init__.py
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)      722 2021-09-22 04:12:20.000000 yachtcharter-1.0.2/yachtcharter/test.py
-drwxr-xr-x   0 nick_evershed   (503) staff       (20)        0 2022-09-20 04:51:56.403696 yachtcharter-1.0.2/yachtcharter.egg-info/
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)      519 2022-09-20 04:51:56.000000 yachtcharter-1.0.2/yachtcharter.egg-info/PKG-INFO
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)      293 2022-09-20 04:51:56.000000 yachtcharter-1.0.2/yachtcharter.egg-info/SOURCES.txt
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)        1 2022-09-20 04:51:56.000000 yachtcharter-1.0.2/yachtcharter.egg-info/dependency_links.txt
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)        1 2021-09-22 03:29:09.000000 yachtcharter-1.0.2/yachtcharter.egg-info/not-zip-safe
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)       17 2022-09-20 04:51:56.000000 yachtcharter-1.0.2/yachtcharter.egg-info/requires.txt
--rwxrwxrwx   0 nick_evershed   (503) staff       (20)       13 2022-09-20 04:51:56.000000 yachtcharter-1.0.2/yachtcharter.egg-info/top_level.txt
+drwxr-xr-x   0 nick_evershed   (503) staff       (20)        0 2023-06-01 05:35:15.944718 yachtcharter-1.0.3/
+-rw-r--r--   0 nick_evershed   (503) staff       (20)      524 2023-06-01 05:35:15.944144 yachtcharter-1.0.3/PKG-INFO
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)       46 2022-09-20 05:00:58.000000 yachtcharter-1.0.3/README.md
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)      103 2021-09-22 03:27:24.000000 yachtcharter-1.0.3/pyproject.toml
+-rw-r--r--   0 nick_evershed   (503) staff       (20)       38 2023-06-01 05:35:15.944869 yachtcharter-1.0.3/setup.cfg
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)      869 2023-06-01 05:26:22.000000 yachtcharter-1.0.3/setup.py
+drwxr-xr-x   0 nick_evershed   (503) staff       (20)        0 2023-06-01 05:35:15.938085 yachtcharter-1.0.3/yachtcharter/
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)     2209 2023-06-01 05:33:46.000000 yachtcharter-1.0.3/yachtcharter/__init__.py
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)      722 2021-09-22 04:12:20.000000 yachtcharter-1.0.3/yachtcharter/test.py
+drwxr-xr-x   0 nick_evershed   (503) staff       (20)        0 2023-06-01 05:35:15.943247 yachtcharter-1.0.3/yachtcharter.egg-info/
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)      524 2023-06-01 05:35:15.000000 yachtcharter-1.0.3/yachtcharter.egg-info/PKG-INFO
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)      293 2023-06-01 05:35:15.000000 yachtcharter-1.0.3/yachtcharter.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)        1 2023-06-01 05:35:15.000000 yachtcharter-1.0.3/yachtcharter.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)        1 2021-09-22 03:29:09.000000 yachtcharter-1.0.3/yachtcharter.egg-info/not-zip-safe
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)       17 2023-06-01 05:35:15.000000 yachtcharter-1.0.3/yachtcharter.egg-info/requires.txt
+-rwxrwxrwx   0 nick_evershed   (503) staff       (20)       13 2023-06-01 05:35:15.000000 yachtcharter-1.0.3/yachtcharter.egg-info/top_level.txt
```

### Comparing `yachtcharter-1.0.2/PKG-INFO` & `yachtcharter-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: yachtcharter
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/guardian/yacht-charter-python-library
 Author: Nick Evershed
 Author-email: nick.evershed@theguardian.com
 License: MIT
 Keywords: data-visualization data data-visualisation data analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 
-Yacht Charter v1
+Yacht Charter v1.0.3
 =======================
+
```

### Comparing `yachtcharter-1.0.2/setup.py` & `yachtcharter-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='yachtcharter',
-      version='1.0.2',
+      version='1.0.3',
       long_description=README,
       long_description_content_type="text/markdown",
       classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Information Analysis',
       ],
```

### Comparing `yachtcharter-1.0.2/yachtcharter/__init__.py` & `yachtcharter-1.0.3/yachtcharter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __init__.py
 
 # Version 
-__version__ = "1.0.0"
+__version__ = "1.0.3"
 
 
 import simplejson as json
 import boto3
 import os
 
 AWS_KEY = os.environ['AWS_ACCESS_KEY_ID']
@@ -25,15 +25,15 @@
 			"labels":[],
 			"chartId":"linechart",
 			"options":[],
 			"dropdown":[]
 			}
 	}
 
-def syncData(jsonObject,id,yacht=False,version=20):
+def syncData(jsonObject,id,yacht=False,version=25):
 
 	finalJson = json.dumps(jsonObject, indent=4)
 
 	print("Connecting to S3")
 	bucket = 'gdn-cdn'
 
 	if 'AWS_SESSION_TOKEN' in os.environ:
@@ -58,19 +58,20 @@
 	object = s3.Object(bucket, key)
 	object.put(Body=finalJson, CacheControl="max-age=30", ACL='public-read', ContentType="application/json")
 
 	print("JSON is updated")
 
 	if yacht:
 		print("data", "https://interactive.guim.co.uk/yacht-charter-data/{id}.json".format(id=id))
-		print("chart", "https://interactive.guim.co.uk/embed/aus/2020/yacht-charter-v{version}/index.html?key={id}&location=yacht-charter-data".format(id=id, version=version))
+		print("yachtcharter", "https://interactive.guim.co.uk/embed/aus/2020/yacht-charter-v{version}/index.html?key={id}&location=yacht-charter-data".format(id=id, version=version))
+		print("superyacht", f"https://interactive.guim.co.uk/embed/aus/superyacht/1/index.html?key={id}&location=yacht-charter-data")
 	else:
 		print("data", "https://interactive.guim.co.uk/{id}.json".format(id=id))
 
-def yachtCharter(template, data, chartName, dropdown = [], lines=[], chartId=[{"type":"linechart"}], options=[{"colorScheme":"guardian"}],key=[], periods=[], labels=[], version=24):
+def yachtCharter(template, data, chartName, dropdown = [], lines=[], chartId=[{"type":"linechart"}], options=[{"colorScheme":"guardian"}],key=[], periods=[], labels=[], version=25):
 
 	jsonDictObject = {
 		"sheets":{
 			"template":template,
 			"data":data,
 			"labels":labels,
 			"key":key,
```

### Comparing `yachtcharter-1.0.2/yachtcharter/test.py` & `yachtcharter-1.0.3/yachtcharter/test.py`

 * *Files identical despite different names*

### Comparing `yachtcharter-1.0.2/yachtcharter.egg-info/PKG-INFO` & `yachtcharter-1.0.3/yachtcharter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: yachtcharter
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/guardian/yacht-charter-python-library
 Author: Nick Evershed
 Author-email: nick.evershed@theguardian.com
 License: MIT
 Keywords: data-visualization data data-visualisation data analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 
-Yacht Charter v1
+Yacht Charter v1.0.3
 =======================
+
```

