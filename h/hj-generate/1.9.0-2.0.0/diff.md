# Comparing `tmp/hj-generate-1.9.0.tar.gz` & `tmp/hj-generate-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-1.9.0.tar", last modified: Thu Jun  1 14:48:53 2023, max compression
+gzip compressed data, was "hj-generate-2.0.0.tar", last modified: Thu Jun  1 14:52:55 2023, max compression
```

## Comparing `hj-generate-1.9.0.tar` & `hj-generate-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:48:53.471045 hj-generate-1.9.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:48:53.470700 hj-generate-1.9.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:48:53.466609 hj-generate-1.9.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.9.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     1862 2023-06-01 14:48:43.000000 hj-generate-1.9.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:48:53.467321 hj-generate-1.9.0/generate/templates/
--rw-r--r--   0 hj         (501) staff       (20)      465 2023-06-01 14:37:57.000000 hj-generate-1.9.0/generate/templates/controller.tpl
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 13:52:14.000000 hj-generate-1.9.0/generate/templates/service.tpl
--rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-1.9.0/generate/templates/sql.tpl
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:48:53.470183 hj-generate-1.9.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:48:53.000000 hj-generate-1.9.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 14:48:53.000000 hj-generate-1.9.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:48:53.000000 hj-generate-1.9.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:48:53.000000 hj-generate-1.9.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:48:53.000000 hj-generate-1.9.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:48:53.000000 hj-generate-1.9.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:48:53.471190 hj-generate-1.9.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 14:48:43.000000 hj-generate-1.9.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:52:55.015869 hj-generate-2.0.0/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:52:55.015480 hj-generate-2.0.0/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:52:55.012541 hj-generate-2.0.0/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-2.0.0/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     1907 2023-06-01 14:52:27.000000 hj-generate-2.0.0/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:52:55.013263 hj-generate-2.0.0/generate/templates/
+-rw-r--r--   0 hj         (501) staff       (20)      465 2023-06-01 14:37:57.000000 hj-generate-2.0.0/generate/templates/controller.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 13:52:14.000000 hj-generate-2.0.0/generate/templates/service.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-2.0.0/generate/templates/sql.tpl
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:52:55.015123 hj-generate-2.0.0/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:52:54.000000 hj-generate-2.0.0/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 14:52:54.000000 hj-generate-2.0.0/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:52:54.000000 hj-generate-2.0.0/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:52:54.000000 hj-generate-2.0.0/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:52:54.000000 hj-generate-2.0.0/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:52:54.000000 hj-generate-2.0.0/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:52:55.015982 hj-generate-2.0.0/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 14:52:38.000000 hj-generate-2.0.0/setup.py
```

### Comparing `hj-generate-1.9.0/generate/generate_code.py` & `hj-generate-2.0.0/generate/generate_code.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 
 # 创建模板环境
 def generate_code(data):
     current_file_path = os.path.abspath(__file__)
     current_package_path = os.path.dirname(current_file_path)
     # print(current_package_path)
     env = Environment(loader=FileSystemLoader(current_package_path + os.sep + 'templates'))
-    controller_template = env.get_template('controllers/controller.tpl')
+    controller_template = env.get_template('controller.tpl')
 
     controller_output = controller_template.render(data)
 
     # 生成文件
-    with open(data.get("name") + '_controller.py', 'w') as f:
+    with open('./controllers' + os.sep + data.get("name") + '_controller.py', 'w') as f:
         f.write(controller_output)
 
-    service_template = env.get_template('service/service.tpl')
+    service_template = env.get_template('service.tpl')
 
     service_output = service_template.render(data)
 
     # 生成文件
-    with open(data.get("name") + '_service.py', 'w') as f:
+    with open('./service' + os.sep + data.get("name") + '_service.py', 'w') as f:
         f.write(service_output)
 
-    sql_template = env.get_template('sql/sql.tpl')
+    sql_template = env.get_template('sql.tpl')
 
     sql_output = sql_template.render(data)
 
     # 生成文件
-    with open(data.get("name") + '_sql.py', 'w') as f:
+    with open('./sql' + os.sep + data.get("name") + '_sql.py', 'w') as f:
         f.write(sql_output)
 
 
 def underscore_to_camelcase(text):
     parts = text.split('_')
     return ''.join(word.capitalize() for word in parts)
```

