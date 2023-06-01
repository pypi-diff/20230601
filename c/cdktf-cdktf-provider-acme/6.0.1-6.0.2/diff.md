# Comparing `tmp/cdktf-cdktf-provider-acme-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-acme-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-acme-6.0.1.tar", last modified: Sat May  6 03:12:48 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-acme-6.0.2.tar", last modified: Thu Jun  1 14:08:39 2023, max compression
```

## Comparing `cdktf-cdktf-provider-acme-6.0.1.tar` & `cdktf-cdktf-provider-acme-6.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.631811 cdktf-cdktf-provider-acme-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46032 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/_jsii/provider-acme@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)   106701 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/registration/
--rw-r--r--   0 runner    (1001) docker     (123)    30961 2023-05-06 03:12:32.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/registration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:12:48.635811 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-06 03:12:48.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-06 03:12:48.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:12:48.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 03:12:48.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 03:12:48.000000 cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.841317 cdktf-cdktf-provider-acme-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-01 14:08:39.841317 cdktf-cdktf-provider-acme-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:08:39.841317 cdktf-cdktf-provider-acme-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.837317 cdktf-cdktf-provider-acme-6.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.837317 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.841317 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46955 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/_jsii/provider-acme@6.0.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.841317 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)   106701 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.841317 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.841317 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)    30961 2023-06-01 14:08:27.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/registration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:08:39.837317 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-01 14:08:39.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-01 14:08:39.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:08:39.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:08:39.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:08:39.000000 cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-acme-6.0.1/LICENSE` & `cdktf-cdktf-provider-acme-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-acme-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-acme-6.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-acme
-Version: 6.0.1
+Version: 6.0.2
 Summary: Prebuilt acme Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-acme.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-acme.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform acme Provider version 1:1. In fact, it always tracks `latest` of `~> 2.10` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform acme Provider](https://github.com/terraform-providers/terraform-provider-acme)
+* [Terraform acme Provider](https://registry.terraform.io/providers/vancluever/acme/2.10.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-acme/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-acme-6.0.1/README.md` & `cdktf-cdktf-provider-acme-6.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform acme Provider version 1:1. In fact, it always tracks `latest` of `~> 2.10` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform acme Provider](https://github.com/terraform-providers/terraform-provider-acme)
+* [Terraform acme Provider](https://registry.terraform.io/providers/vancluever/acme/2.10.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-acme/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-acme-6.0.1/setup.py` & `cdktf-cdktf-provider-acme-6.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-acme",
-    "version": "6.0.1",
+    "version": "6.0.2",
     "description": "Prebuilt acme Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-acme.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,25 +25,25 @@
         "cdktf_cdktf_provider_acme._jsii",
         "cdktf_cdktf_provider_acme.certificate",
         "cdktf_cdktf_provider_acme.provider",
         "cdktf_cdktf_provider_acme.registration"
     ],
     "package_data": {
         "cdktf_cdktf_provider_acme._jsii": [
-            "provider-acme@6.0.1.jsii.tgz"
+            "provider-acme@6.0.2.jsii.tgz"
         ],
         "cdktf_cdktf_provider_acme": [
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

### Comparing `cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/__init__.py` & `cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform acme Provider version 1:1. In fact, it always tracks `latest` of `~> 2.10` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform acme Provider](https://github.com/terraform-providers/terraform-provider-acme)
+* [Terraform acme Provider](https://registry.terraform.io/providers/vancluever/acme/2.10.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-acme/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/certificate/__init__.py` & `cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/provider/__init__.py` & `cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme/registration/__init__.py` & `cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme/registration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/PKG-INFO` & `cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-acme
-Version: 6.0.1
+Version: 6.0.2
 Summary: Prebuilt acme Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-acme.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-acme.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform acme Provider version 1:1. In fact, it always tracks `latest` of `~> 2.10` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform acme Provider](https://github.com/terraform-providers/terraform-provider-acme)
+* [Terraform acme Provider](https://registry.terraform.io/providers/vancluever/acme/2.10.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-acme/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-acme-6.0.1/src/cdktf_cdktf_provider_acme.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-acme-6.0.2/src/cdktf_cdktf_provider_acme.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_acme/py.typed
 src/cdktf_cdktf_provider_acme.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_acme.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_acme.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_acme.egg-info/requires.txt
 src/cdktf_cdktf_provider_acme.egg-info/top_level.txt
 src/cdktf_cdktf_provider_acme/_jsii/__init__.py
-src/cdktf_cdktf_provider_acme/_jsii/provider-acme@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_acme/_jsii/provider-acme@6.0.2.jsii.tgz
 src/cdktf_cdktf_provider_acme/certificate/__init__.py
 src/cdktf_cdktf_provider_acme/provider/__init__.py
 src/cdktf_cdktf_provider_acme/registration/__init__.py
```

