# Comparing `tmp/django_cqrs-2.5.0.tar.gz` & `tmp/django_cqrs-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cqrs-2.5.0.tar", max compression
+gzip compressed data, was "django_cqrs-2.6.0.tar", max compression
```

## Comparing `django_cqrs-2.5.0.tar` & `django_cqrs-2.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11369 2023-04-07 09:19:27.302033 django_cqrs-2.5.0/LICENSE
--rw-r--r--   0        0        0     9066 2023-04-07 09:19:27.302033 django_cqrs-2.5.0/README.md
--rw-r--r--   0        0        0      196 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/__init__.py
--rw-r--r--   0        0        0     7567 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/_validation.py
--rw-r--r--   0        0        0     1842 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/admin.py
--rw-r--r--   0        0        0      289 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/apps.py
--rw-r--r--   0        0        0      728 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/constants.py
--rw-r--r--   0        0        0       60 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/controller/__init__.py
--rw-r--r--   0        0        0     3086 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/controller/consumer.py
--rw-r--r--   0        0        0      285 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/controller/producer.py
--rw-r--r--   0        0        0      698 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/correlation.py
--rw-r--r--   0        0        0     4758 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/dataclasses.py
--rw-r--r--   0        0        0     2229 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/delay.py
--rw-r--r--   0        0        0       60 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/__init__.py
--rw-r--r--   0        0        0       60 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/__init__.py
--rw-r--r--   0        0        0     4084 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_bulk_dump.py
--rw-r--r--   0        0        0     3564 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_bulk_load.py
--rw-r--r--   0        0        0     5915 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_consume.py
--rw-r--r--   0        0        0     5149 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_dead_letters.py
--rw-r--r--   0        0        0     1545 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
--rw-r--r--   0        0        0     2397 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
--rw-r--r--   0        0        0     1178 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
--rw-r--r--   0        0        0     2502 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_diff_master.py
--rw-r--r--   0        0        0     1776 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_diff_replica.py
--rw-r--r--   0        0        0     2132 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_diff_sync.py
--rw-r--r--   0        0        0     4319 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_sync.py
--rw-r--r--   0        0        0      484 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/management/utils.py
--rw-r--r--   0        0        0    12661 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/managers.py
--rw-r--r--   0        0        0     5321 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/metas.py
--rw-r--r--   0        0        0    17101 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/mixins.py
--rw-r--r--   0        0        0     1392 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/registries.py
--rw-r--r--   0        0        0     5197 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/signals.py
--rw-r--r--   0        0        0     1855 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/tracker.py
--rw-r--r--   0        0        0      545 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/transport/__init__.py
--rw-r--r--   0        0        0     1003 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/transport/base.py
--rw-r--r--   0        0        0     6561 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/transport/kombu.py
--rw-r--r--   0        0        0     3250 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/transport/mixins.py
--rw-r--r--   0        0        0      316 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/transport/mock.py
--rw-r--r--   0        0        0    15323 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/transport/rabbit_mq.py
--rw-r--r--   0        0        0     1501 2023-04-07 09:19:27.306033 django_cqrs-2.5.0/dj_cqrs/utils.py
--rw-r--r--   0        0        0     2956 2023-04-07 09:21:46.757298 django_cqrs-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    10645 1970-01-01 00:00:00.000000 django_cqrs-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11369 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/LICENSE
+-rw-r--r--   0        0        0     9066 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/README.md
+-rw-r--r--   0        0        0      196 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/__init__.py
+-rw-r--r--   0        0        0     7567 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/_validation.py
+-rw-r--r--   0        0        0     1842 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/admin.py
+-rw-r--r--   0        0        0      289 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/apps.py
+-rw-r--r--   0        0        0      728 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/constants.py
+-rw-r--r--   0        0        0       60 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/controller/__init__.py
+-rw-r--r--   0        0        0     3086 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/controller/consumer.py
+-rw-r--r--   0        0        0      285 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/controller/producer.py
+-rw-r--r--   0        0        0      698 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/correlation.py
+-rw-r--r--   0        0        0     4758 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/dataclasses.py
+-rw-r--r--   0        0        0     2229 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/delay.py
+-rw-r--r--   0        0        0       60 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/__init__.py
+-rw-r--r--   0        0        0     4084 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_dump.py
+-rw-r--r--   0        0        0     3564 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_load.py
+-rw-r--r--   0        0        0     5915 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_consume.py
+-rw-r--r--   0        0        0     5149 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_dead_letters.py
+-rw-r--r--   0        0        0     1545 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
+-rw-r--r--   0        0        0     2397 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
+-rw-r--r--   0        0        0     1178 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
+-rw-r--r--   0        0        0     2502 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_master.py
+-rw-r--r--   0        0        0     1776 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_replica.py
+-rw-r--r--   0        0        0     2132 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_sync.py
+-rw-r--r--   0        0        0     4319 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_sync.py
+-rw-r--r--   0        0        0      484 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/utils.py
+-rw-r--r--   0        0        0    12661 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/managers.py
+-rw-r--r--   0        0        0     5321 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/metas.py
+-rw-r--r--   0        0        0    17101 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/mixins.py
+-rw-r--r--   0        0        0     1392 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/registries.py
+-rw-r--r--   0        0        0     5197 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/signals.py
+-rw-r--r--   0        0        0     1855 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/tracker.py
+-rw-r--r--   0        0        0      545 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/__init__.py
+-rw-r--r--   0        0        0     1003 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/base.py
+-rw-r--r--   0        0        0     6561 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/kombu.py
+-rw-r--r--   0        0        0     3250 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/mixins.py
+-rw-r--r--   0        0        0      316 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/mock.py
+-rw-r--r--   0        0        0    15323 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/rabbit_mq.py
+-rw-r--r--   0        0        0     1501 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/utils.py
+-rw-r--r--   0        0        0     3214 2023-06-01 06:52:48.383820 django_cqrs-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10343 1970-01-01 00:00:00.000000 django_cqrs-2.6.0/PKG-INFO
```

### Comparing `django_cqrs-2.5.0/LICENSE` & `django_cqrs-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/README.md` & `django_cqrs-2.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -206,26 +206,26 @@
     kubectl exec -i MASTER_CONTAINER -- python manage.py cqrs_deleted_diff_master |
     kubectl exec -i REPLICA_CONTAINER -- python manage.py cqrs_deleted_sync_replica
 ```
 
 Development
 ===========
 
-1. Python >= 3.7
+1. Python >= 3.8
 2. Install dependencies `requirements/dev.txt`
 3. We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
 For convenience you may run `isort .` to order imports.
 
 
 Testing
 =======
 
 Unit testing
 ------
-1. Python >= 3.7
+1. Python >= 3.8
 2. Install dependencies `requirements/test.txt`
 3. `export PYTHONPATH=/your/path/to/django-cqrs/`
 
 Run tests with various RDBMS:
 - `cd integration_tests`
 - `DB=postgres docker-compose -f docker-compose.yml -f rdbms.yml run app_test`
 - `DB=mysql docker-compose -f docker-compose.yml -f rdbms.yml run app_test`
```

### Comparing `django_cqrs-2.5.0/dj_cqrs/_validation.py` & `django_cqrs-2.6.0/dj_cqrs/_validation.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/admin.py` & `django_cqrs-2.6.0/dj_cqrs/admin.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/constants.py` & `django_cqrs-2.6.0/dj_cqrs/constants.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/controller/consumer.py` & `django_cqrs-2.6.0/dj_cqrs/controller/consumer.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/correlation.py` & `django_cqrs-2.6.0/dj_cqrs/correlation.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/dataclasses.py` & `django_cqrs-2.6.0/dj_cqrs/dataclasses.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/delay.py` & `django_cqrs-2.6.0/dj_cqrs/delay.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_bulk_dump.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_dump.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_bulk_load.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_load.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_consume.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_consume.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_dead_letters.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_dead_letters.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_diff_master.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_master.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_diff_replica.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_diff_sync.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_sync.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/management/commands/cqrs_sync.py` & `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_sync.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/managers.py` & `django_cqrs-2.6.0/dj_cqrs/managers.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/metas.py` & `django_cqrs-2.6.0/dj_cqrs/metas.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/mixins.py` & `django_cqrs-2.6.0/dj_cqrs/mixins.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/registries.py` & `django_cqrs-2.6.0/dj_cqrs/registries.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/signals.py` & `django_cqrs-2.6.0/dj_cqrs/signals.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/tracker.py` & `django_cqrs-2.6.0/dj_cqrs/tracker.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/transport/__init__.py` & `django_cqrs-2.6.0/dj_cqrs/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/transport/base.py` & `django_cqrs-2.6.0/dj_cqrs/transport/base.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/transport/kombu.py` & `django_cqrs-2.6.0/dj_cqrs/transport/kombu.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/transport/mixins.py` & `django_cqrs-2.6.0/dj_cqrs/transport/mixins.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/transport/rabbit_mq.py` & `django_cqrs-2.6.0/dj_cqrs/transport/rabbit_mq.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/dj_cqrs/utils.py` & `django_cqrs-2.6.0/dj_cqrs/utils.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.5.0/pyproject.toml` & `django_cqrs-2.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cqrs"
-version = "2.5.0"
+version = "2.6.0"
 description = "Django CQRS data synchronisation"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_cqrs" }
 ]
 readme = "./README.md"
@@ -15,15 +15,14 @@
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: Unix',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Communications',
     'Topic :: Database',
 ]
@@ -32,42 +31,43 @@
     "cqrs",
     "sql",
     "mixin",
     "amqp",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4"
+python = ">=3.8,<4"
 django = ">=3.2"
 pika = ">=1.0.0"
 kombu = ">=4.6.*"
 ujson = ">=5.4.0"
 django-model-utils = ">=4.0.0"
 python-dateutil = ">=2.4"
 watchfiles = "^0.18.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.2.0,<8"
 pytest-cov = ">=2.10.1,<5"
-pytest-mock = "^3.3.1"
+pytest-mock = "^3.10"
 pytest-django = ">=4.4.0"
 pytest-randomly = ">=3.12"
 pytest-deadfixtures = "^2.2.1"
 coverage = {extras = ["toml"], version = ">=5.3,<7"}
 flake8 = ">=3.8,<6"
 flake8-bugbear = ">=20,<23"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "~2.1"
 flake8-future-import = "~0.4"
-flake8-isort = "^5.0"
+flake8-isort = "^6.0"
 flake8-broken-line = ">=0.3,<0.7"
 flake8-comprehensions = "^3.10.1"
 flake8-debugger = "^4.1.2"
 flake8-eradicate = "^1.4.0"
 flake8-string-format = "^0.3.0"
+flake8-pyproject = "^1.2.3"
 djangorestframework = ">=3.12"
 isort = "^5.10"
 django-mptt = "^0.14.0"
 importlib-metadata = "<5"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = ">=1.4"
@@ -100,8 +100,25 @@
 use_parentheses = true
 include_trailing_comma = true
 line_length = 100
 lines_after_imports = 2
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
+
+[tool.flake8]
+exclude = [
+    ".idea",
+    ".vscode",
+    ".git",
+    "pg_data",
+    "venv",
+    "*.eggs",
+    "*.egg",
+    "*.egg-info",
+    "examples/*migrations/*",
+]
+show-source = true
+max-line-length = 100
+max-cognitive-complexity = 20
+ignore = ["FI1", "W503", "W605"]
```

### Comparing `django_cqrs-2.5.0/PKG-INFO` & `django_cqrs-2.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 Metadata-Version: 2.1
 Name: django-cqrs
-Version: 2.5.0
+Version: 2.6.0
 Summary: Django CQRS data synchronisation
 Home-page: https://django-cqrs.readthedocs.org
 License: Apache-2.0
 Keywords: django,cqrs,sql,mixin,amqp
 Author: CloudBlue LLC
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications
 Classifier: Topic :: Database
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-model-utils (>=4.0.0)
 Requires-Dist: kombu (>=4.6)
 Requires-Dist: pika (>=1.0.0)
 Requires-Dist: python-dateutil (>=2.4)
@@ -246,26 +240,26 @@
     kubectl exec -i MASTER_CONTAINER -- python manage.py cqrs_deleted_diff_master |
     kubectl exec -i REPLICA_CONTAINER -- python manage.py cqrs_deleted_sync_replica
 ```
 
 Development
 ===========
 
-1. Python >= 3.7
+1. Python >= 3.8
 2. Install dependencies `requirements/dev.txt`
 3. We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
 For convenience you may run `isort .` to order imports.
 
 
 Testing
 =======
 
 Unit testing
 ------
-1. Python >= 3.7
+1. Python >= 3.8
 2. Install dependencies `requirements/test.txt`
 3. `export PYTHONPATH=/your/path/to/django-cqrs/`
 
 Run tests with various RDBMS:
 - `cd integration_tests`
 - `DB=postgres docker-compose -f docker-compose.yml -f rdbms.yml run app_test`
 - `DB=mysql docker-compose -f docker-compose.yml -f rdbms.yml run app_test`
```

