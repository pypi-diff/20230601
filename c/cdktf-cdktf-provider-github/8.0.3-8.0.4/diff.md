# Comparing `tmp/cdktf-cdktf-provider-github-8.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-github-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-github-8.0.3.tar", last modified: Fri May 19 03:17:13 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-github-8.0.4.tar", last modified: Thu Jun  1 14:24:20 2023, max compression
```

## Comparing `cdktf-cdktf-provider-github-8.0.3.tar` & `cdktf-cdktf-provider-github-8.0.4.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.697975 cdktf-cdktf-provider-github-8.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-19 03:17:13.697975 cdktf-cdktf-provider-github-8.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 03:17:13.697975 cdktf-cdktf-provider-github-8.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.673975 cdktf-cdktf-provider-github-8.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   516097 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/_jsii/provider-github@8.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_environment_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    28811 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_environment_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_environment_variable/
--rw-r--r--   0 runner    (1001) docker     (123)    25446 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_environment_variable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_oidc_subject_claim_customization_template/
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_oidc_subject_claim_customization_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    49774 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    30329 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_secret_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)    21749 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_secret_repositories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_variable/
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_variable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_access_level/
--rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_access_level/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_oidc_subject_claim_customization_template/
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_oidc_subject_claim_customization_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    41880 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_runner_group/
--rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_runner_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    25966 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_variable/
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_variable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/app_installation_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)    21400 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/app_installation_repositories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/app_installation_repository/
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/app_installation_repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch/
--rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_default/
--rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_protection/
--rw-r--r--   0 runner    (1001) docker     (123)   108230 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_protection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_protection_v3/
--rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_protection_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_environment_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    32857 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_environment_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_environment_variables/
--rw-r--r--   0 runner    (1001) docker     (123)    33193 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_environment_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_oidc_subject_claim_customization_template/
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_oidc_subject_claim_customization_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_public_key/
--rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_public_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_registration_token/
--rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_registration_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    26096 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_variables/
--rw-r--r--   0 runner    (1001) docker     (123)    26389 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_public_key/
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_public_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_registration_token/
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_registration_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_repository_oidc_subject_claim_customization_template/
--rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_repository_oidc_subject_claim_customization_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_variables/
--rw-r--r--   0 runner    (1001) docker     (123)    30257 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_app/
--rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_branch/
--rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_branch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_branch_protection_rules/
--rw-r--r--   0 runner    (1001) docker     (123)    27504 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_branch_protection_rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_collaborators/
--rw-r--r--   0 runner    (1001) docker     (123)    34341 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_collaborators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_public_key/
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_public_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    26228 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_public_key/
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_public_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    30108 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_enterprise/
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_enterprise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_external_groups/
--rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_external_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ip_ranges/
--rw-r--r--   0 runner    (1001) docker     (123)    20521 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ip_ranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_issue_labels/
--rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_issue_labels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_membership/
--rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_membership/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization/
--rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.685975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_ip_allow_list/
--rw-r--r--   0 runner    (1001) docker     (123)    26424 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_ip_allow_list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_team_sync_groups/
--rw-r--r--   0 runner    (1001) docker     (123)    25938 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_team_sync_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_teams/
--rw-r--r--   0 runner    (1001) docker     (123)    35432 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_teams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)    25956 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_webhooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ref/
--rw-r--r--   0 runner    (1001) docker     (123)    22063 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ref/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_release/
--rw-r--r--   0 runner    (1001) docker     (123)    39618 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repositories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository/
--rw-r--r--   0 runner    (1001) docker     (123)    58730 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_branches/
--rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_branches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_deploy_keys/
--rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_deploy_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_file/
--rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_milestone/
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_milestone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_pull_request/
--rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_pull_request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_pull_requests/
--rw-r--r--   0 runner    (1001) docker     (123)    44770 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_pull_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_teams/
--rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_teams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_webhooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ssh_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_team/
--rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_tree/
--rw-r--r--   0 runner    (1001) docker     (123)    32177 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_user/
--rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_users/
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_organization_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    30485 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_organization_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_organization_secret_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_organization_secret_repositories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/emu_group_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/emu_group_mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/enterprise_organization/
--rw-r--r--   0 runner    (1001) docker     (123)    27816 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/enterprise_organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/issue/
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/issue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.689975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/issue_label/
--rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/issue_label/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/membership/
--rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/membership/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_block/
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_block/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_project/
--rw-r--r--   0 runner    (1001) docker     (123)    20485 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_security_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_security_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_settings/
--rw-r--r--   0 runner    (1001) docker     (123)   110667 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_webhook/
--rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/project_card/
--rw-r--r--   0 runner    (1001) docker     (123)    25465 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/project_card/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/project_column/
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/project_column/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    35902 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/release/
--rw-r--r--   0 runner    (1001) docker     (123)    40683 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository/
--rw-r--r--   0 runner    (1001) docker     (123)   178960 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_autolink_reference/
--rw-r--r--   0 runner    (1001) docker     (123)    27528 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_autolink_reference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_collaborator/
--rw-r--r--   0 runner    (1001) docker     (123)    27808 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_collaborator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_collaborators/
--rw-r--r--   0 runner    (1001) docker     (123)    54032 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_collaborators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_deploy_key/
--rw-r--r--   0 runner    (1001) docker     (123)    25439 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_deploy_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_environment/
--rw-r--r--   0 runner    (1001) docker     (123)    55845 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_file/
--rw-r--r--   0 runner    (1001) docker     (123)    37207 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_milestone/
--rw-r--r--   0 runner    (1001) docker     (123)    29979 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_milestone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_project/
--rw-r--r--   0 runner    (1001) docker     (123)    22661 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_pull_request/
--rw-r--r--   0 runner    (1001) docker     (123)    35193 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_pull_request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_tag_protection/
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_tag_protection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_webhook/
--rw-r--r--   0 runner    (1001) docker     (123)    42235 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team/
--rw-r--r--   0 runner    (1001) docker     (123)    31938 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_members/
--rw-r--r--   0 runner    (1001) docker     (123)    35090 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_membership/
--rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_membership/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_repository/
--rw-r--r--   0 runner    (1001) docker     (123)    23203 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    33212 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.693975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_sync_group_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)    37948 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_sync_group_mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.697975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_gpg_key/
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_gpg_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.697975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_invitation_accepter/
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_invitation_accepter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.697975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_ssh_key/
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-05-19 03:17:02.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_ssh_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:17:13.681975 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-19 03:17:13.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-19 03:17:13.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:17:13.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 03:17:13.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 03:17:13.000000 cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.350041 cdktf-cdktf-provider-github-8.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-01 14:24:20.350041 cdktf-cdktf-provider-github-8.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:24:20.350041 cdktf-cdktf-provider-github-8.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.322040 cdktf-cdktf-provider-github-8.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.330041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   522938 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/_jsii/provider-github@8.0.4.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_environment_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    28811 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_environment_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_environment_variable/
+-rw-r--r--   0 runner    (1001) docker     (123)    25446 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_environment_variable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_oidc_subject_claim_customization_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_oidc_subject_claim_customization_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    49774 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    30329 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_secret_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)    21749 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_secret_repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_variable/
+-rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_variable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_access_level/
+-rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_access_level/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_oidc_subject_claim_customization_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_oidc_subject_claim_customization_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    41880 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_runner_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_runner_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    25966 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_variable/
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_variable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/app_installation_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)    21400 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/app_installation_repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/app_installation_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/app_installation_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch/
+-rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_default/
+-rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_protection/
+-rw-r--r--   0 runner    (1001) docker     (123)   108230 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_protection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_protection_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_protection_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_environment_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    32857 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_environment_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    33193 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_environment_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_oidc_subject_claim_customization_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_oidc_subject_claim_customization_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_public_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_public_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_registration_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_registration_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    26096 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    26389 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_public_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_public_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_registration_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_registration_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_repository_oidc_subject_claim_customization_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_repository_oidc_subject_claim_customization_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    30257 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_app/
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_branch/
+-rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_branch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_branch_protection_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)    27504 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_branch_protection_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_collaborators/
+-rw-r--r--   0 runner    (1001) docker     (123)    34341 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_collaborators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_public_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_public_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    26228 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_public_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_public_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    30108 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_enterprise/
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_enterprise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_external_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_external_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ip_ranges/
+-rw-r--r--   0 runner    (1001) docker     (123)    20521 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ip_ranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_issue_labels/
+-rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_issue_labels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_membership/
+-rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_membership/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization/
+-rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_ip_allow_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_ip_allow_list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_team_sync_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)    25938 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_team_sync_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.338041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_teams/
+-rw-r--r--   0 runner    (1001) docker     (123)    35432 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_teams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    25956 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_webhooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ref/
+-rw-r--r--   0 runner    (1001) docker     (123)    22063 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ref/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_release/
+-rw-r--r--   0 runner    (1001) docker     (123)    39618 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)    58730 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_branches/
+-rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_branches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_deploy_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_deploy_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_milestone/
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_milestone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_pull_request/
+-rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_pull_request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_pull_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)    44770 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_pull_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_teams/
+-rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_teams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_webhooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ssh_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_team/
+-rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)    32177 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_users/
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_organization_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    30485 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_organization_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_organization_secret_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_organization_secret_repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/emu_group_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/emu_group_mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/enterprise_organization/
+-rw-r--r--   0 runner    (1001) docker     (123)    27816 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/enterprise_organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/issue/
+-rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/issue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/issue_label/
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/issue_label/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/membership/
+-rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/membership/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_block/
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_block/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.342041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_project/
+-rw-r--r--   0 runner    (1001) docker     (123)    20485 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_security_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_security_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)   110667 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/project_card/
+-rw-r--r--   0 runner    (1001) docker     (123)    25465 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/project_card/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/project_column/
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/project_column/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    35902 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/release/
+-rw-r--r--   0 runner    (1001) docker     (123)    40683 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)   178960 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_autolink_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)    27528 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_autolink_reference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_collaborator/
+-rw-r--r--   0 runner    (1001) docker     (123)    27808 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_collaborator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_collaborators/
+-rw-r--r--   0 runner    (1001) docker     (123)    54032 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_collaborators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_deploy_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    25439 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_deploy_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    55845 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    37207 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_milestone/
+-rw-r--r--   0 runner    (1001) docker     (123)    29979 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_milestone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_project/
+-rw-r--r--   0 runner    (1001) docker     (123)    22661 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_pull_request/
+-rw-r--r--   0 runner    (1001) docker     (123)    35193 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_pull_request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_tag_protection/
+-rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_tag_protection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)    42235 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team/
+-rw-r--r--   0 runner    (1001) docker     (123)    31938 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_members/
+-rw-r--r--   0 runner    (1001) docker     (123)    35090 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_membership/
+-rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_membership/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)    23203 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    33212 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.346041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_sync_group_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    37948 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_sync_group_mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.350041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_gpg_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_gpg_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.350041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_invitation_accepter/
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_invitation_accepter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.350041 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_ssh_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-06-01 14:24:09.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_ssh_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:24:20.334040 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-01 14:24:20.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-01 14:24:20.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:24:20.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:24:20.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 14:24:20.000000 cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-github-8.0.3/LICENSE` & `cdktf-cdktf-provider-github-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/PKG-INFO` & `cdktf-cdktf-provider-github-8.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-github
-Version: 8.0.3
+Version: 8.0.4
 Summary: Prebuilt github Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-github.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-github-8.0.3/README.md` & `cdktf-cdktf-provider-github-8.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/setup.py` & `cdktf-cdktf-provider-github-8.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-github",
-    "version": "8.0.3",
+    "version": "8.0.4",
     "description": "Prebuilt github Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-github.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -126,23 +126,23 @@
         "cdktf_cdktf_provider_github.team_sync_group_mapping",
         "cdktf_cdktf_provider_github.user_gpg_key",
         "cdktf_cdktf_provider_github.user_invitation_accepter",
         "cdktf_cdktf_provider_github.user_ssh_key"
     ],
     "package_data": {
         "cdktf_cdktf_provider_github._jsii": [
-            "provider-github@8.0.3.jsii.tgz"
+            "provider-github@8.0.4.jsii.tgz"
         ],
         "cdktf_cdktf_provider_github": [
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

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_environment_secret/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_environment_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_environment_variable/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_environment_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_oidc_subject_claim_customization_template/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_oidc_subject_claim_customization_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_permissions/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_secret/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_secret_repositories/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_secret_repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_organization_variable/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_organization_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_access_level/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_access_level/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_oidc_subject_claim_customization_template/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_oidc_subject_claim_customization_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_repository_permissions/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_repository_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_runner_group/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_runner_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_secret/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/actions_variable/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/actions_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/app_installation_repositories/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/app_installation_repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/app_installation_repository/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/app_installation_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_default/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_default/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_protection/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_protection/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/branch_protection_v3/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/branch_protection_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_environment_secrets/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_environment_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_environment_variables/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_environment_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_oidc_subject_claim_customization_template/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_oidc_subject_claim_customization_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_public_key/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_public_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_registration_token/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_registration_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_secrets/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_organization_variables/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_organization_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_public_key/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_public_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_registration_token/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_registration_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_repository_oidc_subject_claim_customization_template/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_repository_oidc_subject_claim_customization_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_secrets/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_actions_variables/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_actions_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_app/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_app/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_branch/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_branch/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_branch_protection_rules/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_branch_protection_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_collaborators/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_collaborators/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_public_key/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_public_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_secrets/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_organization_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_public_key/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_public_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_dependabot_secrets/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_dependabot_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_enterprise/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_enterprise/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_external_groups/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_external_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ip_ranges/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ip_ranges/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_issue_labels/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_issue_labels/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_membership/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_membership/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_ip_allow_list/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_ip_allow_list/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
     @jsii.member(jsii_name="ipAllowList")
-    def ip_allow_list(self) -> "DataGithubOrganizationIpAllowListIpAllowListList":
-        return typing.cast("DataGithubOrganizationIpAllowListIpAllowListList", jsii.get(self, "ipAllowList"))
+    def ip_allow_list(self) -> "DataGithubOrganizationIpAllowListIpAllowListStructList":
+        return typing.cast("DataGithubOrganizationIpAllowListIpAllowListStructList", jsii.get(self, "ipAllowList"))
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
@@ -258,114 +258,114 @@
     def __repr__(self) -> str:
         return "DataGithubOrganizationIpAllowListConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-github.dataGithubOrganizationIpAllowList.DataGithubOrganizationIpAllowListIpAllowList",
+    jsii_type="@cdktf/provider-github.dataGithubOrganizationIpAllowList.DataGithubOrganizationIpAllowListIpAllowListStruct",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataGithubOrganizationIpAllowListIpAllowList:
+class DataGithubOrganizationIpAllowListIpAllowListStruct:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataGithubOrganizationIpAllowListIpAllowList(%s)" % ", ".join(
+        return "DataGithubOrganizationIpAllowListIpAllowListStruct(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataGithubOrganizationIpAllowListIpAllowListList(
+class DataGithubOrganizationIpAllowListIpAllowListStructList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-github.dataGithubOrganizationIpAllowList.DataGithubOrganizationIpAllowListIpAllowListList",
+    jsii_type="@cdktf/provider-github.dataGithubOrganizationIpAllowList.DataGithubOrganizationIpAllowListIpAllowListStructList",
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
-            type_hints = typing.get_type_hints(_typecheckingstub__947a8f03c69076d5ee6427b369bbf0a257cec04293cb1c5c8d5f09fe2c0bc66d)
+            type_hints = typing.get_type_hints(_typecheckingstub__3da93a6b33124e551b40a79ed7daa028e9d49f30a57af58d3cafdd80456eb770)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataGithubOrganizationIpAllowListIpAllowListOutputReference":
+    ) -> "DataGithubOrganizationIpAllowListIpAllowListStructOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7f8f315c4ffc4495b699e9f94f86db1a56c9493ca10900d92b41b1ced8d1549e)
+            type_hints = typing.get_type_hints(_typecheckingstub__adc455ff017bedf4622087b49171fac6b8fe15883744a05b289e0ee94b535f31)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataGithubOrganizationIpAllowListIpAllowListOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataGithubOrganizationIpAllowListIpAllowListStructOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ebdd4c7e6c148ef990de9ff4013e63fdeb9408500f94c8c90587838f36c441cf)
+            type_hints = typing.get_type_hints(_typecheckingstub__ac988d3faa972da9a97624ee04193be2f179f7fbe7afd68521bb1aab96b23e8d)
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
-            type_hints = typing.get_type_hints(_typecheckingstub__fc658da4dce9a7ceefd0d7f55e098cff1b86f4ff2a8b6a3f891c56d0dc82fb0b)
+            type_hints = typing.get_type_hints(_typecheckingstub__905f66e766807502195e520a54adc5784e6b297e19642dc7ddf939e9f185aef2)
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
-            type_hints = typing.get_type_hints(_typecheckingstub__182fcb00b67ba9f368f21ed028d9a7291498b88d026be6b6514337ff7f8a3604)
+            type_hints = typing.get_type_hints(_typecheckingstub__003621099289117bc2333b79673128178d503d51eb91fdeacba7547dca231d99)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataGithubOrganizationIpAllowListIpAllowListOutputReference(
+class DataGithubOrganizationIpAllowListIpAllowListStructOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-github.dataGithubOrganizationIpAllowList.DataGithubOrganizationIpAllowListIpAllowListOutputReference",
+    jsii_type="@cdktf/provider-github.dataGithubOrganizationIpAllowList.DataGithubOrganizationIpAllowListIpAllowListStructOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -373,15 +373,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__40641c9c718d85974e3aa1659ac2e703139faaac96fdb54238ee15ca3cd5623b)
+            type_hints = typing.get_type_hints(_typecheckingstub__2af8351d490d72fec0e97c1fa12739b381da3f796cfcba073d1561a135f52ef5)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -414,34 +414,34 @@
     def updated_at(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "updatedAt"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataGithubOrganizationIpAllowListIpAllowList]:
-        return typing.cast(typing.Optional[DataGithubOrganizationIpAllowListIpAllowList], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataGithubOrganizationIpAllowListIpAllowListStruct]:
+        return typing.cast(typing.Optional[DataGithubOrganizationIpAllowListIpAllowListStruct], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataGithubOrganizationIpAllowListIpAllowList],
+        value: typing.Optional[DataGithubOrganizationIpAllowListIpAllowListStruct],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ca54b7d780a8e140dff057191edabdd0e32bd703d0b57067b847cb96a26de514)
+            type_hints = typing.get_type_hints(_typecheckingstub__d98b6e66ee69c58c14cf2962b5da61d4eb2711477ecbef51026788a3faf2a0ef)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
     "DataGithubOrganizationIpAllowList",
     "DataGithubOrganizationIpAllowListConfig",
-    "DataGithubOrganizationIpAllowListIpAllowList",
-    "DataGithubOrganizationIpAllowListIpAllowListList",
-    "DataGithubOrganizationIpAllowListIpAllowListOutputReference",
+    "DataGithubOrganizationIpAllowListIpAllowListStruct",
+    "DataGithubOrganizationIpAllowListIpAllowListStructList",
+    "DataGithubOrganizationIpAllowListIpAllowListStructOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__d249c17699f912f63a75c28df40d877d186def13189705d7429f9fffe827a2e4(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
@@ -474,53 +474,53 @@
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__947a8f03c69076d5ee6427b369bbf0a257cec04293cb1c5c8d5f09fe2c0bc66d(
+def _typecheckingstub__3da93a6b33124e551b40a79ed7daa028e9d49f30a57af58d3cafdd80456eb770(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7f8f315c4ffc4495b699e9f94f86db1a56c9493ca10900d92b41b1ced8d1549e(
+def _typecheckingstub__adc455ff017bedf4622087b49171fac6b8fe15883744a05b289e0ee94b535f31(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ebdd4c7e6c148ef990de9ff4013e63fdeb9408500f94c8c90587838f36c441cf(
+def _typecheckingstub__ac988d3faa972da9a97624ee04193be2f179f7fbe7afd68521bb1aab96b23e8d(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__fc658da4dce9a7ceefd0d7f55e098cff1b86f4ff2a8b6a3f891c56d0dc82fb0b(
+def _typecheckingstub__905f66e766807502195e520a54adc5784e6b297e19642dc7ddf939e9f185aef2(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__182fcb00b67ba9f368f21ed028d9a7291498b88d026be6b6514337ff7f8a3604(
+def _typecheckingstub__003621099289117bc2333b79673128178d503d51eb91fdeacba7547dca231d99(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__40641c9c718d85974e3aa1659ac2e703139faaac96fdb54238ee15ca3cd5623b(
+def _typecheckingstub__2af8351d490d72fec0e97c1fa12739b381da3f796cfcba073d1561a135f52ef5(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ca54b7d780a8e140dff057191edabdd0e32bd703d0b57067b847cb96a26de514(
-    value: typing.Optional[DataGithubOrganizationIpAllowListIpAllowList],
+def _typecheckingstub__d98b6e66ee69c58c14cf2962b5da61d4eb2711477ecbef51026788a3faf2a0ef(
+    value: typing.Optional[DataGithubOrganizationIpAllowListIpAllowListStruct],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_team_sync_groups/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_team_sync_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_teams/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_teams/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_organization_webhooks/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_organization_webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ref/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ref/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_release/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_release/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repositories/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_branches/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_branches/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_deploy_keys/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_deploy_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_file/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_milestone/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_milestone/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_pull_request/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_pull_request/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_pull_requests/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_pull_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_teams/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_teams/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_repository_webhooks/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_repository_webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_ssh_keys/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_ssh_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_team/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_team/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_tree/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_user/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/data_github_users/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/data_github_users/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_organization_secret/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_organization_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_organization_secret_repositories/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_organization_secret_repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/dependabot_secret/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/dependabot_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/emu_group_mapping/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/emu_group_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/enterprise_organization/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/enterprise_organization/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/issue/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/issue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/issue_label/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/issue_label/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/membership/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/membership/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_block/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_block/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_project/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_project/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_security_manager/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_security_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_settings/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/organization_webhook/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/organization_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/project_card/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/project_card/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/project_column/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/project_column/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/provider/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/release/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/release/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_autolink_reference/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_autolink_reference/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_collaborator/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_collaborator/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_collaborators/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_collaborators/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_deploy_key/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_deploy_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_environment/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_environment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_file/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_milestone/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_milestone/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_project/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_project/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_pull_request/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_pull_request/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_tag_protection/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_tag_protection/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/repository_webhook/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/repository_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_members/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_members/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_membership/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_membership/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_repository/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_settings/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/team_sync_group_mapping/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/team_sync_group_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_gpg_key/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_gpg_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_invitation_accepter/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_invitation_accepter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github/user_ssh_key/__init__.py` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github/user_ssh_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/PKG-INFO` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-github
-Version: 8.0.3
+Version: 8.0.4
 Summary: Prebuilt github Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-github.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-github-8.0.3/src/cdktf_cdktf_provider_github.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-github-8.0.4/src/cdktf_cdktf_provider_github.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_github/py.typed
 src/cdktf_cdktf_provider_github.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_github.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_github.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_github.egg-info/requires.txt
 src/cdktf_cdktf_provider_github.egg-info/top_level.txt
 src/cdktf_cdktf_provider_github/_jsii/__init__.py
-src/cdktf_cdktf_provider_github/_jsii/provider-github@8.0.3.jsii.tgz
+src/cdktf_cdktf_provider_github/_jsii/provider-github@8.0.4.jsii.tgz
 src/cdktf_cdktf_provider_github/actions_environment_secret/__init__.py
 src/cdktf_cdktf_provider_github/actions_environment_variable/__init__.py
 src/cdktf_cdktf_provider_github/actions_organization_oidc_subject_claim_customization_template/__init__.py
 src/cdktf_cdktf_provider_github/actions_organization_permissions/__init__.py
 src/cdktf_cdktf_provider_github/actions_organization_secret/__init__.py
 src/cdktf_cdktf_provider_github/actions_organization_secret_repositories/__init__.py
 src/cdktf_cdktf_provider_github/actions_organization_variable/__init__.py
```

