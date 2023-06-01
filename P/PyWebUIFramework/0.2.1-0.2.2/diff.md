# Comparing `tmp/PyWebUIFramework-0.2.1.tar.gz` & `tmp/PyWebUIFramework-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyWebUIFramework-0.2.1.tar", last modified: Thu Jun  1 18:49:45 2023, max compression
+gzip compressed data, was "dist\PyWebUIFramework-0.2.2.tar", last modified: Thu Jun  1 18:51:30 2023, max compression
```

## Comparing `PyWebUIFramework-0.2.1.tar` & `PyWebUIFramework-0.2.2.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/
--rw-rw-rw-   0        0        0      279 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-01 17:52:31.000000 PyWebUIFramework-0.2.1/README.md
--rw-rw-rw-   0        0        0      115 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-06-01 18:49:41.000000 PyWebUIFramework-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/PyWebUIFramework.egg-info/
--rw-rw-rw-   0        0        0      279 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/PyWebUIFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4282 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/PyWebUIFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/PyWebUIFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/PyWebUIFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/PyWebUIFramework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/browser/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/browser/__init__.py
--rw-rw-rw-   0        0        0      144 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/browser/alert_actions.py
--rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/browser/base_browser_factory.py
--rw-rw-rw-   0        0        0     8244 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/browser/browser.py
--rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/browser/browser_module.py
--rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/browser/browser_name.py
--rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/browser/browser_tab_navigation.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/browser/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/browser/interfaces/__init__.py
--rw-rw-rw-   0        0        0      567 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/browser/interfaces/browser_factory_interface.py
--rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/browser/java_script.py
--rw-rw-rw-   0        0        0     2128 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/browser/local_browser_factory.py
--rw-rw-rw-   0        0        0     4731 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/browser/py_quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/configuration/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/configuration/__init__.py
--rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/configuration/browser_profile.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/configuration/driver_settings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/configuration/driver_settings/__init__.py
--rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/configuration/driver_settings/base_driver_settings.py
--rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/configuration/driver_settings/chrome_settings.py
--rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/configuration/driver_settings/edge_settings.py
--rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/configuration/driver_settings/firefox_settings.py
--rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/configuration/driver_settings/iexplorer_settings.py
--rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/configuration/timeout.py
--rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/configuration/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/applications/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/applications/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/applications/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/applications/interfaces/__init__.py
--rw-rw-rw-   0        0        0      331 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/applications/interfaces/application_interface.py
--rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/core/applications/quality_module.py
--rw-rw-rw-   0        0        0     2255 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/core/applications/quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/configurations/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/configurations/configuration_module.py
--rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/configurations/element_cache_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/configurations/interfaces/browser_profile_interface.py
--rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/configurations/interfaces/retry_configuration_interface.py
--rw-rw-rw-   0        0        0     1466 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/core/configurations/interfaces/timeout_configuration_interface.py
--rw-rw-rw-   0        0        0      882 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/core/configurations/retry_configuration.py
--rw-rw-rw-   0        0        0     1198 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/core/configurations/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/elements/actions/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/elements/actions/__init__.py
--rw-rw-rw-   0        0        0     2809 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.1/src/core/elements/actions/js_actions.py
--rw-rw-rw-   0        0        0    11790 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/base_element.py
--rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/base_element_cache_handler.py
--rw-rw-rw-   0        0        0     5701 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/base_element_factory.py
--rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/base_parent_element.py
--rw-rw-rw-   0        0        0      797 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/element_cache_handler.py
--rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/element_factory.py
--rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/element_finder.py
--rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/element_finder_interface.py
--rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/elements/highlight_state.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/elements/states/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/elements/states/__init__.py
--rw-rw-rw-   0        0        0     4306 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/core/elements/states/base_element_state_provider.py
--rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/core/elements/states/cached_element_state_provider.py
--rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/core/elements/states/desired_state.py
--rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/elements/states/element_count.py
--rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/elements/states/element_state.py
--rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/elements/states/element_state_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/localization/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/localization/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/configurations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/localization/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py
--rw-rw-rw-   0        0        0      991 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/localization/configurations/logger_configuration.py
--rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/core/localization/localization_module.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/localization/loggers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/localization/loggers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/loggers/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/localization/loggers/interfaces/localized_logger_interface.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/localization/loggers/localized_logger.py
--rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/loggers/logger_config.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/localization/managers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/managers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/localization/managers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/managers/interfaces/__init__.py
--rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/localization/managers/interfaces/localization_interface.py
--rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/localization/managers/localization_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/utilities/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/utilities/action_repeater.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/utilities/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/utilities/interfaces/__init__.py
--rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/utilities/interfaces/action_repeater_interface.py
--rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/utilities/interfaces/settings_file_interface.py
--rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/utilities/json_settings_file.py
--rw-rw-rw-   0        0        0     1474 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/utilities/resource_file.py
--rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/utilities/utilities_module.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/waitings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/waitings/__init__.py
--rw-rw-rw-   0        0        0     5577 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/core/waitings/conditional_wait.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/core/waitings/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/waitings/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/core/waitings/interfaces/conditional_wait_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/elements/__init__.py
--rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/elements/attributes.py
--rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/elements/button.py
--rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/elements/check_box.py
--rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/elements/checkable_element.py
--rw-rw-rw-   0        0        0      295 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/elements/combo_box.py
--rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.1/src/elements/element_factory.py
--rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/elements/label.py
--rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/elements/link.py
--rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/elements/radio_button.py
--rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/elements/text_box.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:49:45.000000 PyWebUIFramework-0.2.1/src/forms/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.1/src/forms/__init__.py
--rw-rw-rw-   0        0        0     1174 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.1/src/forms/base_form.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/
+-rw-rw-rw-   0        0        0      279 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-01 17:52:31.000000 PyWebUIFramework-0.2.2/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      570 2023-06-01 18:51:22.000000 PyWebUIFramework-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:29.000000 PyWebUIFramework-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/PyWebUIFramework.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-06-01 18:51:29.000000 PyWebUIFramework-0.2.2/src/PyWebUIFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-06-01 18:51:29.000000 PyWebUIFramework-0.2.2/src/PyWebUIFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:51:29.000000 PyWebUIFramework-0.2.2/src/PyWebUIFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-06-01 18:51:29.000000 PyWebUIFramework-0.2.2/src/PyWebUIFramework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:51:29.000000 PyWebUIFramework-0.2.2/src/PyWebUIFramework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/browser/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/browser/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/browser/alert_actions.py
+-rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/browser/base_browser_factory.py
+-rw-rw-rw-   0        0        0     8244 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/browser/browser.py
+-rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/browser/browser_module.py
+-rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/browser/browser_name.py
+-rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/browser/browser_tab_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/browser/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/browser/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      567 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/browser/interfaces/browser_factory_interface.py
+-rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/browser/java_script.py
+-rw-rw-rw-   0        0        0     2128 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/browser/local_browser_factory.py
+-rw-rw-rw-   0        0        0     4731 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/browser/py_quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/configuration/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/configuration/browser_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/configuration/driver_settings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/configuration/driver_settings/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/configuration/driver_settings/base_driver_settings.py
+-rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/configuration/driver_settings/chrome_settings.py
+-rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/configuration/driver_settings/edge_settings.py
+-rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/configuration/driver_settings/firefox_settings.py
+-rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/configuration/driver_settings/iexplorer_settings.py
+-rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/configuration/timeout.py
+-rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/configuration/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/applications/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/applications/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/applications/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/applications/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/applications/interfaces/application_interface.py
+-rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/core/applications/quality_module.py
+-rw-rw-rw-   0        0        0     2255 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/core/applications/quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/configurations/configuration_module.py
+-rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/configurations/element_cache_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/configurations/interfaces/browser_profile_interface.py
+-rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/configurations/interfaces/retry_configuration_interface.py
+-rw-rw-rw-   0        0        0     1466 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/core/configurations/interfaces/timeout_configuration_interface.py
+-rw-rw-rw-   0        0        0      882 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/core/configurations/retry_configuration.py
+-rw-rw-rw-   0        0        0     1198 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/core/configurations/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/elements/actions/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/elements/actions/__init__.py
+-rw-rw-rw-   0        0        0     2809 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2.2/src/core/elements/actions/js_actions.py
+-rw-rw-rw-   0        0        0    11790 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/base_element.py
+-rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/base_element_cache_handler.py
+-rw-rw-rw-   0        0        0     5701 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/base_element_factory.py
+-rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/base_parent_element.py
+-rw-rw-rw-   0        0        0      797 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/element_cache_handler.py
+-rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/element_factory.py
+-rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/element_finder.py
+-rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/element_finder_interface.py
+-rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/elements/highlight_state.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/elements/states/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/elements/states/__init__.py
+-rw-rw-rw-   0        0        0     4306 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/core/elements/states/base_element_state_provider.py
+-rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/core/elements/states/cached_element_state_provider.py
+-rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/core/elements/states/desired_state.py
+-rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/elements/states/element_count.py
+-rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/elements/states/element_state.py
+-rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/elements/states/element_state_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/localization/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/localization/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/configurations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/localization/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/configurations/interfaces/logger_configuration_interface.py
+-rw-rw-rw-   0        0        0      991 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/localization/configurations/logger_configuration.py
+-rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/core/localization/localization_module.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/localization/loggers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/localization/loggers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/loggers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/localization/loggers/interfaces/localized_logger_interface.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/localization/loggers/localized_logger.py
+-rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/loggers/logger_config.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/localization/managers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/managers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/localization/managers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/managers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/localization/managers/interfaces/localization_interface.py
+-rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/localization/managers/localization_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/utilities/action_repeater.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/utilities/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/utilities/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/utilities/interfaces/action_repeater_interface.py
+-rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/utilities/interfaces/settings_file_interface.py
+-rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/utilities/json_settings_file.py
+-rw-rw-rw-   0        0        0     1474 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/utilities/resource_file.py
+-rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/utilities/utilities_module.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/waitings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/waitings/__init__.py
+-rw-rw-rw-   0        0        0     5577 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/core/waitings/conditional_wait.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/core/waitings/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/waitings/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/core/waitings/interfaces/conditional_wait_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/elements/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/elements/attributes.py
+-rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/elements/button.py
+-rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/elements/check_box.py
+-rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/elements/checkable_element.py
+-rw-rw-rw-   0        0        0      295 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/elements/combo_box.py
+-rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2.2/src/elements/element_factory.py
+-rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/elements/label.py
+-rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/elements/link.py
+-rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/elements/radio_button.py
+-rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/elements/text_box.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:51:30.000000 PyWebUIFramework-0.2.2/src/forms/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2.2/src/forms/__init__.py
+-rw-rw-rw-   0        0        0     1174 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2.2/src/forms/base_form.py
```

### Comparing `PyWebUIFramework-0.2.1/setup.py` & `PyWebUIFramework-0.2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="PyWebUIFramework",
-    version="0.2.1",
+    version="0.2.2",
     license="MIT",
     author="Philip Vasilevsky",
     author_email="fil13698@gmail.com",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/philip136/PyWebUIFramework",
     keywords="PyWebUIFrame",
     install_requires=[
         "injector==0.18.4",
-        "jsonpath-ng==1.5.3"
-        "loguru==0.5.3"
+        "jsonpath-ng==1.5.3",
+        "loguru==0.5.3",
         "selenium==3.141.0",
         "webdriver-manager==3.4.2",
         "urllib3==1.26.6"
     ]
 )
```

### Comparing `PyWebUIFramework-0.2.1/src/PyWebUIFramework.egg-info/SOURCES.txt` & `PyWebUIFramework-0.2.2/src/PyWebUIFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/base_browser_factory.py` & `PyWebUIFramework-0.2.2/src/browser/base_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/browser.py` & `PyWebUIFramework-0.2.2/src/browser/browser.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/browser_module.py` & `PyWebUIFramework-0.2.2/src/browser/browser_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/browser_tab_navigation.py` & `PyWebUIFramework-0.2.2/src/browser/browser_tab_navigation.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/interfaces/browser_factory_interface.py` & `PyWebUIFramework-0.2.2/src/browser/interfaces/browser_factory_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/java_script.py` & `PyWebUIFramework-0.2.2/src/browser/java_script.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/local_browser_factory.py` & `PyWebUIFramework-0.2.2/src/browser/local_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/browser/py_quality_services.py` & `PyWebUIFramework-0.2.2/src/browser/py_quality_services.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/configuration/browser_profile.py` & `PyWebUIFramework-0.2.2/src/configuration/browser_profile.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/configuration/driver_settings/base_driver_settings.py` & `PyWebUIFramework-0.2.2/src/configuration/driver_settings/base_driver_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/configuration/driver_settings/chrome_settings.py` & `PyWebUIFramework-0.2.2/src/configuration/driver_settings/chrome_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/configuration/driver_settings/edge_settings.py` & `PyWebUIFramework-0.2.2/src/configuration/driver_settings/edge_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/configuration/driver_settings/firefox_settings.py` & `PyWebUIFramework-0.2.2/src/configuration/driver_settings/firefox_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/configuration/driver_settings/iexplorer_settings.py` & `PyWebUIFramework-0.2.2/src/configuration/driver_settings/iexplorer_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/configuration/timeout_configuration.py` & `PyWebUIFramework-0.2.2/src/configuration/timeout_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/applications/quality_module.py` & `PyWebUIFramework-0.2.2/src/core/applications/quality_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/applications/quality_services.py` & `PyWebUIFramework-0.2.2/src/core/applications/quality_services.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/configurations/configuration_module.py` & `PyWebUIFramework-0.2.2/src/core/configurations/configuration_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/configurations/element_cache_configuration.py` & `PyWebUIFramework-0.2.2/src/core/configurations/element_cache_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/configurations/interfaces/browser_profile_interface.py` & `PyWebUIFramework-0.2.2/src/core/configurations/interfaces/browser_profile_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/configurations/interfaces/retry_configuration_interface.py` & `PyWebUIFramework-0.2.2/src/core/configurations/interfaces/retry_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/configurations/interfaces/timeout_configuration_interface.py` & `PyWebUIFramework-0.2.2/src/core/configurations/interfaces/timeout_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/configurations/retry_configuration.py` & `PyWebUIFramework-0.2.2/src/core/configurations/retry_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/configurations/timeout_configuration.py` & `PyWebUIFramework-0.2.2/src/core/configurations/timeout_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/actions/js_actions.py` & `PyWebUIFramework-0.2.2/src/core/elements/actions/js_actions.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/base_element.py` & `PyWebUIFramework-0.2.2/src/core/elements/base_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/base_element_cache_handler.py` & `PyWebUIFramework-0.2.2/src/core/elements/base_element_cache_handler.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/base_element_factory.py` & `PyWebUIFramework-0.2.2/src/core/elements/base_element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/base_parent_element.py` & `PyWebUIFramework-0.2.2/src/core/elements/base_parent_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/element_cache_handler.py` & `PyWebUIFramework-0.2.2/src/core/elements/element_cache_handler.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/element_factory.py` & `PyWebUIFramework-0.2.2/src/core/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/element_finder.py` & `PyWebUIFramework-0.2.2/src/core/elements/element_finder.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/element_finder_interface.py` & `PyWebUIFramework-0.2.2/src/core/elements/element_finder_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/states/base_element_state_provider.py` & `PyWebUIFramework-0.2.2/src/core/elements/states/base_element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/states/cached_element_state_provider.py` & `PyWebUIFramework-0.2.2/src/core/elements/states/cached_element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/states/desired_state.py` & `PyWebUIFramework-0.2.2/src/core/elements/states/desired_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/states/element_state.py` & `PyWebUIFramework-0.2.2/src/core/elements/states/element_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/elements/states/element_state_provider.py` & `PyWebUIFramework-0.2.2/src/core/elements/states/element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py` & `PyWebUIFramework-0.2.2/src/core/localization/configurations/interfaces/logger_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/localization/configurations/logger_configuration.py` & `PyWebUIFramework-0.2.2/src/core/localization/configurations/logger_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/localization/localization_module.py` & `PyWebUIFramework-0.2.2/src/core/localization/localization_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/localization/loggers/interfaces/localized_logger_interface.py` & `PyWebUIFramework-0.2.2/src/core/localization/loggers/interfaces/localized_logger_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/localization/loggers/localized_logger.py` & `PyWebUIFramework-0.2.2/src/core/localization/loggers/localized_logger.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/localization/managers/localization_manager.py` & `PyWebUIFramework-0.2.2/src/core/localization/managers/localization_manager.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/utilities/action_repeater.py` & `PyWebUIFramework-0.2.2/src/core/utilities/action_repeater.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/utilities/interfaces/action_repeater_interface.py` & `PyWebUIFramework-0.2.2/src/core/utilities/interfaces/action_repeater_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/utilities/interfaces/settings_file_interface.py` & `PyWebUIFramework-0.2.2/src/core/utilities/interfaces/settings_file_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/utilities/json_settings_file.py` & `PyWebUIFramework-0.2.2/src/core/utilities/json_settings_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/utilities/resource_file.py` & `PyWebUIFramework-0.2.2/src/core/utilities/resource_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/waitings/conditional_wait.py` & `PyWebUIFramework-0.2.2/src/core/waitings/conditional_wait.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/core/waitings/interfaces/conditional_wait_interface.py` & `PyWebUIFramework-0.2.2/src/core/waitings/interfaces/conditional_wait_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/elements/check_box.py` & `PyWebUIFramework-0.2.2/src/elements/check_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/elements/element_factory.py` & `PyWebUIFramework-0.2.2/src/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/elements/text_box.py` & `PyWebUIFramework-0.2.2/src/elements/text_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.2.1/src/forms/base_form.py` & `PyWebUIFramework-0.2.2/src/forms/base_form.py`

 * *Files identical despite different names*

