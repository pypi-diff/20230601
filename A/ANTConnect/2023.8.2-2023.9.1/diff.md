# Comparing `tmp/ANTConnect-2023.8.2.tar.gz` & `tmp/ANTConnect-2023.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ANTConnect-2023.8.2.tar", last modified: Fri May  5 06:48:00 2023, max compression
+gzip compressed data, was "dist\ANTConnect-2023.9.1.tar", last modified: Thu Jun  1 08:30:52 2023, max compression
```

## Comparing `ANTConnect-2023.8.2.tar` & `ANTConnect-2023.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.842904 ANTConnect-2023.8.2/
-drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.836440 ANTConnect-2023.8.2/ANTConnect.egg-info/
--rw-rw-rw-   0        0        0     1274 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1274 2023-05-05 06:48:00.842904 ANTConnect-2023.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      586 2021-06-28 09:19:30.000000 ANTConnect-2023.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.838403 ANTConnect-2023.8.2/antconnect/
--rw-rw-rw-   0        0        0      146 2023-05-05 06:47:15.000000 ANTConnect-2023.8.2/antconnect/__init__.py
--rw-rw-rw-   0        0        0    50894 2023-05-05 06:47:15.000000 ANTConnect-2023.8.2/antconnect/api.py
--rw-rw-rw-   0        0        0      485 2023-05-05 06:48:00.844901 ANTConnect-2023.8.2/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-05-05 06:47:15.000000 ANTConnect-2023.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.841907 ANTConnect-2023.8.2/tests/
--rw-rw-rw-   0        0        0        0 2020-12-10 14:04:13.000000 ANTConnect-2023.8.2/tests/__init__.py
--rw-rw-rw-   0        0        0      102 2020-12-10 14:04:13.000000 ANTConnect-2023.8.2/tests/test_ant.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.989902 ANTConnect-2023.9.1/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.981921 ANTConnect-2023.9.1/ANTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1274 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1274 2023-06-01 08:30:52.989902 ANTConnect-2023.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2021-06-28 09:19:30.000000 ANTConnect-2023.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.984914 ANTConnect-2023.9.1/antconnect/
+-rw-rw-rw-   0        0        0      144 2023-06-01 08:30:50.000000 ANTConnect-2023.9.1/antconnect/__init__.py
+-rw-rw-rw-   0        0        0    50949 2023-06-01 05:52:54.000000 ANTConnect-2023.9.1/antconnect/api.py
+-rw-rw-rw-   0        0        0      484 2023-06-01 08:30:52.992409 ANTConnect-2023.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-06-01 08:30:31.000000 ANTConnect-2023.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.987906 ANTConnect-2023.9.1/tests/
+-rw-rw-rw-   0        0        0        0 2020-12-10 14:04:13.000000 ANTConnect-2023.9.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      102 2020-12-10 14:04:13.000000 ANTConnect-2023.9.1/tests/test_ant.py
```

### Comparing `ANTConnect-2023.8.2/ANTConnect.egg-info/PKG-INFO` & `ANTConnect-2023.9.1/ANTConnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.8.2
+Version: 2023.9.1
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
 License: UNKNOWN
 Description: # ANTConnect
```

### Comparing `ANTConnect-2023.8.2/PKG-INFO` & `ANTConnect-2023.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.8.2
+Version: 2023.9.1
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
 License: UNKNOWN
 Description: # ANTConnect
```

### Comparing `ANTConnect-2023.8.2/README.md` & `ANTConnect-2023.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ANTConnect-2023.8.2/antconnect/api.py` & `ANTConnect-2023.9.1/antconnect/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -800,26 +800,27 @@
         if user != "":
             filters.append({"column": "assigned_to", "operator": "=", "values": [user]})
         return self._make_api_request(path, 'POST', {
             "advanced_filters": filters
         })
 
     def task_create(self, project_id: str, name: str, description: str, status: str, due_date: str, assigned_user: str,
-                    start_date: str = "", appendix: object = {}, license: str = "", end_date: str = "") -> dict:
+                    start_date: str = "", appendix: object = {}, license: str = "", end_date: str = "", priority="normal") -> dict:
         """ Create a task in a project """
-        path = 'task-create'
+        path = 'tasks-create'
         license = selectLicense(license, self._licenses)
         depreciationMessage("param", "status", "01-02-2023", "taken")
         body = {
             # required
             "license": license,
             "project": project_id,
             "title": name,
             "assigned_to": assigned_user,
             "due": due_date,
+            "priority": priority,
 
             # optional
             "description": description,
             "planned_start": start_date,
             "planned_end": end_date,
         }
         if appendix != {}:
```

### Comparing `ANTConnect-2023.8.2/setup.py` & `ANTConnect-2023.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ANTConnect", # Replace with your own username
-    version="2023.8.2",
+    version="2023.9.1",
     author="ANT CDE",
     author_email="info@antcde.io",
     description="Python SDK for ANT Common Data Engineering",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://antcde.io",
     packages=setuptools.find_packages(),
```

