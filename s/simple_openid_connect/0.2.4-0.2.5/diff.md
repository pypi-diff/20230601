# Comparing `tmp/simple_openid_connect-0.2.4.tar.gz` & `tmp/simple_openid_connect-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_openid_connect-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "simple_openid_connect-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `simple_openid_connect-0.2.4.tar` & `simple_openid_connect-0.2.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       50 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/.gitattributes
--rw-r--r--   0        0        0     1584 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/.github/workflows/checks.yml
--rw-r--r--   0        0        0      136 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/.gitignore
--rw-r--r--   0        0        0      795 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/.readthedocs.yaml
--rw-r--r--   0        0        0      298 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/DEVELOPMENT.md
--rw-r--r--   0        0        0     1116 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/LICENSE
--rw-r--r--   0        0        0     4447 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.4/README.md
--rw-r--r--   0        0        0      679 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/Makefile
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      320 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/api.rst
--rw-r--r--   0        0        0     1790 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/conf.py
--rw-r--r--   0        0        0     5754 2023-05-25 12:12:58.573729 simple_openid_connect-0.2.4/docs/django-integration.rst
--rw-r--r--   0        0        0     2615 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/drf-integration.rst
--rw-r--r--   0        0        0      708 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/index.rst
--rw-r--r--   0        0        0     1247 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/installation.rst
--rw-r--r--   0        0        0     4868 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/docs/usage.rst
--rw-r--r--   0        0        0     2391 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      211 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/requirements.dev.txt
--rw-r--r--   0        0        0      127 2023-05-26 08:20:06.731638 simple_openid_connect-0.2.4/src/simple_openid_connect/__init__.py
--rw-r--r--   0        0        0     4204 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/src/simple_openid_connect/base_data.py
--rw-r--r--   0        0        0    10682 2023-05-25 12:13:07.757788 simple_openid_connect-0.2.4/src/simple_openid_connect/client.py
--rw-r--r--   0        0        0     3443 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.4/src/simple_openid_connect/client_authentication.py
--rw-r--r--   0        0        0    57273 2023-05-25 12:16:39.699145 simple_openid_connect-0.2.4/src/simple_openid_connect/data.py
--rw-r--r--   0        0        0     1819 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/discovery.py
--rw-r--r--   0        0        0     1174 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/exceptions.py
--rw-r--r--   0        0        0      343 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/flows/__init__.py
--rw-r--r--   0        0        0     5631 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
--rw-r--r--   0        0        0     6115 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/flows/authorization_code_flow/client.py
--rw-r--r--   0        0        0     2208 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/flows/direct_access_grant/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/flows/direct_access_grant/client.py
--rw-r--r--   0        0        0       53 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/__init__.py
--rw-r--r--   0        0        0       61 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/__init__.py
--rw-r--r--   0        0        0     5467 2023-05-12 09:43:09.751399 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/apps.py
--rw-r--r--   0        0        0     4555 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/decorators.py
--rw-r--r--   0        0        0     2630 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/migrations/__init__.py
--rw-r--r--   0        0        0     5728 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/models.py
--rw-r--r--   0        0        0      381 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
--rw-r--r--   0        0        0      729 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/urls.py
--rw-r--r--   0        0        0     2338 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/user_mapping.py
--rw-r--r--   0        0        0     4644 2023-05-26 08:18:07.087644 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/views.py
--rw-r--r--   0        0        0      306 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/djangorestframework/__init__.py
--rw-r--r--   0        0        0     4648 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/djangorestframework/authentication.py
--rw-r--r--   0        0        0      957 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
--rw-r--r--   0        0        0     2531 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/djangorestframework/permissions.py
--rw-r--r--   0        0        0      472 2023-05-12 09:43:09.751399 simple_openid_connect-0.2.4/src/simple_openid_connect/jwk.py
--rw-r--r--   0        0        0      621 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/rp_initiated_logout.py
--rw-r--r--   0        0        0     1509 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/token_introspection.py
--rw-r--r--   0        0        0     1566 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.4/src/simple_openid_connect/token_refresh.py
--rw-r--r--   0        0        0     1393 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/src/simple_openid_connect/userinfo.py
--rw-r--r--   0        0        0      781 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/src/simple_openid_connect/utils.py
--rw-r--r--   0        0        0    16938 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/__init__.py
--rw-r--r--   0        0        0     2785 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/settings.py
--rw-r--r--   0        0        0     2586 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/conftest.py
--rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
--rw-r--r--   0        0        0      633 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
--rw-r--r--   0        0        0     5390 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_login.py
--rw-r--r--   0        0        0      687 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_logout.py
--rw-r--r--   0        0        0     1248 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/urls.py
--rw-r--r--   0        0        0      639 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/views.py
--rw-r--r--   0        0        0      415 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/wsgi.py
--rwxr-xr-x   0        0        0      675 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/django_test_project/manage.py
--rw-r--r--   0        0        0     1746 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/interactive_tests/conftest.py
--rw-r--r--   0        0        0     2001 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/interactive_tests/test_google.py
--rw-r--r--   0        0        0     1668 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_authorization_code_flow.py
--rw-r--r--   0        0        0     5139 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_client.py
--rw-r--r--   0        0        0      934 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_client_auth.py
--rw-r--r--   0        0        0     1378 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_direct_access_grant.py
--rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_discovery.py
--rw-r--r--   0        0        0      590 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_jwk.py
--rw-r--r--   0        0        0     2274 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_message_encoding.py
--rw-r--r--   0        0        0      581 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.4/tests/test_rp_initiated_logout.py
--rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 simple_openid_connect-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.gitattributes
+-rw-r--r--   0        0        0     1584 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      136 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.gitignore
+-rw-r--r--   0        0        0      795 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      177 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      298 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/DEVELOPMENT.md
+-rw-r--r--   0        0        0     1116 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4447 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/README.md
+-rw-r--r--   0        0        0      679 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/Makefile
+-rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      320 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/api.rst
+-rw-r--r--   0        0        0     1790 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/conf.py
+-rw-r--r--   0        0        0     5754 2023-05-25 12:12:58.573729 simple_openid_connect-0.2.5/docs/django-integration.rst
+-rw-r--r--   0        0        0     2615 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/drf-integration.rst
+-rw-r--r--   0        0        0      708 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/index.rst
+-rw-r--r--   0        0        0     1247 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/installation.rst
+-rw-r--r--   0        0        0     4868 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/usage.rst
+-rw-r--r--   0        0        0     2391 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/requirements.dev.txt
+-rw-r--r--   0        0        0      127 2023-06-01 11:14:30.712722 simple_openid_connect-0.2.5/src/simple_openid_connect/__init__.py
+-rw-r--r--   0        0        0     4204 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/src/simple_openid_connect/base_data.py
+-rw-r--r--   0        0        0    10682 2023-05-25 12:13:07.757788 simple_openid_connect-0.2.5/src/simple_openid_connect/client.py
+-rw-r--r--   0        0        0     3443 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/src/simple_openid_connect/client_authentication.py
+-rw-r--r--   0        0        0    57273 2023-05-25 12:16:39.699145 simple_openid_connect-0.2.5/src/simple_openid_connect/data.py
+-rw-r--r--   0        0        0     1819 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/discovery.py
+-rw-r--r--   0        0        0     1174 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/exceptions.py
+-rw-r--r--   0        0        0      343 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/__init__.py
+-rw-r--r--   0        0        0     5631 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
+-rw-r--r--   0        0        0     5823 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/client.py
+-rw-r--r--   0        0        0     2208 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/client.py
+-rw-r--r--   0        0        0       53 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/__init__.py
+-rw-r--r--   0        0        0     5467 2023-05-12 09:43:09.751399 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/apps.py
+-rw-r--r--   0        0        0     4555 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/decorators.py
+-rw-r--r--   0        0        0     2630 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/migrations/__init__.py
+-rw-r--r--   0        0        0     5728 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/models.py
+-rw-r--r--   0        0        0      381 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
+-rw-r--r--   0        0        0      729 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/urls.py
+-rw-r--r--   0        0        0     2338 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/user_mapping.py
+-rw-r--r--   0        0        0     4415 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/views.py
+-rw-r--r--   0        0        0      306 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/__init__.py
+-rw-r--r--   0        0        0     4648 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/authentication.py
+-rw-r--r--   0        0        0      957 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
+-rw-r--r--   0        0        0     2531 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/permissions.py
+-rw-r--r--   0        0        0      472 2023-05-12 09:43:09.751399 simple_openid_connect-0.2.5/src/simple_openid_connect/jwk.py
+-rw-r--r--   0        0        0      621 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/rp_initiated_logout.py
+-rw-r--r--   0        0        0     1509 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/token_introspection.py
+-rw-r--r--   0        0        0     1566 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/token_refresh.py
+-rw-r--r--   0        0        0     1393 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/src/simple_openid_connect/userinfo.py
+-rw-r--r--   0        0        0      781 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/src/simple_openid_connect/utils.py
+-rw-r--r--   0        0        0    16938 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/__init__.py
+-rw-r--r--   0        0        0     2785 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/settings.py
+-rw-r--r--   0        0        0     2586 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/conftest.py
+-rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
+-rw-r--r--   0        0        0      633 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
+-rw-r--r--   0        0        0     5247 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_login.py
+-rw-r--r--   0        0        0      687 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_logout.py
+-rw-r--r--   0        0        0     1248 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/urls.py
+-rw-r--r--   0        0        0      639 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/views.py
+-rw-r--r--   0        0        0      415 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/wsgi.py
+-rwxr-xr-x   0        0        0      675 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/manage.py
+-rw-r--r--   0        0        0     1746 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/interactive_tests/conftest.py
+-rw-r--r--   0        0        0     2001 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/interactive_tests/test_google.py
+-rw-r--r--   0        0        0     1668 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_authorization_code_flow.py
+-rw-r--r--   0        0        0     3115 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/tests/test_client.py
+-rw-r--r--   0        0        0      934 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_client_auth.py
+-rw-r--r--   0        0        0     1378 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_direct_access_grant.py
+-rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_discovery.py
+-rw-r--r--   0        0        0      590 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_jwk.py
+-rw-r--r--   0        0        0     2274 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_message_encoding.py
+-rw-r--r--   0        0        0      581 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_rp_initiated_logout.py
+-rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 simple_openid_connect-0.2.5/PKG-INFO
```

### Comparing `simple_openid_connect-0.2.4/.github/workflows/checks.yml` & `simple_openid_connect-0.2.5/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/.pre-commit-config.yaml` & `simple_openid_connect-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/LICENSE` & `simple_openid_connect-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/README.md` & `simple_openid_connect-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/docs/Makefile` & `simple_openid_connect-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/docs/conf.py` & `simple_openid_connect-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/docs/django-integration.rst` & `simple_openid_connect-0.2.5/docs/django-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/docs/drf-integration.rst` & `simple_openid_connect-0.2.5/docs/drf-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/docs/index.rst` & `simple_openid_connect-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/docs/installation.rst` & `simple_openid_connect-0.2.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/docs/usage.rst` & `simple_openid_connect-0.2.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/pyproject.toml` & `simple_openid_connect-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/base_data.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/base_data.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/client.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/client_authentication.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/client_authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/data.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/data.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/discovery.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/exceptions.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/flows/authorization_code_flow/__init__.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/flows/authorization_code_flow/client.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,35 +23,29 @@
 
     It is exposed via :data:`OpenidClient.authorization_code_flow <simple_openid_connect.client.OpenidClient.authorization_code_flow>`.
     """
 
     def __init__(self, base_client: "OpenidClient"):
         self._base_client = base_client
 
-    def start_authentication(
-        self, additional_redirect_args: Optional[Mapping[str, str]] = None
-    ) -> str:
+    def start_authentication(self) -> str:
         """
         Start the authentication process by constructing an appropriate :class:`AuthenticationRequest`, serializing it and
         returning a which the end user now needs to visit.
 
-        :param additional_redirect_args: Additional URL parameters that are added to the redirect uri.
-
         :raises ImpossibleOperationError: If the client has no redirect_uri configured and therefore cannot perform this operation.
 
         :returns: A URL to which the user agent should be redirected
         """
         if self._base_client.authentication_redirect_uri is None:
             raise ImpossibleOperationError(
                 "The client has no redirect_uri configured so no authentication flow can be started"
             )
 
         redirect_uri = furl(self._base_client.authentication_redirect_uri)
-        if additional_redirect_args is not None:
-            redirect_uri.args.update(additional_redirect_args)
 
         return impl.start_authentication(
             self._base_client.provider_config.authorization_endpoint,
             self._base_client.scope,
             self._base_client.client_auth.client_id,
             redirect_uri.tostr(),
         )
```

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/flows/direct_access_grant/__init__.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/flows/direct_access_grant/client.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/apps.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/apps.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/decorators.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/migrations/0001_initial.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/models.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/urls.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/user_mapping.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/user_mapping.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/django/views.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,38 +27,27 @@
 )
 from simple_openid_connect.integrations.django.apps import OpenidAppConfig
 from simple_openid_connect.integrations.django.models import OpenidUser
 
 logger = logging.getLogger(__name__)
 
 
-def _get_redirect_args(request: HttpRequest) -> Mapping[str, str]:
-    """
-    Calculate arguments which are appended to the redirect_uri
-    """
-    if "next" in request.GET.keys():
-        return {
-            "next": request.GET["next"],
-        }
-    return {}
-
-
 class InitLoginView(View):
     """
     The view which handles initiating a login.
 
     It essentially redirects the user agent to the Openid provider.
     """
 
     def get(self, request: HttpRequest) -> HttpResponse:
         logout(request)
+        if "next" in request.GET.keys():
+            request.session["login_redirect_url"] = request.GET["next"]
         client = OpenidAppConfig.get_instance().get_client(request)
-        redirect = client.authorization_code_flow.start_authentication(
-            additional_redirect_args=_get_redirect_args(request),
-        )
+        redirect = client.authorization_code_flow.start_authentication()
         return HttpResponseRedirect(redirect)
 
 
 class LoginCallbackView(View):
     """
     The view which handles login callbacks.
 
@@ -70,15 +59,14 @@
     """
 
     def get(self, request: HttpRequest) -> HttpResponse:
         client = OpenidAppConfig.get_instance().get_client(request)
 
         token_response = client.authorization_code_flow.handle_authentication_result(
             current_url=request.get_full_path(),
-            additional_redirect_args=_get_redirect_args(request),
         )
         if not isinstance(token_response, TokenSuccessResponse):
             return TemplateResponse(
                 request,
                 "simple_openid_connect/login_failed.html",
                 {
                     "token_response": token_response,
@@ -92,16 +80,18 @@
         )
 
         user = OpenidUser.objects.get_or_create_from_id_token(id_token)
         user.update_session(token_response)
         login(request, user.user, backend=settings.AUTHENTICATION_BACKENDS[0])
 
         # redirect to the next get parameter if present, otherwise to the configured default
-        if "next" in request.GET.keys():
-            return HttpResponseRedirect(redirect_to=request.GET["next"])
+        if "login_redirect_url" in request.session.keys():
+            return HttpResponseRedirect(
+                redirect_to=request.session["login_redirect_url"]
+            )
         else:
             return HttpResponseRedirect(
                 redirect_to=resolve_url(settings.LOGIN_REDIRECT_URL)
             )
 
 
 class LogoutView(View):
```

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/djangorestframework/authentication.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/integrations/djangorestframework/permissions.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/permissions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/rp_initiated_logout.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/token_introspection.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/token_introspection.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/token_refresh.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/token_refresh.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/userinfo.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/userinfo.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/src/simple_openid_connect/utils.py` & `simple_openid_connect-0.2.5/src/simple_openid_connect/utils.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/conftest.py` & `simple_openid_connect-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/settings.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/conftest.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_login.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,39 +98,37 @@
     response_mock.get(
         url="https://provider.example.com/auth",
         match=[
             matchers.query_param_matcher(
                 {
                     "client_id": settings.OPENID_CLIENT_ID,
                     "redirect_uri": settings.OPENID_BASE_URI
-                    + resolve_url(settings.OPENID_REDIRECT_URI)
-                    + "?next=%2Ftest-protected-view%2F",
+                    + resolve_url(settings.OPENID_REDIRECT_URI),
                     "response_type": "code",
                     "scope": settings.OPENID_SCOPE,
                 }
             )
         ],
         status=302,
         headers={
             "Location": settings.OPENID_BASE_URI
             + resolve_url(settings.OPENID_REDIRECT_URI)
-            + "?code=code.foobar123&next=%2Ftest-protected-view%2F"
+            + "?code=code.foobar123"
         },
     )
     response_mock.post(
         url="https://provider.example.com/token",
         match=[
             matchers.urlencoded_params_matcher(
                 {
                     "client_id": settings.OPENID_CLIENT_ID,
                     "code": "code.foobar123",
                     "grant_type": "authorization_code",
                     "redirect_uri": settings.OPENID_BASE_URI
-                    + resolve_url(settings.OPENID_REDIRECT_URI)
-                    + "?next=%2Ftest-protected-view%2F",
+                    + resolve_url(settings.OPENID_REDIRECT_URI),
                 }
             ),
             matchers.header_matcher(
                 {
                     "Authorization": f"Basic {client_auth}",
                 }
             ),
```

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/tests/test_logout.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/urls.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/django_test_project/views.py` & `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/django_test_project/manage.py` & `simple_openid_connect-0.2.5/tests/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/interactive_tests/conftest.py` & `simple_openid_connect-0.2.5/tests/interactive_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/interactive_tests/test_google.py` & `simple_openid_connect-0.2.5/tests/interactive_tests/test_google.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/test_authorization_code_flow.py` & `simple_openid_connect-0.2.5/tests/test_authorization_code_flow.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/test_client.py` & `simple_openid_connect-0.2.5/tests/test_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -32,80 +32,14 @@
     result = client.authorization_code_flow.handle_authentication_result(response.url)
 
     # assert
     assert result.access_token
     assert result.id_token
 
 
-def test_additional_redirect_args(
-    user_agent,
-    response_mock,
-    dummy_provider_config,
-):
-    # arrange
-    client = make_client()
-    response_mock.get(
-        url="https://provider.example.com/auth",
-        match=[
-            matchers.query_param_matcher(
-                {
-                    "client_id": "client-id",
-                    "redirect_uri": "https://app.example.com/login-callback?foo=bar",
-                    "response_type": "code",
-                    "scope": "openid",
-                }
-            )
-        ],
-        status=302,
-        headers={
-            "Location": "https://app.example.com/login-callback?code=code.foobar123&foo=bar"
-        },
-    )
-    response_mock.post(
-        url="https://provider.example.com/token",
-        match=[
-            matchers.urlencoded_params_matcher(
-                {
-                    "client_id": "client-id",
-                    "code": "code.foobar123",
-                    "grant_type": "authorization_code",
-                    "redirect_uri": "https://app.example.com/login-callback?foo=bar",
-                }
-            ),
-            matchers.header_matcher(
-                {
-                    "Authorization": f"Basic {b64encode(b'client-id:client-secret').decode()}"
-                }
-            ),
-        ],
-        json={
-            "access_token": "access_token.foobar123",
-            "token_type": "Bearer",
-            "id_token": "id_token.user1",
-        },
-    )
-
-    # act
-    auth_response = user_agent.naviagte_to(
-        client.authorization_code_flow.start_authentication(
-            additional_redirect_args={"foo": "bar"}
-        )
-    )
-    _code_response = client.authorization_code_flow.handle_authentication_result(
-        auth_response.url, additional_redirect_args={"foo": "bar"}
-    )
-
-    # assert
-    assert "foo=bar" in auth_response.url
-    assert any(
-        call.request.body and re.search(r"redirect_uri=.*foo%3Dbar", call.request.body)
-        for call in response_mock.calls
-    )
-
-
 def test_client_type(dummy_provider_config):
     # arrange
     public_client = OpenidClient.from_issuer_url(
         url="https://provider.example.com",
         authentication_redirect_uri="",
         client_id="test",
     )
```

### Comparing `simple_openid_connect-0.2.4/tests/test_client_auth.py` & `simple_openid_connect-0.2.5/tests/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/test_direct_access_grant.py` & `simple_openid_connect-0.2.5/tests/test_direct_access_grant.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/test_discovery.py` & `simple_openid_connect-0.2.5/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/test_jwk.py` & `simple_openid_connect-0.2.5/tests/test_jwk.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/test_message_encoding.py` & `simple_openid_connect-0.2.5/tests/test_message_encoding.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/tests/test_rp_initiated_logout.py` & `simple_openid_connect-0.2.5/tests/test_rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.4/PKG-INFO` & `simple_openid_connect-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_openid_connect
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simple and opinionated OpenID-Connect relying party and resource server implementation
 Author-email: Finn-Thorben Sell <dev@finn-thorben.me>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

