# Comparing `tmp/pulumi_artifactory-3.6.0a1685164706.tar.gz` & `tmp/pulumi_artifactory-3.6.0a1685615210.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_artifactory-3.6.0a1685164706.tar", last modified: Sat May 27 05:26:12 2023, max compression
+gzip compressed data, was "pulumi_artifactory-3.6.0a1685615210.tar", last modified: Thu Jun  1 10:31:17 2023, max compression
```

## Comparing `pulumi_artifactory-3.6.0a1685164706.tar` & `pulumi_artifactory-3.6.0a1685615210.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:26:12.701774 pulumi_artifactory-3.6.0a1685164706/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-27 05:26:12.701774 pulumi_artifactory-3.6.0a1685164706/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:26:12.701774 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/
--rw-r--r--   0 runner    (1001) docker     (123)    45822 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367032 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33734 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    55059 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/anonymous_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/artifact_property_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/artifact_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/artifactory_release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/build_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:26:12.701774 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/distribution_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/distribution_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/docker_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/general_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_terraformbackend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/ldap_group_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/ldap_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_repository_multi_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_repository_single_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_terraform_backend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    26725 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/managed_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/oauth_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   320747 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/permission_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/property_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/pull_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/push_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_repository_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/repository_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/saml_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    41731 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/scoped_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/single_replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/unmanaged_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_terraform_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:26:12.701774 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 05:26:12.701774 pulumi_artifactory-3.6.0a1685164706/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-27 05:26:12.000000 pulumi_artifactory-3.6.0a1685164706/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:31:17.541293 pulumi_artifactory-3.6.0a1685615210/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-01 10:31:17.541293 pulumi_artifactory-3.6.0a1685615210/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:31:17.541293 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/
+-rw-r--r--   0 runner    (1001) docker     (123)    45822 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   367032 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33734 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55059 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/anonymous_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/artifact_property_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/artifact_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/artifactory_release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/build_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:31:17.541293 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/distribution_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/distribution_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/docker_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/general_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_terraformbackend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/ldap_group_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/ldap_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_repository_multi_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_repository_single_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_terraform_backend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26725 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/managed_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/oauth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   320747 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/permission_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/pull_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/push_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_repository_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/repository_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/saml_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45108 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/scoped_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/single_replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/unmanaged_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_terraform_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:31:17.541293 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 10:31:17.541293 pulumi_artifactory-3.6.0a1685615210/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-01 10:31:17.000000 pulumi_artifactory-3.6.0a1685615210/setup.py
```

### Comparing `pulumi_artifactory-3.6.0a1685164706/PKG-INFO` & `pulumi_artifactory-3.6.0a1685615210/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_artifactory
-Version: 3.6.0a1685164706
+Version: 3.6.0a1685615210
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-3.6.0a1685164706/README.md` & `pulumi_artifactory-3.6.0a1685615210/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/__init__.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/_inputs.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/_utilities.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/access_token.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/anonymous_user.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/anonymous_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/api_key.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/artifact_property_webhook.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/artifact_property_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/artifact_webhook.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/artifact_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/artifactory_release_bundle_webhook.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/artifactory_release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/backup.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/build_webhook.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/build_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/certificate.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/config/vars.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/distribution_public_key.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/distribution_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/distribution_webhook.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/distribution_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/docker_v1_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/docker_v2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/docker_webhook.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/docker_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_cargo_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_cocoapods_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_docker_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_docker_v1_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_docker_v2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_gitltfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_maven_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_opkg_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_terraform_module_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_terraform_provider_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/federated_vagrant_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/general_security.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/general_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_cargo_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_cocoapods_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_docker_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_docker_v1_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_docker_v2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_gitlfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_maven_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_opkg_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_terraform_module_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_terraform_provider_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_federated_vagrant_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_file.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_fileinfo.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_fileinfo.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_group.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_cargo_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_cocoapods_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_docker_v1_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_docker_v2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_gitlfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_maven_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_opkg_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_pub_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_terraform_module_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_terraform_provider_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_terraformbackend_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_terraformbackend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_local_vagrant_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_permission_target.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_cargo_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_cocoapods_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_docker_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_gitlfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_maven_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_opkg_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_p2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_pub_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_terraform_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_remote_vcs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_user.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_docker_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_gitlfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_p2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_pub_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/get_virtual_terraform_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/get_virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/group.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/keypair.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/keypair.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/ldap_group_setting.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/ldap_group_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/ldap_setting.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/ldap_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_cargo_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_cocoapods_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_gitltfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_maven_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_opkg_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_pub_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_repository_multi_replication.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_repository_multi_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_repository_single_replication.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_repository_single_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_terraform_backend_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_terraform_backend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_terraform_module_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_terraform_provider_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/local_vagrant_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/managed_user.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/managed_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/maven_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/oauth_settings.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/oauth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/outputs.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/permission_target.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/permission_targets.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/permission_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/property_set.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/property_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/provider.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/proxy.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/pull_replication.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/pull_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/push_replication.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/push_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/release_bundle_webhook.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_cargo_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_cocoapods_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_docker_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_gitlfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_go_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_maven_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_opkg_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_p2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_pub_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_repository_replication.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_repository_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_terraform_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/remote_vcs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/replication_config.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/repository_layout.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/repository_layout.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/saml_settings.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/saml_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/scoped_token.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_puppet_repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,803 +5,736 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ScopedTokenArgs', 'ScopedToken']
+__all__ = ['VirtualPuppetRepositoryArgs', 'VirtualPuppetRepository']
 
 @pulumi.input_type
-class ScopedTokenArgs:
+class VirtualPuppetRepositoryArgs:
     def __init__(__self__, *,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 key: pulumi.Input[str],
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 include_reference_token: Optional[pulumi.Input[bool]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a ScopedToken resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
-        """
-        if audiences is not None:
-            pulumi.set(__self__, "audiences", audiences)
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        The set of arguments for constructing a VirtualPuppetRepository resource.
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        """
+        pulumi.set(__self__, "key", key)
+        if artifactory_requests_can_retrieve_remote_artifacts is not None:
+            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
+        if default_deployment_repo is not None:
+            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if expires_in is not None:
-            pulumi.set(__self__, "expires_in", expires_in)
-        if include_reference_token is not None:
-            pulumi.set(__self__, "include_reference_token", include_reference_token)
-        if refreshable is not None:
-            pulumi.set(__self__, "refreshable", refreshable)
-        if scopes is not None:
-            pulumi.set(__self__, "scopes", scopes)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+        if excludes_pattern is not None:
+            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
+        if includes_pattern is not None:
+            pulumi.set(__self__, "includes_pattern", includes_pattern)
+        if notes is not None:
+            pulumi.set(__self__, "notes", notes)
+        if project_environments is not None:
+            pulumi.set(__self__, "project_environments", project_environments)
+        if project_key is not None:
+            pulumi.set(__self__, "project_key", project_key)
+        if repo_layout_ref is not None:
+            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
+        if repositories is not None:
+            pulumi.set(__self__, "repositories", repositories)
 
     @property
     @pulumi.getter
-    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def key(self) -> pulumi.Input[str]:
         """
-        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+        contain spaces or special characters.
         """
-        return pulumi.get(self, "audiences")
+        return pulumi.get(self, "key")
 
-    @audiences.setter
-    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "audiences", value)
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
+    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+        another Artifactory instance.
+        """
+        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
+
+    @artifactory_requests_can_retrieve_remote_artifacts.setter
+    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
+
+    @property
+    @pulumi.getter(name="defaultDeploymentRepo")
+    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default repository to deploy artifacts.
+        """
+        return pulumi.get(self, "default_deployment_repo")
+
+    @default_deployment_repo.setter
+    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_deployment_repo", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        Public description.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="expiresIn")
-    def expires_in(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="excludesPattern")
+    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+        artifacts are excluded.
         """
-        return pulumi.get(self, "expires_in")
+        return pulumi.get(self, "excludes_pattern")
 
-    @expires_in.setter
-    def expires_in(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expires_in", value)
+    @excludes_pattern.setter
+    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "excludes_pattern", value)
 
     @property
-    @pulumi.getter(name="includeReferenceToken")
-    def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="includesPattern")
+    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Should a reference token also be created? Defaults to `false`
+        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         """
-        return pulumi.get(self, "include_reference_token")
+        return pulumi.get(self, "includes_pattern")
 
-    @include_reference_token.setter
-    def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "include_reference_token", value)
+    @includes_pattern.setter
+    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "includes_pattern", value)
 
     @property
     @pulumi.getter
-    def refreshable(self) -> Optional[pulumi.Input[bool]]:
+    def notes(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Is this token refreshable? Defaults to `false`
+        Internal description.
         """
-        return pulumi.get(self, "refreshable")
+        return pulumi.get(self, "notes")
 
-    @refreshable.setter
-    def refreshable(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "refreshable", value)
+    @notes.setter
+    def notes(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "notes", value)
 
     @property
-    @pulumi.getter
-    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="projectEnvironments")
+    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        """
+        return pulumi.get(self, "project_environments")
+
+    @project_environments.setter
+    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "project_environments", value)
+
+    @property
+    @pulumi.getter(name="projectKey")
+    def project_key(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         """
-        return pulumi.get(self, "scopes")
+        return pulumi.get(self, "project_key")
 
-    @scopes.setter
-    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "scopes", value)
+    @project_key.setter
+    def project_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_key", value)
+
+    @property
+    @pulumi.getter(name="repoLayoutRef")
+    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
+        """
+        Repository layout key for the local repository
+        """
+        return pulumi.get(self, "repo_layout_ref")
+
+    @repo_layout_ref.setter
+    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo_layout_ref", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
+    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        The effective list of actual repositories included in this virtual repository.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "repositories")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @repositories.setter
+    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "repositories", value)
 
 
 @pulumi.input_type
-class _ScopedTokenState:
+class _VirtualPuppetRepositoryState:
     def __init__(__self__, *,
-                 access_token: Optional[pulumi.Input[str]] = None,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 expiry: Optional[pulumi.Input[int]] = None,
-                 include_reference_token: Optional[pulumi.Input[bool]] = None,
-                 issued_at: Optional[pulumi.Input[int]] = None,
-                 issuer: Optional[pulumi.Input[str]] = None,
-                 reference_token: Optional[pulumi.Input[str]] = None,
-                 refresh_token: Optional[pulumi.Input[str]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 subject: Optional[pulumi.Input[str]] = None,
-                 token_type: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering ScopedToken resources.
-        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[int] expiry: Returns the token expiry
-        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
-        :param pulumi.Input[int] issued_at: Returns the token issued at date/time
-        :param pulumi.Input[str] issuer: Returns the token issuer
-        :param pulumi.Input[str] reference_token: Returns the reference token to authenticate to Artifactory
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] subject: Returns the token type
-        :param pulumi.Input[str] token_type: Returns the token type
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
-        """
-        if access_token is not None:
-            pulumi.set(__self__, "access_token", access_token)
-        if audiences is not None:
-            pulumi.set(__self__, "audiences", audiences)
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 package_type: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        Input properties used for looking up and filtering VirtualPuppetRepository resources.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        """
+        if artifactory_requests_can_retrieve_remote_artifacts is not None:
+            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
+        if default_deployment_repo is not None:
+            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if expires_in is not None:
-            pulumi.set(__self__, "expires_in", expires_in)
-        if expiry is not None:
-            pulumi.set(__self__, "expiry", expiry)
-        if include_reference_token is not None:
-            pulumi.set(__self__, "include_reference_token", include_reference_token)
-        if issued_at is not None:
-            pulumi.set(__self__, "issued_at", issued_at)
-        if issuer is not None:
-            pulumi.set(__self__, "issuer", issuer)
-        if reference_token is not None:
-            pulumi.set(__self__, "reference_token", reference_token)
-        if refresh_token is not None:
-            pulumi.set(__self__, "refresh_token", refresh_token)
-        if refreshable is not None:
-            pulumi.set(__self__, "refreshable", refreshable)
-        if scopes is not None:
-            pulumi.set(__self__, "scopes", scopes)
-        if subject is not None:
-            pulumi.set(__self__, "subject", subject)
-        if token_type is not None:
-            pulumi.set(__self__, "token_type", token_type)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
-
-    @property
-    @pulumi.getter(name="accessToken")
-    def access_token(self) -> Optional[pulumi.Input[str]]:
-        """
-        Returns the access token to authenticate to Artifactory
-        """
-        return pulumi.get(self, "access_token")
-
-    @access_token.setter
-    def access_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "access_token", value)
-
-    @property
-    @pulumi.getter
-    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        """
-        return pulumi.get(self, "audiences")
-
-    @audiences.setter
-    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "audiences", value)
+        if excludes_pattern is not None:
+            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
+        if includes_pattern is not None:
+            pulumi.set(__self__, "includes_pattern", includes_pattern)
+        if key is not None:
+            pulumi.set(__self__, "key", key)
+        if notes is not None:
+            pulumi.set(__self__, "notes", notes)
+        if package_type is not None:
+            pulumi.set(__self__, "package_type", package_type)
+        if project_environments is not None:
+            pulumi.set(__self__, "project_environments", project_environments)
+        if project_key is not None:
+            pulumi.set(__self__, "project_key", project_key)
+        if repo_layout_ref is not None:
+            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
+        if repositories is not None:
+            pulumi.set(__self__, "repositories", repositories)
+
+    @property
+    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
+    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+        another Artifactory instance.
+        """
+        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
+
+    @artifactory_requests_can_retrieve_remote_artifacts.setter
+    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
+
+    @property
+    @pulumi.getter(name="defaultDeploymentRepo")
+    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default repository to deploy artifacts.
+        """
+        return pulumi.get(self, "default_deployment_repo")
+
+    @default_deployment_repo.setter
+    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_deployment_repo", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        Public description.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="expiresIn")
-    def expires_in(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="excludesPattern")
+    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+        artifacts are excluded.
         """
-        return pulumi.get(self, "expires_in")
+        return pulumi.get(self, "excludes_pattern")
 
-    @expires_in.setter
-    def expires_in(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expires_in", value)
+    @excludes_pattern.setter
+    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "excludes_pattern", value)
 
     @property
-    @pulumi.getter
-    def expiry(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="includesPattern")
+    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token expiry
+        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         """
-        return pulumi.get(self, "expiry")
+        return pulumi.get(self, "includes_pattern")
 
-    @expiry.setter
-    def expiry(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expiry", value)
-
-    @property
-    @pulumi.getter(name="includeReferenceToken")
-    def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (Optional) Should a reference token also be created? Defaults to `false`
-        """
-        return pulumi.get(self, "include_reference_token")
-
-    @include_reference_token.setter
-    def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "include_reference_token", value)
-
-    @property
-    @pulumi.getter(name="issuedAt")
-    def issued_at(self) -> Optional[pulumi.Input[int]]:
-        """
-        Returns the token issued at date/time
-        """
-        return pulumi.get(self, "issued_at")
-
-    @issued_at.setter
-    def issued_at(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "issued_at", value)
+    @includes_pattern.setter
+    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "includes_pattern", value)
 
     @property
     @pulumi.getter
-    def issuer(self) -> Optional[pulumi.Input[str]]:
+    def key(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token issuer
+        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+        contain spaces or special characters.
         """
-        return pulumi.get(self, "issuer")
+        return pulumi.get(self, "key")
 
-    @issuer.setter
-    def issuer(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "issuer", value)
+    @key.setter
+    def key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key", value)
 
     @property
-    @pulumi.getter(name="referenceToken")
-    def reference_token(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def notes(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the reference token to authenticate to Artifactory
+        Internal description.
         """
-        return pulumi.get(self, "reference_token")
+        return pulumi.get(self, "notes")
 
-    @reference_token.setter
-    def reference_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "reference_token", value)
+    @notes.setter
+    def notes(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "notes", value)
 
     @property
-    @pulumi.getter(name="refreshToken")
-    def refresh_token(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "refresh_token")
+    @pulumi.getter(name="packageType")
+    def package_type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "package_type")
 
-    @refresh_token.setter
-    def refresh_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "refresh_token", value)
+    @package_type.setter
+    def package_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "package_type", value)
 
     @property
-    @pulumi.getter
-    def refreshable(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="projectEnvironments")
+    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (Optional) Is this token refreshable? Defaults to `false`
+        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         """
-        return pulumi.get(self, "refreshable")
+        return pulumi.get(self, "project_environments")
 
-    @refreshable.setter
-    def refreshable(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "refreshable", value)
+    @project_environments.setter
+    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "project_environments", value)
 
     @property
-    @pulumi.getter
-    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="projectKey")
+    def project_key(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         """
-        return pulumi.get(self, "scopes")
+        return pulumi.get(self, "project_key")
 
-    @scopes.setter
-    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "scopes", value)
+    @project_key.setter
+    def project_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_key", value)
 
     @property
-    @pulumi.getter
-    def subject(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="repoLayoutRef")
+    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token type
+        Repository layout key for the local repository
         """
-        return pulumi.get(self, "subject")
+        return pulumi.get(self, "repo_layout_ref")
 
-    @subject.setter
-    def subject(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "subject", value)
-
-    @property
-    @pulumi.getter(name="tokenType")
-    def token_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Returns the token type
-        """
-        return pulumi.get(self, "token_type")
-
-    @token_type.setter
-    def token_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "token_type", value)
+    @repo_layout_ref.setter
+    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo_layout_ref", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
+    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        The effective list of actual repositories included in this virtual repository.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "repositories")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @repositories.setter
+    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "repositories", value)
 
 
-class ScopedToken(pulumi.CustomResource):
+class VirtualPuppetRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 include_reference_token: Optional[pulumi.Input[bool]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Provides an Artifactory Scoped Token resource. This can be used to create and manage Artifactory Scoped Tokens.
-
-        !>Scoped Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
-        state.
-
-        ~>Token would not be saved by Artifactory if `expires_in` is less than the persistency threshold value (default to 10800 seconds) set in Access configuration. See [Persistency Threshold](https://www.jfrog.com/confluence/display/JFROG/Access+Tokens#AccessTokens-PersistencyThreshold) for details.
+        Creates a virtual Puppet repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
 
         ## Example Usage
 
-        ### S
-        ### Create a new Artifactory scoped token for an existing user
-
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        scoped_token = artifactory.ScopedToken("scopedToken", username="existing-user")
+        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="foo-puppet",
+            notes="Internal description",
+            repositories=[])
         ```
 
-        **Note:** This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
-        ### Create a new Artifactory user and scoped token
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        new_user = artifactory.User("newUser",
-            email="new_user@somewhere.com",
-            groups=["readers"])
-        scoped_token_user = artifactory.ScopedToken("scopedTokenUser", username=new_user.name)
-        ```
-        ### Creates a new token for groups
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        scoped_token_group = artifactory.ScopedToken("scopedTokenGroup", scopes=["applied-permissions/groups:readers"])
-        ```
-        ### Create token with expiry
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        scoped_token_no_expiry = artifactory.ScopedToken("scopedTokenNoExpiry",
-            expires_in=7200,
-            username="existing-user")
-        ```
-        ### Creates a refreshable token
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        scoped_token_refreshable = artifactory.ScopedToken("scopedTokenRefreshable",
-            refreshable=True,
-            username="existing-user")
-        ```
-        ### Creates an administrator token
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
+        ## Import
 
-        admin = artifactory.ScopedToken("admin",
-            scopes=["applied-permissions/admin"],
-            username="admin-user")
-        ```
-        ### Creates a token with an audience
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
+        Virtual repositories can be imported using their name, e.g.
 
-        audience = artifactory.ScopedToken("audience",
-            audiences=["jfrt@*"],
-            scopes=["applied-permissions/admin"],
-            username="admin-user")
+        ```sh
+         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
         ```
-        ## References
-
-        - https://www.jfrog.com/confluence/display/JFROG/Access+Tokens
-        - https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-AccessTokens
-
-        ## Import
-
-        Artifactory **does not** retain scoped tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ScopedTokenArgs] = None,
+                 args: VirtualPuppetRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides an Artifactory Scoped Token resource. This can be used to create and manage Artifactory Scoped Tokens.
-
-        !>Scoped Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
-        state.
-
-        ~>Token would not be saved by Artifactory if `expires_in` is less than the persistency threshold value (default to 10800 seconds) set in Access configuration. See [Persistency Threshold](https://www.jfrog.com/confluence/display/JFROG/Access+Tokens#AccessTokens-PersistencyThreshold) for details.
+        Creates a virtual Puppet repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
 
         ## Example Usage
 
-        ### S
-        ### Create a new Artifactory scoped token for an existing user
-
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        scoped_token = artifactory.ScopedToken("scopedToken", username="existing-user")
+        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="foo-puppet",
+            notes="Internal description",
+            repositories=[])
         ```
 
-        **Note:** This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
-        ### Create a new Artifactory user and scoped token
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        new_user = artifactory.User("newUser",
-            email="new_user@somewhere.com",
-            groups=["readers"])
-        scoped_token_user = artifactory.ScopedToken("scopedTokenUser", username=new_user.name)
-        ```
-        ### Creates a new token for groups
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        scoped_token_group = artifactory.ScopedToken("scopedTokenGroup", scopes=["applied-permissions/groups:readers"])
-        ```
-        ### Create token with expiry
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        scoped_token_no_expiry = artifactory.ScopedToken("scopedTokenNoExpiry",
-            expires_in=7200,
-            username="existing-user")
-        ```
-        ### Creates a refreshable token
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        scoped_token_refreshable = artifactory.ScopedToken("scopedTokenRefreshable",
-            refreshable=True,
-            username="existing-user")
-        ```
-        ### Creates an administrator token
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
+        ## Import
 
-        admin = artifactory.ScopedToken("admin",
-            scopes=["applied-permissions/admin"],
-            username="admin-user")
-        ```
-        ### Creates a token with an audience
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
+        Virtual repositories can be imported using their name, e.g.
 
-        audience = artifactory.ScopedToken("audience",
-            audiences=["jfrt@*"],
-            scopes=["applied-permissions/admin"],
-            username="admin-user")
+        ```sh
+         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
         ```
-        ## References
-
-        - https://www.jfrog.com/confluence/display/JFROG/Access+Tokens
-        - https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-AccessTokens
-
-        ## Import
-
-        Artifactory **does not** retain scoped tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
-        :param ScopedTokenArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualPuppetRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ScopedTokenArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualPuppetRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 include_reference_token: Optional[pulumi.Input[bool]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ScopedTokenArgs.__new__(ScopedTokenArgs)
+            __props__ = VirtualPuppetRepositoryArgs.__new__(VirtualPuppetRepositoryArgs)
 
-            __props__.__dict__["audiences"] = audiences
+            __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
+            __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
-            __props__.__dict__["expires_in"] = expires_in
-            __props__.__dict__["include_reference_token"] = include_reference_token
-            __props__.__dict__["refreshable"] = refreshable
-            __props__.__dict__["scopes"] = scopes
-            __props__.__dict__["username"] = username
-            __props__.__dict__["access_token"] = None
-            __props__.__dict__["expiry"] = None
-            __props__.__dict__["issued_at"] = None
-            __props__.__dict__["issuer"] = None
-            __props__.__dict__["reference_token"] = None
-            __props__.__dict__["refresh_token"] = None
-            __props__.__dict__["subject"] = None
-            __props__.__dict__["token_type"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "referenceToken", "refreshToken"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(ScopedToken, __self__).__init__(
-            'artifactory:index/scopedToken:ScopedToken',
+            __props__.__dict__["excludes_pattern"] = excludes_pattern
+            __props__.__dict__["includes_pattern"] = includes_pattern
+            if key is None and not opts.urn:
+                raise TypeError("Missing required property 'key'")
+            __props__.__dict__["key"] = key
+            __props__.__dict__["notes"] = notes
+            __props__.__dict__["project_environments"] = project_environments
+            __props__.__dict__["project_key"] = project_key
+            __props__.__dict__["repo_layout_ref"] = repo_layout_ref
+            __props__.__dict__["repositories"] = repositories
+            __props__.__dict__["package_type"] = None
+        super(VirtualPuppetRepository, __self__).__init__(
+            'artifactory:index/virtualPuppetRepository:VirtualPuppetRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            access_token: Optional[pulumi.Input[str]] = None,
-            audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+            default_deployment_repo: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            expires_in: Optional[pulumi.Input[int]] = None,
-            expiry: Optional[pulumi.Input[int]] = None,
-            include_reference_token: Optional[pulumi.Input[bool]] = None,
-            issued_at: Optional[pulumi.Input[int]] = None,
-            issuer: Optional[pulumi.Input[str]] = None,
-            reference_token: Optional[pulumi.Input[str]] = None,
-            refresh_token: Optional[pulumi.Input[str]] = None,
-            refreshable: Optional[pulumi.Input[bool]] = None,
-            scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            subject: Optional[pulumi.Input[str]] = None,
-            token_type: Optional[pulumi.Input[str]] = None,
-            username: Optional[pulumi.Input[str]] = None) -> 'ScopedToken':
+            excludes_pattern: Optional[pulumi.Input[str]] = None,
+            includes_pattern: Optional[pulumi.Input[str]] = None,
+            key: Optional[pulumi.Input[str]] = None,
+            notes: Optional[pulumi.Input[str]] = None,
+            package_type: Optional[pulumi.Input[str]] = None,
+            project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            project_key: Optional[pulumi.Input[str]] = None,
+            repo_layout_ref: Optional[pulumi.Input[str]] = None,
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualPuppetRepository':
         """
-        Get an existing ScopedToken resource's state with the given name, id, and optional extra
+        Get an existing VirtualPuppetRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[int] expiry: Returns the token expiry
-        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
-        :param pulumi.Input[int] issued_at: Returns the token issued at date/time
-        :param pulumi.Input[str] issuer: Returns the token issuer
-        :param pulumi.Input[str] reference_token: Returns the reference token to authenticate to Artifactory
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] subject: Returns the token type
-        :param pulumi.Input[str] token_type: Returns the token type
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ScopedTokenState.__new__(_ScopedTokenState)
+        __props__ = _VirtualPuppetRepositoryState.__new__(_VirtualPuppetRepositoryState)
 
-        __props__.__dict__["access_token"] = access_token
-        __props__.__dict__["audiences"] = audiences
+        __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
+        __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
-        __props__.__dict__["expires_in"] = expires_in
-        __props__.__dict__["expiry"] = expiry
-        __props__.__dict__["include_reference_token"] = include_reference_token
-        __props__.__dict__["issued_at"] = issued_at
-        __props__.__dict__["issuer"] = issuer
-        __props__.__dict__["reference_token"] = reference_token
-        __props__.__dict__["refresh_token"] = refresh_token
-        __props__.__dict__["refreshable"] = refreshable
-        __props__.__dict__["scopes"] = scopes
-        __props__.__dict__["subject"] = subject
-        __props__.__dict__["token_type"] = token_type
-        __props__.__dict__["username"] = username
-        return ScopedToken(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["excludes_pattern"] = excludes_pattern
+        __props__.__dict__["includes_pattern"] = includes_pattern
+        __props__.__dict__["key"] = key
+        __props__.__dict__["notes"] = notes
+        __props__.__dict__["package_type"] = package_type
+        __props__.__dict__["project_environments"] = project_environments
+        __props__.__dict__["project_key"] = project_key
+        __props__.__dict__["repo_layout_ref"] = repo_layout_ref
+        __props__.__dict__["repositories"] = repositories
+        return VirtualPuppetRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="accessToken")
-    def access_token(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
+    def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
-        Returns the access token to authenticate to Artifactory
+        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+        another Artifactory instance.
         """
-        return pulumi.get(self, "access_token")
+        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
 
     @property
-    @pulumi.getter
-    def audiences(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter(name="defaultDeploymentRepo")
+    def default_deployment_repo(self) -> pulumi.Output[Optional[str]]:
         """
-        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        Default repository to deploy artifacts.
         """
-        return pulumi.get(self, "audiences")
+        return pulumi.get(self, "default_deployment_repo")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        Public description.
         """
         return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="expiresIn")
-    def expires_in(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="excludesPattern")
+    def excludes_pattern(self) -> pulumi.Output[Optional[str]]:
         """
-        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+        artifacts are excluded.
         """
-        return pulumi.get(self, "expires_in")
+        return pulumi.get(self, "excludes_pattern")
 
     @property
-    @pulumi.getter
-    def expiry(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="includesPattern")
+    def includes_pattern(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the token expiry
+        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         """
-        return pulumi.get(self, "expiry")
-
-    @property
-    @pulumi.getter(name="includeReferenceToken")
-    def include_reference_token(self) -> pulumi.Output[Optional[bool]]:
-        """
-        (Optional) Should a reference token also be created? Defaults to `false`
-        """
-        return pulumi.get(self, "include_reference_token")
-
-    @property
-    @pulumi.getter(name="issuedAt")
-    def issued_at(self) -> pulumi.Output[int]:
-        """
-        Returns the token issued at date/time
-        """
-        return pulumi.get(self, "issued_at")
+        return pulumi.get(self, "includes_pattern")
 
     @property
     @pulumi.getter
-    def issuer(self) -> pulumi.Output[str]:
+    def key(self) -> pulumi.Output[str]:
         """
-        Returns the token issuer
+        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+        contain spaces or special characters.
         """
-        return pulumi.get(self, "issuer")
+        return pulumi.get(self, "key")
 
     @property
-    @pulumi.getter(name="referenceToken")
-    def reference_token(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def notes(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the reference token to authenticate to Artifactory
+        Internal description.
         """
-        return pulumi.get(self, "reference_token")
-
-    @property
-    @pulumi.getter(name="refreshToken")
-    def refresh_token(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "refresh_token")
+        return pulumi.get(self, "notes")
 
     @property
-    @pulumi.getter
-    def refreshable(self) -> pulumi.Output[Optional[bool]]:
-        """
-        (Optional) Is this token refreshable? Defaults to `false`
-        """
-        return pulumi.get(self, "refreshable")
+    @pulumi.getter(name="packageType")
+    def package_type(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "package_type")
 
     @property
-    @pulumi.getter
-    def scopes(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="projectEnvironments")
+    def project_environments(self) -> pulumi.Output[Sequence[str]]:
         """
-        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         """
-        return pulumi.get(self, "scopes")
+        return pulumi.get(self, "project_environments")
 
     @property
-    @pulumi.getter
-    def subject(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="projectKey")
+    def project_key(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the token type
+        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         """
-        return pulumi.get(self, "subject")
+        return pulumi.get(self, "project_key")
 
     @property
-    @pulumi.getter(name="tokenType")
-    def token_type(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="repoLayoutRef")
+    def repo_layout_ref(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the token type
+        Repository layout key for the local repository
         """
-        return pulumi.get(self, "token_type")
+        return pulumi.get(self, "repo_layout_ref")
 
     @property
     @pulumi.getter
-    def username(self) -> pulumi.Output[Optional[str]]:
+    def repositories(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        The effective list of actual repositories included in this virtual repository.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "repositories")
```

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/single_replication_config.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/single_replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/unmanaged_user.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/unmanaged_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/user.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_alpine_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_bower_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_chef_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_composer_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_conan_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_conda_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_cran_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_debian_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_docker_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_gems_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_generic_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_gitlfs_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_gradle_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_helm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_ivy_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_npm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_nuget_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_p2_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_pub_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_puppet_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_swift_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualPuppetRepositoryArgs', 'VirtualPuppetRepository']
+__all__ = ['VirtualSwiftRepositoryArgs', 'VirtualSwiftRepository']
 
 @pulumi.input_type
-class VirtualPuppetRepositoryArgs:
+class VirtualSwiftRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a VirtualPuppetRepository resource.
+        The set of arguments for constructing a VirtualSwiftRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -207,30 +207,30 @@
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
 @pulumi.input_type
-class _VirtualPuppetRepositoryState:
+class _VirtualSwiftRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering VirtualPuppetRepository resources.
+        Input properties used for looking up and filtering VirtualSwiftRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -418,15 +418,15 @@
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
-class VirtualPuppetRepository(pulumi.CustomResource):
+class VirtualSwiftRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -436,38 +436,23 @@
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Creates a virtual Puppet repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-puppet",
-            notes="Internal description",
-            repositories=[])
-        ```
+        Creates a virtual Swift repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
+         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -488,50 +473,35 @@
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualPuppetRepositoryArgs,
+                 args: VirtualSwiftRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Puppet repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-puppet",
-            notes="Internal description",
-            repositories=[])
-        ```
+        Creates a virtual Swift repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
+         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualPuppetRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualSwiftRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualPuppetRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualSwiftRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -550,15 +520,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualPuppetRepositoryArgs.__new__(VirtualPuppetRepositoryArgs)
+            __props__ = VirtualSwiftRepositoryArgs.__new__(VirtualSwiftRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -566,16 +536,16 @@
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["package_type"] = None
-        super(VirtualPuppetRepository, __self__).__init__(
-            'artifactory:index/virtualPuppetRepository:VirtualPuppetRepository',
+        super(VirtualSwiftRepository, __self__).__init__(
+            'artifactory:index/virtualSwiftRepository:VirtualSwiftRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -587,17 +557,17 @@
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualPuppetRepository':
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualSwiftRepository':
         """
-        Get an existing VirtualPuppetRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualSwiftRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -617,29 +587,29 @@
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualPuppetRepositoryState.__new__(_VirtualPuppetRepositoryState)
+        __props__ = _VirtualSwiftRepositoryState.__new__(_VirtualSwiftRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
-        return VirtualPuppetRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualSwiftRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_pypi_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_rpm_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_sbt_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_swift_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/virtual_terraform_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualSwiftRepositoryArgs', 'VirtualSwiftRepository']
+__all__ = ['VirtualTerraformRepositoryArgs', 'VirtualTerraformRepository']
 
 @pulumi.input_type
-class VirtualSwiftRepositoryArgs:
+class VirtualTerraformRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a VirtualSwiftRepository resource.
+        The set of arguments for constructing a VirtualTerraformRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -207,30 +207,30 @@
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
 @pulumi.input_type
-class _VirtualSwiftRepositoryState:
+class _VirtualTerraformRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering VirtualSwiftRepository resources.
+        Input properties used for looking up and filtering VirtualTerraformRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -418,15 +418,15 @@
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
-class VirtualSwiftRepository(pulumi.CustomResource):
+class VirtualTerraformRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -436,23 +436,35 @@
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Creates a virtual Swift repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="terraform-remote",
+            notes="Internal description",
+            repositories=[])
+        ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
+         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -473,35 +485,47 @@
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualSwiftRepositoryArgs,
+                 args: VirtualTerraformRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Swift repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="terraform-remote",
+            notes="Internal description",
+            repositories=[])
+        ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
+         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualSwiftRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualTerraformRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualSwiftRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualTerraformRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -520,15 +544,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualSwiftRepositoryArgs.__new__(VirtualSwiftRepositoryArgs)
+            __props__ = VirtualTerraformRepositoryArgs.__new__(VirtualTerraformRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -536,16 +560,16 @@
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["package_type"] = None
-        super(VirtualSwiftRepository, __self__).__init__(
-            'artifactory:index/virtualSwiftRepository:VirtualSwiftRepository',
+        super(VirtualTerraformRepository, __self__).__init__(
+            'artifactory:index/virtualTerraformRepository:VirtualTerraformRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -557,17 +581,17 @@
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualSwiftRepository':
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualTerraformRepository':
         """
-        Get an existing VirtualSwiftRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualTerraformRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -587,29 +611,29 @@
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualSwiftRepositoryState.__new__(_VirtualSwiftRepositoryState)
+        __props__ = _VirtualTerraformRepositoryState.__new__(_VirtualTerraformRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
-        return VirtualSwiftRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualTerraformRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory/virtual_terraform_repository.py` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory/scoped_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,730 +5,817 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualTerraformRepositoryArgs', 'VirtualTerraformRepository']
+__all__ = ['ScopedTokenArgs', 'ScopedToken']
 
 @pulumi.input_type
-class VirtualTerraformRepositoryArgs:
+class ScopedTokenArgs:
     def __init__(__self__, *,
-                 key: pulumi.Input[str],
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        The set of arguments for constructing a VirtualTerraformRepository resource.
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        """
-        pulumi.set(__self__, "key", key)
-        if artifactory_requests_can_retrieve_remote_artifacts is not None:
-            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
-        if default_deployment_repo is not None:
-            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 grant_type: Optional[pulumi.Input[str]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a ScopedToken resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
+        :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
+        :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+               The supported scopes include:
+        :param pulumi.Input[str] username: The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
+        """
+        if audiences is not None:
+            pulumi.set(__self__, "audiences", audiences)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if excludes_pattern is not None:
-            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
-        if includes_pattern is not None:
-            pulumi.set(__self__, "includes_pattern", includes_pattern)
-        if notes is not None:
-            pulumi.set(__self__, "notes", notes)
-        if project_environments is not None:
-            pulumi.set(__self__, "project_environments", project_environments)
-        if project_key is not None:
-            pulumi.set(__self__, "project_key", project_key)
-        if repo_layout_ref is not None:
-            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
-        if repositories is not None:
-            pulumi.set(__self__, "repositories", repositories)
+        if expires_in is not None:
+            pulumi.set(__self__, "expires_in", expires_in)
+        if grant_type is not None:
+            pulumi.set(__self__, "grant_type", grant_type)
+        if include_reference_token is not None:
+            pulumi.set(__self__, "include_reference_token", include_reference_token)
+        if refreshable is not None:
+            pulumi.set(__self__, "refreshable", refreshable)
+        if scopes is not None:
+            pulumi.set(__self__, "scopes", scopes)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
-    def key(self) -> pulumi.Input[str]:
-        """
-        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-        contain spaces or special characters.
-        """
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: pulumi.Input[str]):
-        pulumi.set(self, "key", value)
-
-    @property
-    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
-    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-        another Artifactory instance.
-        """
-        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
-
-    @artifactory_requests_can_retrieve_remote_artifacts.setter
-    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
-
-    @property
-    @pulumi.getter(name="defaultDeploymentRepo")
-    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
-        """
-        Default repository to deploy artifacts.
-        """
-        return pulumi.get(self, "default_deployment_repo")
-
-    @default_deployment_repo.setter
-    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_deployment_repo", value)
+    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
+        """
+        return pulumi.get(self, "audiences")
+
+    @audiences.setter
+    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "audiences", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Public description.
+        Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="excludesPattern")
-    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="expiresIn")
+    def expires_in(self) -> Optional[pulumi.Input[int]]:
         """
-        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-        artifacts are excluded.
+        The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
         """
-        return pulumi.get(self, "excludes_pattern")
+        return pulumi.get(self, "expires_in")
 
-    @excludes_pattern.setter
-    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "excludes_pattern", value)
+    @expires_in.setter
+    def expires_in(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "expires_in", value)
 
     @property
-    @pulumi.getter(name="includesPattern")
-    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="grantType")
+    def grant_type(self) -> Optional[pulumi.Input[str]]:
         """
-        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
         """
-        return pulumi.get(self, "includes_pattern")
+        return pulumi.get(self, "grant_type")
 
-    @includes_pattern.setter
-    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "includes_pattern", value)
+    @grant_type.setter
+    def grant_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "grant_type", value)
 
     @property
-    @pulumi.getter
-    def notes(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="includeReferenceToken")
+    def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
         """
-        Internal description.
+        Also create a reference token which can be used like an API key. Default is `false`.
         """
-        return pulumi.get(self, "notes")
+        return pulumi.get(self, "include_reference_token")
 
-    @notes.setter
-    def notes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "notes", value)
+    @include_reference_token.setter
+    def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "include_reference_token", value)
 
     @property
-    @pulumi.getter(name="projectEnvironments")
-    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        """
-        return pulumi.get(self, "project_environments")
-
-    @project_environments.setter
-    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "project_environments", value)
-
-    @property
-    @pulumi.getter(name="projectKey")
-    def project_key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def refreshable(self) -> Optional[pulumi.Input[bool]]:
         """
-        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        Is this token refreshable? Default is `false`.
         """
-        return pulumi.get(self, "project_key")
+        return pulumi.get(self, "refreshable")
 
-    @project_key.setter
-    def project_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_key", value)
+    @refreshable.setter
+    def refreshable(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "refreshable", value)
 
     @property
-    @pulumi.getter(name="repoLayoutRef")
-    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Repository layout key for the local repository
+        The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        The supported scopes include:
         """
-        return pulumi.get(self, "repo_layout_ref")
+        return pulumi.get(self, "scopes")
 
-    @repo_layout_ref.setter
-    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "repo_layout_ref", value)
+    @scopes.setter
+    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "scopes", value)
 
     @property
     @pulumi.getter
-    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The effective list of actual repositories included in this virtual repository.
+        The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
         """
-        return pulumi.get(self, "repositories")
+        return pulumi.get(self, "username")
 
-    @repositories.setter
-    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "repositories", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
-class _VirtualTerraformRepositoryState:
+class _ScopedTokenState:
     def __init__(__self__, *,
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 access_token: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 package_type: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        Input properties used for looking up and filtering VirtualTerraformRepository resources.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        """
-        if artifactory_requests_can_retrieve_remote_artifacts is not None:
-            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
-        if default_deployment_repo is not None:
-            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 expiry: Optional[pulumi.Input[int]] = None,
+                 grant_type: Optional[pulumi.Input[str]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 issued_at: Optional[pulumi.Input[int]] = None,
+                 issuer: Optional[pulumi.Input[str]] = None,
+                 reference_token: Optional[pulumi.Input[str]] = None,
+                 refresh_token: Optional[pulumi.Input[str]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 subject: Optional[pulumi.Input[str]] = None,
+                 token_type: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering ScopedToken resources.
+        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
+        :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
+        :param pulumi.Input[int] expiry: Returns the token expiry.
+        :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[int] issued_at: Returns the token issued at date/time.
+        :param pulumi.Input[str] issuer: Returns the token issuer.
+        :param pulumi.Input[str] reference_token: Reference Token (alias to Access Token).
+        :param pulumi.Input[str] refresh_token: Refresh token.
+        :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+               The supported scopes include:
+        :param pulumi.Input[str] subject: Returns the token type.
+        :param pulumi.Input[str] token_type: Returns the token type.
+        :param pulumi.Input[str] username: The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
+        """
+        if access_token is not None:
+            pulumi.set(__self__, "access_token", access_token)
+        if audiences is not None:
+            pulumi.set(__self__, "audiences", audiences)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if excludes_pattern is not None:
-            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
-        if includes_pattern is not None:
-            pulumi.set(__self__, "includes_pattern", includes_pattern)
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if notes is not None:
-            pulumi.set(__self__, "notes", notes)
-        if package_type is not None:
-            pulumi.set(__self__, "package_type", package_type)
-        if project_environments is not None:
-            pulumi.set(__self__, "project_environments", project_environments)
-        if project_key is not None:
-            pulumi.set(__self__, "project_key", project_key)
-        if repo_layout_ref is not None:
-            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
-        if repositories is not None:
-            pulumi.set(__self__, "repositories", repositories)
-
-    @property
-    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
-    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-        another Artifactory instance.
-        """
-        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
-
-    @artifactory_requests_can_retrieve_remote_artifacts.setter
-    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
-
-    @property
-    @pulumi.getter(name="defaultDeploymentRepo")
-    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
-        """
-        Default repository to deploy artifacts.
-        """
-        return pulumi.get(self, "default_deployment_repo")
-
-    @default_deployment_repo.setter
-    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_deployment_repo", value)
+        if expires_in is not None:
+            pulumi.set(__self__, "expires_in", expires_in)
+        if expiry is not None:
+            pulumi.set(__self__, "expiry", expiry)
+        if grant_type is not None:
+            pulumi.set(__self__, "grant_type", grant_type)
+        if include_reference_token is not None:
+            pulumi.set(__self__, "include_reference_token", include_reference_token)
+        if issued_at is not None:
+            pulumi.set(__self__, "issued_at", issued_at)
+        if issuer is not None:
+            pulumi.set(__self__, "issuer", issuer)
+        if reference_token is not None:
+            pulumi.set(__self__, "reference_token", reference_token)
+        if refresh_token is not None:
+            pulumi.set(__self__, "refresh_token", refresh_token)
+        if refreshable is not None:
+            pulumi.set(__self__, "refreshable", refreshable)
+        if scopes is not None:
+            pulumi.set(__self__, "scopes", scopes)
+        if subject is not None:
+            pulumi.set(__self__, "subject", subject)
+        if token_type is not None:
+            pulumi.set(__self__, "token_type", token_type)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="accessToken")
+    def access_token(self) -> Optional[pulumi.Input[str]]:
+        """
+        Returns the access token to authenticate to Artifactory.
+        """
+        return pulumi.get(self, "access_token")
+
+    @access_token.setter
+    def access_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "access_token", value)
+
+    @property
+    @pulumi.getter
+    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
+        """
+        return pulumi.get(self, "audiences")
+
+    @audiences.setter
+    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "audiences", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Public description.
+        Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="excludesPattern")
-    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="expiresIn")
+    def expires_in(self) -> Optional[pulumi.Input[int]]:
         """
-        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-        artifacts are excluded.
+        The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
         """
-        return pulumi.get(self, "excludes_pattern")
+        return pulumi.get(self, "expires_in")
 
-    @excludes_pattern.setter
-    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "excludes_pattern", value)
+    @expires_in.setter
+    def expires_in(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "expires_in", value)
 
     @property
-    @pulumi.getter(name="includesPattern")
-    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def expiry(self) -> Optional[pulumi.Input[int]]:
         """
-        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        Returns the token expiry.
         """
-        return pulumi.get(self, "includes_pattern")
+        return pulumi.get(self, "expiry")
 
-    @includes_pattern.setter
-    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "includes_pattern", value)
+    @expiry.setter
+    def expiry(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "expiry", value)
 
     @property
-    @pulumi.getter
-    def key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="grantType")
+    def grant_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
+        """
+        return pulumi.get(self, "grant_type")
+
+    @grant_type.setter
+    def grant_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "grant_type", value)
+
+    @property
+    @pulumi.getter(name="includeReferenceToken")
+    def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Also create a reference token which can be used like an API key. Default is `false`.
         """
-        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-        contain spaces or special characters.
+        return pulumi.get(self, "include_reference_token")
+
+    @include_reference_token.setter
+    def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "include_reference_token", value)
+
+    @property
+    @pulumi.getter(name="issuedAt")
+    def issued_at(self) -> Optional[pulumi.Input[int]]:
         """
-        return pulumi.get(self, "key")
+        Returns the token issued at date/time.
+        """
+        return pulumi.get(self, "issued_at")
 
-    @key.setter
-    def key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key", value)
+    @issued_at.setter
+    def issued_at(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "issued_at", value)
 
     @property
     @pulumi.getter
-    def notes(self) -> Optional[pulumi.Input[str]]:
+    def issuer(self) -> Optional[pulumi.Input[str]]:
+        """
+        Returns the token issuer.
+        """
+        return pulumi.get(self, "issuer")
+
+    @issuer.setter
+    def issuer(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "issuer", value)
+
+    @property
+    @pulumi.getter(name="referenceToken")
+    def reference_token(self) -> Optional[pulumi.Input[str]]:
+        """
+        Reference Token (alias to Access Token).
+        """
+        return pulumi.get(self, "reference_token")
+
+    @reference_token.setter
+    def reference_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "reference_token", value)
+
+    @property
+    @pulumi.getter(name="refreshToken")
+    def refresh_token(self) -> Optional[pulumi.Input[str]]:
         """
-        Internal description.
+        Refresh token.
         """
-        return pulumi.get(self, "notes")
+        return pulumi.get(self, "refresh_token")
 
-    @notes.setter
-    def notes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "notes", value)
+    @refresh_token.setter
+    def refresh_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "refresh_token", value)
 
     @property
-    @pulumi.getter(name="packageType")
-    def package_type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "package_type")
+    @pulumi.getter
+    def refreshable(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Is this token refreshable? Default is `false`.
+        """
+        return pulumi.get(self, "refreshable")
 
-    @package_type.setter
-    def package_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "package_type", value)
+    @refreshable.setter
+    def refreshable(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "refreshable", value)
 
     @property
-    @pulumi.getter(name="projectEnvironments")
-    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        The supported scopes include:
         """
-        return pulumi.get(self, "project_environments")
+        return pulumi.get(self, "scopes")
 
-    @project_environments.setter
-    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "project_environments", value)
+    @scopes.setter
+    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "scopes", value)
 
     @property
-    @pulumi.getter(name="projectKey")
-    def project_key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def subject(self) -> Optional[pulumi.Input[str]]:
         """
-        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        Returns the token type.
         """
-        return pulumi.get(self, "project_key")
+        return pulumi.get(self, "subject")
 
-    @project_key.setter
-    def project_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_key", value)
+    @subject.setter
+    def subject(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subject", value)
 
     @property
-    @pulumi.getter(name="repoLayoutRef")
-    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="tokenType")
+    def token_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Repository layout key for the local repository
+        Returns the token type.
         """
-        return pulumi.get(self, "repo_layout_ref")
+        return pulumi.get(self, "token_type")
 
-    @repo_layout_ref.setter
-    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "repo_layout_ref", value)
+    @token_type.setter
+    def token_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token_type", value)
 
     @property
     @pulumi.getter
-    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The effective list of actual repositories included in this virtual repository.
+        The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
         """
-        return pulumi.get(self, "repositories")
+        return pulumi.get(self, "username")
 
-    @repositories.setter
-    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "repositories", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
 
-class VirtualTerraformRepository(pulumi.CustomResource):
+class ScopedToken(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 grant_type: Optional[pulumi.Input[str]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Provides an Artifactory Scoped Token resource. This can be used to create and manage Artifactory Scoped Tokens.
+
+        !>Scoped Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
+        state.
+
+        ~>Token would not be saved by Artifactory if `expires_in` is less than the persistency threshold value (default to 10800 seconds) set in Access configuration. See [Persistency Threshold](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
+
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="terraform-remote",
-            notes="Internal description",
-            repositories=[])
-        ```
+        ### Create a new Artifactory scoped token for an existing user
 
-        ## Import
+        resource "artifactory_scoped_token" "scoped_token" {
+          username = "existing-user"
+        }
+
+        ### **Note:** This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
+
+        ### Create a new Artifactory user and scoped token
+        resource "artifactory_user" "new_user" {
+          name   = "new_user"
+          email  = "new_user@somewhere.com"
+          groups = ["readers"]
+        }
+
+        resource "artifactory_scoped_token" "scoped_token_user" {
+          username = artifactory_user.new_user.name
+        }
+
+        ### Creates a new token for groups
+        resource "artifactory_scoped_token" "scoped_token_group" {
+          scopes = ["applied-permissions/groups:readers"]
+        }
+
+        ### Create token with expiry
+        resource "artifactory_scoped_token" "scoped_token_no_expiry" {
+          username   = "existing-user"
+          expires_in = 7200 // in seconds
+        }
+
+        ### Creates a refreshable token
+        resource "artifactory_scoped_token" "scoped_token_refreshable" {
+          username    = "existing-user"
+          refreshable = true
+        }
+
+        ### Creates an administrator token
+        resource "artifactory_scoped_token" "admin" {
+          username = "admin-user"
+          scopes   = ["applied-permissions/admin"]
+        }
+        ## References
+
+        - https://jfrog.com/help/r/jfrog-platform-administration-documentation/access-tokens
+        - https://jfrog.com/help/r/jfrog-rest-apis/access-tokens
 
-        Virtual repositories can be imported using their name, e.g.
+        ## Import
 
-        ```sh
-         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
-        ```
+        Artifactory **does not** retain scoped tokens, and they cannot be imported into state.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
+        :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
+        :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+               The supported scopes include:
+        :param pulumi.Input[str] username: The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualTerraformRepositoryArgs,
+                 args: Optional[ScopedTokenArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides an Artifactory Scoped Token resource. This can be used to create and manage Artifactory Scoped Tokens.
+
+        !>Scoped Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
+        state.
+
+        ~>Token would not be saved by Artifactory if `expires_in` is less than the persistency threshold value (default to 10800 seconds) set in Access configuration. See [Persistency Threshold](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
+
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="terraform-remote",
-            notes="Internal description",
-            repositories=[])
-        ```
+        ### Create a new Artifactory scoped token for an existing user
 
-        ## Import
+        resource "artifactory_scoped_token" "scoped_token" {
+          username = "existing-user"
+        }
+
+        ### **Note:** This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
+
+        ### Create a new Artifactory user and scoped token
+        resource "artifactory_user" "new_user" {
+          name   = "new_user"
+          email  = "new_user@somewhere.com"
+          groups = ["readers"]
+        }
+
+        resource "artifactory_scoped_token" "scoped_token_user" {
+          username = artifactory_user.new_user.name
+        }
+
+        ### Creates a new token for groups
+        resource "artifactory_scoped_token" "scoped_token_group" {
+          scopes = ["applied-permissions/groups:readers"]
+        }
+
+        ### Create token with expiry
+        resource "artifactory_scoped_token" "scoped_token_no_expiry" {
+          username   = "existing-user"
+          expires_in = 7200 // in seconds
+        }
+
+        ### Creates a refreshable token
+        resource "artifactory_scoped_token" "scoped_token_refreshable" {
+          username    = "existing-user"
+          refreshable = true
+        }
+
+        ### Creates an administrator token
+        resource "artifactory_scoped_token" "admin" {
+          username = "admin-user"
+          scopes   = ["applied-permissions/admin"]
+        }
+        ## References
+
+        - https://jfrog.com/help/r/jfrog-platform-administration-documentation/access-tokens
+        - https://jfrog.com/help/r/jfrog-rest-apis/access-tokens
 
-        Virtual repositories can be imported using their name, e.g.
+        ## Import
 
-        ```sh
-         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
-        ```
+        Artifactory **does not** retain scoped tokens, and they cannot be imported into state.
 
         :param str resource_name: The name of the resource.
-        :param VirtualTerraformRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param ScopedTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualTerraformRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ScopedTokenArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 grant_type: Optional[pulumi.Input[str]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualTerraformRepositoryArgs.__new__(VirtualTerraformRepositoryArgs)
+            __props__ = ScopedTokenArgs.__new__(ScopedTokenArgs)
 
-            __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
-            __props__.__dict__["default_deployment_repo"] = default_deployment_repo
+            __props__.__dict__["audiences"] = audiences
             __props__.__dict__["description"] = description
-            __props__.__dict__["excludes_pattern"] = excludes_pattern
-            __props__.__dict__["includes_pattern"] = includes_pattern
-            if key is None and not opts.urn:
-                raise TypeError("Missing required property 'key'")
-            __props__.__dict__["key"] = key
-            __props__.__dict__["notes"] = notes
-            __props__.__dict__["project_environments"] = project_environments
-            __props__.__dict__["project_key"] = project_key
-            __props__.__dict__["repo_layout_ref"] = repo_layout_ref
-            __props__.__dict__["repositories"] = repositories
-            __props__.__dict__["package_type"] = None
-        super(VirtualTerraformRepository, __self__).__init__(
-            'artifactory:index/virtualTerraformRepository:VirtualTerraformRepository',
+            __props__.__dict__["expires_in"] = expires_in
+            __props__.__dict__["grant_type"] = grant_type
+            __props__.__dict__["include_reference_token"] = include_reference_token
+            __props__.__dict__["refreshable"] = refreshable
+            __props__.__dict__["scopes"] = scopes
+            __props__.__dict__["username"] = username
+            __props__.__dict__["access_token"] = None
+            __props__.__dict__["expiry"] = None
+            __props__.__dict__["issued_at"] = None
+            __props__.__dict__["issuer"] = None
+            __props__.__dict__["reference_token"] = None
+            __props__.__dict__["refresh_token"] = None
+            __props__.__dict__["subject"] = None
+            __props__.__dict__["token_type"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "referenceToken", "refreshToken"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(ScopedToken, __self__).__init__(
+            'artifactory:index/scopedToken:ScopedToken',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-            default_deployment_repo: Optional[pulumi.Input[str]] = None,
+            access_token: Optional[pulumi.Input[str]] = None,
+            audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            excludes_pattern: Optional[pulumi.Input[str]] = None,
-            includes_pattern: Optional[pulumi.Input[str]] = None,
-            key: Optional[pulumi.Input[str]] = None,
-            notes: Optional[pulumi.Input[str]] = None,
-            package_type: Optional[pulumi.Input[str]] = None,
-            project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            project_key: Optional[pulumi.Input[str]] = None,
-            repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualTerraformRepository':
+            expires_in: Optional[pulumi.Input[int]] = None,
+            expiry: Optional[pulumi.Input[int]] = None,
+            grant_type: Optional[pulumi.Input[str]] = None,
+            include_reference_token: Optional[pulumi.Input[bool]] = None,
+            issued_at: Optional[pulumi.Input[int]] = None,
+            issuer: Optional[pulumi.Input[str]] = None,
+            reference_token: Optional[pulumi.Input[str]] = None,
+            refresh_token: Optional[pulumi.Input[str]] = None,
+            refreshable: Optional[pulumi.Input[bool]] = None,
+            scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            subject: Optional[pulumi.Input[str]] = None,
+            token_type: Optional[pulumi.Input[str]] = None,
+            username: Optional[pulumi.Input[str]] = None) -> 'ScopedToken':
         """
-        Get an existing VirtualTerraformRepository resource's state with the given name, id, and optional extra
+        Get an existing ScopedToken resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
+        :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
+        :param pulumi.Input[int] expiry: Returns the token expiry.
+        :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[int] issued_at: Returns the token issued at date/time.
+        :param pulumi.Input[str] issuer: Returns the token issuer.
+        :param pulumi.Input[str] reference_token: Reference Token (alias to Access Token).
+        :param pulumi.Input[str] refresh_token: Refresh token.
+        :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+               The supported scopes include:
+        :param pulumi.Input[str] subject: Returns the token type.
+        :param pulumi.Input[str] token_type: Returns the token type.
+        :param pulumi.Input[str] username: The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualTerraformRepositoryState.__new__(_VirtualTerraformRepositoryState)
+        __props__ = _ScopedTokenState.__new__(_ScopedTokenState)
 
-        __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
-        __props__.__dict__["default_deployment_repo"] = default_deployment_repo
+        __props__.__dict__["access_token"] = access_token
+        __props__.__dict__["audiences"] = audiences
         __props__.__dict__["description"] = description
-        __props__.__dict__["excludes_pattern"] = excludes_pattern
-        __props__.__dict__["includes_pattern"] = includes_pattern
-        __props__.__dict__["key"] = key
-        __props__.__dict__["notes"] = notes
-        __props__.__dict__["package_type"] = package_type
-        __props__.__dict__["project_environments"] = project_environments
-        __props__.__dict__["project_key"] = project_key
-        __props__.__dict__["repo_layout_ref"] = repo_layout_ref
-        __props__.__dict__["repositories"] = repositories
-        return VirtualTerraformRepository(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["expires_in"] = expires_in
+        __props__.__dict__["expiry"] = expiry
+        __props__.__dict__["grant_type"] = grant_type
+        __props__.__dict__["include_reference_token"] = include_reference_token
+        __props__.__dict__["issued_at"] = issued_at
+        __props__.__dict__["issuer"] = issuer
+        __props__.__dict__["reference_token"] = reference_token
+        __props__.__dict__["refresh_token"] = refresh_token
+        __props__.__dict__["refreshable"] = refreshable
+        __props__.__dict__["scopes"] = scopes
+        __props__.__dict__["subject"] = subject
+        __props__.__dict__["token_type"] = token_type
+        __props__.__dict__["username"] = username
+        return ScopedToken(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
-    def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="accessToken")
+    def access_token(self) -> pulumi.Output[str]:
         """
-        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-        another Artifactory instance.
+        Returns the access token to authenticate to Artifactory.
         """
-        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
+        return pulumi.get(self, "access_token")
 
     @property
-    @pulumi.getter(name="defaultDeploymentRepo")
-    def default_deployment_repo(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def audiences(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Default repository to deploy artifacts.
+        A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
         """
-        return pulumi.get(self, "default_deployment_repo")
+        return pulumi.get(self, "audiences")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Public description.
+        Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         """
         return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="excludesPattern")
-    def excludes_pattern(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="expiresIn")
+    def expires_in(self) -> pulumi.Output[int]:
+        """
+        The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
+        """
+        return pulumi.get(self, "expires_in")
+
+    @property
+    @pulumi.getter
+    def expiry(self) -> pulumi.Output[int]:
         """
-        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-        artifacts are excluded.
+        Returns the token expiry.
         """
-        return pulumi.get(self, "excludes_pattern")
+        return pulumi.get(self, "expiry")
 
     @property
-    @pulumi.getter(name="includesPattern")
-    def includes_pattern(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="grantType")
+    def grant_type(self) -> pulumi.Output[str]:
         """
-        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
         """
-        return pulumi.get(self, "includes_pattern")
+        return pulumi.get(self, "grant_type")
 
     @property
-    @pulumi.getter
-    def key(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="includeReferenceToken")
+    def include_reference_token(self) -> pulumi.Output[bool]:
         """
-        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-        contain spaces or special characters.
+        Also create a reference token which can be used like an API key. Default is `false`.
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "include_reference_token")
+
+    @property
+    @pulumi.getter(name="issuedAt")
+    def issued_at(self) -> pulumi.Output[int]:
+        """
+        Returns the token issued at date/time.
+        """
+        return pulumi.get(self, "issued_at")
 
     @property
     @pulumi.getter
-    def notes(self) -> pulumi.Output[Optional[str]]:
+    def issuer(self) -> pulumi.Output[str]:
+        """
+        Returns the token issuer.
+        """
+        return pulumi.get(self, "issuer")
+
+    @property
+    @pulumi.getter(name="referenceToken")
+    def reference_token(self) -> pulumi.Output[str]:
         """
-        Internal description.
+        Reference Token (alias to Access Token).
         """
-        return pulumi.get(self, "notes")
+        return pulumi.get(self, "reference_token")
 
     @property
-    @pulumi.getter(name="packageType")
-    def package_type(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "package_type")
+    @pulumi.getter(name="refreshToken")
+    def refresh_token(self) -> pulumi.Output[str]:
+        """
+        Refresh token.
+        """
+        return pulumi.get(self, "refresh_token")
 
     @property
-    @pulumi.getter(name="projectEnvironments")
-    def project_environments(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter
+    def refreshable(self) -> pulumi.Output[bool]:
         """
-        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        Is this token refreshable? Default is `false`.
         """
-        return pulumi.get(self, "project_environments")
+        return pulumi.get(self, "refreshable")
 
     @property
-    @pulumi.getter(name="projectKey")
-    def project_key(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def scopes(self) -> pulumi.Output[Sequence[str]]:
+        """
+        The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        The supported scopes include:
+        """
+        return pulumi.get(self, "scopes")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Output[str]:
         """
-        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        Returns the token type.
         """
-        return pulumi.get(self, "project_key")
+        return pulumi.get(self, "subject")
 
     @property
-    @pulumi.getter(name="repoLayoutRef")
-    def repo_layout_ref(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="tokenType")
+    def token_type(self) -> pulumi.Output[str]:
         """
-        Repository layout key for the local repository
+        Returns the token type.
         """
-        return pulumi.get(self, "repo_layout_ref")
+        return pulumi.get(self, "token_type")
 
     @property
     @pulumi.getter
-    def repositories(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def username(self) -> pulumi.Output[Optional[str]]:
         """
-        The effective list of actual repositories included in this virtual repository.
+        The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
         """
-        return pulumi.get(self, "repositories")
+        return pulumi.get(self, "username")
```

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/PKG-INFO` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-artifactory
-Version: 3.6.0a1685164706
+Version: 3.6.0a1685615210
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-3.6.0a1685164706/pulumi_artifactory.egg-info/SOURCES.txt` & `pulumi_artifactory-3.6.0a1685615210/pulumi_artifactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1685164706/setup.py` & `pulumi_artifactory-3.6.0a1685615210/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.6.0a1685164706"
-PLUGIN_VERSION = "3.6.0-alpha.1685164706+38d01b31"
+VERSION = "3.6.0a1685615210"
+PLUGIN_VERSION = "3.6.0-alpha.1685615210+8a20f4c9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'artifactory', PLUGIN_VERSION])
         except OSError as error:
```

