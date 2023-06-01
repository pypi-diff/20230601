# Comparing `tmp/docrobot-1.0.3.tar.gz` & `tmp/docrobot-1.0.4.tar.gz`

## Comparing `docrobot-1.0.3.tar` & `docrobot-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.3/convert.ps1
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 docrobot-1.0.3/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/form.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/form.ui
--rw-r--r--   0        0        0    10924 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/util.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 docrobot-1.0.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.3/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.3/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.4/convert.ps1
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 docrobot-1.0.4/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/form.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/form.ui
+-rw-r--r--   0        0        0    19111 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 docrobot-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.4/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.4/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.4/PKG-INFO
```

### Comparing `docrobot-1.0.3/.github/workflows/python-publish.yml` & `docrobot-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.3/src/docrobot/form.py` & `docrobot-1.0.4/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.3/src/docrobot/form.ui` & `docrobot-1.0.4/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.3/LICENSE` & `docrobot-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.3/pyproject.toml` & `docrobot-1.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "docrobot"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Xu Hong", email="icehong@gmail.com" },
 ]
 description = "一个文档自动化处理工具"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `docrobot-1.0.3/PKG-INFO` & `docrobot-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.3
+Version: 1.0.4
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

