# Comparing `tmp/chaostoolkit-terraform-0.0.4.tar.gz` & `tmp/chaostoolkit-terraform-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaostoolkit-terraform-0.0.4.tar", last modified: Thu Jun  1 10:29:48 2023, max compression
+gzip compressed data, was "chaostoolkit-terraform-0.0.5.tar", last modified: Thu Jun  1 10:41:33 2023, max compression
```

## Comparing `chaostoolkit-terraform-0.0.4.tar` & `chaostoolkit-terraform-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.294477 chaostoolkit-terraform-0.0.4/chaostf/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-01 10:29:41.000000 chaostoolkit-terraform-0.0.4/chaostf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/chaostf/actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/chaostf/control.py
--rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/chaostf/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-01 10:29:48.000000 chaostoolkit-terraform-0.0.4/chaostoolkit_terraform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-01 10:29:41.000000 chaostoolkit-terraform-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:29:48.298477 chaostoolkit-terraform-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-01 10:29:23.000000 chaostoolkit-terraform-0.0.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4381 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/chaostf/
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-01 10:41:28.000000 chaostoolkit-terraform-0.0.5/chaostf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/chaostf/actions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/chaostf/control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/chaostf/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4381 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-01 10:41:28.000000 chaostoolkit-terraform-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/tests/test_version.py
```

### Comparing `chaostoolkit-terraform-0.0.4/LICENSE` & `chaostoolkit-terraform-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.4/README.md` & `chaostoolkit-terraform-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # chaostoolkit-terraform
 
 A [Chaos Toolkit](https://chaostoolkit.org/) driver to extend chaos experiments with [Terraform](https://www.terraform.io/)
 
 ## Package Installation
 
+### From Python package index
+
+To install the latest `chaostoolkit-terraform` stable release:
+
+```shell
+pip install -U chaostoolkit-terraform
+```
+
+### Edge version from the GitHub repository
+
 To install the *edge* version of the `chaostoolkit-terraform` package directly from the repository source code:
 
 ```shell
 pip install -U "git+https://github.com/mcastellin/chaostoolkit-terraform.git#egg=chaostoolkit-terraform"
 ```
 
 ## Usage
```

### Comparing `chaostoolkit-terraform-0.0.4/chaostf/__init__.py` & `chaostoolkit-terraform-0.0.5/chaostf/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 from chaoslib.types import DiscoveredActivities, Discovery
 from logzero import logger
 
 name = "chaostf"
 __author__ = """Manuel Castellin"""
 __email__ = "manuel@castellinconsulting.com"
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __all__ = [
     "discover",
     "__version__",
 ]
 
 
 def discover(discover_system: bool = True) -> Discovery:
```

### Comparing `chaostoolkit-terraform-0.0.4/chaostf/control.py` & `chaostoolkit-terraform-0.0.5/chaostf/control.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.4/chaostf/driver.py` & `chaostoolkit-terraform-0.0.5/chaostf/driver.py`

 * *Files identical despite different names*

