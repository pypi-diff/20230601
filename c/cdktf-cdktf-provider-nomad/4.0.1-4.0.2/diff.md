# Comparing `tmp/cdktf-cdktf-provider-nomad-4.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-nomad-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-nomad-4.0.1.tar", last modified: Fri Apr 21 03:14:09 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-nomad-4.0.2.tar", last modified: Thu Jun  1 14:28:16 2023, max compression
```

## Comparing `cdktf-cdktf-provider-nomad-4.0.1.tar` & `cdktf-cdktf-provider-nomad-4.0.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.611124 cdktf-cdktf-provider-nomad-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.615124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1048926 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@4.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_auth_method/
--rw-r--r--   0 runner    (1001) docker     (123)    60883 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_auth_method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_binding_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    27753 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_binding_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_role/
--rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_token/
--rw-r--r--   0 runner    (1001) docker     (123)    44597 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/
--rw-r--r--   0 runner    (1001) docker     (123)    27317 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/
--rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/
--rw-r--r--   0 runner    (1001) docker     (123)    36354 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/
--rw-r--r--   0 runner    (1001) docker     (123)    28469 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/
--rw-r--r--   0 runner    (1001) docker     (123)    37347 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/
--rw-r--r--   0 runner    (1001) docker     (123)    21815 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/
--rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_job/
--rw-r--r--   0 runner    (1001) docker     (123)    79563 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/
--rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/
--rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    35246 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_regions/
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/
--rw-r--r--   0 runner    (1001) docker     (123)    30320 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/
--rw-r--r--   0 runner    (1001) docker     (123)    25257 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/external_volume/
--rw-r--r--   0 runner    (1001) docker     (123)   134051 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.623124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/job/
--rw-r--r--   0 runner    (1001) docker     (123)   103992 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/namespace/
--rw-r--r--   0 runner    (1001) docker     (123)    36650 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/namespace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    45066 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/quota_specification/
--rw-r--r--   0 runner    (1001) docker     (123)    45637 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/scheduler_config/
--rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/sentinel_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.627124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/volume/
--rw-r--r--   0 runner    (1001) docker     (123)   112384 2023-04-21 03:13:54.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:14:09.619124 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-21 03:14:09.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-21 03:14:09.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:14:09.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 03:14:09.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 03:14:09.000000 cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.118341 cdktf-cdktf-provider-nomad-4.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.122341 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   230514 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@4.0.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_auth_method/
+-rw-r--r--   0 runner    (1001) docker     (123)    60883 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_auth_method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_binding_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    27753 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_binding_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    44597 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)    27317 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)    36354 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    28469 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)    37347 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/
+-rw-r--r--   0 runner    (1001) docker     (123)    21815 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_job/
+-rw-r--r--   0 runner    (1001) docker     (123)    79563 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/
+-rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    35246 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_regions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)    30320 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)    25257 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/external_volume/
+-rw-r--r--   0 runner    (1001) docker     (123)   134051 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/job/
+-rw-r--r--   0 runner    (1001) docker     (123)   103992 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/namespace/
+-rw-r--r--   0 runner    (1001) docker     (123)    36650 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    45066 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/quota_specification/
+-rw-r--r--   0 runner    (1001) docker     (123)    45637 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/scheduler_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/sentinel_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.130342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)   112384 2023-06-01 14:28:01.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:28:16.126342 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-01 14:28:16.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-01 14:28:16.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:28:16.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:28:16.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 14:28:16.000000 cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/LICENSE` & `cdktf-cdktf-provider-nomad-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/PKG-INFO` & `cdktf-cdktf-provider-nomad-4.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-nomad
-Version: 4.0.1
+Version: 4.0.2
 Summary: Prebuilt nomad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-nomad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-nomad.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform nomad Provider](https://github.com/terraform-providers/terraform-provider-nomad)
+* [Terraform nomad Provider](https://registry.terraform.io/providers/hashicorp/nomad/1.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-nomad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/README.md` & `cdktf-cdktf-provider-nomad-4.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform nomad Provider](https://github.com/terraform-providers/terraform-provider-nomad)
+* [Terraform nomad Provider](https://registry.terraform.io/providers/hashicorp/nomad/1.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-nomad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/setup.py` & `cdktf-cdktf-provider-nomad-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-nomad",
-    "version": "4.0.1",
+    "version": "4.0.2",
     "description": "Prebuilt nomad Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-nomad.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -54,25 +54,25 @@
         "cdktf_cdktf_provider_nomad.quota_specification",
         "cdktf_cdktf_provider_nomad.scheduler_config",
         "cdktf_cdktf_provider_nomad.sentinel_policy",
         "cdktf_cdktf_provider_nomad.volume"
     ],
     "package_data": {
         "cdktf_cdktf_provider_nomad._jsii": [
-            "provider-nomad@4.0.1.jsii.tgz"
+            "provider-nomad@4.0.2.jsii.tgz"
         ],
         "cdktf_cdktf_provider_nomad": [
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

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform nomad Provider](https://github.com/terraform-providers/terraform-provider-nomad)
+* [Terraform nomad Provider](https://registry.terraform.io/providers/hashicorp/nomad/1.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-nomad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_auth_method/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_auth_method/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_binding_rule/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_binding_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/acl_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_acl_tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_datacenters/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_job_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_namespace/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_regions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scaling_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_scheduler_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/data_nomad_volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/external_volume/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/job/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/namespace/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/namespace/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/provider/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/quota_specification/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/scheduler_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/sentinel_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad/volume/__init__.py` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-nomad
-Version: 4.0.1
+Version: 4.0.2
 Summary: Prebuilt nomad Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-nomad.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-nomad.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform nomad Provider version 1:1. In fact, it always tracks `latest` of `~> 1.4` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform nomad Provider](https://github.com/terraform-providers/terraform-provider-nomad)
+* [Terraform nomad Provider](https://registry.terraform.io/providers/hashicorp/nomad/1.4.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-nomad/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-nomad-4.0.1/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-nomad-4.0.2/src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_nomad/py.typed
 src/cdktf_cdktf_provider_nomad.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_nomad.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_nomad.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_nomad.egg-info/requires.txt
 src/cdktf_cdktf_provider_nomad.egg-info/top_level.txt
 src/cdktf_cdktf_provider_nomad/_jsii/__init__.py
-src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@4.0.1.jsii.tgz
+src/cdktf_cdktf_provider_nomad/_jsii/provider-nomad@4.0.2.jsii.tgz
 src/cdktf_cdktf_provider_nomad/acl_auth_method/__init__.py
 src/cdktf_cdktf_provider_nomad/acl_binding_rule/__init__.py
 src/cdktf_cdktf_provider_nomad/acl_policy/__init__.py
 src/cdktf_cdktf_provider_nomad/acl_role/__init__.py
 src/cdktf_cdktf_provider_nomad/acl_token/__init__.py
 src/cdktf_cdktf_provider_nomad/data_nomad_acl_policies/__init__.py
 src/cdktf_cdktf_provider_nomad/data_nomad_acl_policy/__init__.py
```

