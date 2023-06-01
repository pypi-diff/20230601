# Comparing `tmp/graphdisplay-0.4.3.tar.gz` & `tmp/graphdisplay-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.4.3.tar", last modified: Thu Jun  1 11:51:08 2023, max compression
+gzip compressed data, was "graphdisplay-0.4.6.tar", last modified: Thu Jun  1 13:51:08 2023, max compression
```

## Comparing `graphdisplay-0.4.3.tar` & `graphdisplay-0.4.6.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.478979 graphdisplay-0.4.3/
--rw-rw-rw-   0        0        0     6795 2023-06-01 11:51:08.477986 graphdisplay-0.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.454082 graphdisplay-0.4.3/graphdisplay/
--rw-rw-rw-   0        0        0      101 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-01 09:21:30.000000 graphdisplay-0.4.3/graphdisplay/about_win_manager.py
--rw-rw-rw-   0        0        0     5199 2023-06-01 11:51:06.000000 graphdisplay-0.4.3/graphdisplay/general_config.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.470458 graphdisplay-0.4.3/graphdisplay/graphs/
--rw-rw-rw-   0        0        0       24 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/graphs/__init__.py
--rw-rw-rw-   0        0        0    23057 2023-05-30 06:46:16.000000 graphdisplay-0.4.3/graphdisplay/graphs/graph.py
--rw-rw-rw-   0        0        0     7686 2023-05-24 10:13:04.000000 graphdisplay-0.4.3/graphdisplay/json_manager.py
--rw-rw-rw-   0        0        0    36268 2023-06-01 09:58:48.000000 graphdisplay-0.4.3/graphdisplay/main.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.471456 graphdisplay-0.4.3/graphdisplay/store/
--rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.4.3/graphdisplay/store/__init__.py
--rw-rw-rw-   0        0        0    17294 2023-05-30 06:46:16.000000 graphdisplay-0.4.3/graphdisplay/tools_win_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.477441 graphdisplay-0.4.3/graphdisplay/trees/
--rw-rw-rw-   0        0        0       88 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/trees/__init__.py
--rw-rw-rw-   0        0        0     3612 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/trees/auto_balance_tree.py
--rw-rw-rw-   0        0        0     3253 2023-05-27 13:25:51.000000 graphdisplay-0.4.3/graphdisplay/trees/binary_search_tree.py
--rw-rw-rw-   0        0        0     6197 2023-05-28 10:30:46.000000 graphdisplay-0.4.3/graphdisplay/trees/binary_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.467469 graphdisplay-0.4.3/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     6795 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 11:51:08.479977 graphdisplay-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-06-01 10:05:17.000000 graphdisplay-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.300131 graphdisplay-0.4.6/
+-rw-rw-rw-   0        0        0     1088 2023-05-07 07:45:49.000000 graphdisplay-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0     6818 2023-06-01 13:51:08.299134 graphdisplay-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6146 2023-06-01 11:38:53.000000 graphdisplay-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.278190 graphdisplay-0.4.6/graphdisplay/
+-rw-rw-rw-   0        0        0      101 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/about_win_manager.py
+-rw-rw-rw-   0        0        0     5199 2023-06-01 13:50:58.000000 graphdisplay-0.4.6/graphdisplay/general_config.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.292153 graphdisplay-0.4.6/graphdisplay/graphs/
+-rw-rw-rw-   0        0        0       24 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/graphs/__init__.py
+-rw-rw-rw-   0        0        0    23057 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/graphs/graph.py
+-rw-rw-rw-   0        0        0     7686 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/json_manager.py
+-rw-rw-rw-   0        0        0    36268 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.293150 graphdisplay-0.4.6/graphdisplay/store/
+-rw-rw-rw-   0        0        0        0 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/store/__init__.py
+-rw-rw-rw-   0        0        0    17294 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/tools_win_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.298137 graphdisplay-0.4.6/graphdisplay/trees/
+-rw-rw-rw-   0        0        0       88 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/__init__.py
+-rw-rw-rw-   0        0        0     3612 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/auto_balance_tree.py
+-rw-rw-rw-   0        0        0     3253 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/binary_search_tree.py
+-rw-rw-rw-   0        0        0     6197 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/binary_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.290157 graphdisplay-0.4.6/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     6818 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 13:51:08.300131 graphdisplay-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1763 2023-06-01 13:48:37.000000 graphdisplay-0.4.6/setup.py
```

### Comparing `graphdisplay-0.4.3/PKG-INFO` & `graphdisplay-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.3
+Version: 0.4.6
 Summary: Librería para representar grafos visualmente
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz (@seniorbeto)
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <p align="center">
   <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
   <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
   <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
 </p>
```

### Comparing `graphdisplay-0.4.3/graphdisplay/about_win_manager.py` & `graphdisplay-0.4.6/graphdisplay/about_win_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay/general_config.py` & `graphdisplay-0.4.6/graphdisplay/general_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.4.3'
+VERSION = '0.4.6'
 DEFAULT_SCR_WIDTH = 600
 DEFAULT_SCR_HEIGHT = 600
 BUTTON_HEIGHT = 30
 BUTTON_WIDTH = 60
 XMARGEN = 7
 YMARGEN = 7
 THEMES = {
```

### Comparing `graphdisplay-0.4.3/graphdisplay/graphs/graph.py` & `graphdisplay-0.4.6/graphdisplay/graphs/graph.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay/json_manager.py` & `graphdisplay-0.4.6/graphdisplay/json_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay/main.py` & `graphdisplay-0.4.6/graphdisplay/main.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay/tools_win_manager.py` & `graphdisplay-0.4.6/graphdisplay/tools_win_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay/trees/auto_balance_tree.py` & `graphdisplay-0.4.6/graphdisplay/trees/auto_balance_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay/trees/binary_search_tree.py` & `graphdisplay-0.4.6/graphdisplay/trees/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay/trees/binary_tree.py` & `graphdisplay-0.4.6/graphdisplay/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.3/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.4.6/graphdisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.3
+Version: 0.4.6
 Summary: Librería para representar grafos visualmente
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz (@seniorbeto)
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <p align="center">
   <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
   <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
   <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
 </p>
```

### Comparing `graphdisplay-0.4.3/graphdisplay.egg-info/SOURCES.txt` & `graphdisplay-0.4.6/graphdisplay.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+README.md
 setup.py
 graphdisplay/__init__.py
 graphdisplay/about_win_manager.py
 graphdisplay/general_config.py
 graphdisplay/json_manager.py
 graphdisplay/main.py
 graphdisplay/tools_win_manager.py
```

