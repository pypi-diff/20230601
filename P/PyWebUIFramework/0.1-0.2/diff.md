# Comparing `tmp/PyWebUIFramework-0.1.tar.gz` & `tmp/PyWebUIFramework-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyWebUIFramework-0.1.tar", last modified: Thu Jun  1 18:12:38 2023, max compression
+gzip compressed data, was "dist\PyWebUIFramework-0.2.tar", last modified: Thu Jun  1 18:42:58 2023, max compression
```

## Comparing `PyWebUIFramework-0.1.tar` & `PyWebUIFramework-0.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/
--rw-rw-rw-   0        0        0      277 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-01 17:52:31.000000 PyWebUIFramework-0.1/README.md
--rw-rw-rw-   0        0        0      115 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/setup.cfg
--rw-rw-rw-   0        0        0      390 2023-06-01 18:08:40.000000 PyWebUIFramework-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/PyWebUIFramework.egg-info/
--rw-rw-rw-   0        0        0      277 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/PyWebUIFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4239 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/PyWebUIFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/PyWebUIFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/PyWebUIFramework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/browser/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/browser/__init__.py
--rw-rw-rw-   0        0        0      144 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/browser/alert_actions.py
--rw-rw-rw-   0        0        0     2176 2023-06-01 18:05:15.000000 PyWebUIFramework-0.1/src/browser/base_browser_factory.py
--rw-rw-rw-   0        0        0     8276 2023-06-01 18:05:32.000000 PyWebUIFramework-0.1/src/browser/browser.py
--rw-rw-rw-   0        0        0     1151 2023-06-01 18:05:50.000000 PyWebUIFramework-0.1/src/browser/browser_module.py
--rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/browser/browser_name.py
--rw-rw-rw-   0        0        0     3133 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/browser/browser_tab_navigation.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/browser/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/browser/interfaces/__init__.py
--rw-rw-rw-   0        0        0      571 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/browser/interfaces/browser_factory_interface.py
--rw-rw-rw-   0        0        0      782 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/browser/java_script.py
--rw-rw-rw-   0        0        0     2136 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/browser/local_browser_factory.py
--rw-rw-rw-   0        0        0     4767 2023-06-01 18:06:05.000000 PyWebUIFramework-0.1/src/browser/py_quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/configuration/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/configuration/__init__.py
--rw-rw-rw-   0        0        0     2895 2023-06-01 18:06:05.000000 PyWebUIFramework-0.1/src/configuration/browser_profile.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/configuration/driver_settings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/configuration/driver_settings/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/configuration/driver_settings/base_driver_settings.py
--rw-rw-rw-   0        0        0      972 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/configuration/driver_settings/chrome_settings.py
--rw-rw-rw-   0        0        0     1026 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/configuration/driver_settings/edge_settings.py
--rw-rw-rw-   0        0        0     1036 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/configuration/driver_settings/firefox_settings.py
--rw-rw-rw-   0        0        0      740 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/configuration/driver_settings/iexplorer_settings.py
--rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/configuration/timeout.py
--rw-rw-rw-   0        0        0     1400 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/configuration/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/applications/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/applications/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/applications/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/applications/interfaces/__init__.py
--rw-rw-rw-   0        0        0      331 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/applications/interfaces/application_interface.py
--rw-rw-rw-   0        0        0     3373 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/applications/quality_module.py
--rw-rw-rw-   0        0        0     2263 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/applications/quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/configurations/__init__.py
--rw-rw-rw-   0        0        0     1603 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/configurations/configuration_module.py
--rw-rw-rw-   0        0        0      530 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/configurations/element_cache_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0     1689 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/core/configurations/interfaces/browser_profile_interface.py
--rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/configurations/interfaces/retry_configuration_interface.py
--rw-rw-rw-   0        0        0     1470 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/configurations/interfaces/timeout_configuration_interface.py
--rw-rw-rw-   0        0        0      890 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/configurations/retry_configuration.py
--rw-rw-rw-   0        0        0     1206 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/configurations/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/elements/actions/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/elements/actions/__init__.py
--rw-rw-rw-   0        0        0     2837 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/core/elements/actions/js_actions.py
--rw-rw-rw-   0        0        0    11862 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/base_element.py
--rw-rw-rw-   0        0        0     1874 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/base_element_cache_handler.py
--rw-rw-rw-   0        0        0     5737 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/base_element_factory.py
--rw-rw-rw-   0        0        0     2574 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/base_parent_element.py
--rw-rw-rw-   0        0        0      801 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/element_cache_handler.py
--rw-rw-rw-   0        0        0     8568 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/element_factory.py
--rw-rw-rw-   0        0        0     3997 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/element_finder.py
--rw-rw-rw-   0        0        0     2520 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/element_finder_interface.py
--rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/elements/highlight_state.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/elements/states/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/elements/states/__init__.py
--rw-rw-rw-   0        0        0     4314 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/states/base_element_state_provider.py
--rw-rw-rw-   0        0        0     6807 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/states/cached_element_state_provider.py
--rw-rw-rw-   0        0        0     1012 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/states/desired_state.py
--rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/elements/states/element_count.py
--rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/elements/states/element_state.py
--rw-rw-rw-   0        0        0     2732 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/elements/states/element_state_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/localization/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/localization/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/configurations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/localization/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py
--rw-rw-rw-   0        0        0      999 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/localization/configurations/logger_configuration.py
--rw-rw-rw-   0        0        0      937 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/localization/localization_module.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/localization/loggers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/localization/loggers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/loggers/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3708 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/localization/loggers/interfaces/localized_logger_interface.py
--rw-rw-rw-   0        0        0     3907 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/localization/loggers/localized_logger.py
--rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/loggers/logger_config.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/localization/managers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/managers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/localization/managers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/managers/interfaces/__init__.py
--rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/localization/managers/interfaces/localization_interface.py
--rw-rw-rw-   0        0        0     2278 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/localization/managers/localization_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/utilities/__init__.py
--rw-rw-rw-   0        0        0     1691 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/utilities/action_repeater.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/utilities/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/utilities/interfaces/__init__.py
--rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/utilities/interfaces/action_repeater_interface.py
--rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/utilities/interfaces/settings_file_interface.py
--rw-rw-rw-   0        0        0     3395 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/utilities/json_settings_file.py
--rw-rw-rw-   0        0        0     1474 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/utilities/resource_file.py
--rw-rw-rw-   0        0        0      399 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/utilities/utilities_module.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/waitings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/waitings/__init__.py
--rw-rw-rw-   0        0        0     5589 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/core/waitings/conditional_wait.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/core/waitings/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/waitings/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/core/waitings/interfaces/conditional_wait_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/elements/__init__.py
--rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/elements/attributes.py
--rw-rw-rw-   0        0        0      219 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/button.py
--rw-rw-rw-   0        0        0      520 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/check_box.py
--rw-rw-rw-   0        0        0      440 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/checkable_element.py
--rw-rw-rw-   0        0        0      299 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/combo_box.py
--rw-rw-rw-   0        0        0     1732 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/element_factory.py
--rw-rw-rw-   0        0        0      217 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/label.py
--rw-rw-rw-   0        0        0      296 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/link.py
--rw-rw-rw-   0        0        0      233 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/radio_button.py
--rw-rw-rw-   0        0        0     1788 2023-06-01 18:03:26.000000 PyWebUIFramework-0.1/src/elements/text_box.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:12:38.000000 PyWebUIFramework-0.1/src/forms/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.1/src/forms/__init__.py
--rw-rw-rw-   0        0        0     1178 2023-06-01 18:03:46.000000 PyWebUIFramework-0.1/src/forms/base_form.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/
+-rw-rw-rw-   0        0        0      277 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-01 17:52:31.000000 PyWebUIFramework-0.2/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      390 2023-06-01 18:42:43.000000 PyWebUIFramework-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/PyWebUIFramework.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/PyWebUIFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4239 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/PyWebUIFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/PyWebUIFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/PyWebUIFramework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/browser/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/browser/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/browser/alert_actions.py
+-rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/browser/base_browser_factory.py
+-rw-rw-rw-   0        0        0     8244 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/browser/browser.py
+-rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/browser/browser_module.py
+-rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/browser/browser_name.py
+-rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/browser/browser_tab_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/browser/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/browser/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      567 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/browser/interfaces/browser_factory_interface.py
+-rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/browser/java_script.py
+-rw-rw-rw-   0        0        0     2128 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/browser/local_browser_factory.py
+-rw-rw-rw-   0        0        0     4731 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/browser/py_quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/configuration/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/configuration/browser_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/configuration/driver_settings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/configuration/driver_settings/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/configuration/driver_settings/base_driver_settings.py
+-rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/configuration/driver_settings/chrome_settings.py
+-rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/configuration/driver_settings/edge_settings.py
+-rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/configuration/driver_settings/firefox_settings.py
+-rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/configuration/driver_settings/iexplorer_settings.py
+-rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/configuration/timeout.py
+-rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/configuration/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/applications/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/applications/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/applications/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/applications/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/applications/interfaces/application_interface.py
+-rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/core/applications/quality_module.py
+-rw-rw-rw-   0        0        0     2255 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/core/applications/quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/configurations/configuration_module.py
+-rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/configurations/element_cache_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/configurations/interfaces/browser_profile_interface.py
+-rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/configurations/interfaces/retry_configuration_interface.py
+-rw-rw-rw-   0        0        0     1466 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/core/configurations/interfaces/timeout_configuration_interface.py
+-rw-rw-rw-   0        0        0      882 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/core/configurations/retry_configuration.py
+-rw-rw-rw-   0        0        0     1198 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/core/configurations/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/elements/actions/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/elements/actions/__init__.py
+-rw-rw-rw-   0        0        0     2809 2023-06-01 18:27:00.000000 PyWebUIFramework-0.2/src/core/elements/actions/js_actions.py
+-rw-rw-rw-   0        0        0    11790 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/base_element.py
+-rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/base_element_cache_handler.py
+-rw-rw-rw-   0        0        0     5701 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/base_element_factory.py
+-rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/base_parent_element.py
+-rw-rw-rw-   0        0        0      797 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/element_cache_handler.py
+-rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/element_factory.py
+-rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/element_finder.py
+-rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/element_finder_interface.py
+-rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/elements/highlight_state.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/elements/states/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/elements/states/__init__.py
+-rw-rw-rw-   0        0        0     4306 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/core/elements/states/base_element_state_provider.py
+-rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/core/elements/states/cached_element_state_provider.py
+-rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/core/elements/states/desired_state.py
+-rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/elements/states/element_count.py
+-rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/elements/states/element_state.py
+-rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/elements/states/element_state_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/localization/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/localization/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/configurations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/localization/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/configurations/interfaces/logger_configuration_interface.py
+-rw-rw-rw-   0        0        0      991 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/localization/configurations/logger_configuration.py
+-rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/core/localization/localization_module.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/localization/loggers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/localization/loggers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/loggers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/localization/loggers/interfaces/localized_logger_interface.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/localization/loggers/localized_logger.py
+-rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/loggers/logger_config.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/localization/managers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/managers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/localization/managers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/managers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/localization/managers/interfaces/localization_interface.py
+-rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/localization/managers/localization_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/utilities/action_repeater.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/utilities/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/utilities/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/utilities/interfaces/action_repeater_interface.py
+-rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/utilities/interfaces/settings_file_interface.py
+-rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/utilities/json_settings_file.py
+-rw-rw-rw-   0        0        0     1474 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/utilities/resource_file.py
+-rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/utilities/utilities_module.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/waitings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/waitings/__init__.py
+-rw-rw-rw-   0        0        0     5577 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/core/waitings/conditional_wait.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/core/waitings/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/waitings/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/core/waitings/interfaces/conditional_wait_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/elements/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/elements/attributes.py
+-rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/elements/button.py
+-rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/elements/check_box.py
+-rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/elements/checkable_element.py
+-rw-rw-rw-   0        0        0      295 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/elements/combo_box.py
+-rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-0.2/src/elements/element_factory.py
+-rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/elements/label.py
+-rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/elements/link.py
+-rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/elements/radio_button.py
+-rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/elements/text_box.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:42:58.000000 PyWebUIFramework-0.2/src/forms/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-0.2/src/forms/__init__.py
+-rw-rw-rw-   0        0        0     1174 2023-06-01 18:36:30.000000 PyWebUIFramework-0.2/src/forms/base_form.py
```

### Comparing `PyWebUIFramework-0.1/src/PyWebUIFramework.egg-info/SOURCES.txt` & `PyWebUIFramework-0.2/src/PyWebUIFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/browser/base_browser_factory.py` & `PyWebUIFramework-0.2/src/browser/base_browser_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC
 from injector import inject
 
-from src.browser.browser import Browser
-from src.browser.interfaces.browser_factory_interface import IBaseBrowserFactory
-from src.core.utilities.interfaces.action_repeater_interface import IActionRepeater
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.configurations.interfaces.browser_profile_interface import IBrowserProfile
-from src.core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
+from browser.browser import Browser
+from browser.interfaces.browser_factory_interface import IBaseBrowserFactory
+from core.utilities.interfaces.action_repeater_interface import IActionRepeater
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.configurations.interfaces.browser_profile_interface import IBrowserProfile
+from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
 from selenium.common.exceptions import SessionNotCreatedException, WebDriverException, TimeoutException
 
 
 class BaseBrowserFactory(IBaseBrowserFactory, ABC):
     """Abstract class BaseBrowserFactory that defines the required web driver."""
 
     @inject
```

### Comparing `PyWebUIFramework-0.1/src/browser/browser.py` & `PyWebUIFramework-0.2/src/browser/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typing as ty
 
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.common.exceptions import NoAlertPresentException
 from selenium.webdriver.remote.webdriver import WebDriver
-from src.core.applications.interfaces.application_interface import IApplication
-from src.core.configurations.interfaces.browser_profile_interface import IBrowserProfile
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
-from src.core.waitings.conditional_wait import ConditionalWait
-from src.browser.browser_tab_navigation import BrowserTabNavigation
-from src.browser.java_script import JavaScript
-from src.browser.alert_actions import AlertActions
+from core.applications.interfaces.application_interface import IApplication
+from core.configurations.interfaces.browser_profile_interface import IBrowserProfile
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
+from core.waitings.conditional_wait import ConditionalWait
+from browser.browser_tab_navigation import BrowserTabNavigation
+from browser.java_script import JavaScript
+from browser.alert_actions import AlertActions
 
 WD = ty.TypeVar('WD', bound=WebDriver)
 
 
 class Browser(IApplication):
     def __init__(self, driver: WD, localized_logger: ILocalizedLogger, browser_profile: IBrowserProfile,
                  timeouts: ITimeoutConfiguration) -> None:
```

### Comparing `PyWebUIFramework-0.1/src/browser/browser_module.py` & `PyWebUIFramework-0.2/src/browser/browser_module.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from injector import ClassProvider, singleton, InstanceProvider, Binder
 
-from src.core.applications.quality_module import QualityModule
-from src.core.configurations.interfaces.browser_profile_interface import IBrowserProfile
-from src.configuration.browser_profile import BrowserProfile
-from src.core.elements.base_element_factory import BaseElementFactory
-from src.core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
-from src.configuration.timeout_configuration import TimeoutConfiguration
-from src.elements.element_factory import ElementFactory
+from core.applications.quality_module import QualityModule
+from core.configurations.interfaces.browser_profile_interface import IBrowserProfile
+from configuration.browser_profile import BrowserProfile
+from core.elements.base_element_factory import BaseElementFactory
+from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
+from configuration.timeout_configuration import TimeoutConfiguration
+from elements.element_factory import ElementFactory
 
 
 class BrowserModule(QualityModule):
     """Class for register providers."""
 
     def configure(self, binder: Binder) -> None:
         """Bind interfaces to implementations.
```

### Comparing `PyWebUIFramework-0.1/src/browser/browser_tab_navigation.py` & `PyWebUIFramework-0.2/src/browser/browser_tab_navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as ty
 
-from src.browser.java_script import JavaScript
+from browser.java_script import JavaScript
 from selenium.webdriver.remote.webdriver import WebDriver
-from src.core.applications.interfaces.application_interface import IApplication
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.applications.interfaces.application_interface import IApplication
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
 
 B = ty.TypeVar('B', bound=IApplication)
 WD = ty.TypeVar('WD', bound=WebDriver)
 TAB = ty.TypeVar('TAB')
 
 
 class BrowserTabNavigation:
```

### Comparing `PyWebUIFramework-0.1/src/browser/interfaces/browser_factory_interface.py` & `PyWebUIFramework-0.2/src/browser/interfaces/browser_factory_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
-from src.browser.browser import Browser
+from browser.browser import Browser
 
 WD = ty.TypeVar('WD')
 
 
 class IBaseBrowserFactory(ABC):
     @abstractmethod
     def get_browser(self) -> Browser:
```

### Comparing `PyWebUIFramework-0.1/src/browser/java_script.py` & `PyWebUIFramework-0.2/src/browser/java_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from enum import Enum
 
-from src.core.utilities.resource_file import ResourceFile
+from core.utilities.resource_file import ResourceFile
 
 
 class JavaScript(Enum):
     IS_PAGE_LOADED = 'pageLoaded.js'
     CLICK_ELEMENT = 'clickElement.js'
     SET_VALUE = 'setValue.js'
     GET_ELEMENT_TEXT = 'getElementText.js.js'
```

### Comparing `PyWebUIFramework-0.1/src/browser/local_browser_factory.py` & `PyWebUIFramework-0.2/src/browser/local_browser_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from selenium.webdriver import Chrome, Firefox, Ie, Edge
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import IEDriverManager
 from webdriver_manager.microsoft import EdgeChromiumDriverManager
 from selenium.webdriver.remote.webdriver import WebDriver as RemoteWebDriver
-from src.browser.browser_name import BrowserName
-from src.browser.base_browser_factory import BaseBrowserFactory
+from browser.browser_name import BrowserName
+from browser.base_browser_factory import BaseBrowserFactory
 
 WD = ty.TypeVar('WD', bound=RemoteWebDriver)
 
 
 class LocalBaseBrowserFactory(BaseBrowserFactory):
     """Class that implements the BaseBrowserFactory interface."""
```

### Comparing `PyWebUIFramework-0.1/src/browser/py_quality_services.py` & `PyWebUIFramework-0.2/src/browser/py_quality_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typing as ty
 from threading import local
 
 from injector import Injector
-from src.browser.browser import Browser
-from src.browser.browser_module import BrowserModule
-from src.browser.base_browser_factory import BaseBrowserFactory
-from src.browser.local_browser_factory import LocalBaseBrowserFactory
-from src.configuration.browser_profile import BrowserProfile
-from src.core.applications.quality_services import QualityServices
-from src.core.waitings.conditional_wait import ConditionalWait
-from src.elements.element_factory import ElementFactory
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from browser.browser import Browser
+from browser.browser_module import BrowserModule
+from browser.base_browser_factory import BaseBrowserFactory
+from browser.local_browser_factory import LocalBaseBrowserFactory
+from configuration.browser_profile import BrowserProfile
+from core.applications.quality_services import QualityServices
+from core.waitings.conditional_wait import ConditionalWait
+from elements.element_factory import ElementFactory
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
 
 T = ty.TypeVar('T', bound=QualityServices)
 BF = ty.TypeVar('BF', bound=BaseBrowserFactory)
 
 LOCAL = local()
```

### Comparing `PyWebUIFramework-0.1/src/configuration/browser_profile.py` & `PyWebUIFramework-0.2/src/configuration/browser_profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from injector import inject
 
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.firefox.options import Options as FirefoxOptions
 from selenium.webdriver.ie.options import Options as IExplorerOptions
 from selenium.webdriver.edge.options import Options as EdgeOptions
 
-from src.browser.browser_name import BrowserName
-from src.configuration.driver_settings.base_driver_settings import BaseDriverSettings
-from src.configuration.driver_settings.chrome_settings import ChromeSettings
-from src.configuration.driver_settings.firefox_settings import FirefoxSettings
-from src.configuration.driver_settings.iexplorer_settings import IExplorerSettings
-from src.configuration.driver_settings.edge_settings import EdgeSettings
-from src.core.configurations.interfaces.browser_profile_interface import IBrowserProfile
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from browser.browser_name import BrowserName
+from configuration.driver_settings.base_driver_settings import BaseDriverSettings
+from configuration.driver_settings.chrome_settings import ChromeSettings
+from configuration.driver_settings.firefox_settings import FirefoxSettings
+from configuration.driver_settings.iexplorer_settings import IExplorerSettings
+from configuration.driver_settings.edge_settings import EdgeSettings
+from core.configurations.interfaces.browser_profile_interface import IBrowserProfile
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
 
 
 class BrowserProfile(IBrowserProfile):
     """Class responsible for basic browser settings."""
 
     @inject
     def __init__(self, settings_file: ISettingsFile, localization_logger: ILocalizedLogger) -> None:
```

### Comparing `PyWebUIFramework-0.1/src/configuration/driver_settings/base_driver_settings.py` & `PyWebUIFramework-0.2/src/configuration/driver_settings/base_driver_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import typing as ty
 from abc import ABC, abstractmethod
 
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
 
 OPT = ty.TypeVar('OPT')
 
 
 class BaseDriverSettings(ABC):
     def __init__(self, options: OPT, settings_file: ISettingsFile) -> None:
         self._options = options
```

### Comparing `PyWebUIFramework-0.1/src/configuration/driver_settings/chrome_settings.py` & `PyWebUIFramework-0.2/src/configuration/driver_settings/chrome_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.chrome.options import Options
-from src.configuration.driver_settings.base_driver_settings import BaseDriverSettings
+from configuration.driver_settings.base_driver_settings import BaseDriverSettings
 
 
 class ChromeSettings(BaseDriverSettings):
     def get_capabilities(self) -> Options:
         """Set and get options for driver.
         :return: Driver options.
         :rtype: Options.
```

### Comparing `PyWebUIFramework-0.1/src/configuration/driver_settings/edge_settings.py` & `PyWebUIFramework-0.2/src/configuration/driver_settings/edge_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.edge.options import Options
-from src.configuration.driver_settings.base_driver_settings import BaseDriverSettings
+from configuration.driver_settings.base_driver_settings import BaseDriverSettings
 
 
 class EdgeSettings(BaseDriverSettings):
     def get_capabilities(self) -> Options:
         """Set and get options for driver.
         :return: Driver options.
         :rtype: Options.
```

### Comparing `PyWebUIFramework-0.1/src/configuration/driver_settings/firefox_settings.py` & `PyWebUIFramework-0.2/src/configuration/driver_settings/firefox_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.firefox.options import Options
-from src.configuration.driver_settings.base_driver_settings import BaseDriverSettings
+from configuration.driver_settings.base_driver_settings import BaseDriverSettings
 
 
 class FirefoxSettings(BaseDriverSettings):
     def get_capabilities(self) -> Options:
         """Set and get options for driver.
         :return: Driver options.
         :rtype: Options.
```

### Comparing `PyWebUIFramework-0.1/src/configuration/driver_settings/iexplorer_settings.py` & `PyWebUIFramework-0.2/src/configuration/driver_settings/iexplorer_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.ie.options import Options
-from src.configuration.driver_settings.base_driver_settings import BaseDriverSettings
+from configuration.driver_settings.base_driver_settings import BaseDriverSettings
 
 
 class IExplorerSettings(BaseDriverSettings):
     def get_capabilities(self) -> Options:
         """Set and get options for driver.
         :return: Driver options.
         :rtype: Options.
```

### Comparing `PyWebUIFramework-0.1/src/configuration/timeout_configuration.py` & `PyWebUIFramework-0.2/src/configuration/timeout_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from injector import inject
-from src.configuration.timeout import Timeout
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.configurations.timeout_configuration import TimeoutConfigurationCore
+from configuration.timeout import Timeout
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.configurations.timeout_configuration import TimeoutConfigurationCore
 
 
 class TimeoutConfiguration(TimeoutConfigurationCore):
     """Class for settings timeouts."""
 
     @inject
     def __init__(self, settings_file: ISettingsFile) -> None:
```

### Comparing `PyWebUIFramework-0.1/src/core/applications/quality_module.py` & `PyWebUIFramework-0.2/src/core/applications/quality_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
 import typing as ty
 from injector import Module, ClassProvider, InstanceProvider, singleton, Binder
 
-from src.core.applications.interfaces.application_interface import IApplication
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.utilities.utilities_module import UtilitiesModule
-from src.core.waitings.interfaces.conditional_wait_interface import IConditionalWait
-from src.core.waitings.conditional_wait import ConditionalWait
-from src.core.configurations.element_cache_configuration import ElementCacheConfiguration
-from src.core.configurations.configuration_module import ConfigurationModule
-from src.core.configurations.interfaces.retry_configuration_interface import IRetryConfiguration
-from src.core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
-from src.core.localization.localization_module import LocalizationModule
-from src.core.localization.managers.interfaces.localization_interface import ILocalizationManager
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
-from src.core.localization.loggers.logger_config import Logger
-from src.core.utilities.interfaces.action_repeater_interface import IActionRepeater
-from src.core.utilities.action_repeater import ActionRepeater
-from src.core.elements.element_finder_interface import IElementFinder
-from src.core.elements.element_finder import ElementFinder
+from core.applications.interfaces.application_interface import IApplication
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.utilities.utilities_module import UtilitiesModule
+from core.waitings.interfaces.conditional_wait_interface import IConditionalWait
+from core.waitings.conditional_wait import ConditionalWait
+from core.configurations.element_cache_configuration import ElementCacheConfiguration
+from core.configurations.configuration_module import ConfigurationModule
+from core.configurations.interfaces.retry_configuration_interface import IRetryConfiguration
+from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
+from core.localization.localization_module import LocalizationModule
+from core.localization.managers.interfaces.localization_interface import ILocalizationManager
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
+from core.localization.loggers.logger_config import Logger
+from core.utilities.interfaces.action_repeater_interface import IActionRepeater
+from core.utilities.action_repeater import ActionRepeater
+from core.elements.element_finder_interface import IElementFinder
+from core.elements.element_finder import ElementFinder
 
 
 class QualityModule(Module):
     """Default class for register providers."""
 
     def __init__(self, application_provider: ty.Callable[..., IApplication]):
         """Initial link for binding."""
```

### Comparing `PyWebUIFramework-0.1/src/core/applications/quality_services.py` & `PyWebUIFramework-0.2/src/core/applications/quality_services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as ty
 
 from injector import Injector
-from src.core.applications.interfaces.application_interface import IApplication
-from src.core.applications.quality_module import QualityModule
+from core.applications.interfaces.application_interface import IApplication
+from core.applications.quality_module import QualityModule
 
 WD = ty.TypeVar('WD')
 
 
 class QualityServices(IApplication):
     __app = None
     __injector = None
```

### Comparing `PyWebUIFramework-0.1/src/core/configurations/configuration_module.py` & `PyWebUIFramework-0.2/src/core/configurations/configuration_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as ty
 
-from src.core.configurations.element_cache_configuration import ElementCacheConfiguration
-from src.core.localization.configurations.logger_configuration import LoggerConfiguration
-from src.core.configurations.retry_configuration import RetryConfiguration
-from src.core.configurations.timeout_configuration import TimeoutConfigurationCore
+from core.configurations.element_cache_configuration import ElementCacheConfiguration
+from core.localization.configurations.logger_configuration import LoggerConfiguration
+from core.configurations.retry_configuration import RetryConfiguration
+from core.configurations.timeout_configuration import TimeoutConfigurationCore
 
 
 class ConfigurationModule:
     @staticmethod
     def get_element_cache_configuration() -> ty.Type[ElementCacheConfiguration]:
         """Get element cache configuration class for further injection.
         :return: ElementCacheConfiguration class.
```

### Comparing `PyWebUIFramework-0.1/src/core/configurations/element_cache_configuration.py` & `PyWebUIFramework-0.2/src/core/configurations/element_cache_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from injector import inject
 
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
 
 
 class ElementCacheConfiguration:
     __IS_ENABLED_PATH = "elementCache.isEnabled"
 
     @inject
     def __init__(self, settings_file: ISettingsFile) -> None:
```

### Comparing `PyWebUIFramework-0.1/src/core/configurations/interfaces/browser_profile_interface.py` & `PyWebUIFramework-0.2/src/core/configurations/interfaces/browser_profile_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
-from src.configuration.driver_settings.base_driver_settings import BaseDriverSettings
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
+from configuration.driver_settings.base_driver_settings import BaseDriverSettings
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
 
 DS = ty.TypeVar('DS', bound=BaseDriverSettings)
 
 
 class IBrowserProfile(ABC):
     """Abstract class responsible for basic browser settings."""
     _driver_settings = None
```

### Comparing `PyWebUIFramework-0.1/src/core/configurations/interfaces/retry_configuration_interface.py` & `PyWebUIFramework-0.2/src/core/configurations/interfaces/retry_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/core/configurations/interfaces/timeout_configuration_interface.py` & `PyWebUIFramework-0.2/src/core/configurations/interfaces/timeout_configuration_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
 
 
 class ITimeoutConfiguration(ABC):
     """Abstraction for timeout configuration."""
     _settings_file: ISettingsFile = NotImplemented
 
     def _get_config_value(self, key: str) -> int:
```

### Comparing `PyWebUIFramework-0.1/src/core/configurations/retry_configuration.py` & `PyWebUIFramework-0.2/src/core/configurations/retry_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from injector import inject
 
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.configurations.interfaces.retry_configuration_interface import IRetryConfiguration
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.configurations.interfaces.retry_configuration_interface import IRetryConfiguration
 
 
 class RetryConfiguration(IRetryConfiguration):
     @inject
     def __init__(self, settings_file: ISettingsFile):
         self._settings_file = settings_file
```

### Comparing `PyWebUIFramework-0.1/src/core/configurations/timeout_configuration.py` & `PyWebUIFramework-0.2/src/core/configurations/timeout_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from injector import inject
 
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
 
 
 class TimeoutConfigurationCore(ITimeoutConfiguration):
     """Core class for setting timeouts."""
     
     @inject
     def __init__(self, settings_file: ISettingsFile):
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/actions/js_actions.py` & `PyWebUIFramework-0.2/src/core/elements/actions/js_actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing as ty
 
-from src.browser.browser import Browser
-from src.browser.java_script import JavaScript
-from src.core.elements.highlight_state import HighlightState
-from src.core.utilities.interfaces.action_repeater_interface import IActionRepeater
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.elements.states.element_state import Displayed, ExistsInAnyState
-from src.core.elements.base_parent_element import BaseParentElement
+from browser.browser import Browser
+from browser.java_script import JavaScript
+from core.elements.highlight_state import HighlightState
+from core.utilities.interfaces.action_repeater_interface import IActionRepeater
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.elements.states.element_state import Displayed, ExistsInAnyState
+from core.elements.base_parent_element import BaseParentElement
 
 T = ty.TypeVar('T')
 
 
 class JsActions:
     def __init__(self, element: BaseParentElement, element_type: ty.Type[ty.Union[Displayed, ExistsInAnyState]],
                  localized_logger: ILocalizedLogger, action_repeater: IActionRepeater, browser: Browser):
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/base_element.py` & `PyWebUIFramework-0.2/src/core/elements/base_element.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
 from selenium.common.exceptions import NoSuchElementException, WebDriverException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.states.element_count import ElementCount
-from src.core.elements.states.element_state import Displayed, ExistsInAnyState
-from src.core.elements.base_parent_element import BaseParentElement
-from src.core.configurations.element_cache_configuration import ElementCacheConfiguration
-from src.core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
-from src.core.localization.managers.interfaces.localization_interface import ILocalizationManager
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.elements.element_finder_interface import IElementFinder
-from src.core.localization.loggers.logger_config import Logger
-from src.core.elements.states.element_state_provider import ElementStateProvider
-from src.core.waitings.interfaces.conditional_wait_interface import IConditionalWait
-from src.core.elements.base_element_factory import BaseElementFactory
-from src.core.applications.interfaces.application_interface import IApplication
-from src.core.utilities.interfaces.action_repeater_interface import IActionRepeater
-from src.core.elements.base_element_cache_handler import BaseElementCacheHandler
-from src.core.elements.element_cache_handler import ElementCacheHandler
-from src.core.elements.states.cached_element_state_provider import CachedElementStateProvider
-from src.core.elements.actions.js_actions import JsActions
+from core.elements.states.element_count import ElementCount
+from core.elements.states.element_state import Displayed, ExistsInAnyState
+from core.elements.base_parent_element import BaseParentElement
+from core.configurations.element_cache_configuration import ElementCacheConfiguration
+from core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
+from core.localization.managers.interfaces.localization_interface import ILocalizationManager
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.elements.element_finder_interface import IElementFinder
+from core.localization.loggers.logger_config import Logger
+from core.elements.states.element_state_provider import ElementStateProvider
+from core.waitings.interfaces.conditional_wait_interface import IConditionalWait
+from core.elements.base_element_factory import BaseElementFactory
+from core.applications.interfaces.application_interface import IApplication
+from core.utilities.interfaces.action_repeater_interface import IActionRepeater
+from core.elements.base_element_cache_handler import BaseElementCacheHandler
+from core.elements.element_cache_handler import ElementCacheHandler
+from core.elements.states.cached_element_state_provider import CachedElementStateProvider
+from core.elements.actions.js_actions import JsActions
 
 T = ty.TypeVar('T')
 TR = ty.TypeVar('TR')
 APP = ty.TypeVar('APP', bound=IApplication)
 
 
 class BaseElement(BaseParentElement, ABC):
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/base_element_cache_handler.py` & `PyWebUIFramework-0.2/src/core/elements/base_element_cache_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.states.element_state import Displayed, ExistsInAnyState
-from src.core.elements.element_finder_interface import IElementFinder
+from core.elements.states.element_state import Displayed, ExistsInAnyState
+from core.elements.element_finder_interface import IElementFinder
 
 
 class BaseElementCacheHandler(ABC):
     """Allows to use cached element."""
 
     def __init__(self, locator: ty.Tuple[By, str], state: ty.Type[ty.Union[Displayed, ExistsInAnyState]],
                  finder: IElementFinder):
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/base_element_factory.py` & `PyWebUIFramework-0.2/src/core/elements/base_element_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
 from injector import inject
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.states.element_state import Displayed
-from src.core.elements.states.element_count import ElementCount
-from src.core.elements.element_finder_interface import IElementFinder
-from src.core.waitings.interfaces.conditional_wait_interface import IConditionalWait
-from src.core.localization.managers.interfaces.localization_interface import ILocalizationManager
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.applications.interfaces.application_interface import IApplication
-from src.core.utilities.interfaces.action_repeater_interface import IActionRepeater
-from src.core.configurations.element_cache_configuration import ElementCacheConfiguration
+from core.elements.states.element_state import Displayed
+from core.elements.states.element_count import ElementCount
+from core.elements.element_finder_interface import IElementFinder
+from core.waitings.interfaces.conditional_wait_interface import IConditionalWait
+from core.localization.managers.interfaces.localization_interface import ILocalizationManager
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.applications.interfaces.application_interface import IApplication
+from core.utilities.interfaces.action_repeater_interface import IActionRepeater
+from core.configurations.element_cache_configuration import ElementCacheConfiguration
 
 T = ty.TypeVar('T')
 
 
 class BaseElementFactory(ABC):
     @inject
     def __init__(self, conditional_wait: IConditionalWait, element_finder: IElementFinder,
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/base_parent_element.py` & `PyWebUIFramework-0.2/src/core/elements/base_parent_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.states.element_state import Displayed
-from src.core.elements.states.element_count import ElementCount
+from core.elements.states.element_state import Displayed
+from core.elements.states.element_count import ElementCount
 
 T = ty.TypeVar('T')
 
 
 class BaseParentElement(ABC):
     @property
     @abstractmethod
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/element_cache_handler.py` & `PyWebUIFramework-0.2/src/core/elements/element_cache_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as ty
 
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.base_element_cache_handler import BaseElementCacheHandler
+from core.elements.base_element_cache_handler import BaseElementCacheHandler
 
 
 class ElementCacheHandler(BaseElementCacheHandler):
     def get_element(self, timeout: int = 0, custom_state: ty.Callable[[WebElement], bool] = None) -> WebElement:
         """
         Allow to get cached element.
         :param timeout: Timeout used to retrieve the element when refresh is needed.
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/element_factory.py` & `PyWebUIFramework-0.2/src/core/elements/element_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as ty
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.base_element_factory import BaseElementFactory
-from src.core.elements.states.element_state import Displayed
-from src.core.elements.states.element_count import ElementCount
-from src.core.elements.base_parent_element import BaseParentElement
+from core.elements.base_element_factory import BaseElementFactory
+from core.elements.states.element_state import Displayed
+from core.elements.states.element_count import ElementCount
+from core.elements.base_parent_element import BaseParentElement
 
 T = ty.TypeVar('T')
 
 
 class ElementFactory(BaseElementFactory):
     """Factory that creates elements."""
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/element_finder.py` & `PyWebUIFramework-0.2/src/core/elements/element_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as ty
 
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import TimeoutException, NoSuchElementException
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.states.element_state import ExistsInAnyState, Displayed
-from src.core.elements.states.desired_state import DesiredState
-from src.core.elements.element_finder_interface import IElementFinder
+from core.elements.states.element_state import ExistsInAnyState, Displayed
+from core.elements.states.desired_state import DesiredState
+from core.elements.element_finder_interface import IElementFinder
 
 
 class ElementFinder(IElementFinder):
     def find_element(self, locator: ty.Tuple[By, str],
                      state: ty.Type[ty.Union[Displayed, ExistsInAnyState]] = ExistsInAnyState(),
                      timeout: int = 0) -> WebElement:
         """
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/element_finder_interface.py` & `PyWebUIFramework-0.2/src/core/elements/element_finder_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
 from injector import inject
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.states.element_state import ExistsInAnyState, Displayed
-from src.core.elements.states.desired_state import DesiredState
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.waitings.conditional_wait import ConditionalWait
+from core.elements.states.element_state import ExistsInAnyState, Displayed
+from core.elements.states.desired_state import DesiredState
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.waitings.conditional_wait import ConditionalWait
 
 
 class IElementFinder(ABC):
     @inject
     def __init__(self, logger: ILocalizedLogger, conditional_wait: ConditionalWait):
         """Initialize finder with required dependencies."""
         self._logger = logger
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/states/base_element_state_provider.py` & `PyWebUIFramework-0.2/src/core/elements/states/base_element_state_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
 from selenium.webdriver.common.by import By
-from src.core.elements.element_finder_interface import IElementFinder
-from src.core.waitings.interfaces.conditional_wait_interface import IConditionalWait
+from core.elements.element_finder_interface import IElementFinder
+from core.waitings.interfaces.conditional_wait_interface import IConditionalWait
 
 
 class BaseElementStateProvider(ABC):
     def __init__(self, element_locator: ty.Tuple[By, str], conditional_wait: IConditionalWait,
                  element_finder: IElementFinder):
         """Initialize provider with required dependencies."""
         self._element_locator = element_locator
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/states/cached_element_state_provider.py` & `PyWebUIFramework-0.2/src/core/elements/states/cached_element_state_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing as ty
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.common.exceptions import StaleElementReferenceException, NoSuchElementException
-from src.core.elements.element_finder_interface import IElementFinder
-from src.core.elements.states.element_state import ExistsInAnyState
-from src.core.waitings.interfaces.conditional_wait_interface import IConditionalWait
-from src.core.elements.base_element_cache_handler import BaseElementCacheHandler
-from src.core.elements.states.base_element_state_provider import BaseElementStateProvider
+from core.elements.element_finder_interface import IElementFinder
+from core.elements.states.element_state import ExistsInAnyState
+from core.waitings.interfaces.conditional_wait_interface import IConditionalWait
+from core.elements.base_element_cache_handler import BaseElementCacheHandler
+from core.elements.states.base_element_state_provider import BaseElementStateProvider
 
 
 class CachedElementStateProvider(BaseElementStateProvider):
     def __init__(self, element_locator: ty.Tuple[By, str], conditional_wait: IConditionalWait,
                  element_finder: IElementFinder, element_cache_handler: BaseElementCacheHandler):
         super(CachedElementStateProvider, self).__init__(element_locator, conditional_wait, element_finder)
         self.__element_cache_handler = element_cache_handler
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/states/desired_state.py` & `PyWebUIFramework-0.2/src/core/elements/states/desired_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as ty
 
-from src.core.elements.states.element_state import ExistsInAnyState, Displayed
+from core.elements.states.element_state import ExistsInAnyState, Displayed
 
 
 class DesiredState:
     def __init__(self, element_state_condition: ty.Type[ty.Union[Displayed, ExistsInAnyState]], state_name: str,
                  except_timeout_exception: bool = False, raise_no_such_element_exception: bool = False):
         self.__element_state_condition = element_state_condition
         self.__except_timeout_exception = except_timeout_exception
```

### Comparing `PyWebUIFramework-0.1/src/core/elements/states/element_state.py` & `PyWebUIFramework-0.2/src/core/elements/states/element_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/core/elements/states/element_state_provider.py` & `PyWebUIFramework-0.2/src/core/elements/states/element_state_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as ty
 
 from selenium.webdriver.remote.webelement import WebElement
-from src.core.elements.states.desired_state import DesiredState
-from src.core.elements.states.element_state import Displayed, ExistsInAnyState
-from src.core.elements.states.base_element_state_provider import BaseElementStateProvider
+from core.elements.states.desired_state import DesiredState
+from core.elements.states.element_state import Displayed, ExistsInAnyState
+from core.elements.states.base_element_state_provider import BaseElementStateProvider
 
 
 class ElementStateProvider(BaseElementStateProvider):
     @property
     def is_clickable(self) -> bool:
         return self.__is_element_clickable(0, True)
```

### Comparing `PyWebUIFramework-0.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py` & `PyWebUIFramework-0.2/src/core/localization/configurations/interfaces/logger_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/core/localization/configurations/logger_configuration.py` & `PyWebUIFramework-0.2/src/core/localization/configurations/logger_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from injector import inject
 
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
 
 
 class LoggerConfiguration(ILoggerConfiguration):
     """Implementation for ILoggerConfiguration."""
 
     @inject
     def __init__(self, settings_file: ISettingsFile):
```

### Comparing `PyWebUIFramework-0.1/src/core/localization/loggers/interfaces/localized_logger_interface.py` & `PyWebUIFramework-0.2/src/core/localization/loggers/interfaces/localized_logger_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as ty
 from abc import ABC, abstractmethod
 
-from src.core.elements.states.element_state import Displayed, ExistsInAnyState
-from src.core.localization.managers.interfaces.localization_interface import ILocalizationManager
-from src.core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
+from core.elements.states.element_state import Displayed, ExistsInAnyState
+from core.localization.managers.interfaces.localization_interface import ILocalizationManager
+from core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
 
 
 class ILocalizedLogger(ABC):
     """Log messages in current language."""
     _localization_manager: ILocalizationManager = NotImplemented
     _configuration: ILoggerConfiguration = NotImplemented
```

### Comparing `PyWebUIFramework-0.1/src/core/localization/loggers/localized_logger.py` & `PyWebUIFramework-0.2/src/core/localization/loggers/localized_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from injector import inject
 from logging import Logger
 
-from src.core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
-from src.core.localization.managers.interfaces.localization_interface import ILocalizationManager
-from src.core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
+from core.localization.loggers.interfaces.localized_logger_interface import ILocalizedLogger
+from core.localization.managers.interfaces.localization_interface import ILocalizationManager
+from core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
 
 
 class LocalizationLogger(ILocalizedLogger):
     @inject
     def __init__(self, localization_manager: ILocalizationManager, logger: Logger,
                  configuration: ILoggerConfiguration) -> None:
         """Initialize with localization manager and logger."""
```

### Comparing `PyWebUIFramework-0.1/src/core/localization/managers/localization_manager.py` & `PyWebUIFramework-0.2/src/core/localization/managers/localization_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from itertools import chain
 from logging import Logger
 from injector import inject
 
-from src.core.localization.managers.interfaces.localization_interface import ILocalizationManager
-from src.core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.utilities.json_settings_file import JsonSettingsFile
-from src.core.utilities.resource_file import ResourceFile
+from core.localization.managers.interfaces.localization_interface import ILocalizationManager
+from core.localization.configurations.interfaces.logger_configuration_interface import ILoggerConfiguration
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.utilities.json_settings_file import JsonSettingsFile
+from core.utilities.resource_file import ResourceFile
 
 
 class LocalizationManager(ILocalizationManager):
     """This class is used for translation messages."""
     __resource_template = 'localization/%s'
 
     @inject
```

### Comparing `PyWebUIFramework-0.1/src/core/utilities/action_repeater.py` & `PyWebUIFramework-0.2/src/core/utilities/action_repeater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import typing as ty
 from injector import inject
 
-from src.core.utilities.interfaces.action_repeater_interface import IActionRepeater
-from src.core.configurations.interfaces.retry_configuration_interface import IRetryConfiguration
+from core.utilities.interfaces.action_repeater_interface import IActionRepeater
+from core.configurations.interfaces.retry_configuration_interface import IRetryConfiguration
 
 T = ty.TypeVar('T')
 
 
 class ActionRepeater(IActionRepeater):
     @inject
     def __init__(self, retry_configuration: IRetryConfiguration):
```

### Comparing `PyWebUIFramework-0.1/src/core/utilities/interfaces/action_repeater_interface.py` & `PyWebUIFramework-0.2/src/core/utilities/interfaces/action_repeater_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/core/utilities/interfaces/settings_file_interface.py` & `PyWebUIFramework-0.2/src/core/utilities/interfaces/settings_file_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/core/utilities/json_settings_file.py` & `PyWebUIFramework-0.2/src/core/utilities/json_settings_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import json
 from loguru import logger
 import typing as ty
 
 from jsonpath_ng import DatumInContext
 from jsonpath_ng import parse
 
-from src.core.utilities.interfaces.settings_file_interface import ISettingsFile
-from src.core.utilities.resource_file import ResourceFile
+from core.utilities.interfaces.settings_file_interface import ISettingsFile
+from core.utilities.resource_file import ResourceFile
 
 
 class JsonSettingsFile(ISettingsFile):
     """Class which defines work with .json settings file."""
 
     def __init__(self, resource_name: str, root_dir: str = None):
         self.__resource_file = ResourceFile(resource_name, root_dir)
```

### Comparing `PyWebUIFramework-0.1/src/core/utilities/resource_file.py` & `PyWebUIFramework-0.2/src/core/utilities/resource_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/core/waitings/conditional_wait.py` & `PyWebUIFramework-0.2/src/core/waitings/conditional_wait.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import time
 import typing as ty
 from injector import inject
 
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.common.exceptions import StaleElementReferenceException
-from src.core.waitings.interfaces.conditional_wait_interface import IConditionalWait
-from src.core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
-from src.core.applications.interfaces.application_interface import IApplication
+from core.waitings.interfaces.conditional_wait_interface import IConditionalWait
+from core.configurations.interfaces.timeout_configuration_interface import ITimeoutConfiguration
+from core.applications.interfaces.application_interface import IApplication
 
 T = ty.TypeVar('T')
 
 
 class ConditionalWait(IConditionalWait):
 
     @inject
```

### Comparing `PyWebUIFramework-0.1/src/core/waitings/interfaces/conditional_wait_interface.py` & `PyWebUIFramework-0.2/src/core/waitings/interfaces/conditional_wait_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-0.1/src/elements/check_box.py` & `PyWebUIFramework-0.2/src/elements/check_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.elements.checkable_element import CheckableElement
+from elements.checkable_element import CheckableElement
 
 
 class CheckBox(CheckableElement):
     @property
     def _element_type(self) -> str:
         return self._localization_manager.get_localized_message('loc.checkbox')
```

### Comparing `PyWebUIFramework-0.1/src/elements/element_factory.py` & `PyWebUIFramework-0.2/src/elements/element_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import typing as ty
 
 from selenium.webdriver.common.by import By
-from src.core.elements.element_factory import ElementFactory as ElementFactoryCore
-from src.core.elements.states.element_state import Displayed
-from src.elements.button import Button
-from src.elements.link import Link
-from src.elements.label import Label
-from src.elements.check_box import CheckBox
-from src.elements.combo_box import ComboBox
-from src.elements.text_box import TextBox
-from src.elements.radio_button import RadioButton
-
+from core.elements.element_factory import ElementFactory as ElementFactoryCore
+from core.elements.states.element_state import Displayed
+from elements.button import Button
+from elements.link import Link
+from elements.label import Label
+from elements.check_box import CheckBox
+from elements.combo_box import ComboBox
+from elements.text_box import TextBox
+from elements.radio_button import RadioButton
 
 
 class ElementFactory(ElementFactoryCore):
     def get_button(self, locator: ty.Tuple[By, str], name: str, element_state=Displayed()) -> Button:
         return Button(locator, name, element_state, self)
 
     def get_radio_button(self, locator: ty.Tuple[By, str], name: str, element_state=Displayed()) -> RadioButton:
```

### Comparing `PyWebUIFramework-0.1/src/elements/text_box.py` & `PyWebUIFramework-0.2/src/elements/text_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.core.elements.base_element import BaseElement
-from src.elements.attributes import Attributes
+from core.elements.base_element import BaseElement
+from elements.attributes import Attributes
 from selenium.webdriver.common.keys import Keys
 
 
 class TextBox(BaseElement):
     __LOG_TYPING = "loc.text.typing"
     __LOG_CLEARING = "loc.text.clearing"
```

### Comparing `PyWebUIFramework-0.1/src/forms/base_form.py` & `PyWebUIFramework-0.2/src/forms/base_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as ty
 from abc import ABC
 
 from selenium.webdriver.common.by import By
-from src.browser.py_quality_services import PyQualityServices
+from browser.py_quality_services import PyQualityServices
 
 
 class BaseForm(ABC):
     def __init__(self, locator: ty.Tuple[By, str], name: str):
         self._locator = locator
         self._name = name
```

