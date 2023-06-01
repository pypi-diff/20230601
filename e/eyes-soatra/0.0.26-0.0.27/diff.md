# Comparing `tmp/eyes_soatra-0.0.26.tar.gz` & `tmp/eyes_soatra-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.26.tar", last modified: Thu Jun  1 04:48:00 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.27.tar", last modified: Thu Jun  1 07:22:20 2023, max compression
```

## Comparing `eyes_soatra-0.0.26.tar` & `eyes_soatra-0.0.27.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.140812 eyes_soatra-0.0.26/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.26/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 04:48:00.140679 eyes_soatra-0.0.26/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.26/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.131397 eyes_soatra-0.0.26/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.26/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.132653 eyes_soatra-0.0.26/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.26/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.132948 eyes_soatra-0.0.26/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.133720 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/end.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.134557 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/end.py
--rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/period.py
--rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/start.py
--rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.135121 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/not_found.py
--rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.26/eyes_soatra/constant/labels.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.135441 eyes_soatra-0.0.26/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.26/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.26/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.135807 eyes_soatra-0.0.26/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.26/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.26/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      747 2023-05-29 02:30:09.000000 eyes_soatra-0.0.26/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.26/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.138559 eyes_soatra-0.0.26/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    20214 2023-06-01 04:21:42.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/time_app.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.139390 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/list.py
--rw-r--r--   0 soatra     (501) staff       (20)     1221 2023-05-27 07:50:00.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)    13743 2023-06-01 04:44:10.000000 eyes_soatra-0.0.26/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.132149 eyes_soatra-0.0.26/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       48 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-01 04:48:00.000000 eyes_soatra-0.0.26/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-01 04:48:00.140855 eyes_soatra-0.0.26/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1147 2023-06-01 03:53:28.000000 eyes_soatra-0.0.26/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 04:48:00.140365 eyes_soatra-0.0.26/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.26/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.26/test/test1.py
--rw-r--r--   0 soatra     (501) staff       (20)      339 2023-06-01 04:46:32.000000 eyes_soatra-0.0.26/test/test2.py
--rw-r--r--   0 soatra     (501) staff       (20)      236 2023-05-30 04:50:51.000000 eyes_soatra-0.0.26/test/test3.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.180416 eyes_soatra-0.0.27/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.27/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 07:22:20.180276 eyes_soatra-0.0.27/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.27/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.174610 eyes_soatra-0.0.27/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.27/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.175650 eyes_soatra-0.0.27/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.27/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.175783 eyes_soatra-0.0.27/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.176265 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.176761 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.177116 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.27/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.177323 eyes_soatra-0.0.27/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.27/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.27/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.177533 eyes_soatra-0.0.27/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.27/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.27/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      747 2023-05-29 02:30:09.000000 eyes_soatra-0.0.27/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.27/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.178939 eyes_soatra-0.0.27/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    20214 2023-06-01 04:21:42.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.179559 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1221 2023-05-27 07:50:00.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)    13936 2023-06-01 07:21:31.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.175270 eyes_soatra-0.0.27/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       48 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-01 07:22:20.180459 eyes_soatra-0.0.27/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1147 2023-06-01 07:22:07.000000 eyes_soatra-0.0.27/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.180061 eyes_soatra-0.0.27/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.27/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.27/test/test1.py
+-rw-r--r--   0 soatra     (501) staff       (20)      277 2023-06-01 06:45:42.000000 eyes_soatra-0.0.27/test/test2.py
+-rw-r--r--   0 soatra     (501) staff       (20)      236 2023-05-30 04:50:51.000000 eyes_soatra-0.0.27/test/test3.py
```

### Comparing `eyes_soatra-0.0.26/PKG-INFO` & `eyes_soatra-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.26
+Version: 0.0.27
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/end.py` & `eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/end.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/period.py` & `eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/period.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/constant/depends/app_date/formats/start.py` & `eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/not_found.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.27/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/constant/vars.py` & `eyes_soatra-0.0.27/eyes_soatra/constant/vars.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/funcs/time_app.py` & `eyes_soatra-0.0.27/eyes_soatra/funcs/time_app.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/funcs/utils/string.py` & `eyes_soatra-0.0.27/eyes_soatra/funcs/utils/string.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.27/eyes_soatra/funcs/view_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,17 +197,26 @@
         }
         
     return result
 
 def __remove_protocol(url):
     return url.removeprefix('http://').removeprefix('https://')
 
-def __back_home(response: __requests.models.Response):
+def __remove_slash(url):
+    while url.endswith('/'):
+        url = url.removesuffix('/')
+    
+    return url
+
+def __back_home(url, response: __requests.models.Response):
+    if __remove_slash(url) == __remove_slash(response.url):
+        return False
+    
     path = __remove_protocol(response.url)
-    path = path.removesuffix('/')
+    path = __remove_slash(path)
     
     if not '/' in path:
         return True
 
     return False
 
 # ------------------------ public function
@@ -269,16 +278,16 @@
             )
             status_code = response.status_code
             redirected = redirected_forward if redirected_forward else response.is_redirect
             expired = response.headers.get('Expires')
             expired = expired if expired else (response.headers.get('expires') or False)
             expired_obj = {'expired': expired} if expired else {}
             current_url = response.url
-            
-            back_home = __back_home(response)
+
+            back_home = __back_home(url, response)
 
             if back_home:
                 return {
                     'active': False,
                     'checked': False,
                     **expired_obj,
                     'error': f'Redirected to Home Page',
```

### Comparing `eyes_soatra-0.0.26/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.27/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.26
+Version: 0.0.27
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.26/eyes_soatra.egg-info/SOURCES.txt` & `eyes_soatra-0.0.27/eyes_soatra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/setup.py` & `eyes_soatra-0.0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.26'
+VERSION = '0.0.27'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

### Comparing `eyes_soatra-0.0.26/test/test.py` & `eyes_soatra-0.0.27/test/test.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.26/test/test1.py` & `eyes_soatra-0.0.27/test/test1.py`

 * *Files identical despite different names*

