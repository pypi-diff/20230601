# Comparing `tmp/gxabm-2.5.0.tar.gz` & `tmp/gxabm-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.5.0.tar", last modified: Mon May  1 01:44:13 2023, max compression
+gzip compressed data, was "gxabm-2.6.0.tar", last modified: Thu Jun  1 19:09:24 2023, max compression
```

## Comparing `gxabm-2.5.0.tar` & `gxabm-2.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.432145 gxabm-2.5.0/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.5.0/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-05-01 01:44:13.431951 gxabm-2.5.0/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.5.0/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.421832 gxabm-2.5.0/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        5 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.429092 gxabm-2.5.0/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.5.0/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.5.0/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     7552 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.5.0/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.5.0/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.5.0/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.5.0/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    10348 2023-04-29 23:23:52.000000 gxabm-2.5.0/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/invocation.py
--rw-r--r--   0 suderman   (502) staff       (20)     3610 2023-04-29 23:23:52.000000 gxabm-2.5.0/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.5.0/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    12004 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.5.0/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.430218 gxabm-2.5.0/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      691 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-05-01 01:44:13.432272 gxabm-2.5.0/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.5.0/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.431516 gxabm-2.5.0/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.5.0/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.5.0/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.5.0/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.5.0/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.5.0/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.682682 gxabm-2.6.0/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.6.0/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-01 19:09:24.682482 gxabm-2.6.0/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.6.0/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.672317 gxabm-2.6.0/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-01 19:08:42.000000 gxabm-2.6.0/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.6.0/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.679330 gxabm-2.6.0/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-06-01 17:49:27.000000 gxabm-2.6.0/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.6.0/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7552 2023-05-04 19:53:38.000000 gxabm-2.6.0/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.6.0/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6485 2023-06-01 19:08:26.000000 gxabm-2.6.0/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.6.0/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.6.0/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    10348 2023-05-04 19:53:38.000000 gxabm-2.6.0/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.6.0/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4038 2023-06-01 19:08:26.000000 gxabm-2.6.0/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.6.0/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12109 2023-06-01 19:08:26.000000 gxabm-2.6.0/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.6.0/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.6.0/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.680253 gxabm-2.6.0/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-01 19:09:24.682733 gxabm-2.6.0/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.6.0/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.681869 gxabm-2.6.0/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.6.0/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.6.0/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.6.0/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.6.0/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.6.0/test/workflow.py
```

### Comparing `gxabm-2.5.0/PKG-INFO` & `gxabm-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.5.0
+Version: 2.6.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.5.0/README.md` & `gxabm-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/__main__.py` & `gxabm-2.6.0/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/benchmark.py` & `gxabm-2.6.0/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/cloudlaunch.py` & `gxabm-2.6.0/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/common.py` & `gxabm-2.6.0/abm/lib/common.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/config.py` & `gxabm-2.6.0/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/dataset.py` & `gxabm-2.6.0/abm/lib/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     if gi is None:
         gi = connect(context)
     response = gi.tools.put_url(url, history, **kwargs)
     print(json.dumps(response, indent=4))
 
 
 def _import_from_url(gi, history, url, **kwargs):
-    response = gi.tools.put_url(url, history, kwargs)
+    response = gi.tools.put_url(url, history, **kwargs)
     print(json.dumps(response, indent=4))
 
 
 def download(context: Context, args: list):
     gi = connect(context)
     if len(args) == 0:
         print('ERROR: no dataset ID given')
```

### Comparing `gxabm-2.5.0/abm/lib/experiment.py` & `gxabm-2.6.0/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/folder.py` & `gxabm-2.6.0/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/helm.py` & `gxabm-2.6.0/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/history.py` & `gxabm-2.6.0/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/invocation.py` & `gxabm-2.6.0/abm/lib/invocation.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/job.py` & `gxabm-2.6.0/abm/lib/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,29 @@
         print("ERROR: Invalid parameters. Job ID is required")
         return
     gi = connect(context)
     job = gi.jobs.show_job(args[0], full_details=True)
     print(json.dumps(job, indent=4))
 
 
+def wait(context:Context, args: list):
+    if len(args) != 1:
+        print("ERROR: Invalid parameters. Job ID is required")
+        return
+    gi = connect(context)
+    state = "Unknown"
+    waiting = True
+    while waiting:
+        job = gi.jobs.show_job(args[0], full_details=False)
+        state = job["state"]
+        if state == "ok" or state == "error":
+            waiting = False
+    print(json.dumps(job, indent=4))
+
+
 def get_value(metric: dict):
     if metric['name'] == 'runtime_seconds':
         return metric['raw_value']
     return metric['value']
 
 
 def metrics(context: Context, args: list):
```

### Comparing `gxabm-2.5.0/abm/lib/kubectl.py` & `gxabm-2.6.0/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/library.py` & `gxabm-2.6.0/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/menu.yml` & `gxabm-2.6.0/abm/lib/menu.yml`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,18 @@
       help: list common problems that may have caused a job to fail
       handler: job.problems
       params: ID
     - name: [cancel, kill]
       help: kills a job
       handler: job.cancel
       params: ID
+    - name: [wait]
+      help: Wait for a job to finish running
+      handler: job.wait
+      params: ID
     - name: [ metrics, stats ]
       help: display runtime metrics for the job, or a list of jobs contained in a history
       handler: job.metrics
       params: "[ID | -h|--history historyID]"
     - name: [ rerun ]
       handler: job.rerun
       params: JOB_ID
```

### Comparing `gxabm-2.5.0/abm/lib/users.py` & `gxabm-2.6.0/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/abm/lib/workflow.py` & `gxabm-2.6.0/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/gxabm.egg-info/PKG-INFO` & `gxabm-2.6.0/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.5.0
+Version: 2.6.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.5.0/gxabm.egg-info/SOURCES.txt` & `gxabm-2.6.0/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/setup.py` & `gxabm-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/test/check_tools.py` & `gxabm-2.6.0/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.5.0/test/metrics.py` & `gxabm-2.6.0/test/metrics.py`

 * *Files identical despite different names*

