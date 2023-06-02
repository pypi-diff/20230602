# Comparing `tmp/PyWebUIFramework-1.0.tar.gz` & `tmp/PyWebUIFramework-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyWebUIFramework-1.0.tar", last modified: Fri Jun  2 17:58:07 2023, max compression
+gzip compressed data, was "dist\PyWebUIFramework-1.1.tar", last modified: Fri Jun  2 18:06:46 2023, max compression
```

## Comparing `PyWebUIFramework-1.0.tar` & `PyWebUIFramework-1.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/
--rw-rw-rw-   0        0        0      281 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-01 17:52:31.000000 PyWebUIFramework-1.0/README.md
--rw-rw-rw-   0        0        0      115 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-06-02 17:58:00.000000 PyWebUIFramework-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/PyWebUIFramework.egg-info/
--rw-rw-rw-   0        0        0      281 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/PyWebUIFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4282 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/PyWebUIFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/PyWebUIFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/PyWebUIFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/PyWebUIFramework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/browser/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/browser/__init__.py
--rw-rw-rw-   0        0        0      144 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/browser/alert_actions.py
--rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/browser/base_browser_factory.py
--rw-rw-rw-   0        0        0     8244 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/browser/browser.py
--rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/browser/browser_module.py
--rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/browser/browser_name.py
--rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/browser/browser_tab_navigation.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/browser/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/browser/interfaces/__init__.py
--rw-rw-rw-   0        0        0      567 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/browser/interfaces/browser_factory_interface.py
--rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/browser/java_script.py
--rw-rw-rw-   0        0        0     2128 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/browser/local_browser_factory.py
--rw-rw-rw-   0        0        0     4731 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/browser/py_quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/configuration/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/configuration/__init__.py
--rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/configuration/browser_profile.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/configuration/driver_settings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/configuration/driver_settings/__init__.py
--rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/configuration/driver_settings/base_driver_settings.py
--rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/configuration/driver_settings/chrome_settings.py
--rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/configuration/driver_settings/edge_settings.py
--rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/configuration/driver_settings/firefox_settings.py
--rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/configuration/driver_settings/iexplorer_settings.py
--rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/configuration/timeout.py
--rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/configuration/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/applications/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/applications/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/applications/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/applications/interfaces/__init__.py
--rw-rw-rw-   0        0        0      331 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/applications/interfaces/application_interface.py
--rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/core/applications/quality_module.py
--rw-rw-rw-   0        0        0     2255 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/core/applications/quality_services.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/configurations/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/configurations/configuration_module.py
--rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/configurations/element_cache_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/configurations/interfaces/browser_profile_interface.py
--rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/configurations/interfaces/retry_configuration_interface.py
--rw-rw-rw-   0        0        0     1466 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/core/configurations/interfaces/timeout_configuration_interface.py
--rw-rw-rw-   0        0        0      882 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/core/configurations/retry_configuration.py
--rw-rw-rw-   0        0        0     1198 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/core/configurations/timeout_configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/elements/actions/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/elements/actions/__init__.py
--rw-rw-rw-   0        0        0     2809 2023-06-01 18:27:00.000000 PyWebUIFramework-1.0/src/core/elements/actions/js_actions.py
--rw-rw-rw-   0        0        0    11790 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/base_element.py
--rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/base_element_cache_handler.py
--rw-rw-rw-   0        0        0     5701 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/base_element_factory.py
--rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/base_parent_element.py
--rw-rw-rw-   0        0        0      797 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/element_cache_handler.py
--rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/element_factory.py
--rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/element_finder.py
--rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/element_finder_interface.py
--rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/elements/highlight_state.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/elements/states/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/elements/states/__init__.py
--rw-rw-rw-   0        0        0     4306 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/core/elements/states/base_element_state_provider.py
--rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/core/elements/states/cached_element_state_provider.py
--rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/core/elements/states/desired_state.py
--rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/elements/states/element_count.py
--rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/elements/states/element_state.py
--rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/elements/states/element_state_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/localization/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/localization/configurations/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/configurations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/localization/configurations/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/configurations/interfaces/__init__.py
--rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/configurations/interfaces/logger_configuration_interface.py
--rw-rw-rw-   0        0        0      991 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/localization/configurations/logger_configuration.py
--rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/core/localization/localization_module.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/localization/loggers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/localization/loggers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/loggers/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/localization/loggers/interfaces/localized_logger_interface.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/localization/loggers/localized_logger.py
--rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/loggers/logger_config.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/localization/managers/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/managers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/localization/managers/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/managers/interfaces/__init__.py
--rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/localization/managers/interfaces/localization_interface.py
--rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/localization/managers/localization_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/utilities/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/utilities/action_repeater.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/utilities/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/utilities/interfaces/__init__.py
--rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/utilities/interfaces/action_repeater_interface.py
--rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/utilities/interfaces/settings_file_interface.py
--rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/utilities/json_settings_file.py
--rw-rw-rw-   0        0        0     3034 2023-06-02 17:00:05.000000 PyWebUIFramework-1.0/src/core/utilities/resource_file.py
--rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/utilities/utilities_module.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/waitings/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/waitings/__init__.py
--rw-rw-rw-   0        0        0     5577 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/core/waitings/conditional_wait.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/core/waitings/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/waitings/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/core/waitings/interfaces/conditional_wait_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/elements/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/elements/__init__.py
--rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/elements/attributes.py
--rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/elements/button.py
--rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/elements/check_box.py
--rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/elements/checkable_element.py
--rw-rw-rw-   0        0        0      295 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/elements/combo_box.py
--rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-1.0/src/elements/element_factory.py
--rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/elements/label.py
--rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/elements/link.py
--rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/elements/radio_button.py
--rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/elements/text_box.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:07.000000 PyWebUIFramework-1.0/src/forms/
--rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.0/src/forms/__init__.py
--rw-rw-rw-   0        0        0     1174 2023-06-01 18:36:30.000000 PyWebUIFramework-1.0/src/forms/base_form.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/
+-rw-rw-rw-   0        0        0      281 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-01 17:52:31.000000 PyWebUIFramework-1.1/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1302 2023-06-02 18:06:44.000000 PyWebUIFramework-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/PyWebUIFramework.egg-info/
+-rw-rw-rw-   0        0        0      281 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/PyWebUIFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/PyWebUIFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/PyWebUIFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/PyWebUIFramework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/PyWebUIFramework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/browser/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/browser/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/browser/alert_actions.py
+-rw-rw-rw-   0        0        0     2152 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/browser/base_browser_factory.py
+-rw-rw-rw-   0        0        0     8244 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/browser/browser.py
+-rw-rw-rw-   0        0        0     1123 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/browser/browser_module.py
+-rw-rw-rw-   0        0        0      200 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/browser/browser_name.py
+-rw-rw-rw-   0        0        0     3121 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/browser/browser_tab_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/browser/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/browser/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      567 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/browser/interfaces/browser_factory_interface.py
+-rw-rw-rw-   0        0        0      778 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/browser/java_script.py
+-rw-rw-rw-   0        0        0     2128 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/browser/local_browser_factory.py
+-rw-rw-rw-   0        0        0     4731 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/browser/py_quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/configuration/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/configuration/browser_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/configuration/driver_settings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/configuration/driver_settings/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/configuration/driver_settings/base_driver_settings.py
+-rw-rw-rw-   0        0        0      968 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/configuration/driver_settings/chrome_settings.py
+-rw-rw-rw-   0        0        0     1022 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/configuration/driver_settings/edge_settings.py
+-rw-rw-rw-   0        0        0     1032 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/configuration/driver_settings/firefox_settings.py
+-rw-rw-rw-   0        0        0      736 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/configuration/driver_settings/iexplorer_settings.py
+-rw-rw-rw-   0        0        0      142 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/configuration/timeout.py
+-rw-rw-rw-   0        0        0     1388 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/configuration/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/applications/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/applications/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/applications/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/applications/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/applications/interfaces/application_interface.py
+-rw-rw-rw-   0        0        0     3301 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/core/applications/quality_module.py
+-rw-rw-rw-   0        0        0     2255 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/core/applications/quality_services.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/configurations/configuration_module.py
+-rw-rw-rw-   0        0        0      526 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/configurations/element_cache_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1681 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/configurations/interfaces/browser_profile_interface.py
+-rw-rw-rw-   0        0        0      549 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/configurations/interfaces/retry_configuration_interface.py
+-rw-rw-rw-   0        0        0     1466 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/core/configurations/interfaces/timeout_configuration_interface.py
+-rw-rw-rw-   0        0        0      882 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/core/configurations/retry_configuration.py
+-rw-rw-rw-   0        0        0     1198 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/core/configurations/timeout_configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/elements/actions/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/elements/actions/__init__.py
+-rw-rw-rw-   0        0        0     2809 2023-06-01 18:27:00.000000 PyWebUIFramework-1.1/src/core/elements/actions/js_actions.py
+-rw-rw-rw-   0        0        0    11790 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/base_element.py
+-rw-rw-rw-   0        0        0     1866 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/base_element_cache_handler.py
+-rw-rw-rw-   0        0        0     5701 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/base_element_factory.py
+-rw-rw-rw-   0        0        0     2566 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/base_parent_element.py
+-rw-rw-rw-   0        0        0      797 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/element_cache_handler.py
+-rw-rw-rw-   0        0        0     8552 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/element_factory.py
+-rw-rw-rw-   0        0        0     3985 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/element_finder.py
+-rw-rw-rw-   0        0        0     2504 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/element_finder_interface.py
+-rw-rw-rw-   0        0        0      147 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/elements/highlight_state.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/elements/states/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/elements/states/__init__.py
+-rw-rw-rw-   0        0        0     4306 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/core/elements/states/base_element_state_provider.py
+-rw-rw-rw-   0        0        0     6787 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/core/elements/states/cached_element_state_provider.py
+-rw-rw-rw-   0        0        0     1008 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/core/elements/states/desired_state.py
+-rw-rw-rw-   0        0        0      105 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/elements/states/element_count.py
+-rw-rw-rw-   0        0        0      614 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/elements/states/element_state.py
+-rw-rw-rw-   0        0        0     2720 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/elements/states/element_state_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/localization/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/localization/configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/configurations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/localization/configurations/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/configurations/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py
+-rw-rw-rw-   0        0        0      991 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/localization/configurations/logger_configuration.py
+-rw-rw-rw-   0        0        0      921 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/core/localization/localization_module.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/localization/loggers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/localization/loggers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/loggers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3696 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/localization/loggers/interfaces/localized_logger_interface.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/localization/loggers/localized_logger.py
+-rw-rw-rw-   0        0        0      332 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/loggers/logger_config.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/localization/managers/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/managers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/localization/managers/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/managers/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/localization/managers/interfaces/localization_interface.py
+-rw-rw-rw-   0        0        0     2258 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/localization/managers/localization_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/utilities/action_repeater.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/utilities/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/utilities/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/utilities/interfaces/action_repeater_interface.py
+-rw-rw-rw-   0        0        0     1619 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/utilities/interfaces/settings_file_interface.py
+-rw-rw-rw-   0        0        0     3387 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/utilities/json_settings_file.py
+-rw-rw-rw-   0        0        0     3034 2023-06-02 17:00:05.000000 PyWebUIFramework-1.1/src/core/utilities/resource_file.py
+-rw-rw-rw-   0        0        0      391 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/utilities/utilities_module.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/waitings/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/waitings/__init__.py
+-rw-rw-rw-   0        0        0     5577 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/core/waitings/conditional_wait.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/core/waitings/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/waitings/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2722 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/core/waitings/interfaces/conditional_wait_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/elements/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/elements/attributes.py
+-rw-rw-rw-   0        0        0      215 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/elements/button.py
+-rw-rw-rw-   0        0        0      516 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/elements/check_box.py
+-rw-rw-rw-   0        0        0      436 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/elements/checkable_element.py
+-rw-rw-rw-   0        0        0      295 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/elements/combo_box.py
+-rw-rw-rw-   0        0        0     1694 2023-06-01 18:36:29.000000 PyWebUIFramework-1.1/src/elements/element_factory.py
+-rw-rw-rw-   0        0        0      213 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/elements/label.py
+-rw-rw-rw-   0        0        0      292 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/elements/link.py
+-rw-rw-rw-   0        0        0      229 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/elements/radio_button.py
+-rw-rw-rw-   0        0        0     1780 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/elements/text_box.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:06:46.000000 PyWebUIFramework-1.1/src/forms/
+-rw-rw-rw-   0        0        0        0 2023-06-01 17:36:37.000000 PyWebUIFramework-1.1/src/forms/__init__.py
+-rw-rw-rw-   0        0        0     1174 2023-06-01 18:36:30.000000 PyWebUIFramework-1.1/src/forms/base_form.py
```

### Comparing `PyWebUIFramework-1.0/setup.py` & `PyWebUIFramework-1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
-from get_project_root import root_path
 from setuptools import setup, find_packages
+from get_project_root import root_path
 
 # PATH VARIABLES
 SOURCE_NAME = "src"
-ROOT_DIR = root_path(ignore_cwd=True)
+ROOT_DIR = root_path()
 FRAMEWORK_NAME = os.path.basename(ROOT_DIR)
 REQUIREMENTS_FILE = os.path.join(ROOT_DIR, "requirements.txt")
 PATH_TO_RESOURCES = os.path.join("core", "resources")
 
 # PROJECT VARIABLES
-CURRENT_VERSION = "1.0"
+CURRENT_VERSION = "1.1"
 LICENSE_TYPE = "MIT"
 
 # AUTHOR VARIABLES
 AUTHOR_FULL_NAME = "Philip Vasilevsky"
 AUTHOR_EMAIL = "fil13698@gmail.com"
 LINK_TO_REPO = "https://github.com/philip136/PyWebUIFramework"
```

### Comparing `PyWebUIFramework-1.0/src/PyWebUIFramework.egg-info/SOURCES.txt` & `PyWebUIFramework-1.1/src/PyWebUIFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/base_browser_factory.py` & `PyWebUIFramework-1.1/src/browser/base_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/browser.py` & `PyWebUIFramework-1.1/src/browser/browser.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/browser_module.py` & `PyWebUIFramework-1.1/src/browser/browser_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/browser_tab_navigation.py` & `PyWebUIFramework-1.1/src/browser/browser_tab_navigation.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/interfaces/browser_factory_interface.py` & `PyWebUIFramework-1.1/src/browser/interfaces/browser_factory_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/java_script.py` & `PyWebUIFramework-1.1/src/browser/java_script.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/local_browser_factory.py` & `PyWebUIFramework-1.1/src/browser/local_browser_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/browser/py_quality_services.py` & `PyWebUIFramework-1.1/src/browser/py_quality_services.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/configuration/browser_profile.py` & `PyWebUIFramework-1.1/src/configuration/browser_profile.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/configuration/driver_settings/base_driver_settings.py` & `PyWebUIFramework-1.1/src/configuration/driver_settings/base_driver_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/configuration/driver_settings/chrome_settings.py` & `PyWebUIFramework-1.1/src/configuration/driver_settings/chrome_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/configuration/driver_settings/edge_settings.py` & `PyWebUIFramework-1.1/src/configuration/driver_settings/edge_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/configuration/driver_settings/firefox_settings.py` & `PyWebUIFramework-1.1/src/configuration/driver_settings/firefox_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/configuration/driver_settings/iexplorer_settings.py` & `PyWebUIFramework-1.1/src/configuration/driver_settings/iexplorer_settings.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/configuration/timeout_configuration.py` & `PyWebUIFramework-1.1/src/configuration/timeout_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/applications/quality_module.py` & `PyWebUIFramework-1.1/src/core/applications/quality_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/applications/quality_services.py` & `PyWebUIFramework-1.1/src/core/applications/quality_services.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/configurations/configuration_module.py` & `PyWebUIFramework-1.1/src/core/configurations/configuration_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/configurations/element_cache_configuration.py` & `PyWebUIFramework-1.1/src/core/configurations/element_cache_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/configurations/interfaces/browser_profile_interface.py` & `PyWebUIFramework-1.1/src/core/configurations/interfaces/browser_profile_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/configurations/interfaces/retry_configuration_interface.py` & `PyWebUIFramework-1.1/src/core/configurations/interfaces/retry_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/configurations/interfaces/timeout_configuration_interface.py` & `PyWebUIFramework-1.1/src/core/configurations/interfaces/timeout_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/configurations/retry_configuration.py` & `PyWebUIFramework-1.1/src/core/configurations/retry_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/configurations/timeout_configuration.py` & `PyWebUIFramework-1.1/src/core/configurations/timeout_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/actions/js_actions.py` & `PyWebUIFramework-1.1/src/core/elements/actions/js_actions.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/base_element.py` & `PyWebUIFramework-1.1/src/core/elements/base_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/base_element_cache_handler.py` & `PyWebUIFramework-1.1/src/core/elements/base_element_cache_handler.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/base_element_factory.py` & `PyWebUIFramework-1.1/src/core/elements/base_element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/base_parent_element.py` & `PyWebUIFramework-1.1/src/core/elements/base_parent_element.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/element_cache_handler.py` & `PyWebUIFramework-1.1/src/core/elements/element_cache_handler.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/element_factory.py` & `PyWebUIFramework-1.1/src/core/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/element_finder.py` & `PyWebUIFramework-1.1/src/core/elements/element_finder.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/element_finder_interface.py` & `PyWebUIFramework-1.1/src/core/elements/element_finder_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/states/base_element_state_provider.py` & `PyWebUIFramework-1.1/src/core/elements/states/base_element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/states/cached_element_state_provider.py` & `PyWebUIFramework-1.1/src/core/elements/states/cached_element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/states/desired_state.py` & `PyWebUIFramework-1.1/src/core/elements/states/desired_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/states/element_state.py` & `PyWebUIFramework-1.1/src/core/elements/states/element_state.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/elements/states/element_state_provider.py` & `PyWebUIFramework-1.1/src/core/elements/states/element_state_provider.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/localization/configurations/interfaces/logger_configuration_interface.py` & `PyWebUIFramework-1.1/src/core/localization/configurations/interfaces/logger_configuration_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/localization/configurations/logger_configuration.py` & `PyWebUIFramework-1.1/src/core/localization/configurations/logger_configuration.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/localization/localization_module.py` & `PyWebUIFramework-1.1/src/core/localization/localization_module.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/localization/loggers/interfaces/localized_logger_interface.py` & `PyWebUIFramework-1.1/src/core/localization/loggers/interfaces/localized_logger_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/localization/loggers/localized_logger.py` & `PyWebUIFramework-1.1/src/core/localization/loggers/localized_logger.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/localization/managers/localization_manager.py` & `PyWebUIFramework-1.1/src/core/localization/managers/localization_manager.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/utilities/action_repeater.py` & `PyWebUIFramework-1.1/src/core/utilities/action_repeater.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/utilities/interfaces/action_repeater_interface.py` & `PyWebUIFramework-1.1/src/core/utilities/interfaces/action_repeater_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/utilities/interfaces/settings_file_interface.py` & `PyWebUIFramework-1.1/src/core/utilities/interfaces/settings_file_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/utilities/json_settings_file.py` & `PyWebUIFramework-1.1/src/core/utilities/json_settings_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/utilities/resource_file.py` & `PyWebUIFramework-1.1/src/core/utilities/resource_file.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/waitings/conditional_wait.py` & `PyWebUIFramework-1.1/src/core/waitings/conditional_wait.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/core/waitings/interfaces/conditional_wait_interface.py` & `PyWebUIFramework-1.1/src/core/waitings/interfaces/conditional_wait_interface.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/elements/check_box.py` & `PyWebUIFramework-1.1/src/elements/check_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/elements/element_factory.py` & `PyWebUIFramework-1.1/src/elements/element_factory.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/elements/text_box.py` & `PyWebUIFramework-1.1/src/elements/text_box.py`

 * *Files identical despite different names*

### Comparing `PyWebUIFramework-1.0/src/forms/base_form.py` & `PyWebUIFramework-1.1/src/forms/base_form.py`

 * *Files identical despite different names*

