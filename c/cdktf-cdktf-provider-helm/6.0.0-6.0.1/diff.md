# Comparing `tmp/cdktf-cdktf-provider-helm-6.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-helm-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-helm-6.0.0.tar", last modified: Tue Apr 18 20:46:24 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-helm-6.0.1.tar", last modified: Thu Jun  1 14:21:05 2023, max compression
```

## Comparing `cdktf-cdktf-provider-helm-6.0.0.tar` & `cdktf-cdktf-provider-helm-6.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.033640 cdktf-cdktf-provider-helm-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.033640 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   268681 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/_jsii/provider-helm@6.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/data_helm_template/
--rw-r--r--   0 runner    (1001) docker     (123)   191283 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/data_helm_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    60885 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/release/
--rw-r--r--   0 runner    (1001) docker     (123)   174871 2023-04-18 20:46:07.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:24.037640 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:46:23.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-18 20:46:24.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:23.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:46:23.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 20:46:23.000000 cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.972620 cdktf-cdktf-provider-helm-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96556 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/_jsii/provider-helm@6.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/data_helm_template/
+-rw-r--r--   0 runner    (1001) docker     (123)   208868 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/data_helm_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    60967 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)   192034 2023-06-01 14:20:54.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:21:05.976621 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:21:05.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-01 14:21:05.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:21:05.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:21:05.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:21:05.000000 cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/LICENSE` & `cdktf-cdktf-provider-helm-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-helm-6.0.0/PKG-INFO` & `cdktf-cdktf-provider-helm-6.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-helm
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt helm Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-helm.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-helm.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform helm Provider version 1:1. In fact, it always tracks `latest` of `~> 2.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform helm Provider](https://github.com/terraform-providers/terraform-provider-helm)
+* [Terraform helm Provider](https://registry.terraform.io/providers/hashicorp/helm/2.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-helm/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/README.md` & `cdktf-cdktf-provider-helm-6.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform helm Provider version 1:1. In fact, it always tracks `latest` of `~> 2.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform helm Provider](https://github.com/terraform-providers/terraform-provider-helm)
+* [Terraform helm Provider](https://registry.terraform.io/providers/hashicorp/helm/2.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-helm/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/setup.py` & `cdktf-cdktf-provider-helm-6.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-helm",
-    "version": "6.0.0",
+    "version": "6.0.1",
     "description": "Prebuilt helm Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-helm.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,25 +25,25 @@
         "cdktf_cdktf_provider_helm._jsii",
         "cdktf_cdktf_provider_helm.data_helm_template",
         "cdktf_cdktf_provider_helm.provider",
         "cdktf_cdktf_provider_helm.release"
     ],
     "package_data": {
         "cdktf_cdktf_provider_helm._jsii": [
-            "provider-helm@6.0.0.jsii.tgz"
+            "provider-helm@6.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_helm": [
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

### Comparing `cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/__init__.py` & `cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform helm Provider version 1:1. In fact, it always tracks `latest` of `~> 2.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform helm Provider](https://github.com/terraform-providers/terraform-provider-helm)
+* [Terraform helm Provider](https://registry.terraform.io/providers/hashicorp/helm/2.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-helm/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/data_helm_template/__init__.py` & `cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/data_helm_template/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_helm_template`
 
-Refer to the Terraform Registory for docs: [`data_helm_template`](https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template).
+Refer to the Terraform Registory for docs: [`data_helm_template`](https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHelmTemplate(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-helm.dataHelmTemplate.DataHelmTemplate",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template helm_template}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template helm_template}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         chart: builtins.str,
@@ -62,14 +62,15 @@
         repository_cert_file: typing.Optional[builtins.str] = None,
         repository_key_file: typing.Optional[builtins.str] = None,
         repository_password: typing.Optional[builtins.str] = None,
         repository_username: typing.Optional[builtins.str] = None,
         reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSet", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetListStruct", typing.Dict[builtins.str, typing.Any]]]]] = None,
         set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetSensitive", typing.Dict[builtins.str, typing.Any]]]]] = None,
         set_string: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetString", typing.Dict[builtins.str, typing.Any]]]]] = None,
         show_only: typing.Optional[typing.Sequence[builtins.str]] = None,
         skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         skip_tests: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         timeout: typing.Optional[jsii.Number] = None,
         validate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -81,62 +82,63 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template helm_template} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template helm_template} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#chart DataHelmTemplate#chart}
-        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}
-        :param api_versions: Kubernetes api versions used for Capabilities.APIVersions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#api_versions DataHelmTemplate#api_versions}
-        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#atomic DataHelmTemplate#atomic}
-        :param crds: List of rendered CRDs from the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#crds DataHelmTemplate#crds}
-        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#create_namespace DataHelmTemplate#create_namespace}
-        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#dependency_update DataHelmTemplate#dependency_update}
-        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#description DataHelmTemplate#description}
-        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#devel DataHelmTemplate#devel}
-        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#disable_openapi_validation DataHelmTemplate#disable_openapi_validation}
-        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#disable_webhooks DataHelmTemplate#disable_webhooks}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#id DataHelmTemplate#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_crds: Include CRDs in the templated output. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#include_crds DataHelmTemplate#include_crds}
-        :param is_upgrade: Set .Release.IsUpgrade instead of .Release.IsInstall. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#is_upgrade DataHelmTemplate#is_upgrade}
-        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#keyring DataHelmTemplate#keyring}
-        :param kube_version: Kubernetes version used for Capabilities.KubeVersion. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#kube_version DataHelmTemplate#kube_version}
-        :param manifest: Concatenated rendered chart templates. This corresponds to the output of the ``helm template`` command. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#manifest DataHelmTemplate#manifest}
-        :param manifests: Map of rendered chart templates indexed by the template name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#manifests DataHelmTemplate#manifests}
-        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#namespace DataHelmTemplate#namespace}
-        :param notes: Rendered notes if the chart contains a ``NOTES.txt``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#notes DataHelmTemplate#notes}
-        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#pass_credentials DataHelmTemplate#pass_credentials}
-        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#postrender DataHelmTemplate#postrender}
-        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#render_subchart_notes DataHelmTemplate#render_subchart_notes}
-        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#replace DataHelmTemplate#replace}
-        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository DataHelmTemplate#repository}
-        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_ca_file DataHelmTemplate#repository_ca_file}
-        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_cert_file DataHelmTemplate#repository_cert_file}
-        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_key_file DataHelmTemplate#repository_key_file}
-        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_password DataHelmTemplate#repository_password}
-        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_username DataHelmTemplate#repository_username}
-        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#reset_values DataHelmTemplate#reset_values}
-        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#reuse_values DataHelmTemplate#reuse_values}
-        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set DataHelmTemplate#set}
-        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set_sensitive DataHelmTemplate#set_sensitive}
-        :param set_string: set_string block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set_string DataHelmTemplate#set_string}
-        :param show_only: Only show manifests rendered from the given templates. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#show_only DataHelmTemplate#show_only}
-        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#skip_crds DataHelmTemplate#skip_crds}
-        :param skip_tests: If set, tests will not be rendered. By default, tests are rendered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#skip_tests DataHelmTemplate#skip_tests}
-        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#timeout DataHelmTemplate#timeout}
-        :param validate: Validate your manifests against the Kubernetes cluster you are currently pointing at. This is the same validation performed on an install Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#validate DataHelmTemplate#validate}
-        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#values DataHelmTemplate#values}
-        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#verify DataHelmTemplate#verify}
-        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#version DataHelmTemplate#version}
-        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#wait DataHelmTemplate#wait}
+        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#chart DataHelmTemplate#chart}
+        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}
+        :param api_versions: Kubernetes api versions used for Capabilities.APIVersions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#api_versions DataHelmTemplate#api_versions}
+        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#atomic DataHelmTemplate#atomic}
+        :param crds: List of rendered CRDs from the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#crds DataHelmTemplate#crds}
+        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#create_namespace DataHelmTemplate#create_namespace}
+        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#dependency_update DataHelmTemplate#dependency_update}
+        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#description DataHelmTemplate#description}
+        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#devel DataHelmTemplate#devel}
+        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#disable_openapi_validation DataHelmTemplate#disable_openapi_validation}
+        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#disable_webhooks DataHelmTemplate#disable_webhooks}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#id DataHelmTemplate#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_crds: Include CRDs in the templated output. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#include_crds DataHelmTemplate#include_crds}
+        :param is_upgrade: Set .Release.IsUpgrade instead of .Release.IsInstall. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#is_upgrade DataHelmTemplate#is_upgrade}
+        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#keyring DataHelmTemplate#keyring}
+        :param kube_version: Kubernetes version used for Capabilities.KubeVersion. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#kube_version DataHelmTemplate#kube_version}
+        :param manifest: Concatenated rendered chart templates. This corresponds to the output of the ``helm template`` command. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#manifest DataHelmTemplate#manifest}
+        :param manifests: Map of rendered chart templates indexed by the template name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#manifests DataHelmTemplate#manifests}
+        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#namespace DataHelmTemplate#namespace}
+        :param notes: Rendered notes if the chart contains a ``NOTES.txt``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#notes DataHelmTemplate#notes}
+        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#pass_credentials DataHelmTemplate#pass_credentials}
+        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#postrender DataHelmTemplate#postrender}
+        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#render_subchart_notes DataHelmTemplate#render_subchart_notes}
+        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#replace DataHelmTemplate#replace}
+        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository DataHelmTemplate#repository}
+        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_ca_file DataHelmTemplate#repository_ca_file}
+        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_cert_file DataHelmTemplate#repository_cert_file}
+        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_key_file DataHelmTemplate#repository_key_file}
+        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_password DataHelmTemplate#repository_password}
+        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_username DataHelmTemplate#repository_username}
+        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#reset_values DataHelmTemplate#reset_values}
+        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#reuse_values DataHelmTemplate#reuse_values}
+        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set DataHelmTemplate#set}
+        :param set_list: set_list block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_list DataHelmTemplate#set_list}
+        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_sensitive DataHelmTemplate#set_sensitive}
+        :param set_string: set_string block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_string DataHelmTemplate#set_string}
+        :param show_only: Only show manifests rendered from the given templates. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#show_only DataHelmTemplate#show_only}
+        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#skip_crds DataHelmTemplate#skip_crds}
+        :param skip_tests: If set, tests will not be rendered. By default, tests are rendered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#skip_tests DataHelmTemplate#skip_tests}
+        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#timeout DataHelmTemplate#timeout}
+        :param validate: Validate your manifests against the Kubernetes cluster you are currently pointing at. This is the same validation performed on an install Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#validate DataHelmTemplate#validate}
+        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#values DataHelmTemplate#values}
+        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#verify DataHelmTemplate#verify}
+        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#version DataHelmTemplate#version}
+        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#wait DataHelmTemplate#wait}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -175,14 +177,15 @@
             repository_cert_file=repository_cert_file,
             repository_key_file=repository_key_file,
             repository_password=repository_password,
             repository_username=repository_username,
             reset_values=reset_values,
             reuse_values=reuse_values,
             set=set,
+            set_list=set_list,
             set_sensitive=set_sensitive,
             set_string=set_string,
             show_only=show_only,
             skip_crds=skip_crds,
             skip_tests=skip_tests,
             timeout=timeout,
             validate=validate,
@@ -200,15 +203,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putPostrender")
     def put_postrender(self, *, binary_path: builtins.str) -> None:
         '''
-        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#binary_path DataHelmTemplate#binary_path}
+        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#binary_path DataHelmTemplate#binary_path}
         '''
         value = DataHelmTemplatePostrender(binary_path=binary_path)
 
         return typing.cast(None, jsii.invoke(self, "putPostrender", [value]))
 
     @jsii.member(jsii_name="putSet")
     def put_set(
@@ -219,14 +222,27 @@
         :param value: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1596ab16b5d874b157172d384e60dca3a78047fbd42fa1f5b63eee3f239c3aab)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putSet", [value]))
 
+    @jsii.member(jsii_name="putSetList")
+    def put_set_list(
+        self,
+        value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetListStruct", typing.Dict[builtins.str, typing.Any]]]],
+    ) -> None:
+        '''
+        :param value: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__152cb09b5fbfc57dbe53841927f1ffb77aaf7ba9a73e8477e7ab141afc3b3863)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        return typing.cast(None, jsii.invoke(self, "putSetList", [value]))
+
     @jsii.member(jsii_name="putSetSensitive")
     def put_set_sensitive(
         self,
         value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetSensitive", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
         :param value: -
@@ -369,14 +385,18 @@
     def reset_reuse_values(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetReuseValues", []))
 
     @jsii.member(jsii_name="resetSet")
     def reset_set(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSet", []))
 
+    @jsii.member(jsii_name="resetSetList")
+    def reset_set_list(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetSetList", []))
+
     @jsii.member(jsii_name="resetSetSensitive")
     def reset_set_sensitive(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSetSensitive", []))
 
     @jsii.member(jsii_name="resetSetString")
     def reset_set_string(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSetString", []))
@@ -433,14 +453,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="set")
     def set(self) -> "DataHelmTemplateSetList":
         return typing.cast("DataHelmTemplateSetList", jsii.get(self, "set"))
 
     @builtins.property
+    @jsii.member(jsii_name="setList")
+    def set_list(self) -> "DataHelmTemplateSetListStructList":
+        return typing.cast("DataHelmTemplateSetListStructList", jsii.get(self, "setList"))
+
+    @builtins.property
     @jsii.member(jsii_name="setSensitive")
     def set_sensitive(self) -> "DataHelmTemplateSetSensitiveList":
         return typing.cast("DataHelmTemplateSetSensitiveList", jsii.get(self, "setSensitive"))
 
     @builtins.property
     @jsii.member(jsii_name="setString")
     def set_string(self) -> "DataHelmTemplateSetStringList":
@@ -638,14 +663,21 @@
     @jsii.member(jsii_name="setInput")
     def set_input(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSet"]]]:
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSet"]]], jsii.get(self, "setInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="setListInput")
+    def set_list_input(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetListStruct"]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetListStruct"]]], jsii.get(self, "setListInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="setSensitiveInput")
     def set_sensitive_input(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetSensitive"]]]:
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetSensitive"]]], jsii.get(self, "setSensitiveInput"))
 
     @builtins.property
@@ -1297,14 +1329,15 @@
         "repository_cert_file": "repositoryCertFile",
         "repository_key_file": "repositoryKeyFile",
         "repository_password": "repositoryPassword",
         "repository_username": "repositoryUsername",
         "reset_values": "resetValues",
         "reuse_values": "reuseValues",
         "set": "set",
+        "set_list": "setList",
         "set_sensitive": "setSensitive",
         "set_string": "setString",
         "show_only": "showOnly",
         "skip_crds": "skipCrds",
         "skip_tests": "skipTests",
         "timeout": "timeout",
         "validate": "validate",
@@ -1354,14 +1387,15 @@
         repository_cert_file: typing.Optional[builtins.str] = None,
         repository_key_file: typing.Optional[builtins.str] = None,
         repository_password: typing.Optional[builtins.str] = None,
         repository_username: typing.Optional[builtins.str] = None,
         reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSet", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetListStruct", typing.Dict[builtins.str, typing.Any]]]]] = None,
         set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetSensitive", typing.Dict[builtins.str, typing.Any]]]]] = None,
         set_string: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataHelmTemplateSetString", typing.Dict[builtins.str, typing.Any]]]]] = None,
         show_only: typing.Optional[typing.Sequence[builtins.str]] = None,
         skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         skip_tests: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         timeout: typing.Optional[jsii.Number] = None,
         validate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -1374,58 +1408,59 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#chart DataHelmTemplate#chart}
-        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}
-        :param api_versions: Kubernetes api versions used for Capabilities.APIVersions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#api_versions DataHelmTemplate#api_versions}
-        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#atomic DataHelmTemplate#atomic}
-        :param crds: List of rendered CRDs from the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#crds DataHelmTemplate#crds}
-        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#create_namespace DataHelmTemplate#create_namespace}
-        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#dependency_update DataHelmTemplate#dependency_update}
-        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#description DataHelmTemplate#description}
-        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#devel DataHelmTemplate#devel}
-        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#disable_openapi_validation DataHelmTemplate#disable_openapi_validation}
-        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#disable_webhooks DataHelmTemplate#disable_webhooks}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#id DataHelmTemplate#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_crds: Include CRDs in the templated output. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#include_crds DataHelmTemplate#include_crds}
-        :param is_upgrade: Set .Release.IsUpgrade instead of .Release.IsInstall. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#is_upgrade DataHelmTemplate#is_upgrade}
-        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#keyring DataHelmTemplate#keyring}
-        :param kube_version: Kubernetes version used for Capabilities.KubeVersion. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#kube_version DataHelmTemplate#kube_version}
-        :param manifest: Concatenated rendered chart templates. This corresponds to the output of the ``helm template`` command. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#manifest DataHelmTemplate#manifest}
-        :param manifests: Map of rendered chart templates indexed by the template name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#manifests DataHelmTemplate#manifests}
-        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#namespace DataHelmTemplate#namespace}
-        :param notes: Rendered notes if the chart contains a ``NOTES.txt``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#notes DataHelmTemplate#notes}
-        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#pass_credentials DataHelmTemplate#pass_credentials}
-        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#postrender DataHelmTemplate#postrender}
-        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#render_subchart_notes DataHelmTemplate#render_subchart_notes}
-        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#replace DataHelmTemplate#replace}
-        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository DataHelmTemplate#repository}
-        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_ca_file DataHelmTemplate#repository_ca_file}
-        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_cert_file DataHelmTemplate#repository_cert_file}
-        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_key_file DataHelmTemplate#repository_key_file}
-        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_password DataHelmTemplate#repository_password}
-        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_username DataHelmTemplate#repository_username}
-        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#reset_values DataHelmTemplate#reset_values}
-        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#reuse_values DataHelmTemplate#reuse_values}
-        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set DataHelmTemplate#set}
-        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set_sensitive DataHelmTemplate#set_sensitive}
-        :param set_string: set_string block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set_string DataHelmTemplate#set_string}
-        :param show_only: Only show manifests rendered from the given templates. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#show_only DataHelmTemplate#show_only}
-        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#skip_crds DataHelmTemplate#skip_crds}
-        :param skip_tests: If set, tests will not be rendered. By default, tests are rendered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#skip_tests DataHelmTemplate#skip_tests}
-        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#timeout DataHelmTemplate#timeout}
-        :param validate: Validate your manifests against the Kubernetes cluster you are currently pointing at. This is the same validation performed on an install Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#validate DataHelmTemplate#validate}
-        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#values DataHelmTemplate#values}
-        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#verify DataHelmTemplate#verify}
-        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#version DataHelmTemplate#version}
-        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#wait DataHelmTemplate#wait}
+        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#chart DataHelmTemplate#chart}
+        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}
+        :param api_versions: Kubernetes api versions used for Capabilities.APIVersions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#api_versions DataHelmTemplate#api_versions}
+        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#atomic DataHelmTemplate#atomic}
+        :param crds: List of rendered CRDs from the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#crds DataHelmTemplate#crds}
+        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#create_namespace DataHelmTemplate#create_namespace}
+        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#dependency_update DataHelmTemplate#dependency_update}
+        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#description DataHelmTemplate#description}
+        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#devel DataHelmTemplate#devel}
+        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#disable_openapi_validation DataHelmTemplate#disable_openapi_validation}
+        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#disable_webhooks DataHelmTemplate#disable_webhooks}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#id DataHelmTemplate#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_crds: Include CRDs in the templated output. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#include_crds DataHelmTemplate#include_crds}
+        :param is_upgrade: Set .Release.IsUpgrade instead of .Release.IsInstall. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#is_upgrade DataHelmTemplate#is_upgrade}
+        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#keyring DataHelmTemplate#keyring}
+        :param kube_version: Kubernetes version used for Capabilities.KubeVersion. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#kube_version DataHelmTemplate#kube_version}
+        :param manifest: Concatenated rendered chart templates. This corresponds to the output of the ``helm template`` command. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#manifest DataHelmTemplate#manifest}
+        :param manifests: Map of rendered chart templates indexed by the template name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#manifests DataHelmTemplate#manifests}
+        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#namespace DataHelmTemplate#namespace}
+        :param notes: Rendered notes if the chart contains a ``NOTES.txt``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#notes DataHelmTemplate#notes}
+        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#pass_credentials DataHelmTemplate#pass_credentials}
+        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#postrender DataHelmTemplate#postrender}
+        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#render_subchart_notes DataHelmTemplate#render_subchart_notes}
+        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#replace DataHelmTemplate#replace}
+        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository DataHelmTemplate#repository}
+        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_ca_file DataHelmTemplate#repository_ca_file}
+        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_cert_file DataHelmTemplate#repository_cert_file}
+        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_key_file DataHelmTemplate#repository_key_file}
+        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_password DataHelmTemplate#repository_password}
+        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_username DataHelmTemplate#repository_username}
+        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#reset_values DataHelmTemplate#reset_values}
+        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#reuse_values DataHelmTemplate#reuse_values}
+        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set DataHelmTemplate#set}
+        :param set_list: set_list block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_list DataHelmTemplate#set_list}
+        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_sensitive DataHelmTemplate#set_sensitive}
+        :param set_string: set_string block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_string DataHelmTemplate#set_string}
+        :param show_only: Only show manifests rendered from the given templates. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#show_only DataHelmTemplate#show_only}
+        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#skip_crds DataHelmTemplate#skip_crds}
+        :param skip_tests: If set, tests will not be rendered. By default, tests are rendered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#skip_tests DataHelmTemplate#skip_tests}
+        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#timeout DataHelmTemplate#timeout}
+        :param validate: Validate your manifests against the Kubernetes cluster you are currently pointing at. This is the same validation performed on an install Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#validate DataHelmTemplate#validate}
+        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#values DataHelmTemplate#values}
+        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#verify DataHelmTemplate#verify}
+        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#version DataHelmTemplate#version}
+        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#wait DataHelmTemplate#wait}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(postrender, dict):
             postrender = DataHelmTemplatePostrender(**postrender)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__aa661fc2bc6a52eec136c130260e43e15fe67a8017a94efddda364fd2b2f33d2)
@@ -1465,14 +1500,15 @@
             check_type(argname="argument repository_cert_file", value=repository_cert_file, expected_type=type_hints["repository_cert_file"])
             check_type(argname="argument repository_key_file", value=repository_key_file, expected_type=type_hints["repository_key_file"])
             check_type(argname="argument repository_password", value=repository_password, expected_type=type_hints["repository_password"])
             check_type(argname="argument repository_username", value=repository_username, expected_type=type_hints["repository_username"])
             check_type(argname="argument reset_values", value=reset_values, expected_type=type_hints["reset_values"])
             check_type(argname="argument reuse_values", value=reuse_values, expected_type=type_hints["reuse_values"])
             check_type(argname="argument set", value=set, expected_type=type_hints["set"])
+            check_type(argname="argument set_list", value=set_list, expected_type=type_hints["set_list"])
             check_type(argname="argument set_sensitive", value=set_sensitive, expected_type=type_hints["set_sensitive"])
             check_type(argname="argument set_string", value=set_string, expected_type=type_hints["set_string"])
             check_type(argname="argument show_only", value=show_only, expected_type=type_hints["show_only"])
             check_type(argname="argument skip_crds", value=skip_crds, expected_type=type_hints["skip_crds"])
             check_type(argname="argument skip_tests", value=skip_tests, expected_type=type_hints["skip_tests"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
             check_type(argname="argument validate", value=validate, expected_type=type_hints["validate"])
@@ -1556,14 +1592,16 @@
             self._values["repository_username"] = repository_username
         if reset_values is not None:
             self._values["reset_values"] = reset_values
         if reuse_values is not None:
             self._values["reuse_values"] = reuse_values
         if set is not None:
             self._values["set"] = set
+        if set_list is not None:
+            self._values["set_list"] = set_list
         if set_sensitive is not None:
             self._values["set_sensitive"] = set_sensitive
         if set_string is not None:
             self._values["set_string"] = set_string
         if show_only is not None:
             self._values["show_only"] = show_only
         if skip_crds is not None:
@@ -1647,449 +1685,460 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def chart(self) -> builtins.str:
         '''Chart name to be installed. A path may be used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#chart DataHelmTemplate#chart}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#chart DataHelmTemplate#chart}
         '''
         result = self._values.get("chart")
         assert result is not None, "Required property 'chart' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Release name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def api_versions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Kubernetes api versions used for Capabilities.APIVersions.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#api_versions DataHelmTemplate#api_versions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#api_versions DataHelmTemplate#api_versions}
         '''
         result = self._values.get("api_versions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def atomic(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#atomic DataHelmTemplate#atomic}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#atomic DataHelmTemplate#atomic}
         '''
         result = self._values.get("atomic")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def crds(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of rendered CRDs from the chart.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#crds DataHelmTemplate#crds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#crds DataHelmTemplate#crds}
         '''
         result = self._values.get("crds")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def create_namespace(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Create the namespace if it does not exist.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#create_namespace DataHelmTemplate#create_namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#create_namespace DataHelmTemplate#create_namespace}
         '''
         result = self._values.get("create_namespace")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def dependency_update(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Run helm dependency update before installing the chart.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#dependency_update DataHelmTemplate#dependency_update}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#dependency_update DataHelmTemplate#dependency_update}
         '''
         result = self._values.get("dependency_update")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Add a custom description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#description DataHelmTemplate#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#description DataHelmTemplate#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def devel(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#devel DataHelmTemplate#devel}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#devel DataHelmTemplate#devel}
         '''
         result = self._values.get("devel")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def disable_openapi_validation(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#disable_openapi_validation DataHelmTemplate#disable_openapi_validation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#disable_openapi_validation DataHelmTemplate#disable_openapi_validation}
         '''
         result = self._values.get("disable_openapi_validation")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def disable_webhooks(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Prevent hooks from running.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#disable_webhooks DataHelmTemplate#disable_webhooks}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#disable_webhooks DataHelmTemplate#disable_webhooks}
         '''
         result = self._values.get("disable_webhooks")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#id DataHelmTemplate#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#id DataHelmTemplate#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def include_crds(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Include CRDs in the templated output.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#include_crds DataHelmTemplate#include_crds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#include_crds DataHelmTemplate#include_crds}
         '''
         result = self._values.get("include_crds")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def is_upgrade(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set .Release.IsUpgrade instead of .Release.IsInstall.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#is_upgrade DataHelmTemplate#is_upgrade}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#is_upgrade DataHelmTemplate#is_upgrade}
         '''
         result = self._values.get("is_upgrade")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def keyring(self) -> typing.Optional[builtins.str]:
         '''Location of public keys used for verification. Used only if ``verify`` is true.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#keyring DataHelmTemplate#keyring}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#keyring DataHelmTemplate#keyring}
         '''
         result = self._values.get("keyring")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def kube_version(self) -> typing.Optional[builtins.str]:
         '''Kubernetes version used for Capabilities.KubeVersion.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#kube_version DataHelmTemplate#kube_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#kube_version DataHelmTemplate#kube_version}
         '''
         result = self._values.get("kube_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def manifest(self) -> typing.Optional[builtins.str]:
         '''Concatenated rendered chart templates. This corresponds to the output of the ``helm template`` command.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#manifest DataHelmTemplate#manifest}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#manifest DataHelmTemplate#manifest}
         '''
         result = self._values.get("manifest")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def manifests(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Map of rendered chart templates indexed by the template name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#manifests DataHelmTemplate#manifests}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#manifests DataHelmTemplate#manifests}
         '''
         result = self._values.get("manifests")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''Namespace to install the release into.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#namespace DataHelmTemplate#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#namespace DataHelmTemplate#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def notes(self) -> typing.Optional[builtins.str]:
         '''Rendered notes if the chart contains a ``NOTES.txt``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#notes DataHelmTemplate#notes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#notes DataHelmTemplate#notes}
         '''
         result = self._values.get("notes")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def pass_credentials(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Pass credentials to all domains.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#pass_credentials DataHelmTemplate#pass_credentials}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#pass_credentials DataHelmTemplate#pass_credentials}
         '''
         result = self._values.get("pass_credentials")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def postrender(self) -> typing.Optional["DataHelmTemplatePostrender"]:
         '''postrender block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#postrender DataHelmTemplate#postrender}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#postrender DataHelmTemplate#postrender}
         '''
         result = self._values.get("postrender")
         return typing.cast(typing.Optional["DataHelmTemplatePostrender"], result)
 
     @builtins.property
     def render_subchart_notes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, render subchart notes along with the parent.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#render_subchart_notes DataHelmTemplate#render_subchart_notes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#render_subchart_notes DataHelmTemplate#render_subchart_notes}
         '''
         result = self._values.get("render_subchart_notes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def replace(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Re-use the given name, even if that name is already used. This is unsafe in production.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#replace DataHelmTemplate#replace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#replace DataHelmTemplate#replace}
         '''
         result = self._values.get("replace")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def repository(self) -> typing.Optional[builtins.str]:
         '''Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository DataHelmTemplate#repository}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository DataHelmTemplate#repository}
         '''
         result = self._values.get("repository")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_ca_file(self) -> typing.Optional[builtins.str]:
         '''The Repositories CA File.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_ca_file DataHelmTemplate#repository_ca_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_ca_file DataHelmTemplate#repository_ca_file}
         '''
         result = self._values.get("repository_ca_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_cert_file(self) -> typing.Optional[builtins.str]:
         '''The repositories cert file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_cert_file DataHelmTemplate#repository_cert_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_cert_file DataHelmTemplate#repository_cert_file}
         '''
         result = self._values.get("repository_cert_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_key_file(self) -> typing.Optional[builtins.str]:
         '''The repositories cert key file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_key_file DataHelmTemplate#repository_key_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_key_file DataHelmTemplate#repository_key_file}
         '''
         result = self._values.get("repository_key_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_password(self) -> typing.Optional[builtins.str]:
         '''Password for HTTP basic authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_password DataHelmTemplate#repository_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_password DataHelmTemplate#repository_password}
         '''
         result = self._values.get("repository_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_username(self) -> typing.Optional[builtins.str]:
         '''Username for HTTP basic authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#repository_username DataHelmTemplate#repository_username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#repository_username DataHelmTemplate#repository_username}
         '''
         result = self._values.get("repository_username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def reset_values(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When upgrading, reset the values to the ones built into the chart.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#reset_values DataHelmTemplate#reset_values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#reset_values DataHelmTemplate#reset_values}
         '''
         result = self._values.get("reset_values")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def reuse_values(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#reuse_values DataHelmTemplate#reuse_values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#reuse_values DataHelmTemplate#reuse_values}
         '''
         result = self._values.get("reuse_values")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def set(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSet"]]]:
         '''set block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set DataHelmTemplate#set}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set DataHelmTemplate#set}
         '''
         result = self._values.get("set")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSet"]]], result)
 
     @builtins.property
+    def set_list(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetListStruct"]]]:
+        '''set_list block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_list DataHelmTemplate#set_list}
+        '''
+        result = self._values.get("set_list")
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetListStruct"]]], result)
+
+    @builtins.property
     def set_sensitive(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetSensitive"]]]:
         '''set_sensitive block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set_sensitive DataHelmTemplate#set_sensitive}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_sensitive DataHelmTemplate#set_sensitive}
         '''
         result = self._values.get("set_sensitive")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetSensitive"]]], result)
 
     @builtins.property
     def set_string(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetString"]]]:
         '''set_string block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#set_string DataHelmTemplate#set_string}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#set_string DataHelmTemplate#set_string}
         '''
         result = self._values.get("set_string")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHelmTemplateSetString"]]], result)
 
     @builtins.property
     def show_only(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Only show manifests rendered from the given templates.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#show_only DataHelmTemplate#show_only}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#show_only DataHelmTemplate#show_only}
         '''
         result = self._values.get("show_only")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def skip_crds(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, no CRDs will be installed. By default, CRDs are installed if not already present.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#skip_crds DataHelmTemplate#skip_crds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#skip_crds DataHelmTemplate#skip_crds}
         '''
         result = self._values.get("skip_crds")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def skip_tests(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, tests will not be rendered. By default, tests are rendered.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#skip_tests DataHelmTemplate#skip_tests}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#skip_tests DataHelmTemplate#skip_tests}
         '''
         result = self._values.get("skip_tests")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def timeout(self) -> typing.Optional[jsii.Number]:
         '''Time in seconds to wait for any individual kubernetes operation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#timeout DataHelmTemplate#timeout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#timeout DataHelmTemplate#timeout}
         '''
         result = self._values.get("timeout")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def validate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Validate your manifests against the Kubernetes cluster you are currently pointing at.
 
         This is the same validation performed on an install
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#validate DataHelmTemplate#validate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#validate DataHelmTemplate#validate}
         '''
         result = self._values.get("validate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def values(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of values in raw yaml format to pass to helm.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#values DataHelmTemplate#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#values DataHelmTemplate#values}
         '''
         result = self._values.get("values")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def verify(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Verify the package before installing it.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#verify DataHelmTemplate#verify}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#verify DataHelmTemplate#verify}
         '''
         result = self._values.get("verify")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def version(self) -> typing.Optional[builtins.str]:
         '''Specify the exact chart version to install. If this is not specified, the latest version is installed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#version DataHelmTemplate#version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#version DataHelmTemplate#version}
         '''
         result = self._values.get("version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def wait(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Will wait until all resources are in a ready state before marking the release as successful.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#wait DataHelmTemplate#wait}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#wait DataHelmTemplate#wait}
         '''
         result = self._values.get("wait")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2106,28 +2155,28 @@
     jsii_type="@cdktf/provider-helm.dataHelmTemplate.DataHelmTemplatePostrender",
     jsii_struct_bases=[],
     name_mapping={"binary_path": "binaryPath"},
 )
 class DataHelmTemplatePostrender:
     def __init__(self, *, binary_path: builtins.str) -> None:
         '''
-        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#binary_path DataHelmTemplate#binary_path}
+        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#binary_path DataHelmTemplate#binary_path}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__70be91cd9aa2015f426d7219063f388bce602de2810050ccafa37320051af63c)
             check_type(argname="argument binary_path", value=binary_path, expected_type=type_hints["binary_path"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "binary_path": binary_path,
         }
 
     @builtins.property
     def binary_path(self) -> builtins.str:
         '''The command binary path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#binary_path DataHelmTemplate#binary_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#binary_path DataHelmTemplate#binary_path}
         '''
         result = self._values.get("binary_path")
         assert result is not None, "Required property 'binary_path' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -2204,17 +2253,17 @@
         self,
         *,
         name: builtins.str,
         value: builtins.str,
         type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#value DataHelmTemplate#value}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#type DataHelmTemplate#type}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#type DataHelmTemplate#type}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e3107b5c6b8ed11069788d0b3982cf940428ac686b9fd0f5a29597828bbe5aba)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -2222,29 +2271,29 @@
             "value": value,
         }
         if type is not None:
             self._values["type"] = type
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#value DataHelmTemplate#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#type DataHelmTemplate#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#type DataHelmTemplate#type}.'''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -2342,14 +2391,233 @@
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf344d6c6d0e3525c45613e9e9c9965817a9ba5bb8aed4c70d3540465ef70091)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
+@jsii.data_type(
+    jsii_type="@cdktf/provider-helm.dataHelmTemplate.DataHelmTemplateSetListStruct",
+    jsii_struct_bases=[],
+    name_mapping={"name": "name", "value": "value"},
+)
+class DataHelmTemplateSetListStruct:
+    def __init__(
+        self,
+        *,
+        name: builtins.str,
+        value: typing.Sequence[builtins.str],
+    ) -> None:
+        '''
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0d42fdc9606495bede7f237b1a9e802de94a71f69efe80fb8c3c065efb2a78e0)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+            "value": value,
+        }
+
+    @builtins.property
+    def name(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.'''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def value(self) -> typing.List[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.'''
+        result = self._values.get("value")
+        assert result is not None, "Required property 'value' is missing"
+        return typing.cast(typing.List[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DataHelmTemplateSetListStruct(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class DataHelmTemplateSetListStructList(
+    _cdktf_9a9027ec.ComplexList,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-helm.dataHelmTemplate.DataHelmTemplateSetListStructList",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        wraps_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c363647b7b98dfae6dea3ed064fbfa5264274ebaf6e903622ffc027360ea3544)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
+
+    @jsii.member(jsii_name="get")
+    def get(self, index: jsii.Number) -> "DataHelmTemplateSetListStructOutputReference":
+        '''
+        :param index: the index of the item to return.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__111974b475103fe7263ddd63889c3425d455b3fae17109a52dac9ee49ca4fdad)
+            check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+        return typing.cast("DataHelmTemplateSetListStructOutputReference", jsii.invoke(self, "get", [index]))
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformAttribute")
+    def _terraform_attribute(self) -> builtins.str:
+        '''The attribute on the parent resource this class is referencing.'''
+        return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
+
+    @_terraform_attribute.setter
+    def _terraform_attribute(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__829c4840c317628f43c98379b5fd3534134d14c21df00c6440bd8d2d68982960)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformAttribute", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformResource")
+    def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
+        '''The parent resource.'''
+        return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
+
+    @_terraform_resource.setter
+    def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bcf08e2cbe2cd3689c4eaac91c7ac6d230fd074d10abd18bcaebbc9a73aa51e0)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformResource", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="wrapsSet")
+    def _wraps_set(self) -> builtins.bool:
+        '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
+        return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
+
+    @_wraps_set.setter
+    def _wraps_set(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__23b597ab3b077d8d80833c8eb6f4622c8eeca04f5a97d4fa747c9f8eed3db6bd)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "wrapsSet", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHelmTemplateSetListStruct]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHelmTemplateSetListStruct]]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHelmTemplateSetListStruct]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f32eba4071b0428b766594486a632f82776cb86fdc6e225d1dc14913219b87ae)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
+class DataHelmTemplateSetListStructOutputReference(
+    _cdktf_9a9027ec.ComplexObject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-helm.dataHelmTemplate.DataHelmTemplateSetListStructOutputReference",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        complex_object_index: jsii.Number,
+        complex_object_is_from_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param complex_object_index: the index of this item in the list.
+        :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6b7db2d482e68961af0c9cb75a431d5c8af5d05104f3dc5c9f4b781e406049f6)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
+            check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
+
+    @builtins.property
+    @jsii.member(jsii_name="nameInput")
+    def name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="valueInput")
+    def value_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "valueInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "name"))
+
+    @name.setter
+    def name(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1990dfb0da6441db22ccdd38a4717adf36677d6fbd7604abf876c197334ac2ac)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "name", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="value")
+    def value(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "value"))
+
+    @value.setter
+    def value(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7434adba18796e6e7a12046632543f0d36a73f9acbb17b92042523a6e0aa2d09)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "value", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[DataHelmTemplateSetListStruct, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[DataHelmTemplateSetListStruct, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[DataHelmTemplateSetListStruct, _cdktf_9a9027ec.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a875cebe0e855ea618c6d23bbe957d7ba99677452ebd01ba71079ff1d9bd1485)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
 class DataHelmTemplateSetOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-helm.dataHelmTemplate.DataHelmTemplateSetOutputReference",
 ):
     def __init__(
         self,
@@ -2455,17 +2723,17 @@
         self,
         *,
         name: builtins.str,
         value: builtins.str,
         type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#value DataHelmTemplate#value}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#type DataHelmTemplate#type}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#type DataHelmTemplate#type}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7b14c003c1e72c0f94da94190926ba8230219d5f38b620f88ba7e9b01fe40ad2)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -2473,29 +2741,29 @@
             "value": value,
         }
         if type is not None:
             self._values["type"] = type
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#value DataHelmTemplate#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#type DataHelmTemplate#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#type DataHelmTemplate#type}.'''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -2700,36 +2968,36 @@
     jsii_type="@cdktf/provider-helm.dataHelmTemplate.DataHelmTemplateSetString",
     jsii_struct_bases=[],
     name_mapping={"name": "name", "value": "value"},
 )
 class DataHelmTemplateSetString:
     def __init__(self, *, name: builtins.str, value: builtins.str) -> None:
         '''
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#value DataHelmTemplate#value}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c83b836dbd7dbbdc2115894cfd13e9de9475d13037a14ca348590dbfa70fc28f)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
             "value": value,
         }
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#name DataHelmTemplate#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#name DataHelmTemplate#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/data-sources/template#value DataHelmTemplate#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/data-sources/template#value DataHelmTemplate#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2913,14 +3181,17 @@
 __all__ = [
     "DataHelmTemplate",
     "DataHelmTemplateConfig",
     "DataHelmTemplatePostrender",
     "DataHelmTemplatePostrenderOutputReference",
     "DataHelmTemplateSet",
     "DataHelmTemplateSetList",
+    "DataHelmTemplateSetListStruct",
+    "DataHelmTemplateSetListStructList",
+    "DataHelmTemplateSetListStructOutputReference",
     "DataHelmTemplateSetOutputReference",
     "DataHelmTemplateSetSensitive",
     "DataHelmTemplateSetSensitiveList",
     "DataHelmTemplateSetSensitiveOutputReference",
     "DataHelmTemplateSetString",
     "DataHelmTemplateSetStringList",
     "DataHelmTemplateSetStringOutputReference",
@@ -2961,14 +3232,15 @@
     repository_cert_file: typing.Optional[builtins.str] = None,
     repository_key_file: typing.Optional[builtins.str] = None,
     repository_password: typing.Optional[builtins.str] = None,
     repository_username: typing.Optional[builtins.str] = None,
     reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSet, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetListStruct, typing.Dict[builtins.str, typing.Any]]]]] = None,
     set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetSensitive, typing.Dict[builtins.str, typing.Any]]]]] = None,
     set_string: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetString, typing.Dict[builtins.str, typing.Any]]]]] = None,
     show_only: typing.Optional[typing.Sequence[builtins.str]] = None,
     skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     skip_tests: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     timeout: typing.Optional[jsii.Number] = None,
     validate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -2989,14 +3261,20 @@
 
 def _typecheckingstub__1596ab16b5d874b157172d384e60dca3a78047fbd42fa1f5b63eee3f239c3aab(
     value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSet, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__152cb09b5fbfc57dbe53841927f1ffb77aaf7ba9a73e8477e7ab141afc3b3863(
+    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetListStruct, typing.Dict[builtins.str, typing.Any]]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__f695897482a9ad07999645b33f485ea7dc3b43747d170cf346beb84d2ac5ea3c(
     value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetSensitive, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9eb5aa1eb8451b1548f355016ba7ed3e5191b60a18ff6392b631264ac3138c2b(
@@ -3283,14 +3561,15 @@
     repository_cert_file: typing.Optional[builtins.str] = None,
     repository_key_file: typing.Optional[builtins.str] = None,
     repository_password: typing.Optional[builtins.str] = None,
     repository_username: typing.Optional[builtins.str] = None,
     reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSet, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetListStruct, typing.Dict[builtins.str, typing.Any]]]]] = None,
     set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetSensitive, typing.Dict[builtins.str, typing.Any]]]]] = None,
     set_string: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataHelmTemplateSetString, typing.Dict[builtins.str, typing.Any]]]]] = None,
     show_only: typing.Optional[typing.Sequence[builtins.str]] = None,
     skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     skip_tests: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     timeout: typing.Optional[jsii.Number] = None,
     validate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -3371,14 +3650,87 @@
 
 def _typecheckingstub__cf344d6c6d0e3525c45613e9e9c9965817a9ba5bb8aed4c70d3540465ef70091(
     value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHelmTemplateSet]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__0d42fdc9606495bede7f237b1a9e802de94a71f69efe80fb8c3c065efb2a78e0(
+    *,
+    name: builtins.str,
+    value: typing.Sequence[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c363647b7b98dfae6dea3ed064fbfa5264274ebaf6e903622ffc027360ea3544(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    wraps_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__111974b475103fe7263ddd63889c3425d455b3fae17109a52dac9ee49ca4fdad(
+    index: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__829c4840c317628f43c98379b5fd3534134d14c21df00c6440bd8d2d68982960(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bcf08e2cbe2cd3689c4eaac91c7ac6d230fd074d10abd18bcaebbc9a73aa51e0(
+    value: _cdktf_9a9027ec.IInterpolatingParent,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__23b597ab3b077d8d80833c8eb6f4622c8eeca04f5a97d4fa747c9f8eed3db6bd(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f32eba4071b0428b766594486a632f82776cb86fdc6e225d1dc14913219b87ae(
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHelmTemplateSetListStruct]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6b7db2d482e68961af0c9cb75a431d5c8af5d05104f3dc5c9f4b781e406049f6(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    complex_object_index: jsii.Number,
+    complex_object_is_from_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1990dfb0da6441db22ccdd38a4717adf36677d6fbd7604abf876c197334ac2ac(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7434adba18796e6e7a12046632543f0d36a73f9acbb17b92042523a6e0aa2d09(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a875cebe0e855ea618c6d23bbe957d7ba99677452ebd01ba71079ff1d9bd1485(
+    value: typing.Optional[typing.Union[DataHelmTemplateSetListStruct, _cdktf_9a9027ec.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__cdc6b11db958720bcf5c5e86250bc1a0ac99593b88ac8aaf121c720790e61556(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/provider/__init__.py` & `cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/provider/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`helm`](https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs).
+Refer to the Terraform Registory for docs: [`helm`](https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HelmProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-helm.provider.HelmProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs helm}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs helm}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
@@ -41,29 +41,29 @@
         kubernetes: typing.Optional[typing.Union["HelmProviderKubernetes", typing.Dict[builtins.str, typing.Any]]] = None,
         plugins_path: typing.Optional[builtins.str] = None,
         registry: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["HelmProviderRegistry", typing.Dict[builtins.str, typing.Any]]]]] = None,
         registry_config_path: typing.Optional[builtins.str] = None,
         repository_cache: typing.Optional[builtins.str] = None,
         repository_config_path: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs helm} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs helm} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#alias HelmProvider#alias}
-        :param burst_limit: Helm burst limit. Increase this if you have a cluster with many CRDs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#burst_limit HelmProvider#burst_limit}
-        :param debug: Debug indicates whether or not Helm is running in Debug mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#debug HelmProvider#debug}
-        :param experiments: experiments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#experiments HelmProvider#experiments}
-        :param helm_driver: The backend storage driver. Values are: configmap, secret, memory, sql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#helm_driver HelmProvider#helm_driver}
-        :param kubernetes: kubernetes block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#kubernetes HelmProvider#kubernetes}
-        :param plugins_path: The path to the helm plugins directory. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#plugins_path HelmProvider#plugins_path}
-        :param registry: registry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#registry HelmProvider#registry}
-        :param registry_config_path: The path to the registry config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#registry_config_path HelmProvider#registry_config_path}
-        :param repository_cache: The path to the file containing cached repository indexes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#repository_cache HelmProvider#repository_cache}
-        :param repository_config_path: The path to the file containing repository names and URLs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#repository_config_path HelmProvider#repository_config_path}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#alias HelmProvider#alias}
+        :param burst_limit: Helm burst limit. Increase this if you have a cluster with many CRDs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#burst_limit HelmProvider#burst_limit}
+        :param debug: Debug indicates whether or not Helm is running in Debug mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#debug HelmProvider#debug}
+        :param experiments: experiments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#experiments HelmProvider#experiments}
+        :param helm_driver: The backend storage driver. Values are: configmap, secret, memory, sql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#helm_driver HelmProvider#helm_driver}
+        :param kubernetes: kubernetes block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#kubernetes HelmProvider#kubernetes}
+        :param plugins_path: The path to the helm plugins directory. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#plugins_path HelmProvider#plugins_path}
+        :param registry: registry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#registry HelmProvider#registry}
+        :param registry_config_path: The path to the registry config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#registry_config_path HelmProvider#registry_config_path}
+        :param repository_cache: The path to the file containing cached repository indexes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#repository_cache HelmProvider#repository_cache}
+        :param repository_config_path: The path to the file containing repository names and URLs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#repository_config_path HelmProvider#repository_config_path}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1a9b1d29236885254322c77ebb49db4debaa433e29b9dba83d7fbc53fe1d63a5)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HelmProviderConfig(
             alias=alias,
@@ -366,25 +366,25 @@
         plugins_path: typing.Optional[builtins.str] = None,
         registry: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["HelmProviderRegistry", typing.Dict[builtins.str, typing.Any]]]]] = None,
         registry_config_path: typing.Optional[builtins.str] = None,
         repository_cache: typing.Optional[builtins.str] = None,
         repository_config_path: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#alias HelmProvider#alias}
-        :param burst_limit: Helm burst limit. Increase this if you have a cluster with many CRDs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#burst_limit HelmProvider#burst_limit}
-        :param debug: Debug indicates whether or not Helm is running in Debug mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#debug HelmProvider#debug}
-        :param experiments: experiments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#experiments HelmProvider#experiments}
-        :param helm_driver: The backend storage driver. Values are: configmap, secret, memory, sql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#helm_driver HelmProvider#helm_driver}
-        :param kubernetes: kubernetes block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#kubernetes HelmProvider#kubernetes}
-        :param plugins_path: The path to the helm plugins directory. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#plugins_path HelmProvider#plugins_path}
-        :param registry: registry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#registry HelmProvider#registry}
-        :param registry_config_path: The path to the registry config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#registry_config_path HelmProvider#registry_config_path}
-        :param repository_cache: The path to the file containing cached repository indexes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#repository_cache HelmProvider#repository_cache}
-        :param repository_config_path: The path to the file containing repository names and URLs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#repository_config_path HelmProvider#repository_config_path}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#alias HelmProvider#alias}
+        :param burst_limit: Helm burst limit. Increase this if you have a cluster with many CRDs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#burst_limit HelmProvider#burst_limit}
+        :param debug: Debug indicates whether or not Helm is running in Debug mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#debug HelmProvider#debug}
+        :param experiments: experiments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#experiments HelmProvider#experiments}
+        :param helm_driver: The backend storage driver. Values are: configmap, secret, memory, sql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#helm_driver HelmProvider#helm_driver}
+        :param kubernetes: kubernetes block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#kubernetes HelmProvider#kubernetes}
+        :param plugins_path: The path to the helm plugins directory. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#plugins_path HelmProvider#plugins_path}
+        :param registry: registry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#registry HelmProvider#registry}
+        :param registry_config_path: The path to the registry config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#registry_config_path HelmProvider#registry_config_path}
+        :param repository_cache: The path to the file containing cached repository indexes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#repository_cache HelmProvider#repository_cache}
+        :param repository_config_path: The path to the file containing repository names and URLs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#repository_config_path HelmProvider#repository_config_path}
         '''
         if isinstance(experiments, dict):
             experiments = HelmProviderExperiments(**experiments)
         if isinstance(kubernetes, dict):
             kubernetes = HelmProviderKubernetes(**kubernetes)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__caf846e980a90ecff087864941949dc254940696c8e5d0be8d4bae4f0f4aa0a9)
@@ -423,109 +423,109 @@
         if repository_config_path is not None:
             self._values["repository_config_path"] = repository_config_path
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#alias HelmProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#alias HelmProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def burst_limit(self) -> typing.Optional[jsii.Number]:
         '''Helm burst limit. Increase this if you have a cluster with many CRDs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#burst_limit HelmProvider#burst_limit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#burst_limit HelmProvider#burst_limit}
         '''
         result = self._values.get("burst_limit")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def debug(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Debug indicates whether or not Helm is running in Debug mode.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#debug HelmProvider#debug}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#debug HelmProvider#debug}
         '''
         result = self._values.get("debug")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def experiments(self) -> typing.Optional["HelmProviderExperiments"]:
         '''experiments block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#experiments HelmProvider#experiments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#experiments HelmProvider#experiments}
         '''
         result = self._values.get("experiments")
         return typing.cast(typing.Optional["HelmProviderExperiments"], result)
 
     @builtins.property
     def helm_driver(self) -> typing.Optional[builtins.str]:
         '''The backend storage driver. Values are: configmap, secret, memory, sql.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#helm_driver HelmProvider#helm_driver}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#helm_driver HelmProvider#helm_driver}
         '''
         result = self._values.get("helm_driver")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def kubernetes(self) -> typing.Optional["HelmProviderKubernetes"]:
         '''kubernetes block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#kubernetes HelmProvider#kubernetes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#kubernetes HelmProvider#kubernetes}
         '''
         result = self._values.get("kubernetes")
         return typing.cast(typing.Optional["HelmProviderKubernetes"], result)
 
     @builtins.property
     def plugins_path(self) -> typing.Optional[builtins.str]:
         '''The path to the helm plugins directory.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#plugins_path HelmProvider#plugins_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#plugins_path HelmProvider#plugins_path}
         '''
         result = self._values.get("plugins_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def registry(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["HelmProviderRegistry"]]]:
         '''registry block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#registry HelmProvider#registry}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#registry HelmProvider#registry}
         '''
         result = self._values.get("registry")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["HelmProviderRegistry"]]], result)
 
     @builtins.property
     def registry_config_path(self) -> typing.Optional[builtins.str]:
         '''The path to the registry config file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#registry_config_path HelmProvider#registry_config_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#registry_config_path HelmProvider#registry_config_path}
         '''
         result = self._values.get("registry_config_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_cache(self) -> typing.Optional[builtins.str]:
         '''The path to the file containing cached repository indexes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#repository_cache HelmProvider#repository_cache}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#repository_cache HelmProvider#repository_cache}
         '''
         result = self._values.get("repository_cache")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_config_path(self) -> typing.Optional[builtins.str]:
         '''The path to the file containing repository names and URLs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#repository_config_path HelmProvider#repository_config_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#repository_config_path HelmProvider#repository_config_path}
         '''
         result = self._values.get("repository_config_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -546,30 +546,30 @@
 class HelmProviderExperiments:
     def __init__(
         self,
         *,
         manifest: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param manifest: Enable full diff by storing the rendered manifest in the state. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#manifest HelmProvider#manifest}
+        :param manifest: Enable full diff by storing the rendered manifest in the state. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#manifest HelmProvider#manifest}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0a0975af09e993360c7b82d25c4fdbe476021cece87b3feb51429d13f8dac830)
             check_type(argname="argument manifest", value=manifest, expected_type=type_hints["manifest"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if manifest is not None:
             self._values["manifest"] = manifest
 
     @builtins.property
     def manifest(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Enable full diff by storing the rendered manifest in the state.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#manifest HelmProvider#manifest}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#manifest HelmProvider#manifest}
         '''
         result = self._values.get("manifest")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -620,29 +620,29 @@
         insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         password: typing.Optional[builtins.str] = None,
         proxy_url: typing.Optional[builtins.str] = None,
         token: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param client_certificate: PEM-encoded client certificate for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#client_certificate HelmProvider#client_certificate}
-        :param client_key: PEM-encoded client certificate key for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#client_key HelmProvider#client_key}
-        :param cluster_ca_certificate: PEM-encoded root certificates bundle for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#cluster_ca_certificate HelmProvider#cluster_ca_certificate}
-        :param config_context: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_context HelmProvider#config_context}.
-        :param config_context_auth_info: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_context_auth_info HelmProvider#config_context_auth_info}.
-        :param config_context_cluster: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_context_cluster HelmProvider#config_context_cluster}.
-        :param config_path: Path to the kube config file. Can be set with KUBE_CONFIG_PATH. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_path HelmProvider#config_path}
-        :param config_paths: A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_paths HelmProvider#config_paths}
-        :param exec: exec block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#exec HelmProvider#exec}
-        :param host: The hostname (in form of URI) of Kubernetes master. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#host HelmProvider#host}
-        :param insecure: Whether server should be accessed without verifying the TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#insecure HelmProvider#insecure}
-        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#password HelmProvider#password}
-        :param proxy_url: URL to the proxy to be used for all API requests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#proxy_url HelmProvider#proxy_url}
-        :param token: Token to authenticate an service account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#token HelmProvider#token}
-        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#username HelmProvider#username}
+        :param client_certificate: PEM-encoded client certificate for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#client_certificate HelmProvider#client_certificate}
+        :param client_key: PEM-encoded client certificate key for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#client_key HelmProvider#client_key}
+        :param cluster_ca_certificate: PEM-encoded root certificates bundle for TLS authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#cluster_ca_certificate HelmProvider#cluster_ca_certificate}
+        :param config_context: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_context HelmProvider#config_context}.
+        :param config_context_auth_info: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_context_auth_info HelmProvider#config_context_auth_info}.
+        :param config_context_cluster: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_context_cluster HelmProvider#config_context_cluster}.
+        :param config_path: Path to the kube config file. Can be set with KUBE_CONFIG_PATH. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_path HelmProvider#config_path}
+        :param config_paths: A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_paths HelmProvider#config_paths}
+        :param exec: exec block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#exec HelmProvider#exec}
+        :param host: The hostname (in form of URI) of Kubernetes master. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#host HelmProvider#host}
+        :param insecure: Whether server should be accessed without verifying the TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#insecure HelmProvider#insecure}
+        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#password HelmProvider#password}
+        :param proxy_url: URL to the proxy to be used for all API requests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#proxy_url HelmProvider#proxy_url}
+        :param token: Token to authenticate an service account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#token HelmProvider#token}
+        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#username HelmProvider#username}
         '''
         if isinstance(exec, dict):
             exec = HelmProviderKubernetesExec(**exec)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__52b2f14a81c02bbc4322b38259371fa6624c27f8399267e3fbd8d6d1383c420d)
             check_type(argname="argument client_certificate", value=client_certificate, expected_type=type_hints["client_certificate"])
             check_type(argname="argument client_key", value=client_key, expected_type=type_hints["client_key"])
@@ -691,134 +691,134 @@
         if username is not None:
             self._values["username"] = username
 
     @builtins.property
     def client_certificate(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded client certificate for TLS authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#client_certificate HelmProvider#client_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#client_certificate HelmProvider#client_certificate}
         '''
         result = self._values.get("client_certificate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_key(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded client certificate key for TLS authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#client_key HelmProvider#client_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#client_key HelmProvider#client_key}
         '''
         result = self._values.get("client_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cluster_ca_certificate(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded root certificates bundle for TLS authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#cluster_ca_certificate HelmProvider#cluster_ca_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#cluster_ca_certificate HelmProvider#cluster_ca_certificate}
         '''
         result = self._values.get("cluster_ca_certificate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_context(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_context HelmProvider#config_context}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_context HelmProvider#config_context}.'''
         result = self._values.get("config_context")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_context_auth_info(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_context_auth_info HelmProvider#config_context_auth_info}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_context_auth_info HelmProvider#config_context_auth_info}.'''
         result = self._values.get("config_context_auth_info")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_context_cluster(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_context_cluster HelmProvider#config_context_cluster}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_context_cluster HelmProvider#config_context_cluster}.'''
         result = self._values.get("config_context_cluster")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_path(self) -> typing.Optional[builtins.str]:
         '''Path to the kube config file. Can be set with KUBE_CONFIG_PATH.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_path HelmProvider#config_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_path HelmProvider#config_path}
         '''
         result = self._values.get("config_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def config_paths(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of paths to kube config files. Can be set with KUBE_CONFIG_PATHS environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#config_paths HelmProvider#config_paths}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#config_paths HelmProvider#config_paths}
         '''
         result = self._values.get("config_paths")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def exec(self) -> typing.Optional["HelmProviderKubernetesExec"]:
         '''exec block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#exec HelmProvider#exec}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#exec HelmProvider#exec}
         '''
         result = self._values.get("exec")
         return typing.cast(typing.Optional["HelmProviderKubernetesExec"], result)
 
     @builtins.property
     def host(self) -> typing.Optional[builtins.str]:
         '''The hostname (in form of URI) of Kubernetes master.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#host HelmProvider#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#host HelmProvider#host}
         '''
         result = self._values.get("host")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether server should be accessed without verifying the TLS certificate.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#insecure HelmProvider#insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#insecure HelmProvider#insecure}
         '''
         result = self._values.get("insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#password HelmProvider#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#password HelmProvider#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def proxy_url(self) -> typing.Optional[builtins.str]:
         '''URL to the proxy to be used for all API requests.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#proxy_url HelmProvider#proxy_url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#proxy_url HelmProvider#proxy_url}
         '''
         result = self._values.get("proxy_url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''Token to authenticate an service account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#token HelmProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#token HelmProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
         '''The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#username HelmProvider#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#username HelmProvider#username}
         '''
         result = self._values.get("username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -847,18 +847,18 @@
         *,
         api_version: builtins.str,
         command: builtins.str,
         args: typing.Optional[typing.Sequence[builtins.str]] = None,
         env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
         '''
-        :param api_version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#api_version HelmProvider#api_version}.
-        :param command: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#command HelmProvider#command}.
-        :param args: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#args HelmProvider#args}.
-        :param env: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#env HelmProvider#env}.
+        :param api_version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#api_version HelmProvider#api_version}.
+        :param command: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#command HelmProvider#command}.
+        :param args: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#args HelmProvider#args}.
+        :param env: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#env HelmProvider#env}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e7e441f97cccff737d356dc06e6be332ad7fe161138eef9da0ab2873bfb11861)
             check_type(argname="argument api_version", value=api_version, expected_type=type_hints["api_version"])
             check_type(argname="argument command", value=command, expected_type=type_hints["command"])
             check_type(argname="argument args", value=args, expected_type=type_hints["args"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
@@ -869,35 +869,35 @@
         if args is not None:
             self._values["args"] = args
         if env is not None:
             self._values["env"] = env
 
     @builtins.property
     def api_version(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#api_version HelmProvider#api_version}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#api_version HelmProvider#api_version}.'''
         result = self._values.get("api_version")
         assert result is not None, "Required property 'api_version' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def command(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#command HelmProvider#command}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#command HelmProvider#command}.'''
         result = self._values.get("command")
         assert result is not None, "Required property 'command' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def args(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#args HelmProvider#args}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#args HelmProvider#args}.'''
         result = self._values.get("args")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def env(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#env HelmProvider#env}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#env HelmProvider#env}.'''
         result = self._values.get("env")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -919,17 +919,17 @@
         self,
         *,
         password: builtins.str,
         url: builtins.str,
         username: builtins.str,
     ) -> None:
         '''
-        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#password HelmProvider#password}
-        :param url: OCI URL in form of oci://host:port or oci://host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#url HelmProvider#url}
-        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#username HelmProvider#username}
+        :param password: The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#password HelmProvider#password}
+        :param url: OCI URL in form of oci://host:port or oci://host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#url HelmProvider#url}
+        :param username: The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#username HelmProvider#username}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1d0228d63de5ac28ee319ff1a2e48bc5105e8a1a7b1ac4396e9898e244d8396a)
             check_type(argname="argument password", value=password, expected_type=type_hints["password"])
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
             check_type(argname="argument username", value=username, expected_type=type_hints["username"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -938,35 +938,35 @@
             "username": username,
         }
 
     @builtins.property
     def password(self) -> builtins.str:
         '''The password to use for HTTP basic authentication when accessing the Kubernetes master endpoint.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#password HelmProvider#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#password HelmProvider#password}
         '''
         result = self._values.get("password")
         assert result is not None, "Required property 'password' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def url(self) -> builtins.str:
         '''OCI URL in form of oci://host:port or oci://host.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#url HelmProvider#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#url HelmProvider#url}
         '''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username to use for HTTP basic authentication when accessing the Kubernetes master endpoint.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs#username HelmProvider#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs#username HelmProvider#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm/release/__init__.py` & `cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm/release/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `helm_release`
 
-Refer to the Terraform Registory for docs: [`helm_release`](https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release).
+Refer to the Terraform Registory for docs: [`helm_release`](https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Release(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-helm.release.Release",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release helm_release}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release helm_release}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         chart: builtins.str,
@@ -60,14 +60,15 @@
         repository_cert_file: typing.Optional[builtins.str] = None,
         repository_key_file: typing.Optional[builtins.str] = None,
         repository_password: typing.Optional[builtins.str] = None,
         repository_username: typing.Optional[builtins.str] = None,
         reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSet", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSetListStruct", typing.Dict[builtins.str, typing.Any]]]]] = None,
         set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSetSensitive", typing.Dict[builtins.str, typing.Any]]]]] = None,
         skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         timeout: typing.Optional[jsii.Number] = None,
         values: typing.Optional[typing.Sequence[builtins.str]] = None,
         verify: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         version: typing.Optional[builtins.str] = None,
         wait: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -76,57 +77,58 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release helm_release} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release helm_release} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#chart Release#chart}
-        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#name Release#name}
-        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#atomic Release#atomic}
-        :param cleanup_on_fail: Allow deletion of new resources created in this upgrade when upgrade fails. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#cleanup_on_fail Release#cleanup_on_fail}
-        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#create_namespace Release#create_namespace}
-        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#dependency_update Release#dependency_update}
-        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#description Release#description}
-        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#devel Release#devel}
-        :param disable_crd_hooks: Prevent CRD hooks from, running, but run other hooks. See helm install --no-crd-hook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_crd_hooks Release#disable_crd_hooks}
-        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_openapi_validation Release#disable_openapi_validation}
-        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_webhooks Release#disable_webhooks}
-        :param force_update: Force resource update through delete/recreate if needed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#force_update Release#force_update}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#id Release#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#keyring Release#keyring}
-        :param lint: Run helm lint when planning. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#lint Release#lint}
-        :param max_history: Limit the maximum number of revisions saved per release. Use 0 for no limit. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#max_history Release#max_history}
-        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#namespace Release#namespace}
-        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#pass_credentials Release#pass_credentials}
-        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#postrender Release#postrender}
-        :param recreate_pods: Perform pods restart during upgrade/rollback. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#recreate_pods Release#recreate_pods}
-        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#render_subchart_notes Release#render_subchart_notes}
-        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#replace Release#replace}
-        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository Release#repository}
-        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_ca_file Release#repository_ca_file}
-        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_cert_file Release#repository_cert_file}
-        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_key_file Release#repository_key_file}
-        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_password Release#repository_password}
-        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_username Release#repository_username}
-        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#reset_values Release#reset_values}
-        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#reuse_values Release#reuse_values}
-        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#set Release#set}
-        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#set_sensitive Release#set_sensitive}
-        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#skip_crds Release#skip_crds}
-        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#timeout Release#timeout}
-        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#values Release#values}
-        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#verify Release#verify}
-        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#version Release#version}
-        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#wait Release#wait}
-        :param wait_for_jobs: If wait is enabled, will wait until all Jobs have been completed before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#wait_for_jobs Release#wait_for_jobs}
+        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#chart Release#chart}
+        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}
+        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#atomic Release#atomic}
+        :param cleanup_on_fail: Allow deletion of new resources created in this upgrade when upgrade fails. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#cleanup_on_fail Release#cleanup_on_fail}
+        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#create_namespace Release#create_namespace}
+        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#dependency_update Release#dependency_update}
+        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#description Release#description}
+        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#devel Release#devel}
+        :param disable_crd_hooks: Prevent CRD hooks from, running, but run other hooks. See helm install --no-crd-hook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_crd_hooks Release#disable_crd_hooks}
+        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_openapi_validation Release#disable_openapi_validation}
+        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_webhooks Release#disable_webhooks}
+        :param force_update: Force resource update through delete/recreate if needed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#force_update Release#force_update}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#id Release#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#keyring Release#keyring}
+        :param lint: Run helm lint when planning. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#lint Release#lint}
+        :param max_history: Limit the maximum number of revisions saved per release. Use 0 for no limit. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#max_history Release#max_history}
+        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#namespace Release#namespace}
+        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#pass_credentials Release#pass_credentials}
+        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#postrender Release#postrender}
+        :param recreate_pods: Perform pods restart during upgrade/rollback. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#recreate_pods Release#recreate_pods}
+        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#render_subchart_notes Release#render_subchart_notes}
+        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#replace Release#replace}
+        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository Release#repository}
+        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_ca_file Release#repository_ca_file}
+        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_cert_file Release#repository_cert_file}
+        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_key_file Release#repository_key_file}
+        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_password Release#repository_password}
+        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_username Release#repository_username}
+        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#reset_values Release#reset_values}
+        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#reuse_values Release#reuse_values}
+        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set Release#set}
+        :param set_list: set_list block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set_list Release#set_list}
+        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set_sensitive Release#set_sensitive}
+        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#skip_crds Release#skip_crds}
+        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#timeout Release#timeout}
+        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#values Release#values}
+        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#verify Release#verify}
+        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#version Release#version}
+        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#wait Release#wait}
+        :param wait_for_jobs: If wait is enabled, will wait until all Jobs have been completed before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#wait_for_jobs Release#wait_for_jobs}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -163,14 +165,15 @@
             repository_cert_file=repository_cert_file,
             repository_key_file=repository_key_file,
             repository_password=repository_password,
             repository_username=repository_username,
             reset_values=reset_values,
             reuse_values=reuse_values,
             set=set,
+            set_list=set_list,
             set_sensitive=set_sensitive,
             skip_crds=skip_crds,
             timeout=timeout,
             values=values,
             verify=verify,
             version=version,
             wait=wait,
@@ -190,16 +193,16 @@
     def put_postrender(
         self,
         *,
         binary_path: builtins.str,
         args: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#binary_path Release#binary_path}
-        :param args: an argument to the post-renderer (can specify multiple). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#args Release#args}
+        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#binary_path Release#binary_path}
+        :param args: an argument to the post-renderer (can specify multiple). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#args Release#args}
         '''
         value = ReleasePostrender(binary_path=binary_path, args=args)
 
         return typing.cast(None, jsii.invoke(self, "putPostrender", [value]))
 
     @jsii.member(jsii_name="putSet")
     def put_set(
@@ -210,14 +213,27 @@
         :param value: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6b72a3657c0803010731fa3fd2044a0f404b98ac9399b1fb916895c0de83919d)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putSet", [value]))
 
+    @jsii.member(jsii_name="putSetList")
+    def put_set_list(
+        self,
+        value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSetListStruct", typing.Dict[builtins.str, typing.Any]]]],
+    ) -> None:
+        '''
+        :param value: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__64e66f987c47878d4a6946a5a1dc06f0d9f1ca6ba2ae98348676c4bd5950c185)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        return typing.cast(None, jsii.invoke(self, "putSetList", [value]))
+
     @jsii.member(jsii_name="putSetSensitive")
     def put_set_sensitive(
         self,
         value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSetSensitive", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
         :param value: -
@@ -339,14 +355,18 @@
     def reset_reuse_values(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetReuseValues", []))
 
     @jsii.member(jsii_name="resetSet")
     def reset_set(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSet", []))
 
+    @jsii.member(jsii_name="resetSetList")
+    def reset_set_list(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetSetList", []))
+
     @jsii.member(jsii_name="resetSetSensitive")
     def reset_set_sensitive(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSetSensitive", []))
 
     @jsii.member(jsii_name="resetSkipCrds")
     def reset_skip_crds(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSkipCrds", []))
@@ -401,14 +421,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="set")
     def set(self) -> "ReleaseSetList":
         return typing.cast("ReleaseSetList", jsii.get(self, "set"))
 
     @builtins.property
+    @jsii.member(jsii_name="setList")
+    def set_list(self) -> "ReleaseSetListStructList":
+        return typing.cast("ReleaseSetListStructList", jsii.get(self, "setList"))
+
+    @builtins.property
     @jsii.member(jsii_name="setSensitive")
     def set_sensitive(self) -> "ReleaseSetSensitiveList":
         return typing.cast("ReleaseSetSensitiveList", jsii.get(self, "setSensitive"))
 
     @builtins.property
     @jsii.member(jsii_name="status")
     def status(self) -> builtins.str:
@@ -600,14 +625,21 @@
     @jsii.member(jsii_name="setInput")
     def set_input(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSet"]]]:
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSet"]]], jsii.get(self, "setInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="setListInput")
+    def set_list_input(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetListStruct"]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetListStruct"]]], jsii.get(self, "setListInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="setSensitiveInput")
     def set_sensitive_input(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetSensitive"]]]:
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetSensitive"]]], jsii.get(self, "setSensitiveInput"))
 
     @builtins.property
@@ -1200,14 +1232,15 @@
         "repository_cert_file": "repositoryCertFile",
         "repository_key_file": "repositoryKeyFile",
         "repository_password": "repositoryPassword",
         "repository_username": "repositoryUsername",
         "reset_values": "resetValues",
         "reuse_values": "reuseValues",
         "set": "set",
+        "set_list": "setList",
         "set_sensitive": "setSensitive",
         "skip_crds": "skipCrds",
         "timeout": "timeout",
         "values": "values",
         "verify": "verify",
         "version": "version",
         "wait": "wait",
@@ -1252,14 +1285,15 @@
         repository_cert_file: typing.Optional[builtins.str] = None,
         repository_key_file: typing.Optional[builtins.str] = None,
         repository_password: typing.Optional[builtins.str] = None,
         repository_username: typing.Optional[builtins.str] = None,
         reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSet", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSetListStruct", typing.Dict[builtins.str, typing.Any]]]]] = None,
         set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ReleaseSetSensitive", typing.Dict[builtins.str, typing.Any]]]]] = None,
         skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         timeout: typing.Optional[jsii.Number] = None,
         values: typing.Optional[typing.Sequence[builtins.str]] = None,
         verify: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         version: typing.Optional[builtins.str] = None,
         wait: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -1269,53 +1303,54 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#chart Release#chart}
-        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#name Release#name}
-        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#atomic Release#atomic}
-        :param cleanup_on_fail: Allow deletion of new resources created in this upgrade when upgrade fails. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#cleanup_on_fail Release#cleanup_on_fail}
-        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#create_namespace Release#create_namespace}
-        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#dependency_update Release#dependency_update}
-        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#description Release#description}
-        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#devel Release#devel}
-        :param disable_crd_hooks: Prevent CRD hooks from, running, but run other hooks. See helm install --no-crd-hook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_crd_hooks Release#disable_crd_hooks}
-        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_openapi_validation Release#disable_openapi_validation}
-        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_webhooks Release#disable_webhooks}
-        :param force_update: Force resource update through delete/recreate if needed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#force_update Release#force_update}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#id Release#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#keyring Release#keyring}
-        :param lint: Run helm lint when planning. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#lint Release#lint}
-        :param max_history: Limit the maximum number of revisions saved per release. Use 0 for no limit. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#max_history Release#max_history}
-        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#namespace Release#namespace}
-        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#pass_credentials Release#pass_credentials}
-        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#postrender Release#postrender}
-        :param recreate_pods: Perform pods restart during upgrade/rollback. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#recreate_pods Release#recreate_pods}
-        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#render_subchart_notes Release#render_subchart_notes}
-        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#replace Release#replace}
-        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository Release#repository}
-        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_ca_file Release#repository_ca_file}
-        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_cert_file Release#repository_cert_file}
-        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_key_file Release#repository_key_file}
-        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_password Release#repository_password}
-        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_username Release#repository_username}
-        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#reset_values Release#reset_values}
-        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#reuse_values Release#reuse_values}
-        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#set Release#set}
-        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#set_sensitive Release#set_sensitive}
-        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#skip_crds Release#skip_crds}
-        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#timeout Release#timeout}
-        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#values Release#values}
-        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#verify Release#verify}
-        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#version Release#version}
-        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#wait Release#wait}
-        :param wait_for_jobs: If wait is enabled, will wait until all Jobs have been completed before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#wait_for_jobs Release#wait_for_jobs}
+        :param chart: Chart name to be installed. A path may be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#chart Release#chart}
+        :param name: Release name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}
+        :param atomic: If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#atomic Release#atomic}
+        :param cleanup_on_fail: Allow deletion of new resources created in this upgrade when upgrade fails. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#cleanup_on_fail Release#cleanup_on_fail}
+        :param create_namespace: Create the namespace if it does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#create_namespace Release#create_namespace}
+        :param dependency_update: Run helm dependency update before installing the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#dependency_update Release#dependency_update}
+        :param description: Add a custom description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#description Release#description}
+        :param devel: Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#devel Release#devel}
+        :param disable_crd_hooks: Prevent CRD hooks from, running, but run other hooks. See helm install --no-crd-hook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_crd_hooks Release#disable_crd_hooks}
+        :param disable_openapi_validation: If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_openapi_validation Release#disable_openapi_validation}
+        :param disable_webhooks: Prevent hooks from running. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_webhooks Release#disable_webhooks}
+        :param force_update: Force resource update through delete/recreate if needed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#force_update Release#force_update}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#id Release#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param keyring: Location of public keys used for verification. Used only if ``verify`` is true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#keyring Release#keyring}
+        :param lint: Run helm lint when planning. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#lint Release#lint}
+        :param max_history: Limit the maximum number of revisions saved per release. Use 0 for no limit. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#max_history Release#max_history}
+        :param namespace: Namespace to install the release into. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#namespace Release#namespace}
+        :param pass_credentials: Pass credentials to all domains. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#pass_credentials Release#pass_credentials}
+        :param postrender: postrender block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#postrender Release#postrender}
+        :param recreate_pods: Perform pods restart during upgrade/rollback. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#recreate_pods Release#recreate_pods}
+        :param render_subchart_notes: If set, render subchart notes along with the parent. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#render_subchart_notes Release#render_subchart_notes}
+        :param replace: Re-use the given name, even if that name is already used. This is unsafe in production. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#replace Release#replace}
+        :param repository: Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository Release#repository}
+        :param repository_ca_file: The Repositories CA File. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_ca_file Release#repository_ca_file}
+        :param repository_cert_file: The repositories cert file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_cert_file Release#repository_cert_file}
+        :param repository_key_file: The repositories cert key file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_key_file Release#repository_key_file}
+        :param repository_password: Password for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_password Release#repository_password}
+        :param repository_username: Username for HTTP basic authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_username Release#repository_username}
+        :param reset_values: When upgrading, reset the values to the ones built into the chart. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#reset_values Release#reset_values}
+        :param reuse_values: When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#reuse_values Release#reuse_values}
+        :param set: set block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set Release#set}
+        :param set_list: set_list block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set_list Release#set_list}
+        :param set_sensitive: set_sensitive block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set_sensitive Release#set_sensitive}
+        :param skip_crds: If set, no CRDs will be installed. By default, CRDs are installed if not already present. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#skip_crds Release#skip_crds}
+        :param timeout: Time in seconds to wait for any individual kubernetes operation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#timeout Release#timeout}
+        :param values: List of values in raw yaml format to pass to helm. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#values Release#values}
+        :param verify: Verify the package before installing it. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#verify Release#verify}
+        :param version: Specify the exact chart version to install. If this is not specified, the latest version is installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#version Release#version}
+        :param wait: Will wait until all resources are in a ready state before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#wait Release#wait}
+        :param wait_for_jobs: If wait is enabled, will wait until all Jobs have been completed before marking the release as successful. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#wait_for_jobs Release#wait_for_jobs}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(postrender, dict):
             postrender = ReleasePostrender(**postrender)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3351956da04ddf8ca86567e1dd64c43a3a02b9b30bc17a13da12597bc326e840)
@@ -1353,14 +1388,15 @@
             check_type(argname="argument repository_cert_file", value=repository_cert_file, expected_type=type_hints["repository_cert_file"])
             check_type(argname="argument repository_key_file", value=repository_key_file, expected_type=type_hints["repository_key_file"])
             check_type(argname="argument repository_password", value=repository_password, expected_type=type_hints["repository_password"])
             check_type(argname="argument repository_username", value=repository_username, expected_type=type_hints["repository_username"])
             check_type(argname="argument reset_values", value=reset_values, expected_type=type_hints["reset_values"])
             check_type(argname="argument reuse_values", value=reuse_values, expected_type=type_hints["reuse_values"])
             check_type(argname="argument set", value=set, expected_type=type_hints["set"])
+            check_type(argname="argument set_list", value=set_list, expected_type=type_hints["set_list"])
             check_type(argname="argument set_sensitive", value=set_sensitive, expected_type=type_hints["set_sensitive"])
             check_type(argname="argument skip_crds", value=skip_crds, expected_type=type_hints["skip_crds"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument verify", value=verify, expected_type=type_hints["verify"])
             check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             check_type(argname="argument wait", value=wait, expected_type=type_hints["wait"])
@@ -1437,14 +1473,16 @@
             self._values["repository_username"] = repository_username
         if reset_values is not None:
             self._values["reset_values"] = reset_values
         if reuse_values is not None:
             self._values["reuse_values"] = reuse_values
         if set is not None:
             self._values["set"] = set
+        if set_list is not None:
+            self._values["set_list"] = set_list
         if set_sensitive is not None:
             self._values["set_sensitive"] = set_sensitive
         if skip_crds is not None:
             self._values["skip_crds"] = skip_crds
         if timeout is not None:
             self._values["timeout"] = timeout
         if values is not None:
@@ -1522,404 +1560,415 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def chart(self) -> builtins.str:
         '''Chart name to be installed. A path may be used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#chart Release#chart}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#chart Release#chart}
         '''
         result = self._values.get("chart")
         assert result is not None, "Required property 'chart' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Release name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#name Release#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def atomic(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, installation process purges chart on fail. The wait flag will be set automatically if atomic is used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#atomic Release#atomic}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#atomic Release#atomic}
         '''
         result = self._values.get("atomic")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def cleanup_on_fail(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Allow deletion of new resources created in this upgrade when upgrade fails.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#cleanup_on_fail Release#cleanup_on_fail}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#cleanup_on_fail Release#cleanup_on_fail}
         '''
         result = self._values.get("cleanup_on_fail")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def create_namespace(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Create the namespace if it does not exist.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#create_namespace Release#create_namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#create_namespace Release#create_namespace}
         '''
         result = self._values.get("create_namespace")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def dependency_update(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Run helm dependency update before installing the chart.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#dependency_update Release#dependency_update}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#dependency_update Release#dependency_update}
         '''
         result = self._values.get("dependency_update")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Add a custom description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#description Release#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#description Release#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def devel(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Use chart development versions, too. Equivalent to version '>0.0.0-0'. If ``version`` is set, this is ignored.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#devel Release#devel}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#devel Release#devel}
         '''
         result = self._values.get("devel")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def disable_crd_hooks(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Prevent CRD hooks from, running, but run other hooks.  See helm install --no-crd-hook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_crd_hooks Release#disable_crd_hooks}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_crd_hooks Release#disable_crd_hooks}
         '''
         result = self._values.get("disable_crd_hooks")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def disable_openapi_validation(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_openapi_validation Release#disable_openapi_validation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_openapi_validation Release#disable_openapi_validation}
         '''
         result = self._values.get("disable_openapi_validation")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def disable_webhooks(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Prevent hooks from running.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#disable_webhooks Release#disable_webhooks}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#disable_webhooks Release#disable_webhooks}
         '''
         result = self._values.get("disable_webhooks")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def force_update(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Force resource update through delete/recreate if needed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#force_update Release#force_update}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#force_update Release#force_update}
         '''
         result = self._values.get("force_update")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#id Release#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#id Release#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def keyring(self) -> typing.Optional[builtins.str]:
         '''Location of public keys used for verification. Used only if ``verify`` is true.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#keyring Release#keyring}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#keyring Release#keyring}
         '''
         result = self._values.get("keyring")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def lint(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Run helm lint when planning.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#lint Release#lint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#lint Release#lint}
         '''
         result = self._values.get("lint")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def max_history(self) -> typing.Optional[jsii.Number]:
         '''Limit the maximum number of revisions saved per release. Use 0 for no limit.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#max_history Release#max_history}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#max_history Release#max_history}
         '''
         result = self._values.get("max_history")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''Namespace to install the release into.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#namespace Release#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#namespace Release#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def pass_credentials(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Pass credentials to all domains.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#pass_credentials Release#pass_credentials}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#pass_credentials Release#pass_credentials}
         '''
         result = self._values.get("pass_credentials")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def postrender(self) -> typing.Optional["ReleasePostrender"]:
         '''postrender block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#postrender Release#postrender}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#postrender Release#postrender}
         '''
         result = self._values.get("postrender")
         return typing.cast(typing.Optional["ReleasePostrender"], result)
 
     @builtins.property
     def recreate_pods(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Perform pods restart during upgrade/rollback.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#recreate_pods Release#recreate_pods}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#recreate_pods Release#recreate_pods}
         '''
         result = self._values.get("recreate_pods")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def render_subchart_notes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, render subchart notes along with the parent.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#render_subchart_notes Release#render_subchart_notes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#render_subchart_notes Release#render_subchart_notes}
         '''
         result = self._values.get("render_subchart_notes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def replace(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Re-use the given name, even if that name is already used. This is unsafe in production.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#replace Release#replace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#replace Release#replace}
         '''
         result = self._values.get("replace")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def repository(self) -> typing.Optional[builtins.str]:
         '''Repository where to locate the requested chart. If is a URL the chart is installed without installing the repository.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository Release#repository}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository Release#repository}
         '''
         result = self._values.get("repository")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_ca_file(self) -> typing.Optional[builtins.str]:
         '''The Repositories CA File.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_ca_file Release#repository_ca_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_ca_file Release#repository_ca_file}
         '''
         result = self._values.get("repository_ca_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_cert_file(self) -> typing.Optional[builtins.str]:
         '''The repositories cert file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_cert_file Release#repository_cert_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_cert_file Release#repository_cert_file}
         '''
         result = self._values.get("repository_cert_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_key_file(self) -> typing.Optional[builtins.str]:
         '''The repositories cert key file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_key_file Release#repository_key_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_key_file Release#repository_key_file}
         '''
         result = self._values.get("repository_key_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_password(self) -> typing.Optional[builtins.str]:
         '''Password for HTTP basic authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_password Release#repository_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_password Release#repository_password}
         '''
         result = self._values.get("repository_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def repository_username(self) -> typing.Optional[builtins.str]:
         '''Username for HTTP basic authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#repository_username Release#repository_username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#repository_username Release#repository_username}
         '''
         result = self._values.get("repository_username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def reset_values(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When upgrading, reset the values to the ones built into the chart.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#reset_values Release#reset_values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#reset_values Release#reset_values}
         '''
         result = self._values.get("reset_values")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def reuse_values(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When upgrading, reuse the last release's values and merge in any overrides. If 'reset_values' is specified, this is ignored.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#reuse_values Release#reuse_values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#reuse_values Release#reuse_values}
         '''
         result = self._values.get("reuse_values")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def set(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSet"]]]:
         '''set block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#set Release#set}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set Release#set}
         '''
         result = self._values.get("set")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSet"]]], result)
 
     @builtins.property
+    def set_list(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetListStruct"]]]:
+        '''set_list block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set_list Release#set_list}
+        '''
+        result = self._values.get("set_list")
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetListStruct"]]], result)
+
+    @builtins.property
     def set_sensitive(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetSensitive"]]]:
         '''set_sensitive block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#set_sensitive Release#set_sensitive}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#set_sensitive Release#set_sensitive}
         '''
         result = self._values.get("set_sensitive")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ReleaseSetSensitive"]]], result)
 
     @builtins.property
     def skip_crds(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, no CRDs will be installed. By default, CRDs are installed if not already present.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#skip_crds Release#skip_crds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#skip_crds Release#skip_crds}
         '''
         result = self._values.get("skip_crds")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def timeout(self) -> typing.Optional[jsii.Number]:
         '''Time in seconds to wait for any individual kubernetes operation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#timeout Release#timeout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#timeout Release#timeout}
         '''
         result = self._values.get("timeout")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def values(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of values in raw yaml format to pass to helm.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#values Release#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#values Release#values}
         '''
         result = self._values.get("values")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def verify(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Verify the package before installing it.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#verify Release#verify}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#verify Release#verify}
         '''
         result = self._values.get("verify")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def version(self) -> typing.Optional[builtins.str]:
         '''Specify the exact chart version to install. If this is not specified, the latest version is installed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#version Release#version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#version Release#version}
         '''
         result = self._values.get("version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def wait(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Will wait until all resources are in a ready state before marking the release as successful.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#wait Release#wait}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#wait Release#wait}
         '''
         result = self._values.get("wait")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def wait_for_jobs(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If wait is enabled, will wait until all Jobs have been completed before marking the release as successful.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#wait_for_jobs Release#wait_for_jobs}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#wait_for_jobs Release#wait_for_jobs}
         '''
         result = self._values.get("wait_for_jobs")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2109,16 +2158,16 @@
     def __init__(
         self,
         *,
         binary_path: builtins.str,
         args: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#binary_path Release#binary_path}
-        :param args: an argument to the post-renderer (can specify multiple). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#args Release#args}
+        :param binary_path: The command binary path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#binary_path Release#binary_path}
+        :param args: an argument to the post-renderer (can specify multiple). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#args Release#args}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__981056baac01e08a9be241caf4b8905301446900d1d7eecfc096ec7c50fd4c55)
             check_type(argname="argument binary_path", value=binary_path, expected_type=type_hints["binary_path"])
             check_type(argname="argument args", value=args, expected_type=type_hints["args"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "binary_path": binary_path,
@@ -2126,25 +2175,25 @@
         if args is not None:
             self._values["args"] = args
 
     @builtins.property
     def binary_path(self) -> builtins.str:
         '''The command binary path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#binary_path Release#binary_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#binary_path Release#binary_path}
         '''
         result = self._values.get("binary_path")
         assert result is not None, "Required property 'binary_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def args(self) -> typing.Optional[typing.List[builtins.str]]:
         '''an argument to the post-renderer (can specify multiple).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#args Release#args}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#args Release#args}
         '''
         result = self._values.get("args")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2238,17 +2287,17 @@
         self,
         *,
         name: builtins.str,
         value: builtins.str,
         type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#name Release#name}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#value Release#value}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#type Release#type}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#value Release#value}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#type Release#type}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b40ee13479cae3240c1ba06fd537a3e15ab3fbca99f29411b2d968f452c5a980)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -2256,29 +2305,29 @@
             "value": value,
         }
         if type is not None:
             self._values["type"] = type
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#name Release#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#value Release#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#value Release#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#type Release#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#type Release#type}.'''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -2376,14 +2425,233 @@
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f9ca85907af9cf85a8ac2dc36272b5268e80c3a54e28b189fccbbaaa77e83094)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
+@jsii.data_type(
+    jsii_type="@cdktf/provider-helm.release.ReleaseSetListStruct",
+    jsii_struct_bases=[],
+    name_mapping={"name": "name", "value": "value"},
+)
+class ReleaseSetListStruct:
+    def __init__(
+        self,
+        *,
+        name: builtins.str,
+        value: typing.Sequence[builtins.str],
+    ) -> None:
+        '''
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#value Release#value}.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__508f3584f37548827519997a7378963046271d485d0bb70d9ba0ee49230f97b1)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+            "value": value,
+        }
+
+    @builtins.property
+    def name(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}.'''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def value(self) -> typing.List[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#value Release#value}.'''
+        result = self._values.get("value")
+        assert result is not None, "Required property 'value' is missing"
+        return typing.cast(typing.List[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "ReleaseSetListStruct(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class ReleaseSetListStructList(
+    _cdktf_9a9027ec.ComplexList,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-helm.release.ReleaseSetListStructList",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        wraps_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__506e3c4fb8d423f7c946de19016f6ebc30c1bcbb7a3ded0e9273d68545fb1dc9)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
+
+    @jsii.member(jsii_name="get")
+    def get(self, index: jsii.Number) -> "ReleaseSetListStructOutputReference":
+        '''
+        :param index: the index of the item to return.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ebea825e6d9857a5a200e3a0a0a0a7f402755c1a9a6f74cce00614feee2edb9f)
+            check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+        return typing.cast("ReleaseSetListStructOutputReference", jsii.invoke(self, "get", [index]))
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformAttribute")
+    def _terraform_attribute(self) -> builtins.str:
+        '''The attribute on the parent resource this class is referencing.'''
+        return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
+
+    @_terraform_attribute.setter
+    def _terraform_attribute(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__650b5d025108ec67ac17015a5be61baa8e0d1d9fd908dbd015d5a0eeb2701e73)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformAttribute", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformResource")
+    def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
+        '''The parent resource.'''
+        return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
+
+    @_terraform_resource.setter
+    def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8ef07a70eee43811f80dae9728021bec9ea4a82e9ea6d05537fba481ed607312)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformResource", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="wrapsSet")
+    def _wraps_set(self) -> builtins.bool:
+        '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
+        return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
+
+    @_wraps_set.setter
+    def _wraps_set(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__60909616a85d34562129544b26e7f3be6d889d64839017ec3d2d5ed9439a7f1a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "wrapsSet", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[ReleaseSetListStruct]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[ReleaseSetListStruct]]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[ReleaseSetListStruct]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9bcca7dc69fbd34bba0bdcfe01d96ba624825aa38bb09e9a24ad6bf77dcaa295)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
+class ReleaseSetListStructOutputReference(
+    _cdktf_9a9027ec.ComplexObject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-helm.release.ReleaseSetListStructOutputReference",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        complex_object_index: jsii.Number,
+        complex_object_is_from_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param complex_object_index: the index of this item in the list.
+        :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a9da10675f069e7d164482711958df693111957ebaa0a5569aff52837d57081e)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
+            check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
+
+    @builtins.property
+    @jsii.member(jsii_name="nameInput")
+    def name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="valueInput")
+    def value_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "valueInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "name"))
+
+    @name.setter
+    def name(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__288d802b0cacbddb2d07c7b72ccf95eb794c3b5f1da482f47cc28254afbd0f0b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "name", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="value")
+    def value(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "value"))
+
+    @value.setter
+    def value(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__28cd18e83dfef4ac26bd1113e6537cf2469ca874f77954d24c1523bb828f497e)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "value", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[ReleaseSetListStruct, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[ReleaseSetListStruct, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[ReleaseSetListStruct, _cdktf_9a9027ec.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__350fa01806e21d206a65b4e7cebe986132bd002ae3ab7d01a7a6e03343183688)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
 class ReleaseSetOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-helm.release.ReleaseSetOutputReference",
 ):
     def __init__(
         self,
@@ -2489,17 +2757,17 @@
         self,
         *,
         name: builtins.str,
         value: builtins.str,
         type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#name Release#name}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#value Release#value}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#type Release#type}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#value Release#value}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#type Release#type}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__819e69b309674d2d9b39573b21155edba86166772433bfb823f741b56247a94e)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -2507,29 +2775,29 @@
             "value": value,
         }
         if type is not None:
             self._values["type"] = type
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#name Release#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#name Release#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#value Release#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#value Release#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.9.0/docs/resources/release#type Release#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/helm/2.10.0/docs/resources/release#type Release#type}.'''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -2736,14 +3004,17 @@
     "ReleaseMetadata",
     "ReleaseMetadataList",
     "ReleaseMetadataOutputReference",
     "ReleasePostrender",
     "ReleasePostrenderOutputReference",
     "ReleaseSet",
     "ReleaseSetList",
+    "ReleaseSetListStruct",
+    "ReleaseSetListStructList",
+    "ReleaseSetListStructOutputReference",
     "ReleaseSetOutputReference",
     "ReleaseSetSensitive",
     "ReleaseSetSensitiveList",
     "ReleaseSetSensitiveOutputReference",
 ]
 
 publication.publish()
@@ -2779,14 +3050,15 @@
     repository_cert_file: typing.Optional[builtins.str] = None,
     repository_key_file: typing.Optional[builtins.str] = None,
     repository_password: typing.Optional[builtins.str] = None,
     repository_username: typing.Optional[builtins.str] = None,
     reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSet, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSetListStruct, typing.Dict[builtins.str, typing.Any]]]]] = None,
     set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSetSensitive, typing.Dict[builtins.str, typing.Any]]]]] = None,
     skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     timeout: typing.Optional[jsii.Number] = None,
     values: typing.Optional[typing.Sequence[builtins.str]] = None,
     verify: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     version: typing.Optional[builtins.str] = None,
     wait: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -2804,14 +3076,20 @@
 
 def _typecheckingstub__6b72a3657c0803010731fa3fd2044a0f404b98ac9399b1fb916895c0de83919d(
     value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSet, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__64e66f987c47878d4a6946a5a1dc06f0d9f1ca6ba2ae98348676c4bd5950c185(
+    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSetListStruct, typing.Dict[builtins.str, typing.Any]]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__aaf9382a783d49a3885b1e5db3d0b63f63fc7a33b8cdeefbeace8a470ca85b20(
     value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSetSensitive, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__b64d1ea2d4d5c0481d8d2a15fc4f143dbdef8ab41305fc11564450cdd45168cd(
@@ -3066,14 +3344,15 @@
     repository_cert_file: typing.Optional[builtins.str] = None,
     repository_key_file: typing.Optional[builtins.str] = None,
     repository_password: typing.Optional[builtins.str] = None,
     repository_username: typing.Optional[builtins.str] = None,
     reset_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     reuse_values: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     set: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSet, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    set_list: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSetListStruct, typing.Dict[builtins.str, typing.Any]]]]] = None,
     set_sensitive: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ReleaseSetSensitive, typing.Dict[builtins.str, typing.Any]]]]] = None,
     skip_crds: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     timeout: typing.Optional[jsii.Number] = None,
     values: typing.Optional[typing.Sequence[builtins.str]] = None,
     verify: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     version: typing.Optional[builtins.str] = None,
     wait: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -3205,14 +3484,87 @@
 
 def _typecheckingstub__f9ca85907af9cf85a8ac2dc36272b5268e80c3a54e28b189fccbbaaa77e83094(
     value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[ReleaseSet]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__508f3584f37548827519997a7378963046271d485d0bb70d9ba0ee49230f97b1(
+    *,
+    name: builtins.str,
+    value: typing.Sequence[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__506e3c4fb8d423f7c946de19016f6ebc30c1bcbb7a3ded0e9273d68545fb1dc9(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    wraps_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ebea825e6d9857a5a200e3a0a0a0a7f402755c1a9a6f74cce00614feee2edb9f(
+    index: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__650b5d025108ec67ac17015a5be61baa8e0d1d9fd908dbd015d5a0eeb2701e73(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8ef07a70eee43811f80dae9728021bec9ea4a82e9ea6d05537fba481ed607312(
+    value: _cdktf_9a9027ec.IInterpolatingParent,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__60909616a85d34562129544b26e7f3be6d889d64839017ec3d2d5ed9439a7f1a(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9bcca7dc69fbd34bba0bdcfe01d96ba624825aa38bb09e9a24ad6bf77dcaa295(
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[ReleaseSetListStruct]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a9da10675f069e7d164482711958df693111957ebaa0a5569aff52837d57081e(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    complex_object_index: jsii.Number,
+    complex_object_is_from_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__288d802b0cacbddb2d07c7b72ccf95eb794c3b5f1da482f47cc28254afbd0f0b(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__28cd18e83dfef4ac26bd1113e6537cf2469ca874f77954d24c1523bb828f497e(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__350fa01806e21d206a65b4e7cebe986132bd002ae3ab7d01a7a6e03343183688(
+    value: typing.Optional[typing.Union[ReleaseSetListStruct, _cdktf_9a9027ec.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__c6efd1b4f4eb146a9e29807c430593a784d3e67a3ca29c40ed2b49dc8658eb55(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/PKG-INFO` & `cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-helm
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt helm Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-helm.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-helm.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform helm Provider version 1:1. In fact, it always tracks `latest` of `~> 2.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform helm Provider](https://github.com/terraform-providers/terraform-provider-helm)
+* [Terraform helm Provider](https://registry.terraform.io/providers/hashicorp/helm/2.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-helm/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-helm-6.0.0/src/cdktf_cdktf_provider_helm.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-helm-6.0.1/src/cdktf_cdktf_provider_helm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_helm/py.typed
 src/cdktf_cdktf_provider_helm.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_helm.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_helm.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_helm.egg-info/requires.txt
 src/cdktf_cdktf_provider_helm.egg-info/top_level.txt
 src/cdktf_cdktf_provider_helm/_jsii/__init__.py
-src/cdktf_cdktf_provider_helm/_jsii/provider-helm@6.0.0.jsii.tgz
+src/cdktf_cdktf_provider_helm/_jsii/provider-helm@6.0.1.jsii.tgz
 src/cdktf_cdktf_provider_helm/data_helm_template/__init__.py
 src/cdktf_cdktf_provider_helm/provider/__init__.py
 src/cdktf_cdktf_provider_helm/release/__init__.py
```

