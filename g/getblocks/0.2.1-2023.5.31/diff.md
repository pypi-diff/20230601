# Comparing `tmp/getblocks-0.2.1.tar.gz` & `tmp/getblocks-2023.5.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-0.2.1.tar", last modified: Fri May 12 22:32:05 2023, max compression
+gzip compressed data, was "getblocks-2023.5.31.tar", last modified: Thu Jun  1 01:14:18 2023, max compression
```

## Comparing `getblocks-0.2.1.tar` & `getblocks-2023.5.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:32:05.249307 getblocks-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 22:31:51.000000 getblocks-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-12 22:32:05.249307 getblocks-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-12 22:31:51.000000 getblocks-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:32:05.249307 getblocks-0.2.1/getblocks/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-12 22:31:51.000000 getblocks-0.2.1/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 22:31:51.000000 getblocks-0.2.1/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-12 22:31:51.000000 getblocks-0.2.1/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:32:05.249307 getblocks-0.2.1/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-12 22:32:05.000000 getblocks-0.2.1/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-12 22:32:05.000000 getblocks-0.2.1/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:32:05.000000 getblocks-0.2.1/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 22:32:05.000000 getblocks-0.2.1/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:32:05.000000 getblocks-0.2.1/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 22:32:05.000000 getblocks-0.2.1/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 22:32:05.000000 getblocks-0.2.1/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 22:32:05.249307 getblocks-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-12 22:31:51.000000 getblocks-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:14:18.826974 getblocks-2023.5.31/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 01:14:07.000000 getblocks-2023.5.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-01 01:14:18.826974 getblocks-2023.5.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-01 01:14:07.000000 getblocks-2023.5.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:14:18.826974 getblocks-2023.5.31/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 01:14:07.000000 getblocks-2023.5.31/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 01:14:07.000000 getblocks-2023.5.31/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-01 01:14:07.000000 getblocks-2023.5.31/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:14:18.826974 getblocks-2023.5.31/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 01:14:18.826974 getblocks-2023.5.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-01 01:14:07.000000 getblocks-2023.5.31/setup.py
```

### Comparing `getblocks-0.2.1/LICENSE` & `getblocks-2023.5.31/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-0.2.1/getblocks/cli.py` & `getblocks-2023.5.31/getblocks/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-import asyncio
 import collections
+import concurrent.futures
 import gzip
 import hashlib
 import math
 import requests
 import shutil
-import warnings
-from aiofile import async_open
 from blake3 import blake3
 from getblocks import __version__
 from pathlib import Path, PurePath
 
-BLOCKSIZE = 65536
-warnings.filterwarnings('ignore')
+def hasher(fname):
 
-### Instance Metadata Service Version 2 (IMDSv2) ###
-
-headers = {'X-aws-ec2-metadata-token-ttl-seconds': '30'}
-token = requests.put('http://169.254.169.254/latest/api/token', headers=headers)
-
-headers = {'X-aws-ec2-metadata-token': token.text}
-r = requests.get('http://169.254.169.254/latest/meta-data/ami-id', headers=headers)
-amiid = r.text
-
-async def hasher(fname):
     try:
         md5_file = ''
         sha256_file = ''
         b3_file = ''
+        BLOCKSIZE = 65536
         md5_hasher = hashlib.md5()
         sha256_hasher = hashlib.sha256()
         b3_hasher = blake3()
         with open(fname,'rb') as afile:
             buf = afile.read(BLOCKSIZE)
             while len(buf) > 0:
                 md5_hasher.update(buf)
@@ -51,110 +39,111 @@
     if sha256_file == 'E3B0C44298FC1C149AFBF4C8996FB92427AE41E4649B934CA495991B7852B855':
         sha256_file = 'EMPTY'
     if b3_file == 'AF1349B9F5F9A1A6A0404DEA36DCC9499BCB25C9ADC112B7CC9A93CAE41F3262':
         b3_file = 'EMPTY'
     hashes = md5_file+'|'+sha256_file+'|'+b3_file
     return hashes
 
-async def matchmeta(meta):
+def matchmeta(meta):
+
     md5_hasher = hashlib.md5()
     sha256_hasher = hashlib.sha256()
     b3_hasher = blake3()
     md5_hasher.update(meta.encode())
     sha256_hasher.update(meta.encode())
     b3_hasher.update(meta.encode())
     md5_meta = md5_hasher.hexdigest().upper()
     sha256_meta = sha256_hasher.hexdigest().upper()
     b3_meta = b3_hasher.hexdigest().upper()
     meta = md5_meta+'|'+sha256_meta+'|'+b3_meta
     return meta
 
-async def normalizepath(path):
-    if path[:1] == '/':					    ### LINUX
+def normalizepath(path):
+
+    if path[:1] == '/':
         out = path.split('/')
         try:
-            if out[1] == 'home':
+            if out[1] == 'home':            ### LINUX
                 out[2] = 'user'
                 path = '/'.join(out)
+            elif out[1] == 'Users':         ### APPLE
+                if out[2] != 'Shared':
+                    out[2] = 'user'
+                    path = '/'.join(out)
         except:
             pass
     elif path[1] == ':': 				    ### WINDOWS
-        new = list(path)
-        new[0] = 'C'
-        path = (''.join(new))
         out = path.split('\\')
         try:
             if out[1] == 'Users' or out[1] == 'Documents and Settings':
                 if out[2] != 'Default' and out[2] != 'Public' and out[2] != 'All Users' and out[2] != 'Default User':
+                    out[0] = 'C:'
                     out[2] = 'Administrator'
                     path = '\\'.join(out)
         except:
             pass
     return path
 
-async def parsefilename(filename):
-    if filename[:1] == '/':					### LINUX
+def parsefilename(filename):
+
+    if filename[:1] == '/':					### UNIX
         out = filename.split('/')
         count = len(out) - 1
     elif filename[1] == ':': 				### WINDOWS
-        new = list(path)
-        new[0] = 'C'
-        path = (''.join(new))
-        out = path.split('\\')
+        out = filename.split('\\')
         count = len(out) - 1
     return out[count]
 
-async def parseonlypath(onlypath):
-    if onlypath[:1] == '/':					### LINUX
+def parseonlypath(onlypath):
+
+    if onlypath[:1] == '/':					### UNIX
         out = onlypath.split('/')
         del out[-1]
         onlypath = '/'.join(out)
     elif onlypath[1] == ':': 				### WINDOWS
-        new = list(path)
-        new[0] = 'C'
-        path = (''.join(new))
-        out = path.split('\\')
+        out = onlypath.split('\\')
         del out[-1]
         onlypath = '\\'.join(out)
     return onlypath
 
-async def parser(p):
+def parser(p, amiid):
+
     try:
         size =  p.stat().st_size		
     except: 
         size = 0
         pass
     if size == 0:
         md5_file = 'EMPTY'
         sha256_file = 'EMPTY'
         b3_file = 'EMPTY'
     elif size > 104857599:
         md5_file = 'LARGE'
         sha256_file = 'LARGE'
         b3_file = 'LARGE'
     else:
-        hashes = await hasher(str(p))
+        hashes = hasher(str(p))
         out = hashes.split('|')
         md5_file = out[0]
         sha256_file = out[1]
         b3_file = out[2]
-    fullpath = await normalizepath(str(p))
-    meta = await matchmeta(fullpath)
+    fullpath = normalizepath(str(p))
+    meta = matchmeta(fullpath)
     out = meta.split('|')
     md5_path = out[0]
     sha256_path = out[1]
     b3_path = out[2]
-    directory = await parseonlypath(fullpath)
-    meta = await matchmeta(directory)
+    directory = parseonlypath(fullpath)
+    meta = matchmeta(directory)
     out = meta.split('|')
     md5_dir = out[0]
     sha256_dir = out[1]
     b3_dir = out[2]
-    filename = await parsefilename(fullpath)
-    meta = await matchmeta(filename)
+    filename = parsefilename(fullpath)
+    meta = matchmeta(filename)
     out = meta.split('|')
     md5_name = out[0]
     sha256_name = out[1]
     b3_name = out[2]
     value = str(amiid)+'|'+ \
         str(fullpath)+'|'+ \
         str(filename)+'|'+ \
@@ -169,15 +158,16 @@
         str(sha256_dir)+'|'+ \
         str(b3_dir)+'|'+ \
         str(md5_name)+'|'+ \
         str(sha256_name)+'|'+ \
         str(b3_name)+'|FILE|-|-|-\n'
     return value
 
-async def sector(p,count):
+def sector(p,count):
+
     block = 512
     ifile = open(p,'rb')
     ifile.seek(count)
     entropy_value = 0
     bases = collections.Counter([tmp_base for tmp_base in ifile.read(block)])
     for base in bases:
         n_i = bases[base]
@@ -187,60 +177,75 @@
     entropy = entropy_value * -1
     ifile.seek(count)
     b3block =  blake3(ifile.read(block)).hexdigest().upper()
     if b3block == 'AF1349B9F5F9A1A6A0404DEA36DCC9499BCB25C9ADC112B7CC9A93CAE41F3262':
         b3block = 'EMPTY'
     return str(entropy)+'|'+b3block
 
-async def start():
-    print('--------------------------------')
-    print('GETBLOCKS v'+__version__)
-    print('--------------------------------')
-    async with async_open(amiid+'.txt', 'w+') as f:
-        await f.write('ami|path|file|size|md5|sha256|b3|md5path|sha256path|b3path|md5dir|sha256dir|b3dir|md5name|sha256name|b3name|type|entropy|block|location\n')
+def start(amiid):
+
+    with open(amiid+'.txt', 'w+') as f:
+        f.write('ami|path|file|size|md5|sha256|b3|md5path|sha256path|b3path|md5dir|sha256dir|b3dir|md5name|sha256name|b3name|type|entropy|block|location\n')
         root = PurePath(Path.cwd()).anchor
         path = Path(root)
         for p in Path(path).glob('*'):
             if str(p) != '/proc':
                 if p.is_file() == True and not str(p).endswith(amiid+'.txt'):
-                    value = await parser(p)
+                    value = parser(p, amiid)
                     if value != None:
-                        await f.write(value)
+                        f.write(value)
                         out = value.split('|')
                         if out[6] != 'LARGE' and out[6] != 'EMPTY' and out[6] != '-':
                             count = 0
                             location = 1
                             while count <= int(out[3]):
                                 try:
-                                    block = await sector(p,count)
+                                    block = sector(p,count)
                                     parse = block.split('|')
-                                    await f.write(str(out[0])+'|-|-|'+str(out[3])+'|-|-|'+str(out[6])+'|-|-|-|-|-|-|-|-|-|SECTOR|'+str(parse[0])+'|'+str(parse[1])+'|'+str(location)+'\n')
+                                    f.write(str(out[0])+'|-|-|'+str(out[3])+'|-|-|'+str(out[6])+'|-|-|-|-|-|-|-|-|-|SECTOR|'+str(parse[0])+'|'+str(parse[1])+'|'+str(location)+'\n')
                                 except:
                                     pass
                                 count = count + 512
                                 location = location + 1
                 else:
                     for s in Path(p).rglob('*'):
                         if s.is_file() == True and not str(s).endswith(amiid+'.txt'):
-                            value = await parser(s)
+                            value = parser(s, amiid)
                             if value != None:
-                                await f.write(value)
+                                f.write(value)
                                 out = value.split('|')
                                 if out[6] != 'LARGE' and out[6] != 'EMPTY' and out[6] != '-':
                                     count = 0
                                     location = 1
                                     while count <= int(out[3]):
                                         try:
-                                            block = await sector(s,count)
+                                            block = sector(s,count)
                                             parse = block.split('|')
-                                            await f.write(str(out[0])+'|-|-|'+str(out[3])+'|-|-|'+str(out[6])+'|-|-|-|-|-|-|-|-|-|SECTOR|'+str(parse[0])+'|'+str(parse[1])+'|'+str(location)+'\n')
+                                            f.write(str(out[0])+'|-|-|'+str(out[3])+'|-|-|'+str(out[6])+'|-|-|-|-|-|-|-|-|-|SECTOR|'+str(parse[0])+'|'+str(parse[1])+'|'+str(location)+'\n')
                                         except:
                                             pass
                                         count = count + 512
                                         location = location + 1
 
 def main():
-    asyncio.run(start())
+
+    print('GETBLOCKS v'+__version__)
+
+    ### Instance Metadata Service Version 2 (IMDSv2) ###
+
+    headers = {'X-aws-ec2-metadata-token-ttl-seconds': '30'}
+    token = requests.put('http://169.254.169.254/latest/api/token', headers=headers)
+
+    headers = {'X-aws-ec2-metadata-token': token.text}
+    r = requests.get('http://169.254.169.254/latest/meta-data/ami-id', headers=headers)
+    amiid = r.text
+
+    print('  '+amiid)
+
+    with concurrent.futures.ThreadPoolExecutor() as executor:
+        executor.submit(start, amiid)
+
     with open(amiid+'.txt', 'rb') as f_in:
         with gzip.open(amiid+'.txt.gz', 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
-    print('Completed!!')
+
+    print('    Done!!')
```

### Comparing `getblocks-0.2.1/setup.py` & `getblocks-2023.5.31/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "getblocks",
     version = __version__,
-    description = "Down to the sector detail!",
+    description = "Down to the smallest sector detail!",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/jblukach/getblocks",
     author = "John Lukach",
     author_email = "hello@lukach.io",
     license = "Apache-2.0",
     packages = [
         "getblocks"
     ],
     install_requires = [
-        "aiofile",
         "blake3",
-        "requests==2.29.0"
+        "requests"
     ],
     zip_safe = False,
     entry_points = {
         "console_scripts": [
             "getblocks=getblocks.cli:main"
         ],
     },
```

