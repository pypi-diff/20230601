# Comparing `tmp/gitautobackup-1.1.0.2.tar.gz` & `tmp/gitautobackup-1.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitautobackup-1.1.0.2.tar", last modified: Wed May 31 22:13:19 2023, max compression
+gzip compressed data, was "gitautobackup-1.1.0.3.tar", last modified: Thu Jun  1 18:35:01 2023, max compression
```

## Comparing `gitautobackup-1.1.0.2.tar` & `gitautobackup-1.1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:13:19.149360 gitautobackup-1.1.0.2/
--rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.1.0.2/LICENSE
--rw-rw-rw-   0        0        0    44908 2023-05-31 22:13:19.147352 gitautobackup-1.1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6929 2023-05-31 14:45:35.000000 gitautobackup-1.1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:13:19.141354 gitautobackup-1.1.0.2/gitautobackup.egg-info/
--rw-rw-rw-   0        0        0    44908 2023-05-31 22:13:18.000000 gitautobackup-1.1.0.2/gitautobackup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-31 22:13:18.000000 gitautobackup-1.1.0.2/gitautobackup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:13:18.000000 gitautobackup-1.1.0.2/gitautobackup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-05-31 22:13:18.000000 gitautobackup-1.1.0.2/gitautobackup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-05-31 22:13:18.000000 gitautobackup-1.1.0.2/gitautobackup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 22:13:18.000000 gitautobackup-1.1.0.2/gitautobackup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-31 22:13:18.000000 gitautobackup-1.1.0.2/gitautobackup.egg-info/zip-safe
--rw-rw-rw-   0        0        0    16843 2023-05-31 22:12:54.000000 gitautobackup-1.1.0.2/gitautobackup.py
--rw-rw-rw-   0        0        0     2277 2023-05-31 22:01:02.000000 gitautobackup-1.1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 22:13:19.149360 gitautobackup-1.1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 18:35:01.612469 gitautobackup-1.1.0.3/
+-rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    45682 2023-06-01 18:35:01.605926 gitautobackup-1.1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6929 2023-05-31 14:45:35.000000 gitautobackup-1.1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 18:35:01.541103 gitautobackup-1.1.0.3/gitautobackup.egg-info/
+-rw-rw-rw-   0        0        0    45682 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-06-01 18:35:01.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 18:34:59.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    16843 2023-06-01 18:32:58.000000 gitautobackup-1.1.0.3/gitautobackup.py
+-rw-rw-rw-   0        0        0     3198 2023-06-01 18:32:58.000000 gitautobackup-1.1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:35:01.613468 gitautobackup-1.1.0.3/setup.cfg
```

### Comparing `gitautobackup-1.1.0.2/LICENSE` & `gitautobackup-1.1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gitautobackup-1.1.0.2/PKG-INFO` & `gitautobackup-1.1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.1.0.2
+Version: 1.1.0.3
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -378,14 +378,29 @@
           defined by the Mozilla Public License, v. 2.0.
         
 Project-URL: Homepage, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Github, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Issues, https://github.com/MarkusHammer/gitautobackup/issues
 Project-URL: Pull Requests, https://github.com/MarkusHammer/gitautobackup/pulls
 Project-URL: Git, https://github.com/MarkusHammer/gitautobackup.git
+Keywords: backup,git,commit,managment,tool,devtool,small,simple,development,utility
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Typing :: Typed
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: Software Development :: Version Control :: Git
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
 # Git Auto Backup Tool
```

### Comparing `gitautobackup-1.1.0.2/README.md` & `gitautobackup-1.1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gitautobackup-1.1.0.2/gitautobackup.egg-info/PKG-INFO` & `gitautobackup-1.1.0.3/gitautobackup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.1.0.2
+Version: 1.1.0.3
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -378,14 +378,29 @@
           defined by the Mozilla Public License, v. 2.0.
         
 Project-URL: Homepage, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Github, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Issues, https://github.com/MarkusHammer/gitautobackup/issues
 Project-URL: Pull Requests, https://github.com/MarkusHammer/gitautobackup/pulls
 Project-URL: Git, https://github.com/MarkusHammer/gitautobackup.git
+Keywords: backup,git,commit,managment,tool,devtool,small,simple,development,utility
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Typing :: Typed
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: Software Development :: Version Control :: Git
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
 # Git Auto Backup Tool
```

### Comparing `gitautobackup-1.1.0.2/gitautobackup.py` & `gitautobackup-1.1.0.3/gitautobackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from git import Repo, InvalidGitRepositoryError, GitCommandNotFound, NoSuchPathError, RepositoryDirtyError
 
 try:
     from typing import Union
 except ImportError:
     from typing_extensions import Union
 
-__version__ = "1.1.0.2"
+__version__ = "1.1.0.3"
 
 def path_hunt_dir(path: Union[Path, str, None]) -> Union['Path', None]:
     """_summary_
 
     Args:
         path (Union[Path,str,None]): The path to search for the parent directory of. If this is set to None the return value will always also be None
```

