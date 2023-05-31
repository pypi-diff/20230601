# Comparing `tmp/datawrapper-0.5.1.tar.gz` & `tmp/datawrapper-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawrapper-0.5.1.tar", last modified: Wed May 24 23:35:15 2023, max compression
+gzip compressed data, was "datawrapper-0.5.2.tar", last modified: Wed May 31 22:45:01 2023, max compression
```

## Comparing `datawrapper-0.5.1.tar` & `datawrapper-0.5.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.236102 datawrapper-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.228102 datawrapper-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/.stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.228102 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.228102 datawrapper-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-24 23:34:57.000000 datawrapper-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-24 23:34:57.000000 datawrapper-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-24 23:34:57.000000 datawrapper-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-24 23:34:57.000000 datawrapper-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-24 23:35:15.236102 datawrapper-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-24 23:34:57.000000 datawrapper-0.5.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    66724 2023-05-24 23:34:57.000000 datawrapper-0.5.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-24 23:34:57.000000 datawrapper-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-24 23:34:57.000000 datawrapper-0.5.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/datawrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 23:34:57.000000 datawrapper-0.5.1/datawrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23015 2023-05-24 23:34:57.000000 datawrapper-0.5.1/datawrapper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 23:34:57.000000 datawrapper-0.5.1/datawrapper/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/datawrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 23:35:15.000000 datawrapper-0.5.1/datawrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/_templates/class.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/about/history.md
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/static/datawrapper_logo_light.png
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/static/datawrapper_logo_light_small.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.232102 datawrapper-0.5.1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/user-guide/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)   117469 2023-05-24 23:34:57.000000 datawrapper-0.5.1/docs/user-guide/usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 23:35:15.236102 datawrapper-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-24 23:34:57.000000 datawrapper-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.224102 datawrapper-0.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:35:15.236102 datawrapper-0.5.1/tests/test_example/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-24 23:34:57.000000 datawrapper-0.5.1/tests/test_example/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/.stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-31 22:44:48.000000 datawrapper-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-31 22:44:48.000000 datawrapper-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-31 22:44:48.000000 datawrapper-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-31 22:45:01.277543 datawrapper-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 22:44:48.000000 datawrapper-0.5.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    66724 2023-05-31 22:44:48.000000 datawrapper-0.5.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-31 22:44:48.000000 datawrapper-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-31 22:44:48.000000 datawrapper-0.5.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/datawrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 22:44:48.000000 datawrapper-0.5.2/datawrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-31 22:44:48.000000 datawrapper-0.5.2/datawrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 22:44:48.000000 datawrapper-0.5.2/datawrapper/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/datawrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/_templates/class.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/static/datawrapper_logo_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/static/datawrapper_logo_light_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/user-guide/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)   117469 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/user-guide/usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 22:45:01.277543 datawrapper-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-31 22:44:48.000000 datawrapper-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.269543 datawrapper-0.5.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/tests/test_example/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 22:44:48.000000 datawrapper-0.5.2/tests/test_example/test_hello.py
```

### Comparing `datawrapper-0.5.1/.github/.stale.yml` & `datawrapper-0.5.2/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `datawrapper-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `datawrapper-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/.github/PULL_REQUEST_TEMPLATE.md` & `datawrapper-0.5.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/.github/dependabot.yml` & `datawrapper-0.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/.github/workflows/continuous-deployment.yml` & `datawrapper-0.5.2/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/.gitignore` & `datawrapper-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/.pre-commit-config.yaml` & `datawrapper-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/CODE_OF_CONDUCT.md` & `datawrapper-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/CONTRIBUTING.md` & `datawrapper-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/LICENSE` & `datawrapper-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/Pipfile.lock` & `datawrapper-0.5.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/SECURITY.md` & `datawrapper-0.5.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/datawrapper/__init__.py` & `datawrapper-0.5.2/datawrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/datawrapper/__main__.py` & `datawrapper-0.5.2/datawrapper/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,14 +470,15 @@
         unit: str = "px",
         mode: str = "rgb",
         width: int = 400,
         plain: bool = False,
         zoom: int = 2,
         scale: int = 1,
         border_width: int = 20,
+        transparent: bool = False,
         output: str = "png",
         filepath: str = "./image.png",
         display: bool = False,
     ) -> Union[Any, None]:
         """Exports a chart, table, or map.
 
         Parameters
@@ -494,14 +495,16 @@
             Defines if only the visualization should be exported (True), or if it should include header and footer as well (False), by default False
         zoom : int, optional
             Defines the multiplier for the png size, by default 2
         scale : int, optional
             Defines the multiplier for the pdf size, by default 1
         border_width : int, optional
             Margin arouund the visualization, by default 20
+        transparent : bool, optional
+            Set to `True` to export your visualization with a transparent background.
         output : str, optional
             One of png, pdf, or svg, by default "png"
         filepath : str, optional
             Name/filepath to save output in, by default "./image.png"
         display : bool, optional
             Whether to display the exported image as output in the notebook cell, by default False
 
@@ -519,14 +522,15 @@
             "unit": unit,
             "mode": mode,
             "width": width,
             "plain": _plain,
             "zoom": zoom,
             "scale": scale,
             "borderWidth": border_width,
+            "transparent": transparent
         }
 
         _header = self._auth_header
         _header["accept"] = "*/*"
 
         export_chart_response = r.get(
             url=_export_url, headers=_header, params=querystring  # type: ignore
```

### Comparing `datawrapper-0.5.1/datawrapper.egg-info/SOURCES.txt` & `datawrapper-0.5.2/datawrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/docs/Makefile` & `datawrapper-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/docs/conf.py` & `datawrapper-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/docs/make.bat` & `datawrapper-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/docs/static/datawrapper_logo_light.png` & `datawrapper-0.5.2/docs/static/datawrapper_logo_light.png`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/docs/static/datawrapper_logo_light_small.png` & `datawrapper-0.5.2/docs/static/datawrapper_logo_light_small.png`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/docs/user-guide/installation.md` & `datawrapper-0.5.2/docs/user-guide/installation.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/docs/user-guide/usage.ipynb` & `datawrapper-0.5.2/docs/user-guide/usage.ipynb`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/setup.py` & `datawrapper-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.1/tests/test_example/test_hello.py` & `datawrapper-0.5.2/tests/test_example/test_hello.py`

 * *Files identical despite different names*

