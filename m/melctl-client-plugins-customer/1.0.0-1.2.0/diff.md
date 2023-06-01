# Comparing `tmp/melctl_client_plugins_customer-1.0.0.tar.gz` & `tmp/melctl_client_plugins_customer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melctl_client_plugins_customer-1.0.0.tar", last modified: Mon Jan 30 15:42:57 2023, max compression
+gzip compressed data, was "melctl_client_plugins_customer-1.2.0.tar", last modified: Thu Jun  1 09:19:03 2023, max compression
```

## Comparing `melctl_client_plugins_customer-1.0.0.tar` & `melctl_client_plugins_customer-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-01-30 15:42:57.863053 melctl_client_plugins_customer-1.0.0/
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     1502 2023-01-30 12:01:00.000000 melctl_client_plugins_customer-1.0.0/LICENSE
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)      263 2023-01-30 15:42:57.863053 melctl_client_plugins_customer-1.0.0/PKG-INFO
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)      281 2023-01-03 14:39:23.000000 melctl_client_plugins_customer-1.0.0/README.md
-drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-01-30 15:42:57.863053 melctl_client_plugins_customer-1.0.0/melctl_client_plugins/
-drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-01-30 15:42:57.863053 melctl_client_plugins_customer-1.0.0/melctl_client_plugins/s3/
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     2066 2023-01-30 13:45:02.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins/s3/__init__.py
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     2213 2023-01-30 12:55:34.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins/s3/config.py
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)    22919 2023-01-30 13:43:55.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins/s3/s3.py
-drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-01-30 15:42:57.863053 melctl_client_plugins_customer-1.0.0/melctl_client_plugins_customer.egg-info/
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)      263 2023-01-30 15:42:57.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins_customer.egg-info/PKG-INFO
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)      398 2023-01-30 15:42:57.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins_customer.egg-info/SOURCES.txt
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)        1 2023-01-30 15:42:57.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins_customer.egg-info/dependency_links.txt
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)       81 2023-01-30 15:42:57.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins_customer.egg-info/requires.txt
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)       22 2023-01-30 15:42:57.000000 melctl_client_plugins_customer-1.0.0/melctl_client_plugins_customer.egg-info/top_level.txt
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)       38 2023-01-30 15:42:57.863053 melctl_client_plugins_customer-1.0.0/setup.cfg
--rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     2340 2023-01-30 14:57:23.000000 melctl_client_plugins_customer-1.0.0/setup.py
+drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-06-01 09:19:03.027694 melctl_client_plugins_customer-1.2.0/
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     1502 2023-01-30 12:01:00.000000 melctl_client_plugins_customer-1.2.0/LICENSE
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     1452 2023-06-01 09:19:03.023694 melctl_client_plugins_customer-1.2.0/PKG-INFO
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)      281 2023-01-03 14:39:23.000000 melctl_client_plugins_customer-1.2.0/README.md
+drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-06-01 09:19:03.023694 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/
+drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-06-01 09:19:03.023694 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s3/
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     2086 2023-02-02 12:15:53.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s3/__init__.py
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     2213 2023-01-30 12:55:34.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s3/config.py
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)    26413 2023-04-04 08:58:14.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s3/s3.py
+drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-06-01 09:19:03.023694 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s8s/
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     2087 2023-04-18 14:51:24.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s8s/__init__.py
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)    15697 2023-04-26 07:56:06.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s8s/s8s.py
+drwxrwxr-x   0 jpclipffel  (1000) jpclipffel  (1000)        0 2023-06-01 09:19:03.023694 melctl_client_plugins_customer-1.2.0/melctl_client_plugins_customer.egg-info/
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     1452 2023-06-01 09:19:02.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins_customer.egg-info/PKG-INFO
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)      469 2023-06-01 09:19:03.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins_customer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)        1 2023-06-01 09:19:02.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins_customer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)       81 2023-06-01 09:19:02.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins_customer.egg-info/requires.txt
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)       22 2023-06-01 09:19:02.000000 melctl_client_plugins_customer-1.2.0/melctl_client_plugins_customer.egg-info/top_level.txt
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)       38 2023-06-01 09:19:03.027694 melctl_client_plugins_customer-1.2.0/setup.cfg
+-rw-rw-r--   0 jpclipffel  (1000) jpclipffel  (1000)     3837 2023-04-26 08:05:13.000000 melctl_client_plugins_customer-1.2.0/setup.py
```

### Comparing `melctl_client_plugins_customer-1.0.0/LICENSE` & `melctl_client_plugins_customer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `melctl_client_plugins_customer-1.0.0/melctl_client_plugins/s3/__init__.py` & `melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,10 +47,11 @@
         s3.Logout,
         s3.Info,
         s3.List,
         s3.MakeBucket,
         s3.DeleteBucket,
         s3.DeleteObjects,
         s3.Copy,
+        s3.Reindex,
         s3.GenConf
     ]
 }
```

### Comparing `melctl_client_plugins_customer-1.0.0/melctl_client_plugins/s3/config.py` & `melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s3/config.py`

 * *Files identical despite different names*

### Comparing `melctl_client_plugins_customer-1.0.0/melctl_client_plugins/s3/s3.py` & `melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s3/s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -280,14 +280,62 @@
                         else:
                             tasks.append(upload_direct(client, str(_src_path), obj_key))
             # Upload
             results = await asyncio.gather(*tasks)
         # Done
         return results
 
+    async def reindex_bucket(self, bucket: str, write: bool, update: bool, delete: bool, mode: str = 'headers'):
+        """Sync a bucket with its underlying file system path.
+
+        :param bucket: Bucket name
+        :param write: If `True`, add new found files to bucket
+        :param update: If `True`, update changed files metadata in bucket
+        :param delete: If `True`, remove deleted files from bucket
+        :param mode: Operation mode, either `query`, `headers` or `payload`
+        """
+
+        def get_ops():
+            return list(filter(None, [
+                write and 'WRITE' or None,
+                update and 'UPDATE' or None,
+                delete and 'DELETE' or None
+            ]))
+
+        def set_request(request, **kwargs):
+            # All modes - Patch URL
+            request.url = f"{'/'.join(request.url.split('/')[0:-1])}?sync"
+            # Headers mode - Add headers
+            if mode == 'headers':
+                ops = get_ops()
+                if len(ops) > 0:
+                    request.headers.add_header('x-ddn-bucket-sync-ops', ','.join(ops))
+
+        async with self.session.create_client(**self.client_kwargs) as client:
+            # All modes - Patch URL
+            client.meta.events.register('before-sign.*', set_request)
+            # Headers and Query modes - No payload
+            if mode in ('query', 'headers'):
+                response = await client.put_object(
+                    Bucket=bucket,
+                    Key='bucketsync_payload_empty'
+                )
+            # Payload mode - Add payload
+            elif mode == 'payload':
+                response = await client.put_object(
+                    Bucket=bucket,
+                    Key='bucketsync_payload',
+                    Body=f'<operation><operationTypes>{",".join(get_ops())}</operationTypes></operation>'
+                )
+            else:
+                raise Exception(f'Invalid mode: got {mode}, excepts one of query,headers,payload')
+            # Get response
+            print(response, type(response))
+            return response
+
 
 class Login(Command):
     """Login to S3 and store credentials.
     """
 
     def __init__(self, subparser):
         super().__init__(subparser, 'login')
@@ -547,14 +595,54 @@
     def target(self, args):
         return asyncio.run(self.s3.delete_objects(
             *S3.parse_path(args.path),
             args.recursive
         ))
 
 
+class Reindex(Command):
+    """Reindex a bucket.
+    """
+
+    def __init__(self, subparser):
+        super().__init__(subparser, 'reindex', headers=('bucket', 'HTTPStatusCode'))
+        self.parser.add_argument('name', type=str, help='Bucket name')
+        self.parser.add_argument('-m', '--mode', type=str,
+            choices=('query', 'headers', 'payload'),
+            default='headers')
+        for op, help in (
+            ('write',      'new files indexation in bucket'),
+            ('update', 'changed files re-indexation in bucket'),
+            ('delete', 'deleted files de-indexation from bucket')
+            ):
+            self.parser.add_argument(f'--{op}', dest=op, action='store_true',
+                default=True, help=f'Enable {help}')
+            self.parser.add_argument(f'--no-{op}', dest=op, action='store_false',
+                default=True, help=f'Disable {help}')
+        self.s3 = S3()
+
+    def target(self, args):
+        bucket = S3.parse_path(args.name)[0]
+        data = asyncio.run(self.s3.reindex_bucket(
+            bucket,
+            args.write,
+            args.update,
+            args.delete,
+            args.mode
+        ))
+        print(type(data))
+        # Extra attributes
+        data.update({
+            'bucket': bucket,
+            'HTTPStatusCode': data.get('ResponseMetadata', {}).get('HTTPStatusCode'),
+        })
+        # Done
+        return data
+
+
 class GenConf(Command):
     """Generates other S3 clients configuration.
     """
 
     generators: dict[str, str] = {
         'aws-conf': '_aws_conf',
         'aws-auth': '_aws_auth',
```

### Comparing `melctl_client_plugins_customer-1.0.0/setup.py` & `melctl_client_plugins_customer-1.2.0/melctl_client_plugins/s8s/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,24 +34,23 @@
 __copyright__  = 'Copyright (c) 2023 LuxProvide S.A.'
 __maintainer__ = 'Jean-Philippe Clipffel'
 
 
 __version__    = '1.0.0'
 
 
-from setuptools import setup, find_namespace_packages
+from . import s8s
 
 
-setup(
-    name='melctl_client_plugins_customer',
-    author='@jpclipffel',
-    url='https://gitlab.lxp.lu/lxp-hpc/iac/meluxina/melctl-client-plugins/customer',
-    version=__version__,
-    packages=find_namespace_packages(include=['melctl_client_plugins.*']),
-    install_requires=[
-        'melctl_client >= 5.2.0, < 6.0.0',
-        'aiofiles >= 22.1',
-        'aiobotocore >= 2.4',
-        # Library stubs
-        'types-aiofiles >= 22.1',
+commands = {
+    's8s': [
+        s8s.SetConfig,
+        s8s.GetConfig,
+        s8s.DelConfig,
+        s8s.RegionsList,
+        s8s.PoolsList,
+        s8s.PoolsGet,
+        s8s.Status,
+        s8s.Resources,
+        s8s.Scale
     ]
-)
+}
```

