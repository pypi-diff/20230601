# Comparing `tmp/acshell-2.0.0.tar.gz` & `tmp/acshell-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acshell-2.0.0.tar", last modified: Sat Mar 25 06:38:11 2023, max compression
+gzip compressed data, was "acshell-2.1.0.tar", last modified: Thu Jun  1 06:56:22 2023, max compression
```

## Comparing `acshell-2.0.0.tar` & `acshell-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-03-25 06:38:11.604185 acshell-2.0.0/
--rw-r--r--   0 tani       (501) staff       (20)     1056 2023-03-25 05:34:51.000000 acshell-2.0.0/LICENSE
--rw-r--r--   0 tani       (501) staff       (20)     3408 2023-03-25 06:38:11.604457 acshell-2.0.0/PKG-INFO
--rw-r--r--   0 tani       (501) staff       (20)        6 2023-03-25 06:37:20.000000 acshell-2.0.0/VERSION
-drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-03-25 06:38:11.595420 acshell-2.0.0/docs/
--rw-r--r--   0 tani       (501) staff       (20)     2736 2023-03-25 06:36:45.000000 acshell-2.0.0/docs/README.md
--rw-r--r--   0 tani       (501) staff       (20)     1010 2023-03-25 06:38:11.605228 acshell-2.0.0/setup.cfg
--rw-r--r--   0 tani       (501) staff       (20)       39 2023-03-12 09:49:21.000000 acshell-2.0.0/setup.py
-drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-03-25 06:38:11.593143 acshell-2.0.0/src/
-drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-03-25 06:38:11.600071 acshell-2.0.0/src/acshell/
--rw-r--r--   0 tani       (501) staff       (20)       23 2023-03-12 08:28:14.000000 acshell-2.0.0/src/acshell/__init__.py
--rw-r--r--   0 tani       (501) staff       (20)     2849 2023-03-25 06:37:47.000000 acshell-2.0.0/src/acshell/acshell.py
--rw-r--r--   0 tani       (501) staff       (20)     2034 2023-03-25 06:37:46.000000 acshell-2.0.0/src/acshell/cheetsheet.py
--rw-r--r--   0 tani       (501) staff       (20)      168 2023-03-12 10:46:24.000000 acshell-2.0.0/src/acshell/consts.py
-drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-03-25 06:38:11.603754 acshell-2.0.0/src/acshell/contest/
--rw-r--r--   0 tani       (501) staff       (20)        0 2023-03-12 08:28:14.000000 acshell-2.0.0/src/acshell/contest/__init__.py
--rw-r--r--   0 tani       (501) staff       (20)    10019 2023-03-25 06:37:46.000000 acshell-2.0.0/src/acshell/contest/contest.py
--rw-r--r--   0 tani       (501) staff       (20)     9664 2023-03-25 06:37:47.000000 acshell-2.0.0/src/acshell/contest/task.py
--rw-r--r--   0 tani       (501) staff       (20)      799 2023-03-12 08:28:14.000000 acshell-2.0.0/src/acshell/help.py
--rw-r--r--   0 tani       (501) staff       (20)     1476 2023-03-12 09:51:16.000000 acshell-2.0.0/src/acshell/login.py
--rw-r--r--   0 tani       (501) staff       (20)      571 2023-03-12 09:51:02.000000 acshell-2.0.0/src/acshell/main.py
--rw-r--r--   0 tani       (501) staff       (20)     4997 2023-03-13 10:14:07.000000 acshell-2.0.0/src/acshell/result.py
--rw-r--r--   0 tani       (501) staff       (20)     1577 2023-03-25 04:33:22.000000 acshell-2.0.0/src/acshell/task_run.py
--rw-r--r--   0 tani       (501) staff       (20)     1762 2023-03-25 06:37:46.000000 acshell-2.0.0/src/acshell/texts.py
--rw-r--r--   0 tani       (501) staff       (20)     6011 2023-03-25 06:37:46.000000 acshell-2.0.0/src/acshell/utils.py
-drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-03-25 06:38:11.602621 acshell-2.0.0/src/acshell.egg-info/
--rw-r--r--   0 tani       (501) staff       (20)     3408 2023-03-25 06:38:11.000000 acshell-2.0.0/src/acshell.egg-info/PKG-INFO
--rw-r--r--   0 tani       (501) staff       (20)      596 2023-03-25 06:38:11.000000 acshell-2.0.0/src/acshell.egg-info/SOURCES.txt
--rw-r--r--   0 tani       (501) staff       (20)        1 2023-03-25 06:38:11.000000 acshell-2.0.0/src/acshell.egg-info/dependency_links.txt
--rw-r--r--   0 tani       (501) staff       (20)       43 2023-03-25 06:38:11.000000 acshell-2.0.0/src/acshell.egg-info/entry_points.txt
--rw-r--r--   0 tani       (501) staff       (20)       78 2023-03-25 06:38:11.000000 acshell-2.0.0/src/acshell.egg-info/requires.txt
--rw-r--r--   0 tani       (501) staff       (20)        8 2023-03-25 06:38:11.000000 acshell-2.0.0/src/acshell.egg-info/top_level.txt
+drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-06-01 06:56:22.916570 acshell-2.1.0/
+-rw-r--r--   0 tani       (501) staff       (20)     1056 2023-03-25 05:34:51.000000 acshell-2.1.0/LICENSE
+-rw-r--r--   0 tani       (501) staff       (20)     3408 2023-06-01 06:56:22.916821 acshell-2.1.0/PKG-INFO
+-rw-r--r--   0 tani       (501) staff       (20)        6 2023-06-01 06:43:00.000000 acshell-2.1.0/VERSION
+drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-06-01 06:56:22.900246 acshell-2.1.0/docs/
+-rw-r--r--   0 tani       (501) staff       (20)     2736 2023-03-25 06:45:50.000000 acshell-2.1.0/docs/README.md
+-rw-r--r--   0 tani       (501) staff       (20)     1010 2023-06-01 06:56:22.918169 acshell-2.1.0/setup.cfg
+-rw-r--r--   0 tani       (501) staff       (20)       39 2023-03-12 09:49:21.000000 acshell-2.1.0/setup.py
+drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-06-01 06:56:22.896782 acshell-2.1.0/src/
+drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-06-01 06:56:22.910066 acshell-2.1.0/src/acshell/
+-rw-r--r--   0 tani       (501) staff       (20)       23 2023-03-12 08:28:14.000000 acshell-2.1.0/src/acshell/__init__.py
+-rw-r--r--   0 tani       (501) staff       (20)     2849 2023-03-25 06:37:47.000000 acshell-2.1.0/src/acshell/acshell.py
+-rw-r--r--   0 tani       (501) staff       (20)     2034 2023-06-01 06:42:39.000000 acshell-2.1.0/src/acshell/cheatsheet.py
+-rw-r--r--   0 tani       (501) staff       (20)      168 2023-03-12 10:46:24.000000 acshell-2.1.0/src/acshell/consts.py
+drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-06-01 06:56:22.915815 acshell-2.1.0/src/acshell/contest/
+-rw-r--r--   0 tani       (501) staff       (20)        0 2023-03-12 08:28:14.000000 acshell-2.1.0/src/acshell/contest/__init__.py
+-rw-r--r--   0 tani       (501) staff       (20)    10047 2023-06-01 06:52:03.000000 acshell-2.1.0/src/acshell/contest/contest.py
+-rw-r--r--   0 tani       (501) staff       (20)     9664 2023-03-25 06:37:47.000000 acshell-2.1.0/src/acshell/contest/task.py
+-rw-r--r--   0 tani       (501) staff       (20)      799 2023-03-12 08:28:14.000000 acshell-2.1.0/src/acshell/help.py
+-rw-r--r--   0 tani       (501) staff       (20)     1476 2023-06-01 06:41:47.000000 acshell-2.1.0/src/acshell/login.py
+-rw-r--r--   0 tani       (501) staff       (20)      571 2023-03-12 09:51:02.000000 acshell-2.1.0/src/acshell/main.py
+-rw-r--r--   0 tani       (501) staff       (20)     4997 2023-03-13 10:14:07.000000 acshell-2.1.0/src/acshell/result.py
+-rw-r--r--   0 tani       (501) staff       (20)     1577 2023-03-25 04:33:22.000000 acshell-2.1.0/src/acshell/task_run.py
+-rw-r--r--   0 tani       (501) staff       (20)     1762 2023-03-25 06:37:46.000000 acshell-2.1.0/src/acshell/texts.py
+-rw-r--r--   0 tani       (501) staff       (20)     6011 2023-03-25 06:37:46.000000 acshell-2.1.0/src/acshell/utils.py
+drwxr-xr-x   0 tani       (501) staff       (20)        0 2023-06-01 06:56:22.913824 acshell-2.1.0/src/acshell.egg-info/
+-rw-r--r--   0 tani       (501) staff       (20)     3408 2023-06-01 06:56:22.000000 acshell-2.1.0/src/acshell.egg-info/PKG-INFO
+-rw-r--r--   0 tani       (501) staff       (20)      596 2023-06-01 06:56:22.000000 acshell-2.1.0/src/acshell.egg-info/SOURCES.txt
+-rw-r--r--   0 tani       (501) staff       (20)        1 2023-06-01 06:56:22.000000 acshell-2.1.0/src/acshell.egg-info/dependency_links.txt
+-rw-r--r--   0 tani       (501) staff       (20)       43 2023-06-01 06:56:22.000000 acshell-2.1.0/src/acshell.egg-info/entry_points.txt
+-rw-r--r--   0 tani       (501) staff       (20)       78 2023-06-01 06:56:22.000000 acshell-2.1.0/src/acshell.egg-info/requires.txt
+-rw-r--r--   0 tani       (501) staff       (20)        8 2023-06-01 06:56:22.000000 acshell-2.1.0/src/acshell.egg-info/top_level.txt
```

### Comparing `acshell-2.0.0/LICENSE` & `acshell-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/PKG-INFO` & `acshell-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acshell
-Version: 2.0.0
+Version: 2.1.0
 Summary: the commandline shell for python and pypy AtCoder user
 Home-page: https://www.github.com/tani-cat/atcoder-shell
 Author: tani-cat
 License: MIT
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acshell-2.0.0/docs/README.md` & `acshell-2.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/setup.cfg` & `acshell-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/acshell.py` & `acshell-2.1.0/src/acshell/acshell.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/cheetsheet.py` & `acshell-2.1.0/src/acshell/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/contest/contest.py` & `acshell-2.1.0/src/acshell/contest/contest.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,15 @@
             assert task_key not in task_info
             # 問題情報に追加する (task.json)
             task_info[task_key] = {
                 'code': REGEX_DIFF.match(task_top['href']).group(1),
                 'name': tr.select('td')[1].a.text.strip(),
                 'time_limit': float(tr.select('td')[2].text.replace('sec', '').strip()),
                 'memory_limit': int(tr.select('td')[3].text.replace('MB', '').strip()),
+                'score': 0,
             }
 
         return task_info
 
     def __scrape_task_score(self, soup: BeautifulSoup) -> Dict:
         """トップページの配点情報を取得する
         """
```

### Comparing `acshell-2.0.0/src/acshell/contest/task.py` & `acshell-2.1.0/src/acshell/contest/task.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/help.py` & `acshell-2.1.0/src/acshell/help.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/login.py` & `acshell-2.1.0/src/acshell/login.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/main.py` & `acshell-2.1.0/src/acshell/main.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/result.py` & `acshell-2.1.0/src/acshell/result.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/task_run.py` & `acshell-2.1.0/src/acshell/task_run.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/texts.py` & `acshell-2.1.0/src/acshell/texts.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell/utils.py` & `acshell-2.1.0/src/acshell/utils.py`

 * *Files identical despite different names*

### Comparing `acshell-2.0.0/src/acshell.egg-info/PKG-INFO` & `acshell-2.1.0/src/acshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acshell
-Version: 2.0.0
+Version: 2.1.0
 Summary: the commandline shell for python and pypy AtCoder user
 Home-page: https://www.github.com/tani-cat/atcoder-shell
 Author: tani-cat
 License: MIT
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acshell-2.0.0/src/acshell.egg-info/SOURCES.txt` & `acshell-2.1.0/src/acshell.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 VERSION
 setup.cfg
 setup.py
 docs/README.md
 src/acshell/__init__.py
 src/acshell/acshell.py
-src/acshell/cheetsheet.py
+src/acshell/cheatsheet.py
 src/acshell/consts.py
 src/acshell/help.py
 src/acshell/login.py
 src/acshell/main.py
 src/acshell/result.py
 src/acshell/task_run.py
 src/acshell/texts.py
```

