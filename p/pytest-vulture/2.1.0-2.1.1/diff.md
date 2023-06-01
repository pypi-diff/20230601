# Comparing `tmp/pytest-vulture-2.1.0.tar.gz` & `tmp/pytest-vulture-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-vulture-2.1.0.tar", last modified: Fri May 19 14:53:15 2023, max compression
+gzip compressed data, was "pytest-vulture-2.1.1.tar", last modified: Thu Jun  1 14:12:51 2023, max compression
```

## Comparing `pytest-vulture-2.1.0.tar` & `pytest-vulture-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/
--rw-rw-r--   0 root         (0) root         (0)     1068 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     2502 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2046 2022-10-12 14:10:16.000000 pytest-vulture-2.1.0/README.rst
--rw-rw-r--   0 root         (0) root         (0)      647 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1648 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture/
--rw-rw-r--   0 root         (0) root         (0)      557 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/src/pytest_vulture/__init__.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture/conf/
--rw-rw-r--   0 root         (0) root         (0)       66 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      951 2022-10-11 15:38:28.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/base.py
--rw-rw-r--   0 root         (0) root         (0)     1626 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/package.py
--rw-rw-r--   0 root         (0) root         (0)     1608 2022-10-11 15:36:03.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/reader.py
--rw-rw-r--   0 root         (0) root         (0)     2657 2022-10-11 15:38:28.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/vulture.py
--rw-rw-r--   0 root         (0) root         (0)     2509 2022-10-12 14:07:59.000000 pytest-vulture-2.1.0/src/pytest_vulture/plugin.py
--rw-rw-r--   0 root         (0) root         (0)     6851 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/src/pytest_vulture/setup_manager.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture/vulture/
--rw-rw-r--   0 root         (0) root         (0)       22 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/src/pytest_vulture/vulture/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3471 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/src/pytest_vulture/vulture/comment.py
--rw-rw-r--   0 root         (0) root         (0)     4101 2022-10-12 12:45:02.000000 pytest-vulture-2.1.0/src/pytest_vulture/vulture/manager.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2502 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      674 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       43 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)      392 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       15 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-01 14:12:51.121530 pytest-vulture-2.1.1/
+-rw-rw-r--   0 root         (0) root         (0)     1068 2022-10-04 08:10:30.000000 pytest-vulture-2.1.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     2502 2023-06-01 14:12:51.121530 pytest-vulture-2.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2046 2022-10-12 14:10:16.000000 pytest-vulture-2.1.1/README.rst
+-rw-rw-r--   0 root         (0) root         (0)      647 2023-06-01 14:12:51.125530 pytest-vulture-2.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1648 2023-06-01 13:57:49.000000 pytest-vulture-2.1.1/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-01 14:12:51.121530 pytest-vulture-2.1.1/src/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-01 14:12:51.121530 pytest-vulture-2.1.1/src/pytest_vulture/
+-rw-rw-r--   0 root         (0) root         (0)      557 2022-10-04 08:10:30.000000 pytest-vulture-2.1.1/src/pytest_vulture/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-01 14:12:51.121530 pytest-vulture-2.1.1/src/pytest_vulture/conf/
+-rw-rw-r--   0 root         (0) root         (0)       66 2022-10-04 08:10:30.000000 pytest-vulture-2.1.1/src/pytest_vulture/conf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      951 2022-10-11 15:38:28.000000 pytest-vulture-2.1.1/src/pytest_vulture/conf/base.py
+-rw-rw-r--   0 root         (0) root         (0)     1626 2023-05-19 14:50:10.000000 pytest-vulture-2.1.1/src/pytest_vulture/conf/package.py
+-rw-rw-r--   0 root         (0) root         (0)     1608 2022-10-11 15:36:03.000000 pytest-vulture-2.1.1/src/pytest_vulture/conf/reader.py
+-rw-rw-r--   0 root         (0) root         (0)     2657 2022-10-11 15:38:28.000000 pytest-vulture-2.1.1/src/pytest_vulture/conf/vulture.py
+-rw-rw-r--   0 root         (0) root         (0)     2509 2022-10-12 14:07:59.000000 pytest-vulture-2.1.1/src/pytest_vulture/plugin.py
+-rw-rw-r--   0 root         (0) root         (0)     6833 2023-06-01 13:59:44.000000 pytest-vulture-2.1.1/src/pytest_vulture/setup_manager.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-01 14:12:51.121530 pytest-vulture-2.1.1/src/pytest_vulture/vulture/
+-rw-rw-r--   0 root         (0) root         (0)       22 2022-10-04 08:10:30.000000 pytest-vulture-2.1.1/src/pytest_vulture/vulture/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3471 2023-05-19 14:50:10.000000 pytest-vulture-2.1.1/src/pytest_vulture/vulture/comment.py
+-rw-rw-r--   0 root         (0) root         (0)     4101 2022-10-12 12:45:02.000000 pytest-vulture-2.1.1/src/pytest_vulture/vulture/manager.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-01 14:12:51.121530 pytest-vulture-2.1.1/src/pytest_vulture.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     2502 2023-06-01 14:12:51.000000 pytest-vulture-2.1.1/src/pytest_vulture.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      674 2023-06-01 14:12:51.000000 pytest-vulture-2.1.1/src/pytest_vulture.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-06-01 14:12:51.000000 pytest-vulture-2.1.1/src/pytest_vulture.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       43 2023-06-01 14:12:51.000000 pytest-vulture-2.1.1/src/pytest_vulture.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)      392 2023-06-01 14:12:51.000000 pytest-vulture-2.1.1/src/pytest_vulture.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       15 2023-06-01 14:12:51.000000 pytest-vulture-2.1.1/src/pytest_vulture.egg-info/top_level.txt
```

### Comparing `pytest-vulture-2.1.0/LICENSE` & `pytest-vulture-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/PKG-INFO` & `pytest-vulture-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-vulture
-Version: 2.1.0
+Version: 2.1.1
 Summary: A pytest plugin to checks dead code with vulture
 Home-page: https://github.com/Gatewatcher/pytest-vulture
 Author: Abadie Moran
 Author-email: moran.abadie@gatewatcher.com
 Maintainer: Abadie Moran
 Maintainer-email: moran.abadie@gatewatcher.com
 License: MIT
```

### Comparing `pytest-vulture-2.1.0/README.rst` & `pytest-vulture-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/setup.cfg` & `pytest-vulture-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/setup.py` & `pytest-vulture-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "pytest11": [
         "vulture = pytest_vulture.plugin",
     ]
 } if not IS_TEST else {}
 
 setup(
     name='pytest-vulture',
-    version='2.1.0',
+    version='2.1.1',
     include_package_data=True,
     author='Abadie Moran',
     author_email='moran.abadie@gatewatcher.com',
     maintainer='Abadie Moran',
     maintainer_email='moran.abadie@gatewatcher.com',
     license='MIT',
     url='https://github.com/Gatewatcher/pytest-vulture',
```

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/__init__.py` & `pytest-vulture-2.1.1/src/pytest_vulture/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/conf/base.py` & `pytest-vulture-2.1.1/src/pytest_vulture/conf/base.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/conf/package.py` & `pytest-vulture-2.1.1/src/pytest_vulture/conf/package.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/conf/reader.py` & `pytest-vulture-2.1.1/src/pytest_vulture/conf/reader.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/conf/vulture.py` & `pytest-vulture-2.1.1/src/pytest_vulture/conf/vulture.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/plugin.py` & `pytest-vulture-2.1.1/src/pytest_vulture/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/setup_manager.py` & `pytest-vulture-2.1.1/src/pytest_vulture/setup_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     _UNUSED_FUNCTION_MESSAGE = "unused function"
     _PY_PROJECT = "[project.scripts]"
 
     def __init__(self, config: IniReader):
         self._entry_points = []
         self._config = config
         try:
-            content = self._config.package_configuration.setup_path.read_text("utf-8").replace("\n", "")
+            content = self._config.package_configuration.setup_path.read_text("utf-8")
         except (OSError, ValueError):
             return
         self._generate_entry_points(content)
 
     def is_entry_point(self, vulture: Item) -> bool:
         """Check if the vulture output is an entry point
         Examples::
```

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/vulture/comment.py` & `pytest-vulture-2.1.1/src/pytest_vulture/vulture/comment.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture/vulture/manager.py` & `pytest-vulture-2.1.1/src/pytest_vulture/vulture/manager.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture.egg-info/PKG-INFO` & `pytest-vulture-2.1.1/src/pytest_vulture.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-vulture
-Version: 2.1.0
+Version: 2.1.1
 Summary: A pytest plugin to checks dead code with vulture
 Home-page: https://github.com/Gatewatcher/pytest-vulture
 Author: Abadie Moran
 Author-email: moran.abadie@gatewatcher.com
 Maintainer: Abadie Moran
 Maintainer-email: moran.abadie@gatewatcher.com
 License: MIT
```

### Comparing `pytest-vulture-2.1.0/src/pytest_vulture.egg-info/SOURCES.txt` & `pytest-vulture-2.1.1/src/pytest_vulture.egg-info/SOURCES.txt`

 * *Files identical despite different names*

