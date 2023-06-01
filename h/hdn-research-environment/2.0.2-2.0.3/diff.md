# Comparing `tmp/hdn-research-environment-2.0.2.tar.gz` & `tmp/hdn-research-environment-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.0.2.tar", last modified: Wed May 31 14:41:02 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.0.3.tar", last modified: Thu Jun  1 15:12:49 2023, max compression
```

## Comparing `hdn-research-environment-2.0.2.tar` & `hdn-research-environment-2.0.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.2/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.2/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.2/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.2/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.2/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    19372 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.2/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.2/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     7049 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.2/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.2/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.2/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.2/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.2/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.2/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    13384 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.2/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.2/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-05-31 14:41:02.000000 hdn-research-environment-2.0.2/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.2/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.3/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.3/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.3/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.3/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.0.3/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    19372 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.3/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.3/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7049 2023-05-31 14:40:16.000000 hdn-research-environment-2.0.3/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1854 2023-05-30 18:52:36.000000 hdn-research-environment-2.0.3/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.3/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.3/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.3/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.3/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.3/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13390 2023-06-01 15:11:29.000000 hdn-research-environment-2.0.3/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2954 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.3/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-01 15:12:49.000000 hdn-research-environment-2.0.3/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.3/setup.py
```

### Comparing `hdn-research-environment-2.0.2/LICENSE` & `hdn-research-environment-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/PKG-INFO` & `hdn-research-environment-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.2/environment/api/v1/__init__.py` & `hdn-research-environment-2.0.3/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/api/v1/auth.py` & `hdn-research-environment-2.0.3/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/api/v1/decorators.py` & `hdn-research-environment-2.0.3/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/api/v2/__init__.py` & `hdn-research-environment-2.0.3/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/api/v2/decorators.py` & `hdn-research-environment-2.0.3/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/constants.py` & `hdn-research-environment-2.0.3/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/decorators.py` & `hdn-research-environment-2.0.3/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/deserializers.py` & `hdn-research-environment-2.0.3/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/entities.py` & `hdn-research-environment-2.0.3/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/exceptions.py` & `hdn-research-environment-2.0.3/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/forms.py` & `hdn-research-environment-2.0.3/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/mailers.py` & `hdn-research-environment-2.0.3/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/migrations/0001_initial.py` & `hdn-research-environment-2.0.3/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.0.3/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.0.3/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.0.3/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.0.3/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/models.py` & `hdn-research-environment-2.0.3/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/services.py` & `hdn-research-environment-2.0.3/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/signals.py` & `hdn-research-environment-2.0.3/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.0.3/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.0.3/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.0.3/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.0.3/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tasks.py` & `hdn-research-environment-2.0.3/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.0.3/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.0.3/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.0.3/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.0.3/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.0.3/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.0.3/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.0.3/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.0.3/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.0.3/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.0.3/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.0.3/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/helpers.py` & `hdn-research-environment-2.0.3/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/mocks.py` & `hdn-research-environment-2.0.3/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/test_decorators.py` & `hdn-research-environment-2.0.3/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/test_services.py` & `hdn-research-environment-2.0.3/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/test_signals.py` & `hdn-research-environment-2.0.3/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/test_utilities.py` & `hdn-research-environment-2.0.3/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/test_validators.py` & `hdn-research-environment-2.0.3/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/tests/test_views.py` & `hdn-research-environment-2.0.3/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/urls.py` & `hdn-research-environment-2.0.3/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/utilities.py` & `hdn-research-environment-2.0.3/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/environment/views.py` & `hdn-research-environment-2.0.3/environment/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             available_project_environment_workflow_triplets
         )
     )
     workspaces_being_created_dict = services.get_workspaces_being_created(request.user)
     environment_projects_pairs_with_creating = (
         projects_with_environments_being_created
         + environment_project_workflow_triplets
-        + workspaces_being_created_dict.values()
+        + list(workspaces_being_created_dict.values())
     )
 
     sorted_environments_project_workflow_triplets_dict = (
         services.sort_environments_per_workspace(
             environment_projects_pairs_with_creating, workspaces_list
         )
     )
```

### Comparing `hdn-research-environment-2.0.2/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.0.3/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.0.2/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.0.3/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.0.2/setup.cfg` & `hdn-research-environment-2.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.0.2
+version = 2.0.3
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

