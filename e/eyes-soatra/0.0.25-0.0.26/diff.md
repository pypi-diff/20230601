# Comparing `tmp/eyes_soatra-0.0.25.tar.gz` & `tmp/eyes_soatra-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.25.tar", last modified: Mon May 29 05:04:49 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.26.tar", last modified: Thu Jun  1 04:48:00 2023, max compression
```

## Comparing `eyes_soatra-0.0.25.tar` & `eyes_soatra-0.0.26.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.985983 eyes_soatra-0.0.25/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.25/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-29 05:04:49.985853 eyes_soatra-0.0.25/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.25/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.977736 eyes_soatra-0.0.25/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.25/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.978774 eyes_soatra-0.0.25/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.25/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.978921 eyes_soatra-0.0.25/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.979504 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/end.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.980141 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/end.py
--rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/period.py
--rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/start.py
--rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.980548 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/not_found.py
--rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.25/eyes_soatra/constant/labels.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.980816 eyes_soatra-0.0.25/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.25/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.25/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.981171 eyes_soatra-0.0.25/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.25/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.25/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      747 2023-05-29 02:30:09.000000 eyes_soatra-0.0.25/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.25/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.983714 eyes_soatra-0.0.25/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    19464 2023-05-29 04:46:40.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/time_app.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.984301 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/list.py
--rw-r--r--   0 soatra     (501) staff       (20)     1221 2023-05-27 07:50:00.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)    12976 2023-05-29 05:03:23.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.978423 eyes_soatra-0.0.25/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-29 05:04:49.986027 eyes_soatra-0.0.25/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-29 05:00:38.000000 eyes_soatra-0.0.25/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.985223 eyes_soatra-0.0.25/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.25/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.25/test/test1.py
--rw-r--r--   0 soatra     (501) staff       (20)      373 2023-05-29 05:02:06.000000 eyes_soatra-0.0.25/test/test2.py
--rw-r--r--   0 soatra     (501) staff       (20)    86427 2023-05-28 08:14:58.000000 eyes_soatra-0.0.25/test/test3.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.140812 eyes_soatra-0.0.26/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.26/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 04:48:00.140679 eyes_soatra-0.0.26/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.26/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.131397 eyes_soatra-0.0.26/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.26/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.132653 eyes_soatra-0.0.26/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.26/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.132948 eyes_soatra-0.0.26/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.133720 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.134557 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.135121 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.26/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.135441 eyes_soatra-0.0.26/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.26/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.26/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.135807 eyes_soatra-0.0.26/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.26/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.26/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      747 2023-05-29 02:30:09.000000 eyes_soatra-0.0.26/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.26/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.138559 eyes_soatra-0.0.26/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    20214 2023-06-01 04:21:42.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.139390 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1221 2023-05-27 07:50:00.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)    13743 2023-06-01 04:44:10.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.132149 eyes_soatra-0.0.26/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       48 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-01 04:48:00.140855 eyes_soatra-0.0.26/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1147 2023-06-01 03:53:28.000000 eyes_soatra-0.0.26/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.140365 eyes_soatra-0.0.26/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.26/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.26/test/test1.py
+-rw-r--r--   0 soatra     (501) staff       (20)      339 2023-06-01 04:46:32.000000 eyes_soatra-0.0.26/test/test2.py
+-rw-r--r--   0 soatra     (501) staff       (20)      236 2023-05-30 04:50:51.000000 eyes_soatra-0.0.26/test/test3.py
```

### Comparing `eyes_soatra-0.0.25/PKG-INFO` & `eyes_soatra-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.25
+Version: 0.0.26
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/end.py` & `eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/end.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/period.py` & `eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/period.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/start.py` & `eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/not_found.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.26/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/eyes_soatra/constant/vars.py` & `eyes_soatra-0.0.26/eyes_soatra/constant/vars.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/eyes_soatra/funcs/time_app.py` & `eyes_soatra-0.0.26/eyes_soatra/funcs/time_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,16 @@
                             ):
                                 break
 
     return result
 
 # ----------- public function
 def time_app(
-    url,
+    url=None,
+    content=None,
     lang='ja',
     xpath=None,
     xpath_desc=None,
     timeout=15,
     verify=False,
     headers=None,
     separator=None,
@@ -472,94 +473,109 @@
     show_all_detail=False,
     show_texts=False,
     show_blog=False,
     give_all=False,
     
     **requests_options
 ):
-    url = __re.sub(r'\s', '', url)
+    if url == None and content == None:
+        raise Exception('Please input one of those: url and content.')
+    
+    if url:
+        url = __re.sub(r'\s', '', url)
+
     tried = 0
     agents = []
     redirected_forward = False
 
     while True:
         try:
             tried += 1
-            user_agent = __random.choice(__User_Agents)
             
-            while user_agent in agents:
+            if content:
+                status_code = 200
+                redirected = False
+                current_url = url
+                html = __html.fromstring(content)
+                __etree.strip_elements(html, *__remove_tags)
+                
+            else:
                 user_agent = __random.choice(__User_Agents)
                 
-            agents.append(user_agent)
+                while user_agent in agents:
+                    user_agent = __random.choice(__User_Agents)
+                    
+                agents.append(user_agent)
+                    
+                response = __requests.get(
+                    **requests_options,
+                    url=url,
+                    timeout=timeout,
+                    allow_redirects=allow_redirects,
+                    verify=verify,
+                    headers={
+                        **(headers if headers else {}),
+                        'USER-AGENT': user_agent,
+                        'ACCEPT' : 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
+                        'ACCEPT-ENCODING' : 'gzip, deflate, br',
+                        'ACCEPT-LANGUAGE' : 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,km-KH;q=0.6,km;q=0.5,ja-JP;q=0.4,ja;q=0.3',
+                        'REFERER' : 'https://www.google.com/'
+                    },
+                )
+                status_code = response.status_code
+                redirected = redirected_forward if redirected_forward else response.is_redirect
+                current_url = response.url
                 
-            response = __requests.get(
-                **requests_options,
-                url=url,
-                timeout=timeout,
-                allow_redirects=allow_redirects,
-                verify=verify,
-                headers={
-                    **(headers if headers else {}),
-                    'USER-AGENT': user_agent,
-                    'ACCEPT' : 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
-                    'ACCEPT-ENCODING' : 'gzip, deflate, br',
-                    'ACCEPT-LANGUAGE' : 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,km-KH;q=0.6,km;q=0.5,ja-JP;q=0.4,ja;q=0.3',
-                    'REFERER' : 'https://www.google.com/'
-                },
-            )
-            status_code = response.status_code
-            redirected = redirected_forward if redirected_forward else response.is_redirect
-            
-            if status_code >= 400 and status_code <= 499:
-                return {
-                    'error': f'Client error responses: {status_code}',
-                    'status': status_code,
-                    'redirected': redirected,
-                    'url': response.url,
-                    'tried': tried,
-                }
+                if status_code >= 400 and status_code <= 499:
+                    return {
+                        'error': f'Client error responses: {status_code}',
+                        'status': status_code,
+                        'redirected': redirected,
+                        'url': current_url,
+                        'tried': tried,
+                    }
+                    
+                if status_code >= 500 and status_code <= 599:
+                    return {
+                        'error': f'Server error responses: {status_code}',
+                        'status': status_code,
+                        'redirected': redirected,
+                        'url': current_url,
+                        'tried': tried,
+                    }
                 
-            if status_code >= 500 and status_code <= 599:
-                return {
-                    'error': f'Server error responses: {status_code}',
-                    'status': status_code,
-                    'redirected': redirected,
-                    'url': response.url,
-                    'tried': tried,
-                }
-            
-            html = __html.fromstring(response.content)
-            __etree.strip_elements(html, *__remove_tags)
-            
-            if allow_redirects:
-                meta_refresh = html.xpath("//meta[translate(@http-equiv,'REFSH','refsh')='refresh']/@content")
+                html = __html.fromstring(response.content)
+                __etree.strip_elements(html, *__remove_tags)
                 
-                if len(meta_refresh):
-                    if tried < tries_forward:
-                        content_refresh = meta_refresh[0]
-                        content_slices = content_refresh.split(';')
-                        
-                        if len(content_slices) > 1:
-                            url_refresh = __strip_space(content_slices[1])
+                if allow_redirects:
+                    meta_refresh = html.xpath("//meta[translate(@http-equiv,'REFSH','refsh')='refresh']/@content")
+                    
+                    if len(meta_refresh):
+                        if tried < tries_forward:
+                            content_refresh = meta_refresh[0]
+                            content_slices = content_refresh.split(';')
                             
-                            if url_refresh.lower().startswith('url='):
-                                url_refresh = url_refresh[4:]
+                            if len(content_slices) > 1:
+                                url_refresh = __strip_space(content_slices[1])
                                 
-                            redirected_forward = True
-                            url = url_refresh
-                            continue
-
-                    else:
-                        return {
-                            'error': f'Out of forwarding tries.',
-                            'redirected': True,
-                            'url': url,
-                            'tried': tried
-                        }
-            
+                                if url_refresh.lower().startswith('url='):
+                                    url_refresh = url_refresh[4:]
+                                    
+                                redirected_forward = True
+                                url = url_refresh
+                                continue
+
+                        else:
+                            return {
+                                'error': f'Out of forwarding tries.',
+                                'redirected': True,
+                                'url': url,
+                                'tried': tried
+                            }
+
             highlight = __highlighter(
                 html,
                 xpath,
                 xpath_desc,
                 separator
             )
             highlight = __translate(
@@ -580,15 +596,15 @@
                 detail,
                 highlight,
                 give_all
             )
             
             return {
                 **time_result,
-                'url': response.url,
+                'url': current_url,
                 'tried': tried,
                 'status': status_code,
                 'redirected': redirected,
                 **({'detail': detail} if show_detail and detail else {}),
                 **({'texts': highlight['texts']} if show_texts else {}),
                 **({'blogs': highlight['blogs']} if show_blog else {}),
             }
```

### Comparing `eyes_soatra-0.0.25/eyes_soatra/funcs/utils/string.py` & `eyes_soatra-0.0.26/eyes_soatra/funcs/utils/string.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.26/eyes_soatra/funcs/view_page.py`

 * *Files 14% similar despite different names*

```diff
@@ -194,14 +194,26 @@
         result = {
             **result,
             'blank': True,
         }
         
     return result
 
+def __remove_protocol(url):
+    return url.removeprefix('http://').removeprefix('https://')
+
+def __back_home(response: __requests.models.Response):
+    path = __remove_protocol(response.url)
+    path = path.removesuffix('/')
+    
+    if not '/' in path:
+        return True
+
+    return False
+
 # ------------------------ public function
 def view_page(
     url,
     lang='ja',
     timeout=15,
     verify=False,
     headers=None,
@@ -236,15 +248,14 @@
             tried += 1
             user_agent = __random.choice(__User_Agents)
             
             while user_agent in agents:
                 user_agent = __random.choice(__User_Agents)
                 
             agents.append(user_agent)
-                
             response = __requests.get(
                 **requests_options,
                 url=url,
                 timeout=timeout,
                 allow_redirects=allow_redirects,
                 verify=verify,
                 headers={
@@ -257,35 +268,50 @@
                 },
             )
             status_code = response.status_code
             redirected = redirected_forward if redirected_forward else response.is_redirect
             expired = response.headers.get('Expires')
             expired = expired if expired else (response.headers.get('expires') or False)
             expired_obj = {'expired': expired} if expired else {}
+            current_url = response.url
+            
+            back_home = __back_home(response)
+
+            if back_home:
+                return {
+                    'active': False,
+                    'checked': False,
+                    **expired_obj,
+                    'error': f'Redirected to Home Page',
+                    'redirected': True,
+                    'url': current_url,
+                    'status': status_code,
+                    'tried': tried,
+                }
             
             if status_code >= 400 and status_code <= 499:
                 return {
                     'active': False,
                     'checked': False,
                     **expired_obj,
                     'error': f'Client error responses: {status_code}',
                     'redirected': redirected,
-                    'url': response.url,
+                    'url': current_url,
                     'status': status_code,
                     'tried': tried,
                 }
                 
             if status_code >= 500 and status_code <= 599:
                 return {
                     'active': False,
                     'checked': False,
                     **expired_obj,
                     'error': f'Server error responses: {status_code}',
                     'redirected': redirected,
-                    'url': response.url,
+                    'url': current_url,
                     'status': status_code,
                     'tried': tried,
                 }
 
             html = __html.fromstring(response.content)
             __etree.strip_elements(html, *__remove_tags)
             
@@ -337,15 +363,15 @@
                     show_highlight,
                     show_header,
                     show_paragraph,
                     show_content,
                 ),
                 **expired_obj,
                 'redirected': redirected,
-                'url': response.url,
+                'url': current_url,
                 'status': status_code,
                 'tried': tried,
             }
 
         except Exception as error:
             if (
                 type(error) == __requests.exceptions.ConnectionError or
```

### Comparing `eyes_soatra-0.0.25/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.26/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.25
+Version: 0.0.26
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.25/eyes_soatra.egg-info/SOURCES.txt` & `eyes_soatra-0.0.26/eyes_soatra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/setup.py` & `eyes_soatra-0.0.26/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.25'
+VERSION = '0.0.26'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
@@ -22,14 +22,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'requests',
         'requests_html',
+        'lxml',
         'jellyfish',
         'translate',
     ],
     keywords=[
         'python',
         'crawler',
         'scanner',
```

### Comparing `eyes_soatra-0.0.25/test/test.py` & `eyes_soatra-0.0.26/test/test.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.25/test/test1.py` & `eyes_soatra-0.0.26/test/test1.py`

 * *Files identical despite different names*

