# Comparing `tmp/tracebloc_package-dev-0.4.2.tar.gz` & `tmp/tracebloc_package-dev-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.4.2.tar", last modified: Thu Jun  1 09:08:14 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.4.3.tar", last modified: Thu Jun  1 11:57:12 2023, max compression
```

## Comparing `tracebloc_package-dev-0.4.2.tar` & `tracebloc_package-dev-0.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 09:08:14.975252 tracebloc_package-dev-0.4.2/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.2/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 09:08:14.975316 tracebloc_package-dev-0.4.2/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.2/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-01 09:08:14.975553 tracebloc_package-dev-0.4.2/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-01 09:07:14.000000 tracebloc_package-dev-0.4.2/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 09:08:14.974160 tracebloc_package-dev-0.4.2/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.4.2/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-05-18 09:32:19.000000 tracebloc_package-dev-0.4.2/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    20998 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    60056 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.2/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)     9777 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10203 2023-06-01 06:15:22.000000 tracebloc_package-dev-0.4.2/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.2/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.4.2/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 09:08:14.975142 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-01 09:08:14.000000 tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 11:57:12.089361 tracebloc_package-dev-0.4.3/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.3/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 11:57:12.089499 tracebloc_package-dev-0.4.3/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.3/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-01 11:57:12.089872 tracebloc_package-dev-0.4.3/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-01 11:56:26.000000 tracebloc_package-dev-0.4.3/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 11:57:12.087909 tracebloc_package-dev-0.4.3/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.4.3/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-05-18 09:32:19.000000 tracebloc_package-dev-0.4.3/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    20998 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.3/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    60056 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.3/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.3/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)     9821 2023-06-01 11:56:14.000000 tracebloc_package-dev-0.4.3/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10203 2023-06-01 06:15:22.000000 tracebloc_package-dev-0.4.3/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.3/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.4.3/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 11:57:12.089143 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.4.2/LICENSE.txt` & `tracebloc_package-dev-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/PKG-INFO` & `tracebloc_package-dev-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.4.2
+Version: 0.4.3
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.2/setup.py` & `tracebloc_package-dev-0.4.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.4.2",
+    version="0.4.3",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/linkModelDataSet.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/messages.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/upload.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,18 +174,18 @@
                 )
             self.progress_bar.close()
             return None
 
     def __upload_model(self):
         model_file = open(self.__model_path, "rb")
         if self.weights:
-            weights_valid, weights = self.checkWeights()
+            weights_valid, weights_data = self.checkWeights()
             if not weights_valid:
                 return None
-            files = {"upload_file": model_file, "upload_weights": weights}
+            files = {"upload_file": model_file, "upload_weights": weights_data}
             values = {
                 "model_name": self.__modelname,
                 "setWeights": True,
                 "type": "functional_test",
             }
         else:
             files = {"upload_file": model_file}
@@ -195,28 +195,29 @@
                 "type": "functional_test",
             }
         # call check-model API to do functional test
         header = {"Authorization": f"Token {self.__token}"}
         r = requests.post(
             self.__check_model_url, headers=header, files=files, data=values
         )
+        if self.weights:
+            weights_data.close()
         model_file.close()
         body_unicode = r.content.decode("utf-8")
         content = json.loads(body_unicode)
         text = content["text"]
         check_status = content["check_status"]
         if not check_status:
             tex = colored(
                 text,
                 "red",
             )
             print(tex, "\n")
             return None
         self.progress_bar.update(1)
-        weights.close()
         return content["model_name"]
 
     def checkWeights(self):
         # load model weights from current directory
         try:
             weights_file = open(self.__weights_path, "rb")
         except FileNotFoundError:
```

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/user.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/utils.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package/weights.py` & `tracebloc_package-dev-0.4.3/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.4.2
+Version: 0.4.3
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.2/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

