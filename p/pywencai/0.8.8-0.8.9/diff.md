# Comparing `tmp/pywencai-0.8.8.tar.gz` & `tmp/pywencai-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.8.8.tar", max compression
+gzip compressed data, was "pywencai-0.8.9.tar", max compression
```

## Comparing `pywencai-0.8.8.tar` & `pywencai-0.8.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-31 15:55:01.769338 pywencai-0.8.8/LICENSE
--rw-r--r--   0        0        0     3043 2023-05-31 15:55:01.769338 pywencai-0.8.8/README.md
--rw-r--r--   0        0        0      612 2023-05-31 15:55:01.769338 pywencai-0.8.8/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/__init__.py
--rw-r--r--   0        0        0     5294 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/convert.py
--rw-r--r--   0        0        0      433 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/headers.py
--rw-r--r--   0        0        0    39677 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4303 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/wencai.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 pywencai-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-01 02:57:57.055427 pywencai-0.8.9/LICENSE
+-rw-r--r--   0        0        0     3043 2023-06-01 02:57:57.055427 pywencai-0.8.9/README.md
+-rw-r--r--   0        0        0      612 2023-06-01 02:57:57.055427 pywencai-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/__init__.py
+-rw-r--r--   0        0        0     5118 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/convert.py
+-rw-r--r--   0        0        0      433 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/headers.py
+-rw-r--r--   0        0        0    39677 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4306 2023-06-01 02:57:57.055427 pywencai-0.8.9/pywencai/wencai.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 pywencai-0.8.9/PKG-INFO
```

### Comparing `pywencai-0.8.8/LICENSE` & `pywencai-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.8/README.md` & `pywencai-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.8/pyproject.toml` & `pywencai-0.8.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.8.8"
+version = "0.8.9"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.8.8/pywencai/convert.py` & `pywencai-0.8.9/pywencai/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,23 +157,16 @@
     '''处理get_robot_data的结果'''
     result = json.loads(res.text)
     content = _.get(result, 'data.answer.0.txt.0.content')
     if type(content) == str:
         content = json.loads(content)
     components = content['components'] 
     params = {}
-    if len(components) == 1:
-        components0 = components[0]
-        if (components0.get('show_type') == 'xuangu_tableV1'):
-            params = {
-                'data': xuangu_tableV1_handler(components0, components)
-            }
-        else:
-            params = {
-                'data': show_type_handler(components0, components)
-            }
-        
+    if (len(components) == 1 and _.get(components[0], 'show_type') == 'xuangu_tableV1'):
+        params = {
+            'data': xuangu_tableV1_handler(components[0], components)
+        }
     else:
         params = {
             'data': multi_show_type_handler(components)
         }
     return params
```

### Comparing `pywencai-0.8.8/pywencai/hexin-v.js` & `pywencai-0.8.9/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.8/pywencai/wencai.py` & `pywencai-0.8.9/pywencai/wencai.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
 
 def get(loop=False, **kwargs):
     '''获取结果'''
     kwargs = {replace_key(key): value for key, value in kwargs.items()}
     params = get_robot_data(**kwargs)
     data = params.get('data')
-    condition = data.get('condition')
+    condition = _.get(data, 'condition')
     if condition is not None:
         kwargs = {**kwargs, **data}
         if loop:
             return loop_page(loop, **kwargs)
         else:
             return get_page(**kwargs)
     else:
```

### Comparing `pywencai-0.8.8/PKG-INFO` & `pywencai-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.8.8
+Version: 0.8.9
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

