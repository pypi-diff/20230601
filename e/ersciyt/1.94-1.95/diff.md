# Comparing `tmp/ersciyt-1.94.tar.gz` & `tmp/ersciyt-1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.94.tar", last modified: Thu Jun  1 06:46:58 2023, max compression
+gzip compressed data, was "ersciyt-1.95.tar", last modified: Thu Jun  1 07:05:20 2023, max compression
```

## Comparing `ersciyt-1.94.tar` & `ersciyt-1.95.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.003349 ersciyt-1.94/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-01 06:46:50.000000 ersciyt-1.94/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 06:46:50.000000 ersciyt-1.94/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 06:46:58.003349 ersciyt-1.94/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-01 06:46:50.000000 ersciyt-1.94/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.001349 ersciyt-1.94/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/apps.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/inst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.002349 ersciyt-1.94/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.002349 ersciyt-1.94/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/inst
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/s
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/ytvid.mp4
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     9385 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.002349 ersciyt-1.94/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-01 06:46:58.003349 ersciyt-1.94/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 06:46:50.000000 ersciyt-1.94/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:05:20.860365 ersciyt-1.95/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-01 07:05:13.000000 ersciyt-1.95/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 07:05:13.000000 ersciyt-1.95/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 07:05:20.860365 ersciyt-1.95/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-01 07:05:13.000000 ersciyt-1.95/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:05:20.858365 ersciyt-1.95/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:05:20.859365 ersciyt-1.95/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:05:20.860365 ersciyt-1.95/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/static/inst
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/static/s
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-06-01 07:05:13.000000 ersciyt-1.95/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:05:20.859365 ersciyt-1.95/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 07:05:20.000000 ersciyt-1.95/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-01 07:05:20.000000 ersciyt-1.95/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 07:05:20.000000 ersciyt-1.95/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 07:05:20.000000 ersciyt-1.95/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 07:05:20.000000 ersciyt-1.95/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-01 07:05:20.861365 ersciyt-1.95/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 07:05:13.000000 ersciyt-1.95/setup.py
```

### Comparing `ersciyt-1.94/LICENSE` & `ersciyt-1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.94/PKG-INFO` & `ersciyt-1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.94
+Version: 1.95
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.94/ersciyt/inst.py` & `ersciyt-1.95/ersciyt/inst.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 def inst():
     try:
         os.system('sudo apt install -y nginx')
         os.system('sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default')
         os.system('sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default')
         os.system('sudo service nginx restart')
         os.system('/usr/local/bin/django-admin  startproject proj')
-        os.system('sed -i "s/ALLOWED_HOSTS = \[/&\'*\'/" proj/proj/settings.py')
-        os.system('sed -i "s/INSTALLED_APPS = \[/& \n\t\t\'ersciyt\',/" proj/proj/settings.py')
-        os.system('sed -i "s/STATIC_URL = \'static\/\'/& \nERSCIYT_LINK = \'https:\/\/80-$WEB_HOST\'/" proj/proj/settings.py')
-        os.system('sed -i "s/from django.urls import path/&,include/" proj/proj/urls.py')
-        os.system('sed -i "s/urlpatterns = \[/&\n\t\tpath('', include(\'ersciyt.urls\')),/"  proj/proj/urls.py')
-        os.system('python proj/manage.py runserver')
+        os.system("sed -i \"s/ALLOWED_HOSTS = \[/&'*'/\" proj/proj/settings.py")
+        os.system("sed -i \"s/INSTALLED_APPS = \[/& \n\t\t'ersciyt',/\" proj/proj/settings.py")
+        os.system("sed -i \"s/STATIC_URL = 'static\/'/& \nERSCIYT_LINK = 'https:\/\/80-$WEB_HOST'/\" proj/proj/settings.py")
+        os.system("sed -i \"s/from django.urls import path/&,include/\" proj/proj/urls.py")
+        os.system("sed -i \"s/urlpatterns = \[/&\n\t\tpath('', include('ersciyt.urls')),/\"  proj/proj/urls.py")
+        os.system("python proj/manage.py runserver")
     except:
         print('Error in command')
```

### Comparing `ersciyt-1.94/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.95/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.94/ersciyt/static/inst` & `ersciyt-1.95/ersciyt/static/inst`

 * *Files identical despite different names*

### Comparing `ersciyt-1.94/ersciyt/urls.py` & `ersciyt-1.95/ersciyt/urls.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.94/ersciyt/views.py` & `ersciyt-1.95/ersciyt/views.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.94/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.95/ersciyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.94
+Version: 1.95
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.94/setup.cfg` & `ersciyt-1.95/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.94
+version = 1.95
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

