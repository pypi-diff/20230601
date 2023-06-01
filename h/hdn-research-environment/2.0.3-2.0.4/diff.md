# Comparing `tmp/hdn-research-environment-2.0.3.tar.gz` & `tmp/hdn-research-environment-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.0.3.tar", last modified: Thu Jun  1 15:12:49 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.0.4.tar", last modified: Thu Jun  1 15:35:31 2023, max compression
```

## Comparing `hdn-research-environment-2.0.3.tar` & `hdn-research-environment-2.0.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.3/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.3/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.3/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.3/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.3/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    19372 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.3/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.3/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     7049 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.3/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.3/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.3/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.3/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    13390 2023-06-01 15:11:29.000000 hdn-research-environment-2.0.3/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.3/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.3/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.4/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.4/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.4/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.4/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.4/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.4/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.4/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    19406 2023-06-01 15:32:47.000000 hdn-research-environment-2.0.4/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.4/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.4/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7049 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.4/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.4/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.4/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.4/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.4/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.4/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.4/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13390 2023-06-01 15:11:29.000000 hdn-research-environment-2.0.4/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.4/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-01 15:35:31.000000 hdn-research-environment-2.0.4/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.4/setup.py
```

### Comparing `hdn-research-environment-2.0.3/LICENSE` & `hdn-research-environment-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/PKG-INFO` & `hdn-research-environment-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.3/environment/api/v1/__init__.py` & `hdn-research-environment-2.0.4/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/api/v1/auth.py` & `hdn-research-environment-2.0.4/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/api/v1/decorators.py` & `hdn-research-environment-2.0.4/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/api/v2/__init__.py` & `hdn-research-environment-2.0.4/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/api/v2/decorators.py` & `hdn-research-environment-2.0.4/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/constants.py` & `hdn-research-environment-2.0.4/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/decorators.py` & `hdn-research-environment-2.0.4/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/deserializers.py` & `hdn-research-environment-2.0.4/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/entities.py` & `hdn-research-environment-2.0.4/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/exceptions.py` & `hdn-research-environment-2.0.4/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/forms.py` & `hdn-research-environment-2.0.4/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/mailers.py` & `hdn-research-environment-2.0.4/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/migrations/0001_initial.py` & `hdn-research-environment-2.0.4/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.0.4/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.0.4/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.0.4/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.0.4/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/models.py` & `hdn-research-environment-2.0.4/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/services.py` & `hdn-research-environment-2.0.4/environment/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,17 +537,17 @@
         subject, body, settings.DEFAULT_FROM_EMAIL, [user.email], fail_silently=False
     )
 
 
 def persist_workflow(
     user: User,
     execution_resource_name: str,
-    project_id: int,
     type: int,
-    workspace_name: str,
+    project_id: Optional[int] = None,
+    workspace_name: Optional[str] = None,
 ) -> Workflow:
     return Workflow.objects.create(
         user=user,
         execution_resource_name=execution_resource_name,
         workspace_name=workspace_name,
         project_id=project_id,
         type=type,
```

### Comparing `hdn-research-environment-2.0.3/environment/signals.py` & `hdn-research-environment-2.0.4/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.0.4/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.0.4/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.0.4/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.0.4/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tasks.py` & `hdn-research-environment-2.0.4/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.0.4/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.0.4/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.0.4/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.0.4/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.0.4/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.0.4/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.0.4/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.0.4/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.0.4/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.0.4/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.0.4/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/helpers.py` & `hdn-research-environment-2.0.4/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/mocks.py` & `hdn-research-environment-2.0.4/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/test_decorators.py` & `hdn-research-environment-2.0.4/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/test_services.py` & `hdn-research-environment-2.0.4/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/test_signals.py` & `hdn-research-environment-2.0.4/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/test_utilities.py` & `hdn-research-environment-2.0.4/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/test_validators.py` & `hdn-research-environment-2.0.4/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/tests/test_views.py` & `hdn-research-environment-2.0.4/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/urls.py` & `hdn-research-environment-2.0.4/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/utilities.py` & `hdn-research-environment-2.0.4/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/environment/views.py` & `hdn-research-environment-2.0.4/environment/views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.0.4/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.3/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.0.4/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.3/setup.cfg` & `hdn-research-environment-2.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.0.3
+version = 2.0.4
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

