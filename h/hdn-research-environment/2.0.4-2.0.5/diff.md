# Comparing `tmp/hdn-research-environment-2.0.4.tar.gz` & `tmp/hdn-research-environment-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.0.4.tar", last modified: Thu Jun  1 15:35:31 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.0.5.tar", last modified: Thu Jun  1 18:10:59 2023, max compression
```

## Comparing `hdn-research-environment-2.0.4.tar` & `hdn-research-environment-2.0.5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.4/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.4/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.4/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.4/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.4/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.4/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.4/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    19406 2023-06-01 15:32:47.000000 hdn-research-environment-2.0.4/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.4/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.4/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     7049 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.4/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.4/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.4/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.4/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.4/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    13390 2023-06-01 15:11:29.000000 hdn-research-environment-2.0.4/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.4/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.4/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.5/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.5/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.5/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.5/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.5/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.5/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    19234 2023-06-01 18:10:39.000000 hdn-research-environment-2.0.5/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4349 2023-06-01 18:10:39.000000 hdn-research-environment-2.0.5/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.5/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.5/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7425 2023-06-01 18:10:39.000000 hdn-research-environment-2.0.5/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.5/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.5/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.5/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.5/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.5/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.5/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13311 2023-06-01 18:10:39.000000 hdn-research-environment-2.0.5/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.5/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-01 18:10:59.000000 hdn-research-environment-2.0.5/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.5/setup.py
```

### Comparing `hdn-research-environment-2.0.4/LICENSE` & `hdn-research-environment-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/PKG-INFO` & `hdn-research-environment-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.4
+Version: 2.0.5
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.4/environment/api/v1/__init__.py` & `hdn-research-environment-2.0.5/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/api/v1/auth.py` & `hdn-research-environment-2.0.5/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/api/v1/decorators.py` & `hdn-research-environment-2.0.5/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/api/v2/__init__.py` & `hdn-research-environment-2.0.5/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/api/v2/decorators.py` & `hdn-research-environment-2.0.5/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/constants.py` & `hdn-research-environment-2.0.5/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/decorators.py` & `hdn-research-environment-2.0.5/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/deserializers.py` & `hdn-research-environment-2.0.5/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/entities.py` & `hdn-research-environment-2.0.5/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/exceptions.py` & `hdn-research-environment-2.0.5/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/forms.py` & `hdn-research-environment-2.0.5/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/mailers.py` & `hdn-research-environment-2.0.5/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/migrations/0001_initial.py` & `hdn-research-environment-2.0.5/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.0.5/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.0.5/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.0.5/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.0.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/models.py` & `hdn-research-environment-2.0.5/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/services.py` & `hdn-research-environment-2.0.5/environment/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,22 +357,18 @@
     return [
         (environment, project, workflows)
         for project, environment, workflows in project_environment_workflow_triplets
         if environment is None and workflows.exists()
     ]
 
 
-def get_workspaces_being_created(user: User) -> Dict[str, Tuple[None, None, Workflow]]:
-    workspace_creation_workflows = Workflow.objects.filter(
+def get_workspace_creation_workflows(user: User) -> Iterable[Workflow]:
+    return Workflow.objects.filter(
         user=user, type=Workflow.WORKSPACE_CREATE, status=Workflow.INPROGRESS
     )
-    return {
-        workflow.get_type_display(): (None, None, workflow)
-        for workflow in workspace_creation_workflows
-    }
 
 
 def get_environment_project_pairs_with_expired_access(
     user: User,
 ) -> Iterable[Tuple[ResearchEnvironment, PublishedProject]]:
     all_environment_project_pairs = get_environments_with_projects(user)
     return [
```

### Comparing `hdn-research-environment-2.0.4/environment/signals.py` & `hdn-research-environment-2.0.5/environment/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 
 Event = apps.get_model("events", "Event")
 
 
 @receiver(post_save, sender=BillingAccountSharingInvite)
 @receiver(post_save, sender=CloudIdentity)
 def consume_billing_account_sharing_invites(sender, created, instance, **kwargs):
-    if not created:
-        return
-
     if sender is CloudIdentity:
+        if not created:
+            return
         cloud_identity = instance
         outstanding_invites = (
             cloud_identity.user.user_billingaccountsharinginvite_set.select_related(
                 "owner__cloud_identity"
             ).filter(is_consumed=False)
         )
     else:  # BillingAccountSharingInvite
```

### Comparing `hdn-research-environment-2.0.4/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.0.5/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.0.5/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.0.5/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.0.5/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tasks.py` & `hdn-research-environment-2.0.5/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.0.5/environment/templates/environment/_available_environments_list.html`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,31 @@
 <div class="d-flex flex-column align-items-end px-4 mb-3">
     <a class="btn btn-primary btn-sm" href="{% url 'create_workspace' %}">
       + Workspace
     </a>
 </div>
 
 <div id="accordion">
+    {% for workflow in workspace_creation_workflows %}
+        <div class="card">
+            <div class="card-header""{{ heading }}">
+                <button class="btn btn-link">
+                    <h6 class="mb-0">
+                        <div class="d-flex align-items-center">
+                            <div style="margin-right: 1.5rem">
+                                Provisioning
+                            </div>
+                            <div class="loader" style="font-size: 3.5px; margin: 0;">Loading...</div>
+                        </div>
+                    </h6>
+                </button>
+            </div>
+        </div>
+    {% endfor %}
+
     {% for workspace_name, environments_project_workflow_triplets in workspace_project_environment_workflow_triplets_dict.items %}
         {% with collapse="collapse-"|add:workspace_name heading="heading-"|add:workspace_name %}
             <div class="card">
                 <div class="card-header" id="{{ heading }}">
                     <button class="btn btn-link" data-toggle="collapse" data-target="#{{ collapse }}" aria-expanded="true" aria-controls="{{ collapse }}">
                         <h6 class="mb-0">
                             {{ workspace_name }}
@@ -31,57 +48,53 @@
                 </div>
 
                 <div id="{{ collapse }}" class="collapse show" aria-labelledby="{{ heading }}" data-parent="#accordion">
                     <div class="card-body">
                         {% if environments_project_workflow_triplets|length %}
                             <ul class="list-group list-group-flush">
                                 {% for environment, project, workflows in environments_project_workflow_triplets %}
-                                    {% if not environment and not project %}
-                                        <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
-                                    {% else %}
-                                        <li class="list-group-item">
-                                            <div class="row">
-                                                <div class="col-md-3">
-                                                    <a href="{% url 'published_project' project.slug project.version %}" target="_blank">
-                                                        {{ project }}
-                                                    </a>
-                                                </div>
-                                                <div class="col-md-3">
-                                                    <small>
-                                                        <i>Environment type:</i> {{ environment.type.value|capfirst }}<br>
-                                                        <i>Instance type:</i> {{ environment.instance_type.value }}<br>
-                                                        <i>Region:</i> {{ environment.region.value }}
-                                                    </small>
-                                                </div>
-                                                <div class="col-md-2">
+                                    <li class="list-group-item">
+                                        <div class="row">
+                                            <div class="col-md-3">
+                                                <a href="{% url 'published_project' project.slug project.version %}" target="_blank">
+                                                    {{ project }}
+                                                </a>
+                                            </div>
+                                            <div class="col-md-3">
+                                                <small>
+                                                    <i>Environment type:</i> {{ environment.type.value|capfirst }}<br>
+                                                    <i>Instance type:</i> {{ environment.instance_type.value }}<br>
+                                                    <i>Region:</i> {{ environment.region.value }}
+                                                </small>
+                                            </div>
+                                            <div class="col-md-2">
+                                                {% if workflows.exists %}
+                                                    {{ workflows.first.get_type_display }}
+                                                {% else %}
+                                                    {{ environment.status.value|capfirst }}
+                                                {% endif %}
+                                            </div>
+                                            <div class="col-md-4">
+                                                <div class="d-flex flex-wrap">
                                                     {% if workflows.exists %}
-                                                        {{ workflows.first.get_type_display }}
-                                                    {% else %}
-                                                        {{ environment.status.value|capfirst }}
-                                                    {% endif %}
-                                                </div>
-                                                <div class="col-md-4">
-                                                    <div class="d-flex flex-wrap">
-                                                        {% if workflows.exists %}
-                                                            <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
-                                                        {% elif environment.is_running or environment.is_paused %}
-                                                            {% if environment.is_running %}
-                                                                <a href="{{ environment.url }}" target="_blank" class="btn btn-sm btn-success m-1">Open</a>
-                                                                {% environment_modal_button environment=environment project=project button_type="modal_pause" %}
-                                                            {% else %}
-                                                                {% environment_modal_button environment=environment project=project button_type="modal_start" %}
-                                                            {% endif %}
-                                                            {% environment_modal_button environment=environment project=project button_type="modal_instance" %}
-                                                            {% environment_modal_button environment=environment project=project button_type="modal_destroy" %}
+                                                        <div class="loader" style="margin: 18px; font-size: 5px">Loading...</div>
+                                                    {% elif environment.is_running or environment.is_paused %}
+                                                        {% if environment.is_running %}
+                                                            <a href="{{ environment.url }}" target="_blank" class="btn btn-sm btn-success m-1">Open</a>
+                                                            {% environment_modal_button environment=environment project=project button_type="modal_pause" %}
+                                                        {% else %}
+                                                            {% environment_modal_button environment=environment project=project button_type="modal_start" %}
                                                         {% endif %}
-                                                    </div>
+                                                        {% environment_modal_button environment=environment project=project button_type="modal_instance" %}
+                                                        {% environment_modal_button environment=environment project=project button_type="modal_destroy" %}
+                                                    {% endif %}
                                                 </div>
                                             </div>
-                                        </li>
-                                    {% endif %}
+                                        </div>
+                                    </li>
                                 {% endfor %}
                             </ul>
                         {% else %}
                             <div class="text-center">
                                 You don't have any worbenches in this workspace.<br>
                                 Create one in the "Projects" tab.
                             </div>
@@ -118,8 +131,12 @@
     }
 
     {% for environment, project, workflows in environment_project_workflow_triplets %}
         {% for workflow in workflows %}
             scheduleExecutionPolling("{{ workflow.execution_resource_name }}", true);
         {% endfor %}
     {% endfor %}
+
+    {% for workflow in workspace_creation_workflows %}
+        scheduleExecutionPolling("{{ workflow.execution_resource_name }}", true);
+    {% endfor %}
 </script>
```

#### html2text {}

```diff
@@ -2,25 +2,26 @@
 %}
 {{ recent_workflow.get_type_display }} {{ recent_workflow.project }} failed!
 Try again later.
 {% elif recent_workflow_succeeded %}
 {{ recent_workflow.get_type_display }} {{ recent_workflow.project }} finished!
 {% endif %} {% endif %}
 +_Workspace
-{% for workspace_name, environments_project_workflow_triplets in
+{% for workflow in workspace_creation_workflows %}
+{{ heading }}">
+Provisioning
+Loading...
+{% endfor %} {% for workspace_name, environments_project_workflow_triplets in
 workspace_project_environment_workflow_triplets_dict.items %} {% with
 collapse="collapse-"|add:workspace_name heading="heading-"|add:workspace_name
 %}
 * {{ workspace_name }} *
 {% if environments_project_workflow_triplets|length %}
     * {% for environment, project, workflows in
-      environments_project_workflow_triplets %} {% if not environment and not
-      project %}
-      Loading...
-    * {% else %}
+      environments_project_workflow_triplets %}
     * {{_project_}}
       Environment type: {{ environment.type.value|capfirst }}
       Instance type: {{ environment.instance_type.value }}
       Region: {{ environment.region.value }}
       {% if workflows.exists %} {{ workflows.first.get_type_display }} {% else
       %} {{ environment.status.value|capfirst }} {% endif %}
       {% if workflows.exists %}
@@ -30,14 +31,14 @@
       environment=environment project=project button_type="modal_pause" %} {%
       else %} {% environment_modal_button environment=environment
       project=project button_type="modal_start" %} {% endif %} {%
       environment_modal_button environment=environment project=project
       button_type="modal_instance" %} {% environment_modal_button
       environment=environment project=project button_type="modal_destroy" %} {%
       endif %}
-    * {% endif %} {% endfor %}
+    * {% endfor %}
 {% else %}
 You don't have any worbenches in this workspace.
 Create one in the "Projects" tab.
 {% endif %}
 {% endwith %} {% endfor %}
```

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.0.5/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.0.5/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.0.5/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.0.5/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.0.5/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.0.5/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.0.5/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.0.5/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.0.5/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.0.5/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/helpers.py` & `hdn-research-environment-2.0.5/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/mocks.py` & `hdn-research-environment-2.0.5/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/test_decorators.py` & `hdn-research-environment-2.0.5/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/test_services.py` & `hdn-research-environment-2.0.5/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/test_signals.py` & `hdn-research-environment-2.0.5/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/test_utilities.py` & `hdn-research-environment-2.0.5/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/test_validators.py` & `hdn-research-environment-2.0.5/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/tests/test_views.py` & `hdn-research-environment-2.0.5/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/urls.py` & `hdn-research-environment-2.0.5/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/utilities.py` & `hdn-research-environment-2.0.5/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/environment/views.py` & `hdn-research-environment-2.0.5/environment/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,52 +63,47 @@
         )
         billing_accounts_list_future = executor.submit(
             services.get_billing_accounts_list, request.user
         )
         environment_project_workflow_future = executor.submit(
             services.get_environments_with_projects, request.user
         )
+        workspace_creation_workflows_future = executor.submit(services.get_workspace_creation_workflows, request.user)
 
     workspaces_list = workspaces_list_future.result()
     environment_project_workflow_triplets = environment_project_workflow_future.result()
     billing_accounts_list = billing_accounts_list_future.result()
+    workspace_creation_workflows = workspace_creation_workflows_future.result()
 
     environments = map(lambda pair: pair[0], environment_project_workflow_triplets)
     available_project_environment_workflow_triplets = (
         services.get_available_projects_with_environments(
             request.user,
             environments,
         )
     )
     projects_with_environments_being_created = (
         services.get_projects_with_environment_being_created(
             available_project_environment_workflow_triplets
         )
     )
-    workspaces_being_created_dict = services.get_workspaces_being_created(request.user)
     environment_projects_pairs_with_creating = (
-        projects_with_environments_being_created
-        + environment_project_workflow_triplets
-        + list(workspaces_being_created_dict.values())
+        projects_with_environments_being_created + environment_project_workflow_triplets
     )
 
     sorted_environments_project_workflow_triplets_dict = (
         services.sort_environments_per_workspace(
             environment_projects_pairs_with_creating, workspaces_list
         )
     )
 
-    sorted_environments_project_workflow_triplets_with_creating_dict = {
-        **sorted_environments_project_workflow_triplets_dict,
-        **workspaces_being_created_dict,
-    }
-
     context = {
         "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
-        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_with_creating_dict,
+        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_dict,
+        "workspace_creation_workflows": workspace_creation_workflows,
         "billing_accounts_list": billing_accounts_list,
     }
 
     return render(
         request,
         "environment/research_environments.html",
         context,
```

### Comparing `hdn-research-environment-2.0.4/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.0.5/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.4
+Version: 2.0.5
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.4/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.0.5/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.4/setup.cfg` & `hdn-research-environment-2.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.0.4
+version = 2.0.5
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

