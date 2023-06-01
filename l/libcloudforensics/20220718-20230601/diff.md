# Comparing `tmp/libcloudforensics-20220718.tar.gz` & `tmp/libcloudforensics-20230601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libcloudforensics-20220718.tar", last modified: Mon Jul 18 09:37:32 2022, max compression
+gzip compressed data, was "dist/libcloudforensics-20230601.tar", last modified: Thu Jun  1 02:38:16 2023, max compression
```

## Comparing `libcloudforensics-20220718.tar` & `libcloudforensics-20230601.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/
--rw-r--r--   0 runner    (1001) docker     (116)      125 2022-07-18 09:37:30.000000 libcloudforensics-20220718/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      664 2022-07-18 09:37:32.000000 libcloudforensics-20220718/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1009 2022-07-18 09:37:30.000000 libcloudforensics-20220718/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/
--rw-r--r--   0 runner    (1001) docker     (116)      659 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2921 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     4407 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     9937 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    25178 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/forensics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6928 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/account.py
--rw-r--r--   0 runner    (1001) docker     (116)     3917 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (116)    22867 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/ebs.py
--rw-r--r--   0 runner    (1001) docker     (116)    27258 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/ec2.py
--rw-r--r--   0 runner    (1001) docker     (116)    13025 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/iam.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/iampolicies/
--rw-r--r--   0 runner    (1001) docker     (116)      518 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/iampolicies/ebs_copy_to_s3_policy.json
--rw-r--r--   0 runner    (1001) docker     (116)      191 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/iampolicies/ec2_assume_role_policy.json
--rw-r--r--   0 runner    (1001) docker     (116)      236 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/iampolicies/revoke_old_sessions.json
--rw-r--r--   0 runner    (1001) docker     (116)     4318 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/kms.py
--rw-r--r--   0 runner    (1001) docker     (116)     2959 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/log.py
--rw-r--r--   0 runner    (1001) docker     (116)    10054 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/aws/internal/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8344 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/forensics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4772 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/account.py
--rw-r--r--   0 runner    (1001) docker     (116)    10864 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (116)    31748 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/compute.py
--rw-r--r--   0 runner    (1001) docker     (116)     3199 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/compute_base_resource.py
--rw-r--r--   0 runner    (1001) docker     (116)     5195 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (116)     7711 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/network.py
--rw-r--r--   0 runner    (1001) docker     (116)     3208 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/resource.py
--rw-r--r--   0 runner    (1001) docker     (116)     4992 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/azure/internal/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    26838 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/forensics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1817 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (116)     4552 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/build.py
--rw-r--r--   0 runner    (1001) docker     (116)     5706 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/cloudresourcemanager.py
--rw-r--r--   0 runner    (1001) docker     (116)     1916 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (116)    11045 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (116)    81883 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/compute.py
--rw-r--r--   0 runner    (1001) docker     (116)     8110 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/compute_base_resource.py
--rw-r--r--   0 runner    (1001) docker     (116)     3496 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/function.py
--rw-r--r--   0 runner    (1001) docker     (116)     8321 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/gke.py
--rw-r--r--   0 runner    (1001) docker     (116)     3768 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/log.py
--rw-r--r--   0 runner    (1001) docker     (116)     6462 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (116)     9160 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/project.py
--rw-r--r--   0 runner    (1001) docker     (116)     3708 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/serviceusage.py
--rw-r--r--   0 runner    (1001) docker     (116)    12610 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     6727 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/storagetransfer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11885 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    11611 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)     2341 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/container.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/enumerations/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/enumerations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13164 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/enumerations/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1751 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/enumerations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (116)     4786 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/mitigation.py
--rw-r--r--   0 runner    (1001) docker     (116)     5769 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/netpol.py
--rw-r--r--   0 runner    (1001) docker     (116)     3344 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/selector.py
--rw-r--r--   0 runner    (1001) docker     (116)     2909 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (116)     2427 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/volume.py
--rw-r--r--   0 runner    (1001) docker     (116)     6809 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/kubernetes/workloads.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/providers/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/providers/utils/storage_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics/scripts/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1697 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/scripts/ebs_snapshot_copy_aws.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      891 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/scripts/forensics_packages_startup.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      788 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/scripts/forensics_packages_startup_aws.sh
--rw-r--r--   0 runner    (1001) docker     (116)     2241 2022-07-18 09:37:30.000000 libcloudforensics-20220718/libcloudforensics/scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      664 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6094 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       51 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      329 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2022-07-18 09:37:32.000000 libcloudforensics-20220718/libcloudforensics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      133 2022-07-18 09:37:30.000000 libcloudforensics-20220718/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      520 2022-07-18 09:37:30.000000 libcloudforensics-20220718/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-07-18 09:37:32.000000 libcloudforensics-20220718/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-07-18 09:37:30.000000 libcloudforensics-20220718/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3671 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/aws_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     5659 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/aws_mocks.py
--rw-r--r--   0 runner    (1001) docker     (116)    14411 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/e2e.py
--rw-r--r--   0 runner    (1001) docker     (116)    12907 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/e2e_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/aws/internal/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2024 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/internal/test_common.py
--rw-r--r--   0 runner    (1001) docker     (116)     9561 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/internal/test_ebs.py
--rw-r--r--   0 runner    (1001) docker     (116)     8943 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/internal/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (116)     1330 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/internal/test_log.py
--rw-r--r--   0 runner    (1001) docker     (116)     1752 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/internal/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (116)     6165 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/aws/test_forensics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3089 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/azure_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     4755 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/azure_mocks.py
--rw-r--r--   0 runner    (1001) docker     (116)     8960 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/e2e.py
--rw-r--r--   0 runner    (1001) docker     (116)    11001 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/e2e_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/azure/internal/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8303 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/internal/test_common.py
--rw-r--r--   0 runner    (1001) docker     (116)    17456 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/internal/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (116)     1990 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/internal/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (116)     1346 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/internal/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (116)     2051 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/internal/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     8938 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/azure/test_forensics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12021 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/e2e.py
--rw-r--r--   0 runner    (1001) docker     (116)    13131 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/e2e_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     2640 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/gcp_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    29699 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/gcp_mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/gcp/internal/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1639 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (116)     2202 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_build.py
--rw-r--r--   0 runner    (1001) docker     (116)     5459 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_cloudresourcemanager.py
--rw-r--r--   0 runner    (1001) docker     (116)     1487 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (116)     3469 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_common.py
--rw-r--r--   0 runner    (1001) docker     (116)    32925 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (116)     1447 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_compute_base_resource.py
--rw-r--r--   0 runner    (1001) docker     (116)     1726 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_gke.py
--rw-r--r--   0 runner    (1001) docker     (116)     1867 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_log.py
--rw-r--r--   0 runner    (1001) docker     (116)     3609 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (116)     3165 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_serviceusage.py
--rw-r--r--   0 runner    (1001) docker     (116)     5324 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     3208 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/internal/test_storagetransfer.py
--rw-r--r--   0 runner    (1001) docker     (116)     7659 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/gcp/test_forensics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5120 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/kubernetes/k8s_mocks.py
--rw-r--r--   0 runner    (1001) docker     (116)     7250 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/kubernetes/test_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     4516 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/kubernetes/test_netpol.py
--rw-r--r--   0 runner    (1001) docker     (116)     1756 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/kubernetes/test_services.py
--rw-r--r--   0 runner    (1001) docker     (116)     7602 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/providers/kubernetes/test_workloads.py
--rw-r--r--   0 runner    (1001) docker     (116)      881 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2179 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tests/scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-18 09:37:32.000000 libcloudforensics-20220718/tools/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10379 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tools/aws_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     7429 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tools/az_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    26694 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    19174 2022-07-18 09:37:30.000000 libcloudforensics-20220718/tools/gcp_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-01 02:38:12.000000 libcloudforensics-20230601/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-01 02:38:16.000000 libcloudforensics-20230601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 02:38:12.000000 libcloudforensics-20230601/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/forensics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22867 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/ebs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27258 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/iam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/iampolicies/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/iampolicies/ebs_copy_to_s3_policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/iampolicies/ec2_assume_role_policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/iampolicies/revoke_old_sessions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/aws/internal/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/forensics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31763 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/compute_base_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/azure/internal/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26838 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/forensics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/cloudresourcemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/cloudsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81883 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/compute_base_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/gke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/serviceusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/storagetransfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/enumerations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/enumerations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/enumerations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/enumerations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/netpol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/kubernetes/workloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/providers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/providers/utils/storage_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/scripts/ebs_snapshot_copy_aws.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/scripts/forensics_packages_startup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/scripts/forensics_packages_startup_aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-01 02:38:12.000000 libcloudforensics-20230601/libcloudforensics/scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/libcloudforensics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-01 02:38:15.000000 libcloudforensics-20230601/libcloudforensics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-01 02:38:15.000000 libcloudforensics-20230601/libcloudforensics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:38:15.000000 libcloudforensics-20230601/libcloudforensics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 02:38:15.000000 libcloudforensics-20230601/libcloudforensics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:38:15.000000 libcloudforensics-20230601/libcloudforensics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 02:38:15.000000 libcloudforensics-20230601/libcloudforensics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 02:38:15.000000 libcloudforensics-20230601/libcloudforensics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 02:38:12.000000 libcloudforensics-20230601/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-01 02:38:12.000000 libcloudforensics-20230601/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 02:38:16.000000 libcloudforensics-20230601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-01 02:38:12.000000 libcloudforensics-20230601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/aws_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/aws_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/e2e_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/aws/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/internal/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/internal/test_ebs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/internal/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/internal/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/internal/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/aws/test_forensics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/azure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/azure_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/e2e_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/azure/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/internal/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/internal/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/internal/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/internal/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/internal/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/azure/test_forensics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/e2e_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/gcp_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29699 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/gcp_mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/gcp/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_cloudresourcemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_cloudsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32925 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_compute_base_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_gke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_serviceusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/internal/test_storagetransfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/gcp/test_forensics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/kubernetes/k8s_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/kubernetes/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/kubernetes/test_netpol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/kubernetes/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/providers/kubernetes/test_workloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tests/scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:16.000000 libcloudforensics-20230601/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tools/aws_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tools/az_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-06-01 02:38:12.000000 libcloudforensics-20230601/tools/gcp_cli.py
```

### Comparing `libcloudforensics-20220718/PKG-INFO` & `libcloudforensics-20230601/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: libcloudforensics
-Version: 20220718
+Version: 20230601
 Summary: libcloudforensics is a set of tools to help acquire forensic evidence from cloud platforms.
 Home-page: http://github.com/google/cloud-forensics-utils/
 Maintainer: Cloud-forensics-utils development team
 Maintainer-email: cloud-forensics-utils-dev@googlegroups.com
 License: Apache License, Version 2.0
 Description: libcloudforensics is a set of tools to help acquire forensic evidence from cloud platforms.
 Platform: UNKNOWN
```

### Comparing `libcloudforensics-20220718/README.md` & `libcloudforensics-20230601/README.md`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/__init__.py` & `libcloudforensics-20230601/libcloudforensics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """libcloud forensics module."""
 
-__version__ = '20220718'
+__version__ = '20230601'
```

### Comparing `libcloudforensics-20220718/libcloudforensics/errors.py` & `libcloudforensics-20230601/libcloudforensics/errors.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/logging_utils.py` & `libcloudforensics-20230601/libcloudforensics/logging_utils.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/prompts.py` & `libcloudforensics-20230601/libcloudforensics/prompts.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/forensics.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/forensics.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/account.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/account.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/common.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # Resource types constant
 INSTANCE = 'instance'
 VOLUME = 'volume'
 SNAPSHOT = 'snapshot'
 
 # Default Amazon Machine Images to use for bootstrapping instances
-UBUNTU_1804_FILTER = 'ubuntu/images/hvm-ssd/ubuntu-bionic-18.04-amd64-server-20200611'  # pylint: disable=line-too-long
+UBUNTU_1804_FILTER = 'ubuntu/images/hvm-ssd/ubuntu-bionic-18.04-amd64-server-20220810'  # pylint: disable=line-too-long
 ALINUX2_BASE_FILTER = 'amzn2-ami-hvm-2*-x86_64-gp2'
 
 
 def CreateTags(resource: str, tags: Dict[str, str]) -> Dict[str, Any]:
   """Create AWS Tag Specifications.
 
   Args:
```

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/ebs.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/ebs.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/ec2.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/ec2.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/iam.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/iam.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """AWS IAM Functionality"""
 
 import datetime
 import json
 import os
-from typing import TYPE_CHECKING, Optional, Tuple
+from typing import TYPE_CHECKING, Tuple
 from libcloudforensics import errors
 from libcloudforensics import logging_utils
 from libcloudforensics.providers.aws.internal import common
 
 if TYPE_CHECKING:
   # TYPE_CHECKING is always False at runtime, therefore it is safe to ignore
   # the following cyclic import, as it it only used for type hints
```

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/iampolicies/ebs_copy_to_s3_policy.json` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/iampolicies/ebs_copy_to_s3_policy.json`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/kms.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/kms.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/log.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/log.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/aws/internal/s3.py` & `libcloudforensics-20230601/libcloudforensics/providers/aws/internal/s3.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/forensics.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/forensics.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/account.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/account.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/common.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/common.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/compute.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # Pylint complains about the import but the library imports just fine,
 # so we can ignore the warning.
 # pylint: disable=import-error
 import sshpubkeys
 from msrestazure import azure_exceptions
 from azure.storage import blob
 from azure.core import exceptions
-from azure.mgmt import compute as compute_sdk
+from azure.mgmt import compute as compute_sdk # type: ignore
 from azure.mgmt.compute.v2020_05_01 import models
 # pylint: enable=import-error
 
 from libcloudforensics import logging_utils
 from libcloudforensics import errors
 from libcloudforensics.providers.azure.internal import compute_base_resource  # pylint: disable=line-too-long, ungrouped-imports
 from libcloudforensics.providers.azure.internal import common  # pylint: disable=line-too-long, ungrouped-imports
```

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/compute_base_resource.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/compute_base_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Azure Compute Base Resource."""
 
 from typing import Optional, List, TYPE_CHECKING
 
-from azure.mgmt import compute as compute_sdk  # pylint: disable=import-error
+# pylint: disable=import-error
+from azure.mgmt import compute as compute_sdk # type: ignore
+# pylint: enable=import-error
 
 from libcloudforensics import errors
 from libcloudforensics.providers.azure.internal import common
 
 if TYPE_CHECKING:
   # TYPE_CHECKING is always False at runtime, therefore it is safe to ignore
   # the following cyclic import, as it it only used for type hints
```

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/monitoring.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/monitoring.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/network.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/network.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/resource.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Azure Resource functionality."""
 
 from typing import TYPE_CHECKING, List
 
 # pylint: disable=import-error
-from azure.mgmt import resource
+from azure.mgmt import resource # type: ignore
 from msrestazure import azure_exceptions
 # pylint: enable=import-error
 
 from libcloudforensics import logging_utils
 
 if TYPE_CHECKING:
   # TYPE_CHECKING is always False at runtime, therefore it is safe to ignore
```

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/azure/internal/storage.py` & `libcloudforensics-20230601/libcloudforensics/providers/azure/internal/storage.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/forensics.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/forensics.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/bigquery.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/bigquery.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/build.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/build.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/cloudresourcemanager.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/cloudresourcemanager.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/cloudsql.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/cloudsql.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/common.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/common.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/compute.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/compute.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/compute_base_resource.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/compute_base_resource.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/function.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/function.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/gke.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/gke.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/log.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/log.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/monitoring.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/monitoring.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/project.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/project.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/serviceusage.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/serviceusage.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/storage.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/storage.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/gcp/internal/storagetransfer.py` & `libcloudforensics-20230601/libcloudforensics/providers/gcp/internal/storagetransfer.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/base.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/base.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/cluster.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/cluster.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/container.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/container.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/enumerations/base.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/enumerations/base.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/enumerations/gcp.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/enumerations/gcp.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/mitigation.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/mitigation.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/netpol.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/netpol.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/selector.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/selector.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/services.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/volume.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/volume.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/kubernetes/workloads.py` & `libcloudforensics-20230601/libcloudforensics/providers/kubernetes/workloads.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/providers/utils/storage_utils.py` & `libcloudforensics-20230601/libcloudforensics/providers/utils/storage_utils.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/scripts/ebs_snapshot_copy_aws.sh` & `libcloudforensics-20230601/libcloudforensics/scripts/ebs_snapshot_copy_aws.sh`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/scripts/forensics_packages_startup.sh` & `libcloudforensics-20230601/libcloudforensics/scripts/forensics_packages_startup.sh`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/scripts/forensics_packages_startup_aws.sh` & `libcloudforensics-20230601/libcloudforensics/scripts/forensics_packages_startup_aws.sh`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics/scripts/utils.py` & `libcloudforensics-20230601/libcloudforensics/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/libcloudforensics.egg-info/PKG-INFO` & `libcloudforensics-20230601/libcloudforensics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: libcloudforensics
-Version: 20220718
+Version: 20230601
 Summary: libcloudforensics is a set of tools to help acquire forensic evidence from cloud platforms.
 Home-page: http://github.com/google/cloud-forensics-utils/
 Maintainer: Cloud-forensics-utils development team
 Maintainer-email: cloud-forensics-utils-dev@googlegroups.com
 License: Apache License, Version 2.0
 Description: libcloudforensics is a set of tools to help acquire forensic evidence from cloud platforms.
 Platform: UNKNOWN
```

### Comparing `libcloudforensics-20220718/libcloudforensics.egg-info/SOURCES.txt` & `libcloudforensics-20230601/libcloudforensics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/setup.py` & `libcloudforensics-20230601/setup.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/aws_cli.py` & `libcloudforensics-20230601/tests/providers/aws/aws_cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/aws_mocks.py` & `libcloudforensics-20230601/tests/providers/aws/aws_mocks.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/e2e.py` & `libcloudforensics-20230601/tests/providers/aws/e2e.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
   def testListImages(self):
     """End to end test on AWS.
 
     Test listing AMI images with a filter.
     """
 
     aws_account = account.AWSAccount(self.zone)
-    qfilter = [{'Name': 'name', 'Values': ['Ubuntu 18.04*']}]
+    qfilter = [{'Name': 'name', 'Values': ['Ubuntu 22.04*']}]
     images = aws_account.ec2.ListImages(qfilter)
 
     self.assertGreater(len(images), 0)
     self.assertIn('Name', images[0])
 
   @typing.no_type_check
   @IgnoreWarnings
```

### Comparing `libcloudforensics-20220718/tests/providers/aws/e2e_cli.py` & `libcloudforensics-20230601/tests/providers/aws/e2e_cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/internal/test_common.py` & `libcloudforensics-20230601/tests/providers/aws/internal/test_common.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/internal/test_ebs.py` & `libcloudforensics-20230601/tests/providers/aws/internal/test_ebs.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/internal/test_ec2.py` & `libcloudforensics-20230601/tests/providers/aws/internal/test_ec2.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/internal/test_log.py` & `libcloudforensics-20230601/tests/providers/aws/internal/test_log.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/internal/test_s3.py` & `libcloudforensics-20230601/tests/providers/aws/internal/test_s3.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/aws/test_forensics.py` & `libcloudforensics-20230601/tests/providers/aws/test_forensics.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/azure_cli.py` & `libcloudforensics-20230601/tests/providers/azure/azure_cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/azure_mocks.py` & `libcloudforensics-20230601/tests/providers/azure/azure_mocks.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/e2e.py` & `libcloudforensics-20230601/tests/providers/azure/e2e.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/e2e_cli.py` & `libcloudforensics-20230601/tests/providers/azure/e2e_cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/internal/test_common.py` & `libcloudforensics-20230601/tests/providers/azure/internal/test_common.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/internal/test_compute.py` & `libcloudforensics-20230601/tests/providers/azure/internal/test_compute.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/internal/test_monitoring.py` & `libcloudforensics-20230601/tests/providers/azure/internal/test_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 
 
 class AZMonitoringTest(unittest.TestCase):
   """Test Azure monitoring class."""
   # pylint: disable=line-too-long
 
   @typing.no_type_check
-  @mock.patch('azure.mgmt.monitor.v2018_01_01.operations._metric_definitions_operations.MetricDefinitionsOperations.list')
+  @mock.patch('azure.mgmt.monitor.v2021_05_01.operations._metric_definitions_operations.MetricDefinitionsOperations.list')
   def testListAvailableMetricsForResource(self, mock_list_metrics):
     """Test that metrics are correctly listed."""
     mock_list_metrics.return_value = azure_mocks.MOCK_LIST_METRICS
     metrics = azure_mocks.FAKE_MONITORING.ListAvailableMetricsForResource(
         'fake-resource-id')
     self.assertEqual(1, len(metrics))
     self.assertIn('fake-metric', metrics)
 
   @typing.no_type_check
-  @mock.patch('azure.mgmt.monitor.v2018_01_01.operations._metrics_operations.MetricsOperations.list')
+  @mock.patch('azure.mgmt.monitor.v2021_05_01.operations._metrics_operations.MetricsOperations.list')
   def testGetMetricsForResource(self, mock_list_metrics_operations):
     """Test that metrics values are correctly retrieved."""
     mock_list_metrics_operations.return_value = azure_mocks.MOCK_METRIC_OPERATION
     metrics = azure_mocks.FAKE_MONITORING.GetMetricsForResource(
         'fake-resource-id', 'fake-metric')
     self.assertIn('fake-metric', metrics)
     self.assertEqual(1, len(metrics['fake-metric']))
```

### Comparing `libcloudforensics-20220718/tests/providers/azure/internal/test_resource.py` & `libcloudforensics-20230601/tests/providers/azure/internal/test_resource.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/azure/internal/test_storage.py` & `libcloudforensics-20230601/tests/providers/azure/internal/test_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from tests.providers.azure import azure_mocks
 
 
 class AZStorageTest(unittest.TestCase):
   """Test Azure storage class."""
   # pylint: disable=line-too-long
 
-  @mock.patch('azure.mgmt.storage.v2021_09_01.operations._storage_accounts_operations.StorageAccountsOperations.list_keys')
-  @mock.patch('azure.mgmt.storage.v2021_09_01.operations._storage_accounts_operations.StorageAccountsOperations.begin_create')
+  @mock.patch('azure.mgmt.storage.v2022_09_01.operations._storage_accounts_operations.StorageAccountsOperations.list_keys')
+  @mock.patch('azure.mgmt.storage.v2022_09_01.operations._storage_accounts_operations.StorageAccountsOperations.begin_create')
   @typing.no_type_check
   def testCreateStorageAccount(self, mock_create, mock_list_keys):
     """Test that a storage account is created and its information retrieved"""
     # pylint: disable=protected-access
     mock_create.return_value.result.return_value = azure_mocks.MOCK_STORAGE_ACCOUNT
     mock_list_keys.return_value = azure_mocks.MOCK_LIST_KEYS
     account_id, account_key = azure_mocks.FAKE_ACCOUNT.storage.CreateStorageAccount(
```

### Comparing `libcloudforensics-20220718/tests/providers/azure/test_forensics.py` & `libcloudforensics-20230601/tests/providers/azure/test_forensics.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/e2e.py` & `libcloudforensics-20230601/tests/providers/gcp/e2e.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/e2e_cli.py` & `libcloudforensics-20230601/tests/providers/gcp/e2e_cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/gcp_cli.py` & `libcloudforensics-20230601/tests/providers/gcp/gcp_cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/gcp_mocks.py` & `libcloudforensics-20230601/tests/providers/gcp/gcp_mocks.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_bigquery.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_build.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_build.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_cloudresourcemanager.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_cloudresourcemanager.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_cloudsql.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_cloudsql.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_common.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_common.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_compute.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_compute.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_compute_base_resource.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_compute_base_resource.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_gke.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_gke.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_log.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_log.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_monitoring.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_serviceusage.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_serviceusage.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_storage.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_storage.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/internal/test_storagetransfer.py` & `libcloudforensics-20230601/tests/providers/gcp/internal/test_storagetransfer.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/gcp/test_forensics.py` & `libcloudforensics-20230601/tests/providers/gcp/test_forensics.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/kubernetes/k8s_mocks.py` & `libcloudforensics-20230601/tests/providers/kubernetes/k8s_mocks.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/kubernetes/test_base.py` & `libcloudforensics-20230601/tests/providers/kubernetes/test_base.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/kubernetes/test_netpol.py` & `libcloudforensics-20230601/tests/providers/kubernetes/test_netpol.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/kubernetes/test_services.py` & `libcloudforensics-20230601/tests/providers/kubernetes/test_services.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/providers/kubernetes/test_workloads.py` & `libcloudforensics-20230601/tests/providers/kubernetes/test_workloads.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/run_tests.py` & `libcloudforensics-20230601/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tests/scripts/utils.py` & `libcloudforensics-20230601/tests/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tools/aws_cli.py` & `libcloudforensics-20230601/tools/aws_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 import json
 import os
 
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 from libcloudforensics.providers.aws.internal import account
-from libcloudforensics.providers.aws.internal import ec2
-from libcloudforensics.providers.aws.internal import iam
 from libcloudforensics.providers.aws.internal import log as aws_log
 from libcloudforensics.providers.aws import forensics
 from libcloudforensics import logging_utils
 
 logging_utils.SetUpLogger(__name__)
 logger = logging_utils.GetLogger(__name__)
```

### Comparing `libcloudforensics-20220718/tools/az_cli.py` & `libcloudforensics-20230601/tools/az_cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tools/cli.py` & `libcloudforensics-20230601/tools/cli.py`

 * *Files identical despite different names*

### Comparing `libcloudforensics-20220718/tools/gcp_cli.py` & `libcloudforensics-20230601/tools/gcp_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     qfilter += args.filter
   elif args.filter:
     qfilter += args.filter
 
   results = logs.ExecuteQuery(qfilter.split(',') if qfilter else None)
   logger.info('Found {0:d} log entries:'.format(len(results)))
   for line in results:
-    logger.info(json.dumps(line))
+    print(json.dumps(line))
 
 
 def CreateDiskFromGCSImage(args: 'argparse.Namespace') -> None:
   """Creates GCE persistent disk from image in GCS.
 
   Please refer to doc string of forensics.CreateDiskFromGCSImage
   function for more details on how the image is created.
```

