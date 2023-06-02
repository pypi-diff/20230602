# Comparing `tmp/capycli-2.0.0.tar.gz` & `tmp/capycli-2.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capycli-2.0.0.tar", max compression
+gzip compressed data, was "capycli-2.0.0.dev8.tar", max compression
```

## Comparing `capycli-2.0.0.tar` & `capycli-2.0.0.dev8.tar`

### file list

```diff
@@ -1,76 +1,75 @@
--rw-r--r--   0        0        0     6267 2023-05-17 09:09:21.101912 capycli-2.0.0/capycli/__init__.py
--rw-r--r--   0        0        0      445 2023-05-17 09:09:21.102694 capycli-2.0.0/capycli/__main__.py
--rw-r--r--   0        0        0      376 2023-05-17 09:09:21.103422 capycli-2.0.0/capycli/bom/__init__.py
--rw-r--r--   0        0        0     7084 2023-05-17 09:09:21.104247 capycli-2.0.0/capycli/bom/bom_convert.py
--rw-r--r--   0        0        0     7591 2023-05-17 09:35:47.841545 capycli-2.0.0/capycli/bom/check_bom.py
--rw-r--r--   0        0        0     8130 2023-05-30 07:53:23.575337 capycli-2.0.0/capycli/bom/check_bom_item_status.py
--rw-r--r--   0        0        0     9418 2023-05-30 07:53:23.576335 capycli-2.0.0/capycli/bom/check_granularity.py
--rw-r--r--   0        0        0    28424 2023-05-30 07:53:23.577343 capycli-2.0.0/capycli/bom/create_components.py
--rw-r--r--   0        0        0     2303 2023-05-30 07:53:23.577343 capycli-2.0.0/capycli/bom/csv.py
--rw-r--r--   0        0        0    10805 2023-05-30 07:53:23.578335 capycli-2.0.0/capycli/bom/diff_bom.py
--rw-r--r--   0        0        0     9071 2023-05-30 07:53:23.578335 capycli-2.0.0/capycli/bom/download_sources.py
--rw-r--r--   0        0        0    12898 2023-05-30 07:53:23.579342 capycli-2.0.0/capycli/bom/filter_bom.py
--rw-r--r--   0        0        0    11342 2023-05-17 09:09:21.109296 capycli-2.0.0/capycli/bom/findsources.py
--rw-r--r--   0        0        0     4868 2023-05-17 09:09:21.110297 capycli-2.0.0/capycli/bom/handle_bom.py
--rw-r--r--   0        0        0     2358 2023-05-30 07:53:23.579342 capycli-2.0.0/capycli/bom/html.py
--rw-r--r--   0        0        0    12554 2023-05-30 07:53:23.580342 capycli-2.0.0/capycli/bom/legacy.py
--rw-r--r--   0        0        0     5878 2023-05-17 09:09:21.119771 capycli-2.0.0/capycli/bom/legacy_cx.py
--rw-r--r--   0        0        0    45026 2023-06-02 07:46:43.725881 capycli-2.0.0/capycli/bom/map_bom.py
--rw-r--r--   0        0        0     6170 2023-05-17 09:09:21.121771 capycli-2.0.0/capycli/bom/merge_bom.py
--rw-r--r--   0        0        0     2312 2023-05-30 07:53:23.581337 capycli-2.0.0/capycli/bom/plaintext.py
--rw-r--r--   0        0        0     2659 2023-05-17 09:09:21.122947 capycli-2.0.0/capycli/bom/show_bom.py
--rw-r--r--   0        0        0      350 2023-05-17 09:09:21.122947 capycli-2.0.0/capycli/common/__init__.py
--rw-r--r--   0        0        0    22454 2023-05-30 07:53:23.581337 capycli-2.0.0/capycli/common/capycli_bom_support.py
--rw-r--r--   0        0        0     5172 2023-05-17 09:09:21.125218 capycli-2.0.0/capycli/common/comparable_version.py
--rw-r--r--   0        0        0     8519 2023-05-17 09:35:47.930366 capycli-2.0.0/capycli/common/component_cache.py
--rw-r--r--   0        0        0     2097 2023-05-17 09:09:21.126220 capycli-2.0.0/capycli/common/dependencies_base.py
--rw-r--r--   0        0        0      728 2023-05-17 09:09:21.126220 capycli-2.0.0/capycli/common/file_support.py
--rw-r--r--   0        0        0     4056 2023-05-17 09:09:21.126220 capycli-2.0.0/capycli/common/html_support.py
--rw-r--r--   0        0        0     1117 2023-05-17 09:09:21.127219 capycli-2.0.0/capycli/common/json_support.py
--rw-r--r--   0        0        0     3782 2023-05-17 09:09:21.127219 capycli-2.0.0/capycli/common/map_result.py
--rw-r--r--   0        0        0     1668 2023-05-17 09:09:21.127219 capycli-2.0.0/capycli/common/print.py
--rw-r--r--   0        0        0     7269 2023-06-02 07:05:02.748136 capycli-2.0.0/capycli/common/purl_service.py
--rw-r--r--   0        0        0     3102 2023-05-17 09:09:21.128219 capycli-2.0.0/capycli/common/purl_store.py
--rw-r--r--   0        0        0     3210 2023-05-17 09:09:21.129220 capycli-2.0.0/capycli/common/purl_utils.py
--rw-r--r--   0        0        0     5881 2023-05-22 07:23:49.894196 capycli-2.0.0/capycli/common/script_base.py
--rw-r--r--   0        0        0     2797 2023-05-17 09:09:21.129220 capycli-2.0.0/capycli/common/script_support.py
--rw-r--r--   0        0        0      329 2023-05-17 09:09:21.130298 capycli-2.0.0/capycli/data/__init__.py
--rw-r--r--   0        0        0   179392 2023-05-30 07:53:23.583348 capycli-2.0.0/capycli/data/granularity_list.csv
--rw-r--r--   0        0        0      344 2023-05-17 09:09:21.130298 capycli-2.0.0/capycli/dependencies/__init__.py
--rw-r--r--   0        0        0     2707 2023-05-17 09:09:21.131323 capycli-2.0.0/capycli/dependencies/handle_dependencies.py
--rw-r--r--   0        0        0    10128 2023-05-17 09:09:21.131323 capycli-2.0.0/capycli/dependencies/javascript.py
--rw-r--r--   0        0        0    13461 2023-05-30 07:53:23.584335 capycli-2.0.0/capycli/dependencies/maven_list.py
--rw-r--r--   0        0        0     5285 2023-05-17 09:09:21.132321 capycli-2.0.0/capycli/dependencies/maven_pom.py
--rw-r--r--   0        0        0     7048 2023-05-17 09:09:21.132321 capycli-2.0.0/capycli/dependencies/nuget.py
--rw-r--r--   0        0        0    19530 2023-05-31 09:39:50.171253 capycli-2.0.0/capycli/dependencies/python.py
--rw-r--r--   0        0        0      363 2023-05-17 09:09:21.133323 capycli-2.0.0/capycli/main/__init__.py
--rw-r--r--   0        0        0     5563 2023-05-17 09:09:21.134322 capycli-2.0.0/capycli/main/application.py
--rw-r--r--   0        0        0     3864 2023-05-17 09:09:21.134322 capycli-2.0.0/capycli/main/argument_parser.py
--rw-r--r--   0        0        0      821 2023-05-17 09:09:21.134322 capycli-2.0.0/capycli/main/cli.py
--rw-r--r--   0        0        0      441 2023-05-17 09:09:21.135549 capycli-2.0.0/capycli/main/exceptions.py
--rw-r--r--   0        0        0    14270 2023-05-22 07:23:49.906516 capycli-2.0.0/capycli/main/options.py
--rw-r--r--   0        0        0     1576 2023-05-17 09:09:21.135787 capycli-2.0.0/capycli/main/result_codes.py
--rw-r--r--   0        0        0     1533 2023-05-17 09:09:21.136793 capycli-2.0.0/capycli/mapping/handle_mapping.py
--rw-r--r--   0        0        0     7116 2023-05-17 09:09:21.136793 capycli-2.0.0/capycli/mapping/mapping_to_html.py
--rw-r--r--   0        0        0     7941 2023-05-17 09:09:21.137793 capycli-2.0.0/capycli/mapping/mapping_to_xlsx.py
--rw-r--r--   0        0        0     1604 2023-05-17 09:09:21.137793 capycli-2.0.0/capycli/moverview/handle_moverview.py
--rw-r--r--   0        0        0     4768 2023-05-17 09:09:21.138795 capycli-2.0.0/capycli/moverview/moverview_to_html.py
--rw-r--r--   0        0        0     6782 2023-05-17 09:09:21.138795 capycli-2.0.0/capycli/moverview/moverview_to_xlsx.py
--rw-r--r--   0        0        0      330 2023-05-17 09:09:21.138795 capycli-2.0.0/capycli/project/__init__.py
--rw-r--r--   0        0        0    12762 2023-05-17 09:09:21.139793 capycli-2.0.0/capycli/project/check_prerequisites.py
--rw-r--r--   0        0        0     7549 2023-05-17 09:35:48.097066 capycli-2.0.0/capycli/project/create_bom.py
--rw-r--r--   0        0        0    14480 2023-05-30 07:53:23.585991 capycli-2.0.0/capycli/project/create_project.py
--rw-r--r--   0        0        0    23010 2023-05-17 09:09:21.140793 capycli-2.0.0/capycli/project/create_readme.py
--rw-r--r--   0        0        0     4878 2023-05-17 09:35:48.108933 capycli-2.0.0/capycli/project/find_project.py
--rw-r--r--   0        0        0     9869 2023-05-17 09:35:48.112774 capycli-2.0.0/capycli/project/get_license_info.py
--rw-r--r--   0        0        0     4393 2023-05-17 09:09:21.141793 capycli-2.0.0/capycli/project/handle_project.py
--rw-r--r--   0        0        0     8729 2023-05-17 09:35:48.118779 capycli-2.0.0/capycli/project/show_ecc.py
--rw-r--r--   0        0        0     7618 2023-05-17 09:09:21.142795 capycli-2.0.0/capycli/project/show_licenses.py
--rw-r--r--   0        0        0     9571 2023-05-17 09:35:48.125375 capycli-2.0.0/capycli/project/show_project.py
--rw-r--r--   0        0        0     8806 2023-05-17 09:35:48.128620 capycli-2.0.0/capycli/project/show_vulnerabilities.py
--rw-r--r--   0        0        0     1218 2023-05-17 11:21:37.449769 capycli-2.0.0/License.md
-drwxr-xr-x   0        0        0        0 2023-05-17 09:11:25.459479 capycli-2.0.0/LICENSES/
--rw-r--r--   0        0        0     2116 2023-06-02 12:49:43.738841 capycli-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    12923 2023-05-30 07:53:23.569335 capycli-2.0.0/Readme.md
--rw-r--r--   0        0        0    14294 1970-01-01 00:00:00.000000 capycli-2.0.0/setup.py
--rw-r--r--   0        0        0    14369 1970-01-01 00:00:00.000000 capycli-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6267 2023-05-17 09:09:21.101912 capycli-2.0.0.dev8/capycli/__init__.py
+-rw-r--r--   0        0        0      445 2023-05-17 09:09:21.102694 capycli-2.0.0.dev8/capycli/__main__.py
+-rw-r--r--   0        0        0      376 2023-05-17 09:09:21.103422 capycli-2.0.0.dev8/capycli/bom/__init__.py
+-rw-r--r--   0        0        0     7084 2023-05-17 09:09:21.104247 capycli-2.0.0.dev8/capycli/bom/bom_convert.py
+-rw-r--r--   0        0        0     7591 2023-05-17 09:35:47.841545 capycli-2.0.0.dev8/capycli/bom/check_bom.py
+-rw-r--r--   0        0        0     8064 2023-05-17 09:35:47.844762 capycli-2.0.0.dev8/capycli/bom/check_bom_item_status.py
+-rw-r--r--   0        0        0     9019 2023-05-17 09:09:21.105296 capycli-2.0.0.dev8/capycli/bom/check_granularity.py
+-rw-r--r--   0        0        0    28418 2023-05-17 09:35:47.855951 capycli-2.0.0.dev8/capycli/bom/create_components.py
+-rw-r--r--   0        0        0     2276 2023-05-17 09:09:21.107298 capycli-2.0.0.dev8/capycli/bom/csv.py
+-rw-r--r--   0        0        0    10779 2023-05-17 09:09:21.108297 capycli-2.0.0.dev8/capycli/bom/diff_bom.py
+-rw-r--r--   0        0        0     9033 2023-05-17 09:09:21.108297 capycli-2.0.0.dev8/capycli/bom/download_sources.py
+-rw-r--r--   0        0        0    12786 2023-05-17 09:09:21.109296 capycli-2.0.0.dev8/capycli/bom/filter_bom.py
+-rw-r--r--   0        0        0    11342 2023-05-17 09:09:21.109296 capycli-2.0.0.dev8/capycli/bom/findsources.py
+-rw-r--r--   0        0        0     4868 2023-05-17 09:09:21.110297 capycli-2.0.0.dev8/capycli/bom/handle_bom.py
+-rw-r--r--   0        0        0     2352 2023-05-17 09:09:21.111298 capycli-2.0.0.dev8/capycli/bom/html.py
+-rw-r--r--   0        0        0    12542 2023-05-17 09:09:21.119771 capycli-2.0.0.dev8/capycli/bom/legacy.py
+-rw-r--r--   0        0        0     5878 2023-05-17 09:09:21.119771 capycli-2.0.0.dev8/capycli/bom/legacy_cx.py
+-rw-r--r--   0        0        0    44173 2023-05-17 09:09:21.121771 capycli-2.0.0.dev8/capycli/bom/map_bom.py
+-rw-r--r--   0        0        0     6170 2023-05-17 09:09:21.121771 capycli-2.0.0.dev8/capycli/bom/merge_bom.py
+-rw-r--r--   0        0        0     2285 2023-05-17 09:09:21.122947 capycli-2.0.0.dev8/capycli/bom/plaintext.py
+-rw-r--r--   0        0        0     2659 2023-05-17 09:09:21.122947 capycli-2.0.0.dev8/capycli/bom/show_bom.py
+-rw-r--r--   0        0        0      350 2023-05-17 09:09:21.122947 capycli-2.0.0.dev8/capycli/common/__init__.py
+-rw-r--r--   0        0        0    22442 2023-05-18 20:51:01.017627 capycli-2.0.0.dev8/capycli/common/capycli_bom_support.py
+-rw-r--r--   0        0        0     5172 2023-05-17 09:09:21.125218 capycli-2.0.0.dev8/capycli/common/comparable_version.py
+-rw-r--r--   0        0        0     8519 2023-05-17 09:35:47.930366 capycli-2.0.0.dev8/capycli/common/component_cache.py
+-rw-r--r--   0        0        0     2097 2023-05-17 09:09:21.126220 capycli-2.0.0.dev8/capycli/common/dependencies_base.py
+-rw-r--r--   0        0        0      728 2023-05-17 09:09:21.126220 capycli-2.0.0.dev8/capycli/common/file_support.py
+-rw-r--r--   0        0        0     4056 2023-05-17 09:09:21.126220 capycli-2.0.0.dev8/capycli/common/html_support.py
+-rw-r--r--   0        0        0     1117 2023-05-17 09:09:21.127219 capycli-2.0.0.dev8/capycli/common/json_support.py
+-rw-r--r--   0        0        0     3782 2023-05-17 09:09:21.127219 capycli-2.0.0.dev8/capycli/common/map_result.py
+-rw-r--r--   0        0        0     1668 2023-05-17 09:09:21.127219 capycli-2.0.0.dev8/capycli/common/print.py
+-rw-r--r--   0        0        0     7244 2023-05-17 09:35:47.945515 capycli-2.0.0.dev8/capycli/common/purl_service.py
+-rw-r--r--   0        0        0     3102 2023-05-17 09:09:21.128219 capycli-2.0.0.dev8/capycli/common/purl_store.py
+-rw-r--r--   0        0        0     3210 2023-05-17 09:09:21.129220 capycli-2.0.0.dev8/capycli/common/purl_utils.py
+-rw-r--r--   0        0        0     5881 2023-05-18 15:33:12.448837 capycli-2.0.0.dev8/capycli/common/script_base.py
+-rw-r--r--   0        0        0     2797 2023-05-17 09:09:21.129220 capycli-2.0.0.dev8/capycli/common/script_support.py
+-rw-r--r--   0        0        0      329 2023-05-17 09:09:21.130298 capycli-2.0.0.dev8/capycli/data/__init__.py
+-rw-r--r--   0        0        0    81841 2023-05-06 15:04:07.043859 capycli-2.0.0.dev8/capycli/data/granularity_list.csv
+-rw-r--r--   0        0        0      344 2023-05-17 09:09:21.130298 capycli-2.0.0.dev8/capycli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2707 2023-05-17 09:09:21.131323 capycli-2.0.0.dev8/capycli/dependencies/handle_dependencies.py
+-rw-r--r--   0        0        0    10128 2023-05-17 09:09:21.131323 capycli-2.0.0.dev8/capycli/dependencies/javascript.py
+-rw-r--r--   0        0        0    13429 2023-05-17 09:09:21.132321 capycli-2.0.0.dev8/capycli/dependencies/maven_list.py
+-rw-r--r--   0        0        0     5285 2023-05-17 09:09:21.132321 capycli-2.0.0.dev8/capycli/dependencies/maven_pom.py
+-rw-r--r--   0        0        0     7048 2023-05-17 09:09:21.132321 capycli-2.0.0.dev8/capycli/dependencies/nuget.py
+-rw-r--r--   0        0        0    13532 2023-05-17 09:09:21.133323 capycli-2.0.0.dev8/capycli/dependencies/python.py
+-rw-r--r--   0        0        0      363 2023-05-17 09:09:21.133323 capycli-2.0.0.dev8/capycli/main/__init__.py
+-rw-r--r--   0        0        0     5563 2023-05-17 09:09:21.134322 capycli-2.0.0.dev8/capycli/main/application.py
+-rw-r--r--   0        0        0     3864 2023-05-17 09:09:21.134322 capycli-2.0.0.dev8/capycli/main/argument_parser.py
+-rw-r--r--   0        0        0      821 2023-05-17 09:09:21.134322 capycli-2.0.0.dev8/capycli/main/cli.py
+-rw-r--r--   0        0        0      441 2023-05-17 09:09:21.135549 capycli-2.0.0.dev8/capycli/main/exceptions.py
+-rw-r--r--   0        0        0    14046 2023-05-17 09:25:27.047940 capycli-2.0.0.dev8/capycli/main/options.py
+-rw-r--r--   0        0        0     1576 2023-05-17 09:09:21.135787 capycli-2.0.0.dev8/capycli/main/result_codes.py
+-rw-r--r--   0        0        0     1533 2023-05-17 09:09:21.136793 capycli-2.0.0.dev8/capycli/mapping/handle_mapping.py
+-rw-r--r--   0        0        0     7116 2023-05-17 09:09:21.136793 capycli-2.0.0.dev8/capycli/mapping/mapping_to_html.py
+-rw-r--r--   0        0        0     7941 2023-05-17 09:09:21.137793 capycli-2.0.0.dev8/capycli/mapping/mapping_to_xlsx.py
+-rw-r--r--   0        0        0     1604 2023-05-17 09:09:21.137793 capycli-2.0.0.dev8/capycli/moverview/handle_moverview.py
+-rw-r--r--   0        0        0     4768 2023-05-17 09:09:21.138795 capycli-2.0.0.dev8/capycli/moverview/moverview_to_html.py
+-rw-r--r--   0        0        0     6782 2023-05-17 09:09:21.138795 capycli-2.0.0.dev8/capycli/moverview/moverview_to_xlsx.py
+-rw-r--r--   0        0        0      330 2023-05-17 09:09:21.138795 capycli-2.0.0.dev8/capycli/project/__init__.py
+-rw-r--r--   0        0        0    12762 2023-05-17 09:09:21.139793 capycli-2.0.0.dev8/capycli/project/check_prerequisites.py
+-rw-r--r--   0        0        0     7549 2023-05-17 09:35:48.097066 capycli-2.0.0.dev8/capycli/project/create_bom.py
+-rw-r--r--   0        0        0    14455 2023-05-17 09:35:48.100852 capycli-2.0.0.dev8/capycli/project/create_project.py
+-rw-r--r--   0        0        0    23010 2023-05-17 09:09:21.140793 capycli-2.0.0.dev8/capycli/project/create_readme.py
+-rw-r--r--   0        0        0     4878 2023-05-17 09:35:48.108933 capycli-2.0.0.dev8/capycli/project/find_project.py
+-rw-r--r--   0        0        0     9869 2023-05-17 09:35:48.112774 capycli-2.0.0.dev8/capycli/project/get_license_info.py
+-rw-r--r--   0        0        0     4393 2023-05-17 09:09:21.141793 capycli-2.0.0.dev8/capycli/project/handle_project.py
+-rw-r--r--   0        0        0     8729 2023-05-17 09:35:48.118779 capycli-2.0.0.dev8/capycli/project/show_ecc.py
+-rw-r--r--   0        0        0     7618 2023-05-17 09:09:21.142795 capycli-2.0.0.dev8/capycli/project/show_licenses.py
+-rw-r--r--   0        0        0     9571 2023-05-17 09:35:48.125375 capycli-2.0.0.dev8/capycli/project/show_project.py
+-rw-r--r--   0        0        0     8806 2023-05-17 09:35:48.128620 capycli-2.0.0.dev8/capycli/project/show_vulnerabilities.py
+-rw-r--r--   0        0        0     1218 2023-05-17 11:21:37.449769 capycli-2.0.0.dev8/License.md
+drwxr-xr-x   0        0        0        0 2023-05-17 09:11:25.459479 capycli-2.0.0.dev8/LICENSES/
+-rw-r--r--   0        0        0     1988 2023-05-19 17:46:30.373643 capycli-2.0.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0    11019 2023-05-18 20:38:48.645609 capycli-2.0.0.dev8/Readme.md
+-rw-r--r--   0        0        0    12389 1970-01-01 00:00:00.000000 capycli-2.0.0.dev8/PKG-INFO
```

### Comparing `capycli-2.0.0/capycli/__init__.py` & `capycli-2.0.0.dev8/capycli/__init__.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/bom/bom_convert.py` & `capycli-2.0.0.dev8/capycli/bom/bom_convert.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/bom/check_bom.py` & `capycli-2.0.0.dev8/capycli/bom/check_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/bom/check_bom_item_status.py` & `capycli-2.0.0.dev8/capycli/bom/check_bom_item_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 import logging
 import os
 import sys
-from typing import Any, Dict, Optional
 
 import requests
 import sw360.sw360_api
 from colorama import Fore, Style
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component
 
@@ -34,15 +33,15 @@
         for item in bom.components:
             sw360id = CycloneDxSupport.get_property_value(item, CycloneDxSupport.CDX_PROP_SW360ID)
             if not sw360id:
                 return True
 
         return False
 
-    def _find_by_id(self, component: Component) -> Optional[Dict[str, Any]]:
+    def _find_by_id(self, component: Component) -> dict | None:
         sw360id = CycloneDxSupport.get_property_value(component, CycloneDxSupport.CDX_PROP_SW360ID)
         try:
             release_details = self.client.get_release(sw360id)
             return release_details
         except sw360.sw360_api.SW360Error as swex:
             if swex.response.status_code == requests.codes['not_found']:
                 print(
@@ -57,15 +56,15 @@
                 print("  Status Code: " + str(swex.response.status_code))
                 if swex.message:
                     print("    Message: " + swex.message)
                 print(Style.RESET_ALL)
 
         return None
 
-    def _find_by_name(self, component: Component) -> Optional[Dict[str, Any]]:
+    def _find_by_name(self, component: Component) -> dict | None:
         try:
             releases = self.client.get_releases_by_name(component.name)
             if not releases:
                 return None
 
             for r in releases:
                 if r.get("version", "") == component.version:
```

### Comparing `capycli-2.0.0/capycli/bom/check_granularity.py` & `capycli-2.0.0.dev8/capycli/bom/check_granularity.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,17 @@
 # Copyright (c) 2021-2023 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
-try:
-    import importlib.resources as pkg_resources
-except ImportError:
-    # Try backported to PY<37 `importlib_resources`.
-    import importlib_resources as pkg_resources
+import importlib.resources
 import os
 import sys
-from typing import List
 
 from cyclonedx.model import ExternalReferenceType
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component
 from packageurl import PackageURL
 from sortedcontainers import SortedSet
 
@@ -48,21 +43,16 @@
         self.granularity_list = []
 
     def read_granularity_list(self) -> None:
         """Reads the granularity list from file."""
         self.granularity_list = []
 
         # read CSV from data resource
-        # depending on the Python version we need different ways for this
-        if sys.version_info >= (3, 9):
-            resources = pkg_resources.files("capycli.data")
-            text_list = (resources / "granularity_list.csv").read_text()
-        else:
-            text_list = pkg_resources.read_text("capycli.data", "granularity_list.csv")
-
+        resources = importlib.resources.files("capycli.data")
+        text_list = (resources / "granularity_list.csv").read_text()
         for line in text_list.splitlines():
             # ignore header (first) line
             if line.startswith("component_name;replacement_name"):
                 continue
 
             # ignore comments
             if line.startswith("#"):
@@ -140,15 +130,15 @@
 
         if component.purl and self.search_meta_data:
             if str(component.purl).startswith("pkg:npm"):
                 component_new = GetJavascriptDependencies().try_find_component_metadata(component_new, "")
 
         return component_new
 
-    def merge_duplicates(self, clist: List[Component]) -> List[Component]:
+    def merge_duplicates(self, clist: list[Component]) -> list[Component]:
         """Checks for each release if there are duplicates after granularity check."""
         new_list = []
         for release in clist:
             count = len([item for item in new_list if item.name == release.name
                          and item.version == release.version])
             if count > 0:
                 continue
```

### Comparing `capycli-2.0.0/capycli/bom/create_components.py` & `capycli-2.0.0.dev8/capycli/bom/create_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -------------------------------------------------------------------------------
 
 import logging
 import os
 import re
 import sys
 import tempfile
-from typing import Any, Dict
+from typing import Any
 from urllib.parse import urlparse
 
 import packageurl
 import requests
 import sw360.sw360_api
 from colorama import Fore, Style
 from cyclonedx.model.bom import Bom
@@ -256,15 +256,15 @@
                 component_id, release_details=data)
         except sw360.sw360_api.SW360Error as swex:
             errortext = "    Error creating component: " + self.get_error_message(swex)
             print_red(errortext)
             sys.exit(ResultCode.RESULT_ERROR_CREATING_COMPONENT)
         return release_new
 
-    def update_release(self, cx_comp: Component, release_data: Dict[str, Any]):
+    def update_release(self, cx_comp: Component, release_data: dict[str, Any]):
         """Update an existing release on SW360
 
         :param item: a single bill of materials item - a release
         :type item: dictionary
         :param release_data: SW360 release data
         :type release_data: release (dictionary)
         """
```

### Comparing `capycli-2.0.0/capycli/bom/csv.py` & `capycli-2.0.0.dev8/capycli/bom/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # Copyright (c) 2023 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
-from typing import List
-
 from cyclonedx.model.component import Component
 
 from capycli import LOG
 
 # -------------------------------------
 # Expected File Format
 #
@@ -23,15 +21,15 @@
 # wheel;0.34.2;
 # tomli;2.0.1;
 # -------------------------------------
 
 
 class CsvSupport():
     @classmethod
-    def csv_to_cdx_components(cls, inputfile: str) -> List[Component]:
+    def csv_to_cdx_components(cls, inputfile: str) -> list[Component]:
         """Convert a csv file of components to a list
         of CycloneDX components."""
         bom = []
         LOG.debug(f"Reading from file {inputfile}")
         with open(inputfile) as fin:
             for line in fin:
                 line = line.strip()
@@ -52,15 +50,15 @@
                     description=description)
 
                 bom.append(cxcomp)
 
         return bom
 
     @classmethod
-    def write_cdx_components_as_csv(cls, bom: List[Component], outputfile: str) -> None:
+    def write_cdx_components_as_csv(cls, bom: list[Component], outputfile: str) -> None:
         LOG.debug(f"Writing to file {outputfile}")
         with open(outputfile, "w", encoding="utf-8") as fout:
             for cx_comp in bom:
 
                 name = cx_comp.name
                 version = cx_comp.version
                 description = ""
```

### Comparing `capycli-2.0.0/capycli/bom/diff_bom.py` & `capycli-2.0.0.dev8/capycli/bom/diff_bom.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 import os
 import sys
 from enum import Enum
-from typing import Tuple
 
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component
 
 import capycli.common.json_support
 import capycli.common.script_base
 from capycli.bom.merge_bom import MergeBom
@@ -57,15 +56,15 @@
         """Searches for an item with the given name and version in the given SBOM."""
         for c in bom.components:
             if MergeBom.are_same(c, component):
                 return c
 
         return None
 
-    def compare_boms(self, bom_old: Bom, bom_new: Bom) -> Tuple[Bom, Bom]:
+    def compare_boms(self, bom_old: Bom, bom_new: Bom) -> tuple[Bom, Bom]:
         equal_bom = SbomCreator.create([])
         diff_bom = SbomCreator.create([])
         for comp_old in bom_old.components:
             found = self.find_in_bom(bom_new, comp_old)
             if found:
                 print_green(
                     "  Release exists in both SBOMs: " +
```

### Comparing `capycli-2.0.0/capycli/bom/download_sources.py` & `capycli-2.0.0.dev8/capycli/bom/download_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import hashlib
 import logging
 import os
 import pathlib
 import re
 import sys
-from typing import Optional, Tuple
 from urllib.parse import urlparse
 
 import requests
 from cyclonedx.model import ExternalReference, ExternalReferenceType, HashAlgorithm, HashType
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component
 
@@ -42,15 +41,15 @@
         if not cd:
             return None
         fname = re.findall('filename=(.+)', cd)
         if len(fname) == 0:
             return None
         return fname[0].rstrip('"').lstrip('"')
 
-    def download_source_file(self, url: str, source_folder: str) -> Optional[Tuple]:
+    def download_source_file(self, url: str, source_folder: str) -> tuple or None:
         """Download a file from a URL.
 
         @params:
             url           - Required : url of the file to get uploaded (string)
             source_folder - Required : folder to store the source files (string)
         """
         print_text("    URL = " + url)
```

### Comparing `capycli-2.0.0/capycli/bom/filter_bom.py` & `capycli-2.0.0.dev8/capycli/bom/filter_bom.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,23 +72,22 @@
             print_text(
                 "  ", comp.get("Name", ""), comp.get("Version", ""),
                 comp.get("RepositoryId", ""), entry["Mode"])
 
     def find_bom_item(self, bom: Bom, filterentry: dict) -> Optional[Component]:
         """Find an entry in list of bom items."""
         for component in bom.components:
-            if component.purl:
-                if filterentry.get("RepositoryId", "x") == component.purl:
-                    return component
+            if filterentry.get("RepositoryId", "x") == component.purl:
+                return component
 
-                if filterentry.get("purl", "x") == component.purl:
-                    return component
+            if filterentry.get("purl", "x") == component.purl:
+                return component
 
-                if filterentry.get("package-url", "x") == component.purl:
-                    return component
+            if filterentry.get("package-url", "x") == component.purl:
+                return component
 
             if filterentry.get("Name", "x") == component.name:
                 if filterentry.get("Version", "x") == component.version:
                     return component
 
         return None
 
@@ -204,19 +203,18 @@
                     else:
                         match = component.name == filterentry["component"]["Name"]
                 elif "RepositoryId" in filterentry["component"]:
                     prefix = ""
                     if filterentry["component"]["RepositoryId"].endswith("*"):
                         prefix = filterentry["component"]["RepositoryId"][:-1]
 
-                    if component.purl:
-                        if prefix:
-                            match = component.purl.startswith(prefix)
-                        else:
-                            match = component.purl == filterentry["component"]["RepositoryId"]
+                    if prefix:
+                        match = component.purl.startswith(prefix)
+                    else:
+                        match = component.purl == filterentry["component"]["RepositoryId"]
 
                 if match:
                     if filterentry["Mode"] == "remove":
                         filterentry["Processed"] = True
                         del_item = True
                         if self.verbose:
                             print_text("  Removing " + component.name + ", " + component.version)
```

### Comparing `capycli-2.0.0/capycli/bom/findsources.py` & `capycli-2.0.0.dev8/capycli/bom/findsources.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/bom/handle_bom.py` & `capycli-2.0.0.dev8/capycli/bom/handle_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/bom/html.py` & `capycli-2.0.0.dev8/capycli/bom/html.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # Copyright (c) 2023 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
-from typing import List, Optional
+from typing import Optional
 
 from cyclonedx.model.component import Component
 
 from capycli import LOG
 from capycli.common.html_support import HtmlSupport
 from capycli.main.exceptions import CaPyCliException
 
 
 class HtmlConversionSupport():
     @classmethod
     def write_cdx_components_as_html(
             cls,
-            bom: List[Component],
+            bom: list[Component],
             outputfile: str,
             project: Optional[Component]) -> None:
         myhtml = HtmlSupport()
         lineend = myhtml.get_lineend()
 
         LOG.debug(f"Writing to file {outputfile}")
         try:
```

### Comparing `capycli-2.0.0/capycli/bom/legacy.py` & `capycli-2.0.0.dev8/capycli/bom/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
-from typing import Any, Dict, List
+from typing import Any
 
 from cyclonedx.model import ExternalReference, ExternalReferenceType, HashAlgorithm, HashType, Property
 from cyclonedx.model.component import Component
 from packageurl import PackageURL  # type: ignore
 
 from capycli import LOG
 from capycli.common import json_support
@@ -45,15 +45,15 @@
 # * ClearingState
 # * ReleaseMainlineState
 # -------------------------------------
 
 
 class LegacySupport():
     @staticmethod
-    def get_purl_from_name(item: Dict[str, Any]) -> Any:
+    def get_purl_from_name(item: dict[str, Any]) -> Any:
         """Builds/guesses a package-url from name, version
         and provided language information."""
         lang = "generic"
         if "Language" in item:
             if item["Language"].lower() == "python":
                 lang = "pypi"
             elif item["Language"].lower() == "c#":
@@ -63,25 +63,25 @@
             if item["Language"].lower() == "javascript":
                 lang = "npm"
 
         purl = PackageURL(type=lang, name=item.get("Name", ""), version=item.get("Version", "")).to_string()
         return purl
 
     @staticmethod
-    def get_purl_from_legacy(item: Dict[str, Any]) -> Any:
+    def get_purl_from_legacy(item: dict[str, Any]) -> Any:
         if "RepositoryType" in item:
             if (item["RepositoryType"] == "package-url") or (item["RepositoryType"] == "purl"):
                 id = item.get("RepositoryId", "")
                 if id:
                     return id
 
         return LegacySupport.get_purl_from_name(item)
 
     @staticmethod
-    def legacy_component_to_cdx(item: Dict[str, Any]) -> Component:
+    def legacy_component_to_cdx(item: dict[str, Any]) -> Component:
         """Convert a single CaPyCLI legacy component to a CycloneDX component."""
         purl = LegacySupport.get_purl_from_legacy(item)
         if purl:
             cxcomp = Component(
                 name=item.get("Name", "").strip(),
                 version=item.get("Version", "").strip(),
                 purl=purl,
@@ -243,30 +243,30 @@
                 name=CycloneDxSupport.CDX_PROP_LANGUAGE,
                 value=language)
             cxcomp.properties.add(prop)
 
         return cxcomp
 
     @classmethod
-    def legacy_to_cdx_components(cls, inputfile: str) -> List[Component]:
+    def legacy_to_cdx_components(cls, inputfile: str) -> list[Component]:
         """Convert a CaPyCLI legacy  list of components to a list
         of CycloneDX components."""
         LOG.debug(f"Reading from file {inputfile}")
         bom = []
         legacy_bom = json_support.load_json_file(inputfile)
         for item in legacy_bom:
             cxcomp = LegacySupport.legacy_component_to_cdx(item)
             LOG.debug(f"  Reading from legacy: name={cxcomp.name}, version={cxcomp.version}")
 
             bom.append(cxcomp)
 
         return bom
 
     @classmethod
-    def cdx_component_to_legacy(cls, cx_comp: Component) -> Dict[str, Any]:
+    def cdx_component_to_legacy(cls, cx_comp: Component) -> dict[str, Any]:
         lcomp = {}
         lcomp["Name"] = cx_comp.name
         lcomp["Version"] = cx_comp.version or ""
         lcomp["Description"] = cx_comp.description or ""
         lcomp["Language"] = CycloneDxSupport.get_property_value(cx_comp, CycloneDxSupport.CDX_PROP_LANGUAGE)
         lcomp["SourceUrl"] = str(CycloneDxSupport.get_ext_ref_source_url(cx_comp))
         lcomp["RepositoryUrl"] = CycloneDxSupport.get_ext_ref_repository(cx_comp)
@@ -295,15 +295,15 @@
         lcomp["ProjectClearingState"] = CycloneDxSupport.get_property_value(
             cx_comp, CycloneDxSupport.CDX_PROP_PROJ_STATE)
         lcomp["ComponentId"] = CycloneDxSupport.get_property_value(cx_comp, CycloneDxSupport.CDX_PROP_COMPONENT_ID)
 
         return lcomp
 
     @classmethod
-    def write_cdx_components_as_legacy(cls, bom: List[Component], outputfile: str) -> None:
+    def write_cdx_components_as_legacy(cls, bom: list[Component], outputfile: str) -> None:
         LOG.debug(f"Writing to file {outputfile}")
 
         legacy_bom = []
         for cx_comp in bom:
             lcomp = cls.cdx_component_to_legacy(cx_comp)
             legacy_bom.append(lcomp)
```

### Comparing `capycli-2.0.0/capycli/bom/legacy_cx.py` & `capycli-2.0.0.dev8/capycli/bom/legacy_cx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/bom/map_bom.py` & `capycli-2.0.0.dev8/capycli/bom/map_bom.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 import json
 import logging
 import os
 import pathlib
 import re
 import sys
-from enum import Enum
-from typing import Any, Dict, List
+from typing import Any
 
 from cyclonedx.model import ExternalReference, ExternalReferenceType
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component
 
 import capycli.common.file_support
 import capycli.common.script_base
@@ -30,35 +29,35 @@
 from capycli.common.print import print_green, print_red, print_text, print_yellow
 from capycli.common.purl_service import PurlService
 from capycli.main.result_codes import ResultCode
 
 LOG = get_logger(__name__)
 
 
-class MapMode(str, Enum):
-    # default, write everything to resulting SBOM
-    ALL = "all"
-    # resulting SBOM shows only components that were found
-    FOUND = "found"
-    # resulting SBOM shows only components that were not found
-    NOT_FOUND = "notfound"
-
-
 class MapBom(capycli.common.script_base.ScriptBase):
     """
     Map a given SBOM to data on SW360
     """
+
+    # default, write everything to resulting SBOM
+    MAP_MODE_ALL = "0"
+
+    # resulting SBOM shows only components that were found
+    MAP_MODE_FOUND = "1"
+
+    # resulting SBOM shows only components that were not found
+    MAP_MODE_NOT_FOUND = "2"
+
     def __init__(self) -> None:
         self.releases = None
         self.old_releases = None
         self.verbosity = 1
         self.relaxed_debian_parsing = False
-        self.mode = MapMode.ALL
+        self.mode = self.MAP_MODE_ALL
         self.purl_service: PurlService = None
-        self.no_match_by_name_only = True
 
     def is_id_match(self, release, component: Component) -> bool:
         """Determines whether this release is a match via identifier for the specified SBOM item"""
         if not component.purl:
             return False
 
         cmp = component.purl.lower()
@@ -118,15 +117,15 @@
                     match_count = match_count + 1
 
             if match_count >= SIMILARITY_THRESHOLD:
                 return True
 
         return False
 
-    def is_better_match(self, releases_found: List[dict], proposed_match_code) -> bool:
+    def is_better_match(self, releases_found: list[dict], proposed_match_code) -> bool:
         if not releases_found:
             return True
 
         best_match = MapResult.NO_MATCH
         for rel in releases_found:
             if rel["MapResult"] < best_match:
                 best_match = rel["MapResult"]
@@ -281,21 +280,17 @@
 
                     if self.verbosity > 1:
                         print("    ADDED (MATCH_BY_FILENAME) " + release["Sw360Id"])
                     break
 
             # fifth check: name and ANY version
             if name_match:
-                if self.is_better_match(result.releases, MapResult.MATCH_BY_NAME):
-                    if self.no_match_by_name_only:
-                        nn = release.get("Name", "")
-                        vv = release.get("Version", "")
-                        print_yellow(f"Match by name only found for {nn}, {component.version} => {vv}, but ignored")
-                        continue
-
+                if self.is_better_match(
+                    result.releases, MapResult.MATCH_BY_NAME
+                ):
                     result.releases.clear()
 
                     if self.verbosity > 1:
                         print("    CLEAR (MATCH_BY_NAME)")
                     result.result = MapResult.MATCH_BY_NAME
 
                 release["MapResult"] = MapResult.MATCH_BY_NAME
@@ -465,20 +460,14 @@
                         result.releases.append(release)
                         if self.verbosity > 1:
                             print("    ADDED (FULL_MATCH_BY_HASH) " + release["Sw360Id"])
                         break
 
                 # fifth check: name and ANY version
                 if self.is_better_match(result.releases, MapResult.MATCH_BY_NAME):
-                    if self.no_match_by_name_only:
-                        nn = release.get("Name", "")
-                        vv = release.get("Version", "")
-                        print_yellow(f"Match by name only found for {nn}, {component.version} => {vv}, but ignored")
-                        continue
-
                     result.releases.clear()
 
                     if self.verbosity > 1:
                         print_text("    CLEAR (MATCH_BY_NAME)")
                     result.result = MapResult.MATCH_BY_NAME
 
                 release["MapResult"] = MapResult.MATCH_BY_NAME
@@ -505,27 +494,27 @@
         cr = ComponentCacheManagement.get_attachment(release, "CLEARING_REPORT")
         if cr:
             return True
 
         return False
 
     def map_bom_to_releases(
-            self, sbom: Bom, check_similar: bool, result_required: bool, nocache: bool = False) -> List[MapResult]:
+            self, sbom: Bom, check_similar: bool, result_required: bool, nocache: bool = False) -> list[MapResult]:
         """Maps the bill of material items to the list of SW360 releases"""
 
         # Initialize external id service now, before ruin the stdout for mapping
         # with information of the cache build
         #
         # quick guess of all purl types in bom, if we make a mistake here, PurlService will
         # retrieve missing types later
         purl_types = set()
         for component in sbom.components:
-            if component.purl and len(component.purl) > 8 and component.purl.startswith("pkg:"):
+            if len(component.purl) > 8 and component.purl.startswith("pkg:"):
                 purl_types.add(component.purl[4:7])
-        self.external_id_svc.build_purl_cache(purl_types, self.verbosity <= 1)
+        self.external_id_svc.build_purl_cache(purl_types, False)
 
         mapresult: list[MapResult] = []
         for component in sbom.components:
             try:
                 print_text("  " + component.name + ", " + component.version)
                 if nocache:
                     res = self.map_bom_item_no_cache(component)
@@ -544,15 +533,15 @@
         pass
 
     def search_binary_hash_match(self, hashvalue):
         """Searches SW360 for a release with an attachment with
         the specified binary file hash"""
         pass
 
-    def create_overview(self, result: List[MapResult]) -> Dict[str, Any]:
+    def create_overview(self, result: list[MapResult]) -> dict[str, Any]:
         """Create JSON data with an mapping result overview"""
         data = {}
         dataitems = []
         overall_result = "COMPLETE"
         count = 0
         for item in result:
             dataitem = {}
@@ -714,34 +703,34 @@
                 CycloneDxSupport.update_or_set_property(
                     component, CycloneDxSupport.CDX_PROP_SW360ID, value_match)
             elif not prop.value:
                 prop.value = value_match
 
         return component
 
-    def create_updated_bom(self, old_bom: Bom, result: List[MapResult]) -> Bom:
+    def create_updated_bom(self, old_bom: Bom, result: list[MapResult]) -> Bom:
         """Create an updated SBOM with the mapping results"""
         newbom = old_bom
 
         # clear all existing components
         newbom.components.clear()
 
         for item in result:
             newitem = None
             if item.result == MapResult.INVALID:
-                if (self.mode == MapMode.FOUND):
+                if (self.mode == self.MAP_MODE_FOUND):
                     continue
 
                 newitem = Component(name="???", version="???")
                 CycloneDxSupport.update_or_set_property(newitem, CycloneDxSupport.CDX_PROP_MAPRESULT, item.result)
                 newbom.components.add(newitem)
             elif (item.result == MapResult.NO_MATCH
                   or not self.is_good_match(item.result)):
 
-                if (self.mode == MapMode.FOUND):
+                if (self.mode == self.MAP_MODE_FOUND):
                     continue
 
                 newitem = item.component
                 CycloneDxSupport.update_or_set_property(
                     newitem,
                     CycloneDxSupport.CDX_PROP_MAPRESULT,
                     MapResult.NO_MATCH)
@@ -762,15 +751,15 @@
                     newitem = self.update_bom_item(None, match_item)
 
                 CycloneDxSupport.update_or_set_property(
                     newitem,
                     CycloneDxSupport.CDX_PROP_MAPRESULT,
                     match_item["MapResult"])
 
-                if (self.mode == MapMode.NOT_FOUND) and (self.is_good_match(match_item["MapResult"])):
+                if (self.mode == self.MAP_MODE_NOT_FOUND) and (self.is_good_match(match_item["MapResult"])):
                     continue
 
                 newbom.components.add(newitem)
 
         return newbom
 
     def write_mapping_result(self, result: dict, filename: str) -> None:
@@ -902,20 +891,19 @@
         print("    -t SW360_TOKEN, --token SW360_TOKEN")
         print("                          use this token for access to SW360")
         print("    -url SW360_URL        use this URL for access to SW360")
         print("    -oa, --oauth2         this is an oauth2 token")
         print("    -v                    be verbose")
         print("    --nocache             do not use component cache")
         print("    -m MODE, --mode MODE  mapping mode")
-        print("                          all = default, write everything to resulting SBOM")
-        print("                          found = resulting SBOM shows only components that were found")
-        print("                          notfound = resulting SBOM shows only components that were not found")
+        print("                          0 = default, write everything to resulting SBOM")
+        print("                          1 = resulting SBOM shows only components that were found")
+        print("                          2 = resulting SBOM shows only components that were not found")
         print("    --dbx                 relaxed Debian version handling: *completely* ignore Debian revision,")
         print("                          so SBOM version 3.1 will match SW360 version 3.1-3.debian")
-        print("    -all                  also report matches for name, but different version")
 
     def run(self, args):
         """Main method()"""
         if args.debug:
             global LOG
             LOG = capycli.get_logger(__name__)
         else:
@@ -946,17 +934,14 @@
         if args.dbx:
             print_text("Using relaxed debian version checks")
             self.relaxed_debian_parsing = True
 
         if args.mode:
             self.mode = args.mode
 
-        if args.all:
-            self.no_match_by_name_only = False
-
         print_text("Loading SBOM file", args.inputfile)
         try:
             sbom = CaPyCliBom.read_sbom(args.inputfile)
         except Exception as ex:
             print_red("Error reading input SBOM file: " + repr(ex))
             sys.exit(ResultCode.RESULT_ERROR_READING_BOM)
         if self.verbosity > 1:
@@ -1018,18 +1003,18 @@
         overview = self.create_overview(result)
         if args.create_overview:
             print_text(" Creating result overview " + args.create_overview)
             self.write_overview(overview, args.create_overview)
 
         if args.outputfile:
             print_text("Writing updated SBOM to " + args.outputfile)
-            if self.mode == MapMode.FOUND:
+            if self.mode == self.MAP_MODE_FOUND:
                 print_yellow(
                     "   Resulting SBOM contains only components were a full natch was found")
-            if self.mode == MapMode.NOT_FOUND:
+            if self.mode == self.MAP_MODE_NOT_FOUND:
                 print_yellow(
                     "   Resulting SBOM contains only components were no match was found")
             new_bom = self.create_updated_bom(sbom, result)
             try:
                 # set Siemens Standard BOM version
                 new_bom.metadata.tools.add(SbomCreator.get_standard_bom_tool())
                 SbomWriter.write_to_json(new_bom, args.outputfile, True)
@@ -1041,14 +1026,14 @@
 
         if args.write_mapresult:
             print_text(" Creating mapping result file " + args.write_mapresult)
             self.write_mapping_result(result, args.write_mapresult)
 
         if overview["OverallResult"] != "COMPLETE":
             print_yellow("No unique mapping found - manual action needed!\n")
-            if self.mode == MapMode.ALL:
+            if self.mode == self.MAP_MODE_ALL:
                 sys.exit(ResultCode.RESULT_NO_UNIQUE_MAPPING)
             else:
                 sys.exit(ResultCode.RESULT_INCOMPLETE_MAPPING)
 
         print_text()
         print_text("done.")
```

### Comparing `capycli-2.0.0/capycli/bom/merge_bom.py` & `capycli-2.0.0.dev8/capycli/bom/merge_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/bom/plaintext.py` & `capycli-2.0.0.dev8/capycli/bom/plaintext.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # Copyright (c) 2023 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
-from typing import List
-
 from cyclonedx.model.component import Component
 
 from capycli import LOG
 from capycli.main.exceptions import CaPyCliException
 
 # -------------------------------------
 # Expected File Format
@@ -24,15 +22,15 @@
 # wheel, 0.34.2
 # tomli, 2.0.1
 # -------------------------------------
 
 
 class PlainTextSupport():
     @classmethod
-    def flatlist_to_cdx_components(cls, inputfile: str) -> List[Component]:
+    def flatlist_to_cdx_components(cls, inputfile: str) -> list[Component]:
         """Convert a flat list of components to a list
         of CycloneDX components."""
         bom = []
         LOG.debug(f"Reading from file {inputfile}")
         try:
             with open(inputfile, encoding="utf-8") as fin:
                 for line in fin:
@@ -53,15 +51,15 @@
         except Exception as exp:
             raise CaPyCliException("Error reading text file: " + str(exp))
 
         LOG.debug("done")
         return bom
 
     @classmethod
-    def write_cdx_components_as_flatlist(cls, bom: List[Component], outputfile: str) -> None:
+    def write_cdx_components_as_flatlist(cls, bom: list[Component], outputfile: str) -> None:
         LOG.debug(f"Writing to file {outputfile}")
         try:
             with open(outputfile, "w", encoding="utf-8") as fout:
                 for cx_comp in bom:
                     name = cx_comp.name
                     version = cx_comp.version
                     fout.write(f"{name}, {version}\n")
```

### Comparing `capycli-2.0.0/capycli/bom/show_bom.py` & `capycli-2.0.0.dev8/capycli/bom/show_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/capycli_bom_support.py` & `capycli-2.0.0.dev8/capycli/common/capycli_bom_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import os
 import tempfile
 import uuid
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional
+from typing import Any, Iterable, Optional
 
 from cyclonedx.model import (
     AttachedText,
     ExternalReference,
     ExternalReferenceType,
     HashAlgorithm,
     HashType,
@@ -50,15 +50,15 @@
     SBOM = 1
     # Legacy-cx format
     LEGACY_CX = 2
 
 
 class SbomJsonParser(BaseParser):
     """Parser to read a CycloneDX SBOM from a JSON file."""
-    def __init__(self, json_content: Dict[str, Any], mode: ParserMode = ParserMode.SBOM):
+    def __init__(self, json_content: dict[str, Any], mode: ParserMode = ParserMode.SBOM):
         super().__init__()
         LOG.debug("Processing CycloneDX data...")
         self.parser_mode = mode
         self.metadata = self.read_metadata(json_content.get("metadata"))
         serial_number = json_content.get("serialNumber", None)
         self.serial_number = uuid.UUID(serial_number) \
             if self.is_valid_serial_number(serial_number) \
@@ -82,15 +82,15 @@
     def link_dependencies_to_project(self, bom: Bom) -> None:
         if not self.metadata.component:
             return
 
         for component in self._components:
             bom.metadata.component.dependencies.add(component.bom_ref)
 
-    def get_tools(self) -> List[Tool]:
+    def get_tools(self) -> list[Tool]:
         """Get the list of tools read by the parser."""
         return self.metadata.tools
 
     def get_metadata_licenses(self) -> SortedSet:
         """Get the metadata licenses read by the parser."""
         return self.metadata.licenses
 
@@ -100,15 +100,15 @@
 
     def is_valid_serial_number(self, serial_number: str) -> bool:
         if not serial_number:
             return False
 
         return not (serial_number is None or "urn:uuid:None" == serial_number)
 
-    def read_tools(self, param: Iterable[Dict[str, Any]]) -> Optional[Iterable[Tool]]:
+    def read_tools(self, param: Iterable[dict[str, Any]]) -> Optional[Iterable[Tool]]:
         if not param:
             return None
 
         LOG.debug("CycloneDX: reading tools")
         tools = []
         for tool in param:
             tools.append(Tool(
@@ -132,28 +132,28 @@
 
     def read_url(self, param: str) -> Optional[XsUri]:
         if not param:
             return None
 
         return XsUri(uri=param)
 
-    def read_license(self, param: Dict[str, Any]) -> Optional[License]:
+    def read_license(self, param: dict[str, Any]) -> Optional[License]:
         if not param:
             return None
 
         text = param.get("text", None)
         license_text = AttachedText(content=text) if text else None
         return License(
             spdx_license_id=param.get("id", None),
             license_name=param.get("name", None),
             license_text=license_text,
             license_url=self.read_url(param.get("url", None)),
         )
 
-    def read_licenses(self, param: Iterable[Dict[str, Any]]) -> Optional[Iterable[LicenseChoice]]:
+    def read_licenses(self, param: Iterable[dict[str, Any]]) -> Optional[Iterable[LicenseChoice]]:
         if not param:
             return None
 
         licenses = []
         for entry in param:
             lic = self.read_license(entry.get("license", None))
             if lic:
@@ -181,27 +181,27 @@
                 metadata.timestamp = timestamp
         metadata.tools = self.read_tools(param.get("tools", None))
         return metadata
 
     def read_hash_algorithm(self, param: Any) -> HashAlgorithm:
         return HashAlgorithm(param)
 
-    def read_hashes(self, hashes: Iterable[Dict[str, Any]]) -> Optional[Iterable[HashType]]:
+    def read_hashes(self, hashes: Iterable[dict[str, Any]]) -> Optional[Iterable[HashType]]:
         if not hashes:
             return None
 
         hash_types = []
         for entry in hashes:
             if entry["alg"]:
                 hash_types.append(HashType(
                     algorithm=self.read_hash_algorithm(entry["alg"]),
                     hash_value=entry["content"]))
         return hash_types
 
-    def read_properties(self, values: Iterable[Dict[str, Any]]) -> Optional[Iterable[Property]]:
+    def read_properties(self, values: Iterable[dict[str, Any]]) -> Optional[Iterable[Property]]:
         if not values:
             return None
 
         LOG.debug("CycloneDX: reading properties")
         properties = []
         for entry in values:
             if self.parser_mode == ParserMode.LEGACY_CX:
@@ -211,30 +211,30 @@
                 properties.append(Property(name=entry["name"], value=entry["value"]))
 
         return properties
 
     def read_external_reference_type(self, value: Any) -> ExternalReferenceType:
         return ExternalReferenceType(value)
 
-    def read_external_references(self, values: Iterable[Dict[str, Any]]) -> Optional[Iterable[ExternalReference]]:
+    def read_external_references(self, values: Iterable[dict[str, Any]]) -> Optional[Iterable[ExternalReference]]:
         if not values:
             return None
 
         ex_refs = []
         for entry in values:
             if entry.get("type"):
                 ex_refs.append(ExternalReference(
                     reference_type=self.read_external_reference_type(entry.get("type")),
                     url=entry.get("url", None),
                     comment=entry.get("comment"),
                     hashes=self.read_hashes(entry.get("hashes", []))
                 ))
         return ex_refs
 
-    def read_component(self, entry: Dict[str, Any]) -> Optional[Component]:
+    def read_component(self, entry: dict[str, Any]) -> Optional[Component]:
         if not entry:
             return None
 
         name = entry.get("name", None)
         version = entry.get("version")
         LOG.debug(f"CycloneDX: reading component {name}, {version}")
         return Component(
@@ -472,15 +472,15 @@
         """Adds the given Siemes Standard BOM profile."""
         prop = Property(
             name=CycloneDxSupport.CDX_PROP_PROFILE,
             value=profile)
         sbom.metadata.properties.add(prop)
 
     @staticmethod
-    def create(bom: List[Component], **kwargs: bool) -> Bom:
+    def create(bom: list[Component], **kwargs: bool) -> Bom:
         sbom = Bom()
 
         if not sbom.metadata.properties:
             sbom.metadata.properties = SortedSet()
 
         if not sbom.metadata.licenses:
             sbom.metadata.licenses = SortedSet()
@@ -614,15 +614,15 @@
             SbomCreator.add_profile(sbom, "capycli")
             SbomWriter.write_to_json(sbom, outputfile, pretty_print=True)
         except Exception as exp:
             raise CaPyCliException("Error writing CaPyCLI file: " + str(exp))
         LOG.debug("done")
 
     @classmethod
-    def write_simple_sbom(cls, bom: List[Component], outputfile: str) -> None:
+    def write_simple_sbom(cls, bom: list[Component], outputfile: str) -> None:
         LOG.debug(f"Writing to file {outputfile}")
         try:
             creator = SbomCreator()
             sbom = creator.create(bom, addlicense=True, addprofile=True, addtools=True)
             SbomWriter.write_to_json(sbom, outputfile, pretty_print=True)
         except Exception as exp:
             raise CaPyCliException("Error writing CaPyCLI file: " + str(exp))
```

### Comparing `capycli-2.0.0/capycli/common/comparable_version.py` & `capycli-2.0.0.dev8/capycli/common/comparable_version.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/component_cache.py` & `capycli-2.0.0.dev8/capycli/common/component_cache.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/dependencies_base.py` & `capycli-2.0.0.dev8/capycli/common/dependencies_base.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/file_support.py` & `capycli-2.0.0.dev8/capycli/common/file_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/html_support.py` & `capycli-2.0.0.dev8/capycli/common/html_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/json_support.py` & `capycli-2.0.0.dev8/capycli/common/json_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/map_result.py` & `capycli-2.0.0.dev8/capycli/common/map_result.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/print.py` & `capycli-2.0.0.dev8/capycli/common/print.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/purl_service.py` & `capycli-2.0.0.dev8/capycli/common/purl_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -------------------------------------------------------------------------------
 # Copyright (c) 2022-2023 Siemens
 # All Rights Reserved.
-# Author: rayk.bajohr@siemens.com, thomas.graf@siemens.com
+# Author: rayk.bajohr@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # ----------
 
 import packageurl
 from sw360 import SW360
```

### Comparing `capycli-2.0.0/capycli/common/purl_store.py` & `capycli-2.0.0.dev8/capycli/common/purl_store.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/purl_utils.py` & `capycli-2.0.0.dev8/capycli/common/purl_utils.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/script_base.py` & `capycli-2.0.0.dev8/capycli/common/script_base.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/common/script_support.py` & `capycli-2.0.0.dev8/capycli/common/script_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/dependencies/handle_dependencies.py` & `capycli-2.0.0.dev8/capycli/dependencies/handle_dependencies.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/dependencies/javascript.py` & `capycli-2.0.0.dev8/capycli/dependencies/javascript.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/dependencies/maven_list.py` & `capycli-2.0.0.dev8/capycli/dependencies/maven_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # -------------------------------------------------------------------------------
 
 import os
 import re
 import subprocess
 import sys
 import xml.etree.ElementTree as ET
-from typing import List, Tuple
 
 import requests
 from cyclonedx.model import ExternalReference, ExternalReferenceType, Property
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component
 from packageurl import PackageURL
 
@@ -30,16 +29,16 @@
 
 class GetJavaMavenTreeDependencies(capycli.common.dependencies_base.DependenciesBase):
     SOURCES_REGEX = r'.*Downloading.+(https://?[-a-zA-Z0-9@:%._+~#=/]{1,256}-(source|sources).jar).*'
     BINARIES_REGEX = r'.*Downloaded.+(https://?[-a-zA-Z0-9@:%._+~#=/]{1,256}.jar).*'
 
     def add_urls(
             self, cx_comp: Component,
-            parsed_sources: List, parsed_binaries: List,
-            source_files: List[str], binary_files: List[str], files_directory: str):
+            parsed_sources: list, parsed_binaries: list,
+            source_files: list[str], binary_files: list[str], files_directory: str):
         """
         Adds URLs to corresponding bom item. This is done by checking if a dependency
         with the corresponding naming exists inside the list of parsed URLs and also
         inside the download folder
 
         :param bomitem: a single bom item
         :param parsed_sources: a list of sources URLs
@@ -95,15 +94,15 @@
         parsed_urls = []
 
         lines = open(download_output_file).read().split("\n")
         for line in lines:
             parts = re.findall(regex, line)
             if parts and len(parts) > 0:
                 url = parts[0]
-                if isinstance(url, Tuple):
+                if isinstance(url, tuple):
                     url = url[0]
                 if url not in parsed_urls:
                     parsed_urls.append(url)
 
         return parsed_urls
 
     def find_package_info(self, binary_file_url):
```

### Comparing `capycli-2.0.0/capycli/dependencies/maven_pom.py` & `capycli-2.0.0.dev8/capycli/dependencies/maven_pom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/dependencies/nuget.py` & `capycli-2.0.0.dev8/capycli/dependencies/nuget.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/main/application.py` & `capycli-2.0.0.dev8/capycli/main/application.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/main/argument_parser.py` & `capycli-2.0.0.dev8/capycli/main/argument_parser.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/main/cli.py` & `capycli-2.0.0.dev8/capycli/main/cli.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/main/options.py` & `capycli-2.0.0.dev8/capycli/main/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 import os
 
 import tomli
 
 import capycli
 from capycli.bom.bom_convert import BomFormat
-from capycli.bom.map_bom import MapMode
 from capycli.main.argument_parser import ArgumentParser
 
 LOG = capycli.get_logger(__name__)
 
 
 class CommandlineSupport():
     CONFIG_FILE_NAME = ".capycli.cfg"
@@ -109,19 +108,14 @@
         output_formats.append(BomFormat.CAPYCLI)
         output_formats.append(BomFormat.SBOM)
         output_formats.append(BomFormat.TEXT)
         output_formats.append(BomFormat.CSV)
         output_formats.append(BomFormat.LEGACY)
         output_formats.append(BomFormat.HTML)
 
-        map_modes = []
-        map_modes.append(MapMode.ALL)
-        map_modes.append(MapMode.FOUND)
-        map_modes.append(MapMode.NOT_FOUND)
-
         self.parser.add_argument(
             "-i",
             "--inputfile",
             dest="inputfile",
             help="input file to read from",
         )
 
@@ -339,15 +333,14 @@
             help="force a specific exit code",
         )
 
         # used by MapBom
         self.parser.add_argument(
             "-m",
             "--mode",
-            choices=map_modes,
             dest="mode",
             help="specific mode for some commands",
         )
 
         # used by bom convert
         self.parser.add_argument(
             "-if",
```

### Comparing `capycli-2.0.0/capycli/main/result_codes.py` & `capycli-2.0.0.dev8/capycli/main/result_codes.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/mapping/handle_mapping.py` & `capycli-2.0.0.dev8/capycli/mapping/handle_mapping.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/mapping/mapping_to_html.py` & `capycli-2.0.0.dev8/capycli/mapping/mapping_to_html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/mapping/mapping_to_xlsx.py` & `capycli-2.0.0.dev8/capycli/mapping/mapping_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/moverview/handle_moverview.py` & `capycli-2.0.0.dev8/capycli/moverview/handle_moverview.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/moverview/moverview_to_html.py` & `capycli-2.0.0.dev8/capycli/moverview/moverview_to_html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/moverview/moverview_to_xlsx.py` & `capycli-2.0.0.dev8/capycli/moverview/moverview_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/check_prerequisites.py` & `capycli-2.0.0.dev8/capycli/project/check_prerequisites.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/create_bom.py` & `capycli-2.0.0.dev8/capycli/project/create_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/create_project.py` & `capycli-2.0.0.dev8/capycli/project/create_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 import logging
 import os
 import sys
-from typing import List
 
 import requests
 import sw360
 from cyclonedx.model.bom import Bom
 
 import capycli.common.script_base
 from capycli import get_logger
@@ -28,15 +27,15 @@
     """
     Create or update a project on SW360.
     """
 
     def __init__(self, onlyUpdateProject=False):
         self.onlyUpdateProject = onlyUpdateProject
 
-    def bom_to_release_list(self, sbom: Bom) -> List[str]:
+    def bom_to_release_list(self, sbom: Bom) -> list[str]:
         """Creates a list with linked releases"""
         linkedReleases = []
 
         for cx_comp in sbom.components:
             rid = CycloneDxSupport.get_property_value(cx_comp, CycloneDxSupport.CDX_PROP_SW360ID)
             if not rid:
                 print_red(
```

### Comparing `capycli-2.0.0/capycli/project/create_readme.py` & `capycli-2.0.0.dev8/capycli/project/create_readme.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/find_project.py` & `capycli-2.0.0.dev8/capycli/project/find_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/get_license_info.py` & `capycli-2.0.0.dev8/capycli/project/get_license_info.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/handle_project.py` & `capycli-2.0.0.dev8/capycli/project/handle_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/show_ecc.py` & `capycli-2.0.0.dev8/capycli/project/show_ecc.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/show_licenses.py` & `capycli-2.0.0.dev8/capycli/project/show_licenses.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/show_project.py` & `capycli-2.0.0.dev8/capycli/project/show_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/capycli/project/show_vulnerabilities.py` & `capycli-2.0.0.dev8/capycli/project/show_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/License.md` & `capycli-2.0.0.dev8/License.md`

 * *Files identical despite different names*

### Comparing `capycli-2.0.0/pyproject.toml` & `capycli-2.0.0.dev8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 # SPDX-FileCopyrightText: (c) 2018-2023 Siemens
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
 name = "capycli"
-version = "2.0.0"
+version = "2.0.0.dev8"
 description = "CaPyCli - Clearing Automation Python Command Line Interface"
 authors = ["Thomas Graf <thomas.graf@siemens.com>"]
 license = "MIT"
 readme="Readme.md"
-repository = "https://github.com/sw360/capycli"
-homepage = "https://github.com/sw360/capycli"
-keywords = ["sw360", "cli, automation", "license", "compliance", "clearing"]
 include = [
     "LICENSE.md",
     { path = "capycli/data/granularity_list.csv", format = "wheel" },
     { path = "capycli/data/__init__.py", format = "wheel" },
     { path = "capycli/data/granularity_list.csv", format = "sdist" },
     { path = "capycli/data/__init__.py", format = "sdist" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
 ]
+repository = "https://github.com/sw360/capycli"
+homepage = "https://github.com/sw360/capycli"
 
 
 [tool.poetry.urls]
 issues = "https://github.com/sw360/capycli/issues"
 
 [tool.poetry.scripts]
 capycli = "capycli.main.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8" # drop support for 3.6 and 3.7 because of wheel and cli-support
 colorama = "^0.4.3"
-requests = "^2.31.0" # fix CVE-2023-32681 
+requests = "^2.22.0"
 packageurl-python = ">0.8, <1.0"
 pyjwt = "^1.7.1"
 openpyxl = "^3.0.3"
 requirements-parser = "^0.2.0"
 sw360 = "^1.2.0"
 wheel = "^0.38.4"
 cli-support = "^1.3"
 chardet = "^3.0.4"
 cyclonedx-python-lib = ">3.1.1"
 cyclonedx-bom = "^3.11.0"
 tomli = "^2.0.1"
 dateparser = "^1.1.8"
 urllib3 = "1.26.15"
-importlib-resources = "^5.12.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = ">=3.7.8"
 coverage = "^5.4"
 responses = "^0.17.0"
 pytest = "^7.2.2"
 vcrpy = "^4.1.1"
```

### Comparing `capycli-2.0.0/Readme.md` & `capycli-2.0.0.dev8/Readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,25 @@
 <!--
 # SPDX-FileCopyrightText: (c) 2018-2023 Siemens
 # SPDX-License-Identifier: MIT
 -->
 
 ![Header_Image](images/Github-social-capycli.png)
 
-# CaPyCli - Clearing Automation Python Command Line Tool for SW360
+# CaPyCli - Clearing Automation Python Command Line Tool
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sw360/capycli/blob/main/License.md)
-[![PyPI](https://shields.io/pypi/v/capycli)](https://pypi.org/project/capycli/)
-[![Python Version](https://img.shields.io/badge/python-3.8%2C3.9%2C3.10%2C3.11-yellow?logo=python)](https://www.python.org/doc/versions/)
+[![Python Version](https://img.shields.io/badge/python-3.8%2C3.7%2C3.9%2C3.10-yellow?logo=python)](https://www.python.org/doc/versions/)
 [![Static Checks](https://github.com/sw360/capycli/actions/workflows/static-checks.yml/badge.svg)](https://github.com/sw360/capycli/actions/workflows/static-checks.yml)
 [![Unit Tests](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/tngraf/c8f15831ecdcf6e86ab2b69cbb2d4f89/raw/df1a91c074c5ee34dc1f0dcf82bc0e76e39b5b4e/capycli-cobertura-coverage.json&color=green)](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml)
 [![SBOM](https://img.shields.io/badge/SBOM-CycloneDX-brightgreen)](https://github.com/tngraf/Tethys.Dgml/blob/master/SBOM/sbom.cyclonedx.xml)
 [![REUSE status](https://api.reuse.software/badge/git.fsfe.org/reuse/api)](https://api.reuse.software/info/git.fsfe.org/reuse/api)
 
-Python 3 scripts to allow license clearing automation using the
-[SW360](https://github.com/eclipse/sw360) software catalogue.
-
-## What is SW360?
-
-[SW360](https://github.com/eclipse/sw360) is a software component catalogue application designed to
-provide a central place for sharing information about software components used by an organization.
-It is designed to neatly integrate into existing infrastructures related to the management of
-software artifacts and projects by providing separate backend services for distinct tasks and a set
-of portlets to access these services. A complete deployment unit exists (vagrant box or docker
-container) that contains a complete configuration of all services and portlets.
-
-Companies like Cariad, Siemens or Toshiba use SW360 to track their use of third party software components.
-
-## Why CaPyCli?
-
-SW360 is for software developers and software developers love to automate tasks. The SW360 user
-interface is nice if you want to check a project or search for a single component. But if you have
-a project with a JavaScript frontend and hundreds of components, you do not want to add all of them
-manually. You want to be able to determine your software bill of materials (SBOM) and you want to
-map this SBOM to the information that is already available of SW360.
-
-CaPyCli allows you to
-
-* determine your list of dependencies, your software bill of materials (SBOM)
-* determine meta-data for the SBOM items and download source files
-* map an SBOM to the data available on SW360
-* create all missing components and releases
-* create a project that contains all releases of your SBOM
-* track the progress on license compliance checks
-* show information about the project and its releases
-* show information about export control information and security vulnerabilities (if tracked via SW360)
+Python 3 scripts to allow clearing automation.
 
 ## Basic Syntax
 
 ```code
 CaPyCli command [sub-command...] [options]
 
 Commands and Sub-Commands
@@ -165,15 +133,15 @@
 
 If you are using pipenv, you can create the `requirements.txt` file via
 
 ```sh
 pipenv lock -r > requirements.txt
 ```
 
-If your dependencies are defined in `setup.py` you may take a look at
+If your dependencies are defined in `setup,py` you may take a look at
 https://dephell.readthedocs.io/cmd-deps-convert.html or
 https://github.com/jazzband/pip-tools#example-usage-for-pip-compile to generate
 a `requirements.txt` file.
 
 Probably the best solution is if you enhance CaPyCli to support poetry, pipenv or setup.py
 directly and open a merge request.
```

### Comparing `capycli-2.0.0/setup.py` & `capycli-2.0.0.dev8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,268 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: capycli
+Version: 2.0.0.dev8
+Summary: CaPyCli - Clearing Automation Python Command Line Interface
+Home-page: https://github.com/sw360/capycli
+License: MIT
+Author: Thomas Graf
+Author-email: thomas.graf@siemens.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: chardet (>=3.0.4,<4.0.0)
+Requires-Dist: cli-support (>=1.3,<2.0)
+Requires-Dist: colorama (>=0.4.3,<0.5.0)
+Requires-Dist: cyclonedx-bom (>=3.11.0,<4.0.0)
+Requires-Dist: cyclonedx-python-lib (>3.1.1)
+Requires-Dist: dateparser (>=1.1.8,<2.0.0)
+Requires-Dist: openpyxl (>=3.0.3,<4.0.0)
+Requires-Dist: packageurl-python (>0.8,<1.0)
+Requires-Dist: pyjwt (>=1.7.1,<2.0.0)
+Requires-Dist: requests (>=2.22.0,<3.0.0)
+Requires-Dist: requirements-parser (>=0.2.0,<0.3.0)
+Requires-Dist: sw360 (>=1.2.0,<2.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: urllib3 (==1.26.15)
+Requires-Dist: wheel (>=0.38.4,<0.39.0)
+Project-URL: Repository, https://github.com/sw360/capycli
+Project-URL: issues, https://github.com/sw360/capycli/issues
+Description-Content-Type: text/markdown
 
-packages = \
-['capycli',
- 'capycli.bom',
- 'capycli.common',
- 'capycli.data',
- 'capycli.dependencies',
- 'capycli.main',
- 'capycli.mapping',
- 'capycli.moverview',
- 'capycli.project']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['chardet>=3.0.4,<4.0.0',
- 'cli-support>=1.3,<2.0',
- 'colorama>=0.4.3,<0.5.0',
- 'cyclonedx-bom>=3.11.0,<4.0.0',
- 'cyclonedx-python-lib>3.1.1',
- 'dateparser>=1.1.8,<2.0.0',
- 'importlib-resources>=5.12.0,<6.0.0',
- 'openpyxl>=3.0.3,<4.0.0',
- 'packageurl-python>0.8,<1.0',
- 'pyjwt>=1.7.1,<2.0.0',
- 'requests>=2.31.0,<3.0.0',
- 'requirements-parser>=0.2.0,<0.3.0',
- 'sw360>=1.2.0,<2.0.0',
- 'tomli>=2.0.1,<3.0.0',
- 'urllib3==1.26.15',
- 'wheel>=0.38.4,<0.39.0']
-
-entry_points = \
-{'console_scripts': ['capycli = capycli.main.cli:main']}
-
-setup_kwargs = {
-    'name': 'capycli',
-    'version': '2.0.0',
-    'description': 'CaPyCli - Clearing Automation Python Command Line Interface',
-    'long_description': '<!--\n# SPDX-FileCopyrightText: (c) 2018-2023 Siemens\n# SPDX-License-Identifier: MIT\n-->\n\n![Header_Image](images/Github-social-capycli.png)\n\n# CaPyCli - Clearing Automation Python Command Line Tool for SW360\n\n[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sw360/capycli/blob/main/License.md)\n[![PyPI](https://shields.io/pypi/v/capycli)](https://pypi.org/project/capycli/)\n[![Python Version](https://img.shields.io/badge/python-3.8%2C3.9%2C3.10%2C3.11-yellow?logo=python)](https://www.python.org/doc/versions/)\n[![Static Checks](https://github.com/sw360/capycli/actions/workflows/static-checks.yml/badge.svg)](https://github.com/sw360/capycli/actions/workflows/static-checks.yml)\n[![Unit Tests](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml)\n[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/tngraf/c8f15831ecdcf6e86ab2b69cbb2d4f89/raw/df1a91c074c5ee34dc1f0dcf82bc0e76e39b5b4e/capycli-cobertura-coverage.json&color=green)](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml)\n[![SBOM](https://img.shields.io/badge/SBOM-CycloneDX-brightgreen)](https://github.com/tngraf/Tethys.Dgml/blob/master/SBOM/sbom.cyclonedx.xml)\n[![REUSE status](https://api.reuse.software/badge/git.fsfe.org/reuse/api)](https://api.reuse.software/info/git.fsfe.org/reuse/api)\n\nPython 3 scripts to allow license clearing automation using the\n[SW360](https://github.com/eclipse/sw360) software catalogue.\n\n## What is SW360?\n\n[SW360](https://github.com/eclipse/sw360) is a software component catalogue application designed to\nprovide a central place for sharing information about software components used by an organization.\nIt is designed to neatly integrate into existing infrastructures related to the management of\nsoftware artifacts and projects by providing separate backend services for distinct tasks and a set\nof portlets to access these services. A complete deployment unit exists (vagrant box or docker\ncontainer) that contains a complete configuration of all services and portlets.\n\nCompanies like Cariad, Siemens or Toshiba use SW360 to track their use of third party software components.\n\n## Why CaPyCli?\n\nSW360 is for software developers and software developers love to automate tasks. The SW360 user\ninterface is nice if you want to check a project or search for a single component. But if you have\na project with a JavaScript frontend and hundreds of components, you do not want to add all of them\nmanually. You want to be able to determine your software bill of materials (SBOM) and you want to\nmap this SBOM to the information that is already available of SW360.\n\nCaPyCli allows you to\n\n* determine your list of dependencies, your software bill of materials (SBOM)\n* determine meta-data for the SBOM items and download source files\n* map an SBOM to the data available on SW360\n* create all missing components and releases\n* create a project that contains all releases of your SBOM\n* track the progress on license compliance checks\n* show information about the project and its releases\n* show information about export control information and security vulnerabilities (if tracked via SW360)\n\n## Basic Syntax\n\n```code\nCaPyCli command [sub-command...] [options]\n\nCommands and Sub-Commands\n    getdependencies     dependency detection specific commands\n        Nuget             determine dependencies for a .Net/Nuget project\n        Python            determine dependencies for a Python project\n        Javascript        determine dependencies for a JavaScript project\n        MavenPom          determine dependencies for a Java/Maven project using the pom.xml file\n        MavenList         determine dependencies for a Java/Maven project using a Maven command\n\n    bom                 bill of material (SBOM) specific commands\n        Show              display contents of a SBOM\n        Convert           convert SBOM formats\n        Filter            apply filter file to a SBOM\n        Check             check that all releases in the SBOM exist on target SW360 instance\n        CheckItemStatus   show additional information about SBOM items on SW360\n        Map               map a given SBOM to data on SW360\n        CreateReleases    create new releases for existing components on SW360\n        CreateComponents  create new components and releases on SW360 (use with care!)\n        DownloadSources   download source files from the URL specified in the SBOM\n        Granularity       check a bill of material for potential component granularity issues\n        Diff              compare two bills of material.\n        Merge             merge two bills of material.\n        Findsources       determine the source code for SBOM items.\n\n    mapping\n        ToHtml            create a HTML page showing the mapping result\n        ToXlsx            create an Excel sheet showing the mapping result\n\n    moverview\n        ToHtml            create a HTML page showing the mapping result overview\n        ToXlsx            create an Excel sheet showing the mapping result overview\n\n    project\n        Find              find a project by name\n        Prerequisites     checks whether all prerequisites for a successfull\n                          software clearing are fulfilled\n        Show              show project details\n        Licenses          show licenses of all cleared compponents\n        Create            create or update a project on SW360\n        Update            update an exiting project, preserving linked releases\n        GetLicenseInfo    get license info of all project components\n        CreateReadme      create a Readme_OSS\n        Vulnerabilities   show security vulnerabilities of a project\n        ECC               Show export control status of a project\n\nOptions:\n  command                                           command and subcommand to process\n  -h, --help                                        show a help message and exit\n  -i INPUTFILE, --inputfile INPUTFILE               input file to read from\n  -ri RAW_INPUT, --raw-input RAW_INPUT              raw data input file to parse repository urls\n  -o OUTPUTFILE, --outputfile OUTPUTFILE            output file to write to\n  -filterfile FILTERFILE                            filter file to use\n  -v VERBOSE                                        be verbose\n  -t SW360_TOKEN, --token SW360_TOKEN               use this token for access to SW360\n  -oa, --oauth2                                     this is an oauth2 token\n  -url SW360_URL                                    use this URL for access to SW360\n  --nocache NOCACHE                                 do not use component cache\n  -cf CACHEFILE, --cachefile CACHEFILE              cache file name to use\n  -rc REFRESH_CACHE, --refresh_cache REFRESH_CACHE  refresh component cache\n  -sc, --similar                                    look for components with similar name\n  -ov CREATE_OVERVIEW, --overview CREATE_OVERVIEW   create an mapping overview JSON file\n  -mr WRITE_MAPRESULT, --mapresult WRITE_MAPRESULT  create a JSON file with the mapping details\n  -name                                             name of the project\n  -version                                          version of the project\n  -id ID                                            SW360 id of the project, supersedes name and \n                                                    version parameters\n  -ncli NCLI, --no-overwrite-cli NCLI               do not overwrite existing CLI files\n  -nconf NCONF, --no-overwrite-config NCONF         do not overwrite an existing configuration file\n  -dest DESTINATION, --destination DESTINATION      the destination folder\n  -source SOURCE                                    source folder or additional source file\n  --dbx DBX                                         relaxed handling of debian version numbers\n  --download                                        enable automatic download of missing sources\n  --search-meta-data SEARCH_META_DATA               search for component meta-data\n  -old-version OLD_VERSION                          previous version\n  -ex                                               show exit code\n  -rr RESULT_REQUIRED                               there must be a clearing result available\n  -xml XML                                          use XML format\n  -package-source PACKAGE_SOURCE                    URL of the package manager to use\n  -all                                              show/use all items\n  -format FORMAT                                    format to use (text, json, xml)\n  -fe FORCE_EXIT, --forceexit FORCE_EXIT            force a specific exit code\n  -m MODE, --mode MODE                              specific mode for some commands\n  -if INPUTFORMAT                                   Specify input file format\n  -of OUTPUTFORMAT                                  Specify output file format\n  -X DEBUG                                          Enable debug output\n```\n\n## Use Cases\n\nOver the time we implemented more and more commands with more and more parameters.  \nWe understand that it is hard for beginners to find the right command for the task\nthey want to do. Have a look at our [Use Case Overview](UseCaseOverview.md).\n\n## Software Clearing Approaches\n\nFrom time to time there are questions **why** a command has been implemented in this\nspecific way or why a command exists at all. Not all organization have the same\napproach when doing license compliance. Have a look at our\n[Software Clearing Approach Overview](SoftwareClearingApproachOverview.md) to see our\napproaches.\n\n## Note about Python Dependency Detection\n\nAt the moment there is only support for dependencies defined in a `requirements.txt` file.  \nPoetry users can create the `requirements.txt` file via\n\n```sh\npoetry export --format requirements.txt -o requirements.txt --without-hashes\n```\n\nIf you are using pipenv, you can create the `requirements.txt` file via\n\n```sh\npipenv lock -r > requirements.txt\n```\n\nIf your dependencies are defined in `setup.py` you may take a look at\nhttps://dephell.readthedocs.io/cmd-deps-convert.html or\nhttps://github.com/jazzband/pip-tools#example-usage-for-pip-compile to generate\na `requirements.txt` file.\n\nProbably the best solution is if you enhance CaPyCli to support poetry, pipenv or setup.py\ndirectly and open a merge request.\n\n## Examples\n\n### Find project by name\n\nCommand:\n\n```sh\ncapycli project find -name "tr-card"\n- or -\npython -m capycli project find -name tr-card\n```\n\nResult\n\n```sh\nCaPyCli - Find a project by name\n\n  Searching for projects by name\n    TR-Card, 1.0 => ID = ff697cd18fe178b26fc601b60e00fcdf\n```\n\nMore examples and usage notes can be found in [examples.md](examples.md).\n\n## Prerequisites\n\n* Python 3\n* A SW360 read (and write) token, see next section.\n\n## API Access\n\nAccess to the SW360 REST API requires an access token.\nThe token can be requested on SW360/Preferences/REST API Token.\n\nThe scripts in this repository expect, that a valid token\nis stored in the environment variable ``SW360ProductionToken``.\nAlternatively you can specify a token using the `-t` option.\n\nFor proper access to an SW360 instance the correct url must be own.\nThe SW360 url can be specified on the commandline with the `-url`\nparameter, via the environment variable ``SW360ServerUrl`` or in the\nconfig file (`.capycli.cfg`).\n\n## SBOM Format\n\nThe software bill of materials (SBOM) is a crucial information for most operations.\nThere is no common description what a bill of materials should contain.\nThere are different formats available, for example the SBOM of CyCloneDX,\nnevertheless most tools have their own SBOM format.\nWe have decided also to have our own flavor of CycloneDX, see [SBOM](Readme_BOM.md),\nfocused on the information we need to handle components, releases and projects\non SW360. It is a simple JSON format. CaPyCli reads or writes exactly the\ninformation that is needed.\nConversion support from or to our SBOM format is available.\nFor converting CycloneDX (XML) to JSON or for converting SPDX SBOMs, we like\nto refer you to the oepn source tools from [CycloneDX](https://cyclonedx.org/).\n\n## Mapping a SBOM to SW360\n\nSBOM mapping is described in an extra file, see [SBOM Mapping](Readme_Mapping.md).\n\n## Project Management\n\nThis is a Python project managed using ```Poetry```.\n\n## Installation\n\n### From PyPi\n\n* using `pip`:\n\n  ```shell\n  pip install capycli\n  ```\n\n## Copyright & License\n\nCopyright 2018-2023 Siemens\n\nThis program and the accompanying materials are made\navailable under the terms of the MIT License.  \nSPDX-License-Identifier: MIT\n',
-    'author': 'Thomas Graf',
-    'author_email': 'thomas.graf@siemens.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sw360/capycli',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+<!--
+# SPDX-FileCopyrightText: (c) 2018-2023 Siemens
+# SPDX-License-Identifier: MIT
+-->
 
+![Header_Image](images/Github-social-capycli.png)
+
+# CaPyCli - Clearing Automation Python Command Line Tool
+
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sw360/capycli/blob/main/License.md)
+[![Python Version](https://img.shields.io/badge/python-3.8%2C3.7%2C3.9%2C3.10-yellow?logo=python)](https://www.python.org/doc/versions/)
+[![Static Checks](https://github.com/sw360/capycli/actions/workflows/static-checks.yml/badge.svg)](https://github.com/sw360/capycli/actions/workflows/static-checks.yml)
+[![Unit Tests](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/tngraf/c8f15831ecdcf6e86ab2b69cbb2d4f89/raw/df1a91c074c5ee34dc1f0dcf82bc0e76e39b5b4e/capycli-cobertura-coverage.json&color=green)](https://github.com/sw360/capycli/actions/workflows/unit-tests.yml)
+[![SBOM](https://img.shields.io/badge/SBOM-CycloneDX-brightgreen)](https://github.com/tngraf/Tethys.Dgml/blob/master/SBOM/sbom.cyclonedx.xml)
+[![REUSE status](https://api.reuse.software/badge/git.fsfe.org/reuse/api)](https://api.reuse.software/info/git.fsfe.org/reuse/api)
+
+Python 3 scripts to allow clearing automation.
+
+## Basic Syntax
+
+```code
+CaPyCli command [sub-command...] [options]
+
+Commands and Sub-Commands
+    getdependencies     dependency detection specific commands
+        Nuget             determine dependencies for a .Net/Nuget project
+        Python            determine dependencies for a Python project
+        Javascript        determine dependencies for a JavaScript project
+        MavenPom          determine dependencies for a Java/Maven project using the pom.xml file
+        MavenList         determine dependencies for a Java/Maven project using a Maven command
+
+    bom                 bill of material (SBOM) specific commands
+        Show              display contents of a SBOM
+        Convert           convert SBOM formats
+        Filter            apply filter file to a SBOM
+        Check             check that all releases in the SBOM exist on target SW360 instance
+        CheckItemStatus   show additional information about SBOM items on SW360
+        Map               map a given SBOM to data on SW360
+        CreateReleases    create new releases for existing components on SW360
+        CreateComponents  create new components and releases on SW360 (use with care!)
+        DownloadSources   download source files from the URL specified in the SBOM
+        Granularity       check a bill of material for potential component granularity issues
+        Diff              compare two bills of material.
+        Merge             merge two bills of material.
+        Findsources       determine the source code for SBOM items.
+
+    mapping
+        ToHtml            create a HTML page showing the mapping result
+        ToXlsx            create an Excel sheet showing the mapping result
+
+    moverview
+        ToHtml            create a HTML page showing the mapping result overview
+        ToXlsx            create an Excel sheet showing the mapping result overview
+
+    project
+        Find              find a project by name
+        Prerequisites     checks whether all prerequisites for a successfull
+                          software clearing are fulfilled
+        Show              show project details
+        Licenses          show licenses of all cleared compponents
+        Create            create or update a project on SW360
+        Update            update an exiting project, preserving linked releases
+        GetLicenseInfo    get license info of all project components
+        CreateReadme      create a Readme_OSS
+        Vulnerabilities   show security vulnerabilities of a project
+        ECC               Show export control status of a project
+
+Options:
+  command                                           command and subcommand to process
+  -h, --help                                        show a help message and exit
+  -i INPUTFILE, --inputfile INPUTFILE               input file to read from
+  -ri RAW_INPUT, --raw-input RAW_INPUT              raw data input file to parse repository urls
+  -o OUTPUTFILE, --outputfile OUTPUTFILE            output file to write to
+  -filterfile FILTERFILE                            filter file to use
+  -v VERBOSE                                        be verbose
+  -t SW360_TOKEN, --token SW360_TOKEN               use this token for access to SW360
+  -oa, --oauth2                                     this is an oauth2 token
+  -url SW360_URL                                    use this URL for access to SW360
+  --nocache NOCACHE                                 do not use component cache
+  -cf CACHEFILE, --cachefile CACHEFILE              cache file name to use
+  -rc REFRESH_CACHE, --refresh_cache REFRESH_CACHE  refresh component cache
+  -sc, --similar                                    look for components with similar name
+  -ov CREATE_OVERVIEW, --overview CREATE_OVERVIEW   create an mapping overview JSON file
+  -mr WRITE_MAPRESULT, --mapresult WRITE_MAPRESULT  create a JSON file with the mapping details
+  -name                                             name of the project
+  -version                                          version of the project
+  -id ID                                            SW360 id of the project, supersedes name and 
+                                                    version parameters
+  -ncli NCLI, --no-overwrite-cli NCLI               do not overwrite existing CLI files
+  -nconf NCONF, --no-overwrite-config NCONF         do not overwrite an existing configuration file
+  -dest DESTINATION, --destination DESTINATION      the destination folder
+  -source SOURCE                                    source folder or additional source file
+  --dbx DBX                                         relaxed handling of debian version numbers
+  --download                                        enable automatic download of missing sources
+  --search-meta-data SEARCH_META_DATA               search for component meta-data
+  -old-version OLD_VERSION                          previous version
+  -ex                                               show exit code
+  -rr RESULT_REQUIRED                               there must be a clearing result available
+  -xml XML                                          use XML format
+  -package-source PACKAGE_SOURCE                    URL of the package manager to use
+  -all                                              show/use all items
+  -format FORMAT                                    format to use (text, json, xml)
+  -fe FORCE_EXIT, --forceexit FORCE_EXIT            force a specific exit code
+  -m MODE, --mode MODE                              specific mode for some commands
+  -if INPUTFORMAT                                   Specify input file format
+  -of OUTPUTFORMAT                                  Specify output file format
+  -X DEBUG                                          Enable debug output
+```
+
+## Use Cases
+
+Over the time we implemented more and more commands with more and more parameters.  
+We understand that it is hard for beginners to find the right command for the task
+they want to do. Have a look at our [Use Case Overview](UseCaseOverview.md).
+
+## Software Clearing Approaches
+
+From time to time there are questions **why** a command has been implemented in this
+specific way or why a command exists at all. Not all organization have the same
+approach when doing license compliance. Have a look at our
+[Software Clearing Approach Overview](SoftwareClearingApproachOverview.md) to see our
+approaches.
+
+## Note about Python Dependency Detection
+
+At the moment there is only support for dependencies defined in a `requirements.txt` file.  
+Poetry users can create the `requirements.txt` file via
+
+```sh
+poetry export --format requirements.txt -o requirements.txt --without-hashes
+```
+
+If you are using pipenv, you can create the `requirements.txt` file via
+
+```sh
+pipenv lock -r > requirements.txt
+```
+
+If your dependencies are defined in `setup,py` you may take a look at
+https://dephell.readthedocs.io/cmd-deps-convert.html or
+https://github.com/jazzband/pip-tools#example-usage-for-pip-compile to generate
+a `requirements.txt` file.
+
+Probably the best solution is if you enhance CaPyCli to support poetry, pipenv or setup.py
+directly and open a merge request.
+
+## Examples
+
+### Find project by name
+
+Command:
+
+```sh
+capycli project find -name "tr-card"
+- or -
+python -m capycli project find -name tr-card
+```
+
+Result
+
+```sh
+CaPyCli - Find a project by name
+
+  Searching for projects by name
+    TR-Card, 1.0 => ID = ff697cd18fe178b26fc601b60e00fcdf
+```
+
+More examples and usage notes can be found in [examples.md](examples.md).
+
+## Prerequisites
+
+* Python 3
+* A SW360 read (and write) token, see next section.
+
+## API Access
+
+Access to the SW360 REST API requires an access token.
+The token can be requested on SW360/Preferences/REST API Token.
+
+The scripts in this repository expect, that a valid token
+is stored in the environment variable ``SW360ProductionToken``.
+Alternatively you can specify a token using the `-t` option.
+
+For proper access to an SW360 instance the correct url must be own.
+The SW360 url can be specified on the commandline with the `-url`
+parameter, via the environment variable ``SW360ServerUrl`` or in the
+config file (`.capycli.cfg`).
+
+## SBOM Format
+
+The software bill of materials (SBOM) is a crucial information for most operations.
+There is no common description what a bill of materials should contain.
+There are different formats available, for example the SBOM of CyCloneDX,
+nevertheless most tools have their own SBOM format.
+We have decided also to have our own flavor of CycloneDX, see [SBOM](Readme_BOM.md),
+focused on the information we need to handle components, releases and projects
+on SW360. It is a simple JSON format. CaPyCli reads or writes exactly the
+information that is needed.
+Conversion support from or to our SBOM format is available.
+For converting CycloneDX (XML) to JSON or for converting SPDX SBOMs, we like
+to refer you to the oepn source tools from [CycloneDX](https://cyclonedx.org/).
+
+## Mapping a SBOM to SW360
+
+SBOM mapping is described in an extra file, see [SBOM Mapping](Readme_Mapping.md).
+
+## Project Management
+
+This is a Python project managed using ```Poetry```.
+
+## Installation
+
+### From PyPi
+
+* using `pip`:
+
+  ```shell
+  pip install capycli
+  ```
+
+## Copyright & License
+
+Copyright 2018-2023 Siemens
+
+This program and the accompanying materials are made
+available under the terms of the MIT License.  
+SPDX-License-Identifier: MIT
 
-setup(**setup_kwargs)
```

