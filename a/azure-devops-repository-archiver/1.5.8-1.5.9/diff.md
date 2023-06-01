# Comparing `tmp/azure-devops-repository-archiver-1.5.8.tar.gz` & `tmp/azure-devops-repository-archiver-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-devops-repository-archiver-1.5.8.tar", last modified: Mon Apr 10 07:45:11 2023, max compression
+gzip compressed data, was "azure-devops-repository-archiver-1.5.9.tar", last modified: Mon May  1 06:37:36 2023, max compression
```

## Comparing `azure-devops-repository-archiver-1.5.8.tar` & `azure-devops-repository-archiver-1.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:45:11.598773 azure-devops-repository-archiver-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-10 07:45:11.598773 azure-devops-repository-archiver-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:45:11.598773 azure-devops-repository-archiver-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:45:11.598773 azure-devops-repository-archiver-1.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:45:11.598773 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)    21253 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:45:11.598773 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29822 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.5.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:45:00.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:45:11.598773 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-10 07:45:11.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-10 07:45:11.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:45:11.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 07:45:11.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 07:45:11.000000 azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:37:36.051603 azure-devops-repository-archiver-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-01 06:37:36.051603 azure-devops-repository-archiver-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:37:36.051603 azure-devops-repository-archiver-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:37:36.051603 azure-devops-repository-archiver-1.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:37:36.051603 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)    21253 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:37:36.051603 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29904 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.5.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:37:22.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:37:36.051603 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-01 06:37:36.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-01 06:37:36.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:37:36.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 06:37:36.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 06:37:36.000000 azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/top_level.txt
```

### Comparing `azure-devops-repository-archiver-1.5.8/LICENSE` & `azure-devops-repository-archiver-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-devops-repository-archiver-1.5.8/PKG-INFO` & `azure-devops-repository-archiver-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-devops-repository-archiver
-Version: 1.5.8
+Version: 1.5.9
 Summary: Archive Azure DevOps git repositories to AWS S3
 Home-page: https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-devops-repository-archiver-1.5.8/README.md` & `azure-devops-repository-archiver-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `azure-devops-repository-archiver-1.5.8/setup.py` & `azure-devops-repository-archiver-1.5.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "azure-devops-repository-archiver",
-    "version": "1.5.8",
+    "version": "1.5.9",
     "description": "Archive Azure DevOps git repositories to AWS S3",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/azure_s3_repository_archiver.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "azure_devops_repository_archiver",
         "azure_devops_repository_archiver._jsii"
     ],
     "package_data": {
         "azure_devops_repository_archiver._jsii": [
-            "azure-devops-repository-archiver@1.5.8.jsii.tgz"
+            "azure-devops-repository-archiver@1.5.9.jsii.tgz"
         ],
         "azure_devops_repository_archiver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver/__init__.py` & `azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/PKG-INFO` & `azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-devops-repository-archiver
-Version: 1.5.8
+Version: 1.5.9
 Summary: Archive Azure DevOps git repositories to AWS S3
 Home-page: https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-devops-repository-archiver-1.5.8/src/azure_devops_repository_archiver.egg-info/SOURCES.txt` & `azure-devops-repository-archiver-1.5.9/src/azure_devops_repository_archiver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/azure_devops_repository_archiver/py.typed
 src/azure_devops_repository_archiver.egg-info/PKG-INFO
 src/azure_devops_repository_archiver.egg-info/SOURCES.txt
 src/azure_devops_repository_archiver.egg-info/dependency_links.txt
 src/azure_devops_repository_archiver.egg-info/requires.txt
 src/azure_devops_repository_archiver.egg-info/top_level.txt
 src/azure_devops_repository_archiver/_jsii/__init__.py
-src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.5.8.jsii.tgz
+src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.5.9.jsii.tgz
```

