# Comparing `tmp/nginx-set-conf-equitania-0.8.2.tar.gz` & `tmp/nginx-set-conf-equitania-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.8.2.tar", last modified: Thu May 25 10:00:06 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.8.3.tar", last modified: Thu Jun  1 11:54:45 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.8.2.tar` & `nginx-set-conf-equitania-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-25 10:00:06.865710 nginx-set-conf-equitania-0.8.2/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.8.2/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-25 10:00:06.865259 nginx-set-conf-equitania-0.8.2/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.8.2/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-25 10:00:06.859965 nginx-set-conf-equitania-0.8.2/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    21092 2023-05-25 09:54:50.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     4006 2023-05-02 13:29:17.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-25 10:00:06.864196 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-25 10:00:06.865782 nginx-set-conf-equitania-0.8.2/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-25 09:46:50.000000 nginx-set-conf-equitania-0.8.2/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-06-01 11:54:45.594727 nginx-set-conf-equitania-0.8.3/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.8.3/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-06-01 11:54:45.594399 nginx-set-conf-equitania-0.8.3/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.8.3/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-06-01 11:54:45.589441 nginx-set-conf-equitania-0.8.3/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    21092 2023-05-25 09:54:50.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     4006 2023-05-02 13:29:17.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-06-01 11:54:45.593795 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-06-01 11:54:45.000000 nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-06-01 11:54:45.594819 nginx-set-conf-equitania-0.8.3/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      903 2023-06-01 11:54:09.000000 nginx-set-conf-equitania-0.8.3/setup.py
```

### Comparing `nginx-set-conf-equitania-0.8.2/LICENSE.txt` & `nginx-set-conf-equitania-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.2/PKG-INFO` & `nginx-set-conf-equitania-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.2
+Version: 0.8.3
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.8.2/README.md` & `nginx-set-conf-equitania-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.2/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.8.3/nginx_set_conf/config_templates.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.2/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.8.3/nginx_set_conf/nginx_set_conf.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.2/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.8.3/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.8.3/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.2
+Version: 0.8.3
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.8.2/setup.py` & `nginx-set-conf-equitania-0.8.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.8.2",
+    version="0.8.3",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx with/without pagespeed for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
@@ -19,11 +19,11 @@
     ],
     python_requires='>=3.6',
     entry_points='''
     [console_scripts]
     nginx-set-conf=nginx_set_conf.nginx_set_conf:start_nginx_set_conf
     ''',
     install_requires=[
-        'click>=8.1.3',
+        'click>=8.0.4',
         'PyYaml>=5.4.1'
     ]
 )
```

