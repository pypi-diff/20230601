# Comparing `tmp/hj-generate-2.1.2.tar.gz` & `tmp/hj-generate-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-2.1.2.tar", last modified: Thu Jun  1 15:13:46 2023, max compression
+gzip compressed data, was "hj-generate-2.1.3.tar", last modified: Thu Jun  1 15:15:40 2023, max compression
```

## Comparing `hj-generate-2.1.2.tar` & `hj-generate-2.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:13:46.599226 hj-generate-2.1.2/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:13:46.598844 hj-generate-2.1.2/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:13:46.596004 hj-generate-2.1.2/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-2.1.2/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     2996 2023-06-01 15:13:38.000000 hj-generate-2.1.2/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:13:46.596706 hj-generate-2.1.2/generate/templates/
--rw-r--r--   0 hj         (501) staff       (20)      463 2023-06-01 14:59:14.000000 hj-generate-2.1.2/generate/templates/controller.tpl
--rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-2.1.2/generate/templates/service.tpl
--rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-2.1.2/generate/templates/sql.tpl
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:13:46.598377 hj-generate-2.1.2/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:13:46.000000 hj-generate-2.1.2/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 15:13:46.000000 hj-generate-2.1.2/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 15:13:46.000000 hj-generate-2.1.2/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 15:13:46.000000 hj-generate-2.1.2/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 15:13:46.000000 hj-generate-2.1.2/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 15:13:46.000000 hj-generate-2.1.2/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 15:13:46.599333 hj-generate-2.1.2/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 15:13:38.000000 hj-generate-2.1.2/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:15:40.484349 hj-generate-2.1.3/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:15:40.483811 hj-generate-2.1.3/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:15:40.479679 hj-generate-2.1.3/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-2.1.3/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     2995 2023-06-01 15:14:58.000000 hj-generate-2.1.3/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:15:40.480497 hj-generate-2.1.3/generate/templates/
+-rw-r--r--   0 hj         (501) staff       (20)      463 2023-06-01 14:59:14.000000 hj-generate-2.1.3/generate/templates/controller.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      123 2023-06-01 14:59:14.000000 hj-generate-2.1.3/generate/templates/service.tpl
+-rw-r--r--   0 hj         (501) staff       (20)      140 2023-06-01 13:51:23.000000 hj-generate-2.1.3/generate/templates/sql.tpl
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 15:15:40.482992 hj-generate-2.1.3/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 15:15:40.000000 hj-generate-2.1.3/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      359 2023-06-01 15:15:40.000000 hj-generate-2.1.3/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 15:15:40.000000 hj-generate-2.1.3/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 15:15:40.000000 hj-generate-2.1.3/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 15:15:40.000000 hj-generate-2.1.3/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 15:15:40.000000 hj-generate-2.1.3/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 15:15:40.484598 hj-generate-2.1.3/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      380 2023-06-01 15:15:31.000000 hj-generate-2.1.3/setup.py
```

### Comparing `hj-generate-2.1.2/generate/generate_code.py` & `hj-generate-2.1.3/generate/generate_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     env = Environment(loader=FileSystemLoader(current_package_path + os.sep + 'templates'))
 
     # controller
     controller_template = env.get_template('controller.tpl')
 
     controller_output = controller_template.render(data)
 
-    con_append = """
+    co_append = """
 from controllers.{{name}}_controller import {{name}}_controller
 blueprint_list.append({{name}}_controller)
             """
     co_str_temp = env.from_string(co_append)
 
     # 追加
     with open('./service' + os.sep + '__init__.py', 'a') as f:
```

