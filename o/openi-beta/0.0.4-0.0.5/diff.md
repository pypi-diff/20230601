# Comparing `tmp/openi-beta-0.0.4.tar.gz` & `tmp/openi-beta-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.4.tar", last modified: Thu Jun  1 03:28:07 2023, max compression
+gzip compressed data, was "openi-beta-0.0.5.tar", last modified: Thu Jun  1 10:10:55 2023, max compression
```

## Comparing `openi-beta-0.0.4.tar` & `openi-beta-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.596904 openi-beta-0.0.4/
--rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 03:28:07.596752 openi-beta-0.0.4/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      878 2023-05-31 09:59:56.000000 openi-beta-0.0.4/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-01 03:28:07.596946 openi-beta-0.0.4/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)      985 2023-06-01 03:27:42.000000 openi-beta-0.0.4/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.594061 openi-beta-0.0.4/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.594566 openi-beta-0.0.4/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       47 2023-05-29 10:23:59.000000 openi-beta-0.0.4/src/openi/__init__.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.594901 openi-beta-0.0.4/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.4/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10658 2023-06-01 03:23:46.000000 openi-beta-0.0.4/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.595380 openi-beta-0.0.4/src/openi/modelarts/
--rw-r--r--   0 jochen10518   (501) staff       (20)       24 2023-05-30 09:14:40.000000 openi-beta-0.0.4/src/openi/modelarts/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     4555 2023-05-31 07:07:02.000000 openi-beta-0.0.4/src/openi/modelarts/helper.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     1669 2023-05-31 07:07:04.000000 openi-beta-0.0.4/src/openi/modelarts/modelarts.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.596208 openi-beta-0.0.4/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      416 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       20 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.596534 openi-beta-0.0.4/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      605 2023-06-01 03:25:57.000000 openi-beta-0.0.4/test/test.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      904 2023-06-01 03:25:51.000000 openi-beta-0.0.4/test/test_thread.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.171168 openi-beta-0.0.5/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 10:10:55.171020 openi-beta-0.0.5/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      878 2023-06-01 03:43:54.000000 openi-beta-0.0.5/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-01 10:10:55.171211 openi-beta-0.0.5/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)      985 2023-06-01 09:26:40.000000 openi-beta-0.0.5/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.168919 openi-beta-0.0.5/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.169447 openi-beta-0.0.5/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-01 10:05:04.000000 openi-beta-0.0.5/src/openi/__init__.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.169738 openi-beta-0.0.5/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.5/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10607 2023-06-01 10:05:03.000000 openi-beta-0.0.5/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.170564 openi-beta-0.0.5/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      321 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       20 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.170830 openi-beta-0.0.5/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      605 2023-06-01 03:43:28.000000 openi-beta-0.0.5/test/test.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      904 2023-06-01 03:43:28.000000 openi-beta-0.0.5/test/test_thread.py
```

### Comparing `openi-beta-0.0.4/PKG-INFO` & `openi-beta-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.4
+Version: 0.0.5
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -43,8 +43,8 @@
     repository = "", # 必填，数据集所属项目名
     token = "", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
     
     cluster = "", # 选填，可填入GPU或NPU，不填写后台默认为NPU
     app_url = "" #选填, 默认为平台地址，开发测试用
     )
 ```
-![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/8d5991eede95316b6a688135ecad790ba2ae165b/media/4.png)
+![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/7d3365f667974c5a06aaeb390003a3b929fde0d9/media/4.png)
```

### Comparing `openi-beta-0.0.4/README.md` & `openi-beta-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     repository = "", # 必填，数据集所属项目名
     token = "", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
     
     cluster = "", # 选填，可填入GPU或NPU，不填写后台默认为NPU
     app_url = "" #选填, 默认为平台地址，开发测试用
     )
 ```
-![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/8d5991eede95316b6a688135ecad790ba2ae165b/media/4.png)
+![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/7d3365f667974c5a06aaeb390003a3b929fde0d9/media/4.png)
```

### Comparing `openi-beta-0.0.4/setup.py` & `openi-beta-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.4',
+    version='0.0.5',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.0.4/src/openi/dataset/dataset.py` & `openi-beta-0.0.5/src/openi/dataset/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 import math
 import emoji
 import requests
 import hashlib
 from tqdm import tqdm
 from collections import OrderedDict
 from datetime import datetime
+import logging
+
+LOG_FORMAT = "%(asctime)s [%(levelname)s] - %(funcName)s() %(lineno)d: %(message)s"
+DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
+logging.basicConfig(filename='openi.log', level=logging.DEBUG, format=LOG_FORMAT, datefmt=DATE_FORMAT)
 
 class DatasetUploadFile:
     """
     Build APIs calls for uploading a file to openi platform.
     This class will start upload process immediatelly once being initialized. 
     """
     def __init__(self, file, username, repository, token, cluster="NPU", app_url="https://openi.pcl.ac.cn/api/v1/"):
@@ -135,23 +140,19 @@
         if x.json()["result_code"] == "-1":
             raise ConnectionRefusedError(f'{emoji.emojize(":cross_mark:")} <{x.status_code} {x.reason}> {x.json()["msg"]}')
 
 
     """
     utils functions
     """
-    def logging(self,message=""):
+    def stdOut(self,message=""):
         asctime = datetime.now().strftime("%H:%M:%S")
         return(f'{asctime} | {self.filename} | {self.cluster} | {message}')
 
     def filePreprocess(self):
-        # suffix1 = self.filename.split(".")[-1]
-        # suffix2 = '.'.join(self.filename.split(".")[-2:])
-        # if suffix1 != "zip" and suffix2 != "tar.gz":
-        #     raise ValueError(f'{emoji.emojize(":cross_mark:")} [{self.filename}] File type is not zip or tar.gz')
         if self.size == 0:
             raise ValueError(f'{emoji.emojize(":cross_mark:")} [{self.filename}] File size is 0')
         if self.size > int(200**10): # 200GB
             raise ValueError(f'{emoji.emojize(":cross_mark:")} [{self.filename}] File size exceeds 200GB')
 
         if self.size > self.max_chunk_size:
             self.total_chunk_counts = math.ceil(self.size / self.max_chunk_size) 
@@ -174,23 +175,23 @@
     """
     Main functions
     uploadProgressBar(): upload file with progress bar.
     uploadMain(): control flow function.
     """
     def uploadProgressBar(self,chunks):
         u = len(self.chunks) - len(chunks)
-        with tqdm(total= self.size, leave=True, unit='B', unit_scale=True, unit_divisor=1000, desc=self.logging(), bar_format='{desc}{percentage:3.0f}%|{bar}{r_bar}')  as pbar:
+        with tqdm(total= self.size, leave=True, unit='B', unit_scale=True, unit_divisor=1000, desc=self.stdOut(), bar_format='{desc}{percentage:3.0f}%|{bar}{r_bar}')  as pbar:
             # checkpoint
             if u != 0: pbar.update(self.max_chunk_size * u)     
 
             # upload chunks
             for n, v in chunks.items():
                 chunk_size = v[1] - v[0]
                 self.getMultipartURL(n,chunk_size)
-                #logging.info(f"[{self.filename}]: [CHUNK {n}] chunk index: {v[0]} to {v[1]}")
+                logging.info(f"[{self.filename}]: [CHUNK {n}] chunk index: {v[0]} to {v[1]}")
 
                 # small file only 1 chunk
                 if self.total_chunk_counts == 1:
                     self.putUpload(n,v[0],chunk_size)
                     pbar.update(chunk_size)
 
                 # large file, divide into 10 pieces for each chunk for more acurrate progress bar
@@ -201,47 +202,47 @@
                     start_index = v[0]
                     for i in range(num_pieces):
                         if i == num_pieces - 1:  # Last piece
                             piece_volume_mb += extra_volume_mb
                         self.putUpload(n,start_index,piece_volume_mb)
                         start_index += piece_volume_mb
                         pbar.update(piece_volume_mb)
-                        #logging.info(f"\t[{self.filename}]: [piece {i}] piece index: {start_index - piece_volume_mb} to {start_index}, volume: {piece_volume_mb}")
+                        logging.info(f"\t[{self.filename}]: [piece {i}] piece index: {start_index - piece_volume_mb} to {start_index}, volume: {piece_volume_mb}")
 
     def uploadMain(self):
 
-        print(self.logging('dataset file processing & checking...'))
+        print(self.stdOut('dataset file processing & checking...'))
         # preprocess
         self.filePreprocess()    
         # checking upload status
         self.getChunks()
 
         # upload starts
         if self.uuid != '':
             if self.uploaded:
                 raise ValueError(f'{emoji.emojize(":cross_mark:")} Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again.')
             else:
-                print(self.logging('continue upload...'))
+                print(self.stdOut('continue upload...'))
                 uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
                 continue_chunks = { i:self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
                 # re-upload last chunk from checkpoint
                 if uploaded_chunks != []:
                     last_chunk_index = max(uploaded_chunks)
                     continue_chunks[last_chunk_index] = self.chunks[last_chunk_index]
                 continue_chunks =  OrderedDict(sorted(continue_chunks.items()))
                 self.uploadProgressBar(continue_chunks)
 
         else:
-            print(self.logging('start new upload...'))
+            print(self.stdOut('start new upload...'))
             self.newMultipart()
             self.uploadProgressBar(self.chunks)
 
         self.completeMultipart()        
         url = f"{self.app_url.split('api')[0]}{self.username}/{self.repo}/datasets"
-        print(self.logging(f'{emoji.emojize(":party_popper:")} Successfully uploaded, view on link: {url}'))
+        print(self.stdOut(f'{emoji.emojize(":party_popper:")} Successfully uploaded, view on link: {url}'))
 
 def upload_file(file, username, repository, token, cluster="", app_url=""):
     d = DatasetUploadFile(
         file = file, 
         username = username, 
         repository = repository, 
         token = token,
```

### Comparing `openi-beta-0.0.4/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.0.5/src/openi_beta.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.4
+Version: 0.0.5
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -43,8 +43,8 @@
     repository = "", # 必填，数据集所属项目名
     token = "", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
     
     cluster = "", # 选填，可填入GPU或NPU，不填写后台默认为NPU
     app_url = "" #选填, 默认为平台地址，开发测试用
     )
 ```
-![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/8d5991eede95316b6a688135ecad790ba2ae165b/media/4.png)
+![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/7d3365f667974c5a06aaeb390003a3b929fde0d9/media/4.png)
```

### Comparing `openi-beta-0.0.4/test/test.py` & `openi-beta-0.0.5/test/test.py`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.4/test/test_thread.py` & `openi-beta-0.0.5/test/test_thread.py`

 * *Files identical despite different names*

