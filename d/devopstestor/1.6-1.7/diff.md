# Comparing `tmp/devopstestor-1.6.tar.gz` & `tmp/devopstestor-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstestor-1.6.tar", last modified: Tue May  9 15:13:17 2023, max compression
+gzip compressed data, was "devopstestor-1.7.tar", last modified: Fri Jun  2 12:37:33 2023, max compression
```

## Comparing `devopstestor-1.6.tar` & `devopstestor-1.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.498255 devopstestor-1.6/
--rw-rw-rw-   0 root         (0) root         (0)    22958 2023-05-09 15:13:04.000000 devopstestor-1.6/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-09 15:13:04.000000 devopstestor-1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-09 15:13:17.498255 devopstestor-1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-09 15:13:04.000000 devopstestor-1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.468050 devopstestor-1.6/devopstestor/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.471711 devopstestor-1.6/devopstestor/config/
--rw-rw-rw-   0 root         (0) root         (0)     2837 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/config/core.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.471711 devopstestor-1.6/devopstestor/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.473542 devopstestor-1.6/devopstestor/src/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/abstract/abstract_machine_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/abstract/abstract_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/abstract/abstract_report.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/abstract/abstract_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.477203 devopstestor-1.6/devopstestor/src/core/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/devopstestor_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/devopstestor_server.py
--rw-rw-rw-   0 root         (0) root         (0)     7926 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/global_config_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8219 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/machines_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/ordonnanceur.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/report_render_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/source_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/core/testcase_executor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.479034 devopstestor-1.6/devopstestor/src/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/lib/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/lib/json_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/lib/log_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.480864 devopstestor-1.6/devopstestor/src/machine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/machine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/machine/debug_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7573 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/machine/docker_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/machine/local_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7560 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/machine/vagrant_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.482695 devopstestor-1.6/devopstestor/src/provisionner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/provisionner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/provisionner/empty_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/provisionner/logstash_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     8768 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/provisionner/minion_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/provisionner/systemd_provisionner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.484525 devopstestor-1.6/devopstestor/src/reporting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/campaign_report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/deployment_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/report_elk_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.485441 devopstestor-1.6/devopstestor/src/reporting/report_html_renderer/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/report_html_renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
--rw-rw-rw-   0 root         (0) root         (0)     7258 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/report_text_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/scenario_report.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/testcase_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/reporting/verifier_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.488186 devopstestor-1.6/devopstestor/src/scenarios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/scenarios/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/scenarios/logstash.py
--rw-rw-rw-   0 root         (0) root         (0)     6385 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/scenarios/mock_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/scenarios/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.489102 devopstestor-1.6/devopstestor/src/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/sources/copytemplate_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/sources/dirlink_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/sources/git_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.490932 devopstestor-1.6/devopstestor/src/testcase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/testcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/testcase/scenario_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/testcase/test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/testcase/testcase_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/src/testcase/tests_cases_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.462558 devopstestor-1.6/devopstestor/testconf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.466219 devopstestor-1.6/devopstestor/testconf/verifiers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.491848 devopstestor-1.6/devopstestor/testconf/verifiers/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.491848 devopstestor-1.6/devopstestor/testconf/verifiers/service/
--rw-rw-rw-   0 root         (0) root         (0)     4529 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/service/http_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.492763 devopstestor-1.6/devopstestor/testconf/verifiers/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.492763 devopstestor-1.6/devopstestor/testconf/verifiers/tests/http_logger/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.493678 devopstestor-1.6/devopstestor/testconf/verifiers/tests/logstash/
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.493678 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.494594 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.494594 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/packages/
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.495509 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.496424 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/users/
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.496424 devopstestor-1.6/devopstestor/testconf/verifiers/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.498255 devopstestor-1.6/devopstestor/testconf/verifiers/utils/logstash/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/utils/logstash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6214 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-05-09 15:13:04.000000 devopstestor-1.6/devopstestor/testconf/verifiers/utils/verififier_luncher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:13:17.469880 devopstestor-1.6/devopstestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-09 15:13:17.000000 devopstestor-1.6/devopstestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4372 2023-05-09 15:13:17.000000 devopstestor-1.6/devopstestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:13:17.000000 devopstestor-1.6/devopstestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-09 15:13:17.000000 devopstestor-1.6/devopstestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 15:13:17.000000 devopstestor-1.6/devopstestor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 15:13:17.499170 devopstestor-1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-05-09 15:13:04.000000 devopstestor-1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.742342 devopstestor-1.7/
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2023-06-02 12:37:23.000000 devopstestor-1.7/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-02 12:37:23.000000 devopstestor-1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-02 12:37:33.742342 devopstestor-1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-02 12:37:23.000000 devopstestor-1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.726342 devopstestor-1.7/devopstestor/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.728342 devopstestor-1.7/devopstestor/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2837 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/core.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.728342 devopstestor-1.7/devopstestor/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.729342 devopstestor-1.7/devopstestor/src/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_machine_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.731342 devopstestor-1.7/devopstestor/src/core/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/devopstestor_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/devopstestor_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8011 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/global_config_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8219 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/machines_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/ordonnanceur.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/report_render_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/source_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/testcase_executor_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.732342 devopstestor-1.7/devopstestor/src/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/json_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/log_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.732342 devopstestor-1.7/devopstestor/src/machine/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/debug_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7573 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/docker_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/local_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/vagrant_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.733342 devopstestor-1.7/devopstestor/src/provisionner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/empty_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/logstash_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     8768 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/minion_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/systemd_provisionner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.735342 devopstestor-1.7/devopstestor/src/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/campaign_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/deployment_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_elk_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.735342 devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_text_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/scenario_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/testcase_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/verifier_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.736342 devopstestor-1.7/devopstestor/src/scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/logstash.py
+-rw-rw-rw-   0 root         (0) root         (0)     6385 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/mock_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.737342 devopstestor-1.7/devopstestor/src/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/copytemplate_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/dirlink_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/git_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.738342 devopstestor-1.7/devopstestor/src/testcase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/scenario_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/testcase_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/tests_cases_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.723342 devopstestor-1.7/devopstestor/testconf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.724342 devopstestor-1.7/devopstestor/testconf/verifiers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.738342 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/service/
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/service/http_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/http_logger/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.740342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.740342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.740342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/packages/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.741342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.741342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/users/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.741342 devopstestor-1.7/devopstestor/testconf/verifiers/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.742342 devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6214 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/utils/verififier_luncher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.726342 devopstestor-1.7/devopstestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 12:37:33.742342 devopstestor-1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-02 12:37:23.000000 devopstestor-1.7/setup.py
```

### Comparing `devopstestor-1.6/LICENCE` & `devopstestor-1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/PKG-INFO` & `devopstestor-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.6
+Version: 1.7
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.6/devopstestor/config/arguments.yml` & `devopstestor-1.7/devopstestor/config/arguments.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/config/machine.yml` & `devopstestor-1.7/devopstestor/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/config/report.yml` & `devopstestor-1.7/devopstestor/config/report.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/config/source_manager.yml` & `devopstestor-1.7/devopstestor/config/source_manager.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/config/testcase.yml` & `devopstestor-1.7/devopstestor/config/testcase.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/abstract/abstract_machine_controller.py` & `devopstestor-1.7/devopstestor/src/abstract/abstract_machine_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/abstract/abstract_provisionner.py` & `devopstestor-1.7/devopstestor/src/abstract/abstract_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/abstract/abstract_report.py` & `devopstestor-1.7/devopstestor/src/abstract/abstract_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/abstract/abstract_source_accessor.py` & `devopstestor-1.7/devopstestor/src/abstract/abstract_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/devopstestor.py` & `devopstestor-1.7/devopstestor/src/core/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/devopstestor_client.py` & `devopstestor-1.7/devopstestor/src/core/devopstestor_client.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/devopstestor_server.py` & `devopstestor-1.7/devopstestor/src/core/devopstestor_server.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/global_config_factory.py` & `devopstestor-1.7/devopstestor/src/core/global_config_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from glob import glob
 import os
 from log_manager import logging
 log = logging.getLogger('core.GlobalConfigLoader')
 from pathlib import Path
 import yaml
 import argparse
 from utils import flat_dict_to_nested_dict_with_array, nested_dict_to_flat_dict_with_array, copy_merge_recursive_dict, valuate_dict_with_context
@@ -144,15 +145,17 @@
             dict_input=base_config.config,
             context=base_config.config
         )
 
         """
             Calcul de chemins absolu
         """
-        list_paths = list(set(base_config.get_node('testcase').get_node('base_path').config))
+        list_paths = []
+        for lpath in list(set(base_config.get_node('testcase').get_node('base_path').config)):
+            list_paths += glob(lpath)
         netlist = []
         for lpath in list_paths:
             lgpath = str(lpath)
             if not os.path.isabs(lgpath):
                 lgpath = os.path.join(os.getcwd(), lpath)
                 if not os.path.exists(lgpath):
                     lgpath = os.path.join(base_config.config['client_path'], lpath)
```

### Comparing `devopstestor-1.6/devopstestor/src/core/machines_factory.py` & `devopstestor-1.7/devopstestor/src/core/machines_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/ordonnanceur.py` & `devopstestor-1.7/devopstestor/src/core/ordonnanceur.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/report_render_manager.py` & `devopstestor-1.7/devopstestor/src/core/report_render_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/source_manager.py` & `devopstestor-1.7/devopstestor/src/core/source_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/core/testcase_executor_factory.py` & `devopstestor-1.7/devopstestor/src/core/testcase_executor_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/lib/config.py` & `devopstestor-1.7/devopstestor/src/lib/config.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/lib/core_utils.py` & `devopstestor-1.7/devopstestor/src/lib/core_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/lib/json_utils.py` & `devopstestor-1.7/devopstestor/src/lib/json_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/lib/log_manager.py` & `devopstestor-1.7/devopstestor/src/lib/log_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/lib/utils.py` & `devopstestor-1.7/devopstestor/src/lib/utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/machine/debug_controller.py` & `devopstestor-1.7/devopstestor/src/machine/debug_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/machine/docker_controller.py` & `devopstestor-1.7/devopstestor/src/machine/docker_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/machine/local_controller.py` & `devopstestor-1.7/devopstestor/src/machine/local_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/machine/vagrant_controller.py` & `devopstestor-1.7/devopstestor/src/machine/vagrant_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/provisionner/empty_provisionner.py` & `devopstestor-1.7/devopstestor/src/provisionner/empty_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/provisionner/logstash_provisionner.py` & `devopstestor-1.7/devopstestor/src/provisionner/logstash_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/provisionner/minion_provisionner.py` & `devopstestor-1.7/devopstestor/src/provisionner/minion_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/provisionner/systemd_provisionner.py` & `devopstestor-1.7/devopstestor/src/provisionner/systemd_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/reporting/report_elk_renderer.py` & `devopstestor-1.7/devopstestor/src/reporting/report_elk_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/reporting/report_html_renderer/__init__.py` & `devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja` & `devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/reporting/report_text_renderer.py` & `devopstestor-1.7/devopstestor/src/reporting/report_text_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/reporting/scenario_report.py` & `devopstestor-1.7/devopstestor/src/reporting/scenario_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/reporting/testcase_report.py` & `devopstestor-1.7/devopstestor/src/reporting/testcase_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/reporting/verifier_report.py` & `devopstestor-1.7/devopstestor/src/reporting/verifier_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/scenarios/devopstestor.py` & `devopstestor-1.7/devopstestor/src/scenarios/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/scenarios/logstash.py` & `devopstestor-1.7/devopstestor/src/scenarios/logstash.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/scenarios/mock_utils.py` & `devopstestor-1.7/devopstestor/src/scenarios/mock_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/scenarios/systemd.py` & `devopstestor-1.7/devopstestor/src/scenarios/systemd.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/sources/copytemplate_source_accessor.py` & `devopstestor-1.7/devopstestor/src/sources/copytemplate_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/sources/dirlink_source_accessor.py` & `devopstestor-1.7/devopstestor/src/sources/dirlink_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/sources/git_source_accessor.py` & `devopstestor-1.7/devopstestor/src/sources/git_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/testcase/scenario_executor.py` & `devopstestor-1.7/devopstestor/src/testcase/scenario_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/testcase/test_case.py` & `devopstestor-1.7/devopstestor/src/testcase/test_case.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/testcase/testcase_executor.py` & `devopstestor-1.7/devopstestor/src/testcase/testcase_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/src/testcase/tests_cases_loader.py` & `devopstestor-1.7/devopstestor/src/testcase/tests_cases_loader.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/fixtures/context_fixtures.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/service/http_logger.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/service/http_logger.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor/testconf/verifiers/utils/verififier_luncher.py` & `devopstestor-1.7/devopstestor/testconf/verifiers/utils/verififier_luncher.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/devopstestor.egg-info/PKG-INFO` & `devopstestor-1.7/devopstestor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.6
+Version: 1.7
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.6/devopstestor.egg-info/SOURCES.txt` & `devopstestor-1.7/devopstestor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devopstestor-1.6/setup.py` & `devopstestor-1.7/setup.py`

 * *Files identical despite different names*

