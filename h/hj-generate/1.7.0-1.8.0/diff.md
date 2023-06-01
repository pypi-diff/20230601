# Comparing `tmp/hj-generate-1.7.0.tar.gz` & `tmp/hj-generate-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-1.7.0.tar", last modified: Thu Jun  1 14:32:56 2023, max compression
+gzip compressed data, was "hj-generate-1.8.0.tar", last modified: Thu Jun  1 14:46:02 2023, max compression
```

## Comparing `hj-generate-1.7.0.tar` & `hj-generate-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:32:56.617735 hj-generate-1.7.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:32:56.617438 hj-generate-1.7.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:32:56.613954 hj-generate-1.7.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.7.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     1838 2023-06-01 14:32:53.000000 hj-generate-1.7.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:32:56.615006 hj-generate-1.7.0/generate/templates/
--rw-r--r--   0 hj         (501) staff       (20)      470 2023-06-01 13:34:18.000000 hj-generate-1.7.0/generate/templates/controller.tpl
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 13:52:14.000000 hj-generate-1.7.0/generate/templates/service.tpl
--rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-1.7.0/generate/templates/sql.tpl
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:32:56.616993 hj-generate-1.7.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:32:56.000000 hj-generate-1.7.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 14:32:56.000000 hj-generate-1.7.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:32:56.000000 hj-generate-1.7.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:32:56.000000 hj-generate-1.7.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:32:56.000000 hj-generate-1.7.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:32:56.000000 hj-generate-1.7.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:32:56.617823 hj-generate-1.7.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 14:32:53.000000 hj-generate-1.7.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:46:02.284848 hj-generate-1.8.0/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:46:02.284217 hj-generate-1.8.0/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:46:02.281588 hj-generate-1.8.0/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.8.0/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     1868 2023-06-01 14:45:15.000000 hj-generate-1.8.0/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:46:02.282431 hj-generate-1.8.0/generate/templates/
+-rw-r--r--   0 hj         (501) staff       (20)      465 2023-06-01 14:37:57.000000 hj-generate-1.8.0/generate/templates/controller.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 13:52:14.000000 hj-generate-1.8.0/generate/templates/service.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-1.8.0/generate/templates/sql.tpl
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:46:02.283855 hj-generate-1.8.0/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:46:02.000000 hj-generate-1.8.0/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 14:46:02.000000 hj-generate-1.8.0/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:46:02.000000 hj-generate-1.8.0/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:46:02.000000 hj-generate-1.8.0/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:46:02.000000 hj-generate-1.8.0/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:46:02.000000 hj-generate-1.8.0/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:46:02.285161 hj-generate-1.8.0/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 14:45:59.000000 hj-generate-1.8.0/setup.py
```

### Comparing `hj-generate-1.7.0/generate/generate_code.py` & `hj-generate-1.8.0/generate/generate_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 # 创建模板环境
 def generate_code(data):
     current_file_path = os.path.abspath(__file__)
     current_package_path = os.path.dirname(current_file_path)
     # print(current_package_path)
     env = Environment(loader=FileSystemLoader(current_package_path + os.sep + 'templates'))
-    controller_template = env.get_template('controller.tpl')
+    controller_template = env.get_template('./controllers/controller.tpl')
 
     controller_output = controller_template.render(data)
 
     # 生成文件
     with open(data.get("name") + '_controller.py', 'w') as f:
         f.write(controller_output)
 
-    service_template = env.get_template('service.tpl')
+    service_template = env.get_template('./service/service.tpl')
 
     service_output = service_template.render(data)
 
     # 生成文件
     with open(data.get("name") + '_service.py', 'w') as f:
         f.write(service_output)
 
-    sql_template = env.get_template('sql.tpl')
+    sql_template = env.get_template('./sql/sql.tpl')
 
     sql_output = sql_template.render(data)
 
     # 生成文件
     with open(data.get("name") + '_sql.py', 'w') as f:
         f.write(sql_output)
```

