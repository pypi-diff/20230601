# Comparing `tmp/br-ci-sdk-0.0.1.tar.gz` & `tmp/br-ci-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "br-ci-sdk-0.0.1.tar", last modified: Thu Jun  1 09:58:53 2023, max compression
+gzip compressed data, was "br-ci-sdk-0.0.2.tar", last modified: Thu Jun  1 10:09:25 2023, max compression
```

## Comparing `br-ci-sdk-0.0.1.tar` & `br-ci-sdk-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1868 2023-05-31 08:38:01.000000 br-ci-sdk-0.0.1/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1534 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2251 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1295 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/br_ci_sdk.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 09:58:53.000000 br-ci-sdk-0.0.1/br_ci_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      676 2023-06-01 09:58:53.000000 br-ci-sdk-0.0.1/br_ci_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-06-01 09:58:53.000000 br-ci-sdk-0.0.1/br_ci_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       39 2023-06-01 09:58:53.000000 br-ci-sdk-0.0.1/br_ci_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       75 2023-06-01 09:58:53.000000 br-ci-sdk-0.0.1/br_ci_sdk.egg-info/requires.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       34 2023-06-01 09:58:53.000000 br-ci-sdk-0.0.1/br_ci_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        8 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3923 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)    10941 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3359 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/handles/repo.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      527 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1360 2023-06-01 09:58:31.000000 br-ci-sdk-0.0.1/setup.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:58:53.734588 br-ci-sdk-0.0.1/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1304 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.1/utils/xml_utils.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1868 2023-05-31 08:38:01.000000 br-ci-sdk-0.0.2/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.243923 br-ci-sdk-0.0.2/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1534 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2251 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1295 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2302 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      676 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       39 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       75 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/requires.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       34 2023-06-01 10:09:25.000000 br-ci-sdk-0.0.2/br_ci_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        8 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3923 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)    10941 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3359 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/handles/repo.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      527 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1360 2023-06-01 10:09:18.000000 br-ci-sdk-0.0.2/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-06-01 10:09:25.247923 br-ci-sdk-0.0.2/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1304 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-06-01 09:50:26.000000 br-ci-sdk-0.0.2/utils/xml_utils.py
```

### Comparing `br-ci-sdk-0.0.1/PKG-INFO` & `br-ci-sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: br-ci-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `br-ci-sdk-0.0.1/README.md` & `br-ci-sdk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/apis/build.py` & `br-ci-sdk-0.0.2/apis/build.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/apis/client.py` & `br-ci-sdk-0.0.2/apis/client.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/apis/pdu.py` & `br-ci-sdk-0.0.2/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/apis/perf.py` & `br-ci-sdk-0.0.2/apis/perf.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/apis/pr.py` & `br-ci-sdk-0.0.2/apis/pr.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/br_ci_sdk.egg-info/PKG-INFO` & `br-ci-sdk-0.0.2/br_ci_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: br-ci-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `br-ci-sdk-0.0.1/br_ci_sdk.egg-info/SOURCES.txt` & `br-ci-sdk-0.0.2/br_ci_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/handles/build.py` & `br-ci-sdk-0.0.2/handles/build.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/handles/pdu.py` & `br-ci-sdk-0.0.2/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/handles/perf.py` & `br-ci-sdk-0.0.2/handles/perf.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/handles/pr.py` & `br-ci-sdk-0.0.2/handles/pr.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/handles/repo.py` & `br-ci-sdk-0.0.2/handles/repo.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/schemas/jenkins.py` & `br-ci-sdk-0.0.2/schemas/jenkins.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/schemas/pull_request.py` & `br-ci-sdk-0.0.2/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/setup.py` & `br-ci-sdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         else:
             requires.append(pkg)
     return requires
 
 
 setuptools.setup(
     name="br-ci-sdk", 
-    version="0.0.1",    
+    version="0.0.2",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
```

### Comparing `br-ci-sdk-0.0.1/utils/csv_utils.py` & `br-ci-sdk-0.0.2/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `br-ci-sdk-0.0.1/utils/xml_utils.py` & `br-ci-sdk-0.0.2/utils/xml_utils.py`

 * *Files identical despite different names*

