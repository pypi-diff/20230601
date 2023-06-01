# Comparing `tmp/cdktf-cdktf-provider-local-6.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-local-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-local-6.0.0.tar", last modified: Tue Apr 18 20:46:15 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-local-6.0.1.tar", last modified: Thu Jun  1 14:24:18 2023, max compression
```

## Comparing `cdktf-cdktf-provider-local-6.0.0.tar` & `cdktf-cdktf-provider-local-6.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98057 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/_jsii/provider-local@6.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_file/
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_sensitive_file/
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/file/
--rw-r--r--   0 runner    (1001) docker     (123)    34989 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/sensitive_file/
--rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.393701 cdktf-cdktf-provider-local-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.393701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32973 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/_jsii/provider-local@6.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/data_local_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/data_local_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/data_local_sensitive_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/file/
+-rw-r--r--   0 runner    (1001) docker     (123)    34989 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/sensitive_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-06-01 14:24:01.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:18.397701 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-01 14:24:18.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 14:24:18.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:24:18.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:24:18.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 14:24:18.000000 cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-local-6.0.0/LICENSE` & `cdktf-cdktf-provider-local-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-6.0.0/PKG-INFO` & `cdktf-cdktf-provider-local-6.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-local
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt local Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-local.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-local.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform local Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform local Provider](https://github.com/terraform-providers/terraform-provider-local)
+* [Terraform local Provider](https://registry.terraform.io/providers/hashicorp/local/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-local/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-local-6.0.0/README.md` & `cdktf-cdktf-provider-local-6.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform local Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform local Provider](https://github.com/terraform-providers/terraform-provider-local)
+* [Terraform local Provider](https://registry.terraform.io/providers/hashicorp/local/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-local/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-local-6.0.0/setup.py` & `cdktf-cdktf-provider-local-6.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-local",
-    "version": "6.0.0",
+    "version": "6.0.1",
     "description": "Prebuilt local Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-local.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -27,25 +27,25 @@
         "cdktf_cdktf_provider_local.data_local_sensitive_file",
         "cdktf_cdktf_provider_local.file",
         "cdktf_cdktf_provider_local.provider",
         "cdktf_cdktf_provider_local.sensitive_file"
     ],
     "package_data": {
         "cdktf_cdktf_provider_local._jsii": [
-            "provider-local@6.0.0.jsii.tgz"
+            "provider-local@6.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_local": [
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

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/__init__.py` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform local Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform local Provider](https://github.com/terraform-providers/terraform-provider-local)
+* [Terraform local Provider](https://registry.terraform.io/providers/hashicorp/local/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-local/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_file/__init__.py` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/data_local_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/file/__init__.py` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/provider/__init__.py` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-local
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt local Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-local.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-local.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform local Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform local Provider](https://github.com/terraform-providers/terraform-provider-local)
+* [Terraform local Provider](https://registry.terraform.io/providers/hashicorp/local/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-local/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-local-6.0.1/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/cdktf_cdktf_provider_local/py.typed
 src/cdktf_cdktf_provider_local.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_local.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_local.egg-info/requires.txt
 src/cdktf_cdktf_provider_local.egg-info/top_level.txt
 src/cdktf_cdktf_provider_local/_jsii/__init__.py
-src/cdktf_cdktf_provider_local/_jsii/provider-local@6.0.0.jsii.tgz
+src/cdktf_cdktf_provider_local/_jsii/provider-local@6.0.1.jsii.tgz
 src/cdktf_cdktf_provider_local/data_local_file/__init__.py
 src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py
 src/cdktf_cdktf_provider_local/file/__init__.py
 src/cdktf_cdktf_provider_local/provider/__init__.py
 src/cdktf_cdktf_provider_local/sensitive_file/__init__.py
```

