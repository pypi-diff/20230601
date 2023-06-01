# Comparing `tmp/gomall-0.0.1.tar.gz` & `tmp/gomall-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gomall-0.0.1.tar", last modified: Fri May 26 11:56:03 2023, max compression
+gzip compressed data, was "gomall-0.0.3.tar", last modified: Thu Jun  1 12:57:52 2023, max compression
```

## Comparing `gomall-0.0.1.tar` & `gomall-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:56:03.783051 gomall-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-05-26 11:23:18.000000 gomall-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      561 2023-05-26 11:56:03.782008 gomall-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-05-26 11:26:17.000000 gomall-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 11:56:03.772461 gomall-0.0.1/gomall/
--rw-rw-rw-   0        0        0       46 2023-05-26 11:41:00.000000 gomall-0.0.1/gomall/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:56:03.781004 gomall-0.0.1/gomall/autolog/
--rw-rw-rw-   0        0        0       90 2023-05-26 11:38:51.000000 gomall-0.0.1/gomall/autolog/__init__.py
--rw-rw-rw-   0        0        0     5474 2023-05-26 02:02:02.000000 gomall-0.0.1/gomall/autolog/log.py
--rw-rw-rw-   0        0        0      880 2023-05-26 11:38:51.000000 gomall-0.0.1/gomall/autolog/model.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:56:03.776988 gomall-0.0.1/gomall.egg-info/
--rw-rw-rw-   0        0        0      561 2023-05-26 11:56:03.000000 gomall-0.0.1/gomall.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-26 11:56:03.000000 gomall-0.0.1/gomall.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:56:03.000000 gomall-0.0.1/gomall.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-26 11:56:03.000000 gomall-0.0.1/gomall.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 11:56:03.000000 gomall-0.0.1/gomall.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 11:56:03.783051 gomall-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-05-26 11:27:05.000000 gomall-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.473168 gomall-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-26 11:23:18.000000 gomall-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      561 2023-06-01 12:57:52.471701 gomall-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-05-26 11:26:17.000000 gomall-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.448982 gomall-0.0.3/gomall/
+-rw-rw-rw-   0        0        0       46 2023-05-26 11:41:00.000000 gomall-0.0.3/gomall/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.469491 gomall-0.0.3/gomall/autolog/
+-rw-rw-rw-   0        0        0       90 2023-05-26 11:38:51.000000 gomall-0.0.3/gomall/autolog/__init__.py
+-rw-rw-rw-   0        0        0     5537 2023-06-01 12:27:11.000000 gomall-0.0.3/gomall/autolog/log.py
+-rw-rw-rw-   0        0        0      880 2023-05-26 11:38:51.000000 gomall-0.0.3/gomall/autolog/model.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.462298 gomall-0.0.3/gomall.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 12:57:52.473168 gomall-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-06-01 12:57:47.000000 gomall-0.0.3/setup.py
```

### Comparing `gomall-0.0.1/LICENSE` & `gomall-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gomall-0.0.1/PKG-INFO` & `gomall-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gomall
-Version: 0.0.1
+Version: 0.0.3
 Summary: 和gomall平台配合使用的python依赖包，包括实验追踪、指令构造、模型评估等工具
 Author: GoMall Development Team
 Author-email: wangwenshan@ict.ac.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `gomall-0.0.1/gomall/autolog/model.py` & `gomall-0.0.3/gomall/autolog/model.py`

 * *Files identical despite different names*

### Comparing `gomall-0.0.1/gomall.egg-info/PKG-INFO` & `gomall-0.0.3/gomall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gomall
-Version: 0.0.1
+Version: 0.0.3
 Summary: 和gomall平台配合使用的python依赖包，包括实验追踪、指令构造、模型评估等工具
 Author: GoMall Development Team
 Author-email: wangwenshan@ict.ac.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `gomall-0.0.1/setup.py` & `gomall-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gomall",
-    version="0.0.1",
+    version="0.0.3",
     author="GoMall Development Team",
     author_email="wangwenshan@ict.ac.cn",
     description="和gomall平台配合使用的python依赖包，包括实验追踪、指令构造、模型评估等工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

