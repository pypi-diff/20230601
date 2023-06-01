# Comparing `tmp/availabl-cli-0.0.4.tar.gz` & `tmp/availabl-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "availabl-cli-0.0.4.tar", last modified: Tue May 16 15:17:00 2023, max compression
+gzip compressed data, was "availabl-cli-0.0.5.tar", last modified: Thu Jun  1 08:20:45 2023, max compression
```

## Comparing `availabl-cli-0.0.4.tar` & `availabl-cli-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-05-16 15:17:00.258279 availabl-cli-0.0.4/
--rw-r--r--   0 arran      (501) staff       (20)      679 2023-05-16 15:17:00.257313 availabl-cli-0.0.4/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      382 2023-05-16 15:08:53.000000 availabl-cli-0.0.4/README.md
--rw-r--r--   0 arran      (501) staff       (20)     3195 2023-05-16 15:08:28.000000 availabl-cli-0.0.4/availabl.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-05-16 15:17:00.256632 availabl-cli-0.0.4/availabl_cli.egg-info/
--rw-r--r--   0 arran      (501) staff       (20)      679 2023-05-16 15:17:00.000000 availabl-cli-0.0.4/availabl_cli.egg-info/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      248 2023-05-16 15:17:00.000000 availabl-cli-0.0.4/availabl_cli.egg-info/SOURCES.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-05-16 15:17:00.000000 availabl-cli-0.0.4/availabl_cli.egg-info/dependency_links.txt
--rw-r--r--   0 arran      (501) staff       (20)       42 2023-05-16 15:17:00.000000 availabl-cli-0.0.4/availabl_cli.egg-info/entry_points.txt
--rw-r--r--   0 arran      (501) staff       (20)       45 2023-05-16 15:17:00.000000 availabl-cli-0.0.4/availabl_cli.egg-info/requires.txt
--rw-r--r--   0 arran      (501) staff       (20)        9 2023-05-16 15:17:00.000000 availabl-cli-0.0.4/availabl_cli.egg-info/top_level.txt
--rw-r--r--   0 arran      (501) staff       (20)       38 2023-05-16 15:17:00.258409 availabl-cli-0.0.4/setup.cfg
--rw-r--r--   0 arran      (501) staff       (20)      817 2023-05-14 16:14:53.000000 availabl-cli-0.0.4/setup.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-06-01 08:20:45.572280 availabl-cli-0.0.5/
+-rw-r--r--   0 arran      (501) staff       (20)      679 2023-06-01 08:20:45.571793 availabl-cli-0.0.5/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      382 2023-05-16 15:08:53.000000 availabl-cli-0.0.5/README.md
+-rw-r--r--   0 arran      (501) staff       (20)     3176 2023-06-01 08:17:13.000000 availabl-cli-0.0.5/availabl.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-06-01 08:20:45.571142 availabl-cli-0.0.5/availabl_cli.egg-info/
+-rw-r--r--   0 arran      (501) staff       (20)      679 2023-06-01 08:20:45.000000 availabl-cli-0.0.5/availabl_cli.egg-info/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      248 2023-06-01 08:20:45.000000 availabl-cli-0.0.5/availabl_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-06-01 08:20:45.000000 availabl-cli-0.0.5/availabl_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 arran      (501) staff       (20)       42 2023-06-01 08:20:45.000000 availabl-cli-0.0.5/availabl_cli.egg-info/entry_points.txt
+-rw-r--r--   0 arran      (501) staff       (20)       45 2023-06-01 08:20:45.000000 availabl-cli-0.0.5/availabl_cli.egg-info/requires.txt
+-rw-r--r--   0 arran      (501) staff       (20)        9 2023-06-01 08:20:45.000000 availabl-cli-0.0.5/availabl_cli.egg-info/top_level.txt
+-rw-r--r--   0 arran      (501) staff       (20)       38 2023-06-01 08:20:45.572387 availabl-cli-0.0.5/setup.cfg
+-rw-r--r--   0 arran      (501) staff       (20)      817 2023-06-01 08:20:32.000000 availabl-cli-0.0.5/setup.py
```

### Comparing `availabl-cli-0.0.4/PKG-INFO` & `availabl-cli-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: availabl-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: availabl cli tool
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `availabl-cli-0.0.4/availabl.py` & `availabl-cli-0.0.5/availabl.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,16 @@
 
     click.echo('Granting availabl access to telemetry data in : {} {} ...'.format(
         account_id, region))
 
     if not role_arn:
         click.confirm('Confirm the creation of a new IAM role with CloudWatchReadOnlyAccess'.format(
             account_id), abort=True)
-
-    # create a IAM role with the availabl policy
-    iam = session.client('iam')
-    
-    if not role_arn:
+        # create a IAM role with the availabl policy
+        iam = session.client('iam')
         role_arn = create_role(iam)
 
     click.echo('Registering role {} with availabl'.format(role_arn))
 
     headers = {
         'x-request-timestamp': str(round(time.time() * 1000)),
         'x-app-id': app_id,
```

### Comparing `availabl-cli-0.0.4/availabl_cli.egg-info/PKG-INFO` & `availabl-cli-0.0.5/availabl_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: availabl-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: availabl cli tool
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `availabl-cli-0.0.4/setup.py` & `availabl-cli-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 setup(
     name = 'availabl-cli',
-    version = '0.0.4',
+    version = '0.0.5',
     author = 'Arran McCabe',
     author_email = 'arran@availabl.ai',
     description = 'availabl cli tool',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     py_modules = ['availabl'],
     packages = find_packages(),
```

