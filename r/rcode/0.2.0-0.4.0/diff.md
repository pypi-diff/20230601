# Comparing `tmp/rcode-0.2.0.tar.gz` & `tmp/rcode-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcode-0.2.0.tar", last modified: Wed May 31 14:28:36 2023, max compression
+gzip compressed data, was "rcode-0.4.0.tar", last modified: Thu Jun  1 09:50:50 2023, max compression
```

## Comparing `rcode-0.2.0.tar` & `rcode-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-31 14:28:36.239100 rcode-0.2.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1075 2023-05-31 14:01:02.000000 rcode-0.2.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      569 2023-05-31 14:28:36.238899 rcode-0.2.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     1075 2023-05-31 14:28:11.000000 rcode-0.2.0/README.md
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-31 14:28:36.236137 rcode-0.2.0/rcode/
--rw-r--r--   0 hyi        (502) staff       (20)       20 2023-05-31 14:01:02.000000 rcode-0.2.0/rcode/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       63 2023-05-31 14:01:02.000000 rcode-0.2.0/rcode/__main__.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5975 2023-05-31 14:26:19.000000 rcode-0.2.0/rcode/rcode.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-31 14:28:36.238491 rcode-0.2.0/rcode.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      569 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      277 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       43 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)        8 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        6 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2023-05-31 14:03:42.000000 rcode-0.2.0/rcode.egg-info/zip-safe
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-05-31 14:28:36.239163 rcode-0.2.0/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)      867 2023-05-31 14:28:23.000000 rcode-0.2.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-06-01 09:50:50.958381 rcode-0.4.0/
+-rw-r--r--   0 hyi        (502) staff       (20)     1075 2023-05-31 14:01:02.000000 rcode-0.4.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      569 2023-06-01 09:50:50.958156 rcode-0.4.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     1156 2023-06-01 09:50:33.000000 rcode-0.4.0/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-06-01 09:50:50.954400 rcode-0.4.0/rcode/
+-rw-r--r--   0 hyi        (502) staff       (20)       21 2023-06-01 09:08:55.000000 rcode-0.4.0/rcode/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       64 2023-06-01 09:07:55.000000 rcode-0.4.0/rcode/__main__.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     7629 2023-06-01 09:48:48.000000 rcode-0.4.0/rcode/rcode.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-06-01 09:50:50.957667 rcode-0.4.0/rcode.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      569 2023-06-01 09:50:50.000000 rcode-0.4.0/rcode.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      277 2023-06-01 09:50:50.000000 rcode-0.4.0/rcode.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-06-01 09:50:50.000000 rcode-0.4.0/rcode.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       43 2023-06-01 09:50:50.000000 rcode-0.4.0/rcode.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        8 2023-06-01 09:50:50.000000 rcode-0.4.0/rcode.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        6 2023-06-01 09:50:50.000000 rcode-0.4.0/rcode.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-05-31 14:03:42.000000 rcode-0.4.0/rcode.egg-info/zip-safe
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-06-01 09:50:50.958464 rcode-0.4.0/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)      853 2023-06-01 09:49:07.000000 rcode-0.4.0/setup.py
```

### Comparing `rcode-0.2.0/LICENSE` & `rcode-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcode-0.2.0/PKG-INFO` & `rcode-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcode
-Version: 0.2.0
+Version: 0.4.0
 Summary: vscode remode code .
 Home-page: https://github.com/yihong0618/code-connect
 Author: chvolkmann, yihong0618
 Author-email: zouzou0208@gmail.com
 Keywords: python vscode
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `rcode-0.2.0/README.md` & `rcode-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 Thanks for this cool repo.
 
 https://user-images.githubusercontent.com/1651790/172983742-b27a3fe0-2704-4fc8-b075-a6544783443a.mp4
 
 
 ## What changed
 
-1. Support python3.6+
-2. PyPI
-3. support local open remote dir command `rcode ${ssh_name} ${ssh_dir}`
+1. PyPI
+2. support local open remote dir command `rcode ${ssh_name} ${ssh_dir}`
 
 ## INFO
 
 1. pip3 install rcode (or clone it pip3 install .)
 2. install socat like: (sudo yum install socat)
 3. just `rcode file` like your VSCode `code .`
 4. local open remote use rcode if you use `.ssh/config` --> `rcode remote_ssh ~/test`
 5. local open latest remote `.ssh/config` --> `rcode -l or rcode --latest`
+6. add shortcut_name `rcode s ~/abc -sn abc` then you can use `rcode -os abc` to open this dir quickly
 
 > Note:
 > - Be sure to [connect to the remote host](https://code.visualstudio.com/docs/remote/ssh#_connect-to-a-remote-host) first before typing any `rcode` in the terminal
 > - We may want to add `~/.local/bin` in to your `$PATH` in your `~/.zshrc` or `~/.bashrc` to enable `rcode` being resolved properly
 > ```diff
 > - export PATH=$PATH:/usr/local/go/bin
 > + export PATH=$PATH:/usr/local/go/bin:~/.local/bin
```

### Comparing `rcode-0.2.0/rcode.egg-info/PKG-INFO` & `rcode-0.4.0/rcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcode
-Version: 0.2.0
+Version: 0.4.0
 Summary: vscode remode code .
 Home-page: https://github.com/yihong0618/code-connect
 Author: chvolkmann, yihong0618
 Author-email: zouzou0208@gmail.com
 Keywords: python vscode
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `rcode-0.2.0/setup.py` & `rcode-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.0"
+VERSION = "0.4.0"
 
 setup(
     name="rcode",
     version=VERSION,
     description="vscode remode code .",
     keywords="python vscode",
     author="chvolkmann, yihong0618",
     author_email="zouzou0208@gmail.com",
     url="https://github.com/yihong0618/code-connect",
     packages=find_packages(),
     include_package_data=True,
     zip_safe=True,
-    install_requires=[
-        'sshconf'
-    ],
+    install_requires=["sshconf"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

