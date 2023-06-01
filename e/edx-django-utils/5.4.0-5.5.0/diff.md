# Comparing `tmp/edx-django-utils-5.4.0.tar.gz` & `tmp/edx-django-utils-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-django-utils-5.4.0.tar", last modified: Wed Apr 12 14:25:41 2023, max compression
+gzip compressed data, was "edx-django-utils-5.5.0.tar", last modified: Thu Jun  1 18:11:23 2023, max compression
```

## Comparing `edx-django-utils-5.4.0.tar` & `edx-django-utils-5.5.0.tar`

### file list

```diff
@@ -1,123 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    12775 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    26136 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6980 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.167745 edx-django-utils-5.4.0/edx_django_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/admin/
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/admin/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/cache/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/cache/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    12463 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/db/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4834 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/db/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/tests/test_queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/tests/test_read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/ip/
--rw-r--r--   0 runner    (1001) docker     (122)     7936 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/ip/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/test_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/logging/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/internal/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/internal/log_sensitive.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/logging/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_log_sensitive.py
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    21330 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3895 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    12959 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6238 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    11923 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/pluggable_override.py
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4082 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.167745 edx-django-utils-5.4.0/edx_django_utils/security/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/security/csp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/security/csp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/security/csp/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/security/csp/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4974 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/security/csp/tests/test_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/tests/test_pluggable_override.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     6487 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     7796 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/tests/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.167745 edx-django-utils-5.4.0/edx_django_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    26136 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    13109 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20617 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6848 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.278468 edx-django-utils-5.5.0/edx_django_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/admin/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/admin/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/cache/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12463 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/cache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils/db/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4834 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/db/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/tests/test_queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/db/tests/test_read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/ip/
+-rw-r--r--   0 runner    (1001) docker     (122)     7936 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/ip/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/test_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/logging/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/internal/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/internal/log_sensitive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.286468 edx-django-utils-5.5.0/edx_django_utils/logging/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_log_sensitive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22556 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3895 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.290468 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12959 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6238 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13475 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/monitoring/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/plugins/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/pluggable_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.278468 edx-django-utils-5.5.0/edx_django_utils/security/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/security/csp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/security/csp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/security/csp/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/security/csp/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4974 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/security/csp/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/tests/test_pluggable_override.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.294468 edx-django-utils-5.5.0/edx_django_utils/user/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6487 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7796 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/edx_django_utils/user/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/edx_django_utils/user/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.282468 edx-django-utils-5.5.0/edx_django_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20617 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3840 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-01 18:11:23.000000 edx-django-utils-5.5.0/edx_django_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:11:23.298468 edx-django-utils-5.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-01 18:11:18.000000 edx-django-utils-5.5.0/tests/test_models.py
```

### Comparing `edx-django-utils-5.4.0/CHANGELOG.rst` & `edx-django-utils-5.5.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,25 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[5.5.0] - 2023-06-01
+--------------------
+
+Changed
+~~~~~~~
+* Switched to ``sphinx-book-theme`` as the new standard theme across all Open
+  edX repos.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+* CookieMonitoringMiddleware will now remove cookies based on a ``COOKIE_PREFIXES_TO_REMOVE`` setting
+
+
 [5.4.0] - 2023-04-12
 --------------------
 
 Added
 ~~~~~
 
 * Added Content-Security-Policy response header middleware under ``security/csp``
```

### Comparing `edx-django-utils-5.4.0/LICENSE.txt` & `edx-django-utils-5.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/README.rst` & `edx-django-utils-5.5.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -128,18 +128,15 @@
 .. _Getting Help: https://openedx.org/getting-help
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
 can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-django-utils/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-django-utils/blob/master/.github/ISSUE_TEMPLATE.md>`_
```

### Comparing `edx-django-utils-5.4.0/edx_django_utils/admin/mixins.py` & `edx-django-utils-5.5.0/edx_django_utils/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/admin/tests/test_mixins.py` & `edx-django-utils-5.5.0/edx_django_utils/admin/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/cache/middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/cache/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_utils.py` & `edx-django-utils-5.5.0/edx_django_utils/cache/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/cache/utils.py` & `edx-django-utils-5.5.0/edx_django_utils/cache/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/db/queryset_utils.py` & `edx-django-utils-5.5.0/edx_django_utils/db/queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/db/read_replica.py` & `edx-django-utils-5.5.0/edx_django_utils/db/read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/db/tests/test_queryset_utils.py` & `edx-django-utils-5.5.0/edx_django_utils/db/tests/test_queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/db/tests/test_read_replica.py` & `edx-django-utils-5.5.0/edx_django_utils/db/tests/test_read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/ip/__init__.py` & `edx-django-utils-5.5.0/edx_django_utils/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/ip/internal/ip.py` & `edx-django-utils-5.5.0/edx_django_utils/ip/internal/ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/test_ip.py` & `edx-django-utils-5.5.0/edx_django_utils/ip/internal/tests/test_ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/logging/internal/filters.py` & `edx-django-utils-5.5.0/edx_django_utils/logging/internal/filters.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/logging/internal/log_sensitive.py` & `edx-django-utils-5.5.0/edx_django_utils/logging/internal/log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_log_sensitive.py` & `edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_logging.py` & `edx-django-utils-5.5.0/edx_django_utils/logging/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/__init__.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/utils.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/code_owner/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,24 +270,40 @@
 class CookieMonitoringMiddleware:
     """
     Middleware for monitoring the size and growth of all our cookies, to see if
     we're running into browser limits.
     """
     def __init__(self, get_response):
         self.get_response = get_response
+        # .. setting_name: COOKIE_PREFIXES_TO_REMOVE
+        # .. setting_default: []
+        # .. setting_description: A list of cookie prefixes. Any cookie starting with a prefix in this list
+        # will be manually removed from responses (i.e. set to expire in the past). This is useful for removing
+        # leftover instances of large cookies that have since been deprecated.
+        self.deprecated_cookie_prefixes = getattr(settings, "COOKIE_PREFIXES_TO_REMOVE", [])
+        if not isinstance(self.deprecated_cookie_prefixes, list):
+            log.warning(f"COOKIE_PREFIXES_TO_REMOVE must be a list of (name, domain) tuples,"
+                        f" not {type(self.deprecated_cookie_prefixes)}. No cookies will be removed.")
+            self.deprecated_cookie_prefixes = []
 
     def __call__(self, request):
         # Monitor at request-time to skip any cookies that may be added during the request.
         log_message = None
         try:
             log_message = self.get_log_message_and_monitor_cookies(request)
         except BaseException:
             log.exception("Unexpected error logging and monitoring cookies.")
 
         response = self.get_response(request)
+        for deprecated_cookie_prefix, domain in self.deprecated_cookie_prefixes:
+            for cookie_name in request.COOKIES.keys():
+                if cookie_name.startswith(deprecated_cookie_prefix):
+                    log.info(f"Deleting cookie {cookie_name} in domain {domain}")
+                    # delete_cookie sets the expiration date to the Unix epoch
+                    response.delete_cookie(cookie_name, domain=domain)
 
         # Delay logging until response-time so that the user id can be included in the log message.
         if log_message:
             log.info(log_message)
 
         return response
```

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/transactions.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/transactions.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/utils.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -276,14 +276,46 @@
         mock_request.META = Mock()
         mock_request.META.side_effect = Exception("Some exception")
 
         middleware(mock_request)
 
         mock_logger.exception.assert_called_once_with("Unexpected error logging and monitoring cookies.")
 
+    @override_settings(COOKIE_PREFIXES_TO_REMOVE=[('old_cookie', 'localhost')])
+    def test_deprecated_cookies_removed(self):
+        self.mock_response.reset_mock()
+        middleware = CookieMonitoringMiddleware(lambda _: self.mock_response)
+        cookies_dict = {'old_cookie': 'x',
+                        'ok_cookie': 'x',
+                        'old_cookie_9000': 'x'
+                        }
+        response = middleware(self.get_mock_request(cookies_dict))
+
+        assert response == self.mock_response
+        assert response.delete_cookie.mock_calls == [
+            call('old_cookie',  domain='localhost'),
+            call('old_cookie_9000', domain='localhost'),
+        ]
+
+    @override_settings(COOKIE_PREFIXES_TO_REMOVE='old_cookie')
+    @patch('edx_django_utils.monitoring.internal.middleware.log', autospec=True)
+    def test_bad_cookie_prefix_setting(self, mock_log):
+        self.mock_response.reset_mock()
+        middleware = CookieMonitoringMiddleware(lambda _: self.mock_response)
+        cookies_dict = {'old_cookie': 'x',
+                        'ok_cookie': 'x',
+                        'old_cookie_9000': 'x'
+                        }
+        response = middleware(self.get_mock_request(cookies_dict))
+
+        assert response == self.mock_response
+        mock_log.warning.assert_called_once_with("COOKIE_PREFIXES_TO_REMOVE must be a list of (name, domain) tuples,"
+                                                 " not <class 'str'>. No cookies will be removed.")
+        response.delete_cookie.assert_not_called()
+
     def get_mock_request(self, cookies_dict):
         """
         Return mock request with the provided cookies in the header.
         """
         factory = RequestFactory()
         for name, value in cookies_dict.items():
             factory.cookies[name] = value
```

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_utils.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/monitoring/utils.py` & `edx-django-utils-5.5.0/edx_django_utils/monitoring/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/__init__.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/constants.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/constants.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/pluggable_override.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_apps.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_apps.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_contexts.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_contexts.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 def get_plugins_view_context(project_type, view_name, existing_context=None):
     """
     Returns a dict of additional view context. Will check if any plugin apps
     have that view in their view_context_config, and if so will call their
     selected function to get their context dicts.
 
     Params:
-        project_type: a string that determines which project (lms or studio) the view is being called in. See the
-            ProjectType enum in plugins/constants.py for valid options
+        project_type: a string that determines which project the view is being called in. See the
+            ProjectType enum in
+            https://github.com/openedx/edx-platform/blob/2dc79bcab42dafed2c122eb808cdd5604327c890/openedx/core/
+            djangoapps/plugins/constants.py#L14
+            for valid options for edx-platform.
         view_name: a string that determines which view needs the additional context. These are globally unique and
             noted in the api.py in the view's app.
         existing_context: a dictionary which includes all of the data that the page was going to render with prior
             to the addition of each plugin's context. This is what will be passed to plugins so they may choose
             what data to add to the view.
     """
     aggregate_context = {"plugins": {}}
```

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_manager.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_settings.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_signals.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_signals.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_urls.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/plugin_urls.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/plugins/utils.py` & `edx-django-utils-5.5.0/edx_django_utils/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/security/csp/middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/security/csp/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/security/csp/tests/test_middleware.py` & `edx-django-utils-5.5.0/edx_django_utils/security/csp/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/tests/test_pluggable_override.py` & `edx-django-utils-5.5.0/edx_django_utils/tests/test_pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/user/__init__.py` & `edx-django-utils-5.5.0/edx_django_utils/user/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_group.py` & `edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_user.py` & `edx-django-utils-5.5.0/edx_django_utils/user/management/commands/manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_group.py` & `edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_user.py` & `edx-django-utils-5.5.0/edx_django_utils/user/management/tests/test_manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils/user/tests/test_user.py` & `edx-django-utils-5.5.0/edx_django_utils/user/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/edx_django_utils.egg-info/SOURCES.txt` & `edx-django-utils-5.5.0/edx_django_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -83,8 +83,9 @@
 edx_django_utils/user/management/commands/manage_user.py
 edx_django_utils/user/management/tests/__init__.py
 edx_django_utils/user/management/tests/test_manage_group.py
 edx_django_utils/user/management/tests/test_manage_user.py
 edx_django_utils/user/tests/__init__.py
 edx_django_utils/user/tests/test_user.py
 requirements/base.in
-requirements/constraints.txt
+requirements/constraints.txt
+tests/test_models.py
```

### Comparing `edx-django-utils-5.4.0/requirements/base.in` & `edx-django-utils-5.5.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/requirements/constraints.txt` & `edx-django-utils-5.5.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.4.0/setup.py` & `edx-django-utils-5.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 CHANGELOG = open(os.path.join(os.path.dirname(__file__), 'CHANGELOG.rst'), encoding="utf8").read()
 
 setup(
     name='edx-django-utils',
     version=VERSION,
     description="""EdX utilities for Django Application development.""",
     long_description=README + '\n\n' + CHANGELOG,
+    long_description_content_type="text/x-rst",
     author='edX',
     author_email='oscm@edx.org',
     url='https://github.com/openedx/edx-django-utils',
     packages=[
         'edx_django_utils',
     ],
     include_package_data=True,
```

