# Comparing `tmp/hj-generate-2.1.0.tar.gz` & `tmp/hj-generate-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-2.1.0.tar", last modified: Thu Jun  1 15:05:43 2023, max compression
+gzip compressed data, was "hj-generate-2.1.1.tar", last modified: Thu Jun  1 15:07:25 2023, max compression
```

## Comparing `hj-generate-2.1.0.tar` & `hj-generate-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:05:43.575885 hj-generate-2.1.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:05:43.575390 hj-generate-2.1.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:05:43.571658 hj-generate-2.1.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-2.1.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     2396 2023-06-01 15:05:28.000000 hj-generate-2.1.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:05:43.572543 hj-generate-2.1.0/generate/templates/
--rw-r--r--   0 hj         (501) staff       (20)      463 2023-06-01 14:59:14.000000 hj-generate-2.1.0/generate/templates/controller.tpl
--rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-2.1.0/generate/templates/service.tpl
--rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-2.1.0/generate/templates/sql.tpl
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:05:43.574860 hj-generate-2.1.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:05:43.000000 hj-generate-2.1.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 15:05:43.000000 hj-generate-2.1.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 15:05:43.000000 hj-generate-2.1.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 15:05:43.000000 hj-generate-2.1.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 15:05:43.000000 hj-generate-2.1.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 15:05:43.000000 hj-generate-2.1.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 15:05:43.576059 hj-generate-2.1.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 15:05:33.000000 hj-generate-2.1.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:07:25.978465 hj-generate-2.1.1/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:07:25.977933 hj-generate-2.1.1/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:07:25.975203 hj-generate-2.1.1/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-2.1.1/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     2388 2023-06-01 15:07:16.000000 hj-generate-2.1.1/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:07:25.976177 hj-generate-2.1.1/generate/templates/
+-rw-r--r--   0 hj         (501) staff       (20)      463 2023-06-01 14:59:14.000000 hj-generate-2.1.1/generate/templates/controller.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-2.1.1/generate/templates/service.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-2.1.1/generate/templates/sql.tpl
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:07:25.977606 hj-generate-2.1.1/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:07:25.000000 hj-generate-2.1.1/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 15:07:25.000000 hj-generate-2.1.1/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 15:07:25.000000 hj-generate-2.1.1/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 15:07:25.000000 hj-generate-2.1.1/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 15:07:25.000000 hj-generate-2.1.1/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 15:07:25.000000 hj-generate-2.1.1/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 15:07:25.978580 hj-generate-2.1.1/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 15:07:16.000000 hj-generate-2.1.1/setup.py
```

### Comparing `hj-generate-2.1.0/generate/generate_code.py` & `hj-generate-2.1.1/generate/generate_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         f.write(service_output)
 
     # sql
     sql_template = env.get_template('sql.tpl')
 
     sql_output = sql_template.render(data)
     sql_append = """
-    from sql.{{name}}_sql import {{className}}Sql
-    {{varName}}Sql = {{className}}Sql()
+from sql.{{name}}_sql import {{className}}Sql
+{{varName}}Sql = {{className}}Sql()
     """
     sql_str_temp = env.from_string(sql_append)
 
     # 追加
     with open('./sql' + os.sep + '__init__.py', 'a') as f:
         f.write(sql_str_temp.render(data))
```

