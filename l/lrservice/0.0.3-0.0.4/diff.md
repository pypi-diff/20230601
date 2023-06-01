# Comparing `tmp/lrservice-0.0.3.tar.gz` & `tmp/lrservice-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lrservice-0.0.3.tar", last modified: Tue May 30 05:49:10 2023, max compression
+gzip compressed data, was "lrservice-0.0.4.tar", last modified: Thu Jun  1 06:30:52 2023, max compression
```

## Comparing `lrservice-0.0.3.tar` & `lrservice-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,20 @@
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 05:49:10.232677 lrservice-0.0.3/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      534 2023-05-30 05:49:10.232385 lrservice-0.0.3/PKG-INFO
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 05:49:10.231239 lrservice-0.0.3/lrservice.egg-info/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      534 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/PKG-INFO
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      182 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/SOURCES.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)        1 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/dependency_links.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)        6 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/top_level.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)       38 2023-05-30 05:49:10.232760 lrservice-0.0.3/setup.cfg
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 05:49:10.231979 lrservice-0.0.3/tests/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 04:43:02.000000 lrservice-0.0.3/tests/__init__.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      587 2023-05-30 05:01:17.000000 lrservice-0.0.3/tests/test_simple_linear_regr.py
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-06-01 06:30:52.418013 lrservice-0.0.4/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1054 2023-05-29 14:57:14.000000 lrservice-0.0.4/LICENSE
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      556 2023-06-01 06:30:52.417752 lrservice-0.0.4/PKG-INFO
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      180 2023-05-31 16:08:21.000000 lrservice-0.0.4/README.md
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-06-01 06:30:52.413900 lrservice-0.0.4/lrservice/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      221 2023-06-01 06:17:07.000000 lrservice-0.0.4/lrservice/__init__.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1363 2022-02-16 23:54:46.000000 lrservice-0.0.4/lrservice/benchmark.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1986 2023-06-01 05:21:11.000000 lrservice-0.0.4/lrservice/main.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     3426 2023-06-01 06:14:16.000000 lrservice-0.0.4/lrservice/simple_linear_regr.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1840 2023-05-29 15:36:07.000000 lrservice-0.0.4/lrservice/simple_linear_regr_utils.py
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-06-01 06:30:52.417171 lrservice-0.0.4/lrservice/tests/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 04:43:02.000000 lrservice-0.0.4/lrservice/tests/__init__.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      585 2023-06-01 06:16:39.000000 lrservice-0.0.4/lrservice/tests/test_simple_linear_regr.py
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-06-01 06:30:52.416039 lrservice-0.0.4/lrservice.egg-info/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      556 2023-06-01 06:30:52.000000 lrservice-0.0.4/lrservice.egg-info/PKG-INFO
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      362 2023-06-01 06:30:52.000000 lrservice-0.0.4/lrservice.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)        1 2023-06-01 06:30:52.000000 lrservice-0.0.4/lrservice.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)       10 2023-06-01 06:30:52.000000 lrservice-0.0.4/lrservice.egg-info/top_level.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)       38 2023-06-01 06:30:52.418114 lrservice-0.0.4/setup.cfg
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      790 2023-06-01 06:28:35.000000 lrservice-0.0.4/setup.py
```

### Comparing `lrservice-0.0.3/PKG-INFO` & `lrservice-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: lrservice
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for demonstrating how to make REST API service for linear regression
 Home-page: https://github.com/CyberPlayerOne/lrservice
 Author: Tyler Tang
 Author-email: tyler.x.tang@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 A python package for demonstrating how to make REST API service for linear regression
```

### Comparing `lrservice-0.0.3/lrservice.egg-info/PKG-INFO` & `lrservice-0.0.4/lrservice.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: lrservice
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for demonstrating how to make REST API service for linear regression
 Home-page: https://github.com/CyberPlayerOne/lrservice
 Author: Tyler Tang
 Author-email: tyler.x.tang@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 A python package for demonstrating how to make REST API service for linear regression
```

