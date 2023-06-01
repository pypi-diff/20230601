# Comparing `tmp/wagtail_sb_imageserializer-0.1.0.tar.gz` & `tmp/wagtail_sb_imageserializer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_imageserializer-0.1.0.tar", max compression
+gzip compressed data, was "wagtail_sb_imageserializer-0.2.0.tar", max compression
```

## Comparing `wagtail_sb_imageserializer-0.1.0.tar` & `wagtail_sb_imageserializer-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       96 2023-05-14 23:30:29.022653 wagtail_sb_imageserializer-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-05-13 23:44:11.385632 wagtail_sb_imageserializer-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1676 2023-05-14 20:18:58.379286 wagtail_sb_imageserializer-0.1.0/README.md
--rw-r--r--   0        0        0     2004 2023-05-14 23:30:29.014653 wagtail_sb_imageserializer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       88 2023-05-14 13:40:32.950259 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/admin.py
--rw-r--r--   0        0        0        0 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/api/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/api/fields.py
--rw-r--r--   0        0        0      182 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/apps.py
--rw-r--r--   0        0        0        0 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/models.py
--rw-r--r--   0        0        0        0 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/tests.py
--rw-r--r--   0        0        0       20 2023-05-14 23:30:29.026653 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/version.py
--rw-r--r--   0        0        0        0 2023-05-13 23:55:56.374468 wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/views.py
--rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 wagtail_sb_imageserializer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      166 2023-06-01 04:52:35.471837 wagtail_sb_imageserializer-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-05-14 23:31:08.874809 wagtail_sb_imageserializer-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1794 2023-06-01 04:52:29.051818 wagtail_sb_imageserializer-0.2.0/README.md
+-rw-r--r--   0        0        0     2034 2023-06-01 04:52:35.471837 wagtail_sb_imageserializer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/admin.py
+-rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/api/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/api/fields.py
+-rw-r--r--   0        0        0      182 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/apps.py
+-rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/models.py
+-rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/tests.py
+-rw-r--r--   0        0        0       20 2023-06-01 04:52:35.471837 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/version.py
+-rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/views.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 wagtail_sb_imageserializer-0.2.0/PKG-INFO
```

### Comparing `wagtail_sb_imageserializer-0.1.0/LICENSE.txt` & `wagtail_sb_imageserializer-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_imageserializer-0.1.0/README.md` & `wagtail_sb_imageserializer-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 Wagtail package to render images with rendition in a single API Field.
 
 ## Requirements
 
 - Python 3.8.1 or higher
 - Django lower than 4.0
 - Wagtail lower than 6.0
+- Django Rest Framework lower than 4.0
 
 ## Install
 
 ```bash
 pip install wagtail-sb-imageserializer
 ```
 
 ## Usage
 
-Add `wagtail_sb_imageserializer` to your `INSTALLED_APPS` settings
+Add `wagtail.api.v2`, `rest_framework` and `wagtail_sb_imageserializer` to your `INSTALLED_APPS` settings
 
 ```
 INSTALLED_APPS = [
   # ...
+  "wagtail.api.v2",
+  "rest_framework",
   "wagtail_sb_imageserializer",
   # ...
 ]
 ```
 
 ## Docs
```

### Comparing `wagtail_sb_imageserializer-0.1.0/pyproject.toml` & `wagtail_sb_imageserializer-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtail-sb-imageserializer"
-version = "0.1.0"
+version = "0.2.0"
 description = "Social Networks settings for wagtail sites."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -28,22 +28,23 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.1.0/wagtail-sb-imageserializer-v0.1.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.2.0/wagtail-sb-imageserializer-v0.2.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">= 3.8.1, < 4.0.0"
 Django = "< 5.0"
 wagtail = "< 6.0"
+djangorestframework = "< 4.0"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
 bandit = "^1.7.4"
 black = "^23.1.0"
 coverage = "^7.1.0"
 flake8 = "^6.0.0"
```

### Comparing `wagtail_sb_imageserializer-0.1.0/src/wagtail_sb_imageserializer/api/fields.py` & `wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/api/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_imageserializer-0.1.0/PKG-INFO` & `wagtail_sb_imageserializer-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-sb-imageserializer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Social Networks settings for wagtail sites.
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -18,18 +18,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (<5.0)
+Requires-Dist: djangorestframework (<4.0)
 Requires-Dist: wagtail (<6.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.1.0/wagtail-sb-imageserializer-v0.1.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.2.0/wagtail-sb-imageserializer-v0.2.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-imageserializer)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-imageserializer)
@@ -43,28 +44,31 @@
 Wagtail package to render images with rendition in a single API Field.
 
 ## Requirements
 
 - Python 3.8.1 or higher
 - Django lower than 4.0
 - Wagtail lower than 6.0
+- Django Rest Framework lower than 4.0
 
 ## Install
 
 ```bash
 pip install wagtail-sb-imageserializer
 ```
 
 ## Usage
 
-Add `wagtail_sb_imageserializer` to your `INSTALLED_APPS` settings
+Add `wagtail.api.v2`, `rest_framework` and `wagtail_sb_imageserializer` to your `INSTALLED_APPS` settings
 
 ```
 INSTALLED_APPS = [
   # ...
+  "wagtail.api.v2",
+  "rest_framework",
   "wagtail_sb_imageserializer",
   # ...
 ]
 ```
 
 ## Docs
```

