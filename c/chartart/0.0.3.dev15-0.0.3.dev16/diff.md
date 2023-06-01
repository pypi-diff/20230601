# Comparing `tmp/chartart-0.0.3.dev15.tar.gz` & `tmp/chartart-0.0.3.dev16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev15.tar", last modified: Wed May 31 13:20:42 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev16.tar", last modified: Thu Jun  1 06:11:02 2023, max compression
```

## Comparing `chartart-0.0.3.dev15.tar` & `chartart-0.0.3.dev16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.888101 chartart-0.0.3.dev15/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-05-31 13:20:42.888423 chartart-0.0.3.dev15/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     1814 2023-05-31 13:18:32.000000 chartart-0.0.3.dev15/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-05-31 13:20:42.890194 chartart-0.0.3.dev15/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.863726 chartart-0.0.3.dev15/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.878116 chartart-0.0.3.dev15/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    80235 2023-05-31 13:16:14.000000 chartart-0.0.3.dev15/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.885937 chartart-0.0.3.dev15/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.883654 chartart-0.0.3.dev15/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-05-31 13:20:42.000000 chartart-0.0.3.dev15/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-05-31 13:20:42.887132 chartart-0.0.3.dev15/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev15/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.535534 chartart-0.0.3.dev16/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-01 06:11:02.535934 chartart-0.0.3.dev16/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1814 2023-05-31 13:18:32.000000 chartart-0.0.3.dev16/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-06-01 06:11:02.540001 chartart-0.0.3.dev16/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.489453 chartart-0.0.3.dev16/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.512547 chartart-0.0.3.dev16/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    80851 2023-06-01 06:10:01.000000 chartart-0.0.3.dev16/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.529989 chartart-0.0.3.dev16/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.520333 chartart-0.0.3.dev16/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-06-01 06:11:02.000000 chartart-0.0.3.dev16/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-01 06:11:02.533020 chartart-0.0.3.dev16/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev16/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev15/LICENSE` & `chartart-0.0.3.dev16/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev15/PKG-INFO` & `chartart-0.0.3.dev16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev15
+Version: 0.0.3.dev16
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chartart-0.0.3.dev15/README.md` & `chartart-0.0.3.dev16/README.md`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev15/setup.cfg` & `chartart-0.0.3.dev16/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev15
+version = 0.0.3.dev16
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev15/src/chartart/__init__.py` & `chartart-0.0.3.dev16/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev15/src/chartart/conftest.py` & `chartart-0.0.3.dev16/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev15/src/chartart/helpers.py` & `chartart-0.0.3.dev16/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev15/src/chartart/plot.py` & `chartart-0.0.3.dev16/src/chartart/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1334,14 +1334,21 @@
         if bubbleColorMappers is not None:
             map_info['bubbleColorMappers'] = bubbleColorMappers
         if legend is not None:
             map_info['legend'] = legend
         if marker is not None:
             map_info['marker'] = marker
         if layers is not None:
+            # Convert 'coordinates':[[10,20], [50,60]] into  'coordinates': [{'latitude': 10, 'longitude': 20}, {'latitude': 50, 'longitude': 60}]
+            # This is because firebase dont allow nested array. For user interface we allowed nested array because geojson has same format.  
+            for layer in layers:
+                if ('coordinates' in layer):
+                    for index, coordinate in enumerate(layer['coordinates']):
+                        if isinstance(coordinate, list):
+                            layer['coordinates'][index] = {'latitude': coordinate[0], 'longitude': coordinate[1]}
             map_info['layers'] = layers
 
         if data is not None:
             map_info['data'] = data 
 
         self.data.insert(map_info)
```

### Comparing `chartart-0.0.3.dev15/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev16/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev15/src/chartart/test_plot.py` & `chartart-0.0.3.dev16/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev15/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev16/src/chartart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev15
+Version: 0.0.3.dev16
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
```

