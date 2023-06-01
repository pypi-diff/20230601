# Comparing `tmp/tc_release-0.2.3.tar.gz` & `tmp/tc_release-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc_release-0.2.3.tar", last modified: Tue May 30 20:19:25 2023, max compression
+gzip compressed data, was "tc_release-0.2.4.tar", last modified: Thu Jun  1 00:44:14 2023, max compression
```

## Comparing `tc_release-0.2.3.tar` & `tc_release-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.793781 tc_release-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-30 20:19:06.000000 tc_release-0.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-05-30 20:19:06.000000 tc_release-0.2.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-30 20:19:06.000000 tc_release-0.2.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-30 20:19:06.000000 tc_release-0.2.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-30 20:19:06.000000 tc_release-0.2.3/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-05-30 20:19:06.000000 tc_release-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-30 20:19:06.000000 tc_release-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-30 20:19:06.000000 tc_release-0.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-30 20:19:06.000000 tc_release-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-30 20:19:06.000000 tc_release-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-30 20:19:06.000000 tc_release-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-30 20:19:25.793781 tc_release-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-05-30 20:19:06.000000 tc_release-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-30 20:19:06.000000 tc_release-0.2.3/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 20:19:06.000000 tc_release-0.2.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-05-30 20:19:06.000000 tc_release-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-30 20:19:06.000000 tc_release-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 20:19:25.793781 tc_release-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/tc_release/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    17600 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/tc_release.py
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/tcgvl.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.793781 tc_release-0.2.3/tc_release/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/tests/test_pass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.793781 tc_release-0.2.3/tc_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.234894 tc_release-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-01 00:43:56.000000 tc_release-0.2.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-01 00:43:56.000000 tc_release-0.2.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-01 00:43:56.000000 tc_release-0.2.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-01 00:43:56.000000 tc_release-0.2.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.226894 tc_release-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.230894 tc_release-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-01 00:43:56.000000 tc_release-0.2.4/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-01 00:43:56.000000 tc_release-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-01 00:43:56.000000 tc_release-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-01 00:43:56.000000 tc_release-0.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-06-01 00:43:56.000000 tc_release-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-06-01 00:43:56.000000 tc_release-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-01 00:43:56.000000 tc_release-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-06-01 00:44:14.234894 tc_release-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-01 00:43:56.000000 tc_release-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.230894 tc_release-0.2.4/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-01 00:43:56.000000 tc_release-0.2.4/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-01 00:43:56.000000 tc_release-0.2.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-06-01 00:43:56.000000 tc_release-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-01 00:43:56.000000 tc_release-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 00:44:14.234894 tc_release-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.230894 tc_release-0.2.4/tc_release/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-01 00:44:14.000000 tc_release-0.2.4/tc_release/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18326 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/tc_release.py
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/tcgvl.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.230894 tc_release-0.2.4/tc_release/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.230894 tc_release-0.2.4/tc_release/tests/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/tests/artifacts/artifacts.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4203 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/tests/test_make_release.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-01 00:43:56.000000 tc_release-0.2.4/tc_release/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 00:44:14.230894 tc_release-0.2.4/tc_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-06-01 00:44:14.000000 tc_release-0.2.4/tc_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-01 00:44:14.000000 tc_release-0.2.4/tc_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 00:44:14.000000 tc_release-0.2.4/tc_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-01 00:44:14.000000 tc_release-0.2.4/tc_release.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-01 00:44:14.000000 tc_release-0.2.4/tc_release.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-01 00:44:14.000000 tc_release-0.2.4/tc_release.egg-info/top_level.txt
```

### Comparing `tc_release-0.2.3/.flake8` & `tc_release-0.2.4/.flake8`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/.github/workflows/standard.yml` & `tc_release-0.2.4/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/.gitignore` & `tc_release-0.2.4/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -108,7 +108,11 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# Tests artifacts folder
+tc_release/tests/artifacts/*
+!tc_release/tests/artifacts/artifacts.txt
```

### Comparing `tc_release-0.2.3/.pre-commit-config.yaml` & `tc_release-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/CONTRIBUTING.rst` & `tc_release-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/LICENSE` & `tc_release-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/PKG-INFO` & `tc_release-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc_release
-Version: 0.2.3
+Version: 0.2.4
 Summary: A TwinCAT project release tool
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `tc_release-0.2.3/README.md` & `tc_release-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/conda-recipe/meta.yaml` & `tc_release-0.2.4/conda-recipe/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   - python >=3.9
   - lxml
   - GitPython
 
 test:
   requires:
   - pytest
+  - requests
   imports:
   - tc_release
 
 about:
   home: https://github.com/pcdshub/tc_release
   license: SLAC Open License
   summary: A TwinCAT project release tool
```

### Comparing `tc_release-0.2.3/pyproject.toml` & `tc_release-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/tc_release/tc_release.py` & `tc_release-0.2.4/tc_release/tc_release.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,77 @@
+from __future__ import annotations
+
 import argparse
 import contextlib
 import fnmatch
 import getpass
 import logging
 import os
 import os.path
 import re
 import shutil
 import stat
 import subprocess
 import sys
+import types
+import typing
 import uuid
 
 from lxml import etree
 
 logger = logging.getLogger(__name__)
 
 # Platform-specific setup
-if 'win' in sys.platform:
+if "win" in sys.platform:
     # Set up git env variables
     username = getpass.getuser()
-    git_app_data = 'C:\\Users\\{user}\\AppData\\Local\\Programs\\Git\\'
-    local_git_install = git_app_data.format(user=username)
+    local_git_install = f"C:\\Users\\{username}\\AppData\\Local\\Programs\\Git\\"
 
     if os.path.exists(local_git_install):
-        os.environ['GIT_PYTHON_GIT_EXECUTABLE'] = (local_git_install +
-                                                   'mingw64\\bin\\git.exe')
-        os.environ['GIT_SSH'] = local_git_install + 'usr\\bin\\ssh.exe'
+        os.environ["GIT_PYTHON_GIT_EXECUTABLE"] = (
+            local_git_install + "mingw64\\bin\\git.exe"
+        )
+        os.environ["GIT_SSH"] = local_git_install + "usr\\bin\\ssh.exe"
 
     # Follow windows standard for working directory
-    dirname = '~tc-release-tmp'
+    dirname = "~tc-release-tmp"
 else:
     # Follow linux standard for working directory
-    dirname = '.tc-release-tmp'
+    dirname = ".tc-release-tmp"
 
 # Late import, needs to be after the above on windows
 from git import Repo  # noqa isort:skip
 
-working_dir = os.path.join(os.getcwd(), dirname)
-
-template_file = os.path.join(os.path.dirname(__file__), 'tcgvl.txt')
+template_file = os.path.join(os.path.dirname(__file__), "tcgvl.txt")
 with open(template_file) as fd:
     GlobalVersion_TcGVL = fd.read()
 
 
-def parse_args():
+class TcReleaseArgs(types.SimpleNamespace):
+    version_string: str
+    repo_url: str
+    plcproj: str
+    deploy: bool
+    deploy_path: str
+    dry_run: bool
+    verbose: int
+
+
+def parse_args(args: typing.Sequence[str] | None = None) -> TcReleaseArgs:
     parser = argparse.ArgumentParser(
         description="Properly tags/version your TC project with GIT",
     )
     parser.add_argument(
         "version_string",
         metavar="VERSION_NUMBER",
         type=str,
         help="Version number must be vMAJOR.MINOR.BUGFIX",
     )
     parser.add_argument(
-        "repo_url", type=str,
-        help="URL or path to the repo (for cloning)"
+        "repo_url", type=str, help="URL or path to the repo (for cloning)"
     )
     parser.add_argument(
         "--plcproj",
         default="",
         help=(
             "If multiple PLC projects in the repo, specify which one to set "
             "the version number on."
@@ -100,15 +111,15 @@
         default=0,
         help=(
             "Increase the number of messages shown in the terminal. This "
             "decreases the log level by 10 for each count of -v, starting "
             "at the INFO level (20)."
         ),
     )
-    return parser.parse_args()
+    return parser.parse_args(args=args, namespace=TcReleaseArgs())
 
 
 def find(pattern: str, path: str) -> list[str]:
     """
     Case-insensitive recursive search of ``path`` for ``pattern``.
 
     Parameters
@@ -129,29 +140,29 @@
         for name in files:
             if fnmatch.fnmatch(name.lower(), pattern.lower()):
                 result.append(os.path.join(root, name))
     return result
 
 
 # Workaround for Windows file lock issues
-def remove_readonly(func, path, _):
+def remove_readonly(func: typing.Callable, path: str, _) -> None:
     "Clear the readonly bit and reattempt the removal"
     os.chmod(path, stat.S_IWRITE)
     func(path)
 
 
 @contextlib.contextmanager
-def pushd(new_dir):
+def pushd(new_dir: str) -> typing.Iterator[None]:
     previous_dir = os.getcwd()
     os.chdir(new_dir)
     yield
     os.chdir(previous_dir)
 
 
-def find_makefiles(directory):
+def find_makefiles(directory: str) -> list[str]:
     """
     Find the subdirectories that contain Makefiles.
 
     This will do a depth-first walk of the directory tree, accumulating a
     directory name whenever a file named "Makefile" is found, and pruning the
     search path at these directories to avoid double-counting any
     sub-Makefiles.
@@ -171,29 +182,29 @@
         The highest-level directories that contain files named "Makefile".
     """
     walker = os.walk(directory)
     make_dirs = []
 
     # Find the first Makefile in every branch of the directory tree
     for dirpath, dirnames, filenames in walker:
-        if 'Makefile' in filenames:
+        if "Makefile" in filenames:
             make_dirs.append(dirpath)
             # Stop searching this branch if we found a Makefile
             dirnames.clear()
             continue
         # Skip the version control directory
         try:
-            dirnames.remove('.git')
+            dirnames.remove(".git")
         except ValueError:
             pass
 
     return make_dirs
 
 
-def deploy(repo_url, tag, directory, dry_run):
+def deploy(repo_url: str, tag: str, directory: str, dry_run: bool):
     """
     Clone a repo to a specific directory at a specific tag, then build the IOC
 
     This will find the highest-level Makefile in the directory tree, then
     shell out to call 'make'.
 
     If more than one such file exists, we will make all of them.
@@ -215,326 +226,349 @@
 
     dry_run : bool
         If True, don't actually do anything.
         If False, do things.
     """
     # Clone the repo
     deploy_dir = os.path.join(directory, tag)
-    logger.info(f'Deploying to {deploy_dir}')
+    logger.info(f"Deploying to {deploy_dir}")
     if not dry_run:
         Repo.clone_from(repo_url, deploy_dir, depth=1, branch=tag)
 
     # Find the makefiles
     if not dry_run:
         make_dirs = find_makefiles(deploy_dir)
 
     # Make all the makefiles
     if not dry_run:
         for make_dir in make_dirs:
             with pushd(make_dir):
-                subprocess.run('make')
+                subprocess.run("make")
 
 
-def make_deploy(args):
+def make_deploy(args: TcReleaseArgs):
     if not args.deploy:
         return
     repo_url = args.repo_url
     tag = args.version_string
     dry_run = args.dry_run
-    repo_name = os.path.split(repo_url)[-1].replace('.git', '')
+    repo_name = os.path.split(repo_url)[-1].replace(".git", "")
 
     if args.deploy_path:
         deploy_path = args.deploy_path
     else:
-        epics_site_top = os.environ.get('EPICS_SITE_TOP',
-                                        '/cds/group/pcds/epics')
-        ioc_dir = os.path.join(epics_site_top, 'ioc')
+        epics_site_top = os.environ.get("EPICS_SITE_TOP", "/cds/group/pcds/epics")
+        ioc_dir = os.path.join(epics_site_top, "ioc")
         categories = next(os.walk(ioc_dir))[1]
-        repo_parts = repo_name.split('-')
+        repo_parts = repo_name.split("-")
 
         correct_category = None
         for cat in categories:
             if cat in repo_parts:
                 correct_category = cat
                 break
 
         if correct_category is None:
-            raise RuntimeError('Cannot determine where to deploy IOC')
+            raise RuntimeError("Cannot determine where to deploy IOC")
 
         deploy_path = os.path.join(ioc_dir, correct_category)
 
     if not os.path.isdir(deploy_path):
-        raise RuntimeError(f'{deploy_path} does not exist! '
-                           'Verify you used a valid path!')
+        raise RuntimeError(
+            f"{deploy_path} does not exist! Verify you used a valid path!"
+        )
 
     repo_deploy_path = os.path.join(deploy_path, repo_name)
 
     if not args.dry_run:
         try:
             os.mkdir(repo_deploy_path)
         except FileExistsError:
             pass
 
-    logger.info(f'Deploying {repo_name} to {repo_deploy_path} at {tag}')
+    logger.info(f"Deploying {repo_name} to {repo_deploy_path} at {tag}")
     deploy(repo_url, tag, repo_deploy_path, dry_run)
 
 
-def initialize_repo():
+def initialize_repo(working_dir: str) -> Repo:
     """
     Create the gitpython Repo object for make_release.
 
     This is done separately to simplify the cleanup. The repo object
     must be closed or else the working directory rmtree will fail.
     """
-    logger.info('Creating working directory: %s', working_dir)
-    logger.info('Initializing bare git repo, establishing remote, and '
-                'checking out master')
+    logger.info("Creating working directory: %s", working_dir)
+    logger.info(
+        "Initializing bare git repo, establishing remote, and checking out master"
+    )
     return Repo.init(working_dir)
 
 
-def make_release(args, repo):
+def make_release(
+    repo: Repo,
+    working_dir: str,
+    full_version_string: str,
+    repo_url: str,
+    select_plcproj: str | None = None,
+    dry_run: bool = False,
+):
     """The core tc_release routine for tagging projects."""
     # Create a temp directory, and clone the repo, and check out master
 
-    logger.info('Adding remote')
-    logger.debug('Working directory: %s, Repo: %s',
-                 working_dir, args.repo_url)
-    origin = repo.create_remote('origin', str(args.repo_url))
+    logger.info("Adding remote")
+    logger.debug("Working directory: %s, Repo: %s", working_dir, repo_url)
+    origin = repo.create_remote("origin", str(repo_url))
 
     if not origin.exists():
-        raise RuntimeError('Repo URL does not exist!')
+        raise RuntimeError("Repo URL does not exist!")
 
     origin.fetch()
 
-    repo.create_head('master', origin.refs.master)
+    repo.create_head("master", origin.refs.master)
 
     repo.heads.master.checkout()
 
     repo.heads.master.set_tracking_branch(origin.refs.master)
 
-    if args.version_string in (tag.name for tag in repo.tags):
-        logger.warning(f'Tag {args.version_string} already exists, skipping')
+    if full_version_string in (tag.name for tag in repo.tags):
+        logger.warning(f"Tag {full_version_string} already exists, skipping")
         return
 
     # Check format of version_number
-    projectVersion_pattern = re.compile(r'v([\d.]+)')
-    version_string = re.search(projectVersion_pattern,
-                               args.version_string).group(1)
+    projectVersion_pattern = re.compile(r"v([\d.]+)")
+    version_string = re.search(projectVersion_pattern, full_version_string).group(1)
     if not version_string:
         raise ValueError('Version string does not match format "vX.X.X"')
 
     # Inject version_number into .tcproj
     # Find .tcproj
 
-    logger.info('Looking for .plcproj')
-    plcproj_path = find('*.plcproj', working_dir)
+    logger.info("Looking for .plcproj")
+    plcproj_path = find("*.plcproj", working_dir)
 
     if not len(plcproj_path):
-        raise RuntimeError('Did not find .plcproj file.')
-    elif args.plcproj:
+        raise RuntimeError("Did not find .plcproj file.")
+    elif select_plcproj:
         for i, proj in enumerate(plcproj_path):
-            if args.plcproj == os.path.split(proj)[1].split('.')[0]:
+            if select_plcproj == os.path.split(proj)[1].split(".")[0]:
                 plcproj_file = plcproj_path[i]
                 break
         else:
-            raise RuntimeError('Did not find specified file '
-                               '{}.plcproj'.format(args.plcproj))
+            raise RuntimeError(f"Did not find specified file {select_plcproj}.plcproj")
     elif len(plcproj_path) > 1:
-        raise RuntimeError('Found multiple .plcproj files.')
+        raise RuntimeError("Found multiple .plcproj files.")
     else:
         plcproj_file = plcproj_path[0]
 
     # Getting our xml structure to work with
-    logger.info('Parsing plcproj')
+    logger.info("Parsing plcproj")
     plcproj_tree = etree.parse(plcproj_file)
 
     plcproj_root = plcproj_tree.getroot()
 
     nsmap = plcproj_root.nsmap
 
     # Getting the ProjectVersion, Company, Author and Title tags
-    projectVersion_tag = plcproj_root.find('.//ProjectVersion', nsmap)
+    projectVersion_tag = plcproj_root.find(".//ProjectVersion", nsmap)
     # company_tag and author_tag are currently unused
     # company_tag = plcproj_root.find('.//Company', nsmap)
     # author_tag = plcproj_root.find('.//Author', nsmap)
-    title_tag = plcproj_root.find('.//Title', nsmap)
+    title_tag = plcproj_root.find(".//Title", nsmap)
 
     if None in (projectVersion_tag, title_tag):
-        err = ('Did not find a plc project version tag or a title tag! '
-               'Did you forgot to set the plc project version to 0.0.0 '
-               'or select an appropriate project title in TwinCAT?')
+        err = (
+            "Did not find a plc project version tag or a title tag! "
+            "Did you forgot to set the plc project version to 0.0.0 "
+            "or select an appropriate project title in TwinCAT?"
+        )
         raise RuntimeError(err)
 
-    logger.info('Updating plcproj with version number: %s', version_string)
+    logger.info("Updating plcproj with version number: %s", version_string)
     # Adding version string to plcproj
 
     projectVersion_tag.text = version_string
 
     # To make this verson number available in the PLC runtime,
     # we must add the Version/Global_Version.TcGVL to the project
     # Whether one exists or not, doesn't matter. We always just create one.
     # To start, we need the TC version of the project
     # and the current TcPlcObject version.
     # We can get this info for scanning for a .TcPOU in the project files
     # (there has to be at least one), and extracting these tags
 
-    logger.info('Creating Global_Version.TcGVL')
-    pouFiles = find('*.TcPOU', working_dir)
+    logger.info("Creating Global_Version.TcGVL")
+    pouFiles = find("*.TcPOU", working_dir)
     pouTree = etree.parse(pouFiles[0])
     pouRoot = pouTree.getroot()
 
-    TcPlcObject_PRODUCT_VERSION = pouRoot.get('ProductVersion')
-    TcPlcObject_VERSION = pouRoot.get('Version')
+    TcPlcObject_PRODUCT_VERSION = pouRoot.get("ProductVersion")
+    TcPlcObject_VERSION = pouRoot.get("Version")
 
     GlobalVersion_TcGVL_root = etree.XML(GlobalVersion_TcGVL)
-    GlobalVersion_TcGVL_tree = etree.ElementTree(
-        element=GlobalVersion_TcGVL_root)
+    GlobalVersion_TcGVL_tree = etree.ElementTree(element=GlobalVersion_TcGVL_root)
 
     GlobalVersion_TcGVL_attributes = GlobalVersion_TcGVL_root.attrib
 
-    GlobalVersion_TcGVL_attributes['ProductVersion'] = (
-        TcPlcObject_PRODUCT_VERSION)
-    GlobalVersion_TcGVL_attributes['Version'] = TcPlcObject_VERSION
+    if TcPlcObject_PRODUCT_VERSION is not None:
+        GlobalVersion_TcGVL_attributes["ProductVersion"] = TcPlcObject_PRODUCT_VERSION
+    GlobalVersion_TcGVL_attributes["Version"] = TcPlcObject_VERSION
 
     # We should also change the GUID, just to be nice.
-    gvl_attrib = GlobalVersion_TcGVL_root.find('.//GVL').attrib
+    gvl_attrib = GlobalVersion_TcGVL_root.find(".//GVL").attrib
 
     try:
-        gvl_attrib['Id'] = str(uuid.uuid4())
+        gvl_attrib["Id"] = str(uuid.uuid4())
     except KeyError:
-        raise RuntimeError('Could not find Id attribute in GVL tag')
+        raise RuntimeError("Could not find Id attribute in GVL tag")
 
     # Now we modify the title and version numbers
-    declaration = GlobalVersion_TcGVL_root.find('.//Declaration')
+    declaration = GlobalVersion_TcGVL_root.find(".//Declaration")
     declaration_text = declaration.text
 
-    split_version_string = version_string.split('.')
+    split_version_string = version_string.split(".")
     major = split_version_string[0]
     minor = split_version_string[1]
     build = split_version_string[2]
     if len(split_version_string) > 3:
         revision = split_version_string[4]
     else:
-        revision = '0'
+        revision = "0"
 
-    pattern = re.compile(r"stLibVersion_(?P<title>.+)\s?:\s?ST_LibVersion.+"
-                         r"iMajor.+(?P<major>\d+).+iMinor.+(?P<minor>\d+).+"
-                         r"iBuild.+(?P<build>\d+).*iRevision.+"
-                         r"(?P<revision>\d+).+sVersion.+"
-                         r"'(?P<version_string>.+)'.+;")
-    fmt = ("stLibVersion_{title} : ST_LibVersion := "
-           "(iMajor := {iMajor}, iMinor := {iMinor}, "
-           "iBuild := {iBuild}, iRevision := {iRevision}, "
-           "sVersion := '{sVersion}');")
+    pattern = re.compile(
+        r"stLibVersion_(?P<title>.+)\s?:\s?ST_LibVersion.+"
+        r"iMajor.+(?P<major>\d+).+iMinor.+(?P<minor>\d+).+"
+        r"iBuild.+(?P<build>\d+).*iRevision.+"
+        r"(?P<revision>\d+).+sVersion.+"
+        r"'(?P<version_string>.+)'.+;"
+    )
+    fmt = (
+        "stLibVersion_{title} : ST_LibVersion := "
+        "(iMajor := {iMajor}, iMinor := {iMinor}, "
+        "iBuild := {iBuild}, iRevision := {iRevision}, "
+        "sVersion := '{sVersion}');"
+    )
     replacement_string = fmt.format(
         iMajor=major,
         iMinor=minor,
         iBuild=build,
         iRevision=revision,
         sVersion=version_string,
-        title=str(title_tag.text).replace(' ', '_').replace('-', '_')
+        title=str(title_tag.text).replace(" ", "_").replace("-", "_"),
     )
 
-    declaration.text = etree.CDATA(pattern.sub(replacement_string,
-                                               declaration_text))
+    declaration.text = etree.CDATA(pattern.sub(replacement_string, declaration_text))
     # Note, using the declaration.text not _ to write it back
     # Also note the use of the CDATA wrapper, this is stripped by .text,
     # so we need to restore it.
 
     # Add this file to the project by adding a Version/ folder and
     # Global_Version.TcGVL file and linking in the .tcproj
 
     # Creating file and folder
-    logger.info('Writing Global_Version.TcGVL to file')
-    version_dir = os.path.join(os.path.dirname(plcproj_file), 'Version')
+    logger.info("Writing Global_Version.TcGVL to file")
+    version_dir = os.path.join(os.path.dirname(plcproj_file), "Version")
     os.makedirs(version_dir, exist_ok=True)
-    GV_TcGVL_file = os.path.join(version_dir, 'Global_Version.TcGVL')
+    GV_TcGVL_file = os.path.join(version_dir, "Global_Version.TcGVL")
 
-    GlobalVersion_TcGVL_tree.write(GV_TcGVL_file, encoding='utf-8',
-                                   xml_declaration=True)
-    logger.info('File created successfully: %s', GV_TcGVL_file)
+    GlobalVersion_TcGVL_tree.write(
+        GV_TcGVL_file, encoding="utf-8", xml_declaration=True
+    )
+    logger.info("File created successfully: %s", GV_TcGVL_file)
 
     # Linking in the .plcproj
-    logger.info('Linking Global_Version.TcGVL into plcproj')
+    logger.info("Linking Global_Version.TcGVL into plcproj")
 
     # Check if Version folder is already linked, if not add it
     folder_find = ".//ItemGroup/Folder[@Include='Version']"
     ver_folders = plcproj_root.find(folder_find, nsmap)
     if ver_folders is None or not len(ver_folders):
-        folder = plcproj_root.find('.//ItemGroup/Folder', nsmap)
+        folder = plcproj_root.find(".//ItemGroup/Folder", nsmap)
         folder.addnext(etree.XML('<Folder Include="Version" />'))
 
     # Check if Compile Include if not add it (it better already be there)
-    compile_find = (r'.//ItemGroup/Compile'
-                    r'[@Include="Version\Global_Version.TcGVL"]')
+    compile_find = r".//ItemGroup/Compile" r'[@Include="Version\Global_Version.TcGVL"]'
     ver_compiles = plcproj_root.find(compile_find, nsmap)
     if ver_compiles is None or not len(ver_compiles):
-        compile_include = plcproj_root.find('.//ItemGroup/Compile', nsmap)
-        compile_include.addnext(etree.XML(r'''
+        compile_include = plcproj_root.find(".//ItemGroup/Compile", nsmap)
+        compile_include.addnext(
+            etree.XML(
+                r"""
         <Compile Include="Version\Global_Version.TcGVL">
             <SubType>Code</SubType>
         </Compile>
-        '''))
+        """
+            )
+        )
 
     # Writing new plcproj to disk
-    logger.info('Writing updated .plcproj to file')
-    plcproj_tree.write(plcproj_file, encoding='utf-8', xml_declaration=True)
-    logger.info('.plc project has been updated')
+    logger.info("Writing updated .plcproj to file")
+    plcproj_tree.write(plcproj_file, encoding="utf-8", xml_declaration=True)
+    logger.info(".plc project has been updated")
 
     # Commit changes
     repoIndex = repo.index
     repoIndex.add([GV_TcGVL_file])
     repoIndex.add([plcproj_file])
     repoIndex.write()
 
-    logger.info('Committing changes')
-    commit_message = "Tagging version {version}".format(
-        version=args.version_string)
+    logger.info("Committing changes")
+    commit_message = f"Tagging version {full_version_string}"
     repoIndex.commit(commit_message, skip_hooks=True)
 
     # Tag this commit
-    repo.create_tag(args.version_string, ref='HEAD', message=commit_message)
+    repo.create_tag(full_version_string, ref="HEAD", message=commit_message)
 
     # Push commit
     # --tags is not ideal, but since this is the only tag we're creating
     # in this temp area, it should be safe
-    if args.dry_run:
+    if dry_run:
         pushStatus = None
-        logger.info('Skipping push for dry-run')
+        logger.info("Skipping push for dry-run")
     else:
         pushStatus = origin.push(tags=True)
-        logger.info('Push complete')
+        logger.info("Push complete")
 
     return pushStatus
 
 
-def _main(args, repo):
-    make_release(args, repo)
+def _main(args: TcReleaseArgs, repo: Repo, working_dir: str):
+    make_release(
+        repo=repo,
+        working_dir=working_dir,
+        full_version_string=args.version_string,
+        repo_url=args.repo_url,
+        select_plcproj=args.plcproj,
+        dry_run=args.dry_run,
+    )
     make_deploy(args)
 
 
-def configure_logging(args):
+def configure_logging(args: TcReleaseArgs):
     level = logging.INFO - args.verbose * 10
-    logging.basicConfig(level=level, format='%(levelname)-8s %(message)s')
+    logging.basicConfig(level=level, format="%(levelname)-8s %(message)s")
 
 
-def main():
-    args = parse_args()
+def main(cli_args: TcReleaseArgs | None = None):
+    return_value = 0
+    args = parse_args(args=cli_args)
     configure_logging(args)
-    repo = initialize_repo()
+    working_dir = os.path.join(os.getcwd(), dirname)
+    repo = initialize_repo(working_dir)
     try:
-        _main(args, repo)
+        _main(args=args, repo=repo, working_dir=working_dir)
     except Exception as exc:
         error_msg = exc.args[0]
         logger.debug(error_msg, exc_info=True)
         logger.error(error_msg)
+        return_value = 1
     finally:
         repo.close()
         if args.dry_run:
-            logger.info(f'Skipping cleanup for dry-run: see {working_dir}.')
+            logger.info(f"Skipping cleanup for dry-run: see {working_dir}.")
         else:
-            logger.info('Cleaning up')
+            logger.info("Cleaning up")
             shutil.rmtree(working_dir, onerror=remove_readonly)
+    return return_value
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tc_release-0.2.3/tc_release/tcgvl.txt` & `tc_release-0.2.4/tc_release/tcgvl.txt`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.3/tc_release/version.py` & `tc_release-0.2.4/tc_release/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,42 +18,45 @@
     1. A git checkout (.git exists)
     2. A git archive / a tarball release from GitHub that includes version
         information in .git_archival.txt.
     3. An existing _version.py generated by setuptools_scm
     4. A fallback in case none of the above match - resulting in a version of
         0.0.unknown
     """
+
     def __init__(self):
         self._version = None
 
     def _get_version(self) -> Optional[str]:
         # Checking for directory is faster than failing out of get_version
         repo_root = Path(__file__).resolve().parent.parent
         if (repo_root / ".git").exists() or (repo_root / ".git_archival.txt").exists():
             try:
                 # Git checkout
                 from setuptools_scm import get_version
+
                 return get_version(root="..", relative_to=__file__)
             except (ImportError, LookupError):
                 ...
 
         # Check this second because it can exist in a git repo if we've
         # done a build at least once.
         try:
             from ._version import version  # noqa: F401
+
             return version
         except ImportError:
             ...
 
         return None
 
     @property
     def data(self) -> str:
         # This is accessed by UserString to allow us to lazily fill in the
         # information
         if self._version is None:
-            self._version = self._get_version() or '0.0.unknown'
+            self._version = self._get_version() or "0.0.unknown"
 
         return self._version
 
 
 __version__ = version = VersionProxy()
```

### Comparing `tc_release-0.2.3/tc_release.egg-info/PKG-INFO` & `tc_release-0.2.4/tc_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-release
-Version: 0.2.3
+Version: 0.2.4
 Summary: A TwinCAT project release tool
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `tc_release-0.2.3/tc_release.egg-info/SOURCES.txt` & `tc_release-0.2.4/tc_release.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 tc_release/version.py
 tc_release.egg-info/PKG-INFO
 tc_release.egg-info/SOURCES.txt
 tc_release.egg-info/dependency_links.txt
 tc_release.egg-info/entry_points.txt
 tc_release.egg-info/requires.txt
 tc_release.egg-info/top_level.txt
-tc_release/tests/test_pass.py
+tc_release/tests/__init__.py
+tc_release/tests/test_make_release.py
+tc_release/tests/artifacts/artifacts.txt
```

