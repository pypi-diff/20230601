# Comparing `tmp/jupyternb-setup-1.3.4rc0.tar.gz` & `tmp/jupyternb-setup-1.3.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyternb-setup-1.3.4rc0.tar", last modified: Thu Jun  1 18:13:29 2023, max compression
+gzip compressed data, was "jupyternb-setup-1.3.4rc1.tar", last modified: Thu Jun  1 18:16:27 2023, max compression
```

## Comparing `jupyternb-setup-1.3.4rc0.tar` & `jupyternb-setup-1.3.4rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1806 2023-06-01 18:13:01.086115 jupyternb-setup-1.3.4rc0/.gitignore
--rw-r--r--   0        0        0     1071 2023-06-01 17:22:55.849765 jupyternb-setup-1.3.4rc0/LICENSE
--rw-r--r--   0        0        0     4667 2023-06-01 17:22:55.850054 jupyternb-setup-1.3.4rc0/README.md
--rw-r--r--   0        0        0       51 2023-06-01 18:11:25.482299 jupyternb-setup-1.3.4rc0/jupyternb/__init__.py
--rw-r--r--   0        0        0    15308 2023-06-01 18:04:49.632842 jupyternb-setup-1.3.4rc0/jupyternb/jupyter_startup.py
--rw-r--r--   0        0        0      900 2023-06-01 18:10:11.994084 jupyternb-setup-1.3.4rc0/pyproject.toml
--rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.4rc0/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-06-01 18:13:01.086115 jupyternb-setup-1.3.4rc1/.gitignore
+-rw-r--r--   0        0        0     1071 2023-06-01 17:22:55.849765 jupyternb-setup-1.3.4rc1/LICENSE
+-rw-r--r--   0        0        0     4667 2023-06-01 17:22:55.850054 jupyternb-setup-1.3.4rc1/README.md
+-rw-r--r--   0        0        0       51 2023-06-01 18:16:04.582303 jupyternb-setup-1.3.4rc1/jupyternb/__init__.py
+-rw-r--r--   0        0        0    15308 2023-06-01 18:04:49.632842 jupyternb-setup-1.3.4rc1/jupyternb/jupyter_startup.py
+-rw-r--r--   0        0        0      961 2023-06-01 18:16:00.357747 jupyternb-setup-1.3.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.4rc1/PKG-INFO
```

### Comparing `jupyternb-setup-1.3.4rc0/.gitignore` & `jupyternb-setup-1.3.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc0/LICENSE` & `jupyternb-setup-1.3.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc0/README.md` & `jupyternb-setup-1.3.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc0/jupyternb/jupyter_startup.py` & `jupyternb-setup-1.3.4rc1/jupyternb/jupyter_startup.py`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc0/pyproject.toml` & `jupyternb-setup-1.3.4rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
                "License :: OSI Approved :: MIT License",
                "Operating System :: OS Independent"]
 description = "Fabric Jupyter Notebook Container Setup"
 dynamic = ["version"]
 
 keywords = ["Fabric Jupyter Notebook Container Setup", "Jupyter Hub", "Jupyter Notebook"]
 
+scripts = {"jupyter-startup" = "jupyternb.jupyter_startup"}
+
 requires-python = '>=3.9'
 dependencies = ["nbgitpuller",
                 "fabric_fss_utils",
                 "atomicwrites",
                 "gitpython",
                 "wget"]
```

### Comparing `jupyternb-setup-1.3.4rc0/PKG-INFO` & `jupyternb-setup-1.3.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyternb-setup
-Version: 1.3.4rc0
+Version: 1.3.4rc1
 Summary: Fabric Jupyter Notebook Container Setup
 Keywords: Fabric Jupyter Notebook Container Setup,Jupyter Hub,Jupyter Notebook
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

