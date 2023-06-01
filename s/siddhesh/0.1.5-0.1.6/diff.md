# Comparing `tmp/siddhesh-0.1.5.tar.gz` & `tmp/siddhesh-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siddhesh-0.1.5.tar", last modified: Mon Apr 24 05:52:04 2023, max compression
+gzip compressed data, was "siddhesh-0.1.6.tar", last modified: Thu Jun  1 16:05:47 2023, max compression
```

## Comparing `siddhesh-0.1.5.tar` & `siddhesh-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 05:52:04.442646 siddhesh-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      767 2023-04-24 05:52:04.442646 siddhesh-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 05:52:04.442646 siddhesh-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-04-24 05:51:58.000000 siddhesh-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 05:52:04.418631 siddhesh-0.1.5/siddhesh/
--rw-rw-rw-   0        0        0     1335 2023-04-24 05:46:53.000000 siddhesh-0.1.5/siddhesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 05:52:04.434635 siddhesh-0.1.5/siddhesh.egg-info/
--rw-rw-rw-   0        0        0      767 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 16:05:47.812002 siddhesh-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      767 2023-06-01 16:05:47.805482 siddhesh-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 16:05:47.812002 siddhesh-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-01 16:04:52.000000 siddhesh-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:05:47.787490 siddhesh-0.1.6/siddhesh/
+-rw-rw-rw-   0        0        0     1359 2023-06-01 16:03:23.000000 siddhesh-0.1.6/siddhesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:05:47.805482 siddhesh-0.1.6/siddhesh.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/top_level.txt
```

### Comparing `siddhesh-0.1.5/LICENSE` & `siddhesh-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.5/PKG-INFO` & `siddhesh-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.5
+Version: 0.1.6
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `siddhesh-0.1.5/README.md` & `siddhesh-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.5/setup.py` & `siddhesh-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5'
-DESCRIPTION = 'Check out Siddhesh Kulthe\'s profile, or send him a direct message!'
-LONG_DESCRIPTION = 'A package that downloads Siddhesh Kulthe\'s Resume on your computer. All you need to do is to import siddhesh and use .Start() method to start the app!'
+VERSION = "0.1.6"
+DESCRIPTION = "Check out Siddhesh Kulthe's profile, or send him a direct message!"
+LONG_DESCRIPTION = "A package that downloads Siddhesh Kulthe's Resume on your computer. All you need to do is to import siddhesh and use .Start() method to start the app!"
 
 # Setting up
 setup(
     name="siddhesh",
     version=VERSION,
     author="Siddhesh Kulthe",
     author_email="siddheshkulthe43@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests'],
-    keywords=['python', 'sid', 'siddhesh kulthe', 'profile', 'message', 'social', 'iamsid47'],
+    install_requires=["requests"],
+    keywords=[
+        "python",
+        "sid",
+        "siddhesh kulthe",
+        "profile",
+        "message",
+        "social",
+        "iamsid47",
+    ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ]
-)
+    ],
+)
```

### Comparing `siddhesh-0.1.5/siddhesh/__init__.py` & `siddhesh-0.1.6/siddhesh/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import requests
 
 URL = "https://linkedin.com/in/siddheshkulthe"
 recipient_email = "siddheshkulthe43@gmail.com"
 
 social_list = []
 
+
 def send_message():
     message = str(input("Enter your message: "))
-    print("...")
     time.sleep(1)
     print("Just so that Siddhesh can get back to you,")
     time.sleep(1)
     email = str(input("Please enter your email:"))
-    vercel_url = "http://34.207.83.162:5000"
-    data = {"message": message, "email" : email}
+    vercel_url = "http://34.204.127.0:5000"
+    data = {"message": message, "email": email}
 
     # Make the HTTP POST request to your Vercel app's endpoint
     response = requests.post(vercel_url, json=data)
 
     if response.status_code == 200:
         print("Message sent successfully!")
     else:
@@ -27,18 +27,22 @@
 
 
 def start():
     print("Hey yo! Nice to meet you :)")
     time.sleep(1)
     print("What would you like to do?\n")
     time.sleep(1)
-    choice = int(input("1. Send Siddhesh A Message \n2. Check out Siddhesh\'s LinkedIn \nEnter (1/2): "))
+    choice = int(
+        input(
+            "1. Send Siddhesh A Message \n2. Check out Siddhesh's LinkedIn \nEnter (1/2): "
+        )
+    )
     if choice == 1:
         send_message()
-    elif choice !=1:
+    elif choice != 1:
         print("\nCool! I'll lead you to his resume!")
         time.sleep(2)
         print("Btw, he's a super cool guy. Would really love to be friends with you :)")
         time.sleep(2)
         print("...")
         time.sleep(3)
-        webbrowser.open(URL)
+        webbrowser.open(URL)
```

### Comparing `siddhesh-0.1.5/siddhesh.egg-info/PKG-INFO` & `siddhesh-0.1.6/siddhesh.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.5
+Version: 0.1.6
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

