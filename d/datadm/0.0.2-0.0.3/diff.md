# Comparing `tmp/datadm-0.0.2.tar.gz` & `tmp/datadm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadm-0.0.2.tar", last modified: Wed May 31 21:31:34 2023, max compression
+gzip compressed data, was "datadm-0.0.3.tar", last modified: Wed May 31 23:42:28 2023, max compression
```

## Comparing `datadm-0.0.2.tar` & `datadm-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:34.357719 datadm-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:34.357719 datadm-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:34.357719 datadm-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-31 21:31:25.000000 datadm-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-31 21:31:25.000000 datadm-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 21:31:25.000000 datadm-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-31 21:31:34.357719 datadm-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 21:31:25.000000 datadm-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:34.357719 datadm-0.0.2/datadm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:25.000000 datadm-0.0.2/datadm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-31 21:31:25.000000 datadm-0.0.2/datadm/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-31 21:31:25.000000 datadm-0.0.2/datadm/repl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:34.357719 datadm-0.0.2/datadm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-31 21:31:34.000000 datadm-0.0.2/datadm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-31 21:31:34.000000 datadm-0.0.2/datadm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:31:34.000000 datadm-0.0.2/datadm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:31:34.000000 datadm-0.0.2/datadm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 21:31:34.000000 datadm-0.0.2/datadm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 21:31:34.000000 datadm-0.0.2/datadm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 21:31:25.000000 datadm-0.0.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-31 21:31:25.000000 datadm-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:31:34.357719 datadm-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:34.357719 datadm-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:31:25.000000 datadm-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-31 21:31:25.000000 datadm-0.0.2/tests/test_repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.342901 datadm-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.330900 datadm-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.334900 datadm-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-31 23:42:16.000000 datadm-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-31 23:42:16.000000 datadm-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-31 23:42:16.000000 datadm-0.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 23:42:16.000000 datadm-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-31 23:42:28.342901 datadm-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 23:42:16.000000 datadm-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.334900 datadm-0.0.3/datadm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:16.000000 datadm-0.0.3/datadm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-05-31 23:42:16.000000 datadm-0.0.3/datadm/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-31 23:42:16.000000 datadm-0.0.3/datadm/repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.338900 datadm-0.0.3/datadm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 23:42:16.000000 datadm-0.0.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-31 23:42:16.000000 datadm-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:42:28.342901 datadm-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.338900 datadm-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:16.000000 datadm-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-31 23:42:16.000000 datadm-0.0.3/tests/test_repl.py
```

### Comparing `datadm-0.0.2/.gitignore` & `datadm-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `datadm-0.0.2/LICENSE` & `datadm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datadm-0.0.2/PKG-INFO` & `datadm-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Chat with your data, personal data assistant, keep your data private with pure local mode, slide into your data's DMs
 License: MIT License
         
         Copyright (c) 2023 Approximate Labs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `datadm-0.0.2/datadm/app.py` & `datadm-0.0.3/datadm/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,10 +268,14 @@
         outputs=None,
         cancels=[submit_event, submit_click_event],
         queue=False,
     )
     clear.click(lambda: (None, []), None, outputs=[chatbot, conversation], queue=False)
 
 
-if __name__ == "__main__":
+def main():
     demo.queue(max_size=128, concurrency_count=1)
-    demo.launch(share=False)
+    demo.launch(share=False)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `datadm-0.0.2/datadm/repl.py` & `datadm-0.0.3/datadm/repl.py`

 * *Files identical despite different names*

### Comparing `datadm-0.0.2/datadm.egg-info/PKG-INFO` & `datadm-0.0.3/datadm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Chat with your data, personal data assistant, keep your data private with pure local mode, slide into your data's DMs
 License: MIT License
         
         Copyright (c) 2023 Approximate Labs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `datadm-0.0.2/pyproject.toml` & `datadm-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "sketch",
     "transformers",
 ]
 urls = {homepage = "https://github.com/approximatelabs/datadm"}
 dynamic = ["version"]
 
 [project.scripts]
-datadm = "datadm:app"
+datadm = "datadm.app:main"
 
 [tool.setuptools_scm]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py38, py39, py310, py311
```

