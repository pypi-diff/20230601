# Comparing `tmp/ersciyt-1.92.tar.gz` & `tmp/ersciyt-1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.92.tar", last modified: Wed May 24 08:47:38 2023, max compression
+gzip compressed data, was "ersciyt-1.94.tar", last modified: Thu Jun  1 06:46:58 2023, max compression
```

## Comparing `ersciyt-1.92.tar` & `ersciyt-1.94.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:47:38.611362 ersciyt-1.92/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-24 08:47:29.000000 ersciyt-1.92/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-24 08:47:29.000000 ersciyt-1.92/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-24 08:47:38.611362 ersciyt-1.92/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-24 08:47:29.000000 ersciyt-1.92/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:47:38.608362 ersciyt-1.92/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:47:38.610362 ersciyt-1.92/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:47:38.610362 ersciyt-1.92/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)        2 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/static/ytvid.mp4
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     9364 2023-05-24 08:47:29.000000 ersciyt-1.92/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:47:38.610362 ersciyt-1.92/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-24 08:47:38.000000 ersciyt-1.92/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-24 08:47:38.000000 ersciyt-1.92/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:47:38.000000 ersciyt-1.92/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-24 08:47:38.000000 ersciyt-1.92/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 08:47:38.000000 ersciyt-1.92/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-24 08:47:38.612362 ersciyt-1.92/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-24 08:47:29.000000 ersciyt-1.92/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.003349 ersciyt-1.94/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-01 06:46:50.000000 ersciyt-1.94/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 06:46:50.000000 ersciyt-1.94/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 06:46:58.003349 ersciyt-1.94/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-01 06:46:50.000000 ersciyt-1.94/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.001349 ersciyt-1.94/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.002349 ersciyt-1.94/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.002349 ersciyt-1.94/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/inst
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/s
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-06-01 06:46:50.000000 ersciyt-1.94/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:46:58.002349 ersciyt-1.94/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 06:46:57.000000 ersciyt-1.94/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-01 06:46:58.003349 ersciyt-1.94/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 06:46:50.000000 ersciyt-1.94/setup.py
```

### Comparing `ersciyt-1.92/LICENSE` & `ersciyt-1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.92/PKG-INFO` & `ersciyt-1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.92
+Version: 1.94
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.92/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.94/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.92/ersciyt/urls.py` & `ersciyt-1.94/ersciyt/urls.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.92/ersciyt/views.py` & `ersciyt-1.94/ersciyt/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,19 @@
         <a href="#" onclick="window.open('/yt/shqr?idx=' + window.location.href);">show QR Code for this site </a>
         <br>
         </p>
         <br>
         You can use /mp4/<Youtube Video ID> to play video with jump into your custom time of video<br>
         before it you should go /nginx to install nginx server and its appropriate configuration<br>
         if <i> Installation failed!!! </i> message appeared You can install nginx with below command with sudo privilage:
+        <br>
+        <b>
         <i>
         sudo apt install -y nginx<br>
         sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default<br>
         sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default<br>
         sudo service nginx restart<br>
-        </i>        
+        </i></b>
         </body></html>
         ''')
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!')
```

### Comparing `ersciyt-1.92/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.94/ersciyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.92
+Version: 1.94
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.92/setup.cfg` & `ersciyt-1.94/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.92
+version = 1.94
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

