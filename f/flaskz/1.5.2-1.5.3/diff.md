# Comparing `tmp/flaskz-1.5.2.tar.gz` & `tmp/flaskz-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.5.2.tar", last modified: Wed May 17 03:00:06 2023, max compression
+gzip compressed data, was "flaskz-1.5.3.tar", last modified: Thu Jun  1 02:01:12 2023, max compression
```

## Comparing `flaskz-1.5.2.tar` & `flaskz-1.5.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.560098 flaskz-1.5.2/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.5.2/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     6223 2023-05-17 03:00:06.560374 flaskz-1.5.2/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     5783 2023-05-17 02:59:18.000000 flaskz-1.5.2/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.5.2/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      704 2023-05-17 03:00:06.561550 flaskz-1.5.2/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.529600 flaskz-1.5.2/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.533692 flaskz-1.5.2/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-05-17 02:59:24.000000 flaskz-1.5.2/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.537079 flaskz-1.5.2/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.5.2/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.5.2/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.539666 flaskz-1.5.2/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.5.2/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.5.2/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)     9693 2023-04-26 10:31:33.000000 flaskz-1.5.2/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.540518 flaskz-1.5.2/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2256 2023-05-15 03:14:20.000000 flaskz-1.5.2/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.544173 flaskz-1.5.2/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5488 2023-05-17 02:06:29.000000 flaskz-1.5.2/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    26672 2023-05-17 02:34:00.000000 flaskz-1.5.2/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.5.2/src/flaskz/models/_model.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6450 2023-05-15 09:29:19.000000 flaskz-1.5.2/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.5.2/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.547035 flaskz-1.5.2/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    19354 2023-04-27 11:45:35.000000 flaskz-1.5.2/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.5.2/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.5.2/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.558693 flaskz-1.5.2/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-05-10 07:01:15.000000 flaskz-1.5.2/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.5.2/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.5.2/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.5.2/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.5.2/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.5.2/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.5.2/src/flaskz/utils/_magic.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6078 2023-05-10 09:11:49.000000 flaskz-1.5.2/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7742 2023-05-16 02:51:46.000000 flaskz-1.5.2/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.5.2/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.5.2/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-05-17 03:00:06.535793 flaskz-1.5.2/src/flaskz.egg-info/
--rwxrwxrwx   0 taozh      (501) staff       (20)     6223 2023-05-17 03:00:06.000000 flaskz-1.5.2/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-05-17 03:00:06.000000 flaskz-1.5.2/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-05-17 03:00:06.000000 flaskz-1.5.2/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-05-17 03:00:06.000000 flaskz-1.5.2/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-05-17 03:00:06.000000 flaskz-1.5.2/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.719781 flaskz-1.5.3/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.5.3/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     6475 2023-06-01 02:01:12.720056 flaskz-1.5.3/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6038 2023-06-01 01:51:10.000000 flaskz-1.5.3/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.5.3/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      704 2023-06-01 02:01:12.721183 flaskz-1.5.3/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.683712 flaskz-1.5.3/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.688234 flaskz-1.5.3/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-06-01 01:51:53.000000 flaskz-1.5.3/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.693620 flaskz-1.5.3/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.5.3/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.5.3/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.697041 flaskz-1.5.3/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.5.3/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.5.3/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)     9693 2023-04-26 10:31:33.000000 flaskz-1.5.3/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.698109 flaskz-1.5.3/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2256 2023-05-15 03:14:20.000000 flaskz-1.5.3/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.703009 flaskz-1.5.3/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5488 2023-05-17 02:06:29.000000 flaskz-1.5.3/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    26672 2023-05-17 02:34:00.000000 flaskz-1.5.3/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.5.3/src/flaskz/models/_model.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6450 2023-05-27 16:43:07.000000 flaskz-1.5.3/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.5.3/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.706321 flaskz-1.5.3/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    19354 2023-04-27 11:45:35.000000 flaskz-1.5.3/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.5.3/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.5.3/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.718852 flaskz-1.5.3/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-05-10 07:01:15.000000 flaskz-1.5.3/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.5.3/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.5.3/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.5.3/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.5.3/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.5.3/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.5.3/src/flaskz/utils/_magic.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6497 2023-05-30 05:37:32.000000 flaskz-1.5.3/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7742 2023-05-16 02:51:46.000000 flaskz-1.5.3/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.5.3/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.5.3/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.691937 flaskz-1.5.3/src/flaskz.egg-info/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6475 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.5.2/LICENSE` & `flaskz-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/PKG-INFO` & `flaskz-1.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.5.2
+Version: 1.5.3
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,17 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5.3** `2023/06/01`
+    - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
+    - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 重构`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
```

### Comparing `flaskz-1.5.2/README.md` & `flaskz-1.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5.3** `2023/06/01`
+    - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
+    - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 重构`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
```

### Comparing `flaskz-1.5.2/setup.cfg` & `flaskz-1.5.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.5.2
+version = 1.5.3
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.5.2/src/flaskz/auth/_jws.py` & `flaskz-1.5.3/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/ext/cypher.py` & `flaskz-1.5.3/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/ext/ssh.py` & `flaskz-1.5.3/src/flaskz/ext/ssh.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/log/__init__.py` & `flaskz-1.5.3/src/flaskz/log/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/models/__init__.py` & `flaskz-1.5.3/src/flaskz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/models/_base.py` & `flaskz-1.5.3/src/flaskz/models/_base.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/models/_model.py` & `flaskz-1.5.3/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/models/_util.py` & `flaskz-1.5.3/src/flaskz/models/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/res_status_codes.py` & `flaskz-1.5.3/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/rest/__init__.py` & `flaskz-1.5.3/src/flaskz/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/rest/_mgmt.py` & `flaskz-1.5.3/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/rest/_util.py` & `flaskz-1.5.3/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_app.py` & `flaskz-1.5.3/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_cache.py` & `flaskz-1.5.3/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_cls.py` & `flaskz-1.5.3/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_common.py` & `flaskz-1.5.3/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_func.py` & `flaskz-1.5.3/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_magic.py` & `flaskz-1.5.3/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_request_api.py` & `flaskz-1.5.3/src/flaskz/utils/_request_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,16 +58,24 @@
         _url = url
 
     if base_url:
         base_url = base_url.rstrip('/')
         _url = _url.lstrip('/')
         _url = base_url + '/' + _url
 
-    if is_dict(url_params):
-        _url = append_url_search_params(_url, url_params)
+    if is_dict(url_params):  # @2023-05-30 update variables(for replace)
+        _url = _url.format(**url_params)
+
+    url_variables = kwargs.get('url_variables', None)  # @2023-05-30 add variables(for replace)
+    if is_dict(url_variables):
+        _url = _url.format(**url_variables)
+
+    url_search_params = kwargs.get('url_search_params', None)  # @2023-05-30 add search_params(for append)
+    if url_search_params is not None:
+        _url = append_url_search_params(_url, url_search_params)
 
     _method = _method.strip().upper()
 
     flaskz_logger.debug('Api request:\n   url={url}\n   method={method}\n   data={data}\n   json={json}'.format(**{
         'url': _url,
         'method': _method,
         'data': kwargs.get('data'),
```

### Comparing `flaskz-1.5.2/src/flaskz/utils/_request_args.py` & `flaskz-1.5.3/src/flaskz/utils/_request_args.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_response.py` & `flaskz-1.5.3/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz/utils/_timer.py` & `flaskz-1.5.3/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.2/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.5.3/src/flaskz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.5.2
+Version: 1.5.3
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,17 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5.3** `2023/06/01`
+    - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
+    - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 重构`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
```

### Comparing `flaskz-1.5.2/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.5.3/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

