# Comparing `tmp/cdktf-cdktf-provider-hcs-4.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-hcs-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-hcs-4.0.0.tar", last modified: Tue Apr 18 20:42:56 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-hcs-4.0.1.tar", last modified: Thu Jun  1 14:20:47 2023, max compression
```

## Comparing `cdktf-cdktf-provider-hcs-4.0.0.tar` & `cdktf-cdktf-provider-hcs-4.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   371955 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@4.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    80990 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/
--rw-r--r--   0 runner    (1001) docker     (123)    29906 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/
--rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    37485 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/
--rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/
--rw-r--r--   0 runner    (1001) docker     (123)    29845 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/
--rw-r--r--   0 runner    (1001) docker     (123)    24761 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    41724 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    38291 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.948791 cdktf-cdktf-provider-hcs-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.948791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.948791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90851 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@4.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    80990 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/cluster_root_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    29906 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    37485 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    29845 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)    24761 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    41724 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.952791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)    38291 2023-06-01 14:20:36.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:20:47.948791 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-01 14:20:47.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-01 14:20:47.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:20:47.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:20:47.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 14:20:47.000000 cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/LICENSE` & `cdktf-cdktf-provider-hcs-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/PKG-INFO` & `cdktf-cdktf-provider-hcs-4.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcs
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt hcs Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcs.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hcs Provider](https://github.com/terraform-providers/terraform-provider-hcs)
+* [Terraform hcs Provider](https://registry.terraform.io/providers/hashicorp/hcs/0.5.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hcs/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/README.md` & `cdktf-cdktf-provider-hcs-4.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hcs Provider](https://github.com/terraform-providers/terraform-provider-hcs)
+* [Terraform hcs Provider](https://registry.terraform.io/providers/hashicorp/hcs/0.5.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hcs/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/setup.py` & `cdktf-cdktf-provider-hcs-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-hcs",
-    "version": "4.0.0",
+    "version": "4.0.1",
     "description": "Prebuilt hcs Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-hcs.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -32,25 +32,25 @@
         "cdktf_cdktf_provider_hcs.data_hcs_federation_token",
         "cdktf_cdktf_provider_hcs.data_hcs_plan_defaults",
         "cdktf_cdktf_provider_hcs.provider",
         "cdktf_cdktf_provider_hcs.snapshot"
     ],
     "package_data": {
         "cdktf_cdktf_provider_hcs._jsii": [
-            "provider-hcs@4.0.0.jsii.tgz"
+            "provider-hcs@4.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_hcs": [
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

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hcs Provider](https://github.com/terraform-providers/terraform-provider-hcs)
+* [Terraform hcs Provider](https://registry.terraform.io/providers/hashicorp/hcs/0.5.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hcs/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/provider/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcs
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt hcs Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcs.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hcs Provider](https://github.com/terraform-providers/terraform-provider-hcs)
+* [Terraform hcs Provider](https://registry.terraform.io/providers/hashicorp/hcs/0.5.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hcs/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-hcs-4.0.1/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_hcs/py.typed
 src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_hcs.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_hcs.egg-info/requires.txt
 src/cdktf_cdktf_provider_hcs.egg-info/top_level.txt
 src/cdktf_cdktf_provider_hcs/_jsii/__init__.py
-src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@4.0.0.jsii.tgz
+src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@4.0.1.jsii.tgz
 src/cdktf_cdktf_provider_hcs/cluster/__init__.py
 src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py
```

