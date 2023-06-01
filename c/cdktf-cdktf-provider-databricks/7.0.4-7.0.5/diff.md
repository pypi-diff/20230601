# Comparing `tmp/cdktf-cdktf-provider-databricks-7.0.4.tar.gz` & `tmp/cdktf-cdktf-provider-databricks-7.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-databricks-7.0.4.tar", last modified: Tue May 23 03:20:37 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-databricks-7.0.5.tar", last modified: Thu Jun  1 14:18:31 2023, max compression
```

## Comparing `cdktf-cdktf-provider-databricks-7.0.4.tar` & `cdktf-cdktf-provider-databricks-7.0.5.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.321760 cdktf-cdktf-provider-databricks-7.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-23 03:20:37.321760 cdktf-cdktf-provider-databricks-7.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 03:20:37.321760 cdktf-cdktf-provider-databricks-7.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.281759 cdktf-cdktf-provider-databricks-7.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.289759 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1467105 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@7.0.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/aws_s3_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    25103 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    37192 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    39923 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_blob_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    34286 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    37205 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   374730 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/cluster_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    31179 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    26627 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   405001 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/
--rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/
--rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/
--rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_directory/
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_group/
--rw-r--r--   0 runner    (1001) docker     (123)    52152 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/
--rw-r--r--   0 runner    (1001) docker     (123)   214292 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.297760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_job/
--rw-r--r--   0 runner    (1001) docker     (123)  1614530 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    18514 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/
--rw-r--r--   0 runner    (1001) docker     (123)    52603 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/
--rw-r--r--   0 runner    (1001) docker     (123)    30210 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/
--rw-r--r--   0 runner    (1001) docker     (123)    21674 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_share/
--rw-r--r--   0 runner    (1001) docker     (123)    91706 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_shares/
--rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/
--rw-r--r--   0 runner    (1001) docker     (123)    43822 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/
--rw-r--r--   0 runner    (1001) docker     (123)    98211 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/
--rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_tables/
--rw-r--r--   0 runner    (1001) docker     (123)    22429 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.301760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_user/
--rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_views/
--rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_zones/
--rw-r--r--   0 runner    (1001) docker     (123)    16121 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/dbfs_file/
--rw-r--r--   0 runner    (1001) docker     (123)    24655 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/directory/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/entitlements/
--rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/external_location/
--rw-r--r--   0 runner    (1001) docker     (123)    32095 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/external_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/git_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    25909 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/global_init_script/
--rw-r--r--   0 runner    (1001) docker     (123)    35510 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/grants/
--rw-r--r--   0 runner    (1001) docker     (123)    55461 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/grants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group/
--rw-r--r--   0 runner    (1001) docker     (123)    38035 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_role/
--rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/instance_pool/
--rw-r--r--   0 runner    (1001) docker     (123)   171446 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    27316 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/ip_access_list/
--rw-r--r--   0 runner    (1001) docker     (123)    24956 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.305760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/job/
--rw-r--r--   0 runner    (1001) docker     (123)  1494749 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/library/
--rw-r--r--   0 runner    (1001) docker     (123)    54504 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore/
--rw-r--r--   0 runner    (1001) docker     (123)    53817 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore_data_access/
--rw-r--r--   0 runner    (1001) docker     (123)    79505 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_experiment/
--rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_model/
--rw-r--r--   0 runner    (1001) docker     (123)    47009 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_webhook/
--rw-r--r--   0 runner    (1001) docker     (123)    53025 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/model_serving/
--rw-r--r--   0 runner    (1001) docker     (123)    81585 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mount/
--rw-r--r--   0 runner    (1001) docker     (123)   121729 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    22803 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/
--rw-r--r--   0 runner    (1001) docker     (123)    46981 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_log_delivery/
--rw-r--r--   0 runner    (1001) docker     (123)    42349 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.309760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_networks/
--rw-r--r--   0 runner    (1001) docker     (123)    85166 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    22828 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    37950 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)   148773 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)    33598 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/obo_token/
--rw-r--r--   0 runner    (1001) docker     (123)    22810 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/permission_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    89543 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)   340923 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    75645 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/provider_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/recipient/
--rw-r--r--   0 runner    (1001) docker     (123)    64355 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/recipient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/repo/
--rw-r--r--   0 runner    (1001) docker     (123)    36402 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret/
--rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret_acl/
--rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret_scope/
--rw-r--r--   0 runner    (1001) docker     (123)    33202 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.313760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    53372 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal_role/
--rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/share/
--rw-r--r--   0 runner    (1001) docker     (123)    89048 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/share/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_alert/
--rw-r--r--   0 runner    (1001) docker     (123)    42260 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    22195 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)   105173 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_global_config/
--rw-r--r--   0 runner    (1001) docker     (123)    30740 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    52298 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_query/
--rw-r--r--   0 runner    (1001) docker     (123)   223497 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_table/
--rw-r--r--   0 runner    (1001) docker     (123)    62781 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_visualization/
--rw-r--r--   0 runner    (1001) docker     (123)    31228 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_widget/
--rw-r--r--   0 runner    (1001) docker     (123)    70645 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/storage_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    78009 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/table/
--rw-r--r--   0 runner    (1001) docker     (123)    75587 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/token/
--rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user/
--rw-r--r--   0 runner    (1001) docker     (123)    51683 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user_instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user_role/
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/workspace_conf/
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.317760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/workspace_file/
--rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-05-23 03:20:21.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:20:37.293760 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-23 03:20:37.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-23 03:20:37.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:20:37.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 03:20:37.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 03:20:37.000000 cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.429785 cdktf-cdktf-provider-databricks-7.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-01 14:18:31.429785 cdktf-cdktf-provider-databricks-7.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:18:31.429785 cdktf-cdktf-provider-databricks-7.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.357785 cdktf-cdktf-provider-databricks-7.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.365785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.365785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1475816 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@7.0.5.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/aws_s3_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    25103 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    37192 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    39923 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_blob_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    34286 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    37205 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   374730 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/cluster_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    31179 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26627 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   405001 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    52152 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.369785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)   214292 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_job/
+-rw-r--r--   0 runner    (1001) docker     (123)  1614530 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    18514 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    52603 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/
+-rw-r--r--   0 runner    (1001) docker     (123)    21674 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.373785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_share/
+-rw-r--r--   0 runner    (1001) docker     (123)    91706 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.381785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_shares/
+-rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.381785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    43822 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    98211 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/
+-rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    22429 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_views/
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_zones/
+-rw-r--r--   0 runner    (1001) docker     (123)    16121 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/dbfs_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    24655 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/entitlements/
+-rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/external_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    32095 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/external_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/git_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    25909 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/global_init_script/
+-rw-r--r--   0 runner    (1001) docker     (123)    35510 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/grants/
+-rw-r--r--   0 runner    (1001) docker     (123)    55461 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/grants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group/
+-rw-r--r--   0 runner    (1001) docker     (123)    38035 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/instance_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)   171446 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    27316 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/ip_access_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    24956 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.385785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/job/
+-rw-r--r--   0 runner    (1001) docker     (123)  1494749 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/library/
+-rw-r--r--   0 runner    (1001) docker     (123)    54504 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore/
+-rw-r--r--   0 runner    (1001) docker     (123)    53817 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore_data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)    79505 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_model/
+-rw-r--r--   0 runner    (1001) docker     (123)    47009 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)    53025 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/model_serving/
+-rw-r--r--   0 runner    (1001) docker     (123)    81585 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)   121729 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    22803 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)    46981 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_log_delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)    42349 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)    85166 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    22828 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    37950 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)   148773 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.389785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)    33598 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/obo_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    22810 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/permission_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    89543 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)   340923 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    75645 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/provider_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/recipient/
+-rw-r--r--   0 runner    (1001) docker     (123)    64516 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/recipient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)    36402 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret_acl/
+-rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret_scope/
+-rw-r--r--   0 runner    (1001) docker     (123)    33202 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    53372 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/share/
+-rw-r--r--   0 runner    (1001) docker     (123)    89048 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/share/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_alert/
+-rw-r--r--   0 runner    (1001) docker     (123)    42260 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    22195 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)   105173 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_global_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    30740 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    52298 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_query/
+-rw-r--r--   0 runner    (1001) docker     (123)   223497 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.393785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_table/
+-rw-r--r--   0 runner    (1001) docker     (123)    62781 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.397785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    31228 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.397785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)    70645 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.397785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/storage_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    78009 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.397785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/table/
+-rw-r--r--   0 runner    (1001) docker     (123)    75587 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.397785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/token/
+-rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.397785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    51683 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.397785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user_instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.429785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.429785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/workspace_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.429785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/workspace_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-06-01 14:18:17.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:18:31.365785 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-01 14:18:31.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-01 14:18:31.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:18:31.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:18:31.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 14:18:31.000000 cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/LICENSE` & `cdktf-cdktf-provider-databricks-7.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/PKG-INFO` & `cdktf-cdktf-provider-databricks-7.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-databricks
-Version: 7.0.4
+Version: 7.0.5
 Summary: Prebuilt databricks Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-databricks.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-databricks.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/README.md` & `cdktf-cdktf-provider-databricks-7.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/setup.py` & `cdktf-cdktf-provider-databricks-7.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-databricks",
-    "version": "7.0.4",
+    "version": "7.0.5",
     "description": "Prebuilt databricks Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-databricks.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -129,23 +129,23 @@
         "cdktf_cdktf_provider_databricks.user_instance_profile",
         "cdktf_cdktf_provider_databricks.user_role",
         "cdktf_cdktf_provider_databricks.workspace_conf",
         "cdktf_cdktf_provider_databricks.workspace_file"
     ],
     "package_data": {
         "cdktf_cdktf_provider_databricks._jsii": [
-            "provider-databricks@7.0.4.jsii.tgz"
+            "provider-databricks@7.0.5.jsii.tgz"
         ],
         "cdktf_cdktf_provider_databricks": [
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

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/catalog/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/cluster/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
     @jsii.member(jsii_name="pathList")
-    def path_list(self) -> "DataDatabricksDbfsFilePathsPathListList":
-        return typing.cast("DataDatabricksDbfsFilePathsPathListList", jsii.get(self, "pathList"))
+    def path_list(self) -> "DataDatabricksDbfsFilePathsPathListStructList":
+        return typing.cast("DataDatabricksDbfsFilePathsPathListStructList", jsii.get(self, "pathList"))
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
@@ -328,114 +328,114 @@
     def __repr__(self) -> str:
         return "DataDatabricksDbfsFilePathsConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-databricks.dataDatabricksDbfsFilePaths.DataDatabricksDbfsFilePathsPathList",
+    jsii_type="@cdktf/provider-databricks.dataDatabricksDbfsFilePaths.DataDatabricksDbfsFilePathsPathListStruct",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataDatabricksDbfsFilePathsPathList:
+class DataDatabricksDbfsFilePathsPathListStruct:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataDatabricksDbfsFilePathsPathList(%s)" % ", ".join(
+        return "DataDatabricksDbfsFilePathsPathListStruct(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataDatabricksDbfsFilePathsPathListList(
+class DataDatabricksDbfsFilePathsPathListStructList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-databricks.dataDatabricksDbfsFilePaths.DataDatabricksDbfsFilePathsPathListList",
+    jsii_type="@cdktf/provider-databricks.dataDatabricksDbfsFilePaths.DataDatabricksDbfsFilePathsPathListStructList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9085a58784d73cb90deba730012a4eee5dda1d86fe02c168d9a6ad09a325efa3)
+            type_hints = typing.get_type_hints(_typecheckingstub__812fca952cdb6e2216e1d84ca6a3b5aa4ba4049a67a535049062506a05ebdcff)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataDatabricksDbfsFilePathsPathListOutputReference":
+    ) -> "DataDatabricksDbfsFilePathsPathListStructOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a2b77a4a43f5b14d0922103ae6bf166c20f24fa661fbdcd5f3467267d9b6a289)
+            type_hints = typing.get_type_hints(_typecheckingstub__796189e5455a643784054dc479343d1c189e03c51d81e61f2bdb026d0ea258ca)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataDatabricksDbfsFilePathsPathListOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataDatabricksDbfsFilePathsPathListStructOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2fbb99d5f8ce6811d23b6802c0c64132ecbc548e49dbe2cfa1868a9ec4d41a03)
+            type_hints = typing.get_type_hints(_typecheckingstub__1d17a848852392aae34d6e5ed88e99c12fe7fa7a79ffc27b18c47cb602fb3dc5)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7958ca776069952a509348993ac2d0e274c8d2ceb8c4e6ff37aaefc2ee803ee6)
+            type_hints = typing.get_type_hints(_typecheckingstub__948824b9a604ec333985834d6678979f6f8473b167a3a2eb89170f5003e04880)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__047e0f4712ae468da9088f7ffdb9b7f0c566fa70aa96f7661153c7f47e82761d)
+            type_hints = typing.get_type_hints(_typecheckingstub__743fe1b35164f563d5558ce02341e463ea18723b0562bab13587b39a6cfcc65e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataDatabricksDbfsFilePathsPathListOutputReference(
+class DataDatabricksDbfsFilePathsPathListStructOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-databricks.dataDatabricksDbfsFilePaths.DataDatabricksDbfsFilePathsPathListOutputReference",
+    jsii_type="@cdktf/provider-databricks.dataDatabricksDbfsFilePaths.DataDatabricksDbfsFilePathsPathListStructOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -443,15 +443,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1f094cc1dc68f8d538ef94650316ecfabe6a75702d76bf3d9c6cf487f810c19b)
+            type_hints = typing.get_type_hints(_typecheckingstub__a5b981bec20b00f7774b8a8b40ad9f943cd9bc86d97b4cb43fe7a9b7cc2898be)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -462,34 +462,36 @@
     @builtins.property
     @jsii.member(jsii_name="path")
     def path(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "path"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataDatabricksDbfsFilePathsPathList]:
-        return typing.cast(typing.Optional[DataDatabricksDbfsFilePathsPathList], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataDatabricksDbfsFilePathsPathListStruct]:
+        return typing.cast(typing.Optional[DataDatabricksDbfsFilePathsPathListStruct], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataDatabricksDbfsFilePathsPathList],
+        value: typing.Optional[DataDatabricksDbfsFilePathsPathListStruct],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5aa00994c2c54f9f752b19c34a9d79cd6ed726441cfd4742bde66bbf100c848e)
+            type_hints = typing.get_type_hints(_typecheckingstub__8c13d29fbdf52897e7f6094bc1a18cbb8a114db1eaf7fad8783000233ec06d12)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
     "DataDatabricksDbfsFilePaths",
     "DataDatabricksDbfsFilePathsConfig",
-    "DataDatabricksDbfsFilePathsPathList",
-    "DataDatabricksDbfsFilePathsPathListList",
-    "DataDatabricksDbfsFilePathsPathListOutputReference",
+    "DataDatabricksDbfsFilePathsPathListStruct",
+    "DataDatabricksDbfsFilePathsPathListStructList",
+    "DataDatabricksDbfsFilePathsPathListStructOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__d88087ceb6c030269b44c1cfdd8bb1ab860f7d30b9221e5008c265ad4af5b66d(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
@@ -538,53 +540,53 @@
     path: builtins.str,
     recursive: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__9085a58784d73cb90deba730012a4eee5dda1d86fe02c168d9a6ad09a325efa3(
+def _typecheckingstub__812fca952cdb6e2216e1d84ca6a3b5aa4ba4049a67a535049062506a05ebdcff(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a2b77a4a43f5b14d0922103ae6bf166c20f24fa661fbdcd5f3467267d9b6a289(
+def _typecheckingstub__796189e5455a643784054dc479343d1c189e03c51d81e61f2bdb026d0ea258ca(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__2fbb99d5f8ce6811d23b6802c0c64132ecbc548e49dbe2cfa1868a9ec4d41a03(
+def _typecheckingstub__1d17a848852392aae34d6e5ed88e99c12fe7fa7a79ffc27b18c47cb602fb3dc5(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7958ca776069952a509348993ac2d0e274c8d2ceb8c4e6ff37aaefc2ee803ee6(
+def _typecheckingstub__948824b9a604ec333985834d6678979f6f8473b167a3a2eb89170f5003e04880(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__047e0f4712ae468da9088f7ffdb9b7f0c566fa70aa96f7661153c7f47e82761d(
+def _typecheckingstub__743fe1b35164f563d5558ce02341e463ea18723b0562bab13587b39a6cfcc65e(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1f094cc1dc68f8d538ef94650316ecfabe6a75702d76bf3d9c6cf487f810c19b(
+def _typecheckingstub__a5b981bec20b00f7774b8a8b40ad9f943cd9bc86d97b4cb43fe7a9b7cc2898be(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__5aa00994c2c54f9f752b19c34a9d79cd6ed726441cfd4742bde66bbf100c848e(
-    value: typing.Optional[DataDatabricksDbfsFilePathsPathList],
+def _typecheckingstub__8c13d29fbdf52897e7f6094bc1a18cbb8a114db1eaf7fad8783000233ec06d12(
+    value: typing.Optional[DataDatabricksDbfsFilePathsPathListStruct],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,18 @@
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
     @jsii.member(jsii_name="notebookPathList")
-    def notebook_path_list(self) -> "DataDatabricksNotebookPathsNotebookPathListList":
-        return typing.cast("DataDatabricksNotebookPathsNotebookPathListList", jsii.get(self, "notebookPathList"))
+    def notebook_path_list(
+        self,
+    ) -> "DataDatabricksNotebookPathsNotebookPathListStructList":
+        return typing.cast("DataDatabricksNotebookPathsNotebookPathListStructList", jsii.get(self, "notebookPathList"))
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
@@ -328,114 +330,114 @@
     def __repr__(self) -> str:
         return "DataDatabricksNotebookPathsConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-databricks.dataDatabricksNotebookPaths.DataDatabricksNotebookPathsNotebookPathList",
+    jsii_type="@cdktf/provider-databricks.dataDatabricksNotebookPaths.DataDatabricksNotebookPathsNotebookPathListStruct",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataDatabricksNotebookPathsNotebookPathList:
+class DataDatabricksNotebookPathsNotebookPathListStruct:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataDatabricksNotebookPathsNotebookPathList(%s)" % ", ".join(
+        return "DataDatabricksNotebookPathsNotebookPathListStruct(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataDatabricksNotebookPathsNotebookPathListList(
+class DataDatabricksNotebookPathsNotebookPathListStructList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-databricks.dataDatabricksNotebookPaths.DataDatabricksNotebookPathsNotebookPathListList",
+    jsii_type="@cdktf/provider-databricks.dataDatabricksNotebookPaths.DataDatabricksNotebookPathsNotebookPathListStructList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__06b4ad130af3027668e27055473da95e25213246992760b84260622de7428e02)
+            type_hints = typing.get_type_hints(_typecheckingstub__2a12cf9e99ed6468683966e02ed51ba30f43062b8ad5a877bdcdeb8e20445147)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataDatabricksNotebookPathsNotebookPathListOutputReference":
+    ) -> "DataDatabricksNotebookPathsNotebookPathListStructOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7433f0f7d70f30cd629fb06f35ff70304e83e67b19fc6d8c07e5502c533a3767)
+            type_hints = typing.get_type_hints(_typecheckingstub__749c4686b6b1995ffe3e28bffb808454391042079fa4889ec4403664894639cd)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataDatabricksNotebookPathsNotebookPathListOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataDatabricksNotebookPathsNotebookPathListStructOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5a7179fcf37e6e22ddf235aee84a17e31414198e181572cdb338922281a529ca)
+            type_hints = typing.get_type_hints(_typecheckingstub__a5cf1f48eed8e2b28cb444b3219b859f1e0e426afe47afe2e85fdfbf4547b0d3)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e395d44210d80102e098562189163b4a45fcf05c1d2daf1917d4167a2db2278e)
+            type_hints = typing.get_type_hints(_typecheckingstub__7811c91232400e6dbc1b429bb7a946e01220615e98d6fa4ca280e2ca8be25ad3)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1d4d6630321c33fd64add6c4ab469ecf19ef53d782fa2352900e26c945da3bf7)
+            type_hints = typing.get_type_hints(_typecheckingstub__a07fe85cec94992c9e1d1ca65ae6182c765e1fa6c7f6db23bc2f009597d3280f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataDatabricksNotebookPathsNotebookPathListOutputReference(
+class DataDatabricksNotebookPathsNotebookPathListStructOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-databricks.dataDatabricksNotebookPaths.DataDatabricksNotebookPathsNotebookPathListOutputReference",
+    jsii_type="@cdktf/provider-databricks.dataDatabricksNotebookPaths.DataDatabricksNotebookPathsNotebookPathListStructOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -443,15 +445,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__46d1e893b5e721c976c042b08103a68f893c4a40d111d4b4676ff93a698a4404)
+            type_hints = typing.get_type_hints(_typecheckingstub__a1f30df702117ca8e212b3d2fae1a8c127290d123644aae1420d6128a106d4a8)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -464,34 +466,34 @@
     def path(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "path"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataDatabricksNotebookPathsNotebookPathList]:
-        return typing.cast(typing.Optional[DataDatabricksNotebookPathsNotebookPathList], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataDatabricksNotebookPathsNotebookPathListStruct]:
+        return typing.cast(typing.Optional[DataDatabricksNotebookPathsNotebookPathListStruct], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataDatabricksNotebookPathsNotebookPathList],
+        value: typing.Optional[DataDatabricksNotebookPathsNotebookPathListStruct],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__551497ab67de5211d5eca28ccdc42e634335952d391955e1351f9f47b2e3f2c3)
+            type_hints = typing.get_type_hints(_typecheckingstub__69283a8d0660d2a554d314ea947099f48eb113ae64f73e8019e83731f7d326e0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
     "DataDatabricksNotebookPaths",
     "DataDatabricksNotebookPathsConfig",
-    "DataDatabricksNotebookPathsNotebookPathList",
-    "DataDatabricksNotebookPathsNotebookPathListList",
-    "DataDatabricksNotebookPathsNotebookPathListOutputReference",
+    "DataDatabricksNotebookPathsNotebookPathListStruct",
+    "DataDatabricksNotebookPathsNotebookPathListStructList",
+    "DataDatabricksNotebookPathsNotebookPathListStructOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__7793b8c43803333b2e9af6a2da8935a777f875a2754bc1e8d00c1a67f78cd7e9(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
@@ -540,53 +542,53 @@
     path: builtins.str,
     recursive: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__06b4ad130af3027668e27055473da95e25213246992760b84260622de7428e02(
+def _typecheckingstub__2a12cf9e99ed6468683966e02ed51ba30f43062b8ad5a877bdcdeb8e20445147(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7433f0f7d70f30cd629fb06f35ff70304e83e67b19fc6d8c07e5502c533a3767(
+def _typecheckingstub__749c4686b6b1995ffe3e28bffb808454391042079fa4889ec4403664894639cd(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__5a7179fcf37e6e22ddf235aee84a17e31414198e181572cdb338922281a529ca(
+def _typecheckingstub__a5cf1f48eed8e2b28cb444b3219b859f1e0e426afe47afe2e85fdfbf4547b0d3(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e395d44210d80102e098562189163b4a45fcf05c1d2daf1917d4167a2db2278e(
+def _typecheckingstub__7811c91232400e6dbc1b429bb7a946e01220615e98d6fa4ca280e2ca8be25ad3(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1d4d6630321c33fd64add6c4ab469ecf19ef53d782fa2352900e26c945da3bf7(
+def _typecheckingstub__a07fe85cec94992c9e1d1ca65ae6182c765e1fa6c7f6db23bc2f009597d3280f(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__46d1e893b5e721c976c042b08103a68f893c4a40d111d4b4676ff93a698a4404(
+def _typecheckingstub__a1f30df702117ca8e212b3d2fae1a8c127290d123644aae1420d6128a106d4a8(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__551497ab67de5211d5eca28ccdc42e634335952d391955e1351f9f47b2e3f2c3(
-    value: typing.Optional[DataDatabricksNotebookPathsNotebookPathList],
+def _typecheckingstub__69283a8d0660d2a554d314ea947099f48eb113ae64f73e8019e83731f7d326e0(
+    value: typing.Optional[DataDatabricksNotebookPathsNotebookPathListStruct],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/directory/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/external_location/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/external_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/grants/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_member/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/group_role/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/group_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/job/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/library/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/library/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mount/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/notebook/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/permissions/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/provider/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/recipient/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/recipient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         id_: builtins.str,
         *,
         authentication_type: builtins.str,
         name: builtins.str,
         comment: typing.Optional[builtins.str] = None,
         data_recipient_global_metastore_id: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
-        ip_access_list: typing.Optional[typing.Union["RecipientIpAccessList", typing.Dict[builtins.str, typing.Any]]] = None,
+        ip_access_list: typing.Optional[typing.Union["RecipientIpAccessListStruct", typing.Dict[builtins.str, typing.Any]]] = None,
         sharing_code: typing.Optional[builtins.str] = None,
         tokens: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["RecipientTokens", typing.Dict[builtins.str, typing.Any]]]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -98,15 +98,15 @@
         self,
         *,
         allowed_ip_addresses: typing.Sequence[builtins.str],
     ) -> None:
         '''
         :param allowed_ip_addresses: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/databricks/databricks/1.17.0/docs/resources/recipient#allowed_ip_addresses Recipient#allowed_ip_addresses}.
         '''
-        value = RecipientIpAccessList(allowed_ip_addresses=allowed_ip_addresses)
+        value = RecipientIpAccessListStruct(allowed_ip_addresses=allowed_ip_addresses)
 
         return typing.cast(None, jsii.invoke(self, "putIpAccessList", [value]))
 
     @jsii.member(jsii_name="putTokens")
     def put_tokens(
         self,
         value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["RecipientTokens", typing.Dict[builtins.str, typing.Any]]]],
@@ -150,16 +150,16 @@
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
     @jsii.member(jsii_name="ipAccessList")
-    def ip_access_list(self) -> "RecipientIpAccessListOutputReference":
-        return typing.cast("RecipientIpAccessListOutputReference", jsii.get(self, "ipAccessList"))
+    def ip_access_list(self) -> "RecipientIpAccessListStructOutputReference":
+        return typing.cast("RecipientIpAccessListStructOutputReference", jsii.get(self, "ipAccessList"))
 
     @builtins.property
     @jsii.member(jsii_name="tokens")
     def tokens(self) -> "RecipientTokensList":
         return typing.cast("RecipientTokensList", jsii.get(self, "tokens"))
 
     @builtins.property
@@ -180,16 +180,16 @@
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
     @jsii.member(jsii_name="ipAccessListInput")
-    def ip_access_list_input(self) -> typing.Optional["RecipientIpAccessList"]:
-        return typing.cast(typing.Optional["RecipientIpAccessList"], jsii.get(self, "ipAccessListInput"))
+    def ip_access_list_input(self) -> typing.Optional["RecipientIpAccessListStruct"]:
+        return typing.cast(typing.Optional["RecipientIpAccessListStruct"], jsii.get(self, "ipAccessListInput"))
 
     @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
@@ -310,15 +310,15 @@
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         authentication_type: builtins.str,
         name: builtins.str,
         comment: typing.Optional[builtins.str] = None,
         data_recipient_global_metastore_id: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
-        ip_access_list: typing.Optional[typing.Union["RecipientIpAccessList", typing.Dict[builtins.str, typing.Any]]] = None,
+        ip_access_list: typing.Optional[typing.Union["RecipientIpAccessListStruct", typing.Dict[builtins.str, typing.Any]]] = None,
         sharing_code: typing.Optional[builtins.str] = None,
         tokens: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["RecipientTokens", typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
@@ -334,15 +334,15 @@
         :param ip_access_list: ip_access_list block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/databricks/databricks/1.17.0/docs/resources/recipient#ip_access_list Recipient#ip_access_list}
         :param sharing_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/databricks/databricks/1.17.0/docs/resources/recipient#sharing_code Recipient#sharing_code}.
         :param tokens: tokens block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/databricks/databricks/1.17.0/docs/resources/recipient#tokens Recipient#tokens}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(ip_access_list, dict):
-            ip_access_list = RecipientIpAccessList(**ip_access_list)
+            ip_access_list = RecipientIpAccessListStruct(**ip_access_list)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__888161899cc76467ddd758ecd507df0ab5bbdd287fd1ebdaf5dca83f24496baf)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
@@ -484,21 +484,21 @@
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def ip_access_list(self) -> typing.Optional["RecipientIpAccessList"]:
+    def ip_access_list(self) -> typing.Optional["RecipientIpAccessListStruct"]:
         '''ip_access_list block.
 
         Docs at Terraform Registry: {@link https://registry.terraform.io/providers/databricks/databricks/1.17.0/docs/resources/recipient#ip_access_list Recipient#ip_access_list}
         '''
         result = self._values.get("ip_access_list")
-        return typing.cast(typing.Optional["RecipientIpAccessList"], result)
+        return typing.cast(typing.Optional["RecipientIpAccessListStruct"], result)
 
     @builtins.property
     def sharing_code(self) -> typing.Optional[builtins.str]:
         '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/databricks/databricks/1.17.0/docs/resources/recipient#sharing_code Recipient#sharing_code}.'''
         result = self._values.get("sharing_code")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -522,25 +522,25 @@
     def __repr__(self) -> str:
         return "RecipientConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-databricks.recipient.RecipientIpAccessList",
+    jsii_type="@cdktf/provider-databricks.recipient.RecipientIpAccessListStruct",
     jsii_struct_bases=[],
     name_mapping={"allowed_ip_addresses": "allowedIpAddresses"},
 )
-class RecipientIpAccessList:
+class RecipientIpAccessListStruct:
     def __init__(self, *, allowed_ip_addresses: typing.Sequence[builtins.str]) -> None:
         '''
         :param allowed_ip_addresses: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/databricks/databricks/1.17.0/docs/resources/recipient#allowed_ip_addresses Recipient#allowed_ip_addresses}.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__16b6633f50a092016db6cb585fb6a7205b7b063ae4383813a132f887e3036805)
+            type_hints = typing.get_type_hints(_typecheckingstub__d7cb0cdd9889bd193f10b1c7f42527d836ea49057372a297fbabe7573b42f657)
             check_type(argname="argument allowed_ip_addresses", value=allowed_ip_addresses, expected_type=type_hints["allowed_ip_addresses"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "allowed_ip_addresses": allowed_ip_addresses,
         }
 
     @builtins.property
     def allowed_ip_addresses(self) -> typing.List[builtins.str]:
@@ -552,35 +552,35 @@
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "RecipientIpAccessList(%s)" % ", ".join(
+        return "RecipientIpAccessListStruct(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class RecipientIpAccessListOutputReference(
+class RecipientIpAccessListStructOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-databricks.recipient.RecipientIpAccessListOutputReference",
+    jsii_type="@cdktf/provider-databricks.recipient.RecipientIpAccessListStructOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a1305185a5a8442405e37486409a6d3cc6846467f41bb5584a2da89b48bded34)
+            type_hints = typing.get_type_hints(_typecheckingstub__27fd25a91f685086f3d488480c26a6d275e44d49be7ca003d1f10477024f7f77)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="allowedIpAddressesInput")
     def allowed_ip_addresses_input(self) -> typing.Optional[typing.List[builtins.str]]:
@@ -590,27 +590,30 @@
     @jsii.member(jsii_name="allowedIpAddresses")
     def allowed_ip_addresses(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "allowedIpAddresses"))
 
     @allowed_ip_addresses.setter
     def allowed_ip_addresses(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__952b08cd64d09fa3ab561b2e2b4305ec2f241168615932eb5c7817a34492ba79)
+            type_hints = typing.get_type_hints(_typecheckingstub__754f28d68851ef0d66179836a8bb88eeba00bea7079dae884c387d570a2f008b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allowedIpAddresses", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[RecipientIpAccessList]:
-        return typing.cast(typing.Optional[RecipientIpAccessList], jsii.get(self, "internalValue"))
+    def internal_value(self) -> typing.Optional[RecipientIpAccessListStruct]:
+        return typing.cast(typing.Optional[RecipientIpAccessListStruct], jsii.get(self, "internalValue"))
 
     @internal_value.setter
-    def internal_value(self, value: typing.Optional[RecipientIpAccessList]) -> None:
+    def internal_value(
+        self,
+        value: typing.Optional[RecipientIpAccessListStruct],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__825ba27613764acb1315e0f5053ab52463ff580329697bec38fd960dfa4f1cd9)
+            type_hints = typing.get_type_hints(_typecheckingstub__00a7bd087a4001cd40dfeeb75882b99ff8d82dfd73083f6dbf37050c77e81ca6)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
     jsii_type="@cdktf/provider-databricks.recipient.RecipientTokens",
     jsii_struct_bases=[],
@@ -1008,16 +1011,16 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
     "Recipient",
     "RecipientConfig",
-    "RecipientIpAccessList",
-    "RecipientIpAccessListOutputReference",
+    "RecipientIpAccessListStruct",
+    "RecipientIpAccessListStructOutputReference",
     "RecipientTokens",
     "RecipientTokensList",
     "RecipientTokensOutputReference",
 ]
 
 publication.publish()
 
@@ -1026,15 +1029,15 @@
     id_: builtins.str,
     *,
     authentication_type: builtins.str,
     name: builtins.str,
     comment: typing.Optional[builtins.str] = None,
     data_recipient_global_metastore_id: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
-    ip_access_list: typing.Optional[typing.Union[RecipientIpAccessList, typing.Dict[builtins.str, typing.Any]]] = None,
+    ip_access_list: typing.Optional[typing.Union[RecipientIpAccessListStruct, typing.Dict[builtins.str, typing.Any]]] = None,
     sharing_code: typing.Optional[builtins.str] = None,
     tokens: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[RecipientTokens, typing.Dict[builtins.str, typing.Any]]]]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -1096,43 +1099,43 @@
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     authentication_type: builtins.str,
     name: builtins.str,
     comment: typing.Optional[builtins.str] = None,
     data_recipient_global_metastore_id: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
-    ip_access_list: typing.Optional[typing.Union[RecipientIpAccessList, typing.Dict[builtins.str, typing.Any]]] = None,
+    ip_access_list: typing.Optional[typing.Union[RecipientIpAccessListStruct, typing.Dict[builtins.str, typing.Any]]] = None,
     sharing_code: typing.Optional[builtins.str] = None,
     tokens: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[RecipientTokens, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__16b6633f50a092016db6cb585fb6a7205b7b063ae4383813a132f887e3036805(
+def _typecheckingstub__d7cb0cdd9889bd193f10b1c7f42527d836ea49057372a297fbabe7573b42f657(
     *,
     allowed_ip_addresses: typing.Sequence[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a1305185a5a8442405e37486409a6d3cc6846467f41bb5584a2da89b48bded34(
+def _typecheckingstub__27fd25a91f685086f3d488480c26a6d275e44d49be7ca003d1f10477024f7f77(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__952b08cd64d09fa3ab561b2e2b4305ec2f241168615932eb5c7817a34492ba79(
+def _typecheckingstub__754f28d68851ef0d66179836a8bb88eeba00bea7079dae884c387d570a2f008b(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__825ba27613764acb1315e0f5053ab52463ff580329697bec38fd960dfa4f1cd9(
-    value: typing.Optional[RecipientIpAccessList],
+def _typecheckingstub__00a7bd087a4001cd40dfeeb75882b99ff8d82dfd73083f6dbf37050c77e81ca6(
+    value: typing.Optional[RecipientIpAccessListStruct],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__42ac5a80329dcd8dfc6a8de5d96858835f89c6ee809af5f79a0a83fb48061c69(
     *,
     activation_url: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/repo/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/schema/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/share/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/share/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/table/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/token/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/user_role/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/user_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-databricks
-Version: 7.0.4
+Version: 7.0.5
 Summary: Prebuilt databricks Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-databricks.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-databricks.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.4/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-databricks-7.0.5/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_databricks/py.typed
 src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
 src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
 src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
-src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@7.0.4.jsii.tgz
+src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@7.0.5.jsii.tgz
 src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/catalog/__init__.py
 src/cdktf_cdktf_provider_databricks/cluster/__init__.py
 src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
```

