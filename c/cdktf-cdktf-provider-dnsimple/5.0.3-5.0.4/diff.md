# Comparing `tmp/cdktf-cdktf-provider-dnsimple-5.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-dnsimple-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dnsimple-5.0.3.tar", last modified: Thu May 18 03:12:25 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dnsimple-5.0.4.tar", last modified: Thu Jun  1 14:15:08 2023, max compression
```

## Comparing `cdktf-cdktf-provider-dnsimple-5.0.3.tar` & `cdktf-cdktf-provider-dnsimple-5.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.320739 cdktf-cdktf-provider-dnsimple-5.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.320739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60139 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/contact/
--rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/domain_delegation/
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/ds_record/
--rw-r--r--   0 runner    (1001) docker     (123)    26171 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/email_forward/
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    26531 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/registered_domain/
--rw-r--r--   0 runner    (1001) docker     (123)    51885 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/zone_record/
--rw-r--r--   0 runner    (1001) docker     (123)    25241 2023-05-18 03:12:14.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:12:25.324739 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 03:12:25.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-18 03:12:25.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:12:25.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 03:12:25.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 03:12:25.000000 cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.755552 cdktf-cdktf-provider-dnsimple-5.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61243 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.4.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/contact/
+-rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/domain_delegation/
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/ds_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    26171 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/email_forward/
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    26531 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/registered_domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    51885 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/zone_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    25241 2023-06-01 14:14:57.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:15:08.759552 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-01 14:15:08.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-01 14:15:08.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:15:08.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:15:08.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 14:15:08.000000 cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/LICENSE` & `cdktf-cdktf-provider-dnsimple-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 5.0.3
+Version: 5.0.4
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/README.md` & `cdktf-cdktf-provider-dnsimple-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/setup.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dnsimple",
-    "version": "5.0.3",
+    "version": "5.0.4",
     "description": "Prebuilt dnsimple Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dnsimple.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -33,23 +33,23 @@
         "cdktf_cdktf_provider_dnsimple.lets_encrypt_certificate",
         "cdktf_cdktf_provider_dnsimple.provider",
         "cdktf_cdktf_provider_dnsimple.registered_domain",
         "cdktf_cdktf_provider_dnsimple.zone_record"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dnsimple._jsii": [
-            "provider-dnsimple@5.0.3.jsii.tgz"
+            "provider-dnsimple@5.0.4.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dnsimple": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.0, <0.17.0",
+        "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 5.0.3
+Version: 5.0.4
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dnsimple-5.0.4/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_dnsimple/py.typed
 src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
-src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.3.jsii.tgz
+src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.4.jsii.tgz
 src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
 src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
 src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
 src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
 src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
```

