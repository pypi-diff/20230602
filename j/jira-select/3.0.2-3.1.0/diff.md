# Comparing `tmp/jira-select-3.0.2.tar.gz` & `tmp/jira-select-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-select-3.0.2.tar", last modified: Sun May 14 23:29:32 2023, max compression
+gzip compressed data, was "jira-select-3.1.0.tar", last modified: Fri Jun  2 01:44:37 2023, max compression
```

## Comparing `jira-select-3.0.2.tar` & `jira-select-3.1.0.tar`

### file list

```diff
@@ -1,143 +1,144 @@
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.232909 jira-select-3.0.2/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      574 2023-05-14 23:29:18.000000 jira-select-3.0.2/.bumpversion.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1097 2023-03-04 07:50:34.000000 jira-select-3.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-26 21:00:29.000000 jira-select-3.0.2/MANIFEST.in
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-05-14 23:29:32.232909 jira-select-3.0.2/PKG-INFO
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.216909 jira-select-3.0.2/docs/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      580 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/Makefile
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.208909 jira-select-3.0.2/docs/_build/
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.208909 jira-select-3.0.2/docs/_build/html/
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.220908 jira-select-3.0.2/docs/_build/html/_sources/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/api_documentation.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      116 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/appendix.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/commands.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6018 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/examples.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/extending.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    16413 2023-03-04 03:10:17.000000 jira-select-3.0.2/docs/_build/html/_sources/functions.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4095 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/how_to.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1741 2023-03-04 06:42:17.000000 jira-select-3.0.2/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2023-03-04 07:50:34.000000 jira-select-3.0.2/docs/_build/html/_sources/parameters.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10703 2023-03-04 06:39:28.000000 jira-select-3.0.2/docs/_build/html/_sources/query.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1110 2023-03-05 04:20:36.000000 jira-select-3.0.2/docs/_build/html/_sources/query_lifecycle.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/quickstart.rst.txt
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.220908 jira-select-3.0.2/docs/_build/html/_sources/source/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.commands.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      903 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.formatters.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.functions.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/source/modules.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/source/setup.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/source/tests.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4099 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/_build/html/_sources/troubleshooting.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/api_documentation.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       99 2023-04-12 19:20:42.000000 jira-select-3.0.2/docs/appendix.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/commands.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5463 2023-05-14 23:29:18.000000 jira-select-3.0.2/docs/conf.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1028 2023-04-13 02:48:26.000000 jira-select-3.0.2/docs/evaluation_location.csv
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6051 2023-04-11 04:23:44.000000 jira-select-3.0.2/docs/examples.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/extending.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    20590 2023-04-12 04:17:05.000000 jira-select-3.0.2/docs/functions.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4124 2023-04-11 04:23:39.000000 jira-select-3.0.2/docs/how_to.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1758 2023-04-12 19:20:56.000000 jira-select-3.0.2/docs/index.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      787 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/make.bat
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      840 2023-04-11 04:20:52.000000 jira-select-3.0.2/docs/parameters.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    12629 2023-04-11 05:08:47.000000 jira-select-3.0.2/docs/query.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1171 2023-04-11 05:01:21.000000 jira-select-3.0.2/docs/query_lifecycle.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/quickstart.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       53 2023-03-05 04:28:37.000000 jira-select-3.0.2/docs/requirements.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      131 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/run.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.224908 jira-select-3.0.2/docs/source/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/source/jira_select.commands.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1240 2023-04-09 01:20:37.000000 jira-select-3.0.2/docs/source/jira_select.formatters.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/source/jira_select.functions.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/source/jira_select.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/source/modules.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/source/setup.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.0.2/docs/source/tests.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4136 2023-04-12 04:16:44.000000 jira-select-3.0.2/docs/troubleshooting.rst
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.224908 jira-select-3.0.2/jira_select/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2023-05-14 23:29:18.000000 jira-select-3.0.2/jira_select/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/__main__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.0.2/jira_select/cache.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.0.2/jira_select/cmdline.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.228908 jira-select-3.0.2/jira_select/commands/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/build_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/configure.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.0.2/jira_select/commands/functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/install_user_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/remove_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.0.2/jira_select/commands/run.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/run_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.0.2/jira_select/commands/schema.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/setup_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.0.2/jira_select/commands/shell.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.0.2/jira_select/commands/show_instances.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/commands/store_password.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/constants.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.0.2/jira_select/exceptions.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.228908 jira-select-3.0.2/jira_select/formatters/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/formatters/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.0.2/jira_select/formatters/csv.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/formatters/html.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.0.2/jira_select/formatters/json.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      386 2023-04-12 03:52:31.000000 jira-select-3.0.2/jira_select/formatters/raw.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.0.2/jira_select/formatters/table.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.0.2/jira_select/formatters/tsv.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.232909 jira-select-3.0.2/jira_select/functions/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.0.2/jira_select/functions/estimate_to_days.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/extract.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/field_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.0.2/jira_select/functions/flatten_changelog.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/flatten_list.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.0.2/jira_select/functions/get_issue.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3339 2023-04-12 02:18:27.000000 jira-select-3.0.2/jira_select/functions/get_issue_snapshot_on_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/get_sprint_by_id.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/get_sprint_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.0.2/jira_select/functions/interval_business_hours.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      859 2023-04-12 01:44:30.000000 jira-select-3.0.2/jira_select/functions/interval_matching.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.0.2/jira_select/functions/interval_size.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.0.2/jira_select/functions/json_dumps.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.0.2/jira_select/functions/parse_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/parse_datetime.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.0.2/jira_select/functions/simple_filter.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/simple_filter_any.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/sprint_details.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/functions/sprint_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1574 2023-04-12 03:38:13.000000 jira-select-3.0.2/jira_select/functions/subquery.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.0.2/jira_select/functions/union.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.0.2/jira_select/functions/workdays_in_state.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10116 2023-04-12 02:18:19.000000 jira-select-3.0.2/jira_select/plugin.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    23290 2023-04-13 02:51:26.000000 jira-select-3.0.2/jira_select/query.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.232909 jira-select-3.0.2/jira_select/sources/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.2/jira_select/sources/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.0.2/jira_select/sources/boards.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3983 2023-04-12 03:22:28.000000 jira-select-3.0.2/jira_select/sources/issues.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.0.2/jira_select/sources/sprints.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2254 2023-04-12 02:50:17.000000 jira-select-3.0.2/jira_select/types.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10705 2023-05-14 23:28:09.000000 jira-select-3.0.2/jira_select/utils.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.224908 jira-select-3.0.2/jira_select.egg-info/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-05-14 23:29:32.000000 jira-select-3.0.2/jira_select.egg-info/PKG-INFO
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4048 2023-05-14 23:29:32.000000 jira-select-3.0.2/jira_select.egg-info/SOURCES.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-05-14 23:29:32.000000 jira-select-3.0.2/jira_select.egg-info/dependency_links.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2594 2023-05-14 23:29:32.000000 jira-select-3.0.2/jira_select.egg-info/entry_points.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.0.2/jira_select.egg-info/not-zip-safe
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-05-14 23:29:32.000000 jira-select-3.0.2/jira_select.egg-info/requires.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-05-14 23:29:32.000000 jira-select-3.0.2/jira_select.egg-info/top_level.txt
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.232909 jira-select-3.0.2/pyinstaller/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2022-05-20 02:53:24.000000 jira-select-3.0.2/pyinstaller/Makefile
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2965 2022-05-20 02:53:24.000000 jira-select-3.0.2/pyinstaller/jira_select.exe.spec
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3160 2022-05-20 02:53:24.000000 jira-select-3.0.2/pyinstaller/jira_select.spec
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      163 2022-05-20 02:53:24.000000 jira-select-3.0.2/pyinstaller/requirements.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2843 2023-04-11 04:15:47.000000 jira-select-3.0.2/readme.md
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-04-26 21:05:39.000000 jira-select-3.0.2/requirements.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-05-14 23:29:32.232909 jira-select-3.0.2/setup.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5715 2023-05-14 23:29:18.000000 jira-select-3.0.2/setup.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-05-14 23:29:32.232909 jira-select-3.0.2/tests/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.2/tests/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.0.2/tests/base.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.0.2/tests/conftest.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.0.2/tests/test_functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.0.2/tests/test_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.0.2/tests/test_utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.649722 jira-select-3.1.0/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      574 2023-06-02 01:43:41.000000 jira-select-3.1.0/.bumpversion.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1097 2023-03-04 07:50:34.000000 jira-select-3.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-26 21:00:29.000000 jira-select-3.1.0/MANIFEST.in
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-06-02 01:44:37.649722 jira-select-3.1.0/PKG-INFO
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.633722 jira-select-3.1.0/docs/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      580 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/Makefile
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.625722 jira-select-3.1.0/docs/_build/
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.625722 jira-select-3.1.0/docs/_build/html/
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.633722 jira-select-3.1.0/docs/_build/html/_sources/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/api_documentation.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      116 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/appendix.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/commands.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6018 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/examples.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/extending.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    16413 2023-03-04 03:10:17.000000 jira-select-3.1.0/docs/_build/html/_sources/functions.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4095 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/how_to.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1741 2023-03-04 06:42:17.000000 jira-select-3.1.0/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2023-03-04 07:50:34.000000 jira-select-3.1.0/docs/_build/html/_sources/parameters.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10703 2023-03-04 06:39:28.000000 jira-select-3.1.0/docs/_build/html/_sources/query.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1110 2023-03-05 04:20:36.000000 jira-select-3.1.0/docs/_build/html/_sources/query_lifecycle.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/quickstart.rst.txt
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.637722 jira-select-3.1.0/docs/_build/html/_sources/source/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.commands.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      903 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.formatters.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.functions.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/source/modules.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/source/setup.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/source/tests.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4099 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/_build/html/_sources/troubleshooting.rst.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/api_documentation.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       99 2023-04-12 19:20:42.000000 jira-select-3.1.0/docs/appendix.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/commands.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5463 2023-06-02 01:43:41.000000 jira-select-3.1.0/docs/conf.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1028 2023-04-13 02:48:26.000000 jira-select-3.1.0/docs/evaluation_location.csv
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6051 2023-04-11 04:23:44.000000 jira-select-3.1.0/docs/examples.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/extending.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    21659 2023-06-02 01:42:06.000000 jira-select-3.1.0/docs/functions.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4124 2023-04-11 04:23:39.000000 jira-select-3.1.0/docs/how_to.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1758 2023-04-12 19:20:56.000000 jira-select-3.1.0/docs/index.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      787 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/make.bat
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      840 2023-04-11 04:20:52.000000 jira-select-3.1.0/docs/parameters.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    12629 2023-04-11 05:08:47.000000 jira-select-3.1.0/docs/query.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1171 2023-04-11 05:01:21.000000 jira-select-3.1.0/docs/query_lifecycle.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/quickstart.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       53 2023-03-05 04:28:37.000000 jira-select-3.1.0/docs/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      131 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/run.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.637722 jira-select-3.1.0/docs/source/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/source/jira_select.commands.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1240 2023-04-09 01:20:37.000000 jira-select-3.1.0/docs/source/jira_select.formatters.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/source/jira_select.functions.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/source/jira_select.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/source/modules.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/source/setup.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.1.0/docs/source/tests.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4136 2023-04-12 04:16:44.000000 jira-select-3.1.0/docs/troubleshooting.rst
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.641722 jira-select-3.1.0/jira_select/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2023-06-02 01:43:41.000000 jira-select-3.1.0/jira_select/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/__main__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.1.0/jira_select/cache.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.1.0/jira_select/cmdline.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.641722 jira-select-3.1.0/jira_select/commands/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/build_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/configure.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.1.0/jira_select/commands/functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/install_user_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/remove_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.1.0/jira_select/commands/run.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/run_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.1.0/jira_select/commands/schema.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/setup_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.1.0/jira_select/commands/shell.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.1.0/jira_select/commands/show_instances.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/commands/store_password.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/constants.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.1.0/jira_select/exceptions.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.641722 jira-select-3.1.0/jira_select/formatters/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/formatters/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.1.0/jira_select/formatters/csv.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/formatters/html.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.1.0/jira_select/formatters/json.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      386 2023-04-12 03:52:31.000000 jira-select-3.1.0/jira_select/formatters/raw.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.1.0/jira_select/formatters/table.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.1.0/jira_select/formatters/tsv.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.645722 jira-select-3.1.0/jira_select/functions/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.1.0/jira_select/functions/estimate_to_days.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/extract.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/field_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.1.0/jira_select/functions/flatten_changelog.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/flatten_list.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.1.0/jira_select/functions/get_issue.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3339 2023-04-12 02:18:27.000000 jira-select-3.1.0/jira_select/functions/get_issue_snapshot_on_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/get_sprint_by_id.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/get_sprint_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.1.0/jira_select/functions/interval_business_hours.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      859 2023-04-12 01:44:30.000000 jira-select-3.1.0/jira_select/functions/interval_matching.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.1.0/jira_select/functions/interval_size.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.1.0/jira_select/functions/json_dumps.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      408 2023-06-02 01:43:27.000000 jira-select-3.1.0/jira_select/functions/now.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.1.0/jira_select/functions/parse_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/parse_datetime.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.1.0/jira_select/functions/simple_filter.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/simple_filter_any.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/sprint_details.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/functions/sprint_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1574 2023-04-12 03:38:13.000000 jira-select-3.1.0/jira_select/functions/subquery.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.1.0/jira_select/functions/union.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.1.0/jira_select/functions/workdays_in_state.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10204 2023-06-02 01:42:06.000000 jira-select-3.1.0/jira_select/plugin.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    23290 2023-04-13 02:51:26.000000 jira-select-3.1.0/jira_select/query.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.649722 jira-select-3.1.0/jira_select/sources/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.1.0/jira_select/sources/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.1.0/jira_select/sources/boards.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3983 2023-04-12 03:22:28.000000 jira-select-3.1.0/jira_select/sources/issues.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.1.0/jira_select/sources/sprints.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2254 2023-04-12 02:50:17.000000 jira-select-3.1.0/jira_select/types.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10705 2023-05-14 23:28:09.000000 jira-select-3.1.0/jira_select/utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.641722 jira-select-3.1.0/jira_select.egg-info/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-06-02 01:44:37.000000 jira-select-3.1.0/jira_select.egg-info/PKG-INFO
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4077 2023-06-02 01:44:37.000000 jira-select-3.1.0/jira_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-06-02 01:44:37.000000 jira-select-3.1.0/jira_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2635 2023-06-02 01:44:37.000000 jira-select-3.1.0/jira_select.egg-info/entry_points.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.1.0/jira_select.egg-info/not-zip-safe
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-06-02 01:44:37.000000 jira-select-3.1.0/jira_select.egg-info/requires.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-06-02 01:44:37.000000 jira-select-3.1.0/jira_select.egg-info/top_level.txt
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.649722 jira-select-3.1.0/pyinstaller/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2022-05-20 02:53:24.000000 jira-select-3.1.0/pyinstaller/Makefile
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2965 2022-05-20 02:53:24.000000 jira-select-3.1.0/pyinstaller/jira_select.exe.spec
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3160 2022-05-20 02:53:24.000000 jira-select-3.1.0/pyinstaller/jira_select.spec
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      163 2022-05-20 02:53:24.000000 jira-select-3.1.0/pyinstaller/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2843 2023-04-11 04:15:47.000000 jira-select-3.1.0/readme.md
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-04-26 21:05:39.000000 jira-select-3.1.0/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-06-02 01:44:37.649722 jira-select-3.1.0/setup.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5771 2023-06-02 01:43:41.000000 jira-select-3.1.0/setup.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-06-02 01:44:37.649722 jira-select-3.1.0/tests/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.1.0/tests/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.1.0/tests/base.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.1.0/tests/conftest.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.1.0/tests/test_functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.1.0/tests/test_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.1.0/tests/test_utils.py
```

### Comparing `jira-select-3.0.2/.bumpversion.cfg` & `jira-select-3.1.0/.bumpversion.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.0.2
+current_version = 3.1.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>.*))?
 serialize = 
 	{major}.{minor}.{patch}.{release}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
```

### Comparing `jira-select-3.0.2/.pre-commit-config.yaml` & `jira-select-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/PKG-INFO` & `jira-select-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.0.2
+Version: 3.1.0
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
```

### Comparing `jira-select-3.0.2/docs/Makefile` & `jira-select-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/commands.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/commands.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/examples.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/extending.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/extending.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/functions.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/functions.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/how_to.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/how_to.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/index.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/parameters.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/parameters.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/query.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/query.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/query_lifecycle.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/query_lifecycle.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/quickstart.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.commands.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.commands.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.formatters.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.formatters.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.functions.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.functions.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/source/jira_select.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/source/jira_select.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/source/tests.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/source/tests.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/_build/html/_sources/troubleshooting.rst.txt` & `jira-select-3.1.0/docs/_build/html/_sources/troubleshooting.rst.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/commands.rst` & `jira-select-3.1.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/conf.py` & `jira-select-3.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 project = "Jira-Select"
 copyright = "2022, Adam Coddington"
 author = "Adam Coddington"
 
 # The short X.Y version
 version = ""
 # The full version, including alpha/beta/rc tags
-release = "3.0.2"
+release = "3.1.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `jira-select-3.0.2/docs/evaluation_location.csv` & `jira-select-3.1.0/docs/evaluation_location.csv`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/examples.rst` & `jira-select-3.1.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/extending.rst` & `jira-select-3.1.0/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/functions.rst` & `jira-select-3.1.0/docs/functions.rst`

 * *Files 4% similar despite different names*

```diff
@@ -351,28 +351,56 @@
    into a single list of the shape::
 
       [1, 2, 3, 4, 5, 6]
 
 Dates
 -----
 
+.. py:function:: now(**replacements) -> datetime.datetime
+
+   Return "now" as a timezone-aware ``datetime.datetime`` object.
+
+   Additional parameters can be passed via keyword arguments;
+   these values will be applied
+   to the ``datetime.datetime`` object
+   via its ``replace`` method.
+   See `Python's documentation <https://docs.python.org/3/library/datetime.html#datetime.datetime.replace>`_ for for more information .
+
+   If you would like to obtain a timezone-unaware datetime object,
+   pass ``tzinfo=None`` as a keyword argument.
+
+.. py:function:: timedelta(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0) -> datetime.timedelta
+
+   Returns a ``datetime.timedelta`` object.
+
+   This object can be used in math
+   with existing ``datetime.datetime``objects.
+
+.. py:function:: datetime(year, month, day, hour=0, minute=0, second=0, microsecond=0, tzinfo=None, *, fold=0) -> datetime.datetime
+
+   Returns a ``datetime.datetime`` object.
+
+   To obtain a ``date`` object, call ``.date()`` on the return value
+   of this function.
+
 .. py:function:: parse_datetime(datetime_string: str, *args, **kwargs) -> datetime.datetime
 
    Parse a date string into a datetime object.
 
    This relies on `python-dateutil`; there are many additional options available
    that you can find documented `here <https://dateutil.readthedocs.io/en/stable/parser.html#dateutil.parser.parse>`_.
 
 .. py:function:: parse_date(date_string: str, *args, **kwargs) -> datetime.date
 
    Parse a date string into a date object.
 
    This relies on `python-dateutil`; there are many additional options available
    that you can find documented `here <https://dateutil.readthedocs.io/en/stable/parser.html#dateutil.parser.parse>`_.
 
+
 Intervals
 ---------
 
 .. py:function:: empty_interval() -> portion.Interval
 
 .. py:function:: closed_interval() -> portion.Interval
```

### Comparing `jira-select-3.0.2/docs/how_to.rst` & `jira-select-3.1.0/docs/how_to.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/index.rst` & `jira-select-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/make.bat` & `jira-select-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/parameters.rst` & `jira-select-3.1.0/docs/parameters.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/query.rst` & `jira-select-3.1.0/docs/query.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/query_lifecycle.rst` & `jira-select-3.1.0/docs/query_lifecycle.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/quickstart.rst` & `jira-select-3.1.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/source/jira_select.commands.rst` & `jira-select-3.1.0/docs/source/jira_select.commands.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/source/jira_select.formatters.rst` & `jira-select-3.1.0/docs/source/jira_select.formatters.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/source/jira_select.functions.rst` & `jira-select-3.1.0/docs/source/jira_select.functions.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/source/jira_select.rst` & `jira-select-3.1.0/docs/source/jira_select.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/source/tests.rst` & `jira-select-3.1.0/docs/source/tests.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/docs/troubleshooting.rst` & `jira-select-3.1.0/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/cache.py` & `jira-select-3.1.0/jira_select/cache.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/cmdline.py` & `jira-select-3.1.0/jira_select/cmdline.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/build_query.py` & `jira-select-3.1.0/jira_select/commands/build_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/configure.py` & `jira-select-3.1.0/jira_select/commands/configure.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/functions.py` & `jira-select-3.1.0/jira_select/commands/functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/install_user_script.py` & `jira-select-3.1.0/jira_select/commands/install_user_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/run.py` & `jira-select-3.1.0/jira_select/commands/run.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/run_script.py` & `jira-select-3.1.0/jira_select/commands/run_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/schema.py` & `jira-select-3.1.0/jira_select/commands/schema.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/setup_instance.py` & `jira-select-3.1.0/jira_select/commands/setup_instance.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/shell.py` & `jira-select-3.1.0/jira_select/commands/shell.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/show_instances.py` & `jira-select-3.1.0/jira_select/commands/show_instances.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/commands/store_password.py` & `jira-select-3.1.0/jira_select/commands/store_password.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/formatters/csv.py` & `jira-select-3.1.0/jira_select/formatters/csv.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/formatters/html.py` & `jira-select-3.1.0/jira_select/formatters/html.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/formatters/json.py` & `jira-select-3.1.0/jira_select/formatters/json.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/formatters/table.py` & `jira-select-3.1.0/jira_select/formatters/table.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/estimate_to_days.py` & `jira-select-3.1.0/jira_select/functions/estimate_to_days.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/extract.py` & `jira-select-3.1.0/jira_select/functions/extract.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/field_by_name.py` & `jira-select-3.1.0/jira_select/functions/field_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/flatten_changelog.py` & `jira-select-3.1.0/jira_select/functions/flatten_changelog.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/get_issue_snapshot_on_date.py` & `jira-select-3.1.0/jira_select/functions/get_issue_snapshot_on_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/get_sprint_by_id.py` & `jira-select-3.1.0/jira_select/functions/get_sprint_by_id.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/get_sprint_by_name.py` & `jira-select-3.1.0/jira_select/functions/get_sprint_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/interval_business_hours.py` & `jira-select-3.1.0/jira_select/functions/interval_business_hours.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/interval_matching.py` & `jira-select-3.1.0/jira_select/functions/interval_matching.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/interval_size.py` & `jira-select-3.1.0/jira_select/functions/interval_size.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/parse_date.py` & `jira-select-3.1.0/jira_select/functions/parse_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/parse_datetime.py` & `jira-select-3.1.0/jira_select/functions/parse_datetime.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/simple_filter.py` & `jira-select-3.1.0/jira_select/functions/simple_filter.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/simple_filter_any.py` & `jira-select-3.1.0/jira_select/functions/simple_filter_any.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/sprint_details.py` & `jira-select-3.1.0/jira_select/functions/sprint_details.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/subquery.py` & `jira-select-3.1.0/jira_select/functions/subquery.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/functions/workdays_in_state.py` & `jira-select-3.1.0/jira_select/functions/workdays_in_state.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/plugin.py` & `jira-select-3.1.0/jira_select/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import copy
+import datetime
 import importlib.util
 import json
 import logging
 import os
 import random
 import statistics
 from abc import ABCMeta
@@ -105,14 +106,16 @@
     # JSON
     "json_loads": json.loads,
     "empty_interval": portion.empty,
     "closed_interval": portion.closed,
     "open_interval": portion.open,
     "openclosed_interval": portion.openclosed,
     "closedopen_interval": portion.closedopen,
+    "datetime": datetime.datetime,
+    "timedelta": datetime.timedelta,
 }
 REGISTERED_FUNCTIONS: Dict[str, Callable] = {}
 
 
 class BaseCommand(SafdieBaseCommand):
     _jira: Optional[JIRA] = None
```

### Comparing `jira-select-3.0.2/jira_select/query.py` & `jira-select-3.1.0/jira_select/query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/sources/boards.py` & `jira-select-3.1.0/jira_select/sources/boards.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/sources/issues.py` & `jira-select-3.1.0/jira_select/sources/issues.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/sources/sprints.py` & `jira-select-3.1.0/jira_select/sources/sprints.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/types.py` & `jira-select-3.1.0/jira_select/types.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select/utils.py` & `jira-select-3.1.0/jira_select/utils.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/jira_select.egg-info/PKG-INFO` & `jira-select-3.1.0/jira_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.0.2
+Version: 3.1.0
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
```

### Comparing `jira-select-3.0.2/jira_select.egg-info/SOURCES.txt` & `jira-select-3.1.0/jira_select.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 jira_select/functions/get_issue_snapshot_on_date.py
 jira_select/functions/get_sprint_by_id.py
 jira_select/functions/get_sprint_by_name.py
 jira_select/functions/interval_business_hours.py
 jira_select/functions/interval_matching.py
 jira_select/functions/interval_size.py
 jira_select/functions/json_dumps.py
+jira_select/functions/now.py
 jira_select/functions/parse_date.py
 jira_select/functions/parse_datetime.py
 jira_select/functions/simple_filter.py
 jira_select/functions/simple_filter_any.py
 jira_select/functions/sprint_details.py
 jira_select/functions/sprint_name.py
 jira_select/functions/subquery.py
```

### Comparing `jira-select-3.0.2/jira_select.egg-info/entry_points.txt` & `jira-select-3.1.0/jira_select.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 get_issue_snapshot_on_date = jira_select.functions.get_issue_snapshot_on_date:Function
 get_sprint_by_id = jira_select.functions.get_sprint_by_id:Function
 get_sprint_by_name = jira_select.functions.get_sprint_by_name:Function
 interval_business_hours = jira_select.functions.interval_business_hours:Function
 interval_matching = jira_select.functions.interval_matching:Function
 interval_size = jira_select.functions.interval_size:Function
 json_dumps = jira_select.functions.json_dumps:Function
+now = jira_select.functions.now:Function
 parse_date = jira_select.functions.parse_date:Function
 parse_datetime = jira_select.functions.parse_datetime:Function
 simple_filter = jira_select.functions.simple_filter:Function
 simple_filter_any = jira_select.functions.simple_filter_any:Function
 sprint_details = jira_select.functions.sprint_details:Function
 sprint_name = jira_select.functions.sprint_name:Function
 subquery = jira_select.functions.subquery:Function
```

### Comparing `jira-select-3.0.2/pyinstaller/Makefile` & `jira-select-3.1.0/pyinstaller/Makefile`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/pyinstaller/jira_select.exe.spec` & `jira-select-3.1.0/pyinstaller/jira_select.exe.spec`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/pyinstaller/jira_select.spec` & `jira-select-3.1.0/pyinstaller/jira_select.spec`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/readme.md` & `jira-select-3.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/setup.cfg` & `jira-select-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/setup.py` & `jira-select-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="jira-select",
-    version="3.0.2",
+    version="3.1.0",
     license="MIT",
     description=(
         "Easily run complex SQL-like queries far beyond what "
         "Jira's standard JQL query language can provide."
     ),
     long_description_content_type="text/markdown",
     long_description=read("readme.md"),
@@ -120,14 +120,15 @@
             "workdays_in_state = jira_select.functions.workdays_in_state:Function",
             "get_issue_snapshot_on_date = jira_select.functions.get_issue_snapshot_on_date:Function",
             "interval_business_hours = jira_select.functions.interval_business_hours:Function",
             "interval_matching = jira_select.functions.interval_matching:Function",
             "interval_size = jira_select.functions.interval_size:Function",
             "subquery = jira_select.functions.subquery:Function",
             "union = jira_select.functions.union:Function",
+            "now = jira_select.functions.now:Function",
         ],
         "jira_select.sources": [
             "issues = jira_select.sources.issues:Source",
             "boards = jira_select.sources.boards:Source",
             "sprints = jira_select.sources.sprints:Source",
         ],
     },
```

### Comparing `jira-select-3.0.2/tests/base.py` & `jira-select-3.1.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/tests/test_functions.py` & `jira-select-3.1.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/tests/test_query.py` & `jira-select-3.1.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.2/tests/test_utils.py` & `jira-select-3.1.0/tests/test_utils.py`

 * *Files identical despite different names*

