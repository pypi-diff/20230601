# Comparing `tmp/cloudservices_arg-0.1.1.tar.gz` & `tmp/cloudservices_arg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudservices_arg-0.1.1.tar", last modified: Thu Jun  1 14:52:02 2023, max compression
+gzip compressed data, was "cloudservices_arg-0.1.2.tar", last modified: Thu Jun  1 15:05:21 2023, max compression
```

## Comparing `cloudservices_arg-0.1.1.tar` & `cloudservices_arg-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:52:02.308726 cloudservices_arg-0.1.1/
--rw-rw-rw-   0        0        0      562 2023-06-01 14:52:02.307228 cloudservices_arg-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 14:52:02.304062 cloudservices_arg-0.1.1/cloudservices_arg.egg-info/
--rw-rw-rw-   0        0        0      562 2023-06-01 14:52:01.000000 cloudservices_arg-0.1.1/cloudservices_arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-06-01 14:52:02.000000 cloudservices_arg-0.1.1/cloudservices_arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:52:01.000000 cloudservices_arg-0.1.1/cloudservices_arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-06-01 14:52:01.000000 cloudservices_arg-0.1.1/cloudservices_arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-01 14:52:01.000000 cloudservices_arg-0.1.1/cloudservices_arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 14:52:02.308726 cloudservices_arg-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-01 14:51:43.000000 cloudservices_arg-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:05:21.736401 cloudservices_arg-0.1.2/
+-rw-rw-rw-   0        0        0      562 2023-06-01 15:05:21.734403 cloudservices_arg-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 15:05:21.569301 cloudservices_arg-0.1.2/cloudservices_arg/
+-rw-rw-rw-   0        0        0      102 2023-06-01 15:02:44.000000 cloudservices_arg-0.1.2/cloudservices_arg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:05:21.730872 cloudservices_arg-0.1.2/cloudservices_arg.egg-info/
+-rw-rw-rw-   0        0        0      562 2023-06-01 15:05:21.000000 cloudservices_arg-0.1.2/cloudservices_arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-06-01 15:05:21.000000 cloudservices_arg-0.1.2/cloudservices_arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 15:05:21.000000 cloudservices_arg-0.1.2/cloudservices_arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2023-06-01 15:05:21.000000 cloudservices_arg-0.1.2/cloudservices_arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 15:05:21.000000 cloudservices_arg-0.1.2/cloudservices_arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 15:05:21.736401 cloudservices_arg-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-01 15:05:03.000000 cloudservices_arg-0.1.2/setup.py
```

### Comparing `cloudservices_arg-0.1.1/PKG-INFO` & `cloudservices_arg-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudservices_arg
-Version: 0.1.1
+Version: 0.1.2
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudservices_arg-0.1.1/cloudservices_arg.egg-info/PKG-INFO` & `cloudservices_arg-0.1.2/cloudservices_arg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudservices-arg
-Version: 0.1.1
+Version: 0.1.2
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudservices_arg-0.1.1/setup.py` & `cloudservices_arg-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='cloudservices_arg',
-    version='0.1.1',
+    version='0.1.2',
     description='A sample Python project for rach pack',
     author='Rac',
     author_email='rachitmahajan6399@gmail.com',
     url='https://github.com/r-mhjn/QuizCreator',
     packages=['cloudservices_arg'],
     install_requires=['google-auth==2.17.3','google-cloud-pubsub==2.13.0','boto3==1.14.60','botocore==1.17.60','apache-libcloud==3.7.0','PyPubSub==4.0.3'],
     classifiers=[
```

