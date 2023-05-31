# Comparing `tmp/itutor_fastapi_middlewares-0.0.6.tar.gz` & `tmp/itutor_fastapi_middlewares-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itutor_fastapi_middlewares-0.0.6.tar", last modified: Wed May 31 23:34:25 2023, max compression
+gzip compressed data, was "itutor_fastapi_middlewares-0.0.7.tar", last modified: Wed May 31 23:41:40 2023, max compression
```

## Comparing `itutor_fastapi_middlewares-0.0.6.tar` & `itutor_fastapi_middlewares-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.230009 itutor_fastapi_middlewares-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/itutor_google_sso/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/itutor_google_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/itutor_google_sso/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/itutor_google_sso/templates/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/css/
--rw-r--r--   0 runner    (1001) docker     (123)   197782 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/css/index.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1187141 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/js/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/js/index.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/src/images/
--rw-r--r--   0 runner    (1001) docker     (123)    26141 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/src/images/itutor-signature-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:25.226009 itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 23:34:25.000000 itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 23:34:25.000000 itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:34:25.000000 itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 23:34:25.000000 itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 23:34:25.000000 itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:34:25.230009 itutor_fastapi_middlewares-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-31 23:34:13.000000 itutor_fastapi_middlewares-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.499671 itutor_fastapi_middlewares-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 23:41:40.499671 itutor_fastapi_middlewares-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.495671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.495671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/itutor_google_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/itutor_google_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.495671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/itutor_google_sso/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/itutor_google_sso/templates/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.491671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.491671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.495671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   197782 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/css/index.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.495671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1187141 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/js/index.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.491671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.495671 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/src/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    26141 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/src/images/itutor-signature-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:41:40.499671 itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 23:41:40.000000 itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 23:41:40.000000 itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:41:40.000000 itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 23:41:40.000000 itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 23:41:40.000000 itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:41:40.499671 itutor_fastapi_middlewares-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-31 23:41:30.000000 itutor_fastapi_middlewares-0.0.7/setup.py
```

### Comparing `itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/examples.py` & `itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/examples.py`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py` & `itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/itutor_google_sso/itutor_google_sso.py`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/itutor_google_sso/templates/login.html` & `itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/itutor_google_sso/templates/login.html`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/css/index.css` & `itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/css/index.css`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/dist/js/index.js` & `itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/dist/js/index.js`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.6/fastapi_middlewares/statics/src/images/itutor-signature-logo.png` & `itutor_fastapi_middlewares-0.0.7/fastapi_middlewares/statics/src/images/itutor-signature-logo.png`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/PKG-INFO` & `itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itutor-fastapi-middlewares
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package for google sso login in FastAPI
 Home-page: https://github.com/bcpitutor/fastapi_middlewares
 Author: Nicolas Acosta
 Author-email: nicolas.acosta@itutor.com
 Keywords: google-sso,fastapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `itutor_fastapi_middlewares-0.0.6/itutor_fastapi_middlewares.egg-info/SOURCES.txt` & `itutor_fastapi_middlewares-0.0.7/itutor_fastapi_middlewares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itutor_fastapi_middlewares-0.0.6/setup.py` & `itutor_fastapi_middlewares-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'Package for google sso login in FastAPI'
 LONG_DESCRIPTION = 'Package for google sso login in FastAPI'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="itutor_fastapi_middlewares", 
@@ -14,17 +14,17 @@
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         package_dir={'fastapi_middlewares': 'fastapi_middlewares'},
         include_package_data = True,
         package_data={'fastapi_middlewares': ['statics/*', 'itutor_google_sso/templates/*']},
         install_requires=[
-            "Authlib==1.0.1", 
-            "httpx==0.23.0", 
-            "itsdangerous==2.1.2", 
+            "Authlib>=1.0.1", 
+            "httpx>=0.23.0", 
+            "itsdangerous>=2.1.2", 
             "jinja2>=3.1.1", 
             "fastapi>=0.75.2", 
         ],
         url="https://github.com/bcpitutor/fastapi_middlewares",
         keywords=['google-sso', 'fastapi'],
         classifiers= [
             "Development Status :: 3 - Alpha",
```

