# Comparing `tmp/hj-generate-1.3.0.tar.gz` & `tmp/hj-generate-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj-generate-1.3.0.tar", last modified: Thu Jun  1 14:17:36 2023, max compression
+gzip compressed data, was "hj-generate-1.4.0.tar", last modified: Thu Jun  1 14:21:16 2023, max compression
```

## Comparing `hj-generate-1.3.0.tar` & `hj-generate-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:17:36.674997 hj-generate-1.3.0/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:17:36.674674 hj-generate-1.3.0/PKG-INFO
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:17:36.672557 hj-generate-1.3.0/generate/
--rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.3.0/generate/__init__.py
--rw-r--r--   0 hj         (501) staff       (20)     1481 2023-06-01 14:01:26.000000 hj-generate-1.3.0/generate/generate_code.py
-drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:17:36.674251 hj-generate-1.3.0/hj_generate.egg-info/
--rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/PKG-INFO
--rw-r--r--   0 hj         (501) staff       (20)      267 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/SOURCES.txt
--rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/dependency_links.txt
--rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/entry_points.txt
--rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/requires.txt
--rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:17:36.000000 hj-generate-1.3.0/hj_generate.egg-info/top_level.txt
--rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:17:36.675162 hj-generate-1.3.0/setup.cfg
--rw-r--r--   0 hj         (501) staff       (20)      314 2023-06-01 14:17:26.000000 hj-generate-1.3.0/setup.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:21:16.161782 hj-generate-1.4.0/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:21:16.161539 hj-generate-1.4.0/PKG-INFO
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:21:16.159298 hj-generate-1.4.0/generate/
+-rw-r--r--   0 hj         (501) staff       (20)        0 2023-06-01 13:14:29.000000 hj-generate-1.4.0/generate/__init__.py
+-rw-r--r--   0 hj         (501) staff       (20)     1490 2023-06-01 14:20:47.000000 hj-generate-1.4.0/generate/generate_code.py
+drwxr-xr-x   0 hj         (501) staff       (20)        0 2023-06-01 14:21:16.161069 hj-generate-1.4.0/hj_generate.egg-info/
+-rw-r--r--   0 hj         (501) staff       (20)      119 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/PKG-INFO
+-rw-r--r--   0 hj         (501) staff       (20)      267 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 hj         (501) staff       (20)        1 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 hj         (501) staff       (20)       60 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/entry_points.txt
+-rw-r--r--   0 hj         (501) staff       (20)        7 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/requires.txt
+-rw-r--r--   0 hj         (501) staff       (20)        9 2023-06-01 14:21:16.000000 hj-generate-1.4.0/hj_generate.egg-info/top_level.txt
+-rw-r--r--   0 hj         (501) staff       (20)       38 2023-06-01 14:21:16.161878 hj-generate-1.4.0/setup.cfg
+-rw-r--r--   0 hj         (501) staff       (20)      314 2023-06-01 14:20:47.000000 hj-generate-1.4.0/setup.py
```

### Comparing `hj-generate-1.3.0/generate/generate_code.py` & `hj-generate-1.4.0/generate/generate_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,24 +36,28 @@
 def underscore_to_camelcase(text):
     parts = text.split('_')
     return ''.join(word.capitalize() for word in parts)
 
 
 # 示例
 
-if __name__ == '__main__':
+
+def main():
     # 创建命令行解析器
     parser = argparse.ArgumentParser(description="代码生成")
 
     # 添加命令行参数和选项
     parser.add_argument("name", help="服务名称")
 
     # 解析命令行参数和选项
     name = parser.parse_args()
-    print(name)
     class_name = underscore_to_camelcase(name.name)
     # 调用相应的命令处理函数
     data = {
         'className': class_name,
         'name': name.name
     }
     generate_code(data)
+
+
+if __name__ == '__main__':
+    main()
```

