# Comparing `tmp/cdktf-cdktf-provider-datadog-6.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-datadog-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-datadog-6.0.3.tar", last modified: Sat May  6 03:21:37 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-datadog-6.0.4.tar", last modified: Thu Jun  1 14:24:44 2023, max compression
```

## Comparing `cdktf-cdktf-provider-datadog-6.0.3.tar` & `cdktf-cdktf-provider-datadog-6.0.4.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)    16012 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     4161 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3205 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     7494 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.255744 cdktf-cdktf-provider-datadog-6.0.3/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.263744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/
--rw-r--r--   0 runner    (1000) runner    (1000)     9611 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.263744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/_jsii/
--rw-r--r--   0 runner    (1000) runner    (1000)      417 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/_jsii/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)  3159911 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/_jsii/provider-datadog@6.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.267744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/api_key/
--rw-r--r--   0 runner    (1000) runner    (1000)    14801 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/api_key/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.267744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/application_key/
--rw-r--r--   0 runner    (1000) runner    (1000)    17867 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/application_key/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.267744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/authn_mapping/
--rw-r--r--   0 runner    (1000) runner    (1000)    21778 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/authn_mapping/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.267744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/child_organization/
--rw-r--r--   0 runner    (1000) runner    (1000)    93760 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/child_organization/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.267744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/cloud_configuration_rule/
--rw-r--r--   0 runner    (1000) runner    (1000)    41659 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/cloud_configuration_rule/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.267744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/cloud_workload_security_agent_rule/
--rw-r--r--   0 runner    (1000) runner    (1000)    26263 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/cloud_workload_security_agent_rule/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.267744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard/
--rw-r--r--   0 runner    (1000) runner    (1000) 17833330 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard_json/
--rw-r--r--   0 runner    (1000) runner    (1000)    23230 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard_json/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard_list/
--rw-r--r--   0 runner    (1000) runner    (1000)    35219 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard_list/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_api_key/
--rw-r--r--   0 runner    (1000) runner    (1000)    18145 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_api_key/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_application_key/
--rw-r--r--   0 runner    (1000) runner    (1000)    18398 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_application_key/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_cloud_workload_security_agent_rules/
--rw-r--r--   0 runner    (1000) runner    (1000)    26601 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_cloud_workload_security_agent_rules/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard/
--rw-r--r--   0 runner    (1000) runner    (1000)    18207 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard_list/
--rw-r--r--   0 runner    (1000) runner    (1000)    17950 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard_list/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_hosts/
--rw-r--r--   0 runner    (1000) runner    (1000)    45646 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_hosts/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_integration_aws_logs_services/
--rw-r--r--   0 runner    (1000) runner    (1000)    25937 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_integration_aws_logs_services/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_ip_ranges/
--rw-r--r--   0 runner    (1000) runner    (1000)    16680 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_ip_ranges/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_archives_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    16158 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_archives_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes/
--rw-r--r--   0 runner    (1000) runner    (1000)    54018 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    16135 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_pipelines/
--rw-r--r--   0 runner    (1000) runner    (1000)    37798 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitor/
--rw-r--r--   0 runner    (1000) runner    (1000)    68201 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitor/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitor_config_policies/
--rw-r--r--   0 runner    (1000) runner    (1000)    36038 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitor_config_policies/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitors/
--rw-r--r--   0 runner    (1000) runner    (1000)    33542 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitors/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_permissions/
--rw-r--r--   0 runner    (1000) runner    (1000)    19782 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_permissions/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_role/
--rw-r--r--   0 runner    (1000) runner    (1000)    18064 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_role/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_roles/
--rw-r--r--   0 runner    (1000) runner    (1000)    27199 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_roles/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_rum_application/
--rw-r--r--   0 runner    (1000) runner    (1000)    21784 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_rum_application/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.283744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_filters/
--rw-r--r--   0 runner    (1000) runner    (1000)    36346 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_filters/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_rules/
--rw-r--r--   0 runner    (1000) runner    (1000)   119828 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_rules/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_group_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    13473 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_group_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_standard_pattern/
--rw-r--r--   0 runner    (1000) runner    (1000)    19236 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_standard_pattern/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objective/
--rw-r--r--   0 runner    (1000) runner    (1000)    34552 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objective/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objectives/
--rw-r--r--   0 runner    (1000) runner    (1000)    36073 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objectives/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_global_variable/
--rw-r--r--   0 runner    (1000) runner    (1000)    18603 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_global_variable/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_locations/
--rw-r--r--   0 runner    (1000) runner    (1000)    16190 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_locations/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_test/
--rw-r--r--   0 runner    (1000) runner    (1000)    18557 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_test/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_user/
--rw-r--r--   0 runner    (1000) runner    (1000)    18050 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_user/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/downtime/
--rw-r--r--   0 runner    (1000) runner    (1000)    64843 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/downtime/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws/
--rw-r--r--   0 runner    (1000) runner    (1000)    51112 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_lambda_arn/
--rw-r--r--   0 runner    (1000) runner    (1000)    20771 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_lambda_arn/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_log_collection/
--rw-r--r--   0 runner    (1000) runner    (1000)    21521 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_log_collection/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_tag_filter/
--rw-r--r--   0 runner    (1000) runner    (1000)    23467 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_tag_filter/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_azure/
--rw-r--r--   0 runner    (1000) runner    (1000)    29133 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_azure/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_cloudflare_account/
--rw-r--r--   0 runner    (1000) runner    (1000)    20145 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_cloudflare_account/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_confluent_account/
--rw-r--r--   0 runner    (1000) runner    (1000)    20414 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_confluent_account/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_confluent_resource/
--rw-r--r--   0 runner    (1000) runner    (1000)    23339 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_confluent_resource/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_fastly_account/
--rw-r--r--   0 runner    (1000) runner    (1000)    17299 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_fastly_account/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_fastly_service/
--rw-r--r--   0 runner    (1000) runner    (1000)    20314 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_fastly_service/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_gcp/
--rw-r--r--   0 runner    (1000) runner    (1000)    37316 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_gcp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_opsgenie_service_object/
--rw-r--r--   0 runner    (1000) runner    (1000)    26906 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_opsgenie_service_object/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_pagerduty/
--rw-r--r--   0 runner    (1000) runner    (1000)    23238 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_pagerduty/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_pagerduty_service_object/
--rw-r--r--   0 runner    (1000) runner    (1000)    22090 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_pagerduty_service_object/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_slack_channel/
--rw-r--r--   0 runner    (1000) runner    (1000)    38009 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_slack_channel/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/ip_allowlist/
--rw-r--r--   0 runner    (1000) runner    (1000)    35459 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/ip_allowlist/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_archive/
--rw-r--r--   0 runner    (1000) runner    (1000)    74888 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_archive/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_archive_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    19158 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_archive_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.287745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_custom_pipeline/
--rw-r--r--   0 runner    (1000) runner    (1000)   685611 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_custom_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_index/
--rw-r--r--   0 runner    (1000) runner    (1000)    70313 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_index/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_index_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    20604 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_index_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_integration_pipeline/
--rw-r--r--   0 runner    (1000) runner    (1000)    19047 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_integration_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_metric/
--rw-r--r--   0 runner    (1000) runner    (1000)    56357 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_metric/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_pipeline_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    21182 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_pipeline_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/metric_metadata/
--rw-r--r--   0 runner    (1000) runner    (1000)    32635 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/metric_metadata/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/metric_tag_configuration/
--rw-r--r--   0 runner    (1000) runner    (1000)    45139 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/metric_tag_configuration/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor/
--rw-r--r--   0 runner    (1000) runner    (1000)   262670 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor_config_policy/
--rw-r--r--   0 runner    (1000) runner    (1000)    31873 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor_config_policy/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor_json/
--rw-r--r--   0 runner    (1000) runner    (1000)    19969 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor_json/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/organization_settings/
--rw-r--r--   0 runner    (1000) runner    (1000)    72504 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/organization_settings/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/provider/
--rw-r--r--   0 runner    (1000) runner    (1000)    33744 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/provider/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/role/
--rw-r--r--   0 runner    (1000) runner    (1000)    36465 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/role/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/rum_application/
--rw-r--r--   0 runner    (1000) runner    (1000)    20421 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/rum_application/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_default_rule/
--rw-r--r--   0 runner    (1000) runner    (1000)    66517 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_default_rule/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_filter/
--rw-r--r--   0 runner    (1000) runner    (1000)    44431 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_filter/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_rule/
--rw-r--r--   0 runner    (1000) runner    (1000)   200772 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_rule/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group/
--rw-r--r--   0 runner    (1000) runner    (1000)    34299 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    15977 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_rule/
--rw-r--r--   0 runner    (1000) runner    (1000)    56417 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_rule/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_account/
--rw-r--r--   0 runner    (1000) runner    (1000)    25564 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_account/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_definition_yaml/
--rw-r--r--   0 runner    (1000) runner    (1000)    18457 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_definition_yaml/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.291745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_level_objective/
--rw-r--r--   0 runner    (1000) runner    (1000)    78433 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_level_objective/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/slo_correction/
--rw-r--r--   0 runner    (1000) runner    (1000)    35232 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/slo_correction/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_global_variable/
--rw-r--r--   0 runner    (1000) runner    (1000)    76860 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_global_variable/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_private_location/
--rw-r--r--   0 runner    (1000) runner    (1000)    32571 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_private_location/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_test/
--rw-r--r--   0 runner    (1000) runner    (1000)   777865 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_test/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/user/
--rw-r--r--   0 runner    (1000) runner    (1000)    28812 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/user/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/webhook/
--rw-r--r--   0 runner    (1000) runner    (1000)    26885 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/webhook/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.295745 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/webhook_custom_variable/
--rw-r--r--   0 runner    (1000) runner    (1000)    23008 2023-05-06 03:21:20.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/webhook_custom_variable/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 03:21:37.263744 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     4161 2023-05-06 03:21:37.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     6623 2023-05-06 03:21:37.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 03:21:37.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      106 2023-05-06 03:21:37.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2023-05-06 03:21:37.000000 cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16012 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     4328 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3372 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7494 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.924781 cdktf-cdktf-provider-datadog-6.0.4/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.928781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/
+-rw-r--r--   0 runner    (1000) runner    (1000)     9778 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.932781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/_jsii/
+-rw-r--r--   0 runner    (1000) runner    (1000)      417 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/_jsii/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)  3171312 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/_jsii/provider-datadog@6.0.4.jsii.tgz
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.932781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/api_key/
+-rw-r--r--   0 runner    (1000) runner    (1000)    14801 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/api_key/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.932781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/application_key/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17867 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/application_key/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.932781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/authn_mapping/
+-rw-r--r--   0 runner    (1000) runner    (1000)    21778 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/authn_mapping/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.936781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/child_organization/
+-rw-r--r--   0 runner    (1000) runner    (1000)    93760 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/child_organization/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.936781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/cloud_configuration_rule/
+-rw-r--r--   0 runner    (1000) runner    (1000)    41659 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/cloud_configuration_rule/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.936781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/cloud_workload_security_agent_rule/
+-rw-r--r--   0 runner    (1000) runner    (1000)    26263 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/cloud_workload_security_agent_rule/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.936781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard/
+-rw-r--r--   0 runner    (1000) runner    (1000) 17833330 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard_json/
+-rw-r--r--   0 runner    (1000) runner    (1000)    23230 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard_json/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard_list/
+-rw-r--r--   0 runner    (1000) runner    (1000)    35219 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard_list/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_api_key/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18145 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_api_key/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_application_key/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18398 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_application_key/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_cloud_workload_security_agent_rules/
+-rw-r--r--   0 runner    (1000) runner    (1000)    26601 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_cloud_workload_security_agent_rules/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18207 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard_list/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17950 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard_list/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_hosts/
+-rw-r--r--   0 runner    (1000) runner    (1000)    45800 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_hosts/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_integration_aws_logs_services/
+-rw-r--r--   0 runner    (1000) runner    (1000)    25937 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_integration_aws_logs_services/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_ip_ranges/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16680 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_ip_ranges/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_archives_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16158 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_archives_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes/
+-rw-r--r--   0 runner    (1000) runner    (1000)    54018 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16135 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_pipelines/
+-rw-r--r--   0 runner    (1000) runner    (1000)    37798 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitor/
+-rw-r--r--   0 runner    (1000) runner    (1000)    68201 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitor/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitor_config_policies/
+-rw-r--r--   0 runner    (1000) runner    (1000)    36038 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitor_config_policies/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitors/
+-rw-r--r--   0 runner    (1000) runner    (1000)    33542 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitors/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_permissions/
+-rw-r--r--   0 runner    (1000) runner    (1000)    19782 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_permissions/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_role/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18064 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_role/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_roles/
+-rw-r--r--   0 runner    (1000) runner    (1000)    27199 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_roles/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_rum_application/
+-rw-r--r--   0 runner    (1000) runner    (1000)    21784 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_rum_application/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_filters/
+-rw-r--r--   0 runner    (1000) runner    (1000)    36346 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_filters/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.952781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_rules/
+-rw-r--r--   0 runner    (1000) runner    (1000)   119828 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_rules/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_group_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13473 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_group_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_standard_pattern/
+-rw-r--r--   0 runner    (1000) runner    (1000)    19236 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_standard_pattern/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objective/
+-rw-r--r--   0 runner    (1000) runner    (1000)    34552 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objective/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objectives/
+-rw-r--r--   0 runner    (1000) runner    (1000)    36073 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objectives/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_global_variable/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18603 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_global_variable/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_locations/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16190 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_locations/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_test/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18557 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_test/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_user/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18050 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_user/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/downtime/
+-rw-r--r--   0 runner    (1000) runner    (1000)    64843 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/downtime/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws/
+-rw-r--r--   0 runner    (1000) runner    (1000)    51112 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_lambda_arn/
+-rw-r--r--   0 runner    (1000) runner    (1000)    20771 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_lambda_arn/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_log_collection/
+-rw-r--r--   0 runner    (1000) runner    (1000)    21521 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_log_collection/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_tag_filter/
+-rw-r--r--   0 runner    (1000) runner    (1000)    23467 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_tag_filter/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_azure/
+-rw-r--r--   0 runner    (1000) runner    (1000)    29133 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_azure/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_cloudflare_account/
+-rw-r--r--   0 runner    (1000) runner    (1000)    20145 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_cloudflare_account/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_confluent_account/
+-rw-r--r--   0 runner    (1000) runner    (1000)    20414 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_confluent_account/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_confluent_resource/
+-rw-r--r--   0 runner    (1000) runner    (1000)    23339 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_confluent_resource/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_fastly_account/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17299 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_fastly_account/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_fastly_service/
+-rw-r--r--   0 runner    (1000) runner    (1000)    20314 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_fastly_service/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_gcp/
+-rw-r--r--   0 runner    (1000) runner    (1000)    37316 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_gcp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_opsgenie_service_object/
+-rw-r--r--   0 runner    (1000) runner    (1000)    26906 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_opsgenie_service_object/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_pagerduty/
+-rw-r--r--   0 runner    (1000) runner    (1000)    23238 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_pagerduty/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_pagerduty_service_object/
+-rw-r--r--   0 runner    (1000) runner    (1000)    22090 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_pagerduty_service_object/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_slack_channel/
+-rw-r--r--   0 runner    (1000) runner    (1000)    38009 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_slack_channel/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/ip_allowlist/
+-rw-r--r--   0 runner    (1000) runner    (1000)    35459 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/ip_allowlist/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_archive/
+-rw-r--r--   0 runner    (1000) runner    (1000)    74888 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_archive/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_archive_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    19158 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_archive_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.956781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_custom_pipeline/
+-rw-r--r--   0 runner    (1000) runner    (1000)   685611 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_custom_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_index/
+-rw-r--r--   0 runner    (1000) runner    (1000)    70313 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_index/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_index_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    20604 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_index_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_integration_pipeline/
+-rw-r--r--   0 runner    (1000) runner    (1000)    19047 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_integration_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_metric/
+-rw-r--r--   0 runner    (1000) runner    (1000)    56357 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_metric/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_pipeline_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    21182 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_pipeline_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/metric_metadata/
+-rw-r--r--   0 runner    (1000) runner    (1000)    32635 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/metric_metadata/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/metric_tag_configuration/
+-rw-r--r--   0 runner    (1000) runner    (1000)    45139 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/metric_tag_configuration/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor/
+-rw-r--r--   0 runner    (1000) runner    (1000)   262670 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor_config_policy/
+-rw-r--r--   0 runner    (1000) runner    (1000)    31873 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor_config_policy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor_json/
+-rw-r--r--   0 runner    (1000) runner    (1000)    19969 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor_json/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/organization_settings/
+-rw-r--r--   0 runner    (1000) runner    (1000)    72504 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/organization_settings/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/provider/
+-rw-r--r--   0 runner    (1000) runner    (1000)    33744 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/provider/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/role/
+-rw-r--r--   0 runner    (1000) runner    (1000)    36465 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/role/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/rum_application/
+-rw-r--r--   0 runner    (1000) runner    (1000)    20421 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/rum_application/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_default_rule/
+-rw-r--r--   0 runner    (1000) runner    (1000)    66517 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_default_rule/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_filter/
+-rw-r--r--   0 runner    (1000) runner    (1000)    44431 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_filter/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_rule/
+-rw-r--r--   0 runner    (1000) runner    (1000)   200772 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_rule/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group/
+-rw-r--r--   0 runner    (1000) runner    (1000)    34299 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    15977 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_rule/
+-rw-r--r--   0 runner    (1000) runner    (1000)    56417 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_rule/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_account/
+-rw-r--r--   0 runner    (1000) runner    (1000)    25564 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_account/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_definition_yaml/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18457 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_definition_yaml/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_level_objective/
+-rw-r--r--   0 runner    (1000) runner    (1000)    78433 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_level_objective/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/slo_correction/
+-rw-r--r--   0 runner    (1000) runner    (1000)    35232 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/slo_correction/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.960781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_global_variable/
+-rw-r--r--   0 runner    (1000) runner    (1000)    76860 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_global_variable/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_private_location/
+-rw-r--r--   0 runner    (1000) runner    (1000)    32571 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_private_location/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_test/
+-rw-r--r--   0 runner    (1000) runner    (1000)   777955 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_test/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/user/
+-rw-r--r--   0 runner    (1000) runner    (1000)    28812 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/user/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/webhook/
+-rw-r--r--   0 runner    (1000) runner    (1000)    26885 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/webhook/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.964781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/webhook_custom_variable/
+-rw-r--r--   0 runner    (1000) runner    (1000)    23008 2023-06-01 14:24:30.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/webhook_custom_variable/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-01 14:24:44.932781 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4328 2023-06-01 14:24:44.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     6623 2023-06-01 14:24:44.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-01 14:24:44.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      106 2023-06-01 14:24:44.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2023-06-01 14:24:44.000000 cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/LICENSE` & `cdktf-cdktf-provider-datadog-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/PKG-INFO` & `cdktf-cdktf-provider-datadog-6.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-datadog
-Version: 6.0.3
+Version: 6.0.4
 Summary: Prebuilt datadog Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-datadog.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-datadog.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform datadog Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform datadog Provider](https://github.com/terraform-providers/terraform-provider-datadog)
+* [Terraform datadog Provider](https://registry.terraform.io/providers/DataDog/datadog/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-datadog/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/README.md` & `cdktf-cdktf-provider-datadog-6.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform datadog Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform datadog Provider](https://github.com/terraform-providers/terraform-provider-datadog)
+* [Terraform datadog Provider](https://registry.terraform.io/providers/DataDog/datadog/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-datadog/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/setup.py` & `cdktf-cdktf-provider-datadog-6.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-datadog",
-    "version": "6.0.3",
+    "version": "6.0.4",
     "description": "Prebuilt datadog Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-datadog.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -110,25 +110,25 @@
         "cdktf_cdktf_provider_datadog.synthetics_test",
         "cdktf_cdktf_provider_datadog.user",
         "cdktf_cdktf_provider_datadog.webhook",
         "cdktf_cdktf_provider_datadog.webhook_custom_variable"
     ],
     "package_data": {
         "cdktf_cdktf_provider_datadog._jsii": [
-            "provider-datadog@6.0.3.jsii.tgz"
+            "provider-datadog@6.0.4.jsii.tgz"
         ],
         "cdktf_cdktf_provider_datadog": [
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

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform datadog Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform datadog Provider](https://github.com/terraform-providers/terraform-provider-datadog)
+* [Terraform datadog Provider](https://registry.terraform.io/providers/DataDog/datadog/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-datadog/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/api_key/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/api_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/application_key/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/application_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/authn_mapping/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/authn_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/child_organization/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/child_organization/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/cloud_configuration_rule/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/cloud_configuration_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/cloud_workload_security_agent_rule/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/cloud_workload_security_agent_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard_json/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard_json/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/dashboard_list/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/dashboard_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_api_key/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_api_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_application_key/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_application_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_cloud_workload_security_agent_rules/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_cloud_workload_security_agent_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard_list/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_dashboard_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_hosts/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_hosts/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,16 +111,16 @@
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
     @jsii.member(jsii_name="hostList")
-    def host_list(self) -> "DataDatadogHostsHostListList":
-        return typing.cast("DataDatadogHostsHostListList", jsii.get(self, "hostList"))
+    def host_list(self) -> "DataDatadogHostsHostListStructList":
+        return typing.cast("DataDatadogHostsHostListStructList", jsii.get(self, "hostList"))
 
     @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
     @builtins.property
@@ -437,108 +437,14 @@
     def __repr__(self) -> str:
         return "DataDatadogHostsConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-datadog.dataDatadogHosts.DataDatadogHostsHostList",
-    jsii_struct_bases=[],
-    name_mapping={},
-)
-class DataDatadogHostsHostList:
-    def __init__(self) -> None:
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "DataDatadogHostsHostList(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-class DataDatadogHostsHostListList(
-    _cdktf_9a9027ec.ComplexList,
-    metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-datadog.dataDatadogHosts.DataDatadogHostsHostListList",
-):
-    def __init__(
-        self,
-        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-        terraform_attribute: builtins.str,
-        wraps_set: builtins.bool,
-    ) -> None:
-        '''
-        :param terraform_resource: The parent resource.
-        :param terraform_attribute: The attribute on the parent resource this class is referencing.
-        :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ac82a341ccc60d366c2d89d137c9de3d02c7eb70ce5d30376a4f863da7b28a00)
-            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
-            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
-            check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
-        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
-
-    @jsii.member(jsii_name="get")
-    def get(self, index: jsii.Number) -> "DataDatadogHostsHostListOutputReference":
-        '''
-        :param index: the index of the item to return.
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__106e4837c73c581cc4825e9d60420d809009548a3b0895c885c00fc9d6f218cb)
-            check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataDatadogHostsHostListOutputReference", jsii.invoke(self, "get", [index]))
-
-    @builtins.property
-    @jsii.member(jsii_name="terraformAttribute")
-    def _terraform_attribute(self) -> builtins.str:
-        '''The attribute on the parent resource this class is referencing.'''
-        return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
-
-    @_terraform_attribute.setter
-    def _terraform_attribute(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6989f39e6826b4b2918fd6a637588d8756abadfedad67a490721a8fb83f43ed1)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "terraformAttribute", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="terraformResource")
-    def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
-        '''The parent resource.'''
-        return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
-
-    @_terraform_resource.setter
-    def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9bb40108fbd0dfc3fe83d69e90dfbd86618e75a725ad62ddfb06aa26f58a0617)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "terraformResource", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="wrapsSet")
-    def _wraps_set(self) -> builtins.bool:
-        '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
-        return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
-
-    @_wraps_set.setter
-    def _wraps_set(self, value: builtins.bool) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a1eeba0ecc84304df2d34cdd2d9e551f900f909b0288a4b901a2a735a64128c9)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "wrapsSet", value)
-
-
-@jsii.data_type(
     jsii_type="@cdktf/provider-datadog.dataDatadogHosts.DataDatadogHostsHostListMeta",
     jsii_struct_bases=[],
     name_mapping={},
 )
 class DataDatadogHostsHostListMeta:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -704,18 +610,115 @@
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__87e2f2bec7fc0f90e7fb49d83a77be82ebabe6d93587ac3b06d66dd57d5630e7)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
-class DataDatadogHostsHostListOutputReference(
+@jsii.data_type(
+    jsii_type="@cdktf/provider-datadog.dataDatadogHosts.DataDatadogHostsHostListStruct",
+    jsii_struct_bases=[],
+    name_mapping={},
+)
+class DataDatadogHostsHostListStruct:
+    def __init__(self) -> None:
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DataDatadogHostsHostListStruct(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class DataDatadogHostsHostListStructList(
+    _cdktf_9a9027ec.ComplexList,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-datadog.dataDatadogHosts.DataDatadogHostsHostListStructList",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        wraps_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6fc9bf6ecc1fd07bae1c9eb39e5d315ae5d453b93b45208d9d13072b75a4c46c)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
+
+    @jsii.member(jsii_name="get")
+    def get(
+        self,
+        index: jsii.Number,
+    ) -> "DataDatadogHostsHostListStructOutputReference":
+        '''
+        :param index: the index of the item to return.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2d9c7f870c87e636cef1652e59df0f94afbfe6aff482f8512df5e024de8e61a9)
+            check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+        return typing.cast("DataDatadogHostsHostListStructOutputReference", jsii.invoke(self, "get", [index]))
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformAttribute")
+    def _terraform_attribute(self) -> builtins.str:
+        '''The attribute on the parent resource this class is referencing.'''
+        return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
+
+    @_terraform_attribute.setter
+    def _terraform_attribute(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bcc0e2a55bc62e2e5f105b1b45c9e7a5eed7dbee42026b28b590f479020e386b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformAttribute", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformResource")
+    def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
+        '''The parent resource.'''
+        return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
+
+    @_terraform_resource.setter
+    def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a25ce29aecf25c4c686cb4ff504956663c727bcbf00e1e712e5555d9a2274dfb)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformResource", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="wrapsSet")
+    def _wraps_set(self) -> builtins.bool:
+        '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
+        return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
+
+    @_wraps_set.setter
+    def _wraps_set(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__dc791cd85041a2a7e1aee3683b9dec8acfe38821b0ab8e574fdd1a78135a7866)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "wrapsSet", value)
+
+
+class DataDatadogHostsHostListStructOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-datadog.dataDatadogHosts.DataDatadogHostsHostListOutputReference",
+    jsii_type="@cdktf/provider-datadog.dataDatadogHosts.DataDatadogHostsHostListStructOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -723,15 +726,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c86ebad0847f85ccaae23a8bb590a534f0164e844147c6991319797b328dc2d6)
+            type_hints = typing.get_type_hints(_typecheckingstub__7cc5f6e256c6f31b54c277b7d6b25a4f2d09d50ba213b73aa0274fdc1da14b2a)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -797,35 +800,38 @@
     @builtins.property
     @jsii.member(jsii_name="up")
     def up(self) -> _cdktf_9a9027ec.IResolvable:
         return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "up"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataDatadogHostsHostList]:
-        return typing.cast(typing.Optional[DataDatadogHostsHostList], jsii.get(self, "internalValue"))
+    def internal_value(self) -> typing.Optional[DataDatadogHostsHostListStruct]:
+        return typing.cast(typing.Optional[DataDatadogHostsHostListStruct], jsii.get(self, "internalValue"))
 
     @internal_value.setter
-    def internal_value(self, value: typing.Optional[DataDatadogHostsHostList]) -> None:
+    def internal_value(
+        self,
+        value: typing.Optional[DataDatadogHostsHostListStruct],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__18a35da22ef74d2409879859066113fcd57ca619b648a38d2414a712897172dc)
+            type_hints = typing.get_type_hints(_typecheckingstub__8499286546cb116610b7dc25ea25c69cb46f39cf517017ef6079029595143f7b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
     "DataDatadogHosts",
     "DataDatadogHostsConfig",
-    "DataDatadogHostsHostList",
-    "DataDatadogHostsHostListList",
     "DataDatadogHostsHostListMeta",
     "DataDatadogHostsHostListMetaOutputReference",
     "DataDatadogHostsHostListMetrics",
     "DataDatadogHostsHostListMetricsOutputReference",
-    "DataDatadogHostsHostListOutputReference",
+    "DataDatadogHostsHostListStruct",
+    "DataDatadogHostsHostListStructList",
+    "DataDatadogHostsHostListStructOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__999654e9d5e5afedbe52698c7cc27aa247a6071dd2f0197450d60280608f89b8(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
@@ -890,79 +896,79 @@
     include_muted_hosts_data: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     sort_dir: typing.Optional[builtins.str] = None,
     sort_field: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ac82a341ccc60d366c2d89d137c9de3d02c7eb70ce5d30376a4f863da7b28a00(
+def _typecheckingstub__99a3299c781760e6d3a22bbf8def9848177c04414c307853b4fef9554fa497b4(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
-    wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__106e4837c73c581cc4825e9d60420d809009548a3b0895c885c00fc9d6f218cb(
-    index: jsii.Number,
+def _typecheckingstub__e4cfb7a657623aac7b97685e6a0c1e2f0a25cd9681dbd9671bb821457f79237e(
+    value: typing.Optional[DataDatadogHostsHostListMeta],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6989f39e6826b4b2918fd6a637588d8756abadfedad67a490721a8fb83f43ed1(
-    value: builtins.str,
+def _typecheckingstub__21fdca0f3eaee89ec2f59cdd997a3f2dffa1c21e38cc2314d5b98472a94a6f78(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__9bb40108fbd0dfc3fe83d69e90dfbd86618e75a725ad62ddfb06aa26f58a0617(
-    value: _cdktf_9a9027ec.IInterpolatingParent,
+def _typecheckingstub__87e2f2bec7fc0f90e7fb49d83a77be82ebabe6d93587ac3b06d66dd57d5630e7(
+    value: typing.Optional[DataDatadogHostsHostListMetrics],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a1eeba0ecc84304df2d34cdd2d9e551f900f909b0288a4b901a2a735a64128c9(
-    value: builtins.bool,
+def _typecheckingstub__6fc9bf6ecc1fd07bae1c9eb39e5d315ae5d453b93b45208d9d13072b75a4c46c(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__99a3299c781760e6d3a22bbf8def9848177c04414c307853b4fef9554fa497b4(
-    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-    terraform_attribute: builtins.str,
+def _typecheckingstub__2d9c7f870c87e636cef1652e59df0f94afbfe6aff482f8512df5e024de8e61a9(
+    index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e4cfb7a657623aac7b97685e6a0c1e2f0a25cd9681dbd9671bb821457f79237e(
-    value: typing.Optional[DataDatadogHostsHostListMeta],
+def _typecheckingstub__bcc0e2a55bc62e2e5f105b1b45c9e7a5eed7dbee42026b28b590f479020e386b(
+    value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__21fdca0f3eaee89ec2f59cdd997a3f2dffa1c21e38cc2314d5b98472a94a6f78(
-    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-    terraform_attribute: builtins.str,
+def _typecheckingstub__a25ce29aecf25c4c686cb4ff504956663c727bcbf00e1e712e5555d9a2274dfb(
+    value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__87e2f2bec7fc0f90e7fb49d83a77be82ebabe6d93587ac3b06d66dd57d5630e7(
-    value: typing.Optional[DataDatadogHostsHostListMetrics],
+def _typecheckingstub__dc791cd85041a2a7e1aee3683b9dec8acfe38821b0ab8e574fdd1a78135a7866(
+    value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c86ebad0847f85ccaae23a8bb590a534f0164e844147c6991319797b328dc2d6(
+def _typecheckingstub__7cc5f6e256c6f31b54c277b7d6b25a4f2d09d50ba213b73aa0274fdc1da14b2a(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__18a35da22ef74d2409879859066113fcd57ca619b648a38d2414a712897172dc(
-    value: typing.Optional[DataDatadogHostsHostList],
+def _typecheckingstub__8499286546cb116610b7dc25ea25c69cb46f39cf517017ef6079029595143f7b(
+    value: typing.Optional[DataDatadogHostsHostListStruct],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_integration_aws_logs_services/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_integration_aws_logs_services/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_ip_ranges/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_ip_ranges/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_archives_order/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_archives_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes_order/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_indexes_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_logs_pipelines/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_logs_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitor/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitor_config_policies/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitor_config_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_monitors/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_monitors/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_permissions/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_role/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_roles/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_rum_application/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_rum_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_filters/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_rules/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_security_monitoring_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_group_order/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_group_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_standard_pattern/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_sensitive_data_scanner_standard_pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objective/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objectives/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_service_level_objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_global_variable/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_global_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_locations/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_locations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_test/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_synthetics_test/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/data_datadog_user/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/data_datadog_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/downtime/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/downtime/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_lambda_arn/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_lambda_arn/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_log_collection/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_log_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_aws_tag_filter/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_aws_tag_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_azure/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_cloudflare_account/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_cloudflare_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_confluent_account/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_confluent_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_confluent_resource/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_confluent_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_fastly_account/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_fastly_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_fastly_service/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_fastly_service/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_gcp/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_opsgenie_service_object/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_opsgenie_service_object/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_pagerduty/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_pagerduty/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_pagerduty_service_object/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_pagerduty_service_object/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/integration_slack_channel/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/integration_slack_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/ip_allowlist/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/ip_allowlist/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_archive/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_archive_order/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_archive_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_custom_pipeline/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_custom_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_index/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_index/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_index_order/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_index_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_integration_pipeline/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_integration_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_metric/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_metric/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/logs_pipeline_order/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/logs_pipeline_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/metric_metadata/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/metric_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/metric_tag_configuration/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/metric_tag_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor_config_policy/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor_config_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/monitor_json/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/monitor_json/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/organization_settings/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/organization_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/provider/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/role/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/rum_application/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/rum_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_default_rule/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_default_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_filter/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/security_monitoring_rule/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/security_monitoring_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group_order/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_group_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_rule/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/sensitive_data_scanner_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_account/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_definition_yaml/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_definition_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/service_level_objective/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/service_level_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/slo_correction/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/slo_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_global_variable/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_global_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_private_location/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_private_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/synthetics_test/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/synthetics_test/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         assertion: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SyntheticsTestAssertion", typing.Dict[builtins.str, typing.Any]]]]] = None,
         browser_step: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SyntheticsTestBrowserStep", typing.Dict[builtins.str, typing.Any]]]]] = None,
         browser_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SyntheticsTestBrowserVariable", typing.Dict[builtins.str, typing.Any]]]]] = None,
         config_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SyntheticsTestConfigVariable", typing.Dict[builtins.str, typing.Any]]]]] = None,
         device_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         id: typing.Optional[builtins.str] = None,
         message: typing.Optional[builtins.str] = None,
-        options_list: typing.Optional[typing.Union["SyntheticsTestOptionsList", typing.Dict[builtins.str, typing.Any]]] = None,
+        options_list: typing.Optional[typing.Union["SyntheticsTestOptionsListStruct", typing.Dict[builtins.str, typing.Any]]] = None,
         request_basicauth: typing.Optional[typing.Union["SyntheticsTestRequestBasicauth", typing.Dict[builtins.str, typing.Any]]] = None,
         request_client_certificate: typing.Optional[typing.Union["SyntheticsTestRequestClientCertificate", typing.Dict[builtins.str, typing.Any]]] = None,
         request_definition: typing.Optional[typing.Union["SyntheticsTestRequestDefinition", typing.Dict[builtins.str, typing.Any]]] = None,
         request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         request_proxy: typing.Optional[typing.Union["SyntheticsTestRequestProxy", typing.Dict[builtins.str, typing.Any]]] = None,
         request_query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         set_cookie: typing.Optional[builtins.str] = None,
@@ -245,15 +245,15 @@
         :param monitor_priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_priority SyntheticsTest#monitor_priority}.
         :param no_screenshot: Prevents saving screenshots of the steps. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#no_screenshot SyntheticsTest#no_screenshot}
         :param restricted_roles: A list of role identifiers pulled from the Roles API to restrict read and write access. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#restricted_roles SyntheticsTest#restricted_roles}
         :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#retry SyntheticsTest#retry}
         :param rum_settings: rum_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#rum_settings SyntheticsTest#rum_settings}
         :param scheduling: scheduling block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#scheduling SyntheticsTest#scheduling}
         '''
-        value = SyntheticsTestOptionsList(
+        value = SyntheticsTestOptionsListStruct(
             tick_every=tick_every,
             accept_self_signed=accept_self_signed,
             allow_insecure=allow_insecure,
             check_certificate_revocation=check_certificate_revocation,
             ci=ci,
             disable_cors=disable_cors,
             disable_csp=disable_csp,
@@ -540,16 +540,16 @@
     @builtins.property
     @jsii.member(jsii_name="monitorId")
     def monitor_id(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "monitorId"))
 
     @builtins.property
     @jsii.member(jsii_name="optionsList")
-    def options_list(self) -> "SyntheticsTestOptionsListOutputReference":
-        return typing.cast("SyntheticsTestOptionsListOutputReference", jsii.get(self, "optionsList"))
+    def options_list(self) -> "SyntheticsTestOptionsListStructOutputReference":
+        return typing.cast("SyntheticsTestOptionsListStructOutputReference", jsii.get(self, "optionsList"))
 
     @builtins.property
     @jsii.member(jsii_name="requestBasicauth")
     def request_basicauth(self) -> "SyntheticsTestRequestBasicauthOutputReference":
         return typing.cast("SyntheticsTestRequestBasicauthOutputReference", jsii.get(self, "requestBasicauth"))
 
     @builtins.property
@@ -627,16 +627,16 @@
     @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
     @jsii.member(jsii_name="optionsListInput")
-    def options_list_input(self) -> typing.Optional["SyntheticsTestOptionsList"]:
-        return typing.cast(typing.Optional["SyntheticsTestOptionsList"], jsii.get(self, "optionsListInput"))
+    def options_list_input(self) -> typing.Optional["SyntheticsTestOptionsListStruct"]:
+        return typing.cast(typing.Optional["SyntheticsTestOptionsListStruct"], jsii.get(self, "optionsListInput"))
 
     @builtins.property
     @jsii.member(jsii_name="requestBasicauthInput")
     def request_basicauth_input(
         self,
     ) -> typing.Optional["SyntheticsTestRequestBasicauth"]:
         return typing.cast(typing.Optional["SyntheticsTestRequestBasicauth"], jsii.get(self, "requestBasicauthInput"))
@@ -7926,15 +7926,15 @@
         assertion: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestAssertion, typing.Dict[builtins.str, typing.Any]]]]] = None,
         browser_step: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestBrowserStep, typing.Dict[builtins.str, typing.Any]]]]] = None,
         browser_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestBrowserVariable, typing.Dict[builtins.str, typing.Any]]]]] = None,
         config_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SyntheticsTestConfigVariable", typing.Dict[builtins.str, typing.Any]]]]] = None,
         device_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         id: typing.Optional[builtins.str] = None,
         message: typing.Optional[builtins.str] = None,
-        options_list: typing.Optional[typing.Union["SyntheticsTestOptionsList", typing.Dict[builtins.str, typing.Any]]] = None,
+        options_list: typing.Optional[typing.Union["SyntheticsTestOptionsListStruct", typing.Dict[builtins.str, typing.Any]]] = None,
         request_basicauth: typing.Optional[typing.Union["SyntheticsTestRequestBasicauth", typing.Dict[builtins.str, typing.Any]]] = None,
         request_client_certificate: typing.Optional[typing.Union["SyntheticsTestRequestClientCertificate", typing.Dict[builtins.str, typing.Any]]] = None,
         request_definition: typing.Optional[typing.Union["SyntheticsTestRequestDefinition", typing.Dict[builtins.str, typing.Any]]] = None,
         request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         request_proxy: typing.Optional[typing.Union["SyntheticsTestRequestProxy", typing.Dict[builtins.str, typing.Any]]] = None,
         request_query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         set_cookie: typing.Optional[builtins.str] = None,
@@ -7971,15 +7971,15 @@
         :param set_cookie: Cookies to be used for a browser test request, using the `Set-Cookie <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie>`_ syntax. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#set_cookie SyntheticsTest#set_cookie}
         :param subtype: The subtype of the Synthetic API test. Defaults to ``http``. Valid values are ``http``, ``ssl``, ``tcp``, ``dns``, ``multi``, ``icmp``, ``udp``, ``websocket``, ``grpc``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#subtype SyntheticsTest#subtype}
         :param tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (``[]``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#tags SyntheticsTest#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(options_list, dict):
-            options_list = SyntheticsTestOptionsList(**options_list)
+            options_list = SyntheticsTestOptionsListStruct(**options_list)
         if isinstance(request_basicauth, dict):
             request_basicauth = SyntheticsTestRequestBasicauth(**request_basicauth)
         if isinstance(request_client_certificate, dict):
             request_client_certificate = SyntheticsTestRequestClientCertificate(**request_client_certificate)
         if isinstance(request_definition, dict):
             request_definition = SyntheticsTestRequestDefinition(**request_definition)
         if isinstance(request_proxy, dict):
@@ -8262,21 +8262,21 @@
 
         Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#message SyntheticsTest#message}
         '''
         result = self._values.get("message")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def options_list(self) -> typing.Optional["SyntheticsTestOptionsList"]:
+    def options_list(self) -> typing.Optional["SyntheticsTestOptionsListStruct"]:
         '''options_list block.
 
         Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#options_list SyntheticsTest#options_list}
         '''
         result = self._values.get("options_list")
-        return typing.cast(typing.Optional["SyntheticsTestOptionsList"], result)
+        return typing.cast(typing.Optional["SyntheticsTestOptionsListStruct"], result)
 
     @builtins.property
     def request_basicauth(self) -> typing.Optional["SyntheticsTestRequestBasicauth"]:
         '''request_basicauth block.
 
         Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#request_basicauth SyntheticsTest#request_basicauth}
         '''
@@ -8760,384 +8760,14 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9b444e981176453dd5e922485f7598e82982d7d82eac74baa256f9087a7387d2)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-datadog.syntheticsTest.SyntheticsTestOptionsList",
-    jsii_struct_bases=[],
-    name_mapping={
-        "tick_every": "tickEvery",
-        "accept_self_signed": "acceptSelfSigned",
-        "allow_insecure": "allowInsecure",
-        "check_certificate_revocation": "checkCertificateRevocation",
-        "ci": "ci",
-        "disable_cors": "disableCors",
-        "disable_csp": "disableCsp",
-        "follow_redirects": "followRedirects",
-        "http_version": "httpVersion",
-        "ignore_server_certificate_error": "ignoreServerCertificateError",
-        "initial_navigation_timeout": "initialNavigationTimeout",
-        "min_failure_duration": "minFailureDuration",
-        "min_location_failed": "minLocationFailed",
-        "monitor_name": "monitorName",
-        "monitor_options": "monitorOptions",
-        "monitor_priority": "monitorPriority",
-        "no_screenshot": "noScreenshot",
-        "restricted_roles": "restrictedRoles",
-        "retry": "retry",
-        "rum_settings": "rumSettings",
-        "scheduling": "scheduling",
-    },
-)
-class SyntheticsTestOptionsList:
-    def __init__(
-        self,
-        *,
-        tick_every: jsii.Number,
-        accept_self_signed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        allow_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        check_certificate_revocation: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        ci: typing.Optional[typing.Union["SyntheticsTestOptionsListCi", typing.Dict[builtins.str, typing.Any]]] = None,
-        disable_cors: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        disable_csp: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        follow_redirects: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        http_version: typing.Optional[builtins.str] = None,
-        ignore_server_certificate_error: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        initial_navigation_timeout: typing.Optional[jsii.Number] = None,
-        min_failure_duration: typing.Optional[jsii.Number] = None,
-        min_location_failed: typing.Optional[jsii.Number] = None,
-        monitor_name: typing.Optional[builtins.str] = None,
-        monitor_options: typing.Optional[typing.Union["SyntheticsTestOptionsListMonitorOptions", typing.Dict[builtins.str, typing.Any]]] = None,
-        monitor_priority: typing.Optional[jsii.Number] = None,
-        no_screenshot: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-        restricted_roles: typing.Optional[typing.Sequence[builtins.str]] = None,
-        retry: typing.Optional[typing.Union["SyntheticsTestOptionsListRetry", typing.Dict[builtins.str, typing.Any]]] = None,
-        rum_settings: typing.Optional[typing.Union["SyntheticsTestOptionsListRumSettings", typing.Dict[builtins.str, typing.Any]]] = None,
-        scheduling: typing.Optional[typing.Union["SyntheticsTestOptionsListScheduling", typing.Dict[builtins.str, typing.Any]]] = None,
-    ) -> None:
-        '''
-        :param tick_every: How often the test should run (in seconds). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#tick_every SyntheticsTest#tick_every}
-        :param accept_self_signed: For SSL test, whether or not the test should allow self signed certificates. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#accept_self_signed SyntheticsTest#accept_self_signed}
-        :param allow_insecure: Allows loading insecure content for an HTTP test. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#allow_insecure SyntheticsTest#allow_insecure}
-        :param check_certificate_revocation: For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#check_certificate_revocation SyntheticsTest#check_certificate_revocation}
-        :param ci: ci block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ci SyntheticsTest#ci}
-        :param disable_cors: Disable Cross-Origin Resource Sharing for browser tests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_cors SyntheticsTest#disable_cors}
-        :param disable_csp: Disable Content Security Policy for browser tests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_csp SyntheticsTest#disable_csp}
-        :param follow_redirects: Determines whether or not the API HTTP test should follow redirects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#follow_redirects SyntheticsTest#follow_redirects}
-        :param http_version: HTTP version to use for a Synthetics API test. Valid values are ``http1``, ``http2``, ``any``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#http_version SyntheticsTest#http_version}
-        :param ignore_server_certificate_error: Ignore server certificate error. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ignore_server_certificate_error SyntheticsTest#ignore_server_certificate_error}
-        :param initial_navigation_timeout: Timeout before declaring the initial step as failed (in seconds) for browser tests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#initial_navigation_timeout SyntheticsTest#initial_navigation_timeout}
-        :param min_failure_duration: Minimum amount of time in failure required to trigger an alert (in seconds). Default is ``0``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_failure_duration SyntheticsTest#min_failure_duration}
-        :param min_location_failed: Minimum number of locations in failure required to trigger an alert. Default is ``1``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_location_failed SyntheticsTest#min_location_failed}
-        :param monitor_name: The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_name SyntheticsTest#monitor_name}
-        :param monitor_options: monitor_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_options SyntheticsTest#monitor_options}
-        :param monitor_priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_priority SyntheticsTest#monitor_priority}.
-        :param no_screenshot: Prevents saving screenshots of the steps. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#no_screenshot SyntheticsTest#no_screenshot}
-        :param restricted_roles: A list of role identifiers pulled from the Roles API to restrict read and write access. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#restricted_roles SyntheticsTest#restricted_roles}
-        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#retry SyntheticsTest#retry}
-        :param rum_settings: rum_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#rum_settings SyntheticsTest#rum_settings}
-        :param scheduling: scheduling block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#scheduling SyntheticsTest#scheduling}
-        '''
-        if isinstance(ci, dict):
-            ci = SyntheticsTestOptionsListCi(**ci)
-        if isinstance(monitor_options, dict):
-            monitor_options = SyntheticsTestOptionsListMonitorOptions(**monitor_options)
-        if isinstance(retry, dict):
-            retry = SyntheticsTestOptionsListRetry(**retry)
-        if isinstance(rum_settings, dict):
-            rum_settings = SyntheticsTestOptionsListRumSettings(**rum_settings)
-        if isinstance(scheduling, dict):
-            scheduling = SyntheticsTestOptionsListScheduling(**scheduling)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__669a64b0c857b3913f6e1304a3b7506ac7351d32b12a1e69230b0fd453c12cb3)
-            check_type(argname="argument tick_every", value=tick_every, expected_type=type_hints["tick_every"])
-            check_type(argname="argument accept_self_signed", value=accept_self_signed, expected_type=type_hints["accept_self_signed"])
-            check_type(argname="argument allow_insecure", value=allow_insecure, expected_type=type_hints["allow_insecure"])
-            check_type(argname="argument check_certificate_revocation", value=check_certificate_revocation, expected_type=type_hints["check_certificate_revocation"])
-            check_type(argname="argument ci", value=ci, expected_type=type_hints["ci"])
-            check_type(argname="argument disable_cors", value=disable_cors, expected_type=type_hints["disable_cors"])
-            check_type(argname="argument disable_csp", value=disable_csp, expected_type=type_hints["disable_csp"])
-            check_type(argname="argument follow_redirects", value=follow_redirects, expected_type=type_hints["follow_redirects"])
-            check_type(argname="argument http_version", value=http_version, expected_type=type_hints["http_version"])
-            check_type(argname="argument ignore_server_certificate_error", value=ignore_server_certificate_error, expected_type=type_hints["ignore_server_certificate_error"])
-            check_type(argname="argument initial_navigation_timeout", value=initial_navigation_timeout, expected_type=type_hints["initial_navigation_timeout"])
-            check_type(argname="argument min_failure_duration", value=min_failure_duration, expected_type=type_hints["min_failure_duration"])
-            check_type(argname="argument min_location_failed", value=min_location_failed, expected_type=type_hints["min_location_failed"])
-            check_type(argname="argument monitor_name", value=monitor_name, expected_type=type_hints["monitor_name"])
-            check_type(argname="argument monitor_options", value=monitor_options, expected_type=type_hints["monitor_options"])
-            check_type(argname="argument monitor_priority", value=monitor_priority, expected_type=type_hints["monitor_priority"])
-            check_type(argname="argument no_screenshot", value=no_screenshot, expected_type=type_hints["no_screenshot"])
-            check_type(argname="argument restricted_roles", value=restricted_roles, expected_type=type_hints["restricted_roles"])
-            check_type(argname="argument retry", value=retry, expected_type=type_hints["retry"])
-            check_type(argname="argument rum_settings", value=rum_settings, expected_type=type_hints["rum_settings"])
-            check_type(argname="argument scheduling", value=scheduling, expected_type=type_hints["scheduling"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "tick_every": tick_every,
-        }
-        if accept_self_signed is not None:
-            self._values["accept_self_signed"] = accept_self_signed
-        if allow_insecure is not None:
-            self._values["allow_insecure"] = allow_insecure
-        if check_certificate_revocation is not None:
-            self._values["check_certificate_revocation"] = check_certificate_revocation
-        if ci is not None:
-            self._values["ci"] = ci
-        if disable_cors is not None:
-            self._values["disable_cors"] = disable_cors
-        if disable_csp is not None:
-            self._values["disable_csp"] = disable_csp
-        if follow_redirects is not None:
-            self._values["follow_redirects"] = follow_redirects
-        if http_version is not None:
-            self._values["http_version"] = http_version
-        if ignore_server_certificate_error is not None:
-            self._values["ignore_server_certificate_error"] = ignore_server_certificate_error
-        if initial_navigation_timeout is not None:
-            self._values["initial_navigation_timeout"] = initial_navigation_timeout
-        if min_failure_duration is not None:
-            self._values["min_failure_duration"] = min_failure_duration
-        if min_location_failed is not None:
-            self._values["min_location_failed"] = min_location_failed
-        if monitor_name is not None:
-            self._values["monitor_name"] = monitor_name
-        if monitor_options is not None:
-            self._values["monitor_options"] = monitor_options
-        if monitor_priority is not None:
-            self._values["monitor_priority"] = monitor_priority
-        if no_screenshot is not None:
-            self._values["no_screenshot"] = no_screenshot
-        if restricted_roles is not None:
-            self._values["restricted_roles"] = restricted_roles
-        if retry is not None:
-            self._values["retry"] = retry
-        if rum_settings is not None:
-            self._values["rum_settings"] = rum_settings
-        if scheduling is not None:
-            self._values["scheduling"] = scheduling
-
-    @builtins.property
-    def tick_every(self) -> jsii.Number:
-        '''How often the test should run (in seconds).
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#tick_every SyntheticsTest#tick_every}
-        '''
-        result = self._values.get("tick_every")
-        assert result is not None, "Required property 'tick_every' is missing"
-        return typing.cast(jsii.Number, result)
-
-    @builtins.property
-    def accept_self_signed(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''For SSL test, whether or not the test should allow self signed certificates.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#accept_self_signed SyntheticsTest#accept_self_signed}
-        '''
-        result = self._values.get("accept_self_signed")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def allow_insecure(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Allows loading insecure content for an HTTP test.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#allow_insecure SyntheticsTest#allow_insecure}
-        '''
-        result = self._values.get("allow_insecure")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def check_certificate_revocation(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#check_certificate_revocation SyntheticsTest#check_certificate_revocation}
-        '''
-        result = self._values.get("check_certificate_revocation")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def ci(self) -> typing.Optional["SyntheticsTestOptionsListCi"]:
-        '''ci block.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ci SyntheticsTest#ci}
-        '''
-        result = self._values.get("ci")
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListCi"], result)
-
-    @builtins.property
-    def disable_cors(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Disable Cross-Origin Resource Sharing for browser tests.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_cors SyntheticsTest#disable_cors}
-        '''
-        result = self._values.get("disable_cors")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def disable_csp(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Disable Content Security Policy for browser tests.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_csp SyntheticsTest#disable_csp}
-        '''
-        result = self._values.get("disable_csp")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def follow_redirects(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Determines whether or not the API HTTP test should follow redirects.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#follow_redirects SyntheticsTest#follow_redirects}
-        '''
-        result = self._values.get("follow_redirects")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def http_version(self) -> typing.Optional[builtins.str]:
-        '''HTTP version to use for a Synthetics API test. Valid values are ``http1``, ``http2``, ``any``.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#http_version SyntheticsTest#http_version}
-        '''
-        result = self._values.get("http_version")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def ignore_server_certificate_error(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Ignore server certificate error.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ignore_server_certificate_error SyntheticsTest#ignore_server_certificate_error}
-        '''
-        result = self._values.get("ignore_server_certificate_error")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def initial_navigation_timeout(self) -> typing.Optional[jsii.Number]:
-        '''Timeout before declaring the initial step as failed (in seconds) for browser tests.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#initial_navigation_timeout SyntheticsTest#initial_navigation_timeout}
-        '''
-        result = self._values.get("initial_navigation_timeout")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def min_failure_duration(self) -> typing.Optional[jsii.Number]:
-        '''Minimum amount of time in failure required to trigger an alert (in seconds). Default is ``0``.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_failure_duration SyntheticsTest#min_failure_duration}
-        '''
-        result = self._values.get("min_failure_duration")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def min_location_failed(self) -> typing.Optional[jsii.Number]:
-        '''Minimum number of locations in failure required to trigger an alert. Default is ``1``.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_location_failed SyntheticsTest#min_location_failed}
-        '''
-        result = self._values.get("min_location_failed")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def monitor_name(self) -> typing.Optional[builtins.str]:
-        '''The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_name SyntheticsTest#monitor_name}
-        '''
-        result = self._values.get("monitor_name")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def monitor_options(
-        self,
-    ) -> typing.Optional["SyntheticsTestOptionsListMonitorOptions"]:
-        '''monitor_options block.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_options SyntheticsTest#monitor_options}
-        '''
-        result = self._values.get("monitor_options")
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListMonitorOptions"], result)
-
-    @builtins.property
-    def monitor_priority(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_priority SyntheticsTest#monitor_priority}.'''
-        result = self._values.get("monitor_priority")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def no_screenshot(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Prevents saving screenshots of the steps.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#no_screenshot SyntheticsTest#no_screenshot}
-        '''
-        result = self._values.get("no_screenshot")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
-
-    @builtins.property
-    def restricted_roles(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''A list of role identifiers pulled from the Roles API to restrict read and write access.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#restricted_roles SyntheticsTest#restricted_roles}
-        '''
-        result = self._values.get("restricted_roles")
-        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
-
-    @builtins.property
-    def retry(self) -> typing.Optional["SyntheticsTestOptionsListRetry"]:
-        '''retry block.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#retry SyntheticsTest#retry}
-        '''
-        result = self._values.get("retry")
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListRetry"], result)
-
-    @builtins.property
-    def rum_settings(self) -> typing.Optional["SyntheticsTestOptionsListRumSettings"]:
-        '''rum_settings block.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#rum_settings SyntheticsTest#rum_settings}
-        '''
-        result = self._values.get("rum_settings")
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListRumSettings"], result)
-
-    @builtins.property
-    def scheduling(self) -> typing.Optional["SyntheticsTestOptionsListScheduling"]:
-        '''scheduling block.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#scheduling SyntheticsTest#scheduling}
-        '''
-        result = self._values.get("scheduling")
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListScheduling"], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "SyntheticsTestOptionsList(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.data_type(
     jsii_type="@cdktf/provider-datadog.syntheticsTest.SyntheticsTestOptionsListCi",
     jsii_struct_bases=[],
     name_mapping={"execution_rule": "executionRule"},
 )
 class SyntheticsTestOptionsListCi:
     def __init__(self, *, execution_rule: typing.Optional[builtins.str] = None) -> None:
         '''
@@ -9327,582 +8957,14 @@
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5d8efaa9b18bd9c319279983db5109ac1996e2195bb489b733584961c476cda0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
-class SyntheticsTestOptionsListOutputReference(
-    _cdktf_9a9027ec.ComplexObject,
-    metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-datadog.syntheticsTest.SyntheticsTestOptionsListOutputReference",
-):
-    def __init__(
-        self,
-        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-        terraform_attribute: builtins.str,
-    ) -> None:
-        '''
-        :param terraform_resource: The parent resource.
-        :param terraform_attribute: The attribute on the parent resource this class is referencing.
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__78a25caa898b8d54783108c1e76beb3e94a916048730439ebeaa41e3f9b5f518)
-            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
-            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
-        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
-
-    @jsii.member(jsii_name="putCi")
-    def put_ci(self, *, execution_rule: typing.Optional[builtins.str] = None) -> None:
-        '''
-        :param execution_rule: Execution rule for a Synthetics test. Valid values are ``blocking``, ``non_blocking``, ``skipped``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#execution_rule SyntheticsTest#execution_rule}
-        '''
-        value = SyntheticsTestOptionsListCi(execution_rule=execution_rule)
-
-        return typing.cast(None, jsii.invoke(self, "putCi", [value]))
-
-    @jsii.member(jsii_name="putMonitorOptions")
-    def put_monitor_options(
-        self,
-        *,
-        renotify_interval: typing.Optional[jsii.Number] = None,
-    ) -> None:
-        '''
-        :param renotify_interval: Specify a renotification frequency in minutes. Values available by default are ``0``, ``10``, ``20``, ``30``, ``40``, ``50``, ``60``, ``90``, ``120``, ``180``, ``240``, ``300``, ``360``, ``720``, ``1440``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#renotify_interval SyntheticsTest#renotify_interval}
-        '''
-        value = SyntheticsTestOptionsListMonitorOptions(
-            renotify_interval=renotify_interval
-        )
-
-        return typing.cast(None, jsii.invoke(self, "putMonitorOptions", [value]))
-
-    @jsii.member(jsii_name="putRetry")
-    def put_retry(
-        self,
-        *,
-        count: typing.Optional[jsii.Number] = None,
-        interval: typing.Optional[jsii.Number] = None,
-    ) -> None:
-        '''
-        :param count: Number of retries needed to consider a location as failed before sending a notification alert. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#count SyntheticsTest#count}
-        :param interval: Interval between a failed test and the next retry in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#interval SyntheticsTest#interval}
-        '''
-        value = SyntheticsTestOptionsListRetry(count=count, interval=interval)
-
-        return typing.cast(None, jsii.invoke(self, "putRetry", [value]))
-
-    @jsii.member(jsii_name="putRumSettings")
-    def put_rum_settings(
-        self,
-        *,
-        is_enabled: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-        application_id: typing.Optional[builtins.str] = None,
-        client_token_id: typing.Optional[jsii.Number] = None,
-    ) -> None:
-        '''
-        :param is_enabled: Determines whether RUM data is collected during test runs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#is_enabled SyntheticsTest#is_enabled}
-        :param application_id: RUM application ID used to collect RUM data for the browser test. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#application_id SyntheticsTest#application_id}
-        :param client_token_id: RUM application API key ID used to collect RUM data for the browser test. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#client_token_id SyntheticsTest#client_token_id}
-        '''
-        value = SyntheticsTestOptionsListRumSettings(
-            is_enabled=is_enabled,
-            application_id=application_id,
-            client_token_id=client_token_id,
-        )
-
-        return typing.cast(None, jsii.invoke(self, "putRumSettings", [value]))
-
-    @jsii.member(jsii_name="putScheduling")
-    def put_scheduling(
-        self,
-        *,
-        timeframes: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SyntheticsTestOptionsListSchedulingTimeframes", typing.Dict[builtins.str, typing.Any]]]],
-        timezone: builtins.str,
-    ) -> None:
-        '''
-        :param timeframes: timeframes block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#timeframes SyntheticsTest#timeframes}
-        :param timezone: Timezone in which the timeframe is based. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#timezone SyntheticsTest#timezone}
-        '''
-        value = SyntheticsTestOptionsListScheduling(
-            timeframes=timeframes, timezone=timezone
-        )
-
-        return typing.cast(None, jsii.invoke(self, "putScheduling", [value]))
-
-    @jsii.member(jsii_name="resetAcceptSelfSigned")
-    def reset_accept_self_signed(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetAcceptSelfSigned", []))
-
-    @jsii.member(jsii_name="resetAllowInsecure")
-    def reset_allow_insecure(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetAllowInsecure", []))
-
-    @jsii.member(jsii_name="resetCheckCertificateRevocation")
-    def reset_check_certificate_revocation(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetCheckCertificateRevocation", []))
-
-    @jsii.member(jsii_name="resetCi")
-    def reset_ci(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetCi", []))
-
-    @jsii.member(jsii_name="resetDisableCors")
-    def reset_disable_cors(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetDisableCors", []))
-
-    @jsii.member(jsii_name="resetDisableCsp")
-    def reset_disable_csp(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetDisableCsp", []))
-
-    @jsii.member(jsii_name="resetFollowRedirects")
-    def reset_follow_redirects(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetFollowRedirects", []))
-
-    @jsii.member(jsii_name="resetHttpVersion")
-    def reset_http_version(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetHttpVersion", []))
-
-    @jsii.member(jsii_name="resetIgnoreServerCertificateError")
-    def reset_ignore_server_certificate_error(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetIgnoreServerCertificateError", []))
-
-    @jsii.member(jsii_name="resetInitialNavigationTimeout")
-    def reset_initial_navigation_timeout(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetInitialNavigationTimeout", []))
-
-    @jsii.member(jsii_name="resetMinFailureDuration")
-    def reset_min_failure_duration(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetMinFailureDuration", []))
-
-    @jsii.member(jsii_name="resetMinLocationFailed")
-    def reset_min_location_failed(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetMinLocationFailed", []))
-
-    @jsii.member(jsii_name="resetMonitorName")
-    def reset_monitor_name(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetMonitorName", []))
-
-    @jsii.member(jsii_name="resetMonitorOptions")
-    def reset_monitor_options(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetMonitorOptions", []))
-
-    @jsii.member(jsii_name="resetMonitorPriority")
-    def reset_monitor_priority(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetMonitorPriority", []))
-
-    @jsii.member(jsii_name="resetNoScreenshot")
-    def reset_no_screenshot(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetNoScreenshot", []))
-
-    @jsii.member(jsii_name="resetRestrictedRoles")
-    def reset_restricted_roles(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetRestrictedRoles", []))
-
-    @jsii.member(jsii_name="resetRetry")
-    def reset_retry(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetRetry", []))
-
-    @jsii.member(jsii_name="resetRumSettings")
-    def reset_rum_settings(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetRumSettings", []))
-
-    @jsii.member(jsii_name="resetScheduling")
-    def reset_scheduling(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetScheduling", []))
-
-    @builtins.property
-    @jsii.member(jsii_name="ci")
-    def ci(self) -> SyntheticsTestOptionsListCiOutputReference:
-        return typing.cast(SyntheticsTestOptionsListCiOutputReference, jsii.get(self, "ci"))
-
-    @builtins.property
-    @jsii.member(jsii_name="monitorOptions")
-    def monitor_options(self) -> SyntheticsTestOptionsListMonitorOptionsOutputReference:
-        return typing.cast(SyntheticsTestOptionsListMonitorOptionsOutputReference, jsii.get(self, "monitorOptions"))
-
-    @builtins.property
-    @jsii.member(jsii_name="retry")
-    def retry(self) -> "SyntheticsTestOptionsListRetryOutputReference":
-        return typing.cast("SyntheticsTestOptionsListRetryOutputReference", jsii.get(self, "retry"))
-
-    @builtins.property
-    @jsii.member(jsii_name="rumSettings")
-    def rum_settings(self) -> "SyntheticsTestOptionsListRumSettingsOutputReference":
-        return typing.cast("SyntheticsTestOptionsListRumSettingsOutputReference", jsii.get(self, "rumSettings"))
-
-    @builtins.property
-    @jsii.member(jsii_name="scheduling")
-    def scheduling(self) -> "SyntheticsTestOptionsListSchedulingOutputReference":
-        return typing.cast("SyntheticsTestOptionsListSchedulingOutputReference", jsii.get(self, "scheduling"))
-
-    @builtins.property
-    @jsii.member(jsii_name="acceptSelfSignedInput")
-    def accept_self_signed_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "acceptSelfSignedInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="allowInsecureInput")
-    def allow_insecure_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "allowInsecureInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="checkCertificateRevocationInput")
-    def check_certificate_revocation_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "checkCertificateRevocationInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="ciInput")
-    def ci_input(self) -> typing.Optional[SyntheticsTestOptionsListCi]:
-        return typing.cast(typing.Optional[SyntheticsTestOptionsListCi], jsii.get(self, "ciInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="disableCorsInput")
-    def disable_cors_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "disableCorsInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="disableCspInput")
-    def disable_csp_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "disableCspInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="followRedirectsInput")
-    def follow_redirects_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "followRedirectsInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="httpVersionInput")
-    def http_version_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "httpVersionInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="ignoreServerCertificateErrorInput")
-    def ignore_server_certificate_error_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "ignoreServerCertificateErrorInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="initialNavigationTimeoutInput")
-    def initial_navigation_timeout_input(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "initialNavigationTimeoutInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="minFailureDurationInput")
-    def min_failure_duration_input(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "minFailureDurationInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="minLocationFailedInput")
-    def min_location_failed_input(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "minLocationFailedInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="monitorNameInput")
-    def monitor_name_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "monitorNameInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="monitorOptionsInput")
-    def monitor_options_input(
-        self,
-    ) -> typing.Optional[SyntheticsTestOptionsListMonitorOptions]:
-        return typing.cast(typing.Optional[SyntheticsTestOptionsListMonitorOptions], jsii.get(self, "monitorOptionsInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="monitorPriorityInput")
-    def monitor_priority_input(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "monitorPriorityInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="noScreenshotInput")
-    def no_screenshot_input(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "noScreenshotInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="restrictedRolesInput")
-    def restricted_roles_input(self) -> typing.Optional[typing.List[builtins.str]]:
-        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "restrictedRolesInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="retryInput")
-    def retry_input(self) -> typing.Optional["SyntheticsTestOptionsListRetry"]:
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListRetry"], jsii.get(self, "retryInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="rumSettingsInput")
-    def rum_settings_input(
-        self,
-    ) -> typing.Optional["SyntheticsTestOptionsListRumSettings"]:
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListRumSettings"], jsii.get(self, "rumSettingsInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="schedulingInput")
-    def scheduling_input(
-        self,
-    ) -> typing.Optional["SyntheticsTestOptionsListScheduling"]:
-        return typing.cast(typing.Optional["SyntheticsTestOptionsListScheduling"], jsii.get(self, "schedulingInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="tickEveryInput")
-    def tick_every_input(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "tickEveryInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="acceptSelfSigned")
-    def accept_self_signed(
-        self,
-    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "acceptSelfSigned"))
-
-    @accept_self_signed.setter
-    def accept_self_signed(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__53d8cc461b8a175588b2371ab85da744cfbc1d28ee657a764ce99696f6fe5abf)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "acceptSelfSigned", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="allowInsecure")
-    def allow_insecure(
-        self,
-    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "allowInsecure"))
-
-    @allow_insecure.setter
-    def allow_insecure(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__906fce1953d4c28ba2f11353abb9b392caddd0f4f980b25309db51dd0c9a9c61)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "allowInsecure", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="checkCertificateRevocation")
-    def check_certificate_revocation(
-        self,
-    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "checkCertificateRevocation"))
-
-    @check_certificate_revocation.setter
-    def check_certificate_revocation(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a32c3a7384117855a7c629b949b1de291a32e238f72ddd1c7a4c2a1e5ad2767b)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "checkCertificateRevocation", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="disableCors")
-    def disable_cors(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "disableCors"))
-
-    @disable_cors.setter
-    def disable_cors(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0b9a91a7f15f54a36f8146eca988c4c423d2799b508f48b6ff93b1e74c6d04d6)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "disableCors", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="disableCsp")
-    def disable_csp(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "disableCsp"))
-
-    @disable_csp.setter
-    def disable_csp(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__53a828f2f2bef55b4cd3c79f4d8b6c47f3bafb288b6938e80503c908fc12c870)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "disableCsp", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="followRedirects")
-    def follow_redirects(
-        self,
-    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "followRedirects"))
-
-    @follow_redirects.setter
-    def follow_redirects(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d00b97833d2dbef78a26064a602de75790e95112e4b030781b0f2cea9fff5bfa)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "followRedirects", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="httpVersion")
-    def http_version(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "httpVersion"))
-
-    @http_version.setter
-    def http_version(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f8e5e784ef27d1e683d19436794c752fbf03778c759a219121893f693c3d1f02)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "httpVersion", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="ignoreServerCertificateError")
-    def ignore_server_certificate_error(
-        self,
-    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "ignoreServerCertificateError"))
-
-    @ignore_server_certificate_error.setter
-    def ignore_server_certificate_error(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__11b2b2eae7abfbcdbdd9ded17ab8fb42540bf2a3224afc34a660b3b94d2298f7)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "ignoreServerCertificateError", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="initialNavigationTimeout")
-    def initial_navigation_timeout(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "initialNavigationTimeout"))
-
-    @initial_navigation_timeout.setter
-    def initial_navigation_timeout(self, value: jsii.Number) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__085bad40cf3518fd9cdc565cec5e66f2fee9b8e86b76d6fcd7b0b53079c40420)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "initialNavigationTimeout", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="minFailureDuration")
-    def min_failure_duration(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "minFailureDuration"))
-
-    @min_failure_duration.setter
-    def min_failure_duration(self, value: jsii.Number) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f81380c6e2b43101946551969262f72f5bfbedbf1c9264024d140575cdb54869)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "minFailureDuration", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="minLocationFailed")
-    def min_location_failed(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "minLocationFailed"))
-
-    @min_location_failed.setter
-    def min_location_failed(self, value: jsii.Number) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6d814b7fd09e8de93d2029a5aa5775ab294dad5122009f972d6f33cf8a3f27aa)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "minLocationFailed", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="monitorName")
-    def monitor_name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "monitorName"))
-
-    @monitor_name.setter
-    def monitor_name(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__604143bda0c23e6b2265036f1a03f897d17524780be0282b7a53c5bfa9b01eb8)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "monitorName", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="monitorPriority")
-    def monitor_priority(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "monitorPriority"))
-
-    @monitor_priority.setter
-    def monitor_priority(self, value: jsii.Number) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__540f0fa4d54daea7a660a4e69ca7bc1626abdf616ea9ef3fc8daaae0dba94932)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "monitorPriority", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="noScreenshot")
-    def no_screenshot(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "noScreenshot"))
-
-    @no_screenshot.setter
-    def no_screenshot(
-        self,
-        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__068da975e3df412bc6fb59c03e825c41a7d5af36551c532ce316775c83fb2bf5)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "noScreenshot", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="restrictedRoles")
-    def restricted_roles(self) -> typing.List[builtins.str]:
-        return typing.cast(typing.List[builtins.str], jsii.get(self, "restrictedRoles"))
-
-    @restricted_roles.setter
-    def restricted_roles(self, value: typing.List[builtins.str]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ef9908b06b86576577772fe00d5df0be963b39c1142a17f9e6aeb9f196f1bd86)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "restrictedRoles", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="tickEvery")
-    def tick_every(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "tickEvery"))
-
-    @tick_every.setter
-    def tick_every(self, value: jsii.Number) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__82e67e70c1e41308d26d3e1f4fd1c484ab3ab7b8ec6a7bd1a73ee6bce9579811)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "tickEvery", value)
-
-    @builtins.property
-    @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[SyntheticsTestOptionsList]:
-        return typing.cast(typing.Optional[SyntheticsTestOptionsList], jsii.get(self, "internalValue"))
-
-    @internal_value.setter
-    def internal_value(self, value: typing.Optional[SyntheticsTestOptionsList]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f92ac44590f538d77cdce4d44de1454c856fc44753f6ddfa1fc43ab723ed6343)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "internalValue", value)
-
-
 @jsii.data_type(
     jsii_type="@cdktf/provider-datadog.syntheticsTest.SyntheticsTestOptionsListRetry",
     jsii_struct_bases=[],
     name_mapping={"count": "count", "interval": "interval"},
 )
 class SyntheticsTestOptionsListRetry:
     def __init__(
@@ -10601,14 +9663,953 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__669853ac122cd3d3ae92702f8c2c07dba4d00caa40cc211569e7857ca6d48ebd)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
+    jsii_type="@cdktf/provider-datadog.syntheticsTest.SyntheticsTestOptionsListStruct",
+    jsii_struct_bases=[],
+    name_mapping={
+        "tick_every": "tickEvery",
+        "accept_self_signed": "acceptSelfSigned",
+        "allow_insecure": "allowInsecure",
+        "check_certificate_revocation": "checkCertificateRevocation",
+        "ci": "ci",
+        "disable_cors": "disableCors",
+        "disable_csp": "disableCsp",
+        "follow_redirects": "followRedirects",
+        "http_version": "httpVersion",
+        "ignore_server_certificate_error": "ignoreServerCertificateError",
+        "initial_navigation_timeout": "initialNavigationTimeout",
+        "min_failure_duration": "minFailureDuration",
+        "min_location_failed": "minLocationFailed",
+        "monitor_name": "monitorName",
+        "monitor_options": "monitorOptions",
+        "monitor_priority": "monitorPriority",
+        "no_screenshot": "noScreenshot",
+        "restricted_roles": "restrictedRoles",
+        "retry": "retry",
+        "rum_settings": "rumSettings",
+        "scheduling": "scheduling",
+    },
+)
+class SyntheticsTestOptionsListStruct:
+    def __init__(
+        self,
+        *,
+        tick_every: jsii.Number,
+        accept_self_signed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        allow_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        check_certificate_revocation: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        ci: typing.Optional[typing.Union[SyntheticsTestOptionsListCi, typing.Dict[builtins.str, typing.Any]]] = None,
+        disable_cors: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        disable_csp: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        follow_redirects: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        http_version: typing.Optional[builtins.str] = None,
+        ignore_server_certificate_error: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        initial_navigation_timeout: typing.Optional[jsii.Number] = None,
+        min_failure_duration: typing.Optional[jsii.Number] = None,
+        min_location_failed: typing.Optional[jsii.Number] = None,
+        monitor_name: typing.Optional[builtins.str] = None,
+        monitor_options: typing.Optional[typing.Union[SyntheticsTestOptionsListMonitorOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        monitor_priority: typing.Optional[jsii.Number] = None,
+        no_screenshot: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        restricted_roles: typing.Optional[typing.Sequence[builtins.str]] = None,
+        retry: typing.Optional[typing.Union[SyntheticsTestOptionsListRetry, typing.Dict[builtins.str, typing.Any]]] = None,
+        rum_settings: typing.Optional[typing.Union[SyntheticsTestOptionsListRumSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        scheduling: typing.Optional[typing.Union[SyntheticsTestOptionsListScheduling, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param tick_every: How often the test should run (in seconds). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#tick_every SyntheticsTest#tick_every}
+        :param accept_self_signed: For SSL test, whether or not the test should allow self signed certificates. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#accept_self_signed SyntheticsTest#accept_self_signed}
+        :param allow_insecure: Allows loading insecure content for an HTTP test. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#allow_insecure SyntheticsTest#allow_insecure}
+        :param check_certificate_revocation: For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#check_certificate_revocation SyntheticsTest#check_certificate_revocation}
+        :param ci: ci block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ci SyntheticsTest#ci}
+        :param disable_cors: Disable Cross-Origin Resource Sharing for browser tests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_cors SyntheticsTest#disable_cors}
+        :param disable_csp: Disable Content Security Policy for browser tests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_csp SyntheticsTest#disable_csp}
+        :param follow_redirects: Determines whether or not the API HTTP test should follow redirects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#follow_redirects SyntheticsTest#follow_redirects}
+        :param http_version: HTTP version to use for a Synthetics API test. Valid values are ``http1``, ``http2``, ``any``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#http_version SyntheticsTest#http_version}
+        :param ignore_server_certificate_error: Ignore server certificate error. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ignore_server_certificate_error SyntheticsTest#ignore_server_certificate_error}
+        :param initial_navigation_timeout: Timeout before declaring the initial step as failed (in seconds) for browser tests. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#initial_navigation_timeout SyntheticsTest#initial_navigation_timeout}
+        :param min_failure_duration: Minimum amount of time in failure required to trigger an alert (in seconds). Default is ``0``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_failure_duration SyntheticsTest#min_failure_duration}
+        :param min_location_failed: Minimum number of locations in failure required to trigger an alert. Default is ``1``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_location_failed SyntheticsTest#min_location_failed}
+        :param monitor_name: The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_name SyntheticsTest#monitor_name}
+        :param monitor_options: monitor_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_options SyntheticsTest#monitor_options}
+        :param monitor_priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_priority SyntheticsTest#monitor_priority}.
+        :param no_screenshot: Prevents saving screenshots of the steps. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#no_screenshot SyntheticsTest#no_screenshot}
+        :param restricted_roles: A list of role identifiers pulled from the Roles API to restrict read and write access. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#restricted_roles SyntheticsTest#restricted_roles}
+        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#retry SyntheticsTest#retry}
+        :param rum_settings: rum_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#rum_settings SyntheticsTest#rum_settings}
+        :param scheduling: scheduling block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#scheduling SyntheticsTest#scheduling}
+        '''
+        if isinstance(ci, dict):
+            ci = SyntheticsTestOptionsListCi(**ci)
+        if isinstance(monitor_options, dict):
+            monitor_options = SyntheticsTestOptionsListMonitorOptions(**monitor_options)
+        if isinstance(retry, dict):
+            retry = SyntheticsTestOptionsListRetry(**retry)
+        if isinstance(rum_settings, dict):
+            rum_settings = SyntheticsTestOptionsListRumSettings(**rum_settings)
+        if isinstance(scheduling, dict):
+            scheduling = SyntheticsTestOptionsListScheduling(**scheduling)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e136bc90e4e687f03e8828ece8dd8370e3f9171ef719b48228a02707d84ae0dc)
+            check_type(argname="argument tick_every", value=tick_every, expected_type=type_hints["tick_every"])
+            check_type(argname="argument accept_self_signed", value=accept_self_signed, expected_type=type_hints["accept_self_signed"])
+            check_type(argname="argument allow_insecure", value=allow_insecure, expected_type=type_hints["allow_insecure"])
+            check_type(argname="argument check_certificate_revocation", value=check_certificate_revocation, expected_type=type_hints["check_certificate_revocation"])
+            check_type(argname="argument ci", value=ci, expected_type=type_hints["ci"])
+            check_type(argname="argument disable_cors", value=disable_cors, expected_type=type_hints["disable_cors"])
+            check_type(argname="argument disable_csp", value=disable_csp, expected_type=type_hints["disable_csp"])
+            check_type(argname="argument follow_redirects", value=follow_redirects, expected_type=type_hints["follow_redirects"])
+            check_type(argname="argument http_version", value=http_version, expected_type=type_hints["http_version"])
+            check_type(argname="argument ignore_server_certificate_error", value=ignore_server_certificate_error, expected_type=type_hints["ignore_server_certificate_error"])
+            check_type(argname="argument initial_navigation_timeout", value=initial_navigation_timeout, expected_type=type_hints["initial_navigation_timeout"])
+            check_type(argname="argument min_failure_duration", value=min_failure_duration, expected_type=type_hints["min_failure_duration"])
+            check_type(argname="argument min_location_failed", value=min_location_failed, expected_type=type_hints["min_location_failed"])
+            check_type(argname="argument monitor_name", value=monitor_name, expected_type=type_hints["monitor_name"])
+            check_type(argname="argument monitor_options", value=monitor_options, expected_type=type_hints["monitor_options"])
+            check_type(argname="argument monitor_priority", value=monitor_priority, expected_type=type_hints["monitor_priority"])
+            check_type(argname="argument no_screenshot", value=no_screenshot, expected_type=type_hints["no_screenshot"])
+            check_type(argname="argument restricted_roles", value=restricted_roles, expected_type=type_hints["restricted_roles"])
+            check_type(argname="argument retry", value=retry, expected_type=type_hints["retry"])
+            check_type(argname="argument rum_settings", value=rum_settings, expected_type=type_hints["rum_settings"])
+            check_type(argname="argument scheduling", value=scheduling, expected_type=type_hints["scheduling"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "tick_every": tick_every,
+        }
+        if accept_self_signed is not None:
+            self._values["accept_self_signed"] = accept_self_signed
+        if allow_insecure is not None:
+            self._values["allow_insecure"] = allow_insecure
+        if check_certificate_revocation is not None:
+            self._values["check_certificate_revocation"] = check_certificate_revocation
+        if ci is not None:
+            self._values["ci"] = ci
+        if disable_cors is not None:
+            self._values["disable_cors"] = disable_cors
+        if disable_csp is not None:
+            self._values["disable_csp"] = disable_csp
+        if follow_redirects is not None:
+            self._values["follow_redirects"] = follow_redirects
+        if http_version is not None:
+            self._values["http_version"] = http_version
+        if ignore_server_certificate_error is not None:
+            self._values["ignore_server_certificate_error"] = ignore_server_certificate_error
+        if initial_navigation_timeout is not None:
+            self._values["initial_navigation_timeout"] = initial_navigation_timeout
+        if min_failure_duration is not None:
+            self._values["min_failure_duration"] = min_failure_duration
+        if min_location_failed is not None:
+            self._values["min_location_failed"] = min_location_failed
+        if monitor_name is not None:
+            self._values["monitor_name"] = monitor_name
+        if monitor_options is not None:
+            self._values["monitor_options"] = monitor_options
+        if monitor_priority is not None:
+            self._values["monitor_priority"] = monitor_priority
+        if no_screenshot is not None:
+            self._values["no_screenshot"] = no_screenshot
+        if restricted_roles is not None:
+            self._values["restricted_roles"] = restricted_roles
+        if retry is not None:
+            self._values["retry"] = retry
+        if rum_settings is not None:
+            self._values["rum_settings"] = rum_settings
+        if scheduling is not None:
+            self._values["scheduling"] = scheduling
+
+    @builtins.property
+    def tick_every(self) -> jsii.Number:
+        '''How often the test should run (in seconds).
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#tick_every SyntheticsTest#tick_every}
+        '''
+        result = self._values.get("tick_every")
+        assert result is not None, "Required property 'tick_every' is missing"
+        return typing.cast(jsii.Number, result)
+
+    @builtins.property
+    def accept_self_signed(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''For SSL test, whether or not the test should allow self signed certificates.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#accept_self_signed SyntheticsTest#accept_self_signed}
+        '''
+        result = self._values.get("accept_self_signed")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def allow_insecure(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Allows loading insecure content for an HTTP test.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#allow_insecure SyntheticsTest#allow_insecure}
+        '''
+        result = self._values.get("allow_insecure")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def check_certificate_revocation(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#check_certificate_revocation SyntheticsTest#check_certificate_revocation}
+        '''
+        result = self._values.get("check_certificate_revocation")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def ci(self) -> typing.Optional[SyntheticsTestOptionsListCi]:
+        '''ci block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ci SyntheticsTest#ci}
+        '''
+        result = self._values.get("ci")
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListCi], result)
+
+    @builtins.property
+    def disable_cors(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Disable Cross-Origin Resource Sharing for browser tests.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_cors SyntheticsTest#disable_cors}
+        '''
+        result = self._values.get("disable_cors")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def disable_csp(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Disable Content Security Policy for browser tests.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#disable_csp SyntheticsTest#disable_csp}
+        '''
+        result = self._values.get("disable_csp")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def follow_redirects(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Determines whether or not the API HTTP test should follow redirects.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#follow_redirects SyntheticsTest#follow_redirects}
+        '''
+        result = self._values.get("follow_redirects")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def http_version(self) -> typing.Optional[builtins.str]:
+        '''HTTP version to use for a Synthetics API test. Valid values are ``http1``, ``http2``, ``any``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#http_version SyntheticsTest#http_version}
+        '''
+        result = self._values.get("http_version")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def ignore_server_certificate_error(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Ignore server certificate error.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#ignore_server_certificate_error SyntheticsTest#ignore_server_certificate_error}
+        '''
+        result = self._values.get("ignore_server_certificate_error")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def initial_navigation_timeout(self) -> typing.Optional[jsii.Number]:
+        '''Timeout before declaring the initial step as failed (in seconds) for browser tests.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#initial_navigation_timeout SyntheticsTest#initial_navigation_timeout}
+        '''
+        result = self._values.get("initial_navigation_timeout")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def min_failure_duration(self) -> typing.Optional[jsii.Number]:
+        '''Minimum amount of time in failure required to trigger an alert (in seconds). Default is ``0``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_failure_duration SyntheticsTest#min_failure_duration}
+        '''
+        result = self._values.get("min_failure_duration")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def min_location_failed(self) -> typing.Optional[jsii.Number]:
+        '''Minimum number of locations in failure required to trigger an alert. Default is ``1``.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#min_location_failed SyntheticsTest#min_location_failed}
+        '''
+        result = self._values.get("min_location_failed")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def monitor_name(self) -> typing.Optional[builtins.str]:
+        '''The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_name SyntheticsTest#monitor_name}
+        '''
+        result = self._values.get("monitor_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def monitor_options(
+        self,
+    ) -> typing.Optional[SyntheticsTestOptionsListMonitorOptions]:
+        '''monitor_options block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_options SyntheticsTest#monitor_options}
+        '''
+        result = self._values.get("monitor_options")
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListMonitorOptions], result)
+
+    @builtins.property
+    def monitor_priority(self) -> typing.Optional[jsii.Number]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#monitor_priority SyntheticsTest#monitor_priority}.'''
+        result = self._values.get("monitor_priority")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def no_screenshot(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Prevents saving screenshots of the steps.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#no_screenshot SyntheticsTest#no_screenshot}
+        '''
+        result = self._values.get("no_screenshot")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
+    def restricted_roles(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''A list of role identifiers pulled from the Roles API to restrict read and write access.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#restricted_roles SyntheticsTest#restricted_roles}
+        '''
+        result = self._values.get("restricted_roles")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def retry(self) -> typing.Optional[SyntheticsTestOptionsListRetry]:
+        '''retry block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#retry SyntheticsTest#retry}
+        '''
+        result = self._values.get("retry")
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListRetry], result)
+
+    @builtins.property
+    def rum_settings(self) -> typing.Optional[SyntheticsTestOptionsListRumSettings]:
+        '''rum_settings block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#rum_settings SyntheticsTest#rum_settings}
+        '''
+        result = self._values.get("rum_settings")
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListRumSettings], result)
+
+    @builtins.property
+    def scheduling(self) -> typing.Optional[SyntheticsTestOptionsListScheduling]:
+        '''scheduling block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#scheduling SyntheticsTest#scheduling}
+        '''
+        result = self._values.get("scheduling")
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListScheduling], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SyntheticsTestOptionsListStruct(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class SyntheticsTestOptionsListStructOutputReference(
+    _cdktf_9a9027ec.ComplexObject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-datadog.syntheticsTest.SyntheticsTestOptionsListStructOutputReference",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3ffa5305eb475362a8f229062b7f170fd402e7aa7e116a6ebdcc315ef565e40a)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
+
+    @jsii.member(jsii_name="putCi")
+    def put_ci(self, *, execution_rule: typing.Optional[builtins.str] = None) -> None:
+        '''
+        :param execution_rule: Execution rule for a Synthetics test. Valid values are ``blocking``, ``non_blocking``, ``skipped``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#execution_rule SyntheticsTest#execution_rule}
+        '''
+        value = SyntheticsTestOptionsListCi(execution_rule=execution_rule)
+
+        return typing.cast(None, jsii.invoke(self, "putCi", [value]))
+
+    @jsii.member(jsii_name="putMonitorOptions")
+    def put_monitor_options(
+        self,
+        *,
+        renotify_interval: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param renotify_interval: Specify a renotification frequency in minutes. Values available by default are ``0``, ``10``, ``20``, ``30``, ``40``, ``50``, ``60``, ``90``, ``120``, ``180``, ``240``, ``300``, ``360``, ``720``, ``1440``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#renotify_interval SyntheticsTest#renotify_interval}
+        '''
+        value = SyntheticsTestOptionsListMonitorOptions(
+            renotify_interval=renotify_interval
+        )
+
+        return typing.cast(None, jsii.invoke(self, "putMonitorOptions", [value]))
+
+    @jsii.member(jsii_name="putRetry")
+    def put_retry(
+        self,
+        *,
+        count: typing.Optional[jsii.Number] = None,
+        interval: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param count: Number of retries needed to consider a location as failed before sending a notification alert. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#count SyntheticsTest#count}
+        :param interval: Interval between a failed test and the next retry in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#interval SyntheticsTest#interval}
+        '''
+        value = SyntheticsTestOptionsListRetry(count=count, interval=interval)
+
+        return typing.cast(None, jsii.invoke(self, "putRetry", [value]))
+
+    @jsii.member(jsii_name="putRumSettings")
+    def put_rum_settings(
+        self,
+        *,
+        is_enabled: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+        application_id: typing.Optional[builtins.str] = None,
+        client_token_id: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param is_enabled: Determines whether RUM data is collected during test runs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#is_enabled SyntheticsTest#is_enabled}
+        :param application_id: RUM application ID used to collect RUM data for the browser test. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#application_id SyntheticsTest#application_id}
+        :param client_token_id: RUM application API key ID used to collect RUM data for the browser test. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#client_token_id SyntheticsTest#client_token_id}
+        '''
+        value = SyntheticsTestOptionsListRumSettings(
+            is_enabled=is_enabled,
+            application_id=application_id,
+            client_token_id=client_token_id,
+        )
+
+        return typing.cast(None, jsii.invoke(self, "putRumSettings", [value]))
+
+    @jsii.member(jsii_name="putScheduling")
+    def put_scheduling(
+        self,
+        *,
+        timeframes: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestOptionsListSchedulingTimeframes, typing.Dict[builtins.str, typing.Any]]]],
+        timezone: builtins.str,
+    ) -> None:
+        '''
+        :param timeframes: timeframes block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#timeframes SyntheticsTest#timeframes}
+        :param timezone: Timezone in which the timeframe is based. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/datadog/datadog/3.25.0/docs/resources/synthetics_test#timezone SyntheticsTest#timezone}
+        '''
+        value = SyntheticsTestOptionsListScheduling(
+            timeframes=timeframes, timezone=timezone
+        )
+
+        return typing.cast(None, jsii.invoke(self, "putScheduling", [value]))
+
+    @jsii.member(jsii_name="resetAcceptSelfSigned")
+    def reset_accept_self_signed(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetAcceptSelfSigned", []))
+
+    @jsii.member(jsii_name="resetAllowInsecure")
+    def reset_allow_insecure(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetAllowInsecure", []))
+
+    @jsii.member(jsii_name="resetCheckCertificateRevocation")
+    def reset_check_certificate_revocation(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetCheckCertificateRevocation", []))
+
+    @jsii.member(jsii_name="resetCi")
+    def reset_ci(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetCi", []))
+
+    @jsii.member(jsii_name="resetDisableCors")
+    def reset_disable_cors(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetDisableCors", []))
+
+    @jsii.member(jsii_name="resetDisableCsp")
+    def reset_disable_csp(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetDisableCsp", []))
+
+    @jsii.member(jsii_name="resetFollowRedirects")
+    def reset_follow_redirects(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetFollowRedirects", []))
+
+    @jsii.member(jsii_name="resetHttpVersion")
+    def reset_http_version(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetHttpVersion", []))
+
+    @jsii.member(jsii_name="resetIgnoreServerCertificateError")
+    def reset_ignore_server_certificate_error(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetIgnoreServerCertificateError", []))
+
+    @jsii.member(jsii_name="resetInitialNavigationTimeout")
+    def reset_initial_navigation_timeout(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetInitialNavigationTimeout", []))
+
+    @jsii.member(jsii_name="resetMinFailureDuration")
+    def reset_min_failure_duration(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMinFailureDuration", []))
+
+    @jsii.member(jsii_name="resetMinLocationFailed")
+    def reset_min_location_failed(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMinLocationFailed", []))
+
+    @jsii.member(jsii_name="resetMonitorName")
+    def reset_monitor_name(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMonitorName", []))
+
+    @jsii.member(jsii_name="resetMonitorOptions")
+    def reset_monitor_options(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMonitorOptions", []))
+
+    @jsii.member(jsii_name="resetMonitorPriority")
+    def reset_monitor_priority(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMonitorPriority", []))
+
+    @jsii.member(jsii_name="resetNoScreenshot")
+    def reset_no_screenshot(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetNoScreenshot", []))
+
+    @jsii.member(jsii_name="resetRestrictedRoles")
+    def reset_restricted_roles(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetRestrictedRoles", []))
+
+    @jsii.member(jsii_name="resetRetry")
+    def reset_retry(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetRetry", []))
+
+    @jsii.member(jsii_name="resetRumSettings")
+    def reset_rum_settings(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetRumSettings", []))
+
+    @jsii.member(jsii_name="resetScheduling")
+    def reset_scheduling(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetScheduling", []))
+
+    @builtins.property
+    @jsii.member(jsii_name="ci")
+    def ci(self) -> SyntheticsTestOptionsListCiOutputReference:
+        return typing.cast(SyntheticsTestOptionsListCiOutputReference, jsii.get(self, "ci"))
+
+    @builtins.property
+    @jsii.member(jsii_name="monitorOptions")
+    def monitor_options(self) -> SyntheticsTestOptionsListMonitorOptionsOutputReference:
+        return typing.cast(SyntheticsTestOptionsListMonitorOptionsOutputReference, jsii.get(self, "monitorOptions"))
+
+    @builtins.property
+    @jsii.member(jsii_name="retry")
+    def retry(self) -> SyntheticsTestOptionsListRetryOutputReference:
+        return typing.cast(SyntheticsTestOptionsListRetryOutputReference, jsii.get(self, "retry"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rumSettings")
+    def rum_settings(self) -> SyntheticsTestOptionsListRumSettingsOutputReference:
+        return typing.cast(SyntheticsTestOptionsListRumSettingsOutputReference, jsii.get(self, "rumSettings"))
+
+    @builtins.property
+    @jsii.member(jsii_name="scheduling")
+    def scheduling(self) -> SyntheticsTestOptionsListSchedulingOutputReference:
+        return typing.cast(SyntheticsTestOptionsListSchedulingOutputReference, jsii.get(self, "scheduling"))
+
+    @builtins.property
+    @jsii.member(jsii_name="acceptSelfSignedInput")
+    def accept_self_signed_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "acceptSelfSignedInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="allowInsecureInput")
+    def allow_insecure_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "allowInsecureInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="checkCertificateRevocationInput")
+    def check_certificate_revocation_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "checkCertificateRevocationInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="ciInput")
+    def ci_input(self) -> typing.Optional[SyntheticsTestOptionsListCi]:
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListCi], jsii.get(self, "ciInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="disableCorsInput")
+    def disable_cors_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "disableCorsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="disableCspInput")
+    def disable_csp_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "disableCspInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="followRedirectsInput")
+    def follow_redirects_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "followRedirectsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="httpVersionInput")
+    def http_version_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "httpVersionInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="ignoreServerCertificateErrorInput")
+    def ignore_server_certificate_error_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "ignoreServerCertificateErrorInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="initialNavigationTimeoutInput")
+    def initial_navigation_timeout_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "initialNavigationTimeoutInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="minFailureDurationInput")
+    def min_failure_duration_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "minFailureDurationInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="minLocationFailedInput")
+    def min_location_failed_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "minLocationFailedInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="monitorNameInput")
+    def monitor_name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "monitorNameInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="monitorOptionsInput")
+    def monitor_options_input(
+        self,
+    ) -> typing.Optional[SyntheticsTestOptionsListMonitorOptions]:
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListMonitorOptions], jsii.get(self, "monitorOptionsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="monitorPriorityInput")
+    def monitor_priority_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "monitorPriorityInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="noScreenshotInput")
+    def no_screenshot_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "noScreenshotInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="restrictedRolesInput")
+    def restricted_roles_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "restrictedRolesInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="retryInput")
+    def retry_input(self) -> typing.Optional[SyntheticsTestOptionsListRetry]:
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListRetry], jsii.get(self, "retryInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rumSettingsInput")
+    def rum_settings_input(
+        self,
+    ) -> typing.Optional[SyntheticsTestOptionsListRumSettings]:
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListRumSettings], jsii.get(self, "rumSettingsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="schedulingInput")
+    def scheduling_input(self) -> typing.Optional[SyntheticsTestOptionsListScheduling]:
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListScheduling], jsii.get(self, "schedulingInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="tickEveryInput")
+    def tick_every_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "tickEveryInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="acceptSelfSigned")
+    def accept_self_signed(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "acceptSelfSigned"))
+
+    @accept_self_signed.setter
+    def accept_self_signed(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__06cf576fa7cfe503144f9527e32c668ce7d9c52a204613e80866bd0572de88c6)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "acceptSelfSigned", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="allowInsecure")
+    def allow_insecure(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "allowInsecure"))
+
+    @allow_insecure.setter
+    def allow_insecure(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e8c22b550b303b7815cb79918dc65e901a9a6a8be33150f69f3bc14575d129b4)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "allowInsecure", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="checkCertificateRevocation")
+    def check_certificate_revocation(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "checkCertificateRevocation"))
+
+    @check_certificate_revocation.setter
+    def check_certificate_revocation(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0030a400077275d53812d521ea01a36b316dcc1a51a8684903c1e1ff17768017)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "checkCertificateRevocation", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="disableCors")
+    def disable_cors(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "disableCors"))
+
+    @disable_cors.setter
+    def disable_cors(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b4d9c48705fc4e2d6200b3bdca981778bd5ecc0d5caa7be66054ed34ce73029d)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "disableCors", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="disableCsp")
+    def disable_csp(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "disableCsp"))
+
+    @disable_csp.setter
+    def disable_csp(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__435428d3271652ee8657616ee2e56504ebdcfef9793375d512446e56842056c4)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "disableCsp", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="followRedirects")
+    def follow_redirects(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "followRedirects"))
+
+    @follow_redirects.setter
+    def follow_redirects(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__784f6b0b37d39744c6a8e99445542d3ea30bef0d2481d9bdb51a327092e53d6d)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "followRedirects", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="httpVersion")
+    def http_version(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "httpVersion"))
+
+    @http_version.setter
+    def http_version(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ec4a0ba019ec359492b578d1e499ffdd03b439098a7f0a5fe8525952fbf31480)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "httpVersion", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ignoreServerCertificateError")
+    def ignore_server_certificate_error(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "ignoreServerCertificateError"))
+
+    @ignore_server_certificate_error.setter
+    def ignore_server_certificate_error(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__69371ccf195f65f1b7261454ca387e313310a68647c92589e8e89b19c4579aa2)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ignoreServerCertificateError", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="initialNavigationTimeout")
+    def initial_navigation_timeout(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "initialNavigationTimeout"))
+
+    @initial_navigation_timeout.setter
+    def initial_navigation_timeout(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__900222028a569a95e8bd7be9bbf6f61a82c3d8c133e79de7d334ee18c0ff3433)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "initialNavigationTimeout", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="minFailureDuration")
+    def min_failure_duration(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "minFailureDuration"))
+
+    @min_failure_duration.setter
+    def min_failure_duration(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ef4b0fcd0c9a4a9b4d00759bbc85d5d6f383b8fec1f9c606b0dc7b1b053b18e7)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "minFailureDuration", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="minLocationFailed")
+    def min_location_failed(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "minLocationFailed"))
+
+    @min_location_failed.setter
+    def min_location_failed(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c3464c0bf5bf4ace26d60413a9d9a380fd48d5e5885c2589c6c5c4c0fdbc2158)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "minLocationFailed", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="monitorName")
+    def monitor_name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "monitorName"))
+
+    @monitor_name.setter
+    def monitor_name(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bf06116189564658354e3721f1db83a85fef5e1927b21d21e9ed59cdec571d53)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "monitorName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="monitorPriority")
+    def monitor_priority(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "monitorPriority"))
+
+    @monitor_priority.setter
+    def monitor_priority(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__304dd09fdfb48308361dae6452a2abbcbc310ce82b61cdc37cb1450593a9f472)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "monitorPriority", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="noScreenshot")
+    def no_screenshot(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "noScreenshot"))
+
+    @no_screenshot.setter
+    def no_screenshot(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8da2fa1d7b12074025e98d8cc6cd0ba18f6f90c322db6318101a8bedf0f69514)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "noScreenshot", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="restrictedRoles")
+    def restricted_roles(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "restrictedRoles"))
+
+    @restricted_roles.setter
+    def restricted_roles(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f7ce0d3b2b478d719416cc877d713f1cdfd84778cbb1681ea2e98cffb87e8296)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "restrictedRoles", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="tickEvery")
+    def tick_every(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "tickEvery"))
+
+    @tick_every.setter
+    def tick_every(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__34a9ba235e30884c0fcb3b865a348dae7c04af4ccd98ebf993e0a715833a1356)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "tickEvery", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(self) -> typing.Optional[SyntheticsTestOptionsListStruct]:
+        return typing.cast(typing.Optional[SyntheticsTestOptionsListStruct], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[SyntheticsTestOptionsListStruct],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f02e68aa24cda7ec478428c0e99c677f67cab8488f518c9062a09429c1f26d20)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
+@jsii.data_type(
     jsii_type="@cdktf/provider-datadog.syntheticsTest.SyntheticsTestRequestBasicauth",
     jsii_struct_bases=[],
     name_mapping={
         "access_key": "accessKey",
         "access_token_url": "accessTokenUrl",
         "audience": "audience",
         "client_id": "clientId",
@@ -12584,29 +12585,29 @@
     "SyntheticsTestBrowserVariable",
     "SyntheticsTestBrowserVariableList",
     "SyntheticsTestBrowserVariableOutputReference",
     "SyntheticsTestConfig",
     "SyntheticsTestConfigVariable",
     "SyntheticsTestConfigVariableList",
     "SyntheticsTestConfigVariableOutputReference",
-    "SyntheticsTestOptionsList",
     "SyntheticsTestOptionsListCi",
     "SyntheticsTestOptionsListCiOutputReference",
     "SyntheticsTestOptionsListMonitorOptions",
     "SyntheticsTestOptionsListMonitorOptionsOutputReference",
-    "SyntheticsTestOptionsListOutputReference",
     "SyntheticsTestOptionsListRetry",
     "SyntheticsTestOptionsListRetryOutputReference",
     "SyntheticsTestOptionsListRumSettings",
     "SyntheticsTestOptionsListRumSettingsOutputReference",
     "SyntheticsTestOptionsListScheduling",
     "SyntheticsTestOptionsListSchedulingOutputReference",
     "SyntheticsTestOptionsListSchedulingTimeframes",
     "SyntheticsTestOptionsListSchedulingTimeframesList",
     "SyntheticsTestOptionsListSchedulingTimeframesOutputReference",
+    "SyntheticsTestOptionsListStruct",
+    "SyntheticsTestOptionsListStructOutputReference",
     "SyntheticsTestRequestBasicauth",
     "SyntheticsTestRequestBasicauthOutputReference",
     "SyntheticsTestRequestClientCertificate",
     "SyntheticsTestRequestClientCertificateCert",
     "SyntheticsTestRequestClientCertificateCertOutputReference",
     "SyntheticsTestRequestClientCertificateKey",
     "SyntheticsTestRequestClientCertificateKeyOutputReference",
@@ -12631,15 +12632,15 @@
     assertion: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestAssertion, typing.Dict[builtins.str, typing.Any]]]]] = None,
     browser_step: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestBrowserStep, typing.Dict[builtins.str, typing.Any]]]]] = None,
     browser_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestBrowserVariable, typing.Dict[builtins.str, typing.Any]]]]] = None,
     config_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestConfigVariable, typing.Dict[builtins.str, typing.Any]]]]] = None,
     device_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     message: typing.Optional[builtins.str] = None,
-    options_list: typing.Optional[typing.Union[SyntheticsTestOptionsList, typing.Dict[builtins.str, typing.Any]]] = None,
+    options_list: typing.Optional[typing.Union[SyntheticsTestOptionsListStruct, typing.Dict[builtins.str, typing.Any]]] = None,
     request_basicauth: typing.Optional[typing.Union[SyntheticsTestRequestBasicauth, typing.Dict[builtins.str, typing.Any]]] = None,
     request_client_certificate: typing.Optional[typing.Union[SyntheticsTestRequestClientCertificate, typing.Dict[builtins.str, typing.Any]]] = None,
     request_definition: typing.Optional[typing.Union[SyntheticsTestRequestDefinition, typing.Dict[builtins.str, typing.Any]]] = None,
     request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     request_proxy: typing.Optional[typing.Union[SyntheticsTestRequestProxy, typing.Dict[builtins.str, typing.Any]]] = None,
     request_query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     set_cookie: typing.Optional[builtins.str] = None,
@@ -14226,15 +14227,15 @@
     assertion: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestAssertion, typing.Dict[builtins.str, typing.Any]]]]] = None,
     browser_step: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestBrowserStep, typing.Dict[builtins.str, typing.Any]]]]] = None,
     browser_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestBrowserVariable, typing.Dict[builtins.str, typing.Any]]]]] = None,
     config_variable: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestConfigVariable, typing.Dict[builtins.str, typing.Any]]]]] = None,
     device_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     message: typing.Optional[builtins.str] = None,
-    options_list: typing.Optional[typing.Union[SyntheticsTestOptionsList, typing.Dict[builtins.str, typing.Any]]] = None,
+    options_list: typing.Optional[typing.Union[SyntheticsTestOptionsListStruct, typing.Dict[builtins.str, typing.Any]]] = None,
     request_basicauth: typing.Optional[typing.Union[SyntheticsTestRequestBasicauth, typing.Dict[builtins.str, typing.Any]]] = None,
     request_client_certificate: typing.Optional[typing.Union[SyntheticsTestRequestClientCertificate, typing.Dict[builtins.str, typing.Any]]] = None,
     request_definition: typing.Optional[typing.Union[SyntheticsTestRequestDefinition, typing.Dict[builtins.str, typing.Any]]] = None,
     request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     request_proxy: typing.Optional[typing.Union[SyntheticsTestRequestProxy, typing.Dict[builtins.str, typing.Any]]] = None,
     request_query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     set_cookie: typing.Optional[builtins.str] = None,
@@ -14341,41 +14342,14 @@
 
 def _typecheckingstub__9b444e981176453dd5e922485f7598e82982d7d82eac74baa256f9087a7387d2(
     value: typing.Optional[typing.Union[SyntheticsTestConfigVariable, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__669a64b0c857b3913f6e1304a3b7506ac7351d32b12a1e69230b0fd453c12cb3(
-    *,
-    tick_every: jsii.Number,
-    accept_self_signed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    allow_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    check_certificate_revocation: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    ci: typing.Optional[typing.Union[SyntheticsTestOptionsListCi, typing.Dict[builtins.str, typing.Any]]] = None,
-    disable_cors: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    disable_csp: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    follow_redirects: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    http_version: typing.Optional[builtins.str] = None,
-    ignore_server_certificate_error: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    initial_navigation_timeout: typing.Optional[jsii.Number] = None,
-    min_failure_duration: typing.Optional[jsii.Number] = None,
-    min_location_failed: typing.Optional[jsii.Number] = None,
-    monitor_name: typing.Optional[builtins.str] = None,
-    monitor_options: typing.Optional[typing.Union[SyntheticsTestOptionsListMonitorOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    monitor_priority: typing.Optional[jsii.Number] = None,
-    no_screenshot: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
-    restricted_roles: typing.Optional[typing.Sequence[builtins.str]] = None,
-    retry: typing.Optional[typing.Union[SyntheticsTestOptionsListRetry, typing.Dict[builtins.str, typing.Any]]] = None,
-    rum_settings: typing.Optional[typing.Union[SyntheticsTestOptionsListRumSettings, typing.Dict[builtins.str, typing.Any]]] = None,
-    scheduling: typing.Optional[typing.Union[SyntheticsTestOptionsListScheduling, typing.Dict[builtins.str, typing.Any]]] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__c0093f6a14d51c2ea4e6d07755ef1fdafdd0b8b9df89ddaf3c83bdcead75f6b1(
     *,
     execution_rule: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -14420,305 +14394,332 @@
 
 def _typecheckingstub__5d8efaa9b18bd9c319279983db5109ac1996e2195bb489b733584961c476cda0(
     value: typing.Optional[SyntheticsTestOptionsListMonitorOptions],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__78a25caa898b8d54783108c1e76beb3e94a916048730439ebeaa41e3f9b5f518(
-    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-    terraform_attribute: builtins.str,
+def _typecheckingstub__1fa0df52a234c3b47310cd58b4e593d79f53079a82be095d4e9a400d73721761(
+    *,
+    count: typing.Optional[jsii.Number] = None,
+    interval: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__53d8cc461b8a175588b2371ab85da744cfbc1d28ee657a764ce99696f6fe5abf(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__34f7a6dd118f08f139e5f7bad453d6db56808e858890e590831c06ea0b67d9b1(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__906fce1953d4c28ba2f11353abb9b392caddd0f4f980b25309db51dd0c9a9c61(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__bf87c3848106f26b72761924188bfa8e1c621d5ff50f56303b3917d77ba3f61b(
+    value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a32c3a7384117855a7c629b949b1de291a32e238f72ddd1c7a4c2a1e5ad2767b(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__ff86c0adf51363ef99f59806789280e4240ed96cb474f0d1c10bedfbbde53231(
+    value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0b9a91a7f15f54a36f8146eca988c4c423d2799b508f48b6ff93b1e74c6d04d6(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__ede7c007211f47688090c465f761136621636b662b5e7d5d74b059ea4c946b80(
+    value: typing.Optional[SyntheticsTestOptionsListRetry],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__53a828f2f2bef55b4cd3c79f4d8b6c47f3bafb288b6938e80503c908fc12c870(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__f6b5f4754bdd2637d48c2b54704c64d2e1663b2f709176c1af7d043ac9495d03(
+    *,
+    is_enabled: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    application_id: typing.Optional[builtins.str] = None,
+    client_token_id: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d00b97833d2dbef78a26064a602de75790e95112e4b030781b0f2cea9fff5bfa(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__20d8766d459895f2e980c5ddba256e3843de943850f16b95e656f4654ff07697(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f8e5e784ef27d1e683d19436794c752fbf03778c759a219121893f693c3d1f02(
+def _typecheckingstub__8ea5e89582a6b6c11aaa9c5cf42d77175ec3fe0cd96be735cc5ec3e0565e572f(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__11b2b2eae7abfbcdbdd9ded17ab8fb42540bf2a3224afc34a660b3b94d2298f7(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__085bad40cf3518fd9cdc565cec5e66f2fee9b8e86b76d6fcd7b0b53079c40420(
+def _typecheckingstub__70e9a4e989e3e37e049769b11072525a15aad3d74e73e59e35fb80fa832a2a53(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f81380c6e2b43101946551969262f72f5bfbedbf1c9264024d140575cdb54869(
-    value: jsii.Number,
+def _typecheckingstub__aac0c828c4a937c80fe94ec79a2ceff1e6ad10dcba147d9b749326fc9a6afc9d(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6d814b7fd09e8de93d2029a5aa5775ab294dad5122009f972d6f33cf8a3f27aa(
-    value: jsii.Number,
+def _typecheckingstub__e1663cc5a33c5ad00036ef45aeb874a10a96854513a0a61fb3ae644a5a5bddd8(
+    value: typing.Optional[SyntheticsTestOptionsListRumSettings],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__604143bda0c23e6b2265036f1a03f897d17524780be0282b7a53c5bfa9b01eb8(
-    value: builtins.str,
+def _typecheckingstub__6433945945039476af498afb9f063790dcd37b61126c86fe56a1c6ad700b3884(
+    *,
+    timeframes: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestOptionsListSchedulingTimeframes, typing.Dict[builtins.str, typing.Any]]]],
+    timezone: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__540f0fa4d54daea7a660a4e69ca7bc1626abdf616ea9ef3fc8daaae0dba94932(
-    value: jsii.Number,
+def _typecheckingstub__864c6afaa59d8100a0fcc1f03d5534a333e76c6e484a02e46c3a7a45d8d26c58(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__068da975e3df412bc6fb59c03e825c41a7d5af36551c532ce316775c83fb2bf5(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__e2ae951b6345aec7073db9a40c78c7ce1056baec44d32fdcebbfadc767326f95(
+    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestOptionsListSchedulingTimeframes, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ef9908b06b86576577772fe00d5df0be963b39c1142a17f9e6aeb9f196f1bd86(
-    value: typing.List[builtins.str],
+def _typecheckingstub__b3baf72f02b6475616478e086a270743dede7fddaf1058745a04b392a91c9307(
+    value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__82e67e70c1e41308d26d3e1f4fd1c484ab3ab7b8ec6a7bd1a73ee6bce9579811(
-    value: jsii.Number,
+def _typecheckingstub__1a0cf738841fc394724e4a8aacc00ae3bb5caaf0f50ec0f629dfdbec32533b47(
+    value: typing.Optional[SyntheticsTestOptionsListScheduling],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f92ac44590f538d77cdce4d44de1454c856fc44753f6ddfa1fc43ab723ed6343(
-    value: typing.Optional[SyntheticsTestOptionsList],
+def _typecheckingstub__adc2ea76ab0f1cbf193fec28e452cd7dda8e0ff496c82704fccf503401afde9e(
+    *,
+    day: jsii.Number,
+    from_: builtins.str,
+    to: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1fa0df52a234c3b47310cd58b4e593d79f53079a82be095d4e9a400d73721761(
-    *,
-    count: typing.Optional[jsii.Number] = None,
-    interval: typing.Optional[jsii.Number] = None,
+def _typecheckingstub__527072430dc1b8ecb743eeb57958fed7b0fe814acc910ceab4985b4029b1471c(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__34f7a6dd118f08f139e5f7bad453d6db56808e858890e590831c06ea0b67d9b1(
-    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-    terraform_attribute: builtins.str,
+def _typecheckingstub__ec4a0594c49056f4fb6b2ddbc58e0c6beb9d41582e29063deb09bc1d6efe0efe(
+    index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bf87c3848106f26b72761924188bfa8e1c621d5ff50f56303b3917d77ba3f61b(
-    value: jsii.Number,
+def _typecheckingstub__058409c34e6023f88ca582536fd6230e230348a4607392cc39c9616876c539ea(
+    value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ff86c0adf51363ef99f59806789280e4240ed96cb474f0d1c10bedfbbde53231(
-    value: jsii.Number,
+def _typecheckingstub__5eaedb45e6a5180f2996a8fbb5881314bdcbc6b91a621434d7e1dcca47488428(
+    value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ede7c007211f47688090c465f761136621636b662b5e7d5d74b059ea4c946b80(
-    value: typing.Optional[SyntheticsTestOptionsListRetry],
+def _typecheckingstub__6d9fd13da3237903b8e665c2c2d6b610ce03b6f4e2c7342e4e97be2da27ef5db(
+    value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f6b5f4754bdd2637d48c2b54704c64d2e1663b2f709176c1af7d043ac9495d03(
-    *,
-    is_enabled: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
-    application_id: typing.Optional[builtins.str] = None,
-    client_token_id: typing.Optional[jsii.Number] = None,
+def _typecheckingstub__643bbb0382c4027797b02deebc680d82e2e581cf77668f1697db3a2fae91882c(
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[SyntheticsTestOptionsListSchedulingTimeframes]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__20d8766d459895f2e980c5ddba256e3843de943850f16b95e656f4654ff07697(
+def _typecheckingstub__3892c88219c497d3d139366cf73a727606deccadd1a6aa9f687109e12ca6101f(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
+    complex_object_index: jsii.Number,
+    complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8ea5e89582a6b6c11aaa9c5cf42d77175ec3fe0cd96be735cc5ec3e0565e572f(
-    value: builtins.str,
+def _typecheckingstub__b42c6bed1710ee91d54b5fba383fddaa768eb93c121c85efc38b0cbb74675f69(
+    value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__70e9a4e989e3e37e049769b11072525a15aad3d74e73e59e35fb80fa832a2a53(
-    value: jsii.Number,
+def _typecheckingstub__4bbe592c2c1aabf1676e68cc3abcb4a6804d6e5d6abf9ce6e40ed81c036790f8(
+    value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__aac0c828c4a937c80fe94ec79a2ceff1e6ad10dcba147d9b749326fc9a6afc9d(
-    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+def _typecheckingstub__87d6567d4180a02582d811bfa90fc89d6e7bbc425a4a1d4bf6b2f66b7d65a6d2(
+    value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e1663cc5a33c5ad00036ef45aeb874a10a96854513a0a61fb3ae644a5a5bddd8(
-    value: typing.Optional[SyntheticsTestOptionsListRumSettings],
+def _typecheckingstub__669853ac122cd3d3ae92702f8c2c07dba4d00caa40cc211569e7857ca6d48ebd(
+    value: typing.Optional[typing.Union[SyntheticsTestOptionsListSchedulingTimeframes, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6433945945039476af498afb9f063790dcd37b61126c86fe56a1c6ad700b3884(
+def _typecheckingstub__e136bc90e4e687f03e8828ece8dd8370e3f9171ef719b48228a02707d84ae0dc(
     *,
-    timeframes: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestOptionsListSchedulingTimeframes, typing.Dict[builtins.str, typing.Any]]]],
-    timezone: builtins.str,
+    tick_every: jsii.Number,
+    accept_self_signed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    allow_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    check_certificate_revocation: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    ci: typing.Optional[typing.Union[SyntheticsTestOptionsListCi, typing.Dict[builtins.str, typing.Any]]] = None,
+    disable_cors: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    disable_csp: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    follow_redirects: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    http_version: typing.Optional[builtins.str] = None,
+    ignore_server_certificate_error: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    initial_navigation_timeout: typing.Optional[jsii.Number] = None,
+    min_failure_duration: typing.Optional[jsii.Number] = None,
+    min_location_failed: typing.Optional[jsii.Number] = None,
+    monitor_name: typing.Optional[builtins.str] = None,
+    monitor_options: typing.Optional[typing.Union[SyntheticsTestOptionsListMonitorOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    monitor_priority: typing.Optional[jsii.Number] = None,
+    no_screenshot: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    restricted_roles: typing.Optional[typing.Sequence[builtins.str]] = None,
+    retry: typing.Optional[typing.Union[SyntheticsTestOptionsListRetry, typing.Dict[builtins.str, typing.Any]]] = None,
+    rum_settings: typing.Optional[typing.Union[SyntheticsTestOptionsListRumSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+    scheduling: typing.Optional[typing.Union[SyntheticsTestOptionsListScheduling, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__864c6afaa59d8100a0fcc1f03d5534a333e76c6e484a02e46c3a7a45d8d26c58(
+def _typecheckingstub__3ffa5305eb475362a8f229062b7f170fd402e7aa7e116a6ebdcc315ef565e40a(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e2ae951b6345aec7073db9a40c78c7ce1056baec44d32fdcebbfadc767326f95(
-    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[SyntheticsTestOptionsListSchedulingTimeframes, typing.Dict[builtins.str, typing.Any]]]],
+def _typecheckingstub__06cf576fa7cfe503144f9527e32c668ce7d9c52a204613e80866bd0572de88c6(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b3baf72f02b6475616478e086a270743dede7fddaf1058745a04b392a91c9307(
-    value: builtins.str,
+def _typecheckingstub__e8c22b550b303b7815cb79918dc65e901a9a6a8be33150f69f3bc14575d129b4(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1a0cf738841fc394724e4a8aacc00ae3bb5caaf0f50ec0f629dfdbec32533b47(
-    value: typing.Optional[SyntheticsTestOptionsListScheduling],
+def _typecheckingstub__0030a400077275d53812d521ea01a36b316dcc1a51a8684903c1e1ff17768017(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__adc2ea76ab0f1cbf193fec28e452cd7dda8e0ff496c82704fccf503401afde9e(
-    *,
-    day: jsii.Number,
-    from_: builtins.str,
-    to: builtins.str,
+def _typecheckingstub__b4d9c48705fc4e2d6200b3bdca981778bd5ecc0d5caa7be66054ed34ce73029d(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__527072430dc1b8ecb743eeb57958fed7b0fe814acc910ceab4985b4029b1471c(
-    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-    terraform_attribute: builtins.str,
-    wraps_set: builtins.bool,
+def _typecheckingstub__435428d3271652ee8657616ee2e56504ebdcfef9793375d512446e56842056c4(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ec4a0594c49056f4fb6b2ddbc58e0c6beb9d41582e29063deb09bc1d6efe0efe(
-    index: jsii.Number,
+def _typecheckingstub__784f6b0b37d39744c6a8e99445542d3ea30bef0d2481d9bdb51a327092e53d6d(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__058409c34e6023f88ca582536fd6230e230348a4607392cc39c9616876c539ea(
+def _typecheckingstub__ec4a0ba019ec359492b578d1e499ffdd03b439098a7f0a5fe8525952fbf31480(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__5eaedb45e6a5180f2996a8fbb5881314bdcbc6b91a621434d7e1dcca47488428(
-    value: _cdktf_9a9027ec.IInterpolatingParent,
+def _typecheckingstub__69371ccf195f65f1b7261454ca387e313310a68647c92589e8e89b19c4579aa2(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6d9fd13da3237903b8e665c2c2d6b610ce03b6f4e2c7342e4e97be2da27ef5db(
-    value: builtins.bool,
+def _typecheckingstub__900222028a569a95e8bd7be9bbf6f61a82c3d8c133e79de7d334ee18c0ff3433(
+    value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__643bbb0382c4027797b02deebc680d82e2e581cf77668f1697db3a2fae91882c(
-    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[SyntheticsTestOptionsListSchedulingTimeframes]]],
+def _typecheckingstub__ef4b0fcd0c9a4a9b4d00759bbc85d5d6f383b8fec1f9c606b0dc7b1b053b18e7(
+    value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3892c88219c497d3d139366cf73a727606deccadd1a6aa9f687109e12ca6101f(
-    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
-    terraform_attribute: builtins.str,
-    complex_object_index: jsii.Number,
-    complex_object_is_from_set: builtins.bool,
+def _typecheckingstub__c3464c0bf5bf4ace26d60413a9d9a380fd48d5e5885c2589c6c5c4c0fdbc2158(
+    value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b42c6bed1710ee91d54b5fba383fddaa768eb93c121c85efc38b0cbb74675f69(
+def _typecheckingstub__bf06116189564658354e3721f1db83a85fef5e1927b21d21e9ed59cdec571d53(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__304dd09fdfb48308361dae6452a2abbcbc310ce82b61cdc37cb1450593a9f472(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4bbe592c2c1aabf1676e68cc3abcb4a6804d6e5d6abf9ce6e40ed81c036790f8(
-    value: builtins.str,
+def _typecheckingstub__8da2fa1d7b12074025e98d8cc6cd0ba18f6f90c322db6318101a8bedf0f69514(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__87d6567d4180a02582d811bfa90fc89d6e7bbc425a4a1d4bf6b2f66b7d65a6d2(
-    value: builtins.str,
+def _typecheckingstub__f7ce0d3b2b478d719416cc877d713f1cdfd84778cbb1681ea2e98cffb87e8296(
+    value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__669853ac122cd3d3ae92702f8c2c07dba4d00caa40cc211569e7857ca6d48ebd(
-    value: typing.Optional[typing.Union[SyntheticsTestOptionsListSchedulingTimeframes, _cdktf_9a9027ec.IResolvable]],
+def _typecheckingstub__34a9ba235e30884c0fcb3b865a348dae7c04af4ccd98ebf993e0a715833a1356(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f02e68aa24cda7ec478428c0e99c677f67cab8488f518c9062a09429c1f26d20(
+    value: typing.Optional[SyntheticsTestOptionsListStruct],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__fc5a48ceb2c2bf2e059d12af9f1e014c367434553afc8a2394e787c56f997510(
     *,
     access_key: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/user/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/webhook/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog/webhook_custom_variable/__init__.py` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog/webhook_custom_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/PKG-INFO` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-datadog
-Version: 6.0.3
+Version: 6.0.4
 Summary: Prebuilt datadog Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-datadog.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-datadog.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform datadog Provider version 1:1. In fact, it always tracks `latest` of `~> 3.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform datadog Provider](https://github.com/terraform-providers/terraform-provider-datadog)
+* [Terraform datadog Provider](https://registry.terraform.io/providers/DataDog/datadog/3.0.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-datadog/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-datadog-6.0.3/src/cdktf_cdktf_provider_datadog.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-datadog-6.0.4/src/cdktf_cdktf_provider_datadog.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_datadog/py.typed
 src/cdktf_cdktf_provider_datadog.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_datadog.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_datadog.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_datadog.egg-info/requires.txt
 src/cdktf_cdktf_provider_datadog.egg-info/top_level.txt
 src/cdktf_cdktf_provider_datadog/_jsii/__init__.py
-src/cdktf_cdktf_provider_datadog/_jsii/provider-datadog@6.0.3.jsii.tgz
+src/cdktf_cdktf_provider_datadog/_jsii/provider-datadog@6.0.4.jsii.tgz
 src/cdktf_cdktf_provider_datadog/api_key/__init__.py
 src/cdktf_cdktf_provider_datadog/application_key/__init__.py
 src/cdktf_cdktf_provider_datadog/authn_mapping/__init__.py
 src/cdktf_cdktf_provider_datadog/child_organization/__init__.py
 src/cdktf_cdktf_provider_datadog/cloud_configuration_rule/__init__.py
 src/cdktf_cdktf_provider_datadog/cloud_workload_security_agent_rule/__init__.py
 src/cdktf_cdktf_provider_datadog/dashboard/__init__.py
```

