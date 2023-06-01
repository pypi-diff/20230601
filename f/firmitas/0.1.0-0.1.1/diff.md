# Comparing `tmp/firmitas-0.1.0.tar.gz` & `tmp/firmitas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firmitas-0.1.0.tar", max compression
+gzip compressed data, was "firmitas-0.1.1.tar", max compression
```

## Comparing `firmitas-0.1.0.tar` & `firmitas-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     9560 2023-06-01 08:38:14.507365 firmitas-0.1.0/README.md
--rw-r--r--   0        0        0     2037 2023-05-26 13:39:42.226571 firmitas-0.1.0/firmitas/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 06:09:59.707985 firmitas-0.1.0/firmitas/base/__init__.py
--rw-r--r--   0        0        0     7304 2023-06-01 08:38:14.510698 firmitas-0.1.0/firmitas/base/maintool.py
--rw-r--r--   0        0        0        0 2023-05-19 06:02:47.021804 firmitas-0.1.0/firmitas/conf/__init__.py
--rw-r--r--   0        0        0    19059 2023-05-26 13:39:42.226571 firmitas-0.1.0/firmitas/conf/certlist.yml
--rw-r--r--   0        0        0      203 2023-05-19 07:42:29.844686 firmitas-0.1.0/firmitas/conf/logrdata.py
--rw-r--r--   0        0        0     1611 2023-06-01 08:38:14.510698 firmitas-0.1.0/firmitas/conf/standard.py
--rw-r--r--   0        0        0      617 2023-05-26 13:39:42.226571 firmitas-0.1.0/firmitas/main.py
--rw-r--r--   0        0        0     1147 2023-05-26 13:39:42.226571 firmitas-0.1.0/firmitas/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 06:44:35.373299 firmitas-0.1.0/firmitas/unit/gogithub.py
--rw-r--r--   0        0        0     2096 2023-05-26 13:39:42.226571 firmitas-0.1.0/firmitas/unit/gopagure.py
--rw-r--r--   0        0        0     1761 2023-06-01 08:42:27.653796 firmitas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11115 1970-01-01 00:00:00.000000 firmitas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-01 12:05:07.834486 firmitas-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9560 2023-06-01 12:03:07.446782 firmitas-0.1.1/README.md
+-rw-r--r--   0        0        0     2037 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/base/__init__.py
+-rw-r--r--   0        0        0     7304 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/base/maintool.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/__init__.py
+-rw-r--r--   0        0        0    19059 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/certlist.yml
+-rw-r--r--   0        0        0      203 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/logrdata.py
+-rw-r--r--   0        0        0     1611 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/standard.py
+-rw-r--r--   0        0        0      617 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/main.py
+-rw-r--r--   0        0        0     1147 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/unit/gogithub.py
+-rw-r--r--   0        0        0     2096 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/unit/gopagure.py
+-rw-r--r--   0        0        0     1780 2023-06-01 12:52:05.267866 firmitas-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10605 2023-06-01 13:20:34.545662 firmitas-0.1.1/setup.py
+-rw-r--r--   0        0        0    11052 2023-06-01 13:20:34.546119 firmitas-0.1.1/PKG-INFO
```

### Comparing `firmitas-0.1.0/README.md` & `firmitas-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/firmitas/__init__.py` & `firmitas-0.1.1/firmitas/__init__.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/firmitas/base/maintool.py` & `firmitas-0.1.1/firmitas/base/maintool.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/firmitas/conf/certlist.yml` & `firmitas-0.1.1/firmitas/conf/certlist.yml`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/firmitas/conf/standard.py` & `firmitas-0.1.1/firmitas/conf/standard.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/firmitas/main.py` & `firmitas-0.1.1/firmitas/main.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/firmitas/unit/__init__.py` & `firmitas-0.1.1/firmitas/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/firmitas/unit/gopagure.py` & `firmitas-0.1.1/firmitas/unit/gopagure.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.0/pyproject.toml` & `firmitas-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firmitas"
-version = "0.1.0"
+version = "0.1.1"
 description = "Simple notification service for X.509-standard TLS certificate statuses"
 authors = ["Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/t0xic0der/firmitas/"
 repository = "https://gitlab.com/t0xic0der/firmitas/"
@@ -23,18 +23,18 @@
     "Topic :: Security :: Cryptography",
     "Topic :: System :: Networking",
     "Topic :: System :: Networking :: Monitoring",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-click = "^8.1.3"
-cryptography = "^40.0.2"
-pyyaml = "^6.0"
-requests = "^2.31.0"
+click = ">=8.0.0,<9"
+cryptography = ">=36.0.0,<40"
+pyyaml = ">=5.0.0,<7"
+requests = ">=2.20.0,<3"
 
 [tool.poetry.dev-dependencies]
 black = "^23.0.0"
 isort = "^5.10.1"
 pytest = "^7.1.3"
 flake8 = "<6.0.1"
 pytest-black = "^0.3.12"
```

### Comparing `firmitas-0.1.0/PKG-INFO` & `firmitas-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firmitas
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple notification service for X.509-standard TLS certificate statuses
 Home-page: https://gitlab.com/t0xic0der/firmitas/
 License: GPL-3.0-or-later
 Keywords: notification,security,certificate
 Author: Akashdeep Dhar
 Author-email: akashdeep.dhar@gmail.com
 Maintainer: Akashdeep Dhar
@@ -13,27 +13,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Operating System
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cryptography (>=40.0.2,<41.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: click (>=8.0.0,<9)
+Requires-Dist: cryptography (>=36.0.0,<40)
+Requires-Dist: pyyaml (>=5.0.0,<7)
+Requires-Dist: requests (>=2.20.0,<3)
 Project-URL: Documentation, https://gitlab.com/t0xic0der/firmitas/-/blob/main/README.md
 Project-URL: Repository, https://gitlab.com/t0xic0der/firmitas/
 Description-Content-Type: text/markdown
 
 # firmitas
 
 Simple notification service for X.509-standard TLS certificate statuses
```

