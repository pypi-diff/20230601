# Comparing `tmp/yao-0.0.5.tar.gz` & `tmp/yao-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.0.5.tar", last modified: Sat May 27 09:16:22 2023, max compression
+gzip compressed data, was "yao-0.0.6.tar", last modified: Thu Jun  1 10:16:59 2023, max compression
```

## Comparing `yao-0.0.5.tar` & `yao-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.079466 yao-0.0.5/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-27 09:16:22.079286 yao-0.0.5/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-05-27 09:16:22.079511 yao-0.0.5/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)      971 2023-05-27 09:06:21.000000 yao-0.0.5/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.073092 yao-0.0.5/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    19302 2023-05-06 07:07:58.000000 yao-0.0.5/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-05-04 09:42:20.000000 yao-0.0.5/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 09:42:20.000000 yao-0.0.5/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.074530 yao-0.0.5/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.075098 yao-0.0.5/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.075644 yao-0.0.5/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.076218 yao-0.0.5/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.076724 yao-0.0.5/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)      992 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.077265 yao-0.0.5/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      665 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.078173 yao-0.0.5/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.078749 yao-0.0.5/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-05-27 08:54:40.000000 yao-0.0.5/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-05-04 09:42:20.000000 yao-0.0.5/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    12051 2023-05-08 03:05:36.000000 yao-0.0.5/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     2062 2023-05-12 09:17:23.000000 yao-0.0.5/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.074075 yao-0.0.5/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      166 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.137529 yao-0.0.6/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-06-01 10:16:59.137302 yao-0.0.6/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2023-06-01 10:16:59.137581 yao-0.0.6/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)      971 2023-06-01 10:15:55.000000 yao-0.0.6/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.130591 yao-0.0.6/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    19302 2023-05-06 07:07:58.000000 yao-0.0.6/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-05-04 09:42:20.000000 yao-0.0.6/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 09:42:20.000000 yao-0.0.6/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.132001 yao-0.0.6/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.132771 yao-0.0.6/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.133430 yao-0.0.6/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.134027 yao-0.0.6/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.135046 yao-0.0.6/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)      992 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.135661 yao-0.0.6/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      665 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.136350 yao-0.0.6/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.137031 yao-0.0.6/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-06-01 10:08:02.000000 yao-0.0.6/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-05-04 09:42:20.000000 yao-0.0.6/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    12834 2023-06-01 10:08:43.000000 yao-0.0.6/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2062 2023-05-12 09:17:23.000000 yao-0.0.6/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.131371 yao-0.0.6/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      166 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/top_level.txt
```

### Comparing `yao-0.0.5/setup.py` & `yao-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.0.5",
+    version="0.0.6",
     description="Dev",
     python_requires=">=3.9",
     author="Lsshu",
     author_email="admin@lsshu.cn",
     url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
```

### Comparing `yao-0.0.5/yao/crud.py` & `yao-0.0.6/yao/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/db.py` & `yao-0.0.6/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/depends.py` & `yao-0.0.6/yao/depends.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/annex/main.py` & `yao-0.0.6/yao/function/annex/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/annex/schema.py` & `yao-0.0.6/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/appointment/crud.py` & `yao-0.0.6/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/appointment/main.py` & `yao-0.0.6/yao/function/appointment/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/appointment/schema.py` & `yao-0.0.6/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/company/main.py` & `yao-0.0.6/yao/function/company/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/company/schema.py` & `yao-0.0.6/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/department/main.py` & `yao-0.0.6/yao/function/department/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/department/schema.py` & `yao-0.0.6/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/log/main.py` & `yao-0.0.6/yao/function/log/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/log/schema.py` & `yao-0.0.6/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/main.py` & `yao-0.0.6/yao/function/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/model.py` & `yao-0.0.6/yao/function/model.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/permission/main.py` & `yao-0.0.6/yao/function/permission/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/permission/schema.py` & `yao-0.0.6/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/user/crud.py` & `yao-0.0.6/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/user/main.py` & `yao-0.0.6/yao/function/user/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/function/user/schema.py` & `yao-0.0.6/yao/function/user/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/helpers.py` & `yao-0.0.6/yao/helpers.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao/method.py` & `yao-0.0.6/yao/method.py`

 * *Files 8% similar despite different names*

```diff
@@ -360,24 +360,47 @@
     ws.title = sheet_name
     ws.append([datum for datum in col_items.values()])
     # [ws.append([str(get_attr(db_obj, key, "")) for key in col_items]) for db_obj in db_list]
     for db_obj in db_list:
         _list = []
         for key in col_items:
             if type(db_obj) is dict:
-                _list.append(str(db_obj.get(key, "")))
+                _list.append(db_obj.get(key, ""))
             else:
-                _list.append(str(get_attr(db_obj, key, "") or ""))
+                _list.append(get_attr(db_obj, key, ""))
         ws.append(_list)
 
     if not os.path.exists(os.path.dirname(export_name)):
         os.makedirs(os.path.dirname(export_name))
     return wb.save(export_name)
 
 
+def export_files(export_name: str, sheet_data: list):
+    """
+    导出文件
+    """
+    from openpyxl import Workbook
+    wb = Workbook()
+    for key, sheet in enumerate(sheet_data):
+        ws = wb.create_sheet(sheet.get("sheet_name"), key)
+        ws.append([datum for datum in sheet.get("col_items", {}).values()])
+        for db_obj in sheet.get("db_list", []):
+            _list = []
+            for key in sheet.get("col_items", {}):
+                if type(db_obj) is dict:
+                    _list.append(db_obj.get(key, ""))
+                else:
+                    _list.append(get_attr(db_obj, key, ""))
+            ws.append(_list)
+
+        if not os.path.exists(os.path.dirname(export_name)):
+            os.makedirs(os.path.dirname(export_name))
+    return wb.save(export_name)
+
+
 def export_file_to_dict(sheet_name: str, export_name: str, col_items: dict, db_list: list):
     """
     导出文件
     """
     from openpyxl import Workbook
     wb = Workbook()
     ws = wb.active
```

### Comparing `yao-0.0.5/yao/schema.py` & `yao-0.0.6/yao/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.5/yao.egg-info/SOURCES.txt` & `yao-0.0.6/yao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

