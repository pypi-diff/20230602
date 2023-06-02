# Comparing `tmp/aind_metadata_service-0.4.6.tar.gz` & `tmp/aind_metadata_service-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.6.tar", last modified: Thu Jun  1 21:46:59 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.7.tar", last modified: Fri Jun  2 18:49:08 2023, max compression
```

## Comparing `aind_metadata_service-0.4.6.tar` & `aind_metadata_service-0.4.7.tar`

### file list

```diff
@@ -1,122 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.378024 aind_metadata_service-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.386024 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.386024 aind_metadata_service-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.386024 aind_metadata_service-0.4.6/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.390024 aind_metadata_service-0.4.6/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.378024 aind_metadata_service-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.390024 aind_metadata_service-0.4.6/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 21:46:45.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.394024 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.394024 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.394024 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.398024 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113119 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.390024 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.398024 aind_metadata_service-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.398024 aind_metadata_service-0.4.6/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.402024 aind_metadata_service-0.4.6/tests/resources/json_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/json_responses/combined.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_las_procedure.json
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_sp_procedure.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.402024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.406024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.406024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66243 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113149 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/tests/resources/json_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/json_responses/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_las_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_sp_procedure.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.901799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.901799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.901799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/test_response_handler.py
```

### Comparing `aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/.github/workflows/ci.yml` & `aind_metadata_service-0.4.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/.github/workflows/publish.yml` & `aind_metadata_service-0.4.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/.gitignore` & `aind_metadata_service-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/Dockerfile` & `aind_metadata_service-0.4.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/LICENSE` & `aind_metadata_service-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/PKG-INFO` & `aind_metadata_service-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.4.6
+Version: 0.4.7
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.6/README.md` & `aind_metadata_service-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/doc_template/Makefile` & `aind_metadata_service-0.4.7/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/doc_template/make.bat` & `aind_metadata_service-0.4.7/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.7/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/doc_template/source/conf.py` & `aind_metadata_service-0.4.7/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/pyproject.toml` & `aind_metadata_service-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/server.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1652,16 +1652,18 @@
         else:
             return {
                 self._nsb.procedure.HP_INJECTION_OPTIC_FIBER: True,
             }.get(self._nsb.procedure, False)
 
     @property
     def has_unknown_procedures(self) -> bool:
-        """Return true if no known procedures are found in nsb model"""
-        if self._nsb.procedure is None:
+        """Return true if no known procedures are found but data is found"""
+        if self._nsb.procedure is None and self.aind_date_of_surgery is None:
+            return False
+        elif self._nsb.procedure is None:
             return True
         else:
             return not (
                 self.has_injection_procedure
                 or self.has_fiber_implant_procedure
                 or self.has_craniotomy_procedure
                 or self.has_head_frame_procedure
```

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/models.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/procedures.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/mapping.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -2625,15 +2625,15 @@
                     animal_weight_post=burr_during_info.weight_post,
                     probes=ophys_probe,
                     anaesthesia=anaesthetic,
                 )
                 procedures.append(fiber_implant_proc)
 
         # Create generic procedure model if no specific procedures found
-        if len(procedures) == 0:
+        if len(procedures) == 0 and self.aind_date_of_surgery:
             subject_procedure = SubjectProcedure.construct(
                 start_date=self.aind_date_of_surgery,
                 end_date=self.aind_date_of_surgery,
                 experimenter_full_name=experimenter_full_name,
                 iacuc_protocol=iacuc_protocol,
                 animal_weight_prior=self.aind_weight_before_surger,
                 animal_weight_post=self.aind_weight_after_surgery,
```

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/models.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/procedures.py` & `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.4.6
+Version: 0.4.7
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -47,44 +47,48 @@
 tests/labtracks/test_query_builder.py
 tests/labtracks/test_response_handler.py
 tests/resources/json_responses/combined.json
 tests/resources/json_responses/mapped_las_procedure.json
 tests/resources/json_responses/mapped_sp_procedure.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
 tests/resources/sharepoint/nsb2019/raw/list_item1.json
 tests/resources/sharepoint/nsb2019/raw/list_item12.json
+tests/resources/sharepoint/nsb2019/raw/list_item19.json
 tests/resources/sharepoint/nsb2019/raw/list_item2.json
 tests/resources/sharepoint/nsb2019/raw/list_item3.json
 tests/resources/sharepoint/nsb2019/raw/list_item4.json
 tests/resources/sharepoint/nsb2019/raw/list_item5.json
 tests/resources/sharepoint/nsb2019/raw/list_item6.json
 tests/resources/sharepoint/nsb2019/raw/list_item7.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
 tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
 tests/resources/sharepoint/nsb2023/raw/list_item10.json
 tests/resources/sharepoint/nsb2023/raw/list_item11.json
 tests/resources/sharepoint/nsb2023/raw/list_item13.json
 tests/resources/sharepoint/nsb2023/raw/list_item14.json
 tests/resources/sharepoint/nsb2023/raw/list_item15.json
 tests/resources/sharepoint/nsb2023/raw/list_item16.json
 tests/resources/sharepoint/nsb2023/raw/list_item17.json
+tests/resources/sharepoint/nsb2023/raw/list_item18.json
 tests/resources/sharepoint/nsb2023/raw/list_item8.json
 tests/resources/sharepoint/nsb2023/raw/list_item9.json
 tests/sharepoint/__init__.py
 tests/sharepoint/test_client.py
 tests/sharepoint/nsb2019/__init__.py
 tests/sharepoint/nsb2019/test_mapping.py
 tests/sharepoint/nsb2019/test_models.py
```

### Comparing `aind_metadata_service-0.4.6/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.7/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.7/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.7/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/json_responses/combined.json` & `aind_metadata_service-0.4.7/tests/resources/json_responses/combined.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_las_procedure.json` & `aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_las_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_sp_procedure.json` & `aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_sp_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_models.py` & `aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.7/tests/sharepoint/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/test_client.py` & `aind_metadata_service-0.4.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.6/tests/test_response_handler.py` & `aind_metadata_service-0.4.7/tests/test_response_handler.py`

 * *Files identical despite different names*

