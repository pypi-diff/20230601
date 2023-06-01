# Comparing `tmp/openi-beta-0.0.3.tar.gz` & `tmp/openi-beta-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.3.tar", last modified: Wed May 31 07:09:27 2023, max compression
+gzip compressed data, was "openi-beta-0.0.4.tar", last modified: Thu Jun  1 03:28:07 2023, max compression
```

## Comparing `openi-beta-0.0.3.tar` & `openi-beta-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.167158 openi-beta-0.0.3/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2636 2023-05-31 07:09:27.167010 openi-beta-0.0.3/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     2006 2023-05-30 10:27:22.000000 openi-beta-0.0.3/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-05-31 07:09:27.167200 openi-beta-0.0.3/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1043 2023-05-31 07:09:25.000000 openi-beta-0.0.3/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.163954 openi-beta-0.0.3/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.164444 openi-beta-0.0.3/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       47 2023-05-29 10:23:59.000000 openi-beta-0.0.3/src/openi/__init__.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.165249 openi-beta-0.0.3/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.3/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10676 2023-05-30 10:27:38.000000 openi-beta-0.0.3/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.165930 openi-beta-0.0.3/src/openi/modelarts/
--rw-r--r--   0 jochen10518   (501) staff       (20)       24 2023-05-30 09:14:40.000000 openi-beta-0.0.3/src/openi/modelarts/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     4555 2023-05-31 07:07:02.000000 openi-beta-0.0.3/src/openi/modelarts/helper.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     1669 2023-05-31 07:07:04.000000 openi-beta-0.0.3/src/openi/modelarts/modelarts.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.166769 openi-beta-0.0.3/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2636 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      383 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       43 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.596904 openi-beta-0.0.4/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 03:28:07.596752 openi-beta-0.0.4/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      878 2023-05-31 09:59:56.000000 openi-beta-0.0.4/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-01 03:28:07.596946 openi-beta-0.0.4/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)      985 2023-06-01 03:27:42.000000 openi-beta-0.0.4/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.594061 openi-beta-0.0.4/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.594566 openi-beta-0.0.4/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       47 2023-05-29 10:23:59.000000 openi-beta-0.0.4/src/openi/__init__.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.594901 openi-beta-0.0.4/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.4/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10658 2023-06-01 03:23:46.000000 openi-beta-0.0.4/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.595380 openi-beta-0.0.4/src/openi/modelarts/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       24 2023-05-30 09:14:40.000000 openi-beta-0.0.4/src/openi/modelarts/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     4555 2023-05-31 07:07:02.000000 openi-beta-0.0.4/src/openi/modelarts/helper.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1669 2023-05-31 07:07:04.000000 openi-beta-0.0.4/src/openi/modelarts/modelarts.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.596208 openi-beta-0.0.4/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      416 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       20 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-01 03:28:07.000000 openi-beta-0.0.4/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 03:28:07.596534 openi-beta-0.0.4/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      605 2023-06-01 03:25:57.000000 openi-beta-0.0.4/test/test.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      904 2023-06-01 03:25:51.000000 openi-beta-0.0.4/test/test_thread.py
```

### Comparing `openi-beta-0.0.3/setup.py` & `openi-beta-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.3',
+    version='0.0.4',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
-    packages=find_packages('src'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
     license='MIT',
     classifiers=[
@@ -23,10 +22,10 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Operating System :: OS Independent',
     ],
-    install_requires=['emoji>=2.4.0', 'requests>=2.30.0','tqdm>=4.65.0'],
+    install_requires=['emoji', 'requests','tqdm'],
     python_requires='>=3.6',
 )
```

### Comparing `openi-beta-0.0.3/src/openi/dataset/dataset.py` & `openi-beta-0.0.4/src/openi/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,17 +135,17 @@
         if x.json()["result_code"] == "-1":
             raise ConnectionRefusedError(f'{emoji.emojize(":cross_mark:")} <{x.status_code} {x.reason}> {x.json()["msg"]}')
 
 
     """
     utils functions
     """
-    def logging(self,message):
-        asctime = datetime.now().strftime("%Y/%m/%d %H:%M:%S")
-        print(f'{asctime} [{self.filename}-{self.cluster}]: {message}')
+    def logging(self,message=""):
+        asctime = datetime.now().strftime("%H:%M:%S")
+        return(f'{asctime} | {self.filename} | {self.cluster} | {message}')
 
     def filePreprocess(self):
         # suffix1 = self.filename.split(".")[-1]
         # suffix2 = '.'.join(self.filename.split(".")[-2:])
         # if suffix1 != "zip" and suffix2 != "tar.gz":
         #     raise ValueError(f'{emoji.emojize(":cross_mark:")} [{self.filename}] File type is not zip or tar.gz')
         if self.size == 0:
@@ -174,15 +174,15 @@
     """
     Main functions
     uploadProgressBar(): upload file with progress bar.
     uploadMain(): control flow function.
     """
     def uploadProgressBar(self,chunks):
         u = len(self.chunks) - len(chunks)
-        with tqdm(total= self.size, desc='Uploading', leave=True, unit='B', unit_scale=True, unit_divisor=1000)  as pbar:
+        with tqdm(total= self.size, leave=True, unit='B', unit_scale=True, unit_divisor=1000, desc=self.logging(), bar_format='{desc}{percentage:3.0f}%|{bar}{r_bar}')  as pbar:
             # checkpoint
             if u != 0: pbar.update(self.max_chunk_size * u)     
 
             # upload chunks
             for n, v in chunks.items():
                 chunk_size = v[1] - v[0]
                 self.getMultipartURL(n,chunk_size)
@@ -205,43 +205,43 @@
                         self.putUpload(n,start_index,piece_volume_mb)
                         start_index += piece_volume_mb
                         pbar.update(piece_volume_mb)
                         #logging.info(f"\t[{self.filename}]: [piece {i}] piece index: {start_index - piece_volume_mb} to {start_index}, volume: {piece_volume_mb}")
 
     def uploadMain(self):
 
-        self.logging(f'{emoji.emojize(":light_bulb:")} dataset file processing & checking...')
+        print(self.logging('dataset file processing & checking...'))
         # preprocess
         self.filePreprocess()    
         # checking upload status
         self.getChunks()
 
         # upload starts
         if self.uuid != '':
             if self.uploaded:
                 raise ValueError(f'{emoji.emojize(":cross_mark:")} Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again.')
             else:
-                self.logging(f'{emoji.emojize(":light_bulb:")} continue upload...')
+                print(self.logging('continue upload...'))
                 uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
                 continue_chunks = { i:self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
                 # re-upload last chunk from checkpoint
                 if uploaded_chunks != []:
                     last_chunk_index = max(uploaded_chunks)
                     continue_chunks[last_chunk_index] = self.chunks[last_chunk_index]
                 continue_chunks =  OrderedDict(sorted(continue_chunks.items()))
                 self.uploadProgressBar(continue_chunks)
 
         else:
-            self.logging(f'{emoji.emojize(":light_bulb:")} start new upload...')
+            print(self.logging('start new upload...'))
             self.newMultipart()
             self.uploadProgressBar(self.chunks)
 
         self.completeMultipart()        
         url = f"{self.app_url.split('api')[0]}{self.username}/{self.repo}/datasets"
-        self.logging(f'{emoji.emojize(":party_popper:")} Successfully uploaded, view on link: {url}')
+        print(self.logging(f'{emoji.emojize(":party_popper:")} Successfully uploaded, view on link: {url}'))
 
 def upload_file(file, username, repository, token, cluster="", app_url=""):
     d = DatasetUploadFile(
         file = file, 
         username = username, 
         repository = repository, 
         token = token,
```

### Comparing `openi-beta-0.0.3/src/openi/modelarts/helper.py` & `openi-beta-0.0.4/src/openi/modelarts/helper.py`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.3/src/openi/modelarts/modelarts.py` & `openi-beta-0.0.4/src/openi/modelarts/modelarts.py`

 * *Files identical despite different names*

