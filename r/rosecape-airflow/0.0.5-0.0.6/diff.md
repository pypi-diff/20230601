# Comparing `tmp/rosecape_airflow-0.0.5.tar.gz` & `tmp/rosecape_airflow-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosecape_airflow-0.0.5.tar", last modified: Mon May 29 17:33:59 2023, max compression
+gzip compressed data, was "rosecape_airflow-0.0.6.tar", last modified: Thu Jun  1 17:28:45 2023, max compression
```

## Comparing `rosecape_airflow-0.0.5.tar` & `rosecape_airflow-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 17:33:59.282139 rosecape_airflow-0.0.5/
--rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-05-29 17:33:59.281998 rosecape_airflow-0.0.5/PKG-INFO
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 17:33:59.280412 rosecape_airflow-0.0.5/rosecape_airflow/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:02:59.000000 rosecape_airflow-0.0.5/rosecape_airflow/__init__.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 17:33:59.281531 rosecape_airflow-0.0.5/rosecape_airflow/aws/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:57.000000 rosecape_airflow-0.0.5/rosecape_airflow/aws/__init__.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     1801 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.5/rosecape_airflow/aws/ec2.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     3941 2023-05-29 14:43:16.000000 rosecape_airflow-0.0.5/rosecape_airflow/aws/ecs.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)    10102 2023-05-29 17:33:24.000000 rosecape_airflow-0.0.5/rosecape_airflow/aws/efs.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 17:33:59.281803 rosecape_airflow-0.0.5/rosecape_airflow/slack/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:52.000000 rosecape_airflow-0.0.5/rosecape_airflow/slack/__init__.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     1507 2023-05-29 12:48:08.000000 rosecape_airflow-0.0.5/rosecape_airflow/slack/task_failed_slack_alert.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 17:33:59.281037 rosecape_airflow-0.0.5/rosecape_airflow.egg-info/
--rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-05-29 17:33:59.000000 rosecape_airflow-0.0.5/rosecape_airflow.egg-info/PKG-INFO
--rw-r--r--   0 nickjoanis   (501) staff       (20)      438 2023-05-29 17:33:59.000000 rosecape_airflow-0.0.5/rosecape_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)        1 2023-05-29 17:33:59.000000 rosecape_airflow-0.0.5/rosecape_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       16 2023-05-29 17:33:59.000000 rosecape_airflow-0.0.5/rosecape_airflow.egg-info/requires.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       17 2023-05-29 17:33:59.000000 rosecape_airflow-0.0.5/rosecape_airflow.egg-info/top_level.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       38 2023-05-29 17:33:59.282185 rosecape_airflow-0.0.5/setup.cfg
--rw-r--r--   0 nickjoanis   (501) staff       (20)      743 2023-05-29 17:33:51.000000 rosecape_airflow-0.0.5/setup.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.809230 rosecape_airflow-0.0.6/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-06-01 17:28:45.809057 rosecape_airflow-0.0.6/PKG-INFO
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.794604 rosecape_airflow-0.0.6/rosecape_airflow/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:02:59.000000 rosecape_airflow-0.0.6/rosecape_airflow/__init__.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.808362 rosecape_airflow-0.0.6/rosecape_airflow/aws/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:57.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/__init__.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     1801 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/ec2.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     3941 2023-05-29 14:43:16.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/ecs.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)    10137 2023-06-01 17:23:56.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/efs.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.808807 rosecape_airflow-0.0.6/rosecape_airflow/slack/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:52.000000 rosecape_airflow-0.0.6/rosecape_airflow/slack/__init__.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     1507 2023-05-29 12:48:08.000000 rosecape_airflow-0.0.6/rosecape_airflow/slack/task_failed_slack_alert.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.795449 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      438 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        1 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       16 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/requires.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       17 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/top_level.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       38 2023-06-01 17:28:45.809300 rosecape_airflow-0.0.6/setup.cfg
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      743 2023-06-01 17:24:06.000000 rosecape_airflow-0.0.6/setup.py
```

### Comparing `rosecape_airflow-0.0.5/rosecape_airflow/aws/ec2.py` & `rosecape_airflow-0.0.6/rosecape_airflow/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.5/rosecape_airflow/aws/ecs.py` & `rosecape_airflow-0.0.6/rosecape_airflow/aws/ecs.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.5/rosecape_airflow/aws/efs.py` & `rosecape_airflow-0.0.6/rosecape_airflow/aws/efs.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :return: EFS filesystem
     :rtype: dict
     """
     hook = AwsHook(aws_conn_id, client_type='efs', region_name=region)
     client = hook.get_client_type()
 
     filesystems = client.describe_file_systems(
-        CreationToken=identifier
+        CreationToken=str(identifier)
     )
 
     if len(filesystems['FileSystems']) > 0:
         return filesystems['FileSystems'][0]
     else:
         return None
     
@@ -47,23 +47,23 @@
     :rtype: dict
     """
 
     hook = AwsHook(aws_conn_id, client_type='efs', region_name=region)
     client = hook.get_client_type()
 
     filesystems = client.describe_file_systems(
-        CreationToken=identifier
+        CreationToken=str(identifier)
     )
 
     if len(filesystems['FileSystems']) > 0:
         filesystem = filesystems['FileSystems'][0]
         logging.info('Filesystem already exists: %s', filesystem)
     else:
         logging.info('Filesystem does not exist yet, creating...')
-        filesystem = client.create_file_system(CreationToken=identifier, **args)
+        filesystem = client.create_file_system(CreationToken=str(identifier), **args)
         logging.info('Filesystem created: %s', filesystem)
 
         waiter_config = {
             "version": 2,
             "waiters": {
                 "EFSLifeCycleStateWaiter": {
                     "operation": "DescribeFileSystems",
@@ -102,15 +102,15 @@
     :rtype: dict
     """
 
     hook = AwsHook(aws_conn_id, client_type='efs', region_name=region)
     client = hook.get_client_type()
 
     filesystems = client.describe_file_systems(
-        CreationToken=identifier
+        CreationToken=str(identifier)
     )
 
     if len(filesystems['FileSystems']) > 0:
         filesystem = filesystems['FileSystems'][0]
         logging.info('Filesystem exists: %s', filesystem)
         client.delete_file_system(FileSystemId=filesystem['FileSystemId'])
         logging.info('Filesystem deleted: %s', filesystem)
@@ -136,15 +136,15 @@
     :rtype: dict
     """
 
     hook = AwsHook(aws_conn_id, client_type='efs', region_name=region)
     client = hook.get_client_type()
 
     filesystems = client.describe_file_systems(
-        CreationToken=identifier
+        CreationToken=str(identifier)
     )
 
     if len(filesystems['FileSystems']) > 0:
         filesystem = filesystems['FileSystems'][0]
         logging.info('Filesystem exists: %s', filesystem)
     else:
         logging.info('Filesystem does not exist: %s', identifier)
@@ -209,15 +209,15 @@
     :rtype: dict
     """
 
     hook = AwsHook(aws_conn_id, client_type='efs', region_name=region)
     client = hook.get_client_type()
 
     filesystems = client.describe_file_systems(
-        CreationToken=identifier
+        CreationToken=str(identifier)
     )
 
     if len(filesystems['FileSystems']) > 0:
         filesystem = filesystems['FileSystems'][0]
         logging.info('Filesystem exists: %s', filesystem)
     else:
         logging.info('Filesystem does not exist: %s', identifier)
@@ -274,15 +274,15 @@
     :rtype: dict
     """
 
     hook = AwsHook(aws_conn_id, client_type='efs', region_name=region)
     client = hook.get_client_type()
 
     filesystems = client.describe_file_systems(
-        CreationToken=identifier
+        CreationToken=str(identifier)
     )
 
     if len(filesystems['FileSystems']) > 0:
         filesystem = filesystems['FileSystems'][0]
         logging.info('Filesystem exists: %s', filesystem)
     else:
         logging.info('Filesystem does not exist: %s', identifier)
```

### Comparing `rosecape_airflow-0.0.5/rosecape_airflow/slack/task_failed_slack_alert.py` & `rosecape_airflow-0.0.6/rosecape_airflow/slack/task_failed_slack_alert.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.5/setup.py` & `rosecape_airflow-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Airflow utilities'
 LONG_DESCRIPTION = 'A package that makes it easy to interact with AWS services from Airflow using PythonOperator'
 
 setup(
     name="rosecape_airflow",
     version=VERSION,
     description=DESCRIPTION,
```

