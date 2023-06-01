# Comparing `tmp/cdktf-cdktf-provider-ad-4.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-ad-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-ad-4.0.0.tar", last modified: Tue Apr 18 20:33:40 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-ad-4.0.1.tar", last modified: Thu Jun  1 14:11:05 2023, max compression
```

## Comparing `cdktf-cdktf-provider-ad-4.0.0.tar` & `cdktf-cdktf-provider-ad-4.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:33:40.084511 cdktf-cdktf-provider-ad-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   494225 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/_jsii/provider-ad@4.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/computer/
--rw-r--r--   0 runner    (1001) docker     (123)    25621 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/computer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/
--rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/
--rw-r--r--   0 runner    (1001) docker     (123)    19386 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/
--rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gplink/
--rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gplink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo/
--rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo_security/
--rw-r--r--   0 runner    (1001) docker     (123)   261974 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group/
--rw-r--r--   0 runner    (1001) docker     (123)    29539 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group_membership/
--rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group_membership/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/ou/
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/ou/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.080511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/user/
--rw-r--r--   0 runner    (1001) docker     (123)   119114 2023-04-18 20:33:27.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:33:40.076511 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 20:33:40.000000 cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.386195 cdktf-cdktf-provider-ad-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130637 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/_jsii/provider-ad@4.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/computer/
+-rw-r--r--   0 runner    (1001) docker     (123)    25621 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/computer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_computer/
+-rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_gpo/
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    19386 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_ou/
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gplink/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gplink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gpo/
+-rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gpo_security/
+-rw-r--r--   0 runner    (1001) docker     (123)   261974 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/group/
+-rw-r--r--   0 runner    (1001) docker     (123)    29539 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/group_membership/
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/group_membership/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/ou/
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/ou/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.394195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/user/
+-rw-r--r--   0 runner    (1001) docker     (123)   119114 2023-06-01 14:10:49.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:05.390195 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-01 14:11:05.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 14:11:05.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:11:05.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:11:05.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 14:11:05.000000 cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-ad-4.0.0/LICENSE` & `cdktf-cdktf-provider-ad-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/PKG-INFO` & `cdktf-cdktf-provider-ad-4.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-ad
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt ad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-ad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-ad.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform ad Provider](https://github.com/terraform-providers/terraform-provider-ad)
+* [Terraform ad Provider](https://registry.terraform.io/providers/hashicorp/ad/0.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-ad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-ad-4.0.0/README.md` & `cdktf-cdktf-provider-ad-4.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform ad Provider](https://github.com/terraform-providers/terraform-provider-ad)
+* [Terraform ad Provider](https://registry.terraform.io/providers/hashicorp/ad/0.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-ad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-ad-4.0.0/setup.py` & `cdktf-cdktf-provider-ad-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-ad",
-    "version": "4.0.0",
+    "version": "4.0.1",
     "description": "Prebuilt ad Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-ad.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -36,25 +36,25 @@
         "cdktf_cdktf_provider_ad.group_membership",
         "cdktf_cdktf_provider_ad.ou",
         "cdktf_cdktf_provider_ad.provider",
         "cdktf_cdktf_provider_ad.user"
     ],
     "package_data": {
         "cdktf_cdktf_provider_ad._jsii": [
-            "provider-ad@4.0.0.jsii.tgz"
+            "provider-ad@4.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_ad": [
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

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform ad Provider](https://github.com/terraform-providers/terraform-provider-ad)
+* [Terraform ad Provider](https://registry.terraform.io/providers/hashicorp/ad/0.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-ad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/computer/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gplink/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gplink/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gpo/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/gpo_security/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/group_membership/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/group_membership/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/ou/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/ou/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/provider/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad/user/__init__.py` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-ad
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt ad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-ad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-ad.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform ad Provider version 1:1. In fact, it always tracks `latest` of `~> 0.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform ad Provider](https://github.com/terraform-providers/terraform-provider-ad)
+* [Terraform ad Provider](https://registry.terraform.io/providers/hashicorp/ad/0.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-ad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-ad-4.0.0/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-ad-4.0.1/src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_ad/py.typed
 src/cdktf_cdktf_provider_ad.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_ad.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_ad.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_ad.egg-info/requires.txt
 src/cdktf_cdktf_provider_ad.egg-info/top_level.txt
 src/cdktf_cdktf_provider_ad/_jsii/__init__.py
-src/cdktf_cdktf_provider_ad/_jsii/provider-ad@4.0.0.jsii.tgz
+src/cdktf_cdktf_provider_ad/_jsii/provider-ad@4.0.1.jsii.tgz
 src/cdktf_cdktf_provider_ad/computer/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_computer/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_gpo/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_group/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_ou/__init__.py
 src/cdktf_cdktf_provider_ad/data_ad_user/__init__.py
 src/cdktf_cdktf_provider_ad/gplink/__init__.py
```

