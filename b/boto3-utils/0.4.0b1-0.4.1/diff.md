# Comparing `tmp/boto3-utils-0.4.0b1.tar.gz` & `tmp/boto3-utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-utils-0.4.0b1.tar", last modified: Sat Nov  5 06:20:52 2022, max compression
+gzip compressed data, was "boto3-utils-0.4.1.tar", last modified: Thu Jun  1 03:01:17 2023, max compression
```

## Comparing `boto3-utils-0.4.0b1.tar` & `boto3-utils-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 06:20:52.239248 boto3-utils-0.4.0b1/
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-05 06:20:52.239248 boto3-utils-0.4.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 06:20:52.239248 boto3-utils-0.4.0b1/boto3_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-05 06:20:52.000000 boto3-utils-0.4.0b1/boto3_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-05 06:20:52.000000 boto3-utils-0.4.0b1/boto3_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-05 06:20:52.000000 boto3-utils-0.4.0b1/boto3_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-05 06:20:52.000000 boto3-utils-0.4.0b1/boto3_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-05 06:20:52.000000 boto3-utils-0.4.0b1/boto3_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 06:20:52.239248 boto3-utils-0.4.0b1/boto3utils/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/boto3utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18048 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/boto3utils/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/boto3utils/s3inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/boto3utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/boto3utils/stepfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/boto3utils/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-05 06:20:52.239248 boto3-utils-0.4.0b1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1225 2022-11-05 06:20:43.000000 boto3-utils-0.4.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:01:17.295945 boto3-utils-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 03:01:17.295945 boto3-utils-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:01:17.295945 boto3-utils-0.4.1/boto3_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 03:01:17.000000 boto3-utils-0.4.1/boto3_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-01 03:01:17.000000 boto3-utils-0.4.1/boto3_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 03:01:17.000000 boto3-utils-0.4.1/boto3_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 03:01:17.000000 boto3-utils-0.4.1/boto3_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 03:01:17.000000 boto3-utils-0.4.1/boto3_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:01:17.295945 boto3-utils-0.4.1/boto3utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/boto3utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/boto3utils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/boto3utils/s3inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/boto3utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/boto3utils/stepfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/boto3utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:01:17.295945 boto3-utils-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-06-01 03:01:06.000000 boto3-utils-0.4.1/setup.py
```

### Comparing `boto3-utils-0.4.0b1/LICENSE` & `boto3-utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-utils-0.4.0b1/README.md` & `boto3-utils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `boto3-utils-0.4.0b1/boto3utils/s3.py` & `boto3-utils-0.4.1/boto3utils/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,21 @@
         return 'https://%s.s3.%s.amazonaws.com/%s' % (parts['bucket'], region,
                                                       parts['key'])
 
     def exists(self, url):
         """ Check if this URL exists on S3 """
         parts = self.urlparse(url)
         try:
-            self.s3.head_object(Bucket=parts['bucket'], Key=parts['key'])
+            kwargs = {}
+            if self.requester_pays:
+                kwargs["RequestPayer"] = "requester"
+
+            self.s3.head_object(Bucket=parts['bucket'],
+                                Key=parts['key'],
+                                **kwargs)
             return True
         except ClientError as exc:
             if exc.response['Error']['Code'] != '404':
                 raise
             return False
 
     def get_bucket_region(self, bucket_name):
@@ -144,14 +150,16 @@
         logger.debug("Retrieving object attributes for %s", uri)
 
         extra_args = deepcopy(
             s3_uri["parameters"]) if "parameters" in s3_uri else {}
         if kwargs:
             for k in kwargs:
                 extra_args[k] = kwargs[k]
+        if self.requester_pays:
+            extra_args["RequestPayer"] = "requester"
 
         response = self.s3.get_object_attributes(
             Bucket=s3_uri["bucket"],
             Key=s3_uri["key"],
             ObjectAttributes=["ETag", "Checksum", "ObjectSize", "ObjectParts"],
             **extra_args)
 
@@ -233,15 +241,20 @@
                 meta[key] = result[key]
 
         return (fout, meta)
 
     def read(self, url):
         """ Read object from s3 """
         parts = self.urlparse(url)
-        response = self.get_object(parts['bucket'], parts['key'])
+        kwargs = {}
+        if self.requester_pays:
+            kwargs["RequestPayer"] = "requester"
+        response = self.get_object(parts['bucket'],
+                                   parts['key'],
+                                   extra_args=kwargs)
         body = response['Body'].read()
         if op.splitext(parts['key'])[1] == '.gz':
             body = GzipFile(None, 'rb', fileobj=BytesIO(body)).read()
         return body.decode('utf-8')
 
     def read_json(self, url):
         """ Download object from S3 as JSON """
@@ -265,14 +278,17 @@
         kwargs = {'Bucket': parts['bucket']}
 
         # If the prefix is a single string (not a tuple of strings), we can
         # do the filtering directly in the S3 API.
         if isinstance(parts['key'], str):
             kwargs['Prefix'] = parts['key']
 
+        if self.requester_pays:
+            kwargs["RequestPayer"] = "requester"
+
         while True:
             # The S3 API response is a large blob of metadata.
             # 'Contents' contains information about the listed objects.
             resp = self.s3.list_objects_v2(**kwargs)
             try:
                 contents = resp['Contents']
             except KeyError:
```

### Comparing `boto3-utils-0.4.0b1/boto3utils/s3inventory.py` & `boto3-utils-0.4.1/boto3utils/s3inventory.py`

 * *Files identical despite different names*

### Comparing `boto3-utils-0.4.0b1/boto3utils/secrets.py` & `boto3-utils-0.4.1/boto3utils/secrets.py`

 * *Files identical despite different names*

### Comparing `boto3-utils-0.4.0b1/boto3utils/stepfunctions.py` & `boto3-utils-0.4.1/boto3utils/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `boto3-utils-0.4.0b1/setup.py` & `boto3-utils-0.4.1/setup.py`

 * *Files identical despite different names*

