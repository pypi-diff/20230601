# Comparing `tmp/slack_approval-0.1.2.tar.gz` & `tmp/slack_approval-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_approval-0.1.2.tar", last modified: Tue May 16 17:38:19 2023, max compression
+gzip compressed data, was "slack_approval-0.1.3.tar", last modified: Thu Jun  1 16:09:44 2023, max compression
```

## Comparing `slack_approval-0.1.2.tar` & `slack_approval-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:38:19.532882 slack_approval-0.1.2/
--rw-r--r--   0 austen.novis   (502) staff       (20)     4910 2023-05-16 17:38:19.532754 slack_approval-0.1.2/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)     4079 2023-05-16 17:36:53.000000 slack_approval-0.1.2/README.md
--rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-05-16 17:38:19.532934 slack_approval-0.1.2/setup.cfg
--rw-r--r--   0 austen.novis   (502) staff       (20)     2826 2023-05-16 17:38:16.000000 slack_approval-0.1.2/setup.py
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:38:19.531652 slack_approval-0.1.2/slack_approval/
--rw-r--r--   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/__init__.py
--rw-r--r--   0 austen.novis   (502) staff       (20)      293 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/cli.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     3881 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/slack_provision.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     4430 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/slack_request.py
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:38:19.532552 slack_approval-0.1.2/slack_approval.egg-info/
--rw-r--r--   0 austen.novis   (502) staff       (20)     4910 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)      363 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/SOURCES.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/dependency_links.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       59 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/entry_points.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       36 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/requires.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       15 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/top_level.txt
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-06-01 16:09:44.964992 slack_approval-0.1.3/
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4910 2023-06-01 16:09:44.964825 slack_approval-0.1.3/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4079 2023-05-16 17:36:53.000000 slack_approval-0.1.3/README.md
+-rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-06-01 16:09:44.965051 slack_approval-0.1.3/setup.cfg
+-rw-r--r--   0 austen.novis   (502) staff       (20)     2826 2023-06-01 16:09:38.000000 slack_approval-0.1.3/setup.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-06-01 16:09:44.962807 slack_approval-0.1.3/slack_approval/
+-rw-r--r--   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:36:53.000000 slack_approval-0.1.3/slack_approval/__init__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)      293 2023-05-16 17:36:53.000000 slack_approval-0.1.3/slack_approval/cli.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3951 2023-06-01 16:08:57.000000 slack_approval-0.1.3/slack_approval/slack_provision.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4430 2023-05-16 17:36:53.000000 slack_approval-0.1.3/slack_approval/slack_request.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-06-01 16:09:44.964568 slack_approval-0.1.3/slack_approval.egg-info/
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4910 2023-06-01 16:09:44.000000 slack_approval-0.1.3/slack_approval.egg-info/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)      363 2023-06-01 16:09:44.000000 slack_approval-0.1.3/slack_approval.egg-info/SOURCES.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-06-01 16:09:44.000000 slack_approval-0.1.3/slack_approval.egg-info/dependency_links.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       59 2023-06-01 16:09:44.000000 slack_approval-0.1.3/slack_approval.egg-info/entry_points.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       36 2023-06-01 16:09:44.000000 slack_approval-0.1.3/slack_approval.egg-info/requires.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       15 2023-06-01 16:09:44.000000 slack_approval-0.1.3/slack_approval.egg-info/top_level.txt
```

### Comparing `slack_approval-0.1.2/PKG-INFO` & `slack_approval-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack_approval
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library for managing and deploying a lightweight approval workflow based on Slack and GCP
 Home-page: https://github.com/premisedata/slack-approval
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `slack_approval-0.1.2/README.md` & `slack_approval-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `slack_approval-0.1.2/setup.py` & `slack_approval-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    version="0.1.2",
+    version="0.1.3",
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `slack_approval-0.1.2/slack_approval/slack_provision.py` & `slack_approval-0.1.3/slack_approval/slack_provision.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         self.headers = request.headers
         payload = json.loads(request.form["payload"])
         action = payload["actions"][0]
         self.action_id = action["action_id"]
         self.inputs = json.loads(action["value"])
         self.ts = self.inputs.pop("ts")
         self.requesters_channel = self.inputs.pop("requesters_channel")
+        self.approvers_channel = self.inputs.pop("approvers_channel")
         self.name = self.inputs["provision_class"]
         self.user = " ".join(
             [s.capitalize() for s in payload["user"]["name"].split(".")]
         )
         self.response_url = payload["response_url"]
         self.exception = None
```

### Comparing `slack_approval-0.1.2/slack_approval/slack_request.py` & `slack_approval-0.1.3/slack_approval/slack_request.py`

 * *Files identical despite different names*

### Comparing `slack_approval-0.1.2/slack_approval.egg-info/PKG-INFO` & `slack_approval-0.1.3/slack_approval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-approval
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library for managing and deploying a lightweight approval workflow based on Slack and GCP
 Home-page: https://github.com/premisedata/slack-approval
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

