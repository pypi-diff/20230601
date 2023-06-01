# Comparing `tmp/cdktf-cdktf-provider-null-6.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-null-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-null-6.0.0.tar", last modified: Tue Apr 18 20:47:41 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-null-6.0.1.tar", last modified: Thu Jun  1 14:26:56 2023, max compression
```

## Comparing `cdktf-cdktf-provider-null-6.0.0.tar` & `cdktf-cdktf-provider-null-6.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48779 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/
--rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-04-18 20:47:28.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:47:41.511517 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 20:47:41.000000 cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.406397 cdktf-cdktf-provider-null-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.406397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23456 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/data_null_data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-null-6.0.0/LICENSE` & `cdktf-cdktf-provider-null-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.0/PKG-INFO` & `cdktf-cdktf-provider-null-6.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-null
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt null Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-null.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-null.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform null Provider](https://github.com/terraform-providers/terraform-provider-null)
+* [Terraform null Provider](https://registry.terraform.io/providers/hashicorp/null/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-null/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-null-6.0.0/README.md` & `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+'''
 # Terraform CDK null Provider ~> 3.0
 
 This repo builds and publishes the Terraform null Provider bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
@@ -55,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform null Provider](https://github.com/terraform-providers/terraform-provider-null)
+* [Terraform null Provider](https://registry.terraform.io/providers/hashicorp/null/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-null/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
@@ -84,7 +87,34 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
+'''
+import abc
+import builtins
+import datetime
+import enum
+import typing
+
+import jsii
+import publication
+import typing_extensions
+
+from typeguard import check_type
+
+from ._jsii import *
+
+__all__ = [
+    "data_null_data_source",
+    "provider",
+    "resource",
+]
+
+publication.publish()
+
+# Loading modules to ensure their types are registered with the jsii runtime library
+from . import data_null_data_source
+from . import provider
+from . import resource
```

### Comparing `cdktf-cdktf-provider-null-6.0.0/setup.py` & `cdktf-cdktf-provider-null-6.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-null",
-    "version": "6.0.0",
+    "version": "6.0.1",
     "description": "Prebuilt null Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-null.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,25 +25,25 @@
         "cdktf_cdktf_provider_null._jsii",
         "cdktf_cdktf_provider_null.data_null_data_source",
         "cdktf_cdktf_provider_null.provider",
         "cdktf_cdktf_provider_null.resource"
     ],
     "package_data": {
         "cdktf_cdktf_provider_null._jsii": [
-            "provider-null@6.0.0.jsii.tgz"
+            "provider-null@6.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_null": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.0, <0.17.0",
+        "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/__init__.py` & `cdktf-cdktf-provider-null-6.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-'''
 # Terraform CDK null Provider ~> 3.0
 
 This repo builds and publishes the Terraform null Provider bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
@@ -56,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform null Provider](https://github.com/terraform-providers/terraform-provider-null)
+* [Terraform null Provider](https://registry.terraform.io/providers/hashicorp/null/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-null/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
@@ -85,34 +86,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-'''
-import abc
-import builtins
-import datetime
-import enum
-import typing
-
-import jsii
-import publication
-import typing_extensions
-
-from typeguard import check_type
-
-from ._jsii import *
-
-__all__ = [
-    "data_null_data_source",
-    "provider",
-    "resource",
-]
-
-publication.publish()
-
-# Loading modules to ensure their types are registered with the jsii runtime library
-from . import data_null_data_source
-from . import provider
-from . import resource
```

### Comparing `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py` & `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py` & `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py` & `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO` & `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-null
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt null Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-null.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-null.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform null Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform null Provider](https://github.com/terraform-providers/terraform-provider-null)
+* [Terraform null Provider](https://registry.terraform.io/providers/hashicorp/null/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-null/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-null-6.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_null/py.typed
 src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_null.egg-info/requires.txt
 src/cdktf_cdktf_provider_null.egg-info/top_level.txt
 src/cdktf_cdktf_provider_null/_jsii/__init__.py
-src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.0.jsii.tgz
+src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.1.jsii.tgz
 src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
 src/cdktf_cdktf_provider_null/provider/__init__.py
 src/cdktf_cdktf_provider_null/resource/__init__.py
```

