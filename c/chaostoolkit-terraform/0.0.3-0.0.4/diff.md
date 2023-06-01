# Comparing `tmp/chaostoolkit-terraform-0.0.3.tar.gz` & `tmp/chaostoolkit-terraform-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaostoolkit-terraform-0.0.3.tar", last modified: Thu Jun  1 10:09:34 2023, max compression
+gzip compressed data, was "chaostoolkit-terraform-0.0.4.tar", last modified: Thu Jun  1 10:29:48 2023, max compression
```

## Comparing `chaostoolkit-terraform-0.0.3.tar` & `chaostoolkit-terraform-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:09:34.030628 chaostoolkit-terraform-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-01 10:09:10.000000 chaostoolkit-terraform-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-01 10:09:34.030628 chaostoolkit-terraform-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-06-01 10:09:10.000000 chaostoolkit-terraform-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:09:34.030628 chaostoolkit-terraform-0.0.3/chaostf/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-01 10:09:27.000000 chaostoolkit-terraform-0.0.3/chaostf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-01 10:09:10.000000 chaostoolkit-terraform-0.0.3/chaostf/actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-06-01 10:09:10.000000 chaostoolkit-terraform-0.0.3/chaostf/control.py
--rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-06-01 10:09:10.000000 chaostoolkit-terraform-0.0.3/chaostf/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:09:34.030628 chaostoolkit-terraform-0.0.3/chaostoolkit_terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-01 10:09:34.000000 chaostoolkit-terraform-0.0.3/chaostoolkit_terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-01 10:09:34.000000 chaostoolkit-terraform-0.0.3/chaostoolkit_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 10:09:34.000000 chaostoolkit-terraform-0.0.3/chaostoolkit_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-01 10:09:34.000000 chaostoolkit-terraform-0.0.3/chaostoolkit_terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-01 10:09:34.000000 chaostoolkit-terraform-0.0.3/chaostoolkit_terraform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-01 10:09:27.000000 chaostoolkit-terraform-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 10:09:34.030628 chaostoolkit-terraform-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:09:34.030628 chaostoolkit-terraform-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-01 10:09:10.000000 chaostoolkit-terraform-0.0.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.294477 chaostoolkit-terraform-0.0.4/chaostf/
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-01 10:29:41.000000 chaostoolkit-terraform-0.0.4/chaostf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/chaostf/actions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/chaostf/control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/chaostf/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-01 10:29:41.000000 chaostoolkit-terraform-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/tests/test_version.py
```

### Comparing `chaostoolkit-terraform-0.0.3/LICENSE` & `chaostoolkit-terraform-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.3/README.md` & `chaostoolkit-terraform-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.3/chaostf/__init__.py` & `chaostoolkit-terraform-0.0.4/chaostf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 from chaoslib.types import DiscoveredActivities, Discovery
 from logzero import logger
 
 name = "chaostf"
 __author__ = """Manuel Castellin"""
 __email__ = "manuel@castellinconsulting.com"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __all__ = [
     "discover",
     "__version__",
 ]
 
 
 def discover(discover_system: bool = True) -> Discovery:
```

### Comparing `chaostoolkit-terraform-0.0.3/chaostf/control.py` & `chaostoolkit-terraform-0.0.4/chaostf/control.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.3/chaostf/driver.py` & `chaostoolkit-terraform-0.0.4/chaostf/driver.py`

 * *Files identical despite different names*

