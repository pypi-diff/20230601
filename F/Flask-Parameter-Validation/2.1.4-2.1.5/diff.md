# Comparing `tmp/Flask-Parameter-Validation-2.1.4.tar.gz` & `tmp/Flask-Parameter-Validation-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Parameter-Validation-2.1.4.tar", last modified: Thu Apr 13 15:53:05 2023, max compression
+gzip compressed data, was "Flask-Parameter-Validation-2.1.5.tar", last modified: Thu Jun  1 15:19:18 2023, max compression
```

## Comparing `Flask-Parameter-Validation-2.1.4.tar` & `Flask-Parameter-Validation-2.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 15:53:05.000000 Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:53:05.243067 Flask-Parameter-Validation-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-13 15:52:55.000000 Flask-Parameter-Validation-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:19:18.232127 Flask-Parameter-Validation-2.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:19:18.228127 Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-01 15:19:18.000000 Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-01 15:19:18.000000 Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:19:18.000000 Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:19:18.000000 Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 15:19:18.000000 Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 15:19:18.000000 Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-01 15:19:18.232127 Flask-Parameter-Validation-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:19:18.228127 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:19:18.228127 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:19:18.232127 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:19:18.232127 Flask-Parameter-Validation-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-01 15:19:06.000000 Flask-Parameter-Validation-2.1.5/setup.py
```

### Comparing `Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/PKG-INFO` & `Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Parameter-Validation
-Version: 2.1.4
+Version: 2.1.5
 Summary: Get and validate all Flask input parameters with ease.
 Home-page: https://github.com/Ge0rg3/flask-parameter-validation
 Author: George Omnet
 Author-email: flaskparametervalidation@georgeom.net
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flask-Parameter-Validation-2.1.4/Flask_Parameter_Validation.egg-info/SOURCES.txt` & `Flask-Parameter-Validation-2.1.5/Flask_Parameter_Validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.4/PKG-INFO` & `Flask-Parameter-Validation-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Parameter-Validation
-Version: 2.1.4
+Version: 2.1.5
 Summary: Get and validate all Flask input parameters with ease.
 Home-page: https://github.com/Ge0rg3/flask-parameter-validation
 Author: George Omnet
 Author-email: flaskparametervalidation@georgeom.net
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flask-Parameter-Validation-2.1.4/README.md` & `Flask-Parameter-Validation-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/exceptions/exceptions.py` & `Flask-Parameter-Validation-2.1.5/flask_parameter_validation/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/file.py` & `Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/file.py`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/parameter.py` & `Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/parameter.py`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_types/query.py` & `Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_types/query.py`

 * *Files identical despite different names*

### Comparing `Flask-Parameter-Validation-2.1.4/flask_parameter_validation/parameter_validation.py` & `Flask-Parameter-Validation-2.1.5/flask_parameter_validation/parameter_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from .parameter_types import Route, Json, Query, Form, File
 from .exceptions import MissingInputError, InvalidParameterTypeError, ValidationError
 from flask import request
 from inspect import signature
 from werkzeug.exceptions import BadRequest
 
 
@@ -13,19 +15,20 @@
     def __call__(self, f):
         """
         Parent flow for validating each required parameter
         """
         def nested_func(**kwargs):
             # Step 1 - Combine all flask input types to one dict
             json_input = None
-            if request.headers.get("content-type") == "application/json":
-                try:
-                    json_input = request.json
-                except BadRequest:
-                    return {"error": "Could not parse JSON."}, 400
+            if request.headers.get("Content-Type") is not None:
+                if re.search("application/[^+]*[+]?(json);?", request.headers.get("Content-Type")):
+                    try:
+                        json_input = request.json
+                    except BadRequest:
+                        return {"error": "Could not parse JSON."}, 400
             request_inputs = {
                 Route: kwargs.copy(),
                 Json: json_input,
                 Query: request.args.to_dict(),
                 Form: request.form.to_dict(),
                 File: request.files.to_dict()
             }
```

### Comparing `Flask-Parameter-Validation-2.1.4/setup.py` & `Flask-Parameter-Validation-2.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='Flask-Parameter-Validation',
-    version='2.1.4',
+    version='2.1.5',
     url='https://github.com/Ge0rg3/flask-parameter-validation',
     license='MIT',
     author='George Omnet',
     author_email='flaskparametervalidation@georgeom.net',
     description='Get and validate all Flask input parameters with ease.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

