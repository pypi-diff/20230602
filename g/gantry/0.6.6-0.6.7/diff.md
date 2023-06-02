# Comparing `tmp/gantry-0.6.6.tar.gz` & `tmp/gantry-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.6.tar", last modified: Thu May 25 20:47:42 2023, max compression
+gzip compressed data, was "gantry-0.6.7.tar", last modified: Fri Jun  2 17:03:46 2023, max compression
```

## Comparing `gantry-0.6.6.tar` & `gantry-0.6.7.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-25 20:47:31.000000 gantry-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 20:47:31.000000 gantry-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 20:47:42.634967 gantry-0.6.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.614966 gantry-0.6.6/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28655 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/automations/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/automations/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/triggers/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93878 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    38303 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:47:42.634967 gantry-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-25 20:47:31.000000 gantry-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_llm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   110078 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    38963 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.123817 gantry-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-02 17:03:32.000000 gantry-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 17:03:32.000000 gantry-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 17:03:46.123817 gantry-0.6.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28849 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/automations/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/automations/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/triggers/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94223 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:03:46.123817 gantry-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-02 17:03:32.000000 gantry-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_llm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110166 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.123817 gantry-0.6.7/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_validator.py
```

### Comparing `gantry-0.6.6/LICENSE` & `gantry-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/PKG-INFO` & `gantry-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.6
+Version: 0.6.7
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.6/gantry/__init__.py` & `gantry-0.6.7/gantry/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/alerts/client.py` & `gantry-0.6.7/gantry/alerts/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/alerts/globals.py` & `gantry-0.6.7/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/alerts/main.py` & `gantry-0.6.7/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/api_client.py` & `gantry-0.6.7/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/applications/client.py` & `gantry-0.6.7/gantry/applications/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/applications/core.py` & `gantry-0.6.7/gantry/applications/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,18 @@
                 For batch global tags, use the 'global_tags' parameter instead.
             global_tags (optional, Dict[str, str]): Specify a set of tags that will be attached to
                 all ingested records from this batch. For record specific tags, you can use
                 'row_tags' param. Only used when log is not called within a run.
             join_keys  (optional, Union[List[str], pd.Series[str]]): provide keys to identify
                 each record. These keys can be used later to provide feedback. If not provided,
                 a random record key will be generated for each record.
+
+        Returns:
+            Tuple ([batch_id, list[join_keys]]): The batch_id will be None if records are not
+            logged as batch. The list of join_keys will be the records keys.
         """
         run_id = None
         run_tags = None
         if Run._current_instance:
             run_id = Run._current_instance.run_id
             run_tags = Run._current_instance.tags
         return log(
@@ -716,15 +720,15 @@
         Args:
             include_deleted (optional, bool): Will include deleted datasets if set to `true`
                 and will omit them otherwise.
         Returns:
             ``List[Dict[str, Any]]``: List of dictionaries, each representing one
             dataset and associated metadata.
         """
-        return dataset.list_datasets(include_deleted=include_deleted, model_node_id=self._id)
+        return dataset.list_datasets(include_deleted=include_deleted, model_node_id=str(self._id))
 
     # NotImplemented: chat/completion functions
 
     def create_version(self, *args, **kwargs):
         """
         :meta private:
         """
```

### Comparing `gantry-0.6.6/gantry/applications/llm.py` & `gantry-0.6.7/gantry/applications/llm.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/applications/llm_utils.py` & `gantry-0.6.7/gantry/applications/llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/applications/main.py` & `gantry-0.6.7/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/actions/actions.py` & `gantry-0.6.7/gantry/automations/actions/actions.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,26 +8,39 @@
     delete_slack_notification,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Action(ABC):
+    """
+    Parent class for all actions.
+    """
+
     pass
 
 
 class SendSlackMessage(Action):
     def __init__(
         self,
         name: str,
         webhook_url: str,
         id: Optional[str] = None,
         notify_daily: bool = False,
         alert_id: Optional[str] = None,
     ):
+        """
+        Initialize a slack notification action.
+
+        Args:
+            name (str): the name of the slack notification.
+            webhook_url (str): the webhook url of the slack channel.
+            notify_daily (bool): If true, send notification daily. Otherwise, send immediately.
+
+        """
         self.id = id
         self.name = name
         self.webhook_url = webhook_url
         self.notify_daily = notify_daily
         self.alert_id = alert_id
 
     def update_trigger(self, alert_id: str):
```

### Comparing `gantry-0.6.6/gantry/automations/automations.py` & `gantry-0.6.7/gantry/automations/automations.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,96 +8,120 @@
 from gantry.automations.curators.main import get_curator
 from gantry.automations.triggers import AggregationTrigger, IntervalTrigger, Trigger
 
 logger = logging.getLogger(__name__)
 
 
 class Automation:
+    """
+    Automation is the process of automatically executing tasks.
+    It consists of 2 main components: Trigger and Action.
+
+    Trigger is the condition that, when met, cause the Action to be executed.
+
+    Currently, we are supporting:
+
+    - **IntervalTrigger**: based on time intervals & delayss
+
+    - **AggregationTrigger**: same idea of Alert on the UI. It tracks if an aggregation is outside
+    of the range for the evaluation window and triggers when conditions are met.
+
+    - **SendSlackMessage** (Action): This action sets up a notification setting that will send
+    users a slack notification when executed by the trigger.
+
+    - **Curator** (Action): This action creates a new curator.
+
+    - **Note**:
+        - `AggregationTrigger` can only be paired with `SendSlackMessage`
+        - `IntervalTrigger` can only be paired with `Curator`
+
+    To setup and start an automation process, there are a few steps:
+
+    - Define the trigger
+        .. code-block:: python
+
+            from gantry.automations.triggers import AggregationTrigger
+            from gantry.query.time_window import RelativeTimeWindow
+
+            alert_trigger = AggregationTrigger(
+                name = "alert-trigger",
+                aggregation = "maximum",
+                fields = ["inputs.speed"],
+                lower_bound = 1,
+                upper_bound = 5,
+                evaluation_window=RelativeTimeWindow(
+                    window_length=datetime.timedelta(minutes=10)
+                ),
+                tags = None
+            )
+
+    - Define the action
+        .. code-block:: python
+
+            from gantry.automations.actions import SendSlackMessage
+            # Set up action to send slack message to the specified webhook.
+            slack_action = SendSlackMessage(
+                name = "demo-slack",
+                webhook_url="SLACK_WEBHOOK_URL"
+            )
+
+    - Define the automation and put trigger & action together
+        .. code-block:: python
+
+            from gantry.automations.automations import Automation
+            # Define automation object and put trigger and action together.
+            automation_alert = Automation(
+                name = "alert-automation",
+                trigger=alert_trigger,
+                action=slack_action
+            )
+    - Add the automation to an application
+        .. code-block:: python
+
+            app.add_automation(automation_alert)
+
+    - When you are done, stop the automation process
+        .. code-block:: python
+
+            automation_alert.stop()
+
+
+    """
+
     def __init__(
         self,
         name: str,
         trigger: Trigger,
         action: Action,
         api_client: Optional[APIClient] = None,
         application: Optional[str] = None,
     ):
         """
-        Automation is the process of automatically executing tasks.
-        It consists of 2 main components: Trigger and Action.
+        Initialize an automation object.
 
-        Trigger is the condition that, when met, cause the action to be executed.
-
-        Currently, we are supporting:
-
-        - **IntervalTrigger**: based on time intervals & delays
-        - **AggregationTrigger**: same idea of Alert on the UI. It tracks if an aggregation
-            is outside of the range for the evaluation window and triggers when conditions are met.
-        - **SendSlackMessage** (Action): This action sets up a notification setting that will send
-        users a slack notification when executed by the trigger.
-        - **Curator** (Action): This action creates a new curator.
-        - Note:
-            - `AggregationTrigger` can only be paired with `SendSlackMessage`
-            - `IntervalTrigger` can only be paired with `Curator`
-
-        To setup and start an automation process, there are a few steps:
-        - Define the trigger
-            .. code-block:: python
-
-                from gantry.automations.triggers import AggregationTrigger
-                from gantry.query.time_window import RelativeTimeWindow
-
-                alert_trigger = AggregationTrigger(
-                    name = "alert-trigger",
-                    aggregation = "maximum",
-                    fields = ["inputs.speed"],
-                    lower_bound = 1,
-                    upper_bound = 5,
-                    evaluation_window=RelativeTimeWindow(
-                        window_length=datetime.timedelta(minutes=10)
-                    ),
-                    tags = None
-                )
-
-        - Define the action
-            .. code-block:: python
-
-                from gantry.automations.actions import SendSlackMessage
-                # Set up action to send slack message to the specified webhook.
-                slack_action = SendSlackMessage(
-                    name = "demo-slack",
-                    webhook_url="SLACK_WEBHOOK_URL"
-                )
-
-        - Define the automation and put trigger & action together
-            .. code-block:: python
-
-                from gantry.automations.automations import Automation
-                # Define automation object and put trigger and action together.
-                automation_alert = Automation(
-                    name = "alert-automation",
-                    trigger=alert_trigger,
-                    action=slack_action
-                )
-        - Add the automation to an application
-            .. code-block:: python
-
-                app.add_automation(automation_alert)
+        Args:
+            name (str): the name of the automation.
+            trigger (:class:`gantry.automations.triggers.Trigger`): the trigger of the automation.
+            action (:class:`gantry.automations.actions.Action`): the action of the automation.
 
         """
         self.name = name
         self.trigger = trigger
         self.action = action
         self.application = application
         self._api_client = globals._API_CLIENT if api_client is None else api_client  # type: ignore
 
     def add_to_application(self, application_name):
         """
         Add automation to an application.
         This method shouldn't be called directly.
         It will be called once you call `application.add_automation()`.
+
+        Args:
+            application_name (str): the name of the application.
         """
         self.application = application_name
         self.trigger.add_to_application(application_name)
         logger.info("Automation has been added to application.")
         self.prep()
         self.start()
 
@@ -165,14 +189,17 @@
     def start(self):
         self.action.start()
         data = self.to_dict()
         self._api_client.request("POST", "/api/v1/automations", json=data, raise_for_status=True)
         logger.info("Automation has started.")
 
     def stop(self):
+        """
+        Stop the automation process.
+        """
         self._api_client.request(
             "DELETE",
             f"/api/v1/automations/{self.name}",
             params={"application_name": self.application},
             raise_for_status=True,
         )
         self.remove_from_application()
```

### Comparing `gantry-0.6.6/gantry/automations/curators/__init__.py` & `gantry-0.6.7/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/curators/curators.py` & `gantry-0.6.7/gantry/automations/curators/curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/curators/main.py` & `gantry-0.6.7/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/curators/models.py` & `gantry-0.6.7/gantry/automations/curators/models.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/curators/selectors.py` & `gantry-0.6.7/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/curators/stock_curators.py` & `gantry-0.6.7/gantry/automations/curators/stock_curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/main.py` & `gantry-0.6.7/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/automations/triggers/triggers.py` & `gantry-0.6.7/gantry/automations/triggers/triggers.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from gantry.alerts import create_alert
 from gantry.alerts.client import AlertsAggregation, AlertsCheck
 from gantry.query.time_window import RelativeTimeWindow
 from gantry.utils import from_isoformat_duration, to_datetime, to_isoformat_duration
 
 
 class Trigger(ABC):
+    """
+    Parent class for all triggers.
+    """
+
     def __init__(self):
         self._application_name = None
 
     def add_to_application(self, application_name: str):
         self._application_name = application_name
 
     def remove_from_application(self):
@@ -25,14 +29,22 @@
 class IntervalTrigger(Trigger):
     def __init__(
         self,
         start_on: datetime.datetime,
         interval: datetime.timedelta,
         delay: datetime.timedelta = datetime.timedelta(),
     ):
+        """
+        Initialize an interval trigger.
+
+        Args:
+            start_on (datetime.datetime): the start time of the interval.
+            interval (datetime.timedelta): the interval of the trigger.
+            delay (datetime.timedelta): the delay of the trigger. Defaults to 0.
+        """
         super().__init__()
         self.start_on = start_on
         self.interval = interval
         self.delay = delay or datetime.timedelta()
 
     def is_triggered(self):
         raise NotImplementedError
@@ -63,14 +75,28 @@
         aggregation: AlertsAggregation,
         fields: List[str],
         lower_bound: float,
         upper_bound: float,
         evaluation_window: RelativeTimeWindow,
         tags: Optional[Dict] = None,
     ):
+        """
+        Initialize an aggregation trigger.
+
+        Args:
+            name (str): the name of the trigger.
+            aggregation (AlertsAggregation): the aggregation of the trigger.
+            fields (List[str]): the fields of the trigger.
+            lower_bound (float): the lower bound of the field.
+            upper_bound (float): the upper bound of the field.
+            evaluation_window (:class:`gantry.query.time_window.RelativeTimeWindow`):: the
+                evaluation window for the trigger.
+            tags (Optional[Dict]): the tags of the trigger. Defaults to None.
+
+        """
         super().__init__()
         self.name = name
         self.aggregation = aggregation
         self.fields = fields
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
         self.evaluation_window = evaluation_window.window_length
```

### Comparing `gantry-0.6.6/gantry/cli/application.py` & `gantry-0.6.7/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/cli/bucket.py` & `gantry-0.6.7/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/cli/data_connector.py` & `gantry-0.6.7/gantry/cli/data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/cli/labeling.py` & `gantry-0.6.7/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/cli/main.py` & `gantry-0.6.7/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/cli/projection.py` & `gantry-0.6.7/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/cli/secret.py` & `gantry-0.6.7/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/data_generator/data_generator.py` & `gantry-0.6.7/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/dataset/client.py` & `gantry-0.6.7/gantry/dataset/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/dataset/constants.py` & `gantry-0.6.7/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/dataset/gantry_dataset.py` & `gantry-0.6.7/gantry/dataset/gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/dataset/main.py` & `gantry-0.6.7/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.7/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/exceptions.py` & `gantry-0.6.7/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/logger/client.py` & `gantry-0.6.7/gantry/logger/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,14 +524,18 @@
 
                 For batch global tags, use the 'global_tags' parameter instead.
             global_tags (optional, Dict[str, str]): Specify a set of tags that will be attached to
                 all ingested records from this batch. For record specific tags, you can use
                 'row_tags' param. Only used when log is not called within a run.
             run_id (optional, str): This should never be provided by user. It will be populated automatically when logging within a run to group records together.
             run_tags (optional, Dict[str, str]): This should never be provided by user. It will be populated automatically when logging within a run to provide global tags for all records in the run.
+
+            Returns:
+            Tuple[batch_id, list[join_keys]]: The batch_id will be None if records are not
+            logged as batch. The list of join_keys will be the records keys.
         """
         if run_id:
             # Generate records/events to be logged as part of the Run.
 
             # Check if inputs, outputs, feedbacks, timestamps, and join keys are singular.
             # If so, convert to list with one element.
             if isinstance(inputs, dict):
@@ -927,16 +931,19 @@
             row_tags = row_tags.to_frame()
         if feedbacks is not None and isinstance(feedbacks, pd.Series):
             feedbacks = feedbacks.to_frame()
         if join_keys is not None and isinstance(join_keys, pd.Series):
             join_keys = join_keys.to_list()
             check_type("join_keys", join_keys, List[str])
 
-        if timestamps is not None and isinstance(timestamps, np.ndarray):
-            timestamps = timestamps.tolist()
+        if timestamps is not None:
+            if isinstance(timestamps, np.ndarray):
+                timestamps = timestamps.tolist()
+            elif isinstance(timestamps, pd.DatetimeIndex):
+                timestamps = [ts.to_pydatetime() for ts in timestamps.tolist()]
             check_type("timestamps", timestamps, List[datetime.datetime])
 
         some_preds_exist = _is_not_empty(inputs) or _is_not_empty(outputs)
         preds_exist = _is_not_empty(inputs) and _is_not_empty(outputs)
         feedbacks_exist = _is_not_empty(feedbacks)
 
         if not preds_exist and some_preds_exist:
```

### Comparing `gantry-0.6.6/gantry/logger/constants.py` & `gantry-0.6.7/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/logger/consumer.py` & `gantry-0.6.7/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/logger/event_builder.py` & `gantry-0.6.7/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/logger/main.py` & `gantry-0.6.7/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/logger/stores.py` & `gantry-0.6.7/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/logger/types.py` & `gantry-0.6.7/gantry/logger/types.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/logger/utils.py` & `gantry-0.6.7/gantry/logger/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,21 +134,19 @@
 
 
 def _concurrent_upload_multipart_batch(
     data_batch_iterator: Iterable[bytes], signed_urls: List[str]
 ) -> List[dict]:
     """Uploads batches to presigned URLs concurrently using threads"""
     with concurrent.futures.ThreadPoolExecutor(max_workers=10) as executor:
-        logger.info("Starting multipart upload")
         futures = [
             executor.submit(_put_block, signed_urls[i], i + 1, block)
             for i, block in enumerate(data_batch_iterator)
         ]
         parts = [f.result() for f in concurrent.futures.as_completed(futures)]
-        logger.info("Multipart upload complete")
         return sorted(parts, key=lambda d: d["PartNumber"])  # type: ignore
 
 
 class JoinKey(str):
     @classmethod
     @typechecked
     def from_dict(cls, dict_: Dict) -> str:
```

### Comparing `gantry-0.6.6/gantry/query/__init__.py` & `gantry-0.6.7/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/client.py` & `gantry-0.6.7/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/core/dataframe.py` & `gantry-0.6.7/gantry/query/core/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,32 @@
 import json
 import pprint
 import sys
 from collections import OrderedDict
 from typing import Any, List, NamedTuple, Optional, Set, Union
 
 import pandas as pd
-from cachetools import TTLCache, cached
 from pandas import DataFrame
 from typeguard import typechecked
 
 from gantry.api_client import APIClient
 from gantry.exceptions import GantryException, QueryError
-from gantry.query.core.constants import MAX_SIZE_CACHE_B, MAX_TTL_CACHE_SECS
 from gantry.query.core.queryframe import GantryQueryFrame, QueryInfo
 from gantry.query.core.utils import (
     get_application_node_id,
     get_application_views,
     get_last_application_version,
     get_start_end_time_from_view,
     runs_on,
 )
 
 MAX_WORKERS = 32  # Arbitrary workers for the 'describe' fetching op in dataframe
 
 
-@cached(TTLCache(maxsize=MAX_SIZE_CACHE_B, ttl=MAX_TTL_CACHE_SECS))
-def _raw_query_cached_request(
-    api_client: APIClient, dumped_json_data: str, resource: str = "aggregate"
-):
+def _raw_query_request(api_client: APIClient, dumped_json_data: str, resource: str = "aggregate"):
     return api_client.request(
         "POST",
         f"/api/v1/{resource}/query",
         json=json.loads(dumped_json_data),
         raise_for_status=True,
     )
 
@@ -260,14 +255,22 @@
                 ret[feature["name"]] = GantrySeries(
                     feature["name"],
                     feature["id"],
                     feature["dtype"],
                     feature["event_type"],
                     self,
                 )
+        for i, tag_name in enumerate(self.metadata.get("tags", [])):  # type: ignore
+            ret[tag_name] = GantrySeries(
+                tag_name,
+                str(i),  # TODO: Fix the schema response to return the tag_id.
+                "tag",
+                "tag",
+                self,
+            )
 
         return ret
 
     def describe(self) -> pd.DataFrame:
         """Print basic stats on the dataframe."""
         table = OrderedDict()  # type: ignore
         # Fetch all stats for series concurrently:
@@ -637,32 +640,38 @@
         try:
             quantiles = self.quantile([0.5], num_points=num_points)
             return quantiles[0.5]
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine median")
 
     def count(
-        self, num_points: int = 1, group_by: Optional[str] = None
+        self, num_points: int = 1, group_by: Optional[str] = None, limit: int = 20
     ) -> Union[float, pd.DataFrame]:
         """
         Get the number of available data points for this GantrySeries, if available.
         Works on all series types.
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
             group_by (str, defaults to None): column to use as group_by. If None
                 then no group_by operation is performed and a single result is returned.
+            limit (int, defaults to 20): maximum number of unique categories to return.
+                If you have many unique values, increase this number to > than number of unique
+                categories.
+                You can use the .unique() query to determine the number of categories and pass it.
 
         Returns:
             Float with count if num_points=1 and group_by=None (the default values),
             else a pd.DataFrame.
         """
         try:
-            return self._aggregate_query("total", num_points=num_points, group_by=group_by)
+            return self._aggregate_query(
+                "total", num_points=num_points, group_by=group_by, limit_buckets=limit
+            )
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine count")
 
     @runs_on("int", "float", "datetime")
     def min(
         self, num_points: int = 1, group_by: Optional[str] = None
     ) -> Union[float, datetime.datetime, pd.DataFrame]:
@@ -723,15 +732,15 @@
         """
         try:
             hist_res = self._aggregate_query("category_percents")
             return hist_res
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine histogram")
 
-    @runs_on("bool", "str")
+    @runs_on("bool", "str", "tag")
     def unique(self) -> Set[str]:
         """
         Runs on bool and str series only.
         Get the unique values in this GantrySeries, if available.
 
         Returns:
             Set[str] List containing all the unique values that occur in this series.
@@ -785,46 +794,55 @@
         return self.datatype
 
     def _aggregate_query(
         self,
         attribute,
         num_points: int = 1,
         group_by: Optional[str] = None,
+        limit_buckets: Optional[int] = None,
         **attribute_kwargs,
     ):
         data = self.query_info.get_base_query_params()
         if num_points <= 0:
             raise ValueError(f"num_points must be an int > 0, but received value of {num_points}")
         data["num_points"] = num_points
+        dtype = (
+            self.parent_dataframe[self.name].datatype  # type: ignore
+            if self.name in self.parent_dataframe.series
+            else None
+        )
         data["queries"] = {
             "query": {
-                "query_type": "feature",
+                "query_type": "features",
                 "model_node_id": self.query_info.application_node_id,
                 "stat": attribute,
                 "stat_kwargs": {attribute: attribute_kwargs},
-                "feature": self.name,
+                "features": [{"name": self.name, "dtype": dtype}],
                 "filters": self.parent_dataframe.filters,
                 "tags": self.parent_dataframe.tags,
             }
         }
+        if limit_buckets:
+            data["queries"]["query"]["limit_buckets"] = limit_buckets
+
         if group_by is not None:
             if group_by not in self.parent_dataframe.series:
                 raise ValueError(f"Cannot find column {group_by} in dataframe.")
             if num_points != 1:
                 raise ValueError(
                     "Metric computations that specify a group_by feature "
                     "cannot also specify num_points."
                 )
             group_by_type = self.parent_dataframe[group_by].datatype  # type: ignore
             data["queries"]["query"]["group_by"] = [
                 {"feature_name": group_by, "dtype": group_by_type}
             ]
         resource = "aggregate" if num_points == 1 else "time_series"
         try:
-            response = _raw_query_cached_request(
+            response = _raw_query_request(
                 self.api_client,
                 json.dumps(data, default=lambda x: x.isoformat()),
                 resource=resource,
             )
             data = response["data"]["query"]
             if group_by is not None:
                 df_result = []
```

### Comparing `gantry-0.6.6/gantry/query/core/distance.py` & `gantry-0.6.7/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/core/metric.py` & `gantry-0.6.7/gantry/query/core/metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/core/queryframe.py` & `gantry-0.6.7/gantry/query/core/queryframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,17 @@
 import json
 from collections import defaultdict
 from distutils.util import strtobool
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import dateparser
 import pandas as pd
-from cachetools import LRUCache, TTLCache, cached
 
 from gantry.api_client import APIClient
-from gantry.query.core.constants import (
-    MAX_SIZE_CACHE_B,
-    MAX_TTL_CACHE_SECS,
-    SCHEMA_TYPES,
-    TIMEZONE,
-)
+from gantry.query.core.constants import SCHEMA_TYPES, TIMEZONE
 from gantry.query.core.utils import _build_empty_df_with_schema
 
 ORDER_ASCENDING = "ascending"
 ORDER_DESCENDING = "descending"
 DRUID_TIME_COLUMN_NAME = "__time"
 TIME_COLUMN_NAME = "timestamp"
 
@@ -37,15 +31,14 @@
         "QueryParams", "application_node_id application version environment start_time end_time"
     )
 ):
     def get_base_query_params(self) -> Dict[str, Any]:
         return build_base_query_params(self.start_time, self.end_time, self.version)
 
 
-@cached(TTLCache(maxsize=MAX_SIZE_CACHE_B, ttl=MAX_TTL_CACHE_SECS))
 def _get_raw_data(api_client: APIClient, query_info: QueryInfo, dumped_json_data: str):
     """TTL-Caches data requests to API to make
     repeated fetching operations faster.
     """
     return api_client.request(
         "POST",
         "/api/v1/applications/{}/raw_data".format(query_info.application_node_id),
@@ -53,15 +46,14 @@
         json=json.loads(
             dumped_json_data
         ),  # Need to receive dumped data because json dicts are not hashable
         raise_for_status=True,
     )
 
 
-@cached(LRUCache(maxsize=MAX_SIZE_CACHE_B))
 def _get_metadata(api_client, application_name, frozen_query_params):
     # Reconstruct the query parameters as a true dictionary here, if not cached
     query_params = {k: v for k, v in frozen_query_params}
     response = api_client.request(
         "GET",
         "/api/v1/models/" + application_name + "/schemas",
         params=query_params,
```

### Comparing `gantry-0.6.6/gantry/query/core/utils.py` & `gantry-0.6.7/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/distance/main.py` & `gantry-0.6.7/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/globals.py` & `gantry-0.6.7/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/main.py` & `gantry-0.6.7/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/metric/__init__.py` & `gantry-0.6.7/gantry/query/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/metric/main.py` & `gantry-0.6.7/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/query/time_window.py` & `gantry-0.6.7/gantry/query/time_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,24 +2,38 @@
 from typing import Optional, Union
 
 
 class TimeWindow:
     def __init__(
         self, start_time: Union[str, datetime.datetime], end_time: Union[str, datetime.datetime]
     ):
+        """
+        Initialize a standard time window.
+
+        Args:
+            start_time (Union[str, datetime.datetime]): the start time of the time window.
+            end_time (Union[str, datetime.datetime]): the end time of the time window.
+        """
         self.start_time = start_time
         self.end_time = end_time
 
 
 class RelativeTimeWindow(TimeWindow):
     def __init__(
         self,
         window_length: datetime.timedelta,
         offset: Optional[datetime.timedelta] = None,
     ):
+        """
+        Initialize a relative time window.
+
+        Args:
+            window_length (datetime.timedelta): the length of the time window.
+            offset (Optional[datetime.timedelta]): the offset of the time window. Defaults to None.
+        """
         self.window_length = window_length
         self.offset = offset
         if self.offset is None:
             self.offset = datetime.timedelta()
         end_time: datetime.datetime = (
             datetime.datetime.utcnow() - self.offset if self.offset else datetime.datetime.utcnow()
         )
```

### Comparing `gantry-0.6.6/gantry/serializers.py` & `gantry-0.6.7/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/utils.py` & `gantry-0.6.7/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry/validators.py` & `gantry-0.6.7/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/gantry.egg-info/PKG-INFO` & `gantry-0.6.7/gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.6
+Version: 0.6.7
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.6/gantry.egg-info/SOURCES.txt` & `gantry-0.6.7/gantry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/setup.py` & `gantry-0.6.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     "aiohttp~=3.8",
     # 1.1.1 contains a fix for a regression in a dependency
     # https://stackoverflow.com/a/71574145
     "dateparser~=1.1,>=1.1.1",
     "typeguard~=2.13",
     "boto3-extensions>=0.11.0",
     "backoff~=2.1.2",
-    "cachetools~=4.2",
     "click>=7.1.2",
     "click-aliases~=1.0",
     "click-spinner>=0.1.10",
     "requests>=2.22.0",
     "pyyaml>=5.3.1",
     "colorama>=0.4.0",
     "label-studio-sdk>=0.0.19,<0.0.22",
```

### Comparing `gantry-0.6.6/tests/alerts/test_client.py` & `gantry-0.6.7/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/alerts/test_main.py` & `gantry-0.6.7/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/applications/test_client.py` & `gantry-0.6.7/tests/applications/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/applications/test_core.py` & `gantry-0.6.7/tests/applications/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     m = mock.Mock()
     with mock.patch("gantry.dataset.main._DATASET", m):
         getattr(m, "list_datasets").return_value = "return_value"
         result = application.list_datasets(include_deleted=True)
         assert result == "return_value"
         getattr(m, "list_datasets").assert_called_once_with(
             include_deleted=True,
-            model_node_id=application._id,
+            model_node_id=str(application._id),
         )
 
 
 def test_get_schema(test_api_client):
     application = Application(name="test_application_name", api_client=test_api_client)
     with responses.RequestsMock() as resp:
         resp.add(
```

### Comparing `gantry-0.6.6/tests/applications/test_llm.py` & `gantry-0.6.7/tests/applications/test_llm.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/applications/test_llm_utils.py` & `gantry-0.6.7/tests/applications/test_llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/cli/test_bucket.py` & `gantry-0.6.7/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/cli/test_data_connector.py` & `gantry-0.6.7/tests/cli/test_data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/cli/test_labeling.py` & `gantry-0.6.7/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/cli/test_projection.py` & `gantry-0.6.7/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/cli/test_secrets.py` & `gantry-0.6.7/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/conftest.py` & `gantry-0.6.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/curator/conftest.py` & `gantry-0.6.7/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/curator/test_curator.py` & `gantry-0.6.7/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/curator/test_main.py` & `gantry-0.6.7/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/curator/test_selectors.py` & `gantry-0.6.7/tests/curator/test_selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/data_generator/test_data_generator.py` & `gantry-0.6.7/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/dataset/conftest.py` & `gantry-0.6.7/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/dataset/test_client.py` & `gantry-0.6.7/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.7/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/dataset/test_main.py` & `gantry-0.6.7/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/logger/test_client.py` & `gantry-0.6.7/tests/logger/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3476,3405 +3476,3411 @@
 0000d930: 2020 2020 2020 285b 4355 5252 454e 545f        ([CURRENT_
 0000d940: 5449 4d45 5d20 2a20 322c 205b 4355 5252  TIME] * 2, [CURR
 0000d950: 454e 545f 5449 4d45 5d20 2a20 3229 2c0a  ENT_TIME] * 2),.
 0000d960: 2020 2020 2020 2020 286e 702e 6172 7261          (np.arra
 0000d970: 7928 5b43 5552 5245 4e54 5f54 494d 455d  y([CURRENT_TIME]
 0000d980: 202a 2032 292c 205b 4355 5252 454e 545f   * 2), [CURRENT_
 0000d990: 5449 4d45 5d20 2a20 3229 2c0a 2020 2020  TIME] * 2),.    
-0000d9a0: 5d2c 0a29 0a40 7079 7465 7374 2e6d 6172  ],.).@pytest.mar
-0000d9b0: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
-0000d9c0: 2020 2028 2274 6573 745f 696e 7075 7473     ("test_inputs
-0000d9d0: 222c 2022 7465 7374 5f6f 7574 7075 7473  ", "test_outputs
-0000d9e0: 222c 2022 7465 7374 5f66 6565 6462 6163  ", "test_feedbac
-0000d9f0: 6b73 2229 2c0a 2020 2020 5445 5354 5f49  ks"),.    TEST_I
-0000da00: 4e50 5554 535f 4f55 5450 5554 535f 4645  NPUTS_OUTPUTS_FE
-0000da10: 4544 4241 434b 532c 0a29 0a40 7079 7465  EDBACKS,.).@pyte
-0000da20: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-0000da30: 697a 6528 2276 6572 7369 6f6e 222c 205b  ize("version", [
-0000da40: 4e6f 6e65 2c20 3130 2c20 2231 2e32 2e33  None, 10, "1.2.3
-0000da50: 225d 290a 4070 7974 6573 742e 6d61 726b  "]).@pytest.mark
-0000da60: 2e70 6172 616d 6574 7269 7a65 2822 7461  .parametrize("ta
-0000da70: 6773 2c20 726f 775f 7461 6773 2c20 676c  gs, row_tags, gl
-0000da80: 6f62 616c 5f74 6167 732c 2065 7870 6563  obal_tags, expec
-0000da90: 7465 645f 7461 6773 5f70 6172 616d 222c  ted_tags_param",
-0000daa0: 2054 4553 545f 5441 4753 290a 4070 7974   TEST_TAGS).@pyt
+0000d9a0: 2020 2020 2870 642e 4461 7465 7469 6d65      (pd.Datetime
+0000d9b0: 496e 6465 7828 5b43 5552 5245 4e54 5f54  Index([CURRENT_T
+0000d9c0: 494d 452c 2041 4e4f 5448 4552 5f54 494d  IME, ANOTHER_TIM
+0000d9d0: 455d 292c 205b 4355 5252 454e 545f 5449  E]), [CURRENT_TI
+0000d9e0: 4d45 2c20 414e 4f54 4845 525f 5449 4d45  ME, ANOTHER_TIME
+0000d9f0: 5d29 2c0a 2020 2020 5d2c 0a29 0a40 7079  ]),.    ],.).@py
+0000da00: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+0000da10: 7472 697a 6528 0a20 2020 2028 2274 6573  trize(.    ("tes
+0000da20: 745f 696e 7075 7473 222c 2022 7465 7374  t_inputs", "test
+0000da30: 5f6f 7574 7075 7473 222c 2022 7465 7374  _outputs", "test
+0000da40: 5f66 6565 6462 6163 6b73 2229 2c0a 2020  _feedbacks"),.  
+0000da50: 2020 5445 5354 5f49 4e50 5554 535f 4f55    TEST_INPUTS_OU
+0000da60: 5450 5554 535f 4645 4544 4241 434b 532c  TPUTS_FEEDBACKS,
+0000da70: 0a29 0a40 7079 7465 7374 2e6d 6172 6b2e  .).@pytest.mark.
+0000da80: 7061 7261 6d65 7472 697a 6528 2276 6572  parametrize("ver
+0000da90: 7369 6f6e 222c 205b 4e6f 6e65 2c20 3130  sion", [None, 10
+0000daa0: 2c20 2231 2e32 2e33 225d 290a 4070 7974  , "1.2.3"]).@pyt
 0000dab0: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
-0000dac0: 7269 7a65 280a 2020 2020 226b 7761 7267  rize(.    "kwarg
-0000dad0: 7322 2c0a 2020 2020 5b0a 2020 2020 2020  s",.    [.      
-0000dae0: 2020 7b22 6665 6564 6261 636b 5f6b 6579    {"feedback_key
-0000daf0: 7322 3a20 5b22 4122 5d7d 2c0a 2020 2020  s": ["A"]},.    
-0000db00: 2020 2020 7b22 6665 6564 6261 636b 5f69      {"feedback_i
-0000db10: 6473 223a 205b 2231 3233 3435 222c 2022  ds": ["12345", "
-0000db20: 3637 3839 3022 5d7d 2c0a 2020 2020 2020  67890"]},.      
-0000db30: 2020 7b22 6a6f 696e 5f6b 6579 7322 3a20    {"join_keys": 
-0000db40: 5b22 3534 3332 3122 2c20 2236 3738 3930  ["54321", "67890
-0000db50: 225d 7d2c 0a20 2020 2020 2020 207b 226a  "]},.        {"j
-0000db60: 6f69 6e5f 6b65 7973 223a 2070 642e 5365  oin_keys": pd.Se
-0000db70: 7269 6573 285b 2235 3433 3231 222c 2022  ries(["54321", "
-0000db80: 3637 3839 3022 5d29 7d2c 0a20 2020 2020  67890"])},.     
-0000db90: 2020 207b 7d2c 0a20 2020 205d 2c0a 290a     {},.    ],.).
-0000dba0: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
-0000dbb0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-0000dbc0: 742e 5f72 6573 6f6c 7665 5f6a 6f69 6e5f  t._resolve_join_
-0000dbd0: 6b65 7973 2229 0a40 6d6f 636b 2e70 6174  keys").@mock.pat
-0000dbe0: 6368 280a 2020 2020 2267 616e 7472 792e  ch(.    "gantry.
-0000dbf0: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
-0000dc00: 6e74 7279 2e5f 6c6f 675f 7072 6564 6963  ntry._log_predic
-0000dc10: 7469 6f6e 5f61 6e64 5f66 6565 6462 6163  tion_and_feedbac
-0000dc20: 6b5f 6576 656e 7473 222c 0a20 2020 2072  k_events",.    r
-0000dc30: 6574 7572 6e5f 7661 6c75 653d 284e 6f6e  eturn_value=(Non
-0000dc40: 652c 205b 2231 3233 3435 222c 2022 3637  e, ["12345", "67
-0000dc50: 3839 3022 5d29 2c0a 290a 406d 6f63 6b2e  890"]),.).@mock.
-0000dc60: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-0000dc70: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-0000dc80: 7279 2e5f 6c6f 675f 7072 6564 6963 7469  ry._log_predicti
-0000dc90: 6f6e 5f65 7665 6e74 7322 290a 406d 6f63  on_events").@moc
-0000dca0: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-0000dcb0: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
-0000dcc0: 6e74 7279 2e5f 6c6f 675f 6665 6564 6261  ntry._log_feedba
-0000dcd0: 636b 5f65 7665 6e74 7322 290a 406d 6f63  ck_events").@moc
-0000dce0: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-0000dcf0: 6c6f 6767 6572 2e63 6c69 656e 742e 5f73  logger.client._s
-0000dd00: 616d 706c 655f 7265 636f 7264 7322 2c20  ample_records", 
-0000dd10: 7369 6465 5f65 6666 6563 743d 636c 6965  side_effect=clie
-0000dd20: 6e74 2e5f 7361 6d70 6c65 5f72 6563 6f72  nt._sample_recor
-0000dd30: 6473 290a 406d 6f63 6b2e 7061 7463 6828  ds).@mock.patch(
+0000dac0: 7269 7a65 2822 7461 6773 2c20 726f 775f  rize("tags, row_
+0000dad0: 7461 6773 2c20 676c 6f62 616c 5f74 6167  tags, global_tag
+0000dae0: 732c 2065 7870 6563 7465 645f 7461 6773  s, expected_tags
+0000daf0: 5f70 6172 616d 222c 2054 4553 545f 5441  _param", TEST_TA
+0000db00: 4753 290a 4070 7974 6573 742e 6d61 726b  GS).@pytest.mark
+0000db10: 2e70 6172 616d 6574 7269 7a65 280a 2020  .parametrize(.  
+0000db20: 2020 226b 7761 7267 7322 2c0a 2020 2020    "kwargs",.    
+0000db30: 5b0a 2020 2020 2020 2020 7b22 6665 6564  [.        {"feed
+0000db40: 6261 636b 5f6b 6579 7322 3a20 5b22 4122  back_keys": ["A"
+0000db50: 5d7d 2c0a 2020 2020 2020 2020 7b22 6665  ]},.        {"fe
+0000db60: 6564 6261 636b 5f69 6473 223a 205b 2231  edback_ids": ["1
+0000db70: 3233 3435 222c 2022 3637 3839 3022 5d7d  2345", "67890"]}
+0000db80: 2c0a 2020 2020 2020 2020 7b22 6a6f 696e  ,.        {"join
+0000db90: 5f6b 6579 7322 3a20 5b22 3534 3332 3122  _keys": ["54321"
+0000dba0: 2c20 2236 3738 3930 225d 7d2c 0a20 2020  , "67890"]},.   
+0000dbb0: 2020 2020 207b 226a 6f69 6e5f 6b65 7973       {"join_keys
+0000dbc0: 223a 2070 642e 5365 7269 6573 285b 2235  ": pd.Series(["5
+0000dbd0: 3433 3231 222c 2022 3637 3839 3022 5d29  4321", "67890"])
+0000dbe0: 7d2c 0a20 2020 2020 2020 207b 7d2c 0a20  },.        {},. 
+0000dbf0: 2020 205d 2c0a 290a 406d 6f63 6b2e 7061     ],.).@mock.pa
+0000dc00: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
+0000dc10: 6572 2e63 6c69 656e 742e 5f72 6573 6f6c  er.client._resol
+0000dc20: 7665 5f6a 6f69 6e5f 6b65 7973 2229 0a40  ve_join_keys").@
+0000dc30: 6d6f 636b 2e70 6174 6368 280a 2020 2020  mock.patch(.    
+0000dc40: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
+0000dc50: 6c69 656e 742e 4761 6e74 7279 2e5f 6c6f  lient.Gantry._lo
+0000dc60: 675f 7072 6564 6963 7469 6f6e 5f61 6e64  g_prediction_and
+0000dc70: 5f66 6565 6462 6163 6b5f 6576 656e 7473  _feedback_events
+0000dc80: 222c 0a20 2020 2072 6574 7572 6e5f 7661  ",.    return_va
+0000dc90: 6c75 653d 284e 6f6e 652c 205b 2231 3233  lue=(None, ["123
+0000dca0: 3435 222c 2022 3637 3839 3022 5d29 2c0a  45", "67890"]),.
+0000dcb0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+0000dcc0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+0000dcd0: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
+0000dce0: 7072 6564 6963 7469 6f6e 5f65 7665 6e74  prediction_event
+0000dcf0: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
+0000dd00: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
+0000dd10: 6c69 656e 742e 4761 6e74 7279 2e5f 6c6f  lient.Gantry._lo
+0000dd20: 675f 6665 6564 6261 636b 5f65 7665 6e74  g_feedback_event
+0000dd30: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
 0000dd40: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
-0000dd50: 6c69 656e 742e 5f64 6566 6175 6c74 5f6a  lient._default_j
-0000dd60: 6f69 6e5f 6b65 795f 6765 6e22 290a 6465  oin_key_gen").de
-0000dd70: 6620 7465 7374 5f73 696e 676c 655f 6c6f  f test_single_lo
-0000dd80: 675f 7265 636f 7264 735f 7072 6564 735f  g_records_preds_
-0000dd90: 616e 645f 6665 6564 6261 636b 280a 2020  and_feedback(.  
-0000dda0: 2020 6d6f 636b 5f6a 6f69 6e5f 6b65 795f    mock_join_key_
-0000ddb0: 6765 6e2c 0a20 2020 206d 6f63 6b5f 7361  gen,.    mock_sa
-0000ddc0: 6d70 6c65 5f72 6563 6f72 6473 2c0a 2020  mple_records,.  
-0000ddd0: 2020 6d6f 636b 5f66 6565 6462 6163 6b2c    mock_feedback,
-0000dde0: 0a20 2020 206d 6f63 6b5f 7072 6564 732c  .    mock_preds,
-0000ddf0: 0a20 2020 206d 6f63 6b5f 7072 6564 735f  .    mock_preds_
-0000de00: 616e 645f 6665 6564 6261 636b 2c0a 2020  and_feedback,.  
-0000de10: 2020 6d6f 636b 5f72 6573 6f6c 7665 5f6a    mock_resolve_j
-0000de20: 6f69 6e5f 6b65 7973 2c0a 2020 2020 6b77  oin_keys,.    kw
-0000de30: 6172 6773 2c0a 2020 2020 7665 7273 696f  args,.    versio
-0000de40: 6e2c 0a20 2020 2074 6167 732c 0a20 2020  n,.    tags,.   
-0000de50: 2072 6f77 5f74 6167 732c 0a20 2020 2067   row_tags,.    g
-0000de60: 6c6f 6261 6c5f 7461 6773 2c0a 2020 2020  lobal_tags,.    
-0000de70: 6578 7065 6374 6564 5f74 6167 735f 7061  expected_tags_pa
-0000de80: 7261 6d2c 0a20 2020 2074 6573 745f 7469  ram,.    test_ti
-0000de90: 6d65 7374 616d 7073 2c0a 2020 2020 7465  mestamps,.    te
-0000dea0: 7374 5f74 696d 6573 7461 6d70 735f 6c69  st_timestamps_li
-0000deb0: 7374 2c0a 2020 2020 7465 7374 5f69 6e70  st,.    test_inp
-0000dec0: 7574 732c 0a20 2020 2074 6573 745f 6f75  uts,.    test_ou
-0000ded0: 7470 7574 732c 0a20 2020 2074 6573 745f  tputs,.    test_
-0000dee0: 6665 6564 6261 636b 732c 0a20 2020 2063  feedbacks,.    c
-0000def0: 6c69 5f6f 626a 2c0a 293a 0a20 2020 206d  li_obj,.):.    m
-0000df00: 6f63 6b5f 6a6f 696e 5f6b 6579 5f67 656e  ock_join_key_gen
-0000df10: 2e73 6964 655f 6566 6665 6374 203d 205b  .side_effect = [
-0000df20: 2236 3738 3930 222c 2022 3132 3334 3522  "67890", "12345"
-0000df30: 5d0a 2020 2020 6d6f 636b 5f72 6573 6f6c  ].    mock_resol
-0000df40: 7665 5f6a 6f69 6e5f 6b65 7973 2e72 6574  ve_join_keys.ret
-0000df50: 7572 6e5f 7661 6c75 6520 3d20 5b22 3132  urn_value = ["12
-0000df60: 3334 3522 2c20 2236 3738 3930 225d 2069  345", "67890"] i
-0000df70: 6620 6b77 6172 6773 2065 6c73 6520 4e6f  f kwargs else No
-0000df80: 6e65 0a20 2020 2061 7373 6572 7420 636c  ne.    assert cl
-0000df90: 695f 6f62 6a2e 7369 6e67 6c65 5f6c 6f67  i_obj.single_log
-0000dfa0: 5f72 6563 6f72 6473 280a 2020 2020 2020  _records(.      
-0000dfb0: 2020 6170 706c 6963 6174 696f 6e3d 2266    application="f
-0000dfc0: 6f6f 6261 7222 2c0a 2020 2020 2020 2020  oobar",.        
-0000dfd0: 7665 7273 696f 6e3d 7665 7273 696f 6e2c  version=version,
-0000dfe0: 0a20 2020 2020 2020 2069 6e70 7574 733d  .        inputs=
-0000dff0: 7465 7374 5f69 6e70 7574 732c 0a20 2020  test_inputs,.   
-0000e000: 2020 2020 206f 7574 7075 7473 3d74 6573       outputs=tes
-0000e010: 745f 6f75 7470 7574 732c 0a20 2020 2020  t_outputs,.     
-0000e020: 2020 2066 6565 6462 6163 6b73 3d74 6573     feedbacks=tes
-0000e030: 745f 6665 6564 6261 636b 732c 0a20 2020  t_feedbacks,.   
-0000e040: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
-0000e050: 7465 7374 5f74 696d 6573 7461 6d70 732c  test_timestamps,
-0000e060: 0a20 2020 2020 2020 2073 6f72 745f 6f6e  .        sort_on
-0000e070: 5f74 696d 6573 7461 6d70 3d54 7275 652c  _timestamp=True,
-0000e080: 0a20 2020 2020 2020 2073 616d 706c 655f  .        sample_
-0000e090: 7261 7465 3d31 2c0a 2020 2020 2020 2020  rate=1,.        
-0000e0a0: 7461 6773 3d74 6167 732c 0a20 2020 2020  tags=tags,.     
-0000e0b0: 2020 2072 6f77 5f74 6167 733d 726f 775f     row_tags=row_
-0000e0c0: 7461 6773 2c0a 2020 2020 2020 2020 676c  tags,.        gl
-0000e0d0: 6f62 616c 5f74 6167 733d 676c 6f62 616c  obal_tags=global
-0000e0e0: 5f74 6167 732c 0a20 2020 2020 2020 202a  _tags,.        *
-0000e0f0: 2a6b 7761 7267 732c 0a20 2020 2029 203d  *kwargs,.    ) =
-0000e100: 3d20 284e 6f6e 652c 205b 2231 3233 3435  = (None, ["12345
-0000e110: 222c 2022 3637 3839 3022 5d29 0a0a 2020  ", "67890"])..  
-0000e120: 2020 6d6f 636b 5f70 7265 6473 5f61 6e64    mock_preds_and
-0000e130: 5f66 6565 6462 6163 6b2e 6173 7365 7274  _feedback.assert
-0000e140: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
-0000e150: 6828 0a20 2020 2020 2020 2061 7070 6c69  h(.        appli
-0000e160: 6361 7469 6f6e 3d22 666f 6f62 6172 222c  cation="foobar",
-0000e170: 0a20 2020 2020 2020 2069 6e70 7574 733d  .        inputs=
-0000e180: 5b7b 2241 223a 2031 3030 7d2c 207b 2241  [{"A": 100}, {"A
-0000e190: 223a 2031 3031 7d5d 2c0a 2020 2020 2020  ": 101}],.      
-0000e1a0: 2020 6f75 7470 7574 733d 5b7b 2242 223a    outputs=[{"B":
-0000e1b0: 2033 3030 7d2c 207b 2242 223a 2033 3031   300}, {"B": 301
-0000e1c0: 7d5d 2c0a 2020 2020 2020 2020 6665 6564  }],.        feed
-0000e1d0: 6261 636b 733d 5b7b 2241 223a 2032 3030  backs=[{"A": 200
-0000e1e0: 7d2c 207b 2241 223a 2032 3031 7d5d 2c0a  }, {"A": 201}],.
-0000e1f0: 2020 2020 2020 2020 6a6f 696e 5f6b 6579          join_key
-0000e200: 733d 5b22 3132 3334 3522 2c20 2236 3738  s=["12345", "678
-0000e210: 3930 225d 2069 6620 6b77 6172 6773 2065  90"] if kwargs e
-0000e220: 6c73 6520 5b22 3637 3839 3022 2c20 2231  lse ["67890", "1
-0000e230: 3233 3435 225d 2c0a 2020 2020 2020 2020  2345"],.        
-0000e240: 7665 7273 696f 6e3d 7665 7273 696f 6e2c  version=version,
-0000e250: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
-0000e260: 696e 7075 7473 3d4e 6f6e 652c 0a20 2020  inputs=None,.   
-0000e270: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
-0000e280: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
-0000e290: 6c69 7374 2c0a 2020 2020 2020 2020 736f  list,.        so
-0000e2a0: 7274 5f6f 6e5f 7469 6d65 7374 616d 703d  rt_on_timestamp=
-0000e2b0: 5472 7565 2c0a 2020 2020 2020 2020 6173  True,.        as
-0000e2c0: 5f62 6174 6368 3d46 616c 7365 2c0a 2020  _batch=False,.  
-0000e2d0: 2020 2020 2020 7461 6773 3d65 7870 6563        tags=expec
-0000e2e0: 7465 645f 7461 6773 5f70 6172 616d 2c0a  ted_tags_param,.
-0000e2f0: 2020 2020 290a 2020 2020 6d6f 636b 5f70      ).    mock_p
-0000e300: 7265 6473 2e61 7373 6572 745f 6e6f 745f  reds.assert_not_
-0000e310: 6361 6c6c 6564 2829 0a20 2020 206d 6f63  called().    moc
-0000e320: 6b5f 6665 6564 6261 636b 2e61 7373 6572  k_feedback.asser
-0000e330: 745f 6e6f 745f 6361 6c6c 6564 2829 0a0a  t_not_called()..
-0000e340: 2020 2020 6d6f 636b 5f73 616d 706c 655f      mock_sample_
-0000e350: 7265 636f 7264 732e 6173 7365 7274 5f63  records.assert_c
-0000e360: 616c 6c65 645f 6f6e 6365 5f77 6974 6828  alled_once_with(
-0000e370: 0a20 2020 2020 2020 2032 2c0a 2020 2020  .        2,.    
-0000e380: 2020 2020 312c 0a20 2020 2020 2020 205b      1,.        [
-0000e390: 7b22 4122 3a20 3130 307d 2c20 7b22 4122  {"A": 100}, {"A"
-0000e3a0: 3a20 3130 317d 5d2c 0a20 2020 2020 2020  : 101}],.       
-0000e3b0: 205b 7b22 4222 3a20 3330 307d 2c20 7b22   [{"B": 300}, {"
-0000e3c0: 4222 3a20 3330 317d 5d2c 0a20 2020 2020  B": 301}],.     
-0000e3d0: 2020 205b 7b22 4122 3a20 3230 307d 2c20     [{"A": 200}, 
-0000e3e0: 7b22 4122 3a20 3230 317d 5d2c 0a20 2020  {"A": 201}],.   
-0000e3f0: 2020 2020 2063 6c69 656e 742e 5f72 6573       client._res
-0000e400: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 282a  olve_join_keys(*
-0000e410: 2a6b 7761 7267 7329 2c0a 2020 2020 2020  *kwargs),.      
-0000e420: 2020 7465 7374 5f74 696d 6573 7461 6d70    test_timestamp
-0000e430: 735f 6c69 7374 2c0a 2020 2020 2020 2020  s_list,.        
-0000e440: 6578 7065 6374 6564 5f74 6167 735f 7061  expected_tags_pa
-0000e450: 7261 6d2c 0a20 2020 2029 0a0a 2020 2020  ram,.    )..    
-0000e460: 6966 206b 7761 7267 733a 0a20 2020 2020  if kwargs:.     
-0000e470: 2020 206d 6f63 6b5f 6a6f 696e 5f6b 6579     mock_join_key
-0000e480: 5f67 656e 2e61 7373 6572 745f 6e6f 745f  _gen.assert_not_
-0000e490: 6361 6c6c 6564 2829 0a20 2020 2065 6c73  called().    els
-0000e4a0: 653a 0a20 2020 2020 2020 206d 6f63 6b5f  e:.        mock_
-0000e4b0: 6a6f 696e 5f6b 6579 5f67 656e 2e61 7373  join_key_gen.ass
-0000e4c0: 6572 745f 6361 6c6c 6564 2829 0a0a 0a40  ert_called()...@
-0000e4d0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-0000e4e0: 6d65 7472 697a 6528 0a20 2020 2022 7465  metrize(.    "te
-0000e4f0: 7374 5f74 696d 6573 7461 6d70 732c 2074  st_timestamps, t
-0000e500: 6573 745f 7469 6d65 7374 616d 7073 5f6c  est_timestamps_l
-0000e510: 6973 7422 2c0a 2020 2020 5b0a 2020 2020  ist",.    [.    
-0000e520: 2020 2020 284e 6f6e 652c 204e 6f6e 6529      (None, None)
-0000e530: 2c0a 2020 2020 2020 2020 285b 4355 5252  ,.        ([CURR
-0000e540: 454e 545f 5449 4d45 5d20 2a20 322c 205b  ENT_TIME] * 2, [
-0000e550: 4355 5252 454e 545f 5449 4d45 5d20 2a20  CURRENT_TIME] * 
-0000e560: 3229 2c0a 2020 2020 2020 2020 286e 702e  2),.        (np.
-0000e570: 6172 7261 7928 5b43 5552 5245 4e54 5f54  array([CURRENT_T
-0000e580: 494d 455d 202a 2032 292c 205b 4355 5252  IME] * 2), [CURR
-0000e590: 454e 545f 5449 4d45 5d20 2a20 3229 2c0a  ENT_TIME] * 2),.
-0000e5a0: 2020 2020 5d2c 0a29 0a40 7079 7465 7374      ],.).@pytest
-0000e5b0: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-0000e5c0: 6528 0a20 2020 2028 2274 6573 745f 696e  e(.    ("test_in
-0000e5d0: 7075 7473 222c 2022 7465 7374 5f6f 7574  puts", "test_out
-0000e5e0: 7075 7473 222c 2022 7465 7374 5f66 6565  puts", "test_fee
-0000e5f0: 6462 6163 6b73 2229 2c0a 2020 2020 5445  dbacks"),.    TE
-0000e600: 5354 5f49 4e50 5554 535f 4f55 5450 5554  ST_INPUTS_OUTPUT
-0000e610: 535f 4645 4544 4241 434b 532c 0a29 0a40  S_FEEDBACKS,.).@
-0000e620: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-0000e630: 6d65 7472 697a 6528 2276 6572 7369 6f6e  metrize("version
-0000e640: 222c 205b 4e6f 6e65 2c20 3130 2c20 2231  ", [None, 10, "1
-0000e650: 2e32 2e33 225d 290a 4070 7974 6573 742e  .2.3"]).@pytest.
-0000e660: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-0000e670: 2822 7461 6773 2c20 726f 775f 7461 6773  ("tags, row_tags
-0000e680: 2c20 676c 6f62 616c 5f74 6167 732c 2065  , global_tags, e
-0000e690: 7870 6563 7465 645f 7461 6773 5f70 6172  xpected_tags_par
-0000e6a0: 616d 222c 2054 4553 545f 5441 4753 290a  am", TEST_TAGS).
+0000dd50: 6c69 656e 742e 5f73 616d 706c 655f 7265  lient._sample_re
+0000dd60: 636f 7264 7322 2c20 7369 6465 5f65 6666  cords", side_eff
+0000dd70: 6563 743d 636c 6965 6e74 2e5f 7361 6d70  ect=client._samp
+0000dd80: 6c65 5f72 6563 6f72 6473 290a 406d 6f63  le_records).@moc
+0000dd90: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
+0000dda0: 6c6f 6767 6572 2e63 6c69 656e 742e 5f64  logger.client._d
+0000ddb0: 6566 6175 6c74 5f6a 6f69 6e5f 6b65 795f  efault_join_key_
+0000ddc0: 6765 6e22 290a 6465 6620 7465 7374 5f73  gen").def test_s
+0000ddd0: 696e 676c 655f 6c6f 675f 7265 636f 7264  ingle_log_record
+0000dde0: 735f 7072 6564 735f 616e 645f 6665 6564  s_preds_and_feed
+0000ddf0: 6261 636b 280a 2020 2020 6d6f 636b 5f6a  back(.    mock_j
+0000de00: 6f69 6e5f 6b65 795f 6765 6e2c 0a20 2020  oin_key_gen,.   
+0000de10: 206d 6f63 6b5f 7361 6d70 6c65 5f72 6563   mock_sample_rec
+0000de20: 6f72 6473 2c0a 2020 2020 6d6f 636b 5f66  ords,.    mock_f
+0000de30: 6565 6462 6163 6b2c 0a20 2020 206d 6f63  eedback,.    moc
+0000de40: 6b5f 7072 6564 732c 0a20 2020 206d 6f63  k_preds,.    moc
+0000de50: 6b5f 7072 6564 735f 616e 645f 6665 6564  k_preds_and_feed
+0000de60: 6261 636b 2c0a 2020 2020 6d6f 636b 5f72  back,.    mock_r
+0000de70: 6573 6f6c 7665 5f6a 6f69 6e5f 6b65 7973  esolve_join_keys
+0000de80: 2c0a 2020 2020 6b77 6172 6773 2c0a 2020  ,.    kwargs,.  
+0000de90: 2020 7665 7273 696f 6e2c 0a20 2020 2074    version,.    t
+0000dea0: 6167 732c 0a20 2020 2072 6f77 5f74 6167  ags,.    row_tag
+0000deb0: 732c 0a20 2020 2067 6c6f 6261 6c5f 7461  s,.    global_ta
+0000dec0: 6773 2c0a 2020 2020 6578 7065 6374 6564  gs,.    expected
+0000ded0: 5f74 6167 735f 7061 7261 6d2c 0a20 2020  _tags_param,.   
+0000dee0: 2074 6573 745f 7469 6d65 7374 616d 7073   test_timestamps
+0000def0: 2c0a 2020 2020 7465 7374 5f74 696d 6573  ,.    test_times
+0000df00: 7461 6d70 735f 6c69 7374 2c0a 2020 2020  tamps_list,.    
+0000df10: 7465 7374 5f69 6e70 7574 732c 0a20 2020  test_inputs,.   
+0000df20: 2074 6573 745f 6f75 7470 7574 732c 0a20   test_outputs,. 
+0000df30: 2020 2074 6573 745f 6665 6564 6261 636b     test_feedback
+0000df40: 732c 0a20 2020 2063 6c69 5f6f 626a 2c0a  s,.    cli_obj,.
+0000df50: 293a 0a20 2020 206d 6f63 6b5f 6a6f 696e  ):.    mock_join
+0000df60: 5f6b 6579 5f67 656e 2e73 6964 655f 6566  _key_gen.side_ef
+0000df70: 6665 6374 203d 205b 2236 3738 3930 222c  fect = ["67890",
+0000df80: 2022 3132 3334 3522 5d0a 2020 2020 6d6f   "12345"].    mo
+0000df90: 636b 5f72 6573 6f6c 7665 5f6a 6f69 6e5f  ck_resolve_join_
+0000dfa0: 6b65 7973 2e72 6574 7572 6e5f 7661 6c75  keys.return_valu
+0000dfb0: 6520 3d20 5b22 3132 3334 3522 2c20 2236  e = ["12345", "6
+0000dfc0: 3738 3930 225d 2069 6620 6b77 6172 6773  7890"] if kwargs
+0000dfd0: 2065 6c73 6520 4e6f 6e65 0a20 2020 2061   else None.    a
+0000dfe0: 7373 6572 7420 636c 695f 6f62 6a2e 7369  ssert cli_obj.si
+0000dff0: 6e67 6c65 5f6c 6f67 5f72 6563 6f72 6473  ngle_log_records
+0000e000: 280a 2020 2020 2020 2020 6170 706c 6963  (.        applic
+0000e010: 6174 696f 6e3d 2266 6f6f 6261 7222 2c0a  ation="foobar",.
+0000e020: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
+0000e030: 7665 7273 696f 6e2c 0a20 2020 2020 2020  version,.       
+0000e040: 2069 6e70 7574 733d 7465 7374 5f69 6e70   inputs=test_inp
+0000e050: 7574 732c 0a20 2020 2020 2020 206f 7574  uts,.        out
+0000e060: 7075 7473 3d74 6573 745f 6f75 7470 7574  puts=test_output
+0000e070: 732c 0a20 2020 2020 2020 2066 6565 6462  s,.        feedb
+0000e080: 6163 6b73 3d74 6573 745f 6665 6564 6261  acks=test_feedba
+0000e090: 636b 732c 0a20 2020 2020 2020 2074 696d  cks,.        tim
+0000e0a0: 6573 7461 6d70 733d 7465 7374 5f74 696d  estamps=test_tim
+0000e0b0: 6573 7461 6d70 732c 0a20 2020 2020 2020  estamps,.       
+0000e0c0: 2073 6f72 745f 6f6e 5f74 696d 6573 7461   sort_on_timesta
+0000e0d0: 6d70 3d54 7275 652c 0a20 2020 2020 2020  mp=True,.       
+0000e0e0: 2073 616d 706c 655f 7261 7465 3d31 2c0a   sample_rate=1,.
+0000e0f0: 2020 2020 2020 2020 7461 6773 3d74 6167          tags=tag
+0000e100: 732c 0a20 2020 2020 2020 2072 6f77 5f74  s,.        row_t
+0000e110: 6167 733d 726f 775f 7461 6773 2c0a 2020  ags=row_tags,.  
+0000e120: 2020 2020 2020 676c 6f62 616c 5f74 6167        global_tag
+0000e130: 733d 676c 6f62 616c 5f74 6167 732c 0a20  s=global_tags,. 
+0000e140: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+0000e150: 0a20 2020 2029 203d 3d20 284e 6f6e 652c  .    ) == (None,
+0000e160: 205b 2231 3233 3435 222c 2022 3637 3839   ["12345", "6789
+0000e170: 3022 5d29 0a0a 2020 2020 6d6f 636b 5f70  0"])..    mock_p
+0000e180: 7265 6473 5f61 6e64 5f66 6565 6462 6163  reds_and_feedbac
+0000e190: 6b2e 6173 7365 7274 5f63 616c 6c65 645f  k.assert_called_
+0000e1a0: 6f6e 6365 5f77 6974 6828 0a20 2020 2020  once_with(.     
+0000e1b0: 2020 2061 7070 6c69 6361 7469 6f6e 3d22     application="
+0000e1c0: 666f 6f62 6172 222c 0a20 2020 2020 2020  foobar",.       
+0000e1d0: 2069 6e70 7574 733d 5b7b 2241 223a 2031   inputs=[{"A": 1
+0000e1e0: 3030 7d2c 207b 2241 223a 2031 3031 7d5d  00}, {"A": 101}]
+0000e1f0: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
+0000e200: 733d 5b7b 2242 223a 2033 3030 7d2c 207b  s=[{"B": 300}, {
+0000e210: 2242 223a 2033 3031 7d5d 2c0a 2020 2020  "B": 301}],.    
+0000e220: 2020 2020 6665 6564 6261 636b 733d 5b7b      feedbacks=[{
+0000e230: 2241 223a 2032 3030 7d2c 207b 2241 223a  "A": 200}, {"A":
+0000e240: 2032 3031 7d5d 2c0a 2020 2020 2020 2020   201}],.        
+0000e250: 6a6f 696e 5f6b 6579 733d 5b22 3132 3334  join_keys=["1234
+0000e260: 3522 2c20 2236 3738 3930 225d 2069 6620  5", "67890"] if 
+0000e270: 6b77 6172 6773 2065 6c73 6520 5b22 3637  kwargs else ["67
+0000e280: 3839 3022 2c20 2231 3233 3435 225d 2c0a  890", "12345"],.
+0000e290: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
+0000e2a0: 7665 7273 696f 6e2c 0a20 2020 2020 2020  version,.       
+0000e2b0: 2069 676e 6f72 655f 696e 7075 7473 3d4e   ignore_inputs=N
+0000e2c0: 6f6e 652c 0a20 2020 2020 2020 2074 696d  one,.        tim
+0000e2d0: 6573 7461 6d70 733d 7465 7374 5f74 696d  estamps=test_tim
+0000e2e0: 6573 7461 6d70 735f 6c69 7374 2c0a 2020  estamps_list,.  
+0000e2f0: 2020 2020 2020 736f 7274 5f6f 6e5f 7469        sort_on_ti
+0000e300: 6d65 7374 616d 703d 5472 7565 2c0a 2020  mestamp=True,.  
+0000e310: 2020 2020 2020 6173 5f62 6174 6368 3d46        as_batch=F
+0000e320: 616c 7365 2c0a 2020 2020 2020 2020 7461  alse,.        ta
+0000e330: 6773 3d65 7870 6563 7465 645f 7461 6773  gs=expected_tags
+0000e340: 5f70 6172 616d 2c0a 2020 2020 290a 2020  _param,.    ).  
+0000e350: 2020 6d6f 636b 5f70 7265 6473 2e61 7373    mock_preds.ass
+0000e360: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
+0000e370: 0a20 2020 206d 6f63 6b5f 6665 6564 6261  .    mock_feedba
+0000e380: 636b 2e61 7373 6572 745f 6e6f 745f 6361  ck.assert_not_ca
+0000e390: 6c6c 6564 2829 0a0a 2020 2020 6d6f 636b  lled()..    mock
+0000e3a0: 5f73 616d 706c 655f 7265 636f 7264 732e  _sample_records.
+0000e3b0: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
+0000e3c0: 6365 5f77 6974 6828 0a20 2020 2020 2020  ce_with(.       
+0000e3d0: 2032 2c0a 2020 2020 2020 2020 312c 0a20   2,.        1,. 
+0000e3e0: 2020 2020 2020 205b 7b22 4122 3a20 3130         [{"A": 10
+0000e3f0: 307d 2c20 7b22 4122 3a20 3130 317d 5d2c  0}, {"A": 101}],
+0000e400: 0a20 2020 2020 2020 205b 7b22 4222 3a20  .        [{"B": 
+0000e410: 3330 307d 2c20 7b22 4222 3a20 3330 317d  300}, {"B": 301}
+0000e420: 5d2c 0a20 2020 2020 2020 205b 7b22 4122  ],.        [{"A"
+0000e430: 3a20 3230 307d 2c20 7b22 4122 3a20 3230  : 200}, {"A": 20
+0000e440: 317d 5d2c 0a20 2020 2020 2020 2063 6c69  1}],.        cli
+0000e450: 656e 742e 5f72 6573 6f6c 7665 5f6a 6f69  ent._resolve_joi
+0000e460: 6e5f 6b65 7973 282a 2a6b 7761 7267 7329  n_keys(**kwargs)
+0000e470: 2c0a 2020 2020 2020 2020 7465 7374 5f74  ,.        test_t
+0000e480: 696d 6573 7461 6d70 735f 6c69 7374 2c0a  imestamps_list,.
+0000e490: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+0000e4a0: 5f74 6167 735f 7061 7261 6d2c 0a20 2020  _tags_param,.   
+0000e4b0: 2029 0a0a 2020 2020 6966 206b 7761 7267   )..    if kwarg
+0000e4c0: 733a 0a20 2020 2020 2020 206d 6f63 6b5f  s:.        mock_
+0000e4d0: 6a6f 696e 5f6b 6579 5f67 656e 2e61 7373  join_key_gen.ass
+0000e4e0: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
+0000e4f0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0000e500: 2020 206d 6f63 6b5f 6a6f 696e 5f6b 6579     mock_join_key
+0000e510: 5f67 656e 2e61 7373 6572 745f 6361 6c6c  _gen.assert_call
+0000e520: 6564 2829 0a0a 0a40 7079 7465 7374 2e6d  ed()...@pytest.m
+0000e530: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+0000e540: 0a20 2020 2022 7465 7374 5f74 696d 6573  .    "test_times
+0000e550: 7461 6d70 732c 2074 6573 745f 7469 6d65  tamps, test_time
+0000e560: 7374 616d 7073 5f6c 6973 7422 2c0a 2020  stamps_list",.  
+0000e570: 2020 5b0a 2020 2020 2020 2020 284e 6f6e    [.        (Non
+0000e580: 652c 204e 6f6e 6529 2c0a 2020 2020 2020  e, None),.      
+0000e590: 2020 285b 4355 5252 454e 545f 5449 4d45    ([CURRENT_TIME
+0000e5a0: 5d20 2a20 322c 205b 4355 5252 454e 545f  ] * 2, [CURRENT_
+0000e5b0: 5449 4d45 5d20 2a20 3229 2c0a 2020 2020  TIME] * 2),.    
+0000e5c0: 2020 2020 286e 702e 6172 7261 7928 5b43      (np.array([C
+0000e5d0: 5552 5245 4e54 5f54 494d 455d 202a 2032  URRENT_TIME] * 2
+0000e5e0: 292c 205b 4355 5252 454e 545f 5449 4d45  ), [CURRENT_TIME
+0000e5f0: 5d20 2a20 3229 2c0a 2020 2020 5d2c 0a29  ] * 2),.    ],.)
+0000e600: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
+0000e610: 7261 6d65 7472 697a 6528 0a20 2020 2028  rametrize(.    (
+0000e620: 2274 6573 745f 696e 7075 7473 222c 2022  "test_inputs", "
+0000e630: 7465 7374 5f6f 7574 7075 7473 222c 2022  test_outputs", "
+0000e640: 7465 7374 5f66 6565 6462 6163 6b73 2229  test_feedbacks")
+0000e650: 2c0a 2020 2020 5445 5354 5f49 4e50 5554  ,.    TEST_INPUT
+0000e660: 535f 4f55 5450 5554 535f 4645 4544 4241  S_OUTPUTS_FEEDBA
+0000e670: 434b 532c 0a29 0a40 7079 7465 7374 2e6d  CKS,.).@pytest.m
+0000e680: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+0000e690: 2276 6572 7369 6f6e 222c 205b 4e6f 6e65  "version", [None
+0000e6a0: 2c20 3130 2c20 2231 2e32 2e33 225d 290a  , 10, "1.2.3"]).
 0000e6b0: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
-0000e6c0: 616d 6574 7269 7a65 280a 2020 2020 226b  ametrize(.    "k
-0000e6d0: 7761 7267 7322 2c0a 2020 2020 5b0a 2020  wargs",.    [.  
-0000e6e0: 2020 2020 2020 7b22 6665 6564 6261 636b        {"feedback
-0000e6f0: 5f6b 6579 7322 3a20 5b22 4122 5d7d 2c0a  _keys": ["A"]},.
-0000e700: 2020 2020 2020 2020 7b22 6665 6564 6261          {"feedba
-0000e710: 636b 5f69 6473 223a 205b 2231 3233 3435  ck_ids": ["12345
-0000e720: 222c 2022 3637 3839 3022 5d7d 2c0a 2020  ", "67890"]},.  
-0000e730: 2020 2020 2020 7b22 6a6f 696e 5f6b 6579        {"join_key
-0000e740: 7322 3a20 5b22 3534 3332 3122 2c20 2236  s": ["54321", "6
-0000e750: 3738 3930 225d 7d2c 0a20 2020 2020 2020  7890"]},.       
-0000e760: 207b 226a 6f69 6e5f 6b65 7973 223a 2070   {"join_keys": p
-0000e770: 642e 5365 7269 6573 285b 2235 3433 3231  d.Series(["54321
-0000e780: 222c 2022 3637 3839 3022 5d29 7d2c 0a20  ", "67890"])},. 
-0000e790: 2020 2020 2020 207b 7d2c 0a20 2020 205d         {},.    ]
-0000e7a0: 2c0a 290a 406d 6f63 6b2e 7061 7463 6828  ,.).@mock.patch(
-0000e7b0: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
-0000e7c0: 6c69 656e 742e 5f72 6573 6f6c 7665 5f6a  lient._resolve_j
-0000e7d0: 6f69 6e5f 6b65 7973 2229 0a40 6d6f 636b  oin_keys").@mock
-0000e7e0: 2e70 6174 6368 280a 2020 2020 2267 616e  .patch(.    "gan
-0000e7f0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-0000e800: 742e 4761 6e74 7279 2e5f 6c6f 675f 7072  t.Gantry._log_pr
-0000e810: 6564 6963 7469 6f6e 5f61 6e64 5f66 6565  ediction_and_fee
-0000e820: 6462 6163 6b5f 6576 656e 7473 222c 0a20  dback_events",. 
-0000e830: 2020 2072 6574 7572 6e5f 7661 6c75 653d     return_value=
-0000e840: 284e 6f6e 652c 205b 2231 3233 3435 222c  (None, ["12345",
-0000e850: 2022 3637 3839 3022 5d29 2c0a 290a 406d   "67890"]),.).@m
-0000e860: 6f63 6b2e 7061 7463 6828 2267 616e 7472  ock.patch("gantr
-0000e870: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
-0000e880: 4761 6e74 7279 2e5f 6c6f 675f 7072 6564  Gantry._log_pred
-0000e890: 6963 7469 6f6e 5f65 7665 6e74 7322 290a  iction_events").
-0000e8a0: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
-0000e8b0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-0000e8c0: 742e 4761 6e74 7279 2e5f 6c6f 675f 6665  t.Gantry._log_fe
-0000e8d0: 6564 6261 636b 5f65 7665 6e74 7322 290a  edback_events").
-0000e8e0: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
-0000e8f0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-0000e900: 742e 5f73 616d 706c 655f 7265 636f 7264  t._sample_record
-0000e910: 7322 2c20 7369 6465 5f65 6666 6563 743d  s", side_effect=
-0000e920: 636c 6965 6e74 2e5f 7361 6d70 6c65 5f72  client._sample_r
-0000e930: 6563 6f72 6473 290a 406d 6f63 6b2e 7061  ecords).@mock.pa
+0000e6c0: 616d 6574 7269 7a65 2822 7461 6773 2c20  ametrize("tags, 
+0000e6d0: 726f 775f 7461 6773 2c20 676c 6f62 616c  row_tags, global
+0000e6e0: 5f74 6167 732c 2065 7870 6563 7465 645f  _tags, expected_
+0000e6f0: 7461 6773 5f70 6172 616d 222c 2054 4553  tags_param", TES
+0000e700: 545f 5441 4753 290a 4070 7974 6573 742e  T_TAGS).@pytest.
+0000e710: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+0000e720: 280a 2020 2020 226b 7761 7267 7322 2c0a  (.    "kwargs",.
+0000e730: 2020 2020 5b0a 2020 2020 2020 2020 7b22      [.        {"
+0000e740: 6665 6564 6261 636b 5f6b 6579 7322 3a20  feedback_keys": 
+0000e750: 5b22 4122 5d7d 2c0a 2020 2020 2020 2020  ["A"]},.        
+0000e760: 7b22 6665 6564 6261 636b 5f69 6473 223a  {"feedback_ids":
+0000e770: 205b 2231 3233 3435 222c 2022 3637 3839   ["12345", "6789
+0000e780: 3022 5d7d 2c0a 2020 2020 2020 2020 7b22  0"]},.        {"
+0000e790: 6a6f 696e 5f6b 6579 7322 3a20 5b22 3534  join_keys": ["54
+0000e7a0: 3332 3122 2c20 2236 3738 3930 225d 7d2c  321", "67890"]},
+0000e7b0: 0a20 2020 2020 2020 207b 226a 6f69 6e5f  .        {"join_
+0000e7c0: 6b65 7973 223a 2070 642e 5365 7269 6573  keys": pd.Series
+0000e7d0: 285b 2235 3433 3231 222c 2022 3637 3839  (["54321", "6789
+0000e7e0: 3022 5d29 7d2c 0a20 2020 2020 2020 207b  0"])},.        {
+0000e7f0: 7d2c 0a20 2020 205d 2c0a 290a 406d 6f63  },.    ],.).@moc
+0000e800: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
+0000e810: 6c6f 6767 6572 2e63 6c69 656e 742e 5f72  logger.client._r
+0000e820: 6573 6f6c 7665 5f6a 6f69 6e5f 6b65 7973  esolve_join_keys
+0000e830: 2229 0a40 6d6f 636b 2e70 6174 6368 280a  ").@mock.patch(.
+0000e840: 2020 2020 2267 616e 7472 792e 6c6f 6767      "gantry.logg
+0000e850: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
+0000e860: 2e5f 6c6f 675f 7072 6564 6963 7469 6f6e  ._log_prediction
+0000e870: 5f61 6e64 5f66 6565 6462 6163 6b5f 6576  _and_feedback_ev
+0000e880: 656e 7473 222c 0a20 2020 2072 6574 7572  ents",.    retur
+0000e890: 6e5f 7661 6c75 653d 284e 6f6e 652c 205b  n_value=(None, [
+0000e8a0: 2231 3233 3435 222c 2022 3637 3839 3022  "12345", "67890"
+0000e8b0: 5d29 2c0a 290a 406d 6f63 6b2e 7061 7463  ]),.).@mock.patc
+0000e8c0: 6828 2267 616e 7472 792e 6c6f 6767 6572  h("gantry.logger
+0000e8d0: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
+0000e8e0: 6c6f 675f 7072 6564 6963 7469 6f6e 5f65  log_prediction_e
+0000e8f0: 7665 6e74 7322 290a 406d 6f63 6b2e 7061  vents").@mock.pa
+0000e900: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
+0000e910: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
+0000e920: 2e5f 6c6f 675f 6665 6564 6261 636b 5f65  ._log_feedback_e
+0000e930: 7665 6e74 7322 290a 406d 6f63 6b2e 7061  vents").@mock.pa
 0000e940: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
-0000e950: 6572 2e63 6c69 656e 742e 5f64 6566 6175  er.client._defau
-0000e960: 6c74 5f6a 6f69 6e5f 6b65 795f 6765 6e22  lt_join_key_gen"
-0000e970: 290a 6465 6620 7465 7374 5f6c 6f67 5f72  ).def test_log_r
-0000e980: 6563 6f72 6473 5f70 7265 6473 5f61 6e64  ecords_preds_and
-0000e990: 5f66 6565 6462 6163 6b28 0a20 2020 206d  _feedback(.    m
-0000e9a0: 6f63 6b5f 6a6f 696e 5f6b 6579 5f67 656e  ock_join_key_gen
-0000e9b0: 2c0a 2020 2020 6d6f 636b 5f73 616d 706c  ,.    mock_sampl
-0000e9c0: 655f 7265 636f 7264 732c 0a20 2020 206d  e_records,.    m
-0000e9d0: 6f63 6b5f 6665 6564 6261 636b 2c0a 2020  ock_feedback,.  
-0000e9e0: 2020 6d6f 636b 5f70 7265 6473 2c0a 2020    mock_preds,.  
-0000e9f0: 2020 6d6f 636b 5f70 7265 6473 5f61 6e64    mock_preds_and
-0000ea00: 5f66 6565 6462 6163 6b2c 0a20 2020 206d  _feedback,.    m
-0000ea10: 6f63 6b5f 7265 736f 6c76 655f 6a6f 696e  ock_resolve_join
-0000ea20: 5f6b 6579 732c 0a20 2020 206b 7761 7267  _keys,.    kwarg
-0000ea30: 732c 0a20 2020 2076 6572 7369 6f6e 2c0a  s,.    version,.
-0000ea40: 2020 2020 7461 6773 2c0a 2020 2020 726f      tags,.    ro
-0000ea50: 775f 7461 6773 2c0a 2020 2020 676c 6f62  w_tags,.    glob
-0000ea60: 616c 5f74 6167 732c 0a20 2020 2065 7870  al_tags,.    exp
-0000ea70: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
-0000ea80: 2c0a 2020 2020 7465 7374 5f74 696d 6573  ,.    test_times
-0000ea90: 7461 6d70 732c 0a20 2020 2074 6573 745f  tamps,.    test_
-0000eaa0: 7469 6d65 7374 616d 7073 5f6c 6973 742c  timestamps_list,
-0000eab0: 0a20 2020 2074 6573 745f 696e 7075 7473  .    test_inputs
-0000eac0: 2c0a 2020 2020 7465 7374 5f6f 7574 7075  ,.    test_outpu
-0000ead0: 7473 2c0a 2020 2020 7465 7374 5f66 6565  ts,.    test_fee
-0000eae0: 6462 6163 6b73 2c0a 2020 2020 636c 695f  dbacks,.    cli_
-0000eaf0: 6f62 6a2c 0a29 3a0a 2020 2020 6d6f 636b  obj,.):.    mock
-0000eb00: 5f6a 6f69 6e5f 6b65 795f 6765 6e2e 7369  _join_key_gen.si
-0000eb10: 6465 5f65 6666 6563 7420 3d20 5b22 3637  de_effect = ["67
-0000eb20: 3839 3022 2c20 2231 3233 3435 225d 0a20  890", "12345"]. 
-0000eb30: 2020 206d 6f63 6b5f 7265 736f 6c76 655f     mock_resolve_
-0000eb40: 6a6f 696e 5f6b 6579 732e 7265 7475 726e  join_keys.return
-0000eb50: 5f76 616c 7565 203d 205b 2231 3233 3435  _value = ["12345
-0000eb60: 222c 2022 3637 3839 3022 5d20 6966 206b  ", "67890"] if k
-0000eb70: 7761 7267 7320 656c 7365 204e 6f6e 650a  wargs else None.
-0000eb80: 2020 2020 6173 7365 7274 2063 6c69 5f6f      assert cli_o
-0000eb90: 626a 2e6c 6f67 5f72 6563 6f72 6473 280a  bj.log_records(.
-0000eba0: 2020 2020 2020 2020 6170 706c 6963 6174          applicat
-0000ebb0: 696f 6e3d 2266 6f6f 6261 7222 2c0a 2020  ion="foobar",.  
-0000ebc0: 2020 2020 2020 7665 7273 696f 6e3d 7665        version=ve
-0000ebd0: 7273 696f 6e2c 0a20 2020 2020 2020 2069  rsion,.        i
-0000ebe0: 6e70 7574 733d 7465 7374 5f69 6e70 7574  nputs=test_input
-0000ebf0: 732c 0a20 2020 2020 2020 206f 7574 7075  s,.        outpu
-0000ec00: 7473 3d74 6573 745f 6f75 7470 7574 732c  ts=test_outputs,
-0000ec10: 0a20 2020 2020 2020 2066 6565 6462 6163  .        feedbac
-0000ec20: 6b73 3d74 6573 745f 6665 6564 6261 636b  ks=test_feedback
-0000ec30: 732c 0a20 2020 2020 2020 2074 696d 6573  s,.        times
-0000ec40: 7461 6d70 733d 7465 7374 5f74 696d 6573  tamps=test_times
-0000ec50: 7461 6d70 732c 0a20 2020 2020 2020 2073  tamps,.        s
-0000ec60: 6f72 745f 6f6e 5f74 696d 6573 7461 6d70  ort_on_timestamp
-0000ec70: 3d54 7275 652c 0a20 2020 2020 2020 2073  =True,.        s
-0000ec80: 616d 706c 655f 7261 7465 3d31 2c0a 2020  ample_rate=1,.  
-0000ec90: 2020 2020 2020 7461 6773 3d74 6167 732c        tags=tags,
-0000eca0: 0a20 2020 2020 2020 2072 6f77 5f74 6167  .        row_tag
-0000ecb0: 733d 726f 775f 7461 6773 2c0a 2020 2020  s=row_tags,.    
-0000ecc0: 2020 2020 676c 6f62 616c 5f74 6167 733d      global_tags=
-0000ecd0: 676c 6f62 616c 5f74 6167 732c 0a20 2020  global_tags,.   
-0000ece0: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
-0000ecf0: 2020 2029 203d 3d20 284e 6f6e 652c 205b     ) == (None, [
-0000ed00: 2231 3233 3435 222c 2022 3637 3839 3022  "12345", "67890"
-0000ed10: 5d29 0a0a 2020 2020 6d6f 636b 5f70 7265  ])..    mock_pre
-0000ed20: 6473 5f61 6e64 5f66 6565 6462 6163 6b2e  ds_and_feedback.
-0000ed30: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
-0000ed40: 6365 5f77 6974 6828 0a20 2020 2020 2020  ce_with(.       
-0000ed50: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
-0000ed60: 6f62 6172 222c 0a20 2020 2020 2020 2069  obar",.        i
-0000ed70: 6e70 7574 733d 5b7b 2241 223a 2031 3030  nputs=[{"A": 100
-0000ed80: 7d2c 207b 2241 223a 2031 3031 7d5d 2c0a  }, {"A": 101}],.
-0000ed90: 2020 2020 2020 2020 6f75 7470 7574 733d          outputs=
-0000eda0: 5b7b 2242 223a 2033 3030 7d2c 207b 2242  [{"B": 300}, {"B
-0000edb0: 223a 2033 3031 7d5d 2c0a 2020 2020 2020  ": 301}],.      
-0000edc0: 2020 6665 6564 6261 636b 733d 5b7b 2241    feedbacks=[{"A
-0000edd0: 223a 2032 3030 7d2c 207b 2241 223a 2032  ": 200}, {"A": 2
-0000ede0: 3031 7d5d 2c0a 2020 2020 2020 2020 6a6f  01}],.        jo
-0000edf0: 696e 5f6b 6579 733d 5b22 3132 3334 3522  in_keys=["12345"
-0000ee00: 2c20 2236 3738 3930 225d 2069 6620 6b77  , "67890"] if kw
-0000ee10: 6172 6773 2065 6c73 6520 5b22 3637 3839  args else ["6789
-0000ee20: 3022 2c20 2231 3233 3435 225d 2c0a 2020  0", "12345"],.  
-0000ee30: 2020 2020 2020 7665 7273 696f 6e3d 7665        version=ve
-0000ee40: 7273 696f 6e2c 0a20 2020 2020 2020 2069  rsion,.        i
-0000ee50: 676e 6f72 655f 696e 7075 7473 3d4e 6f6e  gnore_inputs=Non
-0000ee60: 652c 0a20 2020 2020 2020 2074 696d 6573  e,.        times
-0000ee70: 7461 6d70 733d 7465 7374 5f74 696d 6573  tamps=test_times
-0000ee80: 7461 6d70 735f 6c69 7374 2c0a 2020 2020  tamps_list,.    
-0000ee90: 2020 2020 736f 7274 5f6f 6e5f 7469 6d65      sort_on_time
-0000eea0: 7374 616d 703d 5472 7565 2c0a 2020 2020  stamp=True,.    
-0000eeb0: 2020 2020 6173 5f62 6174 6368 3d46 616c      as_batch=Fal
-0000eec0: 7365 2c0a 2020 2020 2020 2020 7461 6773  se,.        tags
-0000eed0: 3d65 7870 6563 7465 645f 7461 6773 5f70  =expected_tags_p
-0000eee0: 6172 616d 2c0a 2020 2020 290a 2020 2020  aram,.    ).    
-0000eef0: 6d6f 636b 5f70 7265 6473 2e61 7373 6572  mock_preds.asser
-0000ef00: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
-0000ef10: 2020 206d 6f63 6b5f 6665 6564 6261 636b     mock_feedback
-0000ef20: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-0000ef30: 6564 2829 0a0a 2020 2020 6d6f 636b 5f73  ed()..    mock_s
-0000ef40: 616d 706c 655f 7265 636f 7264 732e 6173  ample_records.as
-0000ef50: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
-0000ef60: 5f77 6974 6828 0a20 2020 2020 2020 2032  _with(.        2
-0000ef70: 2c0a 2020 2020 2020 2020 312c 0a20 2020  ,.        1,.   
-0000ef80: 2020 2020 205b 7b22 4122 3a20 3130 307d       [{"A": 100}
-0000ef90: 2c20 7b22 4122 3a20 3130 317d 5d2c 0a20  , {"A": 101}],. 
-0000efa0: 2020 2020 2020 205b 7b22 4222 3a20 3330         [{"B": 30
-0000efb0: 307d 2c20 7b22 4222 3a20 3330 317d 5d2c  0}, {"B": 301}],
-0000efc0: 0a20 2020 2020 2020 205b 7b22 4122 3a20  .        [{"A": 
-0000efd0: 3230 307d 2c20 7b22 4122 3a20 3230 317d  200}, {"A": 201}
-0000efe0: 5d2c 0a20 2020 2020 2020 2063 6c69 656e  ],.        clien
-0000eff0: 742e 5f72 6573 6f6c 7665 5f6a 6f69 6e5f  t._resolve_join_
-0000f000: 6b65 7973 282a 2a6b 7761 7267 7329 2c0a  keys(**kwargs),.
-0000f010: 2020 2020 2020 2020 7465 7374 5f74 696d          test_tim
-0000f020: 6573 7461 6d70 735f 6c69 7374 2c0a 2020  estamps_list,.  
-0000f030: 2020 2020 2020 6578 7065 6374 6564 5f74        expected_t
-0000f040: 6167 735f 7061 7261 6d2c 0a20 2020 2029  ags_param,.    )
-0000f050: 0a0a 2020 2020 6966 206b 7761 7267 733a  ..    if kwargs:
-0000f060: 0a20 2020 2020 2020 206d 6f63 6b5f 6a6f  .        mock_jo
-0000f070: 696e 5f6b 6579 5f67 656e 2e61 7373 6572  in_key_gen.asser
-0000f080: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
-0000f090: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f0a0: 206d 6f63 6b5f 6a6f 696e 5f6b 6579 5f67   mock_join_key_g
-0000f0b0: 656e 2e61 7373 6572 745f 6361 6c6c 6564  en.assert_called
-0000f0c0: 2829 0a0a 0a40 7079 7465 7374 2e6d 6172  ()...@pytest.mar
-0000f0d0: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
-0000f0e0: 2020 2022 7465 7374 5f74 696d 6573 7461     "test_timesta
-0000f0f0: 6d70 732c 2074 6573 745f 7469 6d65 7374  mps, test_timest
-0000f100: 616d 7073 5f6c 6973 7422 2c0a 2020 2020  amps_list",.    
-0000f110: 5b0a 2020 2020 2020 2020 284e 6f6e 652c  [.        (None,
-0000f120: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
-0000f130: 285b 4355 5252 454e 545f 5449 4d45 5d20  ([CURRENT_TIME] 
-0000f140: 2a20 322c 205b 4355 5252 454e 545f 5449  * 2, [CURRENT_TI
-0000f150: 4d45 5d20 2a20 3229 2c0a 2020 2020 2020  ME] * 2),.      
-0000f160: 2020 286e 702e 6172 7261 7928 5b43 5552    (np.array([CUR
-0000f170: 5245 4e54 5f54 494d 455d 202a 2032 292c  RENT_TIME] * 2),
-0000f180: 205b 4355 5252 454e 545f 5449 4d45 5d20   [CURRENT_TIME] 
-0000f190: 2a20 3229 2c0a 2020 2020 5d2c 0a29 0a40  * 2),.    ],.).@
-0000f1a0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-0000f1b0: 6d65 7472 697a 6528 0a20 2020 2028 2274  metrize(.    ("t
-0000f1c0: 6573 745f 696e 7075 7473 222c 2022 7465  est_inputs", "te
-0000f1d0: 7374 5f6f 7574 7075 7473 222c 2022 7465  st_outputs", "te
-0000f1e0: 7374 5f66 6565 6462 6163 6b73 2229 2c0a  st_feedbacks"),.
-0000f1f0: 2020 2020 5445 5354 5f49 4e50 5554 535f      TEST_INPUTS_
-0000f200: 4f55 5450 5554 535f 4645 4544 4241 434b  OUTPUTS_FEEDBACK
-0000f210: 532c 0a29 0a40 7079 7465 7374 2e6d 6172  S,.).@pytest.mar
-0000f220: 6b2e 7061 7261 6d65 7472 697a 6528 2276  k.parametrize("v
-0000f230: 6572 7369 6f6e 222c 205b 4e6f 6e65 2c20  ersion", [None, 
-0000f240: 3130 2c20 2231 2e32 2e33 225d 290a 4070  10, "1.2.3"]).@p
-0000f250: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-0000f260: 6574 7269 7a65 2822 7461 6773 2c20 726f  etrize("tags, ro
-0000f270: 775f 7461 6773 2c20 676c 6f62 616c 5f74  w_tags, global_t
-0000f280: 6167 732c 2065 7870 6563 7465 645f 7461  ags, expected_ta
-0000f290: 6773 5f70 6172 616d 222c 2054 4553 545f  gs_param", TEST_
-0000f2a0: 5441 4753 290a 4070 7974 6573 742e 6d61  TAGS).@pytest.ma
-0000f2b0: 726b 2e70 6172 616d 6574 7269 7a65 280a  rk.parametrize(.
-0000f2c0: 2020 2020 226b 7761 7267 7322 2c0a 2020      "kwargs",.  
-0000f2d0: 2020 5b0a 2020 2020 2020 2020 7b22 6a6f    [.        {"jo
-0000f2e0: 696e 5f6b 6579 7322 3a20 5b22 3534 3332  in_keys": ["5432
-0000f2f0: 3122 2c20 2236 3738 3930 225d 7d2c 0a20  1", "67890"]},. 
-0000f300: 2020 2020 2020 207b 226a 6f69 6e5f 6b65         {"join_ke
-0000f310: 7973 223a 2070 642e 5365 7269 6573 285b  ys": pd.Series([
-0000f320: 2235 3433 3231 222c 2022 3637 3839 3022  "54321", "67890"
-0000f330: 5d29 7d2c 0a20 2020 2020 2020 207b 7d2c  ])},.        {},
-0000f340: 0a20 2020 205d 2c0a 290a 406d 6f63 6b2e  .    ],.).@mock.
-0000f350: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-0000f360: 6767 6572 2e63 6c69 656e 742e 5f72 6573  gger.client._res
-0000f370: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2229  olve_join_keys")
-0000f380: 0a40 6d6f 636b 2e70 6174 6368 280a 2020  .@mock.patch(.  
-0000f390: 2020 2267 616e 7472 792e 6c6f 6767 6572    "gantry.logger
-0000f3a0: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-0000f3b0: 6765 6e65 7261 7465 5f70 7265 6469 6374  generate_predict
-0000f3c0: 696f 6e5f 616e 645f 6665 6564 6261 636b  ion_and_feedback
-0000f3d0: 5f65 7665 6e74 7322 2c0a 2020 2020 7265  _events",.    re
-0000f3e0: 7475 726e 5f76 616c 7565 3d28 5b7b 2265  turn_value=([{"e
-0000f3f0: 7665 6e74 223a 2022 706c 6163 655f 686f  vent": "place_ho
-0000f400: 6c64 6572 227d 5d2c 205b 2231 3233 3435  lder"}], ["12345
-0000f410: 222c 2022 3637 3839 3022 5d29 2c0a 290a  ", "67890"]),.).
-0000f420: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
-0000f430: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-0000f440: 742e 4761 6e74 7279 2e5f 6765 6e65 7261  t.Gantry._genera
-0000f450: 7465 5f70 7265 6469 6374 696f 6e5f 6576  te_prediction_ev
-0000f460: 656e 7473 2229 0a40 6d6f 636b 2e70 6174  ents").@mock.pat
-0000f470: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
-0000f480: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
-0000f490: 5f67 656e 6572 6174 655f 6665 6564 6261  _generate_feedba
-0000f4a0: 636b 5f65 7665 6e74 7322 290a 406d 6f63  ck_events").@moc
-0000f4b0: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-0000f4c0: 6c6f 6767 6572 2e63 6c69 656e 742e 5f73  logger.client._s
-0000f4d0: 616d 706c 655f 7265 636f 7264 7322 2c20  ample_records", 
-0000f4e0: 7369 6465 5f65 6666 6563 743d 636c 6965  side_effect=clie
-0000f4f0: 6e74 2e5f 7361 6d70 6c65 5f72 6563 6f72  nt._sample_recor
-0000f500: 6473 290a 406d 6f63 6b2e 7061 7463 6828  ds).@mock.patch(
+0000e950: 6572 2e63 6c69 656e 742e 5f73 616d 706c  er.client._sampl
+0000e960: 655f 7265 636f 7264 7322 2c20 7369 6465  e_records", side
+0000e970: 5f65 6666 6563 743d 636c 6965 6e74 2e5f  _effect=client._
+0000e980: 7361 6d70 6c65 5f72 6563 6f72 6473 290a  sample_records).
+0000e990: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
+0000e9a0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
+0000e9b0: 742e 5f64 6566 6175 6c74 5f6a 6f69 6e5f  t._default_join_
+0000e9c0: 6b65 795f 6765 6e22 290a 6465 6620 7465  key_gen").def te
+0000e9d0: 7374 5f6c 6f67 5f72 6563 6f72 6473 5f70  st_log_records_p
+0000e9e0: 7265 6473 5f61 6e64 5f66 6565 6462 6163  reds_and_feedbac
+0000e9f0: 6b28 0a20 2020 206d 6f63 6b5f 6a6f 696e  k(.    mock_join
+0000ea00: 5f6b 6579 5f67 656e 2c0a 2020 2020 6d6f  _key_gen,.    mo
+0000ea10: 636b 5f73 616d 706c 655f 7265 636f 7264  ck_sample_record
+0000ea20: 732c 0a20 2020 206d 6f63 6b5f 6665 6564  s,.    mock_feed
+0000ea30: 6261 636b 2c0a 2020 2020 6d6f 636b 5f70  back,.    mock_p
+0000ea40: 7265 6473 2c0a 2020 2020 6d6f 636b 5f70  reds,.    mock_p
+0000ea50: 7265 6473 5f61 6e64 5f66 6565 6462 6163  reds_and_feedbac
+0000ea60: 6b2c 0a20 2020 206d 6f63 6b5f 7265 736f  k,.    mock_reso
+0000ea70: 6c76 655f 6a6f 696e 5f6b 6579 732c 0a20  lve_join_keys,. 
+0000ea80: 2020 206b 7761 7267 732c 0a20 2020 2076     kwargs,.    v
+0000ea90: 6572 7369 6f6e 2c0a 2020 2020 7461 6773  ersion,.    tags
+0000eaa0: 2c0a 2020 2020 726f 775f 7461 6773 2c0a  ,.    row_tags,.
+0000eab0: 2020 2020 676c 6f62 616c 5f74 6167 732c      global_tags,
+0000eac0: 0a20 2020 2065 7870 6563 7465 645f 7461  .    expected_ta
+0000ead0: 6773 5f70 6172 616d 2c0a 2020 2020 7465  gs_param,.    te
+0000eae0: 7374 5f74 696d 6573 7461 6d70 732c 0a20  st_timestamps,. 
+0000eaf0: 2020 2074 6573 745f 7469 6d65 7374 616d     test_timestam
+0000eb00: 7073 5f6c 6973 742c 0a20 2020 2074 6573  ps_list,.    tes
+0000eb10: 745f 696e 7075 7473 2c0a 2020 2020 7465  t_inputs,.    te
+0000eb20: 7374 5f6f 7574 7075 7473 2c0a 2020 2020  st_outputs,.    
+0000eb30: 7465 7374 5f66 6565 6462 6163 6b73 2c0a  test_feedbacks,.
+0000eb40: 2020 2020 636c 695f 6f62 6a2c 0a29 3a0a      cli_obj,.):.
+0000eb50: 2020 2020 6d6f 636b 5f6a 6f69 6e5f 6b65      mock_join_ke
+0000eb60: 795f 6765 6e2e 7369 6465 5f65 6666 6563  y_gen.side_effec
+0000eb70: 7420 3d20 5b22 3637 3839 3022 2c20 2231  t = ["67890", "1
+0000eb80: 3233 3435 225d 0a20 2020 206d 6f63 6b5f  2345"].    mock_
+0000eb90: 7265 736f 6c76 655f 6a6f 696e 5f6b 6579  resolve_join_key
+0000eba0: 732e 7265 7475 726e 5f76 616c 7565 203d  s.return_value =
+0000ebb0: 205b 2231 3233 3435 222c 2022 3637 3839   ["12345", "6789
+0000ebc0: 3022 5d20 6966 206b 7761 7267 7320 656c  0"] if kwargs el
+0000ebd0: 7365 204e 6f6e 650a 2020 2020 6173 7365  se None.    asse
+0000ebe0: 7274 2063 6c69 5f6f 626a 2e6c 6f67 5f72  rt cli_obj.log_r
+0000ebf0: 6563 6f72 6473 280a 2020 2020 2020 2020  ecords(.        
+0000ec00: 6170 706c 6963 6174 696f 6e3d 2266 6f6f  application="foo
+0000ec10: 6261 7222 2c0a 2020 2020 2020 2020 7665  bar",.        ve
+0000ec20: 7273 696f 6e3d 7665 7273 696f 6e2c 0a20  rsion=version,. 
+0000ec30: 2020 2020 2020 2069 6e70 7574 733d 7465         inputs=te
+0000ec40: 7374 5f69 6e70 7574 732c 0a20 2020 2020  st_inputs,.     
+0000ec50: 2020 206f 7574 7075 7473 3d74 6573 745f     outputs=test_
+0000ec60: 6f75 7470 7574 732c 0a20 2020 2020 2020  outputs,.       
+0000ec70: 2066 6565 6462 6163 6b73 3d74 6573 745f   feedbacks=test_
+0000ec80: 6665 6564 6261 636b 732c 0a20 2020 2020  feedbacks,.     
+0000ec90: 2020 2074 696d 6573 7461 6d70 733d 7465     timestamps=te
+0000eca0: 7374 5f74 696d 6573 7461 6d70 732c 0a20  st_timestamps,. 
+0000ecb0: 2020 2020 2020 2073 6f72 745f 6f6e 5f74         sort_on_t
+0000ecc0: 696d 6573 7461 6d70 3d54 7275 652c 0a20  imestamp=True,. 
+0000ecd0: 2020 2020 2020 2073 616d 706c 655f 7261         sample_ra
+0000ece0: 7465 3d31 2c0a 2020 2020 2020 2020 7461  te=1,.        ta
+0000ecf0: 6773 3d74 6167 732c 0a20 2020 2020 2020  gs=tags,.       
+0000ed00: 2072 6f77 5f74 6167 733d 726f 775f 7461   row_tags=row_ta
+0000ed10: 6773 2c0a 2020 2020 2020 2020 676c 6f62  gs,.        glob
+0000ed20: 616c 5f74 6167 733d 676c 6f62 616c 5f74  al_tags=global_t
+0000ed30: 6167 732c 0a20 2020 2020 2020 202a 2a6b  ags,.        **k
+0000ed40: 7761 7267 732c 0a20 2020 2029 203d 3d20  wargs,.    ) == 
+0000ed50: 284e 6f6e 652c 205b 2231 3233 3435 222c  (None, ["12345",
+0000ed60: 2022 3637 3839 3022 5d29 0a0a 2020 2020   "67890"])..    
+0000ed70: 6d6f 636b 5f70 7265 6473 5f61 6e64 5f66  mock_preds_and_f
+0000ed80: 6565 6462 6163 6b2e 6173 7365 7274 5f63  eedback.assert_c
+0000ed90: 616c 6c65 645f 6f6e 6365 5f77 6974 6828  alled_once_with(
+0000eda0: 0a20 2020 2020 2020 2061 7070 6c69 6361  .        applica
+0000edb0: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
+0000edc0: 2020 2020 2020 2069 6e70 7574 733d 5b7b         inputs=[{
+0000edd0: 2241 223a 2031 3030 7d2c 207b 2241 223a  "A": 100}, {"A":
+0000ede0: 2031 3031 7d5d 2c0a 2020 2020 2020 2020   101}],.        
+0000edf0: 6f75 7470 7574 733d 5b7b 2242 223a 2033  outputs=[{"B": 3
+0000ee00: 3030 7d2c 207b 2242 223a 2033 3031 7d5d  00}, {"B": 301}]
+0000ee10: 2c0a 2020 2020 2020 2020 6665 6564 6261  ,.        feedba
+0000ee20: 636b 733d 5b7b 2241 223a 2032 3030 7d2c  cks=[{"A": 200},
+0000ee30: 207b 2241 223a 2032 3031 7d5d 2c0a 2020   {"A": 201}],.  
+0000ee40: 2020 2020 2020 6a6f 696e 5f6b 6579 733d        join_keys=
+0000ee50: 5b22 3132 3334 3522 2c20 2236 3738 3930  ["12345", "67890
+0000ee60: 225d 2069 6620 6b77 6172 6773 2065 6c73  "] if kwargs els
+0000ee70: 6520 5b22 3637 3839 3022 2c20 2231 3233  e ["67890", "123
+0000ee80: 3435 225d 2c0a 2020 2020 2020 2020 7665  45"],.        ve
+0000ee90: 7273 696f 6e3d 7665 7273 696f 6e2c 0a20  rsion=version,. 
+0000eea0: 2020 2020 2020 2069 676e 6f72 655f 696e         ignore_in
+0000eeb0: 7075 7473 3d4e 6f6e 652c 0a20 2020 2020  puts=None,.     
+0000eec0: 2020 2074 696d 6573 7461 6d70 733d 7465     timestamps=te
+0000eed0: 7374 5f74 696d 6573 7461 6d70 735f 6c69  st_timestamps_li
+0000eee0: 7374 2c0a 2020 2020 2020 2020 736f 7274  st,.        sort
+0000eef0: 5f6f 6e5f 7469 6d65 7374 616d 703d 5472  _on_timestamp=Tr
+0000ef00: 7565 2c0a 2020 2020 2020 2020 6173 5f62  ue,.        as_b
+0000ef10: 6174 6368 3d46 616c 7365 2c0a 2020 2020  atch=False,.    
+0000ef20: 2020 2020 7461 6773 3d65 7870 6563 7465      tags=expecte
+0000ef30: 645f 7461 6773 5f70 6172 616d 2c0a 2020  d_tags_param,.  
+0000ef40: 2020 290a 2020 2020 6d6f 636b 5f70 7265    ).    mock_pre
+0000ef50: 6473 2e61 7373 6572 745f 6e6f 745f 6361  ds.assert_not_ca
+0000ef60: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
+0000ef70: 6665 6564 6261 636b 2e61 7373 6572 745f  feedback.assert_
+0000ef80: 6e6f 745f 6361 6c6c 6564 2829 0a0a 2020  not_called()..  
+0000ef90: 2020 6d6f 636b 5f73 616d 706c 655f 7265    mock_sample_re
+0000efa0: 636f 7264 732e 6173 7365 7274 5f63 616c  cords.assert_cal
+0000efb0: 6c65 645f 6f6e 6365 5f77 6974 6828 0a20  led_once_with(. 
+0000efc0: 2020 2020 2020 2032 2c0a 2020 2020 2020         2,.      
+0000efd0: 2020 312c 0a20 2020 2020 2020 205b 7b22    1,.        [{"
+0000efe0: 4122 3a20 3130 307d 2c20 7b22 4122 3a20  A": 100}, {"A": 
+0000eff0: 3130 317d 5d2c 0a20 2020 2020 2020 205b  101}],.        [
+0000f000: 7b22 4222 3a20 3330 307d 2c20 7b22 4222  {"B": 300}, {"B"
+0000f010: 3a20 3330 317d 5d2c 0a20 2020 2020 2020  : 301}],.       
+0000f020: 205b 7b22 4122 3a20 3230 307d 2c20 7b22   [{"A": 200}, {"
+0000f030: 4122 3a20 3230 317d 5d2c 0a20 2020 2020  A": 201}],.     
+0000f040: 2020 2063 6c69 656e 742e 5f72 6573 6f6c     client._resol
+0000f050: 7665 5f6a 6f69 6e5f 6b65 7973 282a 2a6b  ve_join_keys(**k
+0000f060: 7761 7267 7329 2c0a 2020 2020 2020 2020  wargs),.        
+0000f070: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
+0000f080: 6c69 7374 2c0a 2020 2020 2020 2020 6578  list,.        ex
+0000f090: 7065 6374 6564 5f74 6167 735f 7061 7261  pected_tags_para
+0000f0a0: 6d2c 0a20 2020 2029 0a0a 2020 2020 6966  m,.    )..    if
+0000f0b0: 206b 7761 7267 733a 0a20 2020 2020 2020   kwargs:.       
+0000f0c0: 206d 6f63 6b5f 6a6f 696e 5f6b 6579 5f67   mock_join_key_g
+0000f0d0: 656e 2e61 7373 6572 745f 6e6f 745f 6361  en.assert_not_ca
+0000f0e0: 6c6c 6564 2829 0a20 2020 2065 6c73 653a  lled().    else:
+0000f0f0: 0a20 2020 2020 2020 206d 6f63 6b5f 6a6f  .        mock_jo
+0000f100: 696e 5f6b 6579 5f67 656e 2e61 7373 6572  in_key_gen.asser
+0000f110: 745f 6361 6c6c 6564 2829 0a0a 0a40 7079  t_called()...@py
+0000f120: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+0000f130: 7472 697a 6528 0a20 2020 2022 7465 7374  trize(.    "test
+0000f140: 5f74 696d 6573 7461 6d70 732c 2074 6573  _timestamps, tes
+0000f150: 745f 7469 6d65 7374 616d 7073 5f6c 6973  t_timestamps_lis
+0000f160: 7422 2c0a 2020 2020 5b0a 2020 2020 2020  t",.    [.      
+0000f170: 2020 284e 6f6e 652c 204e 6f6e 6529 2c0a    (None, None),.
+0000f180: 2020 2020 2020 2020 285b 4355 5252 454e          ([CURREN
+0000f190: 545f 5449 4d45 5d20 2a20 322c 205b 4355  T_TIME] * 2, [CU
+0000f1a0: 5252 454e 545f 5449 4d45 5d20 2a20 3229  RRENT_TIME] * 2)
+0000f1b0: 2c0a 2020 2020 2020 2020 286e 702e 6172  ,.        (np.ar
+0000f1c0: 7261 7928 5b43 5552 5245 4e54 5f54 494d  ray([CURRENT_TIM
+0000f1d0: 455d 202a 2032 292c 205b 4355 5252 454e  E] * 2), [CURREN
+0000f1e0: 545f 5449 4d45 5d20 2a20 3229 2c0a 2020  T_TIME] * 2),.  
+0000f1f0: 2020 5d2c 0a29 0a40 7079 7465 7374 2e6d    ],.).@pytest.m
+0000f200: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+0000f210: 0a20 2020 2028 2274 6573 745f 696e 7075  .    ("test_inpu
+0000f220: 7473 222c 2022 7465 7374 5f6f 7574 7075  ts", "test_outpu
+0000f230: 7473 222c 2022 7465 7374 5f66 6565 6462  ts", "test_feedb
+0000f240: 6163 6b73 2229 2c0a 2020 2020 5445 5354  acks"),.    TEST
+0000f250: 5f49 4e50 5554 535f 4f55 5450 5554 535f  _INPUTS_OUTPUTS_
+0000f260: 4645 4544 4241 434b 532c 0a29 0a40 7079  FEEDBACKS,.).@py
+0000f270: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+0000f280: 7472 697a 6528 2276 6572 7369 6f6e 222c  trize("version",
+0000f290: 205b 4e6f 6e65 2c20 3130 2c20 2231 2e32   [None, 10, "1.2
+0000f2a0: 2e33 225d 290a 4070 7974 6573 742e 6d61  .3"]).@pytest.ma
+0000f2b0: 726b 2e70 6172 616d 6574 7269 7a65 2822  rk.parametrize("
+0000f2c0: 7461 6773 2c20 726f 775f 7461 6773 2c20  tags, row_tags, 
+0000f2d0: 676c 6f62 616c 5f74 6167 732c 2065 7870  global_tags, exp
+0000f2e0: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
+0000f2f0: 222c 2054 4553 545f 5441 4753 290a 4070  ", TEST_TAGS).@p
+0000f300: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
+0000f310: 6574 7269 7a65 280a 2020 2020 226b 7761  etrize(.    "kwa
+0000f320: 7267 7322 2c0a 2020 2020 5b0a 2020 2020  rgs",.    [.    
+0000f330: 2020 2020 7b22 6a6f 696e 5f6b 6579 7322      {"join_keys"
+0000f340: 3a20 5b22 3534 3332 3122 2c20 2236 3738  : ["54321", "678
+0000f350: 3930 225d 7d2c 0a20 2020 2020 2020 207b  90"]},.        {
+0000f360: 226a 6f69 6e5f 6b65 7973 223a 2070 642e  "join_keys": pd.
+0000f370: 5365 7269 6573 285b 2235 3433 3231 222c  Series(["54321",
+0000f380: 2022 3637 3839 3022 5d29 7d2c 0a20 2020   "67890"])},.   
+0000f390: 2020 2020 207b 7d2c 0a20 2020 205d 2c0a       {},.    ],.
+0000f3a0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+0000f3b0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+0000f3c0: 656e 742e 5f72 6573 6f6c 7665 5f6a 6f69  ent._resolve_joi
+0000f3d0: 6e5f 6b65 7973 2229 0a40 6d6f 636b 2e70  n_keys").@mock.p
+0000f3e0: 6174 6368 280a 2020 2020 2267 616e 7472  atch(.    "gantr
+0000f3f0: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+0000f400: 4761 6e74 7279 2e5f 6765 6e65 7261 7465  Gantry._generate
+0000f410: 5f70 7265 6469 6374 696f 6e5f 616e 645f  _prediction_and_
+0000f420: 6665 6564 6261 636b 5f65 7665 6e74 7322  feedback_events"
+0000f430: 2c0a 2020 2020 7265 7475 726e 5f76 616c  ,.    return_val
+0000f440: 7565 3d28 5b7b 2265 7665 6e74 223a 2022  ue=([{"event": "
+0000f450: 706c 6163 655f 686f 6c64 6572 227d 5d2c  place_holder"}],
+0000f460: 205b 2231 3233 3435 222c 2022 3637 3839   ["12345", "6789
+0000f470: 3022 5d29 2c0a 290a 406d 6f63 6b2e 7061  0"]),.).@mock.pa
+0000f480: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
+0000f490: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
+0000f4a0: 2e5f 6765 6e65 7261 7465 5f70 7265 6469  ._generate_predi
+0000f4b0: 6374 696f 6e5f 6576 656e 7473 2229 0a40  ction_events").@
+0000f4c0: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
+0000f4d0: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
+0000f4e0: 2e47 616e 7472 792e 5f67 656e 6572 6174  .Gantry._generat
+0000f4f0: 655f 6665 6564 6261 636b 5f65 7665 6e74  e_feedback_event
+0000f500: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
 0000f510: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
-0000f520: 6c69 656e 742e 5f64 6566 6175 6c74 5f6a  lient._default_j
-0000f530: 6f69 6e5f 6b65 795f 6765 6e22 290a 6465  oin_key_gen").de
-0000f540: 6620 7465 7374 5f67 656e 6572 6174 655f  f test_generate_
-0000f550: 7265 636f 7264 735f 7072 6564 735f 616e  records_preds_an
-0000f560: 645f 6665 6564 6261 636b 280a 2020 2020  d_feedback(.    
-0000f570: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
-0000f580: 6e2c 0a20 2020 206d 6f63 6b5f 7361 6d70  n,.    mock_samp
-0000f590: 6c65 5f72 6563 6f72 6473 2c0a 2020 2020  le_records,.    
-0000f5a0: 6d6f 636b 5f67 656e 6572 6174 655f 6665  mock_generate_fe
-0000f5b0: 6564 6261 636b 2c0a 2020 2020 6d6f 636b  edback,.    mock
-0000f5c0: 5f67 656e 6572 6174 655f 7072 6564 732c  _generate_preds,
-0000f5d0: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
-0000f5e0: 7465 5f70 7265 6473 5f61 6e64 5f66 6565  te_preds_and_fee
-0000f5f0: 6462 6163 6b2c 0a20 2020 206d 6f63 6b5f  dback,.    mock_
-0000f600: 7265 736f 6c76 655f 6a6f 696e 5f6b 6579  resolve_join_key
-0000f610: 732c 0a20 2020 206b 7761 7267 732c 0a20  s,.    kwargs,. 
-0000f620: 2020 2076 6572 7369 6f6e 2c0a 2020 2020     version,.    
-0000f630: 7461 6773 2c0a 2020 2020 726f 775f 7461  tags,.    row_ta
-0000f640: 6773 2c0a 2020 2020 676c 6f62 616c 5f74  gs,.    global_t
-0000f650: 6167 732c 0a20 2020 2065 7870 6563 7465  ags,.    expecte
-0000f660: 645f 7461 6773 5f70 6172 616d 2c0a 2020  d_tags_param,.  
-0000f670: 2020 7465 7374 5f74 696d 6573 7461 6d70    test_timestamp
-0000f680: 732c 0a20 2020 2074 6573 745f 7469 6d65  s,.    test_time
-0000f690: 7374 616d 7073 5f6c 6973 742c 0a20 2020  stamps_list,.   
-0000f6a0: 2074 6573 745f 696e 7075 7473 2c0a 2020   test_inputs,.  
-0000f6b0: 2020 7465 7374 5f6f 7574 7075 7473 2c0a    test_outputs,.
-0000f6c0: 2020 2020 7465 7374 5f66 6565 6462 6163      test_feedbac
-0000f6d0: 6b73 2c0a 2020 2020 636c 695f 6f62 6a2c  ks,.    cli_obj,
-0000f6e0: 0a29 3a0a 2020 2020 6966 2069 7369 6e73  .):.    if isins
-0000f6f0: 7461 6e63 6528 7461 6773 2c20 6c69 7374  tance(tags, list
-0000f700: 293a 0a20 2020 2020 2020 2070 7974 6573  ):.        pytes
-0000f710: 742e 736b 6970 2822 5468 6973 2074 6573  t.skip("This tes
-0000f720: 7420 6973 206e 6f74 2061 7070 6c69 6361  t is not applica
-0000f730: 626c 6520 746f 206c 6973 7420 7461 6773  ble to list tags
-0000f740: 2229 0a0a 2020 2020 6d6f 636b 5f6a 6f69  ")..    mock_joi
-0000f750: 6e5f 6b65 795f 6765 6e2e 7369 6465 5f65  n_key_gen.side_e
-0000f760: 6666 6563 7420 3d20 5b22 3637 3839 3022  ffect = ["67890"
-0000f770: 2c20 2231 3233 3435 225d 0a20 2020 206d  , "12345"].    m
-0000f780: 6f63 6b5f 7265 736f 6c76 655f 6a6f 696e  ock_resolve_join
-0000f790: 5f6b 6579 732e 7265 7475 726e 5f76 616c  _keys.return_val
-0000f7a0: 7565 203d 205b 2231 3233 3435 222c 2022  ue = ["12345", "
-0000f7b0: 3637 3839 3022 5d20 6966 206b 7761 7267  67890"] if kwarg
-0000f7c0: 7320 656c 7365 204e 6f6e 650a 2020 2020  s else None.    
-0000f7d0: 7275 6e5f 6964 203d 2073 7472 2875 7569  run_id = str(uui
-0000f7e0: 642e 7575 6964 3428 2929 0a20 2020 2072  d.uuid4()).    r
-0000f7f0: 756e 5f74 6167 7320 3d20 4e6f 6e65 0a20  un_tags = None. 
-0000f800: 2020 2069 6620 7461 6773 2061 6e64 2067     if tags and g
-0000f810: 6c6f 6261 6c5f 7461 6773 3a0a 2020 2020  lobal_tags:.    
-0000f820: 2020 2020 7275 6e5f 7461 6773 203d 207b      run_tags = {
-0000f830: 2a2a 7461 6773 2c20 2a2a 676c 6f62 616c  **tags, **global
-0000f840: 5f74 6167 737d 0a20 2020 2065 6c69 6620  _tags}.    elif 
-0000f850: 7461 6773 3a0a 2020 2020 2020 2020 7275  tags:.        ru
-0000f860: 6e5f 7461 6773 203d 2074 6167 730a 2020  n_tags = tags.  
-0000f870: 2020 656c 6966 2067 6c6f 6261 6c5f 7461    elif global_ta
-0000f880: 6773 3a0a 2020 2020 2020 2020 7275 6e5f  gs:.        run_
-0000f890: 7461 6773 203d 2067 6c6f 6261 6c5f 7461  tags = global_ta
-0000f8a0: 6773 0a20 2020 2061 7373 6572 7420 636c  gs.    assert cl
-0000f8b0: 695f 6f62 6a2e 6c6f 6728 0a20 2020 2020  i_obj.log(.     
-0000f8c0: 2020 2061 7070 6c69 6361 7469 6f6e 3d22     application="
-0000f8d0: 666f 6f62 6172 222c 0a20 2020 2020 2020  foobar",.       
-0000f8e0: 2076 6572 7369 6f6e 3d76 6572 7369 6f6e   version=version
-0000f8f0: 2c0a 2020 2020 2020 2020 696e 7075 7473  ,.        inputs
-0000f900: 3d74 6573 745f 696e 7075 7473 2c0a 2020  =test_inputs,.  
-0000f910: 2020 2020 2020 6f75 7470 7574 733d 7465        outputs=te
-0000f920: 7374 5f6f 7574 7075 7473 2c0a 2020 2020  st_outputs,.    
-0000f930: 2020 2020 6665 6564 6261 636b 733d 7465      feedbacks=te
-0000f940: 7374 5f66 6565 6462 6163 6b73 2c0a 2020  st_feedbacks,.  
-0000f950: 2020 2020 2020 7469 6d65 7374 616d 7073        timestamps
-0000f960: 3d74 6573 745f 7469 6d65 7374 616d 7073  =test_timestamps
-0000f970: 2c0a 2020 2020 2020 2020 736f 7274 5f6f  ,.        sort_o
-0000f980: 6e5f 7469 6d65 7374 616d 703d 5472 7565  n_timestamp=True
-0000f990: 2c0a 2020 2020 2020 2020 7361 6d70 6c65  ,.        sample
-0000f9a0: 5f72 6174 653d 312c 0a20 2020 2020 2020  _rate=1,.       
-0000f9b0: 2072 756e 5f74 6167 733d 7275 6e5f 7461   run_tags=run_ta
-0000f9c0: 6773 2c0a 2020 2020 2020 2020 726f 775f  gs,.        row_
-0000f9d0: 7461 6773 3d72 6f77 5f74 6167 732c 0a20  tags=row_tags,. 
-0000f9e0: 2020 2020 2020 2072 756e 5f69 643d 7275         run_id=ru
-0000f9f0: 6e5f 6964 2c0a 2020 2020 2020 2020 2a2a  n_id,.        **
-0000fa00: 6b77 6172 6773 2c0a 2020 2020 2920 3d3d  kwargs,.    ) ==
-0000fa10: 205b 7b22 6576 656e 7422 3a20 2270 6c61   [{"event": "pla
-0000fa20: 6365 5f68 6f6c 6465 7222 7d5d 0a0a 2020  ce_holder"}]..  
-0000fa30: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
-0000fa40: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-0000fa50: 636b 2e61 7373 6572 745f 6361 6c6c 6564  ck.assert_called
-0000fa60: 5f6f 6e63 655f 7769 7468 280a 2020 2020  _once_with(.    
-0000fa70: 2020 2020 6170 706c 6963 6174 696f 6e3d      application=
-0000fa80: 2266 6f6f 6261 7222 2c0a 2020 2020 2020  "foobar",.      
-0000fa90: 2020 696e 7075 7473 3d5b 7b22 4122 3a20    inputs=[{"A": 
-0000faa0: 3130 307d 2c20 7b22 4122 3a20 3130 317d  100}, {"A": 101}
-0000fab0: 5d2c 0a20 2020 2020 2020 206f 7574 7075  ],.        outpu
-0000fac0: 7473 3d5b 7b22 4222 3a20 3330 307d 2c20  ts=[{"B": 300}, 
-0000fad0: 7b22 4222 3a20 3330 317d 5d2c 0a20 2020  {"B": 301}],.   
-0000fae0: 2020 2020 2066 6565 6462 6163 6b73 3d5b       feedbacks=[
-0000faf0: 7b22 4122 3a20 3230 307d 2c20 7b22 4122  {"A": 200}, {"A"
-0000fb00: 3a20 3230 317d 5d2c 0a20 2020 2020 2020  : 201}],.       
-0000fb10: 206a 6f69 6e5f 6b65 7973 3d5b 2231 3233   join_keys=["123
-0000fb20: 3435 222c 2022 3637 3839 3022 5d20 6966  45", "67890"] if
-0000fb30: 206b 7761 7267 7320 656c 7365 205b 2236   kwargs else ["6
-0000fb40: 3738 3930 222c 2022 3132 3334 3522 5d2c  7890", "12345"],
-0000fb50: 0a20 2020 2020 2020 2076 6572 7369 6f6e  .        version
-0000fb60: 3d76 6572 7369 6f6e 2c0a 2020 2020 2020  =version,.      
-0000fb70: 2020 6967 6e6f 7265 5f69 6e70 7574 733d    ignore_inputs=
-0000fb80: 4e6f 6e65 2c0a 2020 2020 2020 2020 7469  None,.        ti
-0000fb90: 6d65 7374 616d 7073 3d74 6573 745f 7469  mestamps=test_ti
-0000fba0: 6d65 7374 616d 7073 5f6c 6973 742c 0a20  mestamps_list,. 
-0000fbb0: 2020 2020 2020 2073 6f72 745f 6f6e 5f74         sort_on_t
-0000fbc0: 696d 6573 7461 6d70 3d54 7275 652c 0a20  imestamp=True,. 
-0000fbd0: 2020 2020 2020 2072 756e 5f69 643d 7275         run_id=ru
-0000fbe0: 6e5f 6964 2c0a 2020 2020 2020 2020 7461  n_id,.        ta
-0000fbf0: 6773 3d65 7870 6563 7465 645f 7461 6773  gs=expected_tags
-0000fc00: 5f70 6172 616d 2c0a 2020 2020 290a 2020  _param,.    ).  
-0000fc10: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
-0000fc20: 7072 6564 732e 6173 7365 7274 5f6e 6f74  preds.assert_not
-0000fc30: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
-0000fc40: 636b 5f67 656e 6572 6174 655f 6665 6564  ck_generate_feed
-0000fc50: 6261 636b 2e61 7373 6572 745f 6e6f 745f  back.assert_not_
-0000fc60: 6361 6c6c 6564 2829 0a0a 2020 2020 6d6f  called()..    mo
-0000fc70: 636b 5f73 616d 706c 655f 7265 636f 7264  ck_sample_record
-0000fc80: 732e 6173 7365 7274 5f63 616c 6c65 645f  s.assert_called_
-0000fc90: 6f6e 6365 5f77 6974 6828 0a20 2020 2020  once_with(.     
-0000fca0: 2020 2032 2c0a 2020 2020 2020 2020 312c     2,.        1,
-0000fcb0: 0a20 2020 2020 2020 205b 7b22 4122 3a20  .        [{"A": 
-0000fcc0: 3130 307d 2c20 7b22 4122 3a20 3130 317d  100}, {"A": 101}
-0000fcd0: 5d2c 0a20 2020 2020 2020 205b 7b22 4222  ],.        [{"B"
-0000fce0: 3a20 3330 307d 2c20 7b22 4222 3a20 3330  : 300}, {"B": 30
-0000fcf0: 317d 5d2c 0a20 2020 2020 2020 205b 7b22  1}],.        [{"
-0000fd00: 4122 3a20 3230 307d 2c20 7b22 4122 3a20  A": 200}, {"A": 
-0000fd10: 3230 317d 5d2c 0a20 2020 2020 2020 2063  201}],.        c
-0000fd20: 6c69 656e 742e 5f72 6573 6f6c 7665 5f6a  lient._resolve_j
-0000fd30: 6f69 6e5f 6b65 7973 282a 2a6b 7761 7267  oin_keys(**kwarg
-0000fd40: 7329 2c0a 2020 2020 2020 2020 7465 7374  s),.        test
-0000fd50: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
-0000fd60: 2c0a 2020 2020 2020 2020 6578 7065 6374  ,.        expect
-0000fd70: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
-0000fd80: 2020 2029 0a0a 2020 2020 6966 206b 7761     )..    if kwa
-0000fd90: 7267 733a 0a20 2020 2020 2020 206d 6f63  rgs:.        moc
-0000fda0: 6b5f 6a6f 696e 5f6b 6579 5f67 656e 2e61  k_join_key_gen.a
-0000fdb0: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
-0000fdc0: 2829 0a20 2020 2065 6c73 653a 0a20 2020  ().    else:.   
-0000fdd0: 2020 2020 206d 6f63 6b5f 6a6f 696e 5f6b       mock_join_k
-0000fde0: 6579 5f67 656e 2e61 7373 6572 745f 6361  ey_gen.assert_ca
-0000fdf0: 6c6c 6564 2829 0a0a 0a40 7079 7465 7374  lled()...@pytest
-0000fe00: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-0000fe10: 6528 0a20 2020 2022 7465 7374 5f74 696d  e(.    "test_tim
-0000fe20: 6573 7461 6d70 732c 2074 6573 745f 7469  estamps, test_ti
-0000fe30: 6d65 7374 616d 7073 5f6c 6973 7422 2c0a  mestamps_list",.
-0000fe40: 2020 2020 5b0a 2020 2020 2020 2020 284e      [.        (N
-0000fe50: 6f6e 652c 204e 6f6e 6529 2c0a 2020 2020  one, None),.    
-0000fe60: 2020 2020 285b 4355 5252 454e 545f 5449      ([CURRENT_TI
-0000fe70: 4d45 5d20 2a20 322c 205b 4355 5252 454e  ME] * 2, [CURREN
-0000fe80: 545f 5449 4d45 5d20 2a20 3229 2c0a 2020  T_TIME] * 2),.  
-0000fe90: 2020 2020 2020 286e 702e 6172 7261 7928        (np.array(
-0000fea0: 5b43 5552 5245 4e54 5f54 494d 455d 202a  [CURRENT_TIME] *
-0000feb0: 2032 292c 205b 4355 5252 454e 545f 5449   2), [CURRENT_TI
-0000fec0: 4d45 5d20 2a20 3229 2c0a 2020 2020 5d2c  ME] * 2),.    ],
-0000fed0: 0a29 0a40 7079 7465 7374 2e6d 6172 6b2e  .).@pytest.mark.
-0000fee0: 7061 7261 6d65 7472 697a 6528 0a20 2020  parametrize(.   
-0000fef0: 2028 2274 6573 745f 696e 7075 7473 222c   ("test_inputs",
-0000ff00: 2022 7465 7374 5f6f 7574 7075 7473 222c   "test_outputs",
-0000ff10: 2022 7465 7374 5f66 6565 6462 6163 6b73   "test_feedbacks
-0000ff20: 2229 2c0a 2020 2020 5445 5354 5f49 4e50  "),.    TEST_INP
-0000ff30: 5554 535f 4f55 5450 5554 535f 4645 4544  UTS_OUTPUTS_FEED
-0000ff40: 4241 434b 532c 0a29 0a40 7079 7465 7374  BACKS,.).@pytest
-0000ff50: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-0000ff60: 6528 2276 6572 7369 6f6e 222c 205b 4e6f  e("version", [No
-0000ff70: 6e65 2c20 3130 2c20 2231 2e32 2e33 225d  ne, 10, "1.2.3"]
-0000ff80: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
-0000ff90: 6172 616d 6574 7269 7a65 2822 7461 6773  arametrize("tags
-0000ffa0: 2c20 726f 775f 7461 6773 2c20 676c 6f62  , row_tags, glob
-0000ffb0: 616c 5f74 6167 732c 2065 7870 6563 7465  al_tags, expecte
-0000ffc0: 645f 7461 6773 5f70 6172 616d 222c 2054  d_tags_param", T
-0000ffd0: 4553 545f 5441 4753 290a 4070 7974 6573  EST_TAGS).@pytes
+0000f520: 6c69 656e 742e 5f73 616d 706c 655f 7265  lient._sample_re
+0000f530: 636f 7264 7322 2c20 7369 6465 5f65 6666  cords", side_eff
+0000f540: 6563 743d 636c 6965 6e74 2e5f 7361 6d70  ect=client._samp
+0000f550: 6c65 5f72 6563 6f72 6473 290a 406d 6f63  le_records).@moc
+0000f560: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
+0000f570: 6c6f 6767 6572 2e63 6c69 656e 742e 5f64  logger.client._d
+0000f580: 6566 6175 6c74 5f6a 6f69 6e5f 6b65 795f  efault_join_key_
+0000f590: 6765 6e22 290a 6465 6620 7465 7374 5f67  gen").def test_g
+0000f5a0: 656e 6572 6174 655f 7265 636f 7264 735f  enerate_records_
+0000f5b0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+0000f5c0: 636b 280a 2020 2020 6d6f 636b 5f6a 6f69  ck(.    mock_joi
+0000f5d0: 6e5f 6b65 795f 6765 6e2c 0a20 2020 206d  n_key_gen,.    m
+0000f5e0: 6f63 6b5f 7361 6d70 6c65 5f72 6563 6f72  ock_sample_recor
+0000f5f0: 6473 2c0a 2020 2020 6d6f 636b 5f67 656e  ds,.    mock_gen
+0000f600: 6572 6174 655f 6665 6564 6261 636b 2c0a  erate_feedback,.
+0000f610: 2020 2020 6d6f 636b 5f67 656e 6572 6174      mock_generat
+0000f620: 655f 7072 6564 732c 0a20 2020 206d 6f63  e_preds,.    moc
+0000f630: 6b5f 6765 6e65 7261 7465 5f70 7265 6473  k_generate_preds
+0000f640: 5f61 6e64 5f66 6565 6462 6163 6b2c 0a20  _and_feedback,. 
+0000f650: 2020 206d 6f63 6b5f 7265 736f 6c76 655f     mock_resolve_
+0000f660: 6a6f 696e 5f6b 6579 732c 0a20 2020 206b  join_keys,.    k
+0000f670: 7761 7267 732c 0a20 2020 2076 6572 7369  wargs,.    versi
+0000f680: 6f6e 2c0a 2020 2020 7461 6773 2c0a 2020  on,.    tags,.  
+0000f690: 2020 726f 775f 7461 6773 2c0a 2020 2020    row_tags,.    
+0000f6a0: 676c 6f62 616c 5f74 6167 732c 0a20 2020  global_tags,.   
+0000f6b0: 2065 7870 6563 7465 645f 7461 6773 5f70   expected_tags_p
+0000f6c0: 6172 616d 2c0a 2020 2020 7465 7374 5f74  aram,.    test_t
+0000f6d0: 696d 6573 7461 6d70 732c 0a20 2020 2074  imestamps,.    t
+0000f6e0: 6573 745f 7469 6d65 7374 616d 7073 5f6c  est_timestamps_l
+0000f6f0: 6973 742c 0a20 2020 2074 6573 745f 696e  ist,.    test_in
+0000f700: 7075 7473 2c0a 2020 2020 7465 7374 5f6f  puts,.    test_o
+0000f710: 7574 7075 7473 2c0a 2020 2020 7465 7374  utputs,.    test
+0000f720: 5f66 6565 6462 6163 6b73 2c0a 2020 2020  _feedbacks,.    
+0000f730: 636c 695f 6f62 6a2c 0a29 3a0a 2020 2020  cli_obj,.):.    
+0000f740: 6966 2069 7369 6e73 7461 6e63 6528 7461  if isinstance(ta
+0000f750: 6773 2c20 6c69 7374 293a 0a20 2020 2020  gs, list):.     
+0000f760: 2020 2070 7974 6573 742e 736b 6970 2822     pytest.skip("
+0000f770: 5468 6973 2074 6573 7420 6973 206e 6f74  This test is not
+0000f780: 2061 7070 6c69 6361 626c 6520 746f 206c   applicable to l
+0000f790: 6973 7420 7461 6773 2229 0a0a 2020 2020  ist tags")..    
+0000f7a0: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
+0000f7b0: 6e2e 7369 6465 5f65 6666 6563 7420 3d20  n.side_effect = 
+0000f7c0: 5b22 3637 3839 3022 2c20 2231 3233 3435  ["67890", "12345
+0000f7d0: 225d 0a20 2020 206d 6f63 6b5f 7265 736f  "].    mock_reso
+0000f7e0: 6c76 655f 6a6f 696e 5f6b 6579 732e 7265  lve_join_keys.re
+0000f7f0: 7475 726e 5f76 616c 7565 203d 205b 2231  turn_value = ["1
+0000f800: 3233 3435 222c 2022 3637 3839 3022 5d20  2345", "67890"] 
+0000f810: 6966 206b 7761 7267 7320 656c 7365 204e  if kwargs else N
+0000f820: 6f6e 650a 2020 2020 7275 6e5f 6964 203d  one.    run_id =
+0000f830: 2073 7472 2875 7569 642e 7575 6964 3428   str(uuid.uuid4(
+0000f840: 2929 0a20 2020 2072 756e 5f74 6167 7320  )).    run_tags 
+0000f850: 3d20 4e6f 6e65 0a20 2020 2069 6620 7461  = None.    if ta
+0000f860: 6773 2061 6e64 2067 6c6f 6261 6c5f 7461  gs and global_ta
+0000f870: 6773 3a0a 2020 2020 2020 2020 7275 6e5f  gs:.        run_
+0000f880: 7461 6773 203d 207b 2a2a 7461 6773 2c20  tags = {**tags, 
+0000f890: 2a2a 676c 6f62 616c 5f74 6167 737d 0a20  **global_tags}. 
+0000f8a0: 2020 2065 6c69 6620 7461 6773 3a0a 2020     elif tags:.  
+0000f8b0: 2020 2020 2020 7275 6e5f 7461 6773 203d        run_tags =
+0000f8c0: 2074 6167 730a 2020 2020 656c 6966 2067   tags.    elif g
+0000f8d0: 6c6f 6261 6c5f 7461 6773 3a0a 2020 2020  lobal_tags:.    
+0000f8e0: 2020 2020 7275 6e5f 7461 6773 203d 2067      run_tags = g
+0000f8f0: 6c6f 6261 6c5f 7461 6773 0a20 2020 2061  lobal_tags.    a
+0000f900: 7373 6572 7420 636c 695f 6f62 6a2e 6c6f  ssert cli_obj.lo
+0000f910: 6728 0a20 2020 2020 2020 2061 7070 6c69  g(.        appli
+0000f920: 6361 7469 6f6e 3d22 666f 6f62 6172 222c  cation="foobar",
+0000f930: 0a20 2020 2020 2020 2076 6572 7369 6f6e  .        version
+0000f940: 3d76 6572 7369 6f6e 2c0a 2020 2020 2020  =version,.      
+0000f950: 2020 696e 7075 7473 3d74 6573 745f 696e    inputs=test_in
+0000f960: 7075 7473 2c0a 2020 2020 2020 2020 6f75  puts,.        ou
+0000f970: 7470 7574 733d 7465 7374 5f6f 7574 7075  tputs=test_outpu
+0000f980: 7473 2c0a 2020 2020 2020 2020 6665 6564  ts,.        feed
+0000f990: 6261 636b 733d 7465 7374 5f66 6565 6462  backs=test_feedb
+0000f9a0: 6163 6b73 2c0a 2020 2020 2020 2020 7469  acks,.        ti
+0000f9b0: 6d65 7374 616d 7073 3d74 6573 745f 7469  mestamps=test_ti
+0000f9c0: 6d65 7374 616d 7073 2c0a 2020 2020 2020  mestamps,.      
+0000f9d0: 2020 736f 7274 5f6f 6e5f 7469 6d65 7374    sort_on_timest
+0000f9e0: 616d 703d 5472 7565 2c0a 2020 2020 2020  amp=True,.      
+0000f9f0: 2020 7361 6d70 6c65 5f72 6174 653d 312c    sample_rate=1,
+0000fa00: 0a20 2020 2020 2020 2072 756e 5f74 6167  .        run_tag
+0000fa10: 733d 7275 6e5f 7461 6773 2c0a 2020 2020  s=run_tags,.    
+0000fa20: 2020 2020 726f 775f 7461 6773 3d72 6f77      row_tags=row
+0000fa30: 5f74 6167 732c 0a20 2020 2020 2020 2072  _tags,.        r
+0000fa40: 756e 5f69 643d 7275 6e5f 6964 2c0a 2020  un_id=run_id,.  
+0000fa50: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
+0000fa60: 2020 2020 2920 3d3d 205b 7b22 6576 656e      ) == [{"even
+0000fa70: 7422 3a20 2270 6c61 6365 5f68 6f6c 6465  t": "place_holde
+0000fa80: 7222 7d5d 0a0a 2020 2020 6d6f 636b 5f67  r"}]..    mock_g
+0000fa90: 656e 6572 6174 655f 7072 6564 735f 616e  enerate_preds_an
+0000faa0: 645f 6665 6564 6261 636b 2e61 7373 6572  d_feedback.asser
+0000fab0: 745f 6361 6c6c 6564 5f6f 6e63 655f 7769  t_called_once_wi
+0000fac0: 7468 280a 2020 2020 2020 2020 6170 706c  th(.        appl
+0000fad0: 6963 6174 696f 6e3d 2266 6f6f 6261 7222  ication="foobar"
+0000fae0: 2c0a 2020 2020 2020 2020 696e 7075 7473  ,.        inputs
+0000faf0: 3d5b 7b22 4122 3a20 3130 307d 2c20 7b22  =[{"A": 100}, {"
+0000fb00: 4122 3a20 3130 317d 5d2c 0a20 2020 2020  A": 101}],.     
+0000fb10: 2020 206f 7574 7075 7473 3d5b 7b22 4222     outputs=[{"B"
+0000fb20: 3a20 3330 307d 2c20 7b22 4222 3a20 3330  : 300}, {"B": 30
+0000fb30: 317d 5d2c 0a20 2020 2020 2020 2066 6565  1}],.        fee
+0000fb40: 6462 6163 6b73 3d5b 7b22 4122 3a20 3230  dbacks=[{"A": 20
+0000fb50: 307d 2c20 7b22 4122 3a20 3230 317d 5d2c  0}, {"A": 201}],
+0000fb60: 0a20 2020 2020 2020 206a 6f69 6e5f 6b65  .        join_ke
+0000fb70: 7973 3d5b 2231 3233 3435 222c 2022 3637  ys=["12345", "67
+0000fb80: 3839 3022 5d20 6966 206b 7761 7267 7320  890"] if kwargs 
+0000fb90: 656c 7365 205b 2236 3738 3930 222c 2022  else ["67890", "
+0000fba0: 3132 3334 3522 5d2c 0a20 2020 2020 2020  12345"],.       
+0000fbb0: 2076 6572 7369 6f6e 3d76 6572 7369 6f6e   version=version
+0000fbc0: 2c0a 2020 2020 2020 2020 6967 6e6f 7265  ,.        ignore
+0000fbd0: 5f69 6e70 7574 733d 4e6f 6e65 2c0a 2020  _inputs=None,.  
+0000fbe0: 2020 2020 2020 7469 6d65 7374 616d 7073        timestamps
+0000fbf0: 3d74 6573 745f 7469 6d65 7374 616d 7073  =test_timestamps
+0000fc00: 5f6c 6973 742c 0a20 2020 2020 2020 2073  _list,.        s
+0000fc10: 6f72 745f 6f6e 5f74 696d 6573 7461 6d70  ort_on_timestamp
+0000fc20: 3d54 7275 652c 0a20 2020 2020 2020 2072  =True,.        r
+0000fc30: 756e 5f69 643d 7275 6e5f 6964 2c0a 2020  un_id=run_id,.  
+0000fc40: 2020 2020 2020 7461 6773 3d65 7870 6563        tags=expec
+0000fc50: 7465 645f 7461 6773 5f70 6172 616d 2c0a  ted_tags_param,.
+0000fc60: 2020 2020 290a 2020 2020 6d6f 636b 5f67      ).    mock_g
+0000fc70: 656e 6572 6174 655f 7072 6564 732e 6173  enerate_preds.as
+0000fc80: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
+0000fc90: 290a 2020 2020 6d6f 636b 5f67 656e 6572  ).    mock_gener
+0000fca0: 6174 655f 6665 6564 6261 636b 2e61 7373  ate_feedback.ass
+0000fcb0: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
+0000fcc0: 0a0a 2020 2020 6d6f 636b 5f73 616d 706c  ..    mock_sampl
+0000fcd0: 655f 7265 636f 7264 732e 6173 7365 7274  e_records.assert
+0000fce0: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+0000fcf0: 6828 0a20 2020 2020 2020 2032 2c0a 2020  h(.        2,.  
+0000fd00: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+0000fd10: 205b 7b22 4122 3a20 3130 307d 2c20 7b22   [{"A": 100}, {"
+0000fd20: 4122 3a20 3130 317d 5d2c 0a20 2020 2020  A": 101}],.     
+0000fd30: 2020 205b 7b22 4222 3a20 3330 307d 2c20     [{"B": 300}, 
+0000fd40: 7b22 4222 3a20 3330 317d 5d2c 0a20 2020  {"B": 301}],.   
+0000fd50: 2020 2020 205b 7b22 4122 3a20 3230 307d       [{"A": 200}
+0000fd60: 2c20 7b22 4122 3a20 3230 317d 5d2c 0a20  , {"A": 201}],. 
+0000fd70: 2020 2020 2020 2063 6c69 656e 742e 5f72         client._r
+0000fd80: 6573 6f6c 7665 5f6a 6f69 6e5f 6b65 7973  esolve_join_keys
+0000fd90: 282a 2a6b 7761 7267 7329 2c0a 2020 2020  (**kwargs),.    
+0000fda0: 2020 2020 7465 7374 5f74 696d 6573 7461      test_timesta
+0000fdb0: 6d70 735f 6c69 7374 2c0a 2020 2020 2020  mps_list,.      
+0000fdc0: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
+0000fdd0: 7061 7261 6d2c 0a20 2020 2029 0a0a 2020  param,.    )..  
+0000fde0: 2020 6966 206b 7761 7267 733a 0a20 2020    if kwargs:.   
+0000fdf0: 2020 2020 206d 6f63 6b5f 6a6f 696e 5f6b       mock_join_k
+0000fe00: 6579 5f67 656e 2e61 7373 6572 745f 6e6f  ey_gen.assert_no
+0000fe10: 745f 6361 6c6c 6564 2829 0a20 2020 2065  t_called().    e
+0000fe20: 6c73 653a 0a20 2020 2020 2020 206d 6f63  lse:.        moc
+0000fe30: 6b5f 6a6f 696e 5f6b 6579 5f67 656e 2e61  k_join_key_gen.a
+0000fe40: 7373 6572 745f 6361 6c6c 6564 2829 0a0a  ssert_called()..
+0000fe50: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
+0000fe60: 7261 6d65 7472 697a 6528 0a20 2020 2022  rametrize(.    "
+0000fe70: 7465 7374 5f74 696d 6573 7461 6d70 732c  test_timestamps,
+0000fe80: 2074 6573 745f 7469 6d65 7374 616d 7073   test_timestamps
+0000fe90: 5f6c 6973 7422 2c0a 2020 2020 5b0a 2020  _list",.    [.  
+0000fea0: 2020 2020 2020 284e 6f6e 652c 204e 6f6e        (None, Non
+0000feb0: 6529 2c0a 2020 2020 2020 2020 285b 4355  e),.        ([CU
+0000fec0: 5252 454e 545f 5449 4d45 5d20 2a20 322c  RRENT_TIME] * 2,
+0000fed0: 205b 4355 5252 454e 545f 5449 4d45 5d20   [CURRENT_TIME] 
+0000fee0: 2a20 3229 2c0a 2020 2020 2020 2020 286e  * 2),.        (n
+0000fef0: 702e 6172 7261 7928 5b43 5552 5245 4e54  p.array([CURRENT
+0000ff00: 5f54 494d 455d 202a 2032 292c 205b 4355  _TIME] * 2), [CU
+0000ff10: 5252 454e 545f 5449 4d45 5d20 2a20 3229  RRENT_TIME] * 2)
+0000ff20: 2c0a 2020 2020 5d2c 0a29 0a40 7079 7465  ,.    ],.).@pyte
+0000ff30: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
+0000ff40: 697a 6528 0a20 2020 2028 2274 6573 745f  ize(.    ("test_
+0000ff50: 696e 7075 7473 222c 2022 7465 7374 5f6f  inputs", "test_o
+0000ff60: 7574 7075 7473 222c 2022 7465 7374 5f66  utputs", "test_f
+0000ff70: 6565 6462 6163 6b73 2229 2c0a 2020 2020  eedbacks"),.    
+0000ff80: 5445 5354 5f49 4e50 5554 535f 4f55 5450  TEST_INPUTS_OUTP
+0000ff90: 5554 535f 4645 4544 4241 434b 532c 0a29  UTS_FEEDBACKS,.)
+0000ffa0: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
+0000ffb0: 7261 6d65 7472 697a 6528 2276 6572 7369  rametrize("versi
+0000ffc0: 6f6e 222c 205b 4e6f 6e65 2c20 3130 2c20  on", [None, 10, 
+0000ffd0: 2231 2e32 2e33 225d 290a 4070 7974 6573  "1.2.3"]).@pytes
 0000ffe0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-0000fff0: 7a65 280a 2020 2020 226b 7761 7267 7322  ze(.    "kwargs"
-00010000: 2c0a 2020 2020 5b0a 2020 2020 2020 2020  ,.    [.        
-00010010: 7b22 6a6f 696e 5f6b 6579 7322 3a20 5b22  {"join_keys": ["
-00010020: 3534 3332 3122 2c20 2236 3738 3930 225d  54321", "67890"]
-00010030: 7d2c 0a20 2020 2020 2020 207b 226a 6f69  },.        {"joi
-00010040: 6e5f 6b65 7973 223a 2070 642e 5365 7269  n_keys": pd.Seri
-00010050: 6573 285b 2235 3433 3231 222c 2022 3637  es(["54321", "67
-00010060: 3839 3022 5d29 7d2c 0a20 2020 2020 2020  890"])},.       
-00010070: 207b 7d2c 0a20 2020 205d 2c0a 290a 406d   {},.    ],.).@m
-00010080: 6f63 6b2e 7061 7463 6828 2267 616e 7472  ock.patch("gantr
-00010090: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
-000100a0: 5f72 6573 6f6c 7665 5f6a 6f69 6e5f 6b65  _resolve_join_ke
-000100b0: 7973 2229 0a40 6d6f 636b 2e70 6174 6368  ys").@mock.patch
-000100c0: 280a 2020 2020 2267 616e 7472 792e 6c6f  (.    "gantry.lo
-000100d0: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-000100e0: 7279 2e5f 6c6f 675f 7072 6564 6963 7469  ry._log_predicti
-000100f0: 6f6e 5f61 6e64 5f66 6565 6462 6163 6b5f  on_and_feedback_
-00010100: 6576 656e 7473 222c 0a20 2020 2072 6574  events",.    ret
-00010110: 7572 6e5f 7661 6c75 653d 284e 6f6e 652c  urn_value=(None,
-00010120: 205b 2231 3233 3435 222c 2022 3637 3839   ["12345", "6789
-00010130: 3022 5d29 2c0a 290a 406d 6f63 6b2e 7061  0"]),.).@mock.pa
-00010140: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
-00010150: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
-00010160: 2e5f 6c6f 675f 7072 6564 6963 7469 6f6e  ._log_prediction
-00010170: 5f65 7665 6e74 7322 290a 406d 6f63 6b2e  _events").@mock.
-00010180: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-00010190: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-000101a0: 7279 2e5f 6c6f 675f 6665 6564 6261 636b  ry._log_feedback
-000101b0: 5f65 7665 6e74 7322 290a 406d 6f63 6b2e  _events").@mock.
-000101c0: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-000101d0: 6767 6572 2e63 6c69 656e 742e 5f73 616d  gger.client._sam
-000101e0: 706c 655f 7265 636f 7264 7322 2c20 7369  ple_records", si
-000101f0: 6465 5f65 6666 6563 743d 636c 6965 6e74  de_effect=client
-00010200: 2e5f 7361 6d70 6c65 5f72 6563 6f72 6473  ._sample_records
+0000fff0: 7a65 2822 7461 6773 2c20 726f 775f 7461  ze("tags, row_ta
+00010000: 6773 2c20 676c 6f62 616c 5f74 6167 732c  gs, global_tags,
+00010010: 2065 7870 6563 7465 645f 7461 6773 5f70   expected_tags_p
+00010020: 6172 616d 222c 2054 4553 545f 5441 4753  aram", TEST_TAGS
+00010030: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
+00010040: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
+00010050: 226b 7761 7267 7322 2c0a 2020 2020 5b0a  "kwargs",.    [.
+00010060: 2020 2020 2020 2020 7b22 6a6f 696e 5f6b          {"join_k
+00010070: 6579 7322 3a20 5b22 3534 3332 3122 2c20  eys": ["54321", 
+00010080: 2236 3738 3930 225d 7d2c 0a20 2020 2020  "67890"]},.     
+00010090: 2020 207b 226a 6f69 6e5f 6b65 7973 223a     {"join_keys":
+000100a0: 2070 642e 5365 7269 6573 285b 2235 3433   pd.Series(["543
+000100b0: 3231 222c 2022 3637 3839 3022 5d29 7d2c  21", "67890"])},
+000100c0: 0a20 2020 2020 2020 207b 7d2c 0a20 2020  .        {},.   
+000100d0: 205d 2c0a 290a 406d 6f63 6b2e 7061 7463   ],.).@mock.patc
+000100e0: 6828 2267 616e 7472 792e 6c6f 6767 6572  h("gantry.logger
+000100f0: 2e63 6c69 656e 742e 5f72 6573 6f6c 7665  .client._resolve
+00010100: 5f6a 6f69 6e5f 6b65 7973 2229 0a40 6d6f  _join_keys").@mo
+00010110: 636b 2e70 6174 6368 280a 2020 2020 2267  ck.patch(.    "g
+00010120: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+00010130: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
+00010140: 7072 6564 6963 7469 6f6e 5f61 6e64 5f66  prediction_and_f
+00010150: 6565 6462 6163 6b5f 6576 656e 7473 222c  eedback_events",
+00010160: 0a20 2020 2072 6574 7572 6e5f 7661 6c75  .    return_valu
+00010170: 653d 284e 6f6e 652c 205b 2231 3233 3435  e=(None, ["12345
+00010180: 222c 2022 3637 3839 3022 5d29 2c0a 290a  ", "67890"]),.).
+00010190: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
+000101a0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
+000101b0: 742e 4761 6e74 7279 2e5f 6c6f 675f 7072  t.Gantry._log_pr
+000101c0: 6564 6963 7469 6f6e 5f65 7665 6e74 7322  ediction_events"
+000101d0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+000101e0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+000101f0: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
+00010200: 6665 6564 6261 636b 5f65 7665 6e74 7322  feedback_events"
 00010210: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
 00010220: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00010230: 656e 742e 5f64 6566 6175 6c74 5f6a 6f69  ent._default_joi
-00010240: 6e5f 6b65 795f 6765 6e22 290a 6465 6620  n_key_gen").def 
-00010250: 7465 7374 5f73 696e 676c 655f 6c6f 675f  test_single_log_
-00010260: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-00010270: 636b 280a 2020 2020 6d6f 636b 5f6a 6f69  ck(.    mock_joi
-00010280: 6e5f 6b65 795f 6765 6e2c 0a20 2020 206d  n_key_gen,.    m
-00010290: 6f63 6b5f 7361 6d70 6c65 5f72 6563 6f72  ock_sample_recor
-000102a0: 6473 2c0a 2020 2020 6d6f 636b 5f6c 6f67  ds,.    mock_log
-000102b0: 5f66 6565 6462 6163 6b2c 0a20 2020 206d  _feedback,.    m
-000102c0: 6f63 6b5f 6c6f 675f 7072 6564 732c 0a20  ock_log_preds,. 
-000102d0: 2020 206d 6f63 6b5f 6c6f 675f 7072 6564     mock_log_pred
-000102e0: 735f 616e 645f 6665 6564 6261 636b 2c0a  s_and_feedback,.
-000102f0: 2020 2020 6d6f 636b 5f72 6573 6f6c 7665      mock_resolve
-00010300: 5f6a 6f69 6e5f 6b65 7973 2c0a 2020 2020  _join_keys,.    
-00010310: 6b77 6172 6773 2c0a 2020 2020 7665 7273  kwargs,.    vers
-00010320: 696f 6e2c 0a20 2020 2074 6167 732c 0a20  ion,.    tags,. 
-00010330: 2020 2072 6f77 5f74 6167 732c 0a20 2020     row_tags,.   
-00010340: 2067 6c6f 6261 6c5f 7461 6773 2c0a 2020   global_tags,.  
-00010350: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
-00010360: 7061 7261 6d2c 0a20 2020 2074 6573 745f  param,.    test_
-00010370: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
-00010380: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
-00010390: 6c69 7374 2c0a 2020 2020 7465 7374 5f69  list,.    test_i
-000103a0: 6e70 7574 732c 0a20 2020 2074 6573 745f  nputs,.    test_
-000103b0: 6f75 7470 7574 732c 0a20 2020 2074 6573  outputs,.    tes
-000103c0: 745f 6665 6564 6261 636b 732c 0a20 2020  t_feedbacks,.   
-000103d0: 2063 6c69 5f6f 626a 2c0a 293a 0a20 2020   cli_obj,.):.   
-000103e0: 206d 6f63 6b5f 6a6f 696e 5f6b 6579 5f67   mock_join_key_g
-000103f0: 656e 2e73 6964 655f 6566 6665 6374 203d  en.side_effect =
-00010400: 205b 2236 3738 3930 222c 2022 3132 3334   ["67890", "1234
-00010410: 3522 5d0a 2020 2020 6d6f 636b 5f72 6573  5"].    mock_res
-00010420: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2e72  olve_join_keys.r
-00010430: 6574 7572 6e5f 7661 6c75 6520 3d20 5b22  eturn_value = ["
-00010440: 3132 3334 3522 2c20 2236 3738 3930 225d  12345", "67890"]
-00010450: 2069 6620 6b77 6172 6773 2065 6c73 6520   if kwargs else 
-00010460: 4e6f 6e65 0a20 2020 2063 6c69 5f6f 626a  None.    cli_obj
-00010470: 2e6c 6f67 280a 2020 2020 2020 2020 6170  .log(.        ap
-00010480: 706c 6963 6174 696f 6e3d 2266 6f6f 6261  plication="fooba
-00010490: 7222 2c0a 2020 2020 2020 2020 7665 7273  r",.        vers
-000104a0: 696f 6e3d 7665 7273 696f 6e2c 0a20 2020  ion=version,.   
-000104b0: 2020 2020 2069 6e70 7574 733d 7465 7374       inputs=test
-000104c0: 5f69 6e70 7574 732c 0a20 2020 2020 2020  _inputs,.       
-000104d0: 206f 7574 7075 7473 3d74 6573 745f 6f75   outputs=test_ou
-000104e0: 7470 7574 732c 0a20 2020 2020 2020 2066  tputs,.        f
-000104f0: 6565 6462 6163 6b73 3d74 6573 745f 6665  eedbacks=test_fe
-00010500: 6564 6261 636b 732c 0a20 2020 2020 2020  edbacks,.       
-00010510: 2074 696d 6573 7461 6d70 733d 7465 7374   timestamps=test
-00010520: 5f74 696d 6573 7461 6d70 732c 0a20 2020  _timestamps,.   
-00010530: 2020 2020 2073 6f72 745f 6f6e 5f74 696d       sort_on_tim
-00010540: 6573 7461 6d70 3d54 7275 652c 0a20 2020  estamp=True,.   
-00010550: 2020 2020 2073 616d 706c 655f 7261 7465       sample_rate
-00010560: 3d31 2c0a 2020 2020 2020 2020 676c 6f62  =1,.        glob
-00010570: 616c 5f74 6167 733d 676c 6f62 616c 5f74  al_tags=global_t
-00010580: 6167 732c 0a20 2020 2020 2020 2074 6167  ags,.        tag
-00010590: 733d 7461 6773 2c0a 2020 2020 2020 2020  s=tags,.        
-000105a0: 726f 775f 7461 6773 3d72 6f77 5f74 6167  row_tags=row_tag
-000105b0: 732c 0a20 2020 2020 2020 202a 2a6b 7761  s,.        **kwa
-000105c0: 7267 732c 0a20 2020 2029 0a0a 2020 2020  rgs,.    )..    
-000105d0: 6d6f 636b 5f6c 6f67 5f70 7265 6473 5f61  mock_log_preds_a
-000105e0: 6e64 5f66 6565 6462 6163 6b2e 6173 7365  nd_feedback.asse
-000105f0: 7274 5f63 616c 6c65 645f 6f6e 6365 5f77  rt_called_once_w
-00010600: 6974 6828 0a20 2020 2020 2020 2061 7070  ith(.        app
-00010610: 6c69 6361 7469 6f6e 3d22 666f 6f62 6172  lication="foobar
-00010620: 222c 0a20 2020 2020 2020 2069 6e70 7574  ",.        input
-00010630: 733d 5b7b 2241 223a 2031 3030 7d2c 207b  s=[{"A": 100}, {
-00010640: 2241 223a 2031 3031 7d5d 2c0a 2020 2020  "A": 101}],.    
-00010650: 2020 2020 6f75 7470 7574 733d 5b7b 2242      outputs=[{"B
-00010660: 223a 2033 3030 7d2c 207b 2242 223a 2033  ": 300}, {"B": 3
-00010670: 3031 7d5d 2c0a 2020 2020 2020 2020 6665  01}],.        fe
-00010680: 6564 6261 636b 733d 5b7b 2241 223a 2032  edbacks=[{"A": 2
-00010690: 3030 7d2c 207b 2241 223a 2032 3031 7d5d  00}, {"A": 201}]
-000106a0: 2c0a 2020 2020 2020 2020 6a6f 696e 5f6b  ,.        join_k
-000106b0: 6579 733d 5b22 3132 3334 3522 2c20 2236  eys=["12345", "6
-000106c0: 3738 3930 225d 2069 6620 6b77 6172 6773  7890"] if kwargs
-000106d0: 2065 6c73 6520 5b22 3637 3839 3022 2c20   else ["67890", 
-000106e0: 2231 3233 3435 225d 2c0a 2020 2020 2020  "12345"],.      
-000106f0: 2020 7665 7273 696f 6e3d 7665 7273 696f    version=versio
-00010700: 6e2c 0a20 2020 2020 2020 2069 676e 6f72  n,.        ignor
-00010710: 655f 696e 7075 7473 3d4e 6f6e 652c 0a20  e_inputs=None,. 
-00010720: 2020 2020 2020 2074 696d 6573 7461 6d70         timestamp
-00010730: 733d 7465 7374 5f74 696d 6573 7461 6d70  s=test_timestamp
-00010740: 735f 6c69 7374 2c0a 2020 2020 2020 2020  s_list,.        
-00010750: 736f 7274 5f6f 6e5f 7469 6d65 7374 616d  sort_on_timestam
-00010760: 703d 5472 7565 2c0a 2020 2020 2020 2020  p=True,.        
-00010770: 7461 6773 3d65 7870 6563 7465 645f 7461  tags=expected_ta
-00010780: 6773 5f70 6172 616d 2c0a 2020 2020 2020  gs_param,.      
-00010790: 2020 6173 5f62 6174 6368 3d46 616c 7365    as_batch=False
-000107a0: 2c0a 2020 2020 290a 2020 2020 6d6f 636b  ,.    ).    mock
-000107b0: 5f6c 6f67 5f70 7265 6473 2e61 7373 6572  _log_preds.asser
-000107c0: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
-000107d0: 2020 206d 6f63 6b5f 6c6f 675f 6665 6564     mock_log_feed
-000107e0: 6261 636b 2e61 7373 6572 745f 6e6f 745f  back.assert_not_
-000107f0: 6361 6c6c 6564 2829 0a0a 2020 2020 6d6f  called()..    mo
-00010800: 636b 5f73 616d 706c 655f 7265 636f 7264  ck_sample_record
-00010810: 732e 6173 7365 7274 5f63 616c 6c65 645f  s.assert_called_
-00010820: 6f6e 6365 5f77 6974 6828 0a20 2020 2020  once_with(.     
-00010830: 2020 2032 2c0a 2020 2020 2020 2020 312c     2,.        1,
-00010840: 0a20 2020 2020 2020 205b 7b22 4122 3a20  .        [{"A": 
-00010850: 3130 307d 2c20 7b22 4122 3a20 3130 317d  100}, {"A": 101}
-00010860: 5d2c 0a20 2020 2020 2020 205b 7b22 4222  ],.        [{"B"
-00010870: 3a20 3330 307d 2c20 7b22 4222 3a20 3330  : 300}, {"B": 30
-00010880: 317d 5d2c 0a20 2020 2020 2020 205b 7b22  1}],.        [{"
-00010890: 4122 3a20 3230 307d 2c20 7b22 4122 3a20  A": 200}, {"A": 
-000108a0: 3230 317d 5d2c 0a20 2020 2020 2020 2063  201}],.        c
-000108b0: 6c69 656e 742e 5f72 6573 6f6c 7665 5f6a  lient._resolve_j
-000108c0: 6f69 6e5f 6b65 7973 282a 2a6b 7761 7267  oin_keys(**kwarg
-000108d0: 7329 2c0a 2020 2020 2020 2020 7465 7374  s),.        test
-000108e0: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
-000108f0: 2c0a 2020 2020 2020 2020 6578 7065 6374  ,.        expect
-00010900: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
-00010910: 2020 2029 0a0a 2020 2020 6966 206b 7761     )..    if kwa
-00010920: 7267 733a 0a20 2020 2020 2020 206d 6f63  rgs:.        moc
-00010930: 6b5f 6a6f 696e 5f6b 6579 5f67 656e 2e61  k_join_key_gen.a
-00010940: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
-00010950: 2829 0a20 2020 2065 6c73 653a 0a20 2020  ().    else:.   
-00010960: 2020 2020 206d 6f63 6b5f 6a6f 696e 5f6b       mock_join_k
-00010970: 6579 5f67 656e 2e61 7373 6572 745f 6361  ey_gen.assert_ca
-00010980: 6c6c 6564 2829 0a0a 0a40 7079 7465 7374  lled()...@pytest
-00010990: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-000109a0: 6528 0a20 2020 2022 696e 7075 7473 2c20  e(.    "inputs, 
-000109b0: 6f75 7470 7574 732c 2066 6565 6462 6163  outputs, feedbac
-000109c0: 6b73 222c 0a20 2020 205b 0a20 2020 2020  ks",.    [.     
-000109d0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-000109e0: 206e 702e 6172 7261 7928 5b32 3030 2c20   np.array([200, 
-000109f0: 3230 315d 292c 0a20 2020 2020 2020 2020  201]),.         
-00010a00: 2020 205b 7b22 4222 3a20 3230 307d 2c20     [{"B": 200}, 
-00010a10: 7b22 4222 3a20 3230 317d 5d2c 0a20 2020  {"B": 201}],.   
-00010a20: 2020 2020 2020 2020 205b 7b22 4122 3a20           [{"A": 
-00010a30: 3230 307d 2c20 7b22 4122 3a20 3230 317d  200}, {"A": 201}
-00010a40: 5d2c 0a20 2020 2020 2020 2029 2c0a 2020  ],.        ),.  
-00010a50: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-00010a60: 2020 2020 6e70 2e61 7272 6179 285b 3230      np.array([20
-00010a70: 302c 2032 3031 5d29 2c0a 2020 2020 2020  0, 201]),.      
-00010a80: 2020 2020 2020 5b7b 2242 223a 2032 3030        [{"B": 200
-00010a90: 7d2c 207b 2242 223a 2032 3031 7d5d 2c0a  }, {"B": 201}],.
-00010aa0: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
-00010ab0: 2c0a 2020 2020 2020 2020 292c 0a20 2020  ,.        ),.   
-00010ac0: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
-00010ad0: 2020 206e 702e 6172 7261 7928 5b32 3030     np.array([200
-00010ae0: 2c20 3230 315d 292c 0a20 2020 2020 2020  , 201]),.       
-00010af0: 2020 2020 206e 702e 6172 7261 7928 5b32       np.array([2
-00010b00: 3030 2c20 3230 315d 292c 0a20 2020 2020  00, 201]),.     
-00010b10: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
-00010b20: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00010b30: 280a 2020 2020 2020 2020 2020 2020 5b7b  (.            [{
-00010b40: 2242 223a 2032 3030 7d2c 207b 2242 223a  "B": 200}, {"B":
-00010b50: 2032 3031 7d5d 2c0a 2020 2020 2020 2020   201}],.        
-00010b60: 2020 2020 6e70 2e61 7272 6179 285b 3230      np.array([20
-00010b70: 302c 2032 3031 5d29 2c0a 2020 2020 2020  0, 201]),.      
-00010b80: 2020 2020 2020 5b7b 2241 223a 2032 3030        [{"A": 200
-00010b90: 7d2c 207b 2241 223a 2032 3031 7d5d 2c0a  }, {"A": 201}],.
-00010ba0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00010bb0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-00010bc0: 205b 7b22 4222 3a20 3230 307d 2c20 7b22   [{"B": 200}, {"
-00010bd0: 4222 3a20 3230 317d 5d2c 0a20 2020 2020  B": 201}],.     
-00010be0: 2020 2020 2020 205b 7b22 4122 3a20 3230         [{"A": 20
-00010bf0: 307d 2c20 7b22 4122 3a20 3230 317d 5d2c  0}, {"A": 201}],
-00010c00: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00010c10: 6172 7261 7928 5b32 3030 2c20 3230 315d  array([200, 201]
-00010c20: 292c 0a20 2020 2020 2020 2029 2c0a 2020  ),.        ),.  
-00010c30: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-00010c40: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
-00010c50: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
-00010c60: 2020 2020 2020 2020 6e70 2e61 7272 6179          np.array
-00010c70: 285b 3230 302c 2032 3031 5d29 2c0a 2020  ([200, 201]),.  
-00010c80: 2020 2020 2020 292c 0a20 2020 205d 2c0a        ),.    ],.
-00010c90: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-00010ca0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00010cb0: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
-00010cc0: 7072 6564 6963 7469 6f6e 5f61 6e64 5f66  prediction_and_f
-00010cd0: 6565 6462 6163 6b5f 6576 656e 7473 2229  eedback_events")
-00010ce0: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
-00010cf0: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
-00010d00: 6e74 2e47 616e 7472 792e 5f6c 6f67 5f70  nt.Gantry._log_p
-00010d10: 7265 6469 6374 696f 6e5f 6576 656e 7473  rediction_events
-00010d20: 2229 0a40 6d6f 636b 2e70 6174 6368 2822  ").@mock.patch("
-00010d30: 6761 6e74 7279 2e6c 6f67 6765 722e 636c  gantry.logger.cl
-00010d40: 6965 6e74 2e47 616e 7472 792e 5f6c 6f67  ient.Gantry._log
-00010d50: 5f66 6565 6462 6163 6b5f 6576 656e 7473  _feedback_events
-00010d60: 2229 0a64 6566 2074 6573 745f 6c6f 675f  ").def test_log_
-00010d70: 7265 636f 7264 735f 7072 6564 735f 616e  records_preds_an
-00010d80: 645f 6665 6564 6261 636b 5f77 726f 6e67  d_feedback_wrong
-00010d90: 5f6e 705f 6172 7261 7928 0a20 2020 206d  _np_array(.    m
-00010da0: 6f63 6b5f 6665 6564 6261 636b 2c0a 2020  ock_feedback,.  
-00010db0: 2020 6d6f 636b 5f70 7265 6473 2c0a 2020    mock_preds,.  
-00010dc0: 2020 6d6f 636b 5f70 7265 6473 5f61 6e64    mock_preds_and
-00010dd0: 5f66 6565 6462 6163 6b2c 0a20 2020 2069  _feedback,.    i
-00010de0: 6e70 7574 732c 0a20 2020 206f 7574 7075  nputs,.    outpu
-00010df0: 7473 2c0a 2020 2020 6665 6564 6261 636b  ts,.    feedback
-00010e00: 732c 0a20 2020 2063 6c69 5f6f 626a 2c0a  s,.    cli_obj,.
-00010e10: 293a 0a20 2020 2061 7373 6572 7420 280a  ):.    assert (.
-00010e20: 2020 2020 2020 2020 636c 695f 6f62 6a2e          cli_obj.
-00010e30: 6c6f 675f 7265 636f 7264 7328 0a20 2020  log_records(.   
-00010e40: 2020 2020 2020 2020 2061 7070 6c69 6361           applica
-00010e50: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
-00010e60: 2020 2020 2020 2020 2020 2076 6572 7369             versi
-00010e70: 6f6e 3d22 312e 322e 3322 2c0a 2020 2020  on="1.2.3",.    
-00010e80: 2020 2020 2020 2020 696e 7075 7473 3d69          inputs=i
-00010e90: 6e70 7574 732c 0a20 2020 2020 2020 2020  nputs,.         
-00010ea0: 2020 206f 7574 7075 7473 3d6f 7574 7075     outputs=outpu
-00010eb0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-00010ec0: 6665 6564 6261 636b 733d 6665 6564 6261  feedbacks=feedba
-00010ed0: 636b 732c 0a20 2020 2020 2020 2020 2020  cks,.           
-00010ee0: 2074 696d 6573 7461 6d70 733d 4e6f 6e65   timestamps=None
-00010ef0: 2c0a 2020 2020 2020 2020 2020 2020 736f  ,.            so
-00010f00: 7274 5f6f 6e5f 7469 6d65 7374 616d 703d  rt_on_timestamp=
-00010f10: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00010f20: 2020 7361 6d70 6c65 5f72 6174 653d 312c    sample_rate=1,
-00010f30: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
-00010f40: 6e5f 6b65 7973 3d5b 2266 6f6f 6261 7222  n_keys=["foobar"
-00010f50: 2c20 2262 6172 6261 7a22 5d2c 0a20 2020  , "barbaz"],.   
-00010f60: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-00010f70: 7320 4e6f 6e65 0a20 2020 2029 0a20 2020  s None.    ).   
-00010f80: 206d 6f63 6b5f 7072 6564 735f 616e 645f   mock_preds_and_
-00010f90: 6665 6564 6261 636b 2e61 7373 6572 745f  feedback.assert_
-00010fa0: 6e6f 745f 6361 6c6c 6564 2829 0a20 2020  not_called().   
-00010fb0: 206d 6f63 6b5f 7072 6564 732e 6173 7365   mock_preds.asse
-00010fc0: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00010fd0: 2020 2020 6d6f 636b 5f66 6565 6462 6163      mock_feedbac
-00010fe0: 6b2e 6173 7365 7274 5f6e 6f74 5f63 616c  k.assert_not_cal
-00010ff0: 6c65 6428 290a 0a0a 4070 7974 6573 742e  led()...@pytest.
-00011000: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-00011010: 280a 2020 2020 2269 6e70 7574 732c 206f  (.    "inputs, o
-00011020: 7574 7075 7473 2c20 6665 6564 6261 636b  utputs, feedback
-00011030: 7322 2c0a 2020 2020 5b0a 2020 2020 2020  s",.    [.      
-00011040: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00011050: 6e70 2e61 7272 6179 285b 3230 302c 2032  np.array([200, 2
-00011060: 3031 5d29 2c0a 2020 2020 2020 2020 2020  01]),.          
-00011070: 2020 5b7b 2242 223a 2032 3030 7d2c 207b    [{"B": 200}, {
-00011080: 2242 223a 2032 3031 7d5d 2c0a 2020 2020  "B": 201}],.    
-00011090: 2020 2020 2020 2020 5b7b 2241 223a 2032          [{"A": 2
-000110a0: 3030 7d2c 207b 2241 223a 2032 3031 7d5d  00}, {"A": 201}]
-000110b0: 2c0a 2020 2020 2020 2020 292c 0a20 2020  ,.        ),.   
-000110c0: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
-000110d0: 2020 206e 702e 6172 7261 7928 5b32 3030     np.array([200
-000110e0: 2c20 3230 315d 292c 0a20 2020 2020 2020  , 201]),.       
-000110f0: 2020 2020 205b 7b22 4222 3a20 3230 307d       [{"B": 200}
-00011100: 2c20 7b22 4222 3a20 3230 317d 5d2c 0a20  , {"B": 201}],. 
-00011110: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
-00011120: 0a20 2020 2020 2020 2029 2c0a 2020 2020  .        ),.    
-00011130: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00011140: 2020 6e70 2e61 7272 6179 285b 3230 302c    np.array([200,
-00011150: 2032 3031 5d29 2c0a 2020 2020 2020 2020   201]),.        
-00011160: 2020 2020 6e70 2e61 7272 6179 285b 3230      np.array([20
-00011170: 302c 2032 3031 5d29 2c0a 2020 2020 2020  0, 201]),.      
-00011180: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
-00011190: 2020 2020 292c 0a20 2020 2020 2020 2028      ),.        (
-000111a0: 0a20 2020 2020 2020 2020 2020 205b 7b22  .            [{"
-000111b0: 4222 3a20 3230 307d 2c20 7b22 4222 3a20  B": 200}, {"B": 
-000111c0: 3230 317d 5d2c 0a20 2020 2020 2020 2020  201}],.         
-000111d0: 2020 206e 702e 6172 7261 7928 5b32 3030     np.array([200
-000111e0: 2c20 3230 315d 292c 0a20 2020 2020 2020  , 201]),.       
-000111f0: 2020 2020 205b 7b22 4122 3a20 3230 307d       [{"A": 200}
-00011200: 2c20 7b22 4122 3a20 3230 317d 5d2c 0a20  , {"A": 201}],. 
-00011210: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00011220: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00011230: 5b7b 2242 223a 2032 3030 7d2c 207b 2242  [{"B": 200}, {"B
-00011240: 223a 2032 3031 7d5d 2c0a 2020 2020 2020  ": 201}],.      
-00011250: 2020 2020 2020 5b7b 2241 223a 2032 3030        [{"A": 200
-00011260: 7d2c 207b 2241 223a 2032 3031 7d5d 2c0a  }, {"A": 201}],.
-00011270: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
-00011280: 7272 6179 285b 3230 302c 2032 3031 5d29  rray([200, 201])
-00011290: 2c0a 2020 2020 2020 2020 292c 0a20 2020  ,.        ),.   
-000112a0: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
-000112b0: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
-000112c0: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
-000112d0: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
-000112e0: 5b32 3030 2c20 3230 315d 292c 0a20 2020  [200, 201]),.   
-000112f0: 2020 2020 2029 2c0a 2020 2020 5d2c 0a29       ),.    ],.)
-00011300: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
-00011310: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
-00011320: 6e74 2e47 616e 7472 792e 5f67 656e 6572  nt.Gantry._gener
-00011330: 6174 655f 7072 6564 6963 7469 6f6e 5f61  ate_prediction_a
-00011340: 6e64 5f66 6565 6462 6163 6b5f 6576 656e  nd_feedback_even
-00011350: 7473 2229 0a40 6d6f 636b 2e70 6174 6368  ts").@mock.patch
-00011360: 2822 6761 6e74 7279 2e6c 6f67 6765 722e  ("gantry.logger.
-00011370: 636c 6965 6e74 2e47 616e 7472 792e 5f67  client.Gantry._g
-00011380: 656e 6572 6174 655f 7072 6564 6963 7469  enerate_predicti
-00011390: 6f6e 5f65 7665 6e74 7322 290a 406d 6f63  on_events").@moc
-000113a0: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-000113b0: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
-000113c0: 6e74 7279 2e5f 6765 6e65 7261 7465 5f66  ntry._generate_f
-000113d0: 6565 6462 6163 6b5f 6576 656e 7473 2229  eedback_events")
-000113e0: 0a64 6566 2074 6573 745f 6765 6e65 7261  .def test_genera
-000113f0: 7465 5f72 6563 6f72 6473 5f70 7265 6473  te_records_preds
-00011400: 5f61 6e64 5f66 6565 6462 6163 6b5f 7772  _and_feedback_wr
-00011410: 6f6e 675f 6e70 5f61 7272 6179 280a 2020  ong_np_array(.  
-00011420: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
-00011430: 6665 6564 6261 636b 2c0a 2020 2020 6d6f  feedback,.    mo
-00011440: 636b 5f67 656e 6572 6174 655f 7072 6564  ck_generate_pred
-00011450: 732c 0a20 2020 206d 6f63 6b5f 6765 6e65  s,.    mock_gene
-00011460: 7261 7465 5f70 7265 6473 5f61 6e64 5f66  rate_preds_and_f
-00011470: 6565 6462 6163 6b2c 0a20 2020 2069 6e70  eedback,.    inp
-00011480: 7574 732c 0a20 2020 206f 7574 7075 7473  uts,.    outputs
-00011490: 2c0a 2020 2020 6665 6564 6261 636b 732c  ,.    feedbacks,
-000114a0: 0a20 2020 2063 6c69 5f6f 626a 2c0a 293a  .    cli_obj,.):
-000114b0: 0a20 2020 2061 7373 6572 7420 280a 2020  .    assert (.  
-000114c0: 2020 2020 2020 636c 695f 6f62 6a2e 6765        cli_obj.ge
-000114d0: 6e65 7261 7465 5f72 6563 6f72 6473 280a  nerate_records(.
-000114e0: 2020 2020 2020 2020 2020 2020 6170 706c              appl
-000114f0: 6963 6174 696f 6e3d 2266 6f6f 6261 7222  ication="foobar"
-00011500: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
-00011510: 7273 696f 6e3d 2231 2e32 2e33 222c 0a20  rsion="1.2.3",. 
-00011520: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-00011530: 733d 696e 7075 7473 2c0a 2020 2020 2020  s=inputs,.      
-00011540: 2020 2020 2020 6f75 7470 7574 733d 6f75        outputs=ou
-00011550: 7470 7574 732c 0a20 2020 2020 2020 2020  tputs,.         
-00011560: 2020 2066 6565 6462 6163 6b73 3d66 6565     feedbacks=fee
-00011570: 6462 6163 6b73 2c0a 2020 2020 2020 2020  dbacks,.        
-00011580: 2020 2020 7469 6d65 7374 616d 7073 3d4e      timestamps=N
-00011590: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-000115a0: 2073 6f72 745f 6f6e 5f74 696d 6573 7461   sort_on_timesta
-000115b0: 6d70 3d54 7275 652c 0a20 2020 2020 2020  mp=True,.       
-000115c0: 2020 2020 2073 616d 706c 655f 7261 7465       sample_rate
-000115d0: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
-000115e0: 6a6f 696e 5f6b 6579 733d 5b22 666f 6f62  join_keys=["foob
-000115f0: 6172 222c 2022 6261 7262 617a 225d 2c0a  ar", "barbaz"],.
-00011600: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011610: 2020 6973 204e 6f6e 650a 2020 2020 290a    is None.    ).
-00011620: 2020 2020 6d6f 636b 5f67 656e 6572 6174      mock_generat
-00011630: 655f 7072 6564 735f 616e 645f 6665 6564  e_preds_and_feed
-00011640: 6261 636b 2e61 7373 6572 745f 6e6f 745f  back.assert_not_
-00011650: 6361 6c6c 6564 2829 0a20 2020 206d 6f63  called().    moc
-00011660: 6b5f 6765 6e65 7261 7465 5f70 7265 6473  k_generate_preds
-00011670: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-00011680: 6564 2829 0a20 2020 206d 6f63 6b5f 6765  ed().    mock_ge
-00011690: 6e65 7261 7465 5f66 6565 6462 6163 6b2e  nerate_feedback.
-000116a0: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
-000116b0: 6428 290a 0a0a 4070 7974 6573 742e 6d61  d()...@pytest.ma
-000116c0: 726b 2e70 6172 616d 6574 7269 7a65 280a  rk.parametrize(.
-000116d0: 2020 2020 2274 696d 6573 7461 6d70 7322      "timestamps"
-000116e0: 2c0a 2020 2020 5b0a 2020 2020 2020 2020  ,.    [.        
-000116f0: 6e70 2e61 7272 6179 285b 3230 302c 2032  np.array([200, 2
-00011700: 3031 5d29 2c0a 2020 2020 2020 2020 6e70  01]),.        np
-00011710: 2e61 7272 6179 285b 3230 302c 2043 5552  .array([200, CUR
-00011720: 5245 4e54 5f54 494d 455d 292c 0a20 2020  RENT_TIME]),.   
-00011730: 205d 2c0a 290a 406d 6f63 6b2e 7061 7463   ],.).@mock.patc
-00011740: 6828 2267 616e 7472 792e 6c6f 6767 6572  h("gantry.logger
-00011750: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-00011760: 6c6f 675f 7072 6564 6963 7469 6f6e 5f61  log_prediction_a
-00011770: 6e64 5f66 6565 6462 6163 6b5f 6576 656e  nd_feedback_even
-00011780: 7473 2229 0a40 6d6f 636b 2e70 6174 6368  ts").@mock.patch
-00011790: 2822 6761 6e74 7279 2e6c 6f67 6765 722e  ("gantry.logger.
-000117a0: 636c 6965 6e74 2e47 616e 7472 792e 5f6c  client.Gantry._l
-000117b0: 6f67 5f70 7265 6469 6374 696f 6e5f 6576  og_prediction_ev
-000117c0: 656e 7473 2229 0a40 6d6f 636b 2e70 6174  ents").@mock.pat
-000117d0: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
-000117e0: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
-000117f0: 5f6c 6f67 5f66 6565 6462 6163 6b5f 6576  _log_feedback_ev
-00011800: 656e 7473 2229 0a64 6566 2074 6573 745f  ents").def test_
-00011810: 6c6f 675f 7265 636f 7264 735f 7072 6564  log_records_pred
-00011820: 735f 616e 645f 6665 6564 6261 636b 5f77  s_and_feedback_w
-00011830: 726f 6e67 5f74 696d 6573 7461 6d70 7328  rong_timestamps(
-00011840: 0a20 2020 206d 6f63 6b5f 6665 6564 6261  .    mock_feedba
-00011850: 636b 2c0a 2020 2020 6d6f 636b 5f70 7265  ck,.    mock_pre
-00011860: 6473 2c0a 2020 2020 6d6f 636b 5f70 7265  ds,.    mock_pre
-00011870: 6473 5f61 6e64 5f66 6565 6462 6163 6b2c  ds_and_feedback,
-00011880: 0a20 2020 2074 696d 6573 7461 6d70 732c  .    timestamps,
-00011890: 0a20 2020 2063 6c69 5f6f 626a 2c0a 293a  .    cli_obj,.):
-000118a0: 0a20 2020 2061 7373 6572 7420 280a 2020  .    assert (.  
-000118b0: 2020 2020 2020 636c 695f 6f62 6a2e 6c6f        cli_obj.lo
-000118c0: 675f 7265 636f 7264 7328 0a20 2020 2020  g_records(.     
-000118d0: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
-000118e0: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
-000118f0: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
-00011900: 3d22 312e 322e 3322 2c0a 2020 2020 2020  ="1.2.3",.      
-00011910: 2020 2020 2020 696e 7075 7473 3d5b 7b22        inputs=[{"
-00011920: 666f 6f22 3a20 2262 6172 227d 2c20 7b22  foo": "bar"}, {"
-00011930: 666f 6f22 3a20 2262 617a 227d 5d2c 0a20  foo": "baz"}],. 
-00011940: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00011950: 7473 3d5b 7b22 666f 6f22 3a20 2262 6172  ts=[{"foo": "bar
-00011960: 227d 2c20 7b22 666f 6f22 3a20 2262 617a  "}, {"foo": "baz
-00011970: 227d 5d2c 0a20 2020 2020 2020 2020 2020  "}],.           
-00011980: 2066 6565 6462 6163 6b73 3d4e 6f6e 652c   feedbacks=None,
-00011990: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-000119a0: 6573 7461 6d70 733d 7469 6d65 7374 616d  estamps=timestam
-000119b0: 7073 2c0a 2020 2020 2020 2020 2020 2020  ps,.            
-000119c0: 736f 7274 5f6f 6e5f 7469 6d65 7374 616d  sort_on_timestam
-000119d0: 703d 5472 7565 2c0a 2020 2020 2020 2020  p=True,.        
-000119e0: 2020 2020 7361 6d70 6c65 5f72 6174 653d      sample_rate=
-000119f0: 312c 0a20 2020 2020 2020 2020 2020 206a  1,.            j
-00011a00: 6f69 6e5f 6b65 7973 3d5b 2266 6f6f 6261  oin_keys=["fooba
-00011a10: 7222 2c20 2262 6172 6261 7a22 5d2c 0a20  r", "barbaz"],. 
-00011a20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00011a30: 2069 7320 4e6f 6e65 0a20 2020 2029 0a20   is None.    ). 
-00011a40: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
-00011a50: 645f 6665 6564 6261 636b 2e61 7373 6572  d_feedback.asser
-00011a60: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
-00011a70: 2020 206d 6f63 6b5f 7072 6564 732e 6173     mock_preds.as
-00011a80: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
-00011a90: 290a 2020 2020 6d6f 636b 5f66 6565 6462  ).    mock_feedb
-00011aa0: 6163 6b2e 6173 7365 7274 5f6e 6f74 5f63  ack.assert_not_c
-00011ab0: 616c 6c65 6428 290a 0a0a 4070 7974 6573  alled()...@pytes
-00011ac0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00011ad0: 7a65 280a 2020 2020 2274 696d 6573 7461  ze(.    "timesta
-00011ae0: 6d70 7322 2c0a 2020 2020 5b0a 2020 2020  mps",.    [.    
-00011af0: 2020 2020 6e70 2e61 7272 6179 285b 3230      np.array([20
-00011b00: 302c 2032 3031 5d29 2c0a 2020 2020 2020  0, 201]),.      
-00011b10: 2020 6e70 2e61 7272 6179 285b 3230 302c    np.array([200,
-00011b20: 2043 5552 5245 4e54 5f54 494d 455d 292c   CURRENT_TIME]),
-00011b30: 0a20 2020 205d 2c0a 290a 406d 6f63 6b2e  .    ],.).@mock.
-00011b40: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-00011b50: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-00011b60: 7279 2e5f 6765 6e65 7261 7465 5f70 7265  ry._generate_pre
-00011b70: 6469 6374 696f 6e5f 616e 645f 6665 6564  diction_and_feed
-00011b80: 6261 636b 5f65 7665 6e74 7322 290a 406d  back_events").@m
-00011b90: 6f63 6b2e 7061 7463 6828 2267 616e 7472  ock.patch("gantr
-00011ba0: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
-00011bb0: 4761 6e74 7279 2e5f 6765 6e65 7261 7465  Gantry._generate
-00011bc0: 5f70 7265 6469 6374 696f 6e5f 6576 656e  _prediction_even
-00011bd0: 7473 2229 0a40 6d6f 636b 2e70 6174 6368  ts").@mock.patch
-00011be0: 2822 6761 6e74 7279 2e6c 6f67 6765 722e  ("gantry.logger.
-00011bf0: 636c 6965 6e74 2e47 616e 7472 792e 5f67  client.Gantry._g
-00011c00: 656e 6572 6174 655f 6665 6564 6261 636b  enerate_feedback
-00011c10: 5f65 7665 6e74 7322 290a 6465 6620 7465  _events").def te
-00011c20: 7374 5f67 656e 6572 6174 655f 7265 636f  st_generate_reco
-00011c30: 7264 735f 7072 6564 735f 616e 645f 6665  rds_preds_and_fe
-00011c40: 6564 6261 636b 5f77 726f 6e67 5f74 696d  edback_wrong_tim
-00011c50: 6573 7461 6d70 7328 0a20 2020 206d 6f63  estamps(.    moc
-00011c60: 6b5f 6765 6e65 7261 7465 5f66 6565 6462  k_generate_feedb
-00011c70: 6163 6b2c 0a20 2020 206d 6f63 6b5f 6765  ack,.    mock_ge
-00011c80: 6e65 7261 7465 5f70 7265 6473 2c0a 2020  nerate_preds,.  
-00011c90: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
-00011ca0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-00011cb0: 636b 2c0a 2020 2020 7469 6d65 7374 616d  ck,.    timestam
-00011cc0: 7073 2c0a 2020 2020 636c 695f 6f62 6a2c  ps,.    cli_obj,
-00011cd0: 0a29 3a0a 2020 2020 6173 7365 7274 2028  .):.    assert (
-00011ce0: 0a20 2020 2020 2020 2063 6c69 5f6f 626a  .        cli_obj
-00011cf0: 2e67 656e 6572 6174 655f 7265 636f 7264  .generate_record
-00011d00: 7328 0a20 2020 2020 2020 2020 2020 2061  s(.            a
-00011d10: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
-00011d20: 6172 222c 0a20 2020 2020 2020 2020 2020  ar",.           
-00011d30: 2076 6572 7369 6f6e 3d22 312e 322e 3322   version="1.2.3"
-00011d40: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-00011d50: 7075 7473 3d5b 7b22 666f 6f22 3a20 2262  puts=[{"foo": "b
-00011d60: 6172 227d 2c20 7b22 666f 6f22 3a20 2262  ar"}, {"foo": "b
-00011d70: 617a 227d 5d2c 0a20 2020 2020 2020 2020  az"}],.         
-00011d80: 2020 206f 7574 7075 7473 3d5b 7b22 666f     outputs=[{"fo
-00011d90: 6f22 3a20 2262 6172 227d 2c20 7b22 666f  o": "bar"}, {"fo
-00011da0: 6f22 3a20 2262 617a 227d 5d2c 0a20 2020  o": "baz"}],.   
-00011db0: 2020 2020 2020 2020 2066 6565 6462 6163           feedbac
-00011dc0: 6b73 3d4e 6f6e 652c 0a20 2020 2020 2020  ks=None,.       
-00011dd0: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
-00011de0: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
-00011df0: 2020 2020 2020 2020 736f 7274 5f6f 6e5f          sort_on_
-00011e00: 7469 6d65 7374 616d 703d 5472 7565 2c0a  timestamp=True,.
-00011e10: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
-00011e20: 6c65 5f72 6174 653d 312c 0a20 2020 2020  le_rate=1,.     
-00011e30: 2020 2020 2020 206a 6f69 6e5f 6b65 7973         join_keys
-00011e40: 3d5b 2266 6f6f 6261 7222 2c20 2262 6172  =["foobar", "bar
-00011e50: 6261 7a22 5d2c 0a20 2020 2020 2020 2029  baz"],.        )
-00011e60: 0a20 2020 2020 2020 2069 7320 4e6f 6e65  .        is None
-00011e70: 0a20 2020 2029 0a20 2020 206d 6f63 6b5f  .    ).    mock_
-00011e80: 6765 6e65 7261 7465 5f70 7265 6473 5f61  generate_preds_a
-00011e90: 6e64 5f66 6565 6462 6163 6b2e 6173 7365  nd_feedback.asse
-00011ea0: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00011eb0: 2020 2020 6d6f 636b 5f67 656e 6572 6174      mock_generat
-00011ec0: 655f 7072 6564 732e 6173 7365 7274 5f6e  e_preds.assert_n
-00011ed0: 6f74 5f63 616c 6c65 6428 290a 2020 2020  ot_called().    
-00011ee0: 6d6f 636b 5f67 656e 6572 6174 655f 6665  mock_generate_fe
-00011ef0: 6564 6261 636b 2e61 7373 6572 745f 6e6f  edback.assert_no
-00011f00: 745f 6361 6c6c 6564 2829 0a0a 0a40 7079  t_called()...@py
-00011f10: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
-00011f20: 7472 697a 6528 226a 6f69 6e5f 6b65 7973  trize("join_keys
-00011f30: 222c 205b 5b31 2c20 322c 2033 5d2c 2070  ", [[1, 2, 3], p
-00011f40: 642e 5365 7269 6573 285b 312c 2032 2c20  d.Series([1, 2, 
-00011f50: 335d 295d 290a 406d 6f63 6b2e 7061 7463  3])]).@mock.patc
-00011f60: 6828 2267 616e 7472 792e 6c6f 6767 6572  h("gantry.logger
-00011f70: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-00011f80: 6c6f 675f 7072 6564 6963 7469 6f6e 5f61  log_prediction_a
-00011f90: 6e64 5f66 6565 6462 6163 6b5f 6576 656e  nd_feedback_even
-00011fa0: 7473 2229 0a40 6d6f 636b 2e70 6174 6368  ts").@mock.patch
-00011fb0: 2822 6761 6e74 7279 2e6c 6f67 6765 722e  ("gantry.logger.
-00011fc0: 636c 6965 6e74 2e47 616e 7472 792e 5f6c  client.Gantry._l
-00011fd0: 6f67 5f70 7265 6469 6374 696f 6e5f 6576  og_prediction_ev
-00011fe0: 656e 7473 2229 0a40 6d6f 636b 2e70 6174  ents").@mock.pat
-00011ff0: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
-00012000: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
-00012010: 5f6c 6f67 5f66 6565 6462 6163 6b5f 6576  _log_feedback_ev
-00012020: 656e 7473 2229 0a64 6566 2074 6573 745f  ents").def test_
-00012030: 6c6f 675f 7265 636f 7264 735f 7072 6564  log_records_pred
-00012040: 735f 616e 645f 6665 6564 6261 636b 5f77  s_and_feedback_w
-00012050: 726f 6e67 5f6a 6f69 6e5f 6b65 7973 280a  rong_join_keys(.
-00012060: 2020 2020 6d6f 636b 5f66 6565 6462 6163      mock_feedbac
-00012070: 6b2c 0a20 2020 206d 6f63 6b5f 7072 6564  k,.    mock_pred
-00012080: 732c 0a20 2020 206d 6f63 6b5f 7072 6564  s,.    mock_pred
-00012090: 735f 616e 645f 6665 6564 6261 636b 2c0a  s_and_feedback,.
-000120a0: 2020 2020 6a6f 696e 5f6b 6579 732c 0a20      join_keys,. 
-000120b0: 2020 2063 6c69 5f6f 626a 2c0a 293a 0a20     cli_obj,.):. 
-000120c0: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
-000120d0: 2020 2020 636c 695f 6f62 6a2e 6c6f 675f      cli_obj.log_
-000120e0: 7265 636f 7264 7328 0a20 2020 2020 2020  records(.       
-000120f0: 2020 2020 2061 7070 6c69 6361 7469 6f6e       application
-00012100: 3d22 666f 6f62 6172 222c 0a20 2020 2020  ="foobar",.     
-00012110: 2020 2020 2020 2076 6572 7369 6f6e 3d22         version="
-00012120: 312e 322e 3322 2c0a 2020 2020 2020 2020  1.2.3",.        
-00012130: 2020 2020 696e 7075 7473 3d5b 7b22 4122      inputs=[{"A"
-00012140: 3a20 3230 307d 2c20 7b22 4122 3a20 3230  : 200}, {"A": 20
-00012150: 317d 5d2c 0a20 2020 2020 2020 2020 2020  1}],.           
-00012160: 206f 7574 7075 7473 3d5b 7b22 4222 3a20   outputs=[{"B": 
-00012170: 3230 307d 2c20 7b22 4222 3a20 3230 317d  200}, {"B": 201}
-00012180: 5d2c 0a20 2020 2020 2020 2020 2020 2066  ],.            f
-00012190: 6565 6462 6163 6b73 3d5b 7b22 4322 3a20  eedbacks=[{"C": 
-000121a0: 3230 307d 2c20 7b22 4322 3a20 3230 317d  200}, {"C": 201}
-000121b0: 5d2c 0a20 2020 2020 2020 2020 2020 2074  ],.            t
-000121c0: 696d 6573 7461 6d70 733d 4e6f 6e65 2c0a  imestamps=None,.
-000121d0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-000121e0: 5f6f 6e5f 7469 6d65 7374 616d 703d 5472  _on_timestamp=Tr
-000121f0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00012200: 7361 6d70 6c65 5f72 6174 653d 312c 0a20  sample_rate=1,. 
-00012210: 2020 2020 2020 2020 2020 206a 6f69 6e5f             join_
-00012220: 6b65 7973 3d6a 6f69 6e5f 6b65 7973 2c0a  keys=join_keys,.
-00012230: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00012240: 2020 6973 204e 6f6e 650a 2020 2020 290a    is None.    ).
-00012250: 2020 2020 6d6f 636b 5f70 7265 6473 5f61      mock_preds_a
-00012260: 6e64 5f66 6565 6462 6163 6b2e 6173 7365  nd_feedback.asse
-00012270: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00012280: 2020 2020 6d6f 636b 5f70 7265 6473 2e61      mock_preds.a
-00012290: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
-000122a0: 2829 0a20 2020 206d 6f63 6b5f 6665 6564  ().    mock_feed
-000122b0: 6261 636b 2e61 7373 6572 745f 6e6f 745f  back.assert_not_
-000122c0: 6361 6c6c 6564 2829 0a0a 0a40 7079 7465  called()...@pyte
-000122d0: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-000122e0: 697a 6528 226a 6f69 6e5f 6b65 7973 222c  ize("join_keys",
-000122f0: 205b 5b31 2c20 322c 2033 5d2c 2070 642e   [[1, 2, 3], pd.
-00012300: 5365 7269 6573 285b 312c 2032 2c20 335d  Series([1, 2, 3]
-00012310: 295d 290a 406d 6f63 6b2e 7061 7463 6828  )]).@mock.patch(
-00012320: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
-00012330: 6c69 656e 742e 4761 6e74 7279 2e5f 6765  lient.Gantry._ge
-00012340: 6e65 7261 7465 5f70 7265 6469 6374 696f  nerate_predictio
-00012350: 6e5f 616e 645f 6665 6564 6261 636b 5f65  n_and_feedback_e
-00012360: 7665 6e74 7322 290a 406d 6f63 6b2e 7061  vents").@mock.pa
-00012370: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
-00012380: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
-00012390: 2e5f 6765 6e65 7261 7465 5f70 7265 6469  ._generate_predi
-000123a0: 6374 696f 6e5f 6576 656e 7473 2229 0a40  ction_events").@
-000123b0: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
-000123c0: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
-000123d0: 2e47 616e 7472 792e 5f67 656e 6572 6174  .Gantry._generat
-000123e0: 655f 6665 6564 6261 636b 5f65 7665 6e74  e_feedback_event
-000123f0: 7322 290a 6465 6620 7465 7374 5f67 656e  s").def test_gen
-00012400: 6572 6174 655f 7265 636f 7264 735f 7072  erate_records_pr
-00012410: 6564 735f 616e 645f 6665 6564 6261 636b  eds_and_feedback
-00012420: 5f77 726f 6e67 5f6a 6f69 6e5f 6b65 7973  _wrong_join_keys
-00012430: 280a 2020 2020 6d6f 636b 5f67 656e 6572  (.    mock_gener
-00012440: 6174 655f 6665 6564 6261 636b 2c0a 2020  ate_feedback,.  
-00012450: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
-00012460: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
-00012470: 6765 6e65 7261 7465 5f70 7265 6473 5f61  generate_preds_a
-00012480: 6e64 5f66 6565 6462 6163 6b2c 0a20 2020  nd_feedback,.   
-00012490: 206a 6f69 6e5f 6b65 7973 2c0a 2020 2020   join_keys,.    
-000124a0: 636c 695f 6f62 6a2c 0a29 3a0a 2020 2020  cli_obj,.):.    
-000124b0: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
-000124c0: 2063 6c69 5f6f 626a 2e67 656e 6572 6174   cli_obj.generat
-000124d0: 655f 7265 636f 7264 7328 0a20 2020 2020  e_records(.     
-000124e0: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
-000124f0: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
-00012500: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
-00012510: 3d22 312e 322e 3322 2c0a 2020 2020 2020  ="1.2.3",.      
-00012520: 2020 2020 2020 696e 7075 7473 3d5b 7b22        inputs=[{"
-00012530: 4122 3a20 3230 307d 2c20 7b22 4122 3a20  A": 200}, {"A": 
-00012540: 3230 317d 5d2c 0a20 2020 2020 2020 2020  201}],.         
-00012550: 2020 206f 7574 7075 7473 3d5b 7b22 4222     outputs=[{"B"
-00012560: 3a20 3230 307d 2c20 7b22 4222 3a20 3230  : 200}, {"B": 20
-00012570: 317d 5d2c 0a20 2020 2020 2020 2020 2020  1}],.           
-00012580: 2066 6565 6462 6163 6b73 3d5b 7b22 4322   feedbacks=[{"C"
-00012590: 3a20 3230 307d 2c20 7b22 4322 3a20 3230  : 200}, {"C": 20
-000125a0: 317d 5d2c 0a20 2020 2020 2020 2020 2020  1}],.           
-000125b0: 2074 696d 6573 7461 6d70 733d 4e6f 6e65   timestamps=None
-000125c0: 2c0a 2020 2020 2020 2020 2020 2020 736f  ,.            so
-000125d0: 7274 5f6f 6e5f 7469 6d65 7374 616d 703d  rt_on_timestamp=
-000125e0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-000125f0: 2020 7361 6d70 6c65 5f72 6174 653d 312c    sample_rate=1,
-00012600: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
-00012610: 6e5f 6b65 7973 3d6a 6f69 6e5f 6b65 7973  n_keys=join_keys
-00012620: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00012630: 2020 2020 6973 204e 6f6e 650a 2020 2020      is None.    
-00012640: 290a 2020 2020 6d6f 636b 5f67 656e 6572  ).    mock_gener
-00012650: 6174 655f 7072 6564 735f 616e 645f 6665  ate_preds_and_fe
-00012660: 6564 6261 636b 2e61 7373 6572 745f 6e6f  edback.assert_no
-00012670: 745f 6361 6c6c 6564 2829 0a20 2020 206d  t_called().    m
-00012680: 6f63 6b5f 6765 6e65 7261 7465 5f70 7265  ock_generate_pre
-00012690: 6473 2e61 7373 6572 745f 6e6f 745f 6361  ds.assert_not_ca
-000126a0: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
-000126b0: 6765 6e65 7261 7465 5f66 6565 6462 6163  generate_feedbac
-000126c0: 6b2e 6173 7365 7274 5f6e 6f74 5f63 616c  k.assert_not_cal
-000126d0: 6c65 6428 290a 0a0a 4070 7974 6573 742e  led()...@pytest.
-000126e0: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-000126f0: 280a 2020 2020 2274 6573 745f 7469 6d65  (.    "test_time
-00012700: 7374 616d 7073 2c20 7465 7374 5f74 696d  stamps, test_tim
-00012710: 6573 7461 6d70 735f 6c69 7374 222c 0a20  estamps_list",. 
-00012720: 2020 205b 0a20 2020 2020 2020 2028 4e6f     [.        (No
-00012730: 6e65 2c20 4e6f 6e65 292c 0a20 2020 2020  ne, None),.     
-00012740: 2020 2028 5b43 5552 5245 4e54 5f54 494d     ([CURRENT_TIM
-00012750: 455d 202a 2032 2c20 5b43 5552 5245 4e54  E] * 2, [CURRENT
-00012760: 5f54 494d 455d 202a 2032 292c 0a20 2020  _TIME] * 2),.   
-00012770: 2020 2020 2028 6e70 2e61 7272 6179 285b       (np.array([
-00012780: 4355 5252 454e 545f 5449 4d45 5d20 2a20  CURRENT_TIME] * 
-00012790: 3229 2c20 5b43 5552 5245 4e54 5f54 494d  2), [CURRENT_TIM
-000127a0: 455d 202a 2032 292c 0a20 2020 205d 2c0a  E] * 2),.    ],.
-000127b0: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
-000127c0: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
-000127d0: 226b 7761 7267 7322 2c0a 2020 2020 5b0a  "kwargs",.    [.
-000127e0: 2020 2020 2020 2020 7b22 6665 6564 6261          {"feedba
-000127f0: 636b 5f6b 6579 7322 3a20 5b22 4122 5d7d  ck_keys": ["A"]}
-00012800: 2c0a 2020 2020 2020 2020 7b22 6665 6564  ,.        {"feed
-00012810: 6261 636b 5f69 6473 223a 205b 2231 3233  back_ids": ["123
-00012820: 3435 222c 2022 3637 3839 3022 5d7d 2c0a  45", "67890"]},.
-00012830: 2020 2020 2020 2020 7b22 6a6f 696e 5f6b          {"join_k
-00012840: 6579 7322 3a20 5b22 3534 3332 3122 2c20  eys": ["54321", 
-00012850: 2236 3738 3930 225d 7d2c 0a20 2020 2020  "67890"]},.     
-00012860: 2020 207b 226a 6f69 6e5f 6b65 7973 223a     {"join_keys":
-00012870: 2070 642e 5365 7269 6573 285b 2235 3433   pd.Series(["543
-00012880: 3231 222c 2022 3637 3839 3022 5d29 7d2c  21", "67890"])},
-00012890: 0a20 2020 2020 2020 207b 7d2c 0a20 2020  .        {},.   
-000128a0: 205d 2c0a 290a 4070 7974 6573 742e 6d61   ],.).@pytest.ma
-000128b0: 726b 2e70 6172 616d 6574 7269 7a65 280a  rk.parametrize(.
-000128c0: 2020 2020 2822 7465 7374 5f6f 7574 7075      ("test_outpu
-000128d0: 7473 222c 2022 7465 7374 5f69 6e70 7574  ts", "test_input
-000128e0: 7322 292c 0a20 2020 206c 6973 7428 7a69  s"),.    list(zi
-000128f0: 7028 5445 5354 5f4f 5554 5055 5453 2c20  p(TEST_OUTPUTS, 
-00012900: 5445 5354 5f49 4e50 5554 5329 292c 0a29  TEST_INPUTS)),.)
-00012910: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
-00012920: 7261 6d65 7472 697a 6528 2276 6572 7369  rametrize("versi
-00012930: 6f6e 222c 205b 4e6f 6e65 2c20 3130 2c20  on", [None, 10, 
-00012940: 2231 2e32 2e33 225d 290a 4070 7974 6573  "1.2.3"]).@pytes
-00012950: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00012960: 7a65 2822 7461 6773 2c20 726f 775f 7461  ze("tags, row_ta
-00012970: 6773 2c20 676c 6f62 616c 5f74 6167 732c  gs, global_tags,
-00012980: 2065 7870 6563 7465 645f 7461 6773 5f70   expected_tags_p
-00012990: 6172 616d 222c 2054 4553 545f 5441 4753  aram", TEST_TAGS
-000129a0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-000129b0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-000129c0: 656e 742e 5f72 6573 6f6c 7665 5f6a 6f69  ent._resolve_joi
-000129d0: 6e5f 6b65 7973 2229 0a40 6d6f 636b 2e70  n_keys").@mock.p
-000129e0: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
-000129f0: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-00012a00: 792e 5f6c 6f67 5f70 7265 6469 6374 696f  y._log_predictio
-00012a10: 6e5f 616e 645f 6665 6564 6261 636b 5f65  n_and_feedback_e
-00012a20: 7665 6e74 7322 290a 406d 6f63 6b2e 7061  vents").@mock.pa
-00012a30: 7463 6828 0a20 2020 2022 6761 6e74 7279  tch(.    "gantry
-00012a40: 2e6c 6f67 6765 722e 636c 6965 6e74 2e47  .logger.client.G
-00012a50: 616e 7472 792e 5f6c 6f67 5f70 7265 6469  antry._log_predi
-00012a60: 6374 696f 6e5f 6576 656e 7473 222c 2072  ction_events", r
-00012a70: 6574 7572 6e5f 7661 6c75 653d 284e 6f6e  eturn_value=(Non
-00012a80: 652c 205b 2231 3233 3435 222c 2022 3637  e, ["12345", "67
-00012a90: 3839 3022 5d29 0a29 0a40 6d6f 636b 2e70  890"]).).@mock.p
-00012aa0: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
-00012ab0: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-00012ac0: 792e 5f6c 6f67 5f66 6565 6462 6163 6b5f  y._log_feedback_
-00012ad0: 6576 656e 7473 2229 0a40 6d6f 636b 2e70  events").@mock.p
-00012ae0: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
-00012af0: 6765 722e 636c 6965 6e74 2e5f 7361 6d70  ger.client._samp
-00012b00: 6c65 5f72 6563 6f72 6473 222c 2073 6964  le_records", sid
-00012b10: 655f 6566 6665 6374 3d63 6c69 656e 742e  e_effect=client.
-00012b20: 5f73 616d 706c 655f 7265 636f 7264 7329  _sample_records)
+00010230: 656e 742e 5f73 616d 706c 655f 7265 636f  ent._sample_reco
+00010240: 7264 7322 2c20 7369 6465 5f65 6666 6563  rds", side_effec
+00010250: 743d 636c 6965 6e74 2e5f 7361 6d70 6c65  t=client._sample
+00010260: 5f72 6563 6f72 6473 290a 406d 6f63 6b2e  _records).@mock.
+00010270: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+00010280: 6767 6572 2e63 6c69 656e 742e 5f64 6566  gger.client._def
+00010290: 6175 6c74 5f6a 6f69 6e5f 6b65 795f 6765  ault_join_key_ge
+000102a0: 6e22 290a 6465 6620 7465 7374 5f73 696e  n").def test_sin
+000102b0: 676c 655f 6c6f 675f 7072 6564 735f 616e  gle_log_preds_an
+000102c0: 645f 6665 6564 6261 636b 280a 2020 2020  d_feedback(.    
+000102d0: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
+000102e0: 6e2c 0a20 2020 206d 6f63 6b5f 7361 6d70  n,.    mock_samp
+000102f0: 6c65 5f72 6563 6f72 6473 2c0a 2020 2020  le_records,.    
+00010300: 6d6f 636b 5f6c 6f67 5f66 6565 6462 6163  mock_log_feedbac
+00010310: 6b2c 0a20 2020 206d 6f63 6b5f 6c6f 675f  k,.    mock_log_
+00010320: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
+00010330: 6c6f 675f 7072 6564 735f 616e 645f 6665  log_preds_and_fe
+00010340: 6564 6261 636b 2c0a 2020 2020 6d6f 636b  edback,.    mock
+00010350: 5f72 6573 6f6c 7665 5f6a 6f69 6e5f 6b65  _resolve_join_ke
+00010360: 7973 2c0a 2020 2020 6b77 6172 6773 2c0a  ys,.    kwargs,.
+00010370: 2020 2020 7665 7273 696f 6e2c 0a20 2020      version,.   
+00010380: 2074 6167 732c 0a20 2020 2072 6f77 5f74   tags,.    row_t
+00010390: 6167 732c 0a20 2020 2067 6c6f 6261 6c5f  ags,.    global_
+000103a0: 7461 6773 2c0a 2020 2020 6578 7065 6374  tags,.    expect
+000103b0: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
+000103c0: 2020 2074 6573 745f 7469 6d65 7374 616d     test_timestam
+000103d0: 7073 2c0a 2020 2020 7465 7374 5f74 696d  ps,.    test_tim
+000103e0: 6573 7461 6d70 735f 6c69 7374 2c0a 2020  estamps_list,.  
+000103f0: 2020 7465 7374 5f69 6e70 7574 732c 0a20    test_inputs,. 
+00010400: 2020 2074 6573 745f 6f75 7470 7574 732c     test_outputs,
+00010410: 0a20 2020 2074 6573 745f 6665 6564 6261  .    test_feedba
+00010420: 636b 732c 0a20 2020 2063 6c69 5f6f 626a  cks,.    cli_obj
+00010430: 2c0a 293a 0a20 2020 206d 6f63 6b5f 6a6f  ,.):.    mock_jo
+00010440: 696e 5f6b 6579 5f67 656e 2e73 6964 655f  in_key_gen.side_
+00010450: 6566 6665 6374 203d 205b 2236 3738 3930  effect = ["67890
+00010460: 222c 2022 3132 3334 3522 5d0a 2020 2020  ", "12345"].    
+00010470: 6d6f 636b 5f72 6573 6f6c 7665 5f6a 6f69  mock_resolve_joi
+00010480: 6e5f 6b65 7973 2e72 6574 7572 6e5f 7661  n_keys.return_va
+00010490: 6c75 6520 3d20 5b22 3132 3334 3522 2c20  lue = ["12345", 
+000104a0: 2236 3738 3930 225d 2069 6620 6b77 6172  "67890"] if kwar
+000104b0: 6773 2065 6c73 6520 4e6f 6e65 0a20 2020  gs else None.   
+000104c0: 2063 6c69 5f6f 626a 2e6c 6f67 280a 2020   cli_obj.log(.  
+000104d0: 2020 2020 2020 6170 706c 6963 6174 696f        applicatio
+000104e0: 6e3d 2266 6f6f 6261 7222 2c0a 2020 2020  n="foobar",.    
+000104f0: 2020 2020 7665 7273 696f 6e3d 7665 7273      version=vers
+00010500: 696f 6e2c 0a20 2020 2020 2020 2069 6e70  ion,.        inp
+00010510: 7574 733d 7465 7374 5f69 6e70 7574 732c  uts=test_inputs,
+00010520: 0a20 2020 2020 2020 206f 7574 7075 7473  .        outputs
+00010530: 3d74 6573 745f 6f75 7470 7574 732c 0a20  =test_outputs,. 
+00010540: 2020 2020 2020 2066 6565 6462 6163 6b73         feedbacks
+00010550: 3d74 6573 745f 6665 6564 6261 636b 732c  =test_feedbacks,
+00010560: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
+00010570: 6d70 733d 7465 7374 5f74 696d 6573 7461  mps=test_timesta
+00010580: 6d70 732c 0a20 2020 2020 2020 2073 6f72  mps,.        sor
+00010590: 745f 6f6e 5f74 696d 6573 7461 6d70 3d54  t_on_timestamp=T
+000105a0: 7275 652c 0a20 2020 2020 2020 2073 616d  rue,.        sam
+000105b0: 706c 655f 7261 7465 3d31 2c0a 2020 2020  ple_rate=1,.    
+000105c0: 2020 2020 676c 6f62 616c 5f74 6167 733d      global_tags=
+000105d0: 676c 6f62 616c 5f74 6167 732c 0a20 2020  global_tags,.   
+000105e0: 2020 2020 2074 6167 733d 7461 6773 2c0a       tags=tags,.
+000105f0: 2020 2020 2020 2020 726f 775f 7461 6773          row_tags
+00010600: 3d72 6f77 5f74 6167 732c 0a20 2020 2020  =row_tags,.     
+00010610: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
+00010620: 2029 0a0a 2020 2020 6d6f 636b 5f6c 6f67   )..    mock_log
+00010630: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
+00010640: 6163 6b2e 6173 7365 7274 5f63 616c 6c65  ack.assert_calle
+00010650: 645f 6f6e 6365 5f77 6974 6828 0a20 2020  d_once_with(.   
+00010660: 2020 2020 2061 7070 6c69 6361 7469 6f6e       application
+00010670: 3d22 666f 6f62 6172 222c 0a20 2020 2020  ="foobar",.     
+00010680: 2020 2069 6e70 7574 733d 5b7b 2241 223a     inputs=[{"A":
+00010690: 2031 3030 7d2c 207b 2241 223a 2031 3031   100}, {"A": 101
+000106a0: 7d5d 2c0a 2020 2020 2020 2020 6f75 7470  }],.        outp
+000106b0: 7574 733d 5b7b 2242 223a 2033 3030 7d2c  uts=[{"B": 300},
+000106c0: 207b 2242 223a 2033 3031 7d5d 2c0a 2020   {"B": 301}],.  
+000106d0: 2020 2020 2020 6665 6564 6261 636b 733d        feedbacks=
+000106e0: 5b7b 2241 223a 2032 3030 7d2c 207b 2241  [{"A": 200}, {"A
+000106f0: 223a 2032 3031 7d5d 2c0a 2020 2020 2020  ": 201}],.      
+00010700: 2020 6a6f 696e 5f6b 6579 733d 5b22 3132    join_keys=["12
+00010710: 3334 3522 2c20 2236 3738 3930 225d 2069  345", "67890"] i
+00010720: 6620 6b77 6172 6773 2065 6c73 6520 5b22  f kwargs else ["
+00010730: 3637 3839 3022 2c20 2231 3233 3435 225d  67890", "12345"]
+00010740: 2c0a 2020 2020 2020 2020 7665 7273 696f  ,.        versio
+00010750: 6e3d 7665 7273 696f 6e2c 0a20 2020 2020  n=version,.     
+00010760: 2020 2069 676e 6f72 655f 696e 7075 7473     ignore_inputs
+00010770: 3d4e 6f6e 652c 0a20 2020 2020 2020 2074  =None,.        t
+00010780: 696d 6573 7461 6d70 733d 7465 7374 5f74  imestamps=test_t
+00010790: 696d 6573 7461 6d70 735f 6c69 7374 2c0a  imestamps_list,.
+000107a0: 2020 2020 2020 2020 736f 7274 5f6f 6e5f          sort_on_
+000107b0: 7469 6d65 7374 616d 703d 5472 7565 2c0a  timestamp=True,.
+000107c0: 2020 2020 2020 2020 7461 6773 3d65 7870          tags=exp
+000107d0: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
+000107e0: 2c0a 2020 2020 2020 2020 6173 5f62 6174  ,.        as_bat
+000107f0: 6368 3d46 616c 7365 2c0a 2020 2020 290a  ch=False,.    ).
+00010800: 2020 2020 6d6f 636b 5f6c 6f67 5f70 7265      mock_log_pre
+00010810: 6473 2e61 7373 6572 745f 6e6f 745f 6361  ds.assert_not_ca
+00010820: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
+00010830: 6c6f 675f 6665 6564 6261 636b 2e61 7373  log_feedback.ass
+00010840: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
+00010850: 0a0a 2020 2020 6d6f 636b 5f73 616d 706c  ..    mock_sampl
+00010860: 655f 7265 636f 7264 732e 6173 7365 7274  e_records.assert
+00010870: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+00010880: 6828 0a20 2020 2020 2020 2032 2c0a 2020  h(.        2,.  
+00010890: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+000108a0: 205b 7b22 4122 3a20 3130 307d 2c20 7b22   [{"A": 100}, {"
+000108b0: 4122 3a20 3130 317d 5d2c 0a20 2020 2020  A": 101}],.     
+000108c0: 2020 205b 7b22 4222 3a20 3330 307d 2c20     [{"B": 300}, 
+000108d0: 7b22 4222 3a20 3330 317d 5d2c 0a20 2020  {"B": 301}],.   
+000108e0: 2020 2020 205b 7b22 4122 3a20 3230 307d       [{"A": 200}
+000108f0: 2c20 7b22 4122 3a20 3230 317d 5d2c 0a20  , {"A": 201}],. 
+00010900: 2020 2020 2020 2063 6c69 656e 742e 5f72         client._r
+00010910: 6573 6f6c 7665 5f6a 6f69 6e5f 6b65 7973  esolve_join_keys
+00010920: 282a 2a6b 7761 7267 7329 2c0a 2020 2020  (**kwargs),.    
+00010930: 2020 2020 7465 7374 5f74 696d 6573 7461      test_timesta
+00010940: 6d70 735f 6c69 7374 2c0a 2020 2020 2020  mps_list,.      
+00010950: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
+00010960: 7061 7261 6d2c 0a20 2020 2029 0a0a 2020  param,.    )..  
+00010970: 2020 6966 206b 7761 7267 733a 0a20 2020    if kwargs:.   
+00010980: 2020 2020 206d 6f63 6b5f 6a6f 696e 5f6b       mock_join_k
+00010990: 6579 5f67 656e 2e61 7373 6572 745f 6e6f  ey_gen.assert_no
+000109a0: 745f 6361 6c6c 6564 2829 0a20 2020 2065  t_called().    e
+000109b0: 6c73 653a 0a20 2020 2020 2020 206d 6f63  lse:.        moc
+000109c0: 6b5f 6a6f 696e 5f6b 6579 5f67 656e 2e61  k_join_key_gen.a
+000109d0: 7373 6572 745f 6361 6c6c 6564 2829 0a0a  ssert_called()..
+000109e0: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
+000109f0: 7261 6d65 7472 697a 6528 0a20 2020 2022  rametrize(.    "
+00010a00: 696e 7075 7473 2c20 6f75 7470 7574 732c  inputs, outputs,
+00010a10: 2066 6565 6462 6163 6b73 222c 0a20 2020   feedbacks",.   
+00010a20: 205b 0a20 2020 2020 2020 2028 0a20 2020   [.        (.   
+00010a30: 2020 2020 2020 2020 206e 702e 6172 7261           np.arra
+00010a40: 7928 5b32 3030 2c20 3230 315d 292c 0a20  y([200, 201]),. 
+00010a50: 2020 2020 2020 2020 2020 205b 7b22 4222             [{"B"
+00010a60: 3a20 3230 307d 2c20 7b22 4222 3a20 3230  : 200}, {"B": 20
+00010a70: 317d 5d2c 0a20 2020 2020 2020 2020 2020  1}],.           
+00010a80: 205b 7b22 4122 3a20 3230 307d 2c20 7b22   [{"A": 200}, {"
+00010a90: 4122 3a20 3230 317d 5d2c 0a20 2020 2020  A": 201}],.     
+00010aa0: 2020 2029 2c0a 2020 2020 2020 2020 280a     ),.        (.
+00010ab0: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
+00010ac0: 7272 6179 285b 3230 302c 2032 3031 5d29  rray([200, 201])
+00010ad0: 2c0a 2020 2020 2020 2020 2020 2020 5b7b  ,.            [{
+00010ae0: 2242 223a 2032 3030 7d2c 207b 2242 223a  "B": 200}, {"B":
+00010af0: 2032 3031 7d5d 2c0a 2020 2020 2020 2020   201}],.        
+00010b00: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
+00010b10: 2020 292c 0a20 2020 2020 2020 2028 0a20    ),.        (. 
+00010b20: 2020 2020 2020 2020 2020 206e 702e 6172             np.ar
+00010b30: 7261 7928 5b32 3030 2c20 3230 315d 292c  ray([200, 201]),
+00010b40: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+00010b50: 6172 7261 7928 5b32 3030 2c20 3230 315d  array([200, 201]
+00010b60: 292c 0a20 2020 2020 2020 2020 2020 204e  ),.            N
+00010b70: 6f6e 652c 0a20 2020 2020 2020 2029 2c0a  one,.        ),.
+00010b80: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+00010b90: 2020 2020 2020 5b7b 2242 223a 2032 3030        [{"B": 200
+00010ba0: 7d2c 207b 2242 223a 2032 3031 7d5d 2c0a  }, {"B": 201}],.
+00010bb0: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
+00010bc0: 7272 6179 285b 3230 302c 2032 3031 5d29  rray([200, 201])
+00010bd0: 2c0a 2020 2020 2020 2020 2020 2020 5b7b  ,.            [{
+00010be0: 2241 223a 2032 3030 7d2c 207b 2241 223a  "A": 200}, {"A":
+00010bf0: 2032 3031 7d5d 2c0a 2020 2020 2020 2020   201}],.        
+00010c00: 292c 0a20 2020 2020 2020 2028 0a20 2020  ),.        (.   
+00010c10: 2020 2020 2020 2020 205b 7b22 4222 3a20           [{"B": 
+00010c20: 3230 307d 2c20 7b22 4222 3a20 3230 317d  200}, {"B": 201}
+00010c30: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00010c40: 7b22 4122 3a20 3230 307d 2c20 7b22 4122  {"A": 200}, {"A"
+00010c50: 3a20 3230 317d 5d2c 0a20 2020 2020 2020  : 201}],.       
+00010c60: 2020 2020 206e 702e 6172 7261 7928 5b32       np.array([2
+00010c70: 3030 2c20 3230 315d 292c 0a20 2020 2020  00, 201]),.     
+00010c80: 2020 2029 2c0a 2020 2020 2020 2020 280a     ),.        (.
+00010c90: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
+00010ca0: 2c0a 2020 2020 2020 2020 2020 2020 4e6f  ,.            No
+00010cb0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00010cc0: 6e70 2e61 7272 6179 285b 3230 302c 2032  np.array([200, 2
+00010cd0: 3031 5d29 2c0a 2020 2020 2020 2020 292c  01]),.        ),
+00010ce0: 0a20 2020 205d 2c0a 290a 406d 6f63 6b2e  .    ],.).@mock.
+00010cf0: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+00010d00: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
+00010d10: 7279 2e5f 6c6f 675f 7072 6564 6963 7469  ry._log_predicti
+00010d20: 6f6e 5f61 6e64 5f66 6565 6462 6163 6b5f  on_and_feedback_
+00010d30: 6576 656e 7473 2229 0a40 6d6f 636b 2e70  events").@mock.p
+00010d40: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
+00010d50: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
+00010d60: 792e 5f6c 6f67 5f70 7265 6469 6374 696f  y._log_predictio
+00010d70: 6e5f 6576 656e 7473 2229 0a40 6d6f 636b  n_events").@mock
+00010d80: 2e70 6174 6368 2822 6761 6e74 7279 2e6c  .patch("gantry.l
+00010d90: 6f67 6765 722e 636c 6965 6e74 2e47 616e  ogger.client.Gan
+00010da0: 7472 792e 5f6c 6f67 5f66 6565 6462 6163  try._log_feedbac
+00010db0: 6b5f 6576 656e 7473 2229 0a64 6566 2074  k_events").def t
+00010dc0: 6573 745f 6c6f 675f 7265 636f 7264 735f  est_log_records_
+00010dd0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+00010de0: 636b 5f77 726f 6e67 5f6e 705f 6172 7261  ck_wrong_np_arra
+00010df0: 7928 0a20 2020 206d 6f63 6b5f 6665 6564  y(.    mock_feed
+00010e00: 6261 636b 2c0a 2020 2020 6d6f 636b 5f70  back,.    mock_p
+00010e10: 7265 6473 2c0a 2020 2020 6d6f 636b 5f70  reds,.    mock_p
+00010e20: 7265 6473 5f61 6e64 5f66 6565 6462 6163  reds_and_feedbac
+00010e30: 6b2c 0a20 2020 2069 6e70 7574 732c 0a20  k,.    inputs,. 
+00010e40: 2020 206f 7574 7075 7473 2c0a 2020 2020     outputs,.    
+00010e50: 6665 6564 6261 636b 732c 0a20 2020 2063  feedbacks,.    c
+00010e60: 6c69 5f6f 626a 2c0a 293a 0a20 2020 2061  li_obj,.):.    a
+00010e70: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
+00010e80: 636c 695f 6f62 6a2e 6c6f 675f 7265 636f  cli_obj.log_reco
+00010e90: 7264 7328 0a20 2020 2020 2020 2020 2020  rds(.           
+00010ea0: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
+00010eb0: 6f62 6172 222c 0a20 2020 2020 2020 2020  obar",.         
+00010ec0: 2020 2076 6572 7369 6f6e 3d22 312e 322e     version="1.2.
+00010ed0: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
+00010ee0: 696e 7075 7473 3d69 6e70 7574 732c 0a20  inputs=inputs,. 
+00010ef0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00010f00: 7473 3d6f 7574 7075 7473 2c0a 2020 2020  ts=outputs,.    
+00010f10: 2020 2020 2020 2020 6665 6564 6261 636b          feedback
+00010f20: 733d 6665 6564 6261 636b 732c 0a20 2020  s=feedbacks,.   
+00010f30: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
+00010f40: 6d70 733d 4e6f 6e65 2c0a 2020 2020 2020  mps=None,.      
+00010f50: 2020 2020 2020 736f 7274 5f6f 6e5f 7469        sort_on_ti
+00010f60: 6d65 7374 616d 703d 5472 7565 2c0a 2020  mestamp=True,.  
+00010f70: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+00010f80: 5f72 6174 653d 312c 0a20 2020 2020 2020  _rate=1,.       
+00010f90: 2020 2020 206a 6f69 6e5f 6b65 7973 3d5b       join_keys=[
+00010fa0: 2266 6f6f 6261 7222 2c20 2262 6172 6261  "foobar", "barba
+00010fb0: 7a22 5d2c 0a20 2020 2020 2020 2029 0a20  z"],.        ). 
+00010fc0: 2020 2020 2020 2069 7320 4e6f 6e65 0a20         is None. 
+00010fd0: 2020 2029 0a20 2020 206d 6f63 6b5f 7072     ).    mock_pr
+00010fe0: 6564 735f 616e 645f 6665 6564 6261 636b  eds_and_feedback
+00010ff0: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
+00011000: 6564 2829 0a20 2020 206d 6f63 6b5f 7072  ed().    mock_pr
+00011010: 6564 732e 6173 7365 7274 5f6e 6f74 5f63  eds.assert_not_c
+00011020: 616c 6c65 6428 290a 2020 2020 6d6f 636b  alled().    mock
+00011030: 5f66 6565 6462 6163 6b2e 6173 7365 7274  _feedback.assert
+00011040: 5f6e 6f74 5f63 616c 6c65 6428 290a 0a0a  _not_called()...
+00011050: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
+00011060: 616d 6574 7269 7a65 280a 2020 2020 2269  ametrize(.    "i
+00011070: 6e70 7574 732c 206f 7574 7075 7473 2c20  nputs, outputs, 
+00011080: 6665 6564 6261 636b 7322 2c0a 2020 2020  feedbacks",.    
+00011090: 5b0a 2020 2020 2020 2020 280a 2020 2020  [.        (.    
+000110a0: 2020 2020 2020 2020 6e70 2e61 7272 6179          np.array
+000110b0: 285b 3230 302c 2032 3031 5d29 2c0a 2020  ([200, 201]),.  
+000110c0: 2020 2020 2020 2020 2020 5b7b 2242 223a            [{"B":
+000110d0: 2032 3030 7d2c 207b 2242 223a 2032 3031   200}, {"B": 201
+000110e0: 7d5d 2c0a 2020 2020 2020 2020 2020 2020  }],.            
+000110f0: 5b7b 2241 223a 2032 3030 7d2c 207b 2241  [{"A": 200}, {"A
+00011100: 223a 2032 3031 7d5d 2c0a 2020 2020 2020  ": 201}],.      
+00011110: 2020 292c 0a20 2020 2020 2020 2028 0a20    ),.        (. 
+00011120: 2020 2020 2020 2020 2020 206e 702e 6172             np.ar
+00011130: 7261 7928 5b32 3030 2c20 3230 315d 292c  ray([200, 201]),
+00011140: 0a20 2020 2020 2020 2020 2020 205b 7b22  .            [{"
+00011150: 4222 3a20 3230 307d 2c20 7b22 4222 3a20  B": 200}, {"B": 
+00011160: 3230 317d 5d2c 0a20 2020 2020 2020 2020  201}],.         
+00011170: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
+00011180: 2029 2c0a 2020 2020 2020 2020 280a 2020   ),.        (.  
+00011190: 2020 2020 2020 2020 2020 6e70 2e61 7272            np.arr
+000111a0: 6179 285b 3230 302c 2032 3031 5d29 2c0a  ay([200, 201]),.
+000111b0: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
+000111c0: 7272 6179 285b 3230 302c 2032 3031 5d29  rray([200, 201])
+000111d0: 2c0a 2020 2020 2020 2020 2020 2020 4e6f  ,.            No
+000111e0: 6e65 2c0a 2020 2020 2020 2020 292c 0a20  ne,.        ),. 
+000111f0: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
+00011200: 2020 2020 205b 7b22 4222 3a20 3230 307d       [{"B": 200}
+00011210: 2c20 7b22 4222 3a20 3230 317d 5d2c 0a20  , {"B": 201}],. 
+00011220: 2020 2020 2020 2020 2020 206e 702e 6172             np.ar
+00011230: 7261 7928 5b32 3030 2c20 3230 315d 292c  ray([200, 201]),
+00011240: 0a20 2020 2020 2020 2020 2020 205b 7b22  .            [{"
+00011250: 4122 3a20 3230 307d 2c20 7b22 4122 3a20  A": 200}, {"A": 
+00011260: 3230 317d 5d2c 0a20 2020 2020 2020 2029  201}],.        )
+00011270: 2c0a 2020 2020 2020 2020 280a 2020 2020  ,.        (.    
+00011280: 2020 2020 2020 2020 5b7b 2242 223a 2032          [{"B": 2
+00011290: 3030 7d2c 207b 2242 223a 2032 3031 7d5d  00}, {"B": 201}]
+000112a0: 2c0a 2020 2020 2020 2020 2020 2020 5b7b  ,.            [{
+000112b0: 2241 223a 2032 3030 7d2c 207b 2241 223a  "A": 200}, {"A":
+000112c0: 2032 3031 7d5d 2c0a 2020 2020 2020 2020   201}],.        
+000112d0: 2020 2020 6e70 2e61 7272 6179 285b 3230      np.array([20
+000112e0: 302c 2032 3031 5d29 2c0a 2020 2020 2020  0, 201]),.      
+000112f0: 2020 292c 0a20 2020 2020 2020 2028 0a20    ),.        (. 
+00011300: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
+00011310: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
+00011320: 652c 0a20 2020 2020 2020 2020 2020 206e  e,.            n
+00011330: 702e 6172 7261 7928 5b32 3030 2c20 3230  p.array([200, 20
+00011340: 315d 292c 0a20 2020 2020 2020 2029 2c0a  1]),.        ),.
+00011350: 2020 2020 5d2c 0a29 0a40 6d6f 636b 2e70      ],.).@mock.p
+00011360: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
+00011370: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
+00011380: 792e 5f67 656e 6572 6174 655f 7072 6564  y._generate_pred
+00011390: 6963 7469 6f6e 5f61 6e64 5f66 6565 6462  iction_and_feedb
+000113a0: 6163 6b5f 6576 656e 7473 2229 0a40 6d6f  ack_events").@mo
+000113b0: 636b 2e70 6174 6368 2822 6761 6e74 7279  ck.patch("gantry
+000113c0: 2e6c 6f67 6765 722e 636c 6965 6e74 2e47  .logger.client.G
+000113d0: 616e 7472 792e 5f67 656e 6572 6174 655f  antry._generate_
+000113e0: 7072 6564 6963 7469 6f6e 5f65 7665 6e74  prediction_event
+000113f0: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
+00011400: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
+00011410: 6c69 656e 742e 4761 6e74 7279 2e5f 6765  lient.Gantry._ge
+00011420: 6e65 7261 7465 5f66 6565 6462 6163 6b5f  nerate_feedback_
+00011430: 6576 656e 7473 2229 0a64 6566 2074 6573  events").def tes
+00011440: 745f 6765 6e65 7261 7465 5f72 6563 6f72  t_generate_recor
+00011450: 6473 5f70 7265 6473 5f61 6e64 5f66 6565  ds_preds_and_fee
+00011460: 6462 6163 6b5f 7772 6f6e 675f 6e70 5f61  dback_wrong_np_a
+00011470: 7272 6179 280a 2020 2020 6d6f 636b 5f67  rray(.    mock_g
+00011480: 656e 6572 6174 655f 6665 6564 6261 636b  enerate_feedback
+00011490: 2c0a 2020 2020 6d6f 636b 5f67 656e 6572  ,.    mock_gener
+000114a0: 6174 655f 7072 6564 732c 0a20 2020 206d  ate_preds,.    m
+000114b0: 6f63 6b5f 6765 6e65 7261 7465 5f70 7265  ock_generate_pre
+000114c0: 6473 5f61 6e64 5f66 6565 6462 6163 6b2c  ds_and_feedback,
+000114d0: 0a20 2020 2069 6e70 7574 732c 0a20 2020  .    inputs,.   
+000114e0: 206f 7574 7075 7473 2c0a 2020 2020 6665   outputs,.    fe
+000114f0: 6564 6261 636b 732c 0a20 2020 2063 6c69  edbacks,.    cli
+00011500: 5f6f 626a 2c0a 293a 0a20 2020 2061 7373  _obj,.):.    ass
+00011510: 6572 7420 280a 2020 2020 2020 2020 636c  ert (.        cl
+00011520: 695f 6f62 6a2e 6765 6e65 7261 7465 5f72  i_obj.generate_r
+00011530: 6563 6f72 6473 280a 2020 2020 2020 2020  ecords(.        
+00011540: 2020 2020 6170 706c 6963 6174 696f 6e3d      application=
+00011550: 2266 6f6f 6261 7222 2c0a 2020 2020 2020  "foobar",.      
+00011560: 2020 2020 2020 7665 7273 696f 6e3d 2231        version="1
+00011570: 2e32 2e33 222c 0a20 2020 2020 2020 2020  .2.3",.         
+00011580: 2020 2069 6e70 7574 733d 696e 7075 7473     inputs=inputs
+00011590: 2c0a 2020 2020 2020 2020 2020 2020 6f75  ,.            ou
+000115a0: 7470 7574 733d 6f75 7470 7574 732c 0a20  tputs=outputs,. 
+000115b0: 2020 2020 2020 2020 2020 2066 6565 6462             feedb
+000115c0: 6163 6b73 3d66 6565 6462 6163 6b73 2c0a  acks=feedbacks,.
+000115d0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+000115e0: 7374 616d 7073 3d4e 6f6e 652c 0a20 2020  stamps=None,.   
+000115f0: 2020 2020 2020 2020 2073 6f72 745f 6f6e           sort_on
+00011600: 5f74 696d 6573 7461 6d70 3d54 7275 652c  _timestamp=True,
+00011610: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
+00011620: 706c 655f 7261 7465 3d31 2c0a 2020 2020  ple_rate=1,.    
+00011630: 2020 2020 2020 2020 6a6f 696e 5f6b 6579          join_key
+00011640: 733d 5b22 666f 6f62 6172 222c 2022 6261  s=["foobar", "ba
+00011650: 7262 617a 225d 2c0a 2020 2020 2020 2020  rbaz"],.        
+00011660: 290a 2020 2020 2020 2020 6973 204e 6f6e  ).        is Non
+00011670: 650a 2020 2020 290a 2020 2020 6d6f 636b  e.    ).    mock
+00011680: 5f67 656e 6572 6174 655f 7072 6564 735f  _generate_preds_
+00011690: 616e 645f 6665 6564 6261 636b 2e61 7373  and_feedback.ass
+000116a0: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
+000116b0: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
+000116c0: 7465 5f70 7265 6473 2e61 7373 6572 745f  te_preds.assert_
+000116d0: 6e6f 745f 6361 6c6c 6564 2829 0a20 2020  not_called().   
+000116e0: 206d 6f63 6b5f 6765 6e65 7261 7465 5f66   mock_generate_f
+000116f0: 6565 6462 6163 6b2e 6173 7365 7274 5f6e  eedback.assert_n
+00011700: 6f74 5f63 616c 6c65 6428 290a 0a0a 4070  ot_called()...@p
+00011710: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
+00011720: 6574 7269 7a65 280a 2020 2020 2274 696d  etrize(.    "tim
+00011730: 6573 7461 6d70 7322 2c0a 2020 2020 5b0a  estamps",.    [.
+00011740: 2020 2020 2020 2020 6e70 2e61 7272 6179          np.array
+00011750: 285b 3230 302c 2032 3031 5d29 2c0a 2020  ([200, 201]),.  
+00011760: 2020 2020 2020 6e70 2e61 7272 6179 285b        np.array([
+00011770: 3230 302c 2043 5552 5245 4e54 5f54 494d  200, CURRENT_TIM
+00011780: 455d 292c 0a20 2020 205d 2c0a 290a 406d  E]),.    ],.).@m
+00011790: 6f63 6b2e 7061 7463 6828 2267 616e 7472  ock.patch("gantr
+000117a0: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+000117b0: 4761 6e74 7279 2e5f 6c6f 675f 7072 6564  Gantry._log_pred
+000117c0: 6963 7469 6f6e 5f61 6e64 5f66 6565 6462  iction_and_feedb
+000117d0: 6163 6b5f 6576 656e 7473 2229 0a40 6d6f  ack_events").@mo
+000117e0: 636b 2e70 6174 6368 2822 6761 6e74 7279  ck.patch("gantry
+000117f0: 2e6c 6f67 6765 722e 636c 6965 6e74 2e47  .logger.client.G
+00011800: 616e 7472 792e 5f6c 6f67 5f70 7265 6469  antry._log_predi
+00011810: 6374 696f 6e5f 6576 656e 7473 2229 0a40  ction_events").@
+00011820: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
+00011830: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
+00011840: 2e47 616e 7472 792e 5f6c 6f67 5f66 6565  .Gantry._log_fee
+00011850: 6462 6163 6b5f 6576 656e 7473 2229 0a64  dback_events").d
+00011860: 6566 2074 6573 745f 6c6f 675f 7265 636f  ef test_log_reco
+00011870: 7264 735f 7072 6564 735f 616e 645f 6665  rds_preds_and_fe
+00011880: 6564 6261 636b 5f77 726f 6e67 5f74 696d  edback_wrong_tim
+00011890: 6573 7461 6d70 7328 0a20 2020 206d 6f63  estamps(.    moc
+000118a0: 6b5f 6665 6564 6261 636b 2c0a 2020 2020  k_feedback,.    
+000118b0: 6d6f 636b 5f70 7265 6473 2c0a 2020 2020  mock_preds,.    
+000118c0: 6d6f 636b 5f70 7265 6473 5f61 6e64 5f66  mock_preds_and_f
+000118d0: 6565 6462 6163 6b2c 0a20 2020 2074 696d  eedback,.    tim
+000118e0: 6573 7461 6d70 732c 0a20 2020 2063 6c69  estamps,.    cli
+000118f0: 5f6f 626a 2c0a 293a 0a20 2020 2061 7373  _obj,.):.    ass
+00011900: 6572 7420 280a 2020 2020 2020 2020 636c  ert (.        cl
+00011910: 695f 6f62 6a2e 6c6f 675f 7265 636f 7264  i_obj.log_record
+00011920: 7328 0a20 2020 2020 2020 2020 2020 2061  s(.            a
+00011930: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
+00011940: 6172 222c 0a20 2020 2020 2020 2020 2020  ar",.           
+00011950: 2076 6572 7369 6f6e 3d22 312e 322e 3322   version="1.2.3"
+00011960: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+00011970: 7075 7473 3d5b 7b22 666f 6f22 3a20 2262  puts=[{"foo": "b
+00011980: 6172 227d 2c20 7b22 666f 6f22 3a20 2262  ar"}, {"foo": "b
+00011990: 617a 227d 5d2c 0a20 2020 2020 2020 2020  az"}],.         
+000119a0: 2020 206f 7574 7075 7473 3d5b 7b22 666f     outputs=[{"fo
+000119b0: 6f22 3a20 2262 6172 227d 2c20 7b22 666f  o": "bar"}, {"fo
+000119c0: 6f22 3a20 2262 617a 227d 5d2c 0a20 2020  o": "baz"}],.   
+000119d0: 2020 2020 2020 2020 2066 6565 6462 6163           feedbac
+000119e0: 6b73 3d4e 6f6e 652c 0a20 2020 2020 2020  ks=None,.       
+000119f0: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
+00011a00: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
+00011a10: 2020 2020 2020 2020 736f 7274 5f6f 6e5f          sort_on_
+00011a20: 7469 6d65 7374 616d 703d 5472 7565 2c0a  timestamp=True,.
+00011a30: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+00011a40: 6c65 5f72 6174 653d 312c 0a20 2020 2020  le_rate=1,.     
+00011a50: 2020 2020 2020 206a 6f69 6e5f 6b65 7973         join_keys
+00011a60: 3d5b 2266 6f6f 6261 7222 2c20 2262 6172  =["foobar", "bar
+00011a70: 6261 7a22 5d2c 0a20 2020 2020 2020 2029  baz"],.        )
+00011a80: 0a20 2020 2020 2020 2069 7320 4e6f 6e65  .        is None
+00011a90: 0a20 2020 2029 0a20 2020 206d 6f63 6b5f  .    ).    mock_
+00011aa0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+00011ab0: 636b 2e61 7373 6572 745f 6e6f 745f 6361  ck.assert_not_ca
+00011ac0: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
+00011ad0: 7072 6564 732e 6173 7365 7274 5f6e 6f74  preds.assert_not
+00011ae0: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
+00011af0: 636b 5f66 6565 6462 6163 6b2e 6173 7365  ck_feedback.asse
+00011b00: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
+00011b10: 0a0a 4070 7974 6573 742e 6d61 726b 2e70  ..@pytest.mark.p
+00011b20: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
+00011b30: 2274 696d 6573 7461 6d70 7322 2c0a 2020  "timestamps",.  
+00011b40: 2020 5b0a 2020 2020 2020 2020 6e70 2e61    [.        np.a
+00011b50: 7272 6179 285b 3230 302c 2032 3031 5d29  rray([200, 201])
+00011b60: 2c0a 2020 2020 2020 2020 6e70 2e61 7272  ,.        np.arr
+00011b70: 6179 285b 3230 302c 2043 5552 5245 4e54  ay([200, CURRENT
+00011b80: 5f54 494d 455d 292c 0a20 2020 205d 2c0a  _TIME]),.    ],.
+00011b90: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+00011ba0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+00011bb0: 656e 742e 4761 6e74 7279 2e5f 6765 6e65  ent.Gantry._gene
+00011bc0: 7261 7465 5f70 7265 6469 6374 696f 6e5f  rate_prediction_
+00011bd0: 616e 645f 6665 6564 6261 636b 5f65 7665  and_feedback_eve
+00011be0: 6e74 7322 290a 406d 6f63 6b2e 7061 7463  nts").@mock.patc
+00011bf0: 6828 2267 616e 7472 792e 6c6f 6767 6572  h("gantry.logger
+00011c00: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
+00011c10: 6765 6e65 7261 7465 5f70 7265 6469 6374  generate_predict
+00011c20: 696f 6e5f 6576 656e 7473 2229 0a40 6d6f  ion_events").@mo
+00011c30: 636b 2e70 6174 6368 2822 6761 6e74 7279  ck.patch("gantry
+00011c40: 2e6c 6f67 6765 722e 636c 6965 6e74 2e47  .logger.client.G
+00011c50: 616e 7472 792e 5f67 656e 6572 6174 655f  antry._generate_
+00011c60: 6665 6564 6261 636b 5f65 7665 6e74 7322  feedback_events"
+00011c70: 290a 6465 6620 7465 7374 5f67 656e 6572  ).def test_gener
+00011c80: 6174 655f 7265 636f 7264 735f 7072 6564  ate_records_pred
+00011c90: 735f 616e 645f 6665 6564 6261 636b 5f77  s_and_feedback_w
+00011ca0: 726f 6e67 5f74 696d 6573 7461 6d70 7328  rong_timestamps(
+00011cb0: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
+00011cc0: 7465 5f66 6565 6462 6163 6b2c 0a20 2020  te_feedback,.   
+00011cd0: 206d 6f63 6b5f 6765 6e65 7261 7465 5f70   mock_generate_p
+00011ce0: 7265 6473 2c0a 2020 2020 6d6f 636b 5f67  reds,.    mock_g
+00011cf0: 656e 6572 6174 655f 7072 6564 735f 616e  enerate_preds_an
+00011d00: 645f 6665 6564 6261 636b 2c0a 2020 2020  d_feedback,.    
+00011d10: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
+00011d20: 636c 695f 6f62 6a2c 0a29 3a0a 2020 2020  cli_obj,.):.    
+00011d30: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
+00011d40: 2063 6c69 5f6f 626a 2e67 656e 6572 6174   cli_obj.generat
+00011d50: 655f 7265 636f 7264 7328 0a20 2020 2020  e_records(.     
+00011d60: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
+00011d70: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
+00011d80: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
+00011d90: 3d22 312e 322e 3322 2c0a 2020 2020 2020  ="1.2.3",.      
+00011da0: 2020 2020 2020 696e 7075 7473 3d5b 7b22        inputs=[{"
+00011db0: 666f 6f22 3a20 2262 6172 227d 2c20 7b22  foo": "bar"}, {"
+00011dc0: 666f 6f22 3a20 2262 617a 227d 5d2c 0a20  foo": "baz"}],. 
+00011dd0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00011de0: 7473 3d5b 7b22 666f 6f22 3a20 2262 6172  ts=[{"foo": "bar
+00011df0: 227d 2c20 7b22 666f 6f22 3a20 2262 617a  "}, {"foo": "baz
+00011e00: 227d 5d2c 0a20 2020 2020 2020 2020 2020  "}],.           
+00011e10: 2066 6565 6462 6163 6b73 3d4e 6f6e 652c   feedbacks=None,
+00011e20: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00011e30: 6573 7461 6d70 733d 7469 6d65 7374 616d  estamps=timestam
+00011e40: 7073 2c0a 2020 2020 2020 2020 2020 2020  ps,.            
+00011e50: 736f 7274 5f6f 6e5f 7469 6d65 7374 616d  sort_on_timestam
+00011e60: 703d 5472 7565 2c0a 2020 2020 2020 2020  p=True,.        
+00011e70: 2020 2020 7361 6d70 6c65 5f72 6174 653d      sample_rate=
+00011e80: 312c 0a20 2020 2020 2020 2020 2020 206a  1,.            j
+00011e90: 6f69 6e5f 6b65 7973 3d5b 2266 6f6f 6261  oin_keys=["fooba
+00011ea0: 7222 2c20 2262 6172 6261 7a22 5d2c 0a20  r", "barbaz"],. 
+00011eb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011ec0: 2069 7320 4e6f 6e65 0a20 2020 2029 0a20   is None.    ). 
+00011ed0: 2020 206d 6f63 6b5f 6765 6e65 7261 7465     mock_generate
+00011ee0: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
+00011ef0: 6163 6b2e 6173 7365 7274 5f6e 6f74 5f63  ack.assert_not_c
+00011f00: 616c 6c65 6428 290a 2020 2020 6d6f 636b  alled().    mock
+00011f10: 5f67 656e 6572 6174 655f 7072 6564 732e  _generate_preds.
+00011f20: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
+00011f30: 6428 290a 2020 2020 6d6f 636b 5f67 656e  d().    mock_gen
+00011f40: 6572 6174 655f 6665 6564 6261 636b 2e61  erate_feedback.a
+00011f50: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
+00011f60: 2829 0a0a 0a40 7079 7465 7374 2e6d 6172  ()...@pytest.mar
+00011f70: 6b2e 7061 7261 6d65 7472 697a 6528 226a  k.parametrize("j
+00011f80: 6f69 6e5f 6b65 7973 222c 205b 5b31 2c20  oin_keys", [[1, 
+00011f90: 322c 2033 5d2c 2070 642e 5365 7269 6573  2, 3], pd.Series
+00011fa0: 285b 312c 2032 2c20 335d 295d 290a 406d  ([1, 2, 3])]).@m
+00011fb0: 6f63 6b2e 7061 7463 6828 2267 616e 7472  ock.patch("gantr
+00011fc0: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+00011fd0: 4761 6e74 7279 2e5f 6c6f 675f 7072 6564  Gantry._log_pred
+00011fe0: 6963 7469 6f6e 5f61 6e64 5f66 6565 6462  iction_and_feedb
+00011ff0: 6163 6b5f 6576 656e 7473 2229 0a40 6d6f  ack_events").@mo
+00012000: 636b 2e70 6174 6368 2822 6761 6e74 7279  ck.patch("gantry
+00012010: 2e6c 6f67 6765 722e 636c 6965 6e74 2e47  .logger.client.G
+00012020: 616e 7472 792e 5f6c 6f67 5f70 7265 6469  antry._log_predi
+00012030: 6374 696f 6e5f 6576 656e 7473 2229 0a40  ction_events").@
+00012040: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
+00012050: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
+00012060: 2e47 616e 7472 792e 5f6c 6f67 5f66 6565  .Gantry._log_fee
+00012070: 6462 6163 6b5f 6576 656e 7473 2229 0a64  dback_events").d
+00012080: 6566 2074 6573 745f 6c6f 675f 7265 636f  ef test_log_reco
+00012090: 7264 735f 7072 6564 735f 616e 645f 6665  rds_preds_and_fe
+000120a0: 6564 6261 636b 5f77 726f 6e67 5f6a 6f69  edback_wrong_joi
+000120b0: 6e5f 6b65 7973 280a 2020 2020 6d6f 636b  n_keys(.    mock
+000120c0: 5f66 6565 6462 6163 6b2c 0a20 2020 206d  _feedback,.    m
+000120d0: 6f63 6b5f 7072 6564 732c 0a20 2020 206d  ock_preds,.    m
+000120e0: 6f63 6b5f 7072 6564 735f 616e 645f 6665  ock_preds_and_fe
+000120f0: 6564 6261 636b 2c0a 2020 2020 6a6f 696e  edback,.    join
+00012100: 5f6b 6579 732c 0a20 2020 2063 6c69 5f6f  _keys,.    cli_o
+00012110: 626a 2c0a 293a 0a20 2020 2061 7373 6572  bj,.):.    asser
+00012120: 7420 280a 2020 2020 2020 2020 636c 695f  t (.        cli_
+00012130: 6f62 6a2e 6c6f 675f 7265 636f 7264 7328  obj.log_records(
+00012140: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+00012150: 6c69 6361 7469 6f6e 3d22 666f 6f62 6172  lication="foobar
+00012160: 222c 0a20 2020 2020 2020 2020 2020 2076  ",.            v
+00012170: 6572 7369 6f6e 3d22 312e 322e 3322 2c0a  ersion="1.2.3",.
+00012180: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+00012190: 7473 3d5b 7b22 4122 3a20 3230 307d 2c20  ts=[{"A": 200}, 
+000121a0: 7b22 4122 3a20 3230 317d 5d2c 0a20 2020  {"A": 201}],.   
+000121b0: 2020 2020 2020 2020 206f 7574 7075 7473           outputs
+000121c0: 3d5b 7b22 4222 3a20 3230 307d 2c20 7b22  =[{"B": 200}, {"
+000121d0: 4222 3a20 3230 317d 5d2c 0a20 2020 2020  B": 201}],.     
+000121e0: 2020 2020 2020 2066 6565 6462 6163 6b73         feedbacks
+000121f0: 3d5b 7b22 4322 3a20 3230 307d 2c20 7b22  =[{"C": 200}, {"
+00012200: 4322 3a20 3230 317d 5d2c 0a20 2020 2020  C": 201}],.     
+00012210: 2020 2020 2020 2074 696d 6573 7461 6d70         timestamp
+00012220: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+00012230: 2020 2020 736f 7274 5f6f 6e5f 7469 6d65      sort_on_time
+00012240: 7374 616d 703d 5472 7565 2c0a 2020 2020  stamp=True,.    
+00012250: 2020 2020 2020 2020 7361 6d70 6c65 5f72          sample_r
+00012260: 6174 653d 312c 0a20 2020 2020 2020 2020  ate=1,.         
+00012270: 2020 206a 6f69 6e5f 6b65 7973 3d6a 6f69     join_keys=joi
+00012280: 6e5f 6b65 7973 2c0a 2020 2020 2020 2020  n_keys,.        
+00012290: 290a 2020 2020 2020 2020 6973 204e 6f6e  ).        is Non
+000122a0: 650a 2020 2020 290a 2020 2020 6d6f 636b  e.    ).    mock
+000122b0: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
+000122c0: 6163 6b2e 6173 7365 7274 5f6e 6f74 5f63  ack.assert_not_c
+000122d0: 616c 6c65 6428 290a 2020 2020 6d6f 636b  alled().    mock
+000122e0: 5f70 7265 6473 2e61 7373 6572 745f 6e6f  _preds.assert_no
+000122f0: 745f 6361 6c6c 6564 2829 0a20 2020 206d  t_called().    m
+00012300: 6f63 6b5f 6665 6564 6261 636b 2e61 7373  ock_feedback.ass
+00012310: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
+00012320: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+00012330: 7061 7261 6d65 7472 697a 6528 226a 6f69  parametrize("joi
+00012340: 6e5f 6b65 7973 222c 205b 5b31 2c20 322c  n_keys", [[1, 2,
+00012350: 2033 5d2c 2070 642e 5365 7269 6573 285b   3], pd.Series([
+00012360: 312c 2032 2c20 335d 295d 290a 406d 6f63  1, 2, 3])]).@moc
+00012370: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
+00012380: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
+00012390: 6e74 7279 2e5f 6765 6e65 7261 7465 5f70  ntry._generate_p
+000123a0: 7265 6469 6374 696f 6e5f 616e 645f 6665  rediction_and_fe
+000123b0: 6564 6261 636b 5f65 7665 6e74 7322 290a  edback_events").
+000123c0: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
+000123d0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
+000123e0: 742e 4761 6e74 7279 2e5f 6765 6e65 7261  t.Gantry._genera
+000123f0: 7465 5f70 7265 6469 6374 696f 6e5f 6576  te_prediction_ev
+00012400: 656e 7473 2229 0a40 6d6f 636b 2e70 6174  ents").@mock.pat
+00012410: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
+00012420: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
+00012430: 5f67 656e 6572 6174 655f 6665 6564 6261  _generate_feedba
+00012440: 636b 5f65 7665 6e74 7322 290a 6465 6620  ck_events").def 
+00012450: 7465 7374 5f67 656e 6572 6174 655f 7265  test_generate_re
+00012460: 636f 7264 735f 7072 6564 735f 616e 645f  cords_preds_and_
+00012470: 6665 6564 6261 636b 5f77 726f 6e67 5f6a  feedback_wrong_j
+00012480: 6f69 6e5f 6b65 7973 280a 2020 2020 6d6f  oin_keys(.    mo
+00012490: 636b 5f67 656e 6572 6174 655f 6665 6564  ck_generate_feed
+000124a0: 6261 636b 2c0a 2020 2020 6d6f 636b 5f67  back,.    mock_g
+000124b0: 656e 6572 6174 655f 7072 6564 732c 0a20  enerate_preds,. 
+000124c0: 2020 206d 6f63 6b5f 6765 6e65 7261 7465     mock_generate
+000124d0: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
+000124e0: 6163 6b2c 0a20 2020 206a 6f69 6e5f 6b65  ack,.    join_ke
+000124f0: 7973 2c0a 2020 2020 636c 695f 6f62 6a2c  ys,.    cli_obj,
+00012500: 0a29 3a0a 2020 2020 6173 7365 7274 2028  .):.    assert (
+00012510: 0a20 2020 2020 2020 2063 6c69 5f6f 626a  .        cli_obj
+00012520: 2e67 656e 6572 6174 655f 7265 636f 7264  .generate_record
+00012530: 7328 0a20 2020 2020 2020 2020 2020 2061  s(.            a
+00012540: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
+00012550: 6172 222c 0a20 2020 2020 2020 2020 2020  ar",.           
+00012560: 2076 6572 7369 6f6e 3d22 312e 322e 3322   version="1.2.3"
+00012570: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+00012580: 7075 7473 3d5b 7b22 4122 3a20 3230 307d  puts=[{"A": 200}
+00012590: 2c20 7b22 4122 3a20 3230 317d 5d2c 0a20  , {"A": 201}],. 
+000125a0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000125b0: 7473 3d5b 7b22 4222 3a20 3230 307d 2c20  ts=[{"B": 200}, 
+000125c0: 7b22 4222 3a20 3230 317d 5d2c 0a20 2020  {"B": 201}],.   
+000125d0: 2020 2020 2020 2020 2066 6565 6462 6163           feedbac
+000125e0: 6b73 3d5b 7b22 4322 3a20 3230 307d 2c20  ks=[{"C": 200}, 
+000125f0: 7b22 4322 3a20 3230 317d 5d2c 0a20 2020  {"C": 201}],.   
+00012600: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
+00012610: 6d70 733d 4e6f 6e65 2c0a 2020 2020 2020  mps=None,.      
+00012620: 2020 2020 2020 736f 7274 5f6f 6e5f 7469        sort_on_ti
+00012630: 6d65 7374 616d 703d 5472 7565 2c0a 2020  mestamp=True,.  
+00012640: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+00012650: 5f72 6174 653d 312c 0a20 2020 2020 2020  _rate=1,.       
+00012660: 2020 2020 206a 6f69 6e5f 6b65 7973 3d6a       join_keys=j
+00012670: 6f69 6e5f 6b65 7973 2c0a 2020 2020 2020  oin_keys,.      
+00012680: 2020 290a 2020 2020 2020 2020 6973 204e    ).        is N
+00012690: 6f6e 650a 2020 2020 290a 2020 2020 6d6f  one.    ).    mo
+000126a0: 636b 5f67 656e 6572 6174 655f 7072 6564  ck_generate_pred
+000126b0: 735f 616e 645f 6665 6564 6261 636b 2e61  s_and_feedback.a
+000126c0: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
+000126d0: 2829 0a20 2020 206d 6f63 6b5f 6765 6e65  ().    mock_gene
+000126e0: 7261 7465 5f70 7265 6473 2e61 7373 6572  rate_preds.asser
+000126f0: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
+00012700: 2020 206d 6f63 6b5f 6765 6e65 7261 7465     mock_generate
+00012710: 5f66 6565 6462 6163 6b2e 6173 7365 7274  _feedback.assert
+00012720: 5f6e 6f74 5f63 616c 6c65 6428 290a 0a0a  _not_called()...
+00012730: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
+00012740: 616d 6574 7269 7a65 280a 2020 2020 2274  ametrize(.    "t
+00012750: 6573 745f 7469 6d65 7374 616d 7073 2c20  est_timestamps, 
+00012760: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
+00012770: 6c69 7374 222c 0a20 2020 205b 0a20 2020  list",.    [.   
+00012780: 2020 2020 2028 4e6f 6e65 2c20 4e6f 6e65       (None, None
+00012790: 292c 0a20 2020 2020 2020 2028 5b43 5552  ),.        ([CUR
+000127a0: 5245 4e54 5f54 494d 455d 202a 2032 2c20  RENT_TIME] * 2, 
+000127b0: 5b43 5552 5245 4e54 5f54 494d 455d 202a  [CURRENT_TIME] *
+000127c0: 2032 292c 0a20 2020 2020 2020 2028 6e70   2),.        (np
+000127d0: 2e61 7272 6179 285b 4355 5252 454e 545f  .array([CURRENT_
+000127e0: 5449 4d45 5d20 2a20 3229 2c20 5b43 5552  TIME] * 2), [CUR
+000127f0: 5245 4e54 5f54 494d 455d 202a 2032 292c  RENT_TIME] * 2),
+00012800: 0a20 2020 205d 2c0a 290a 4070 7974 6573  .    ],.).@pytes
+00012810: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+00012820: 7a65 280a 2020 2020 226b 7761 7267 7322  ze(.    "kwargs"
+00012830: 2c0a 2020 2020 5b0a 2020 2020 2020 2020  ,.    [.        
+00012840: 7b22 6665 6564 6261 636b 5f6b 6579 7322  {"feedback_keys"
+00012850: 3a20 5b22 4122 5d7d 2c0a 2020 2020 2020  : ["A"]},.      
+00012860: 2020 7b22 6665 6564 6261 636b 5f69 6473    {"feedback_ids
+00012870: 223a 205b 2231 3233 3435 222c 2022 3637  ": ["12345", "67
+00012880: 3839 3022 5d7d 2c0a 2020 2020 2020 2020  890"]},.        
+00012890: 7b22 6a6f 696e 5f6b 6579 7322 3a20 5b22  {"join_keys": ["
+000128a0: 3534 3332 3122 2c20 2236 3738 3930 225d  54321", "67890"]
+000128b0: 7d2c 0a20 2020 2020 2020 207b 226a 6f69  },.        {"joi
+000128c0: 6e5f 6b65 7973 223a 2070 642e 5365 7269  n_keys": pd.Seri
+000128d0: 6573 285b 2235 3433 3231 222c 2022 3637  es(["54321", "67
+000128e0: 3839 3022 5d29 7d2c 0a20 2020 2020 2020  890"])},.       
+000128f0: 207b 7d2c 0a20 2020 205d 2c0a 290a 4070   {},.    ],.).@p
+00012900: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
+00012910: 6574 7269 7a65 280a 2020 2020 2822 7465  etrize(.    ("te
+00012920: 7374 5f6f 7574 7075 7473 222c 2022 7465  st_outputs", "te
+00012930: 7374 5f69 6e70 7574 7322 292c 0a20 2020  st_inputs"),.   
+00012940: 206c 6973 7428 7a69 7028 5445 5354 5f4f   list(zip(TEST_O
+00012950: 5554 5055 5453 2c20 5445 5354 5f49 4e50  UTPUTS, TEST_INP
+00012960: 5554 5329 292c 0a29 0a40 7079 7465 7374  UTS)),.).@pytest
+00012970: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00012980: 6528 2276 6572 7369 6f6e 222c 205b 4e6f  e("version", [No
+00012990: 6e65 2c20 3130 2c20 2231 2e32 2e33 225d  ne, 10, "1.2.3"]
+000129a0: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
+000129b0: 6172 616d 6574 7269 7a65 2822 7461 6773  arametrize("tags
+000129c0: 2c20 726f 775f 7461 6773 2c20 676c 6f62  , row_tags, glob
+000129d0: 616c 5f74 6167 732c 2065 7870 6563 7465  al_tags, expecte
+000129e0: 645f 7461 6773 5f70 6172 616d 222c 2054  d_tags_param", T
+000129f0: 4553 545f 5441 4753 290a 406d 6f63 6b2e  EST_TAGS).@mock.
+00012a00: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+00012a10: 6767 6572 2e63 6c69 656e 742e 5f72 6573  gger.client._res
+00012a20: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2229  olve_join_keys")
+00012a30: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
+00012a40: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+00012a50: 6e74 2e47 616e 7472 792e 5f6c 6f67 5f70  nt.Gantry._log_p
+00012a60: 7265 6469 6374 696f 6e5f 616e 645f 6665  rediction_and_fe
+00012a70: 6564 6261 636b 5f65 7665 6e74 7322 290a  edback_events").
+00012a80: 406d 6f63 6b2e 7061 7463 6828 0a20 2020  @mock.patch(.   
+00012a90: 2022 6761 6e74 7279 2e6c 6f67 6765 722e   "gantry.logger.
+00012aa0: 636c 6965 6e74 2e47 616e 7472 792e 5f6c  client.Gantry._l
+00012ab0: 6f67 5f70 7265 6469 6374 696f 6e5f 6576  og_prediction_ev
+00012ac0: 656e 7473 222c 2072 6574 7572 6e5f 7661  ents", return_va
+00012ad0: 6c75 653d 284e 6f6e 652c 205b 2231 3233  lue=(None, ["123
+00012ae0: 3435 222c 2022 3637 3839 3022 5d29 0a29  45", "67890"]).)
+00012af0: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
+00012b00: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+00012b10: 6e74 2e47 616e 7472 792e 5f6c 6f67 5f66  nt.Gantry._log_f
+00012b20: 6565 6462 6163 6b5f 6576 656e 7473 2229  eedback_events")
 00012b30: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
 00012b40: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
-00012b50: 6e74 2e5f 6465 6661 756c 745f 6a6f 696e  nt._default_join
-00012b60: 5f6b 6579 5f67 656e 2229 0a64 6566 2074  _key_gen").def t
-00012b70: 6573 745f 6c6f 675f 7265 636f 7264 735f  est_log_records_
-00012b80: 7072 6564 735f 6f6e 6c79 280a 2020 2020  preds_only(.    
-00012b90: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
-00012ba0: 6e2c 0a20 2020 206d 6f63 6b5f 7361 6d70  n,.    mock_samp
-00012bb0: 6c65 5f72 6563 6f72 6473 2c0a 2020 2020  le_records,.    
-00012bc0: 6d6f 636b 5f66 6565 6462 6163 6b2c 0a20  mock_feedback,. 
-00012bd0: 2020 206d 6f63 6b5f 7072 6564 732c 0a20     mock_preds,. 
-00012be0: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
-00012bf0: 645f 6665 6564 6261 636b 2c0a 2020 2020  d_feedback,.    
-00012c00: 6d6f 636b 5f72 6573 6f6c 7665 5f6a 6f69  mock_resolve_joi
-00012c10: 6e5f 6b65 7973 2c0a 2020 2020 7665 7273  n_keys,.    vers
-00012c20: 696f 6e2c 0a20 2020 2074 6167 732c 0a20  ion,.    tags,. 
-00012c30: 2020 2072 6f77 5f74 6167 732c 0a20 2020     row_tags,.   
-00012c40: 2067 6c6f 6261 6c5f 7461 6773 2c0a 2020   global_tags,.  
-00012c50: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
-00012c60: 7061 7261 6d2c 0a20 2020 2074 6573 745f  param,.    test_
-00012c70: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
-00012c80: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
-00012c90: 6c69 7374 2c0a 2020 2020 7465 7374 5f69  list,.    test_i
-00012ca0: 6e70 7574 732c 0a20 2020 2074 6573 745f  nputs,.    test_
-00012cb0: 6f75 7470 7574 732c 0a20 2020 206b 7761  outputs,.    kwa
-00012cc0: 7267 732c 0a20 2020 2063 6c69 5f6f 626a  rgs,.    cli_obj
-00012cd0: 2c0a 293a 0a20 2020 206d 6f63 6b5f 6a6f  ,.):.    mock_jo
-00012ce0: 696e 5f6b 6579 5f67 656e 2e73 6964 655f  in_key_gen.side_
-00012cf0: 6566 6665 6374 203d 205b 2236 3738 3930  effect = ["67890
-00012d00: 222c 2022 3132 3334 3522 5d0a 2020 2020  ", "12345"].    
-00012d10: 6d6f 636b 5f72 6573 6f6c 7665 5f6a 6f69  mock_resolve_joi
-00012d20: 6e5f 6b65 7973 2e72 6574 7572 6e5f 7661  n_keys.return_va
-00012d30: 6c75 6520 3d20 5b22 3132 3334 3522 2c20  lue = ["12345", 
-00012d40: 2236 3738 3930 225d 2069 6620 6b77 6172  "67890"] if kwar
-00012d50: 6773 2065 6c73 6520 4e6f 6e65 0a20 2020  gs else None.   
-00012d60: 2061 7373 6572 7420 636c 695f 6f62 6a2e   assert cli_obj.
-00012d70: 6c6f 675f 7265 636f 7264 7328 0a20 2020  log_records(.   
-00012d80: 2020 2020 2061 7070 6c69 6361 7469 6f6e       application
-00012d90: 3d22 666f 6f62 6172 222c 0a20 2020 2020  ="foobar",.     
-00012da0: 2020 2076 6572 7369 6f6e 3d76 6572 7369     version=versi
-00012db0: 6f6e 2c0a 2020 2020 2020 2020 696e 7075  on,.        inpu
-00012dc0: 7473 3d74 6573 745f 696e 7075 7473 2c0a  ts=test_inputs,.
-00012dd0: 2020 2020 2020 2020 6f75 7470 7574 733d          outputs=
-00012de0: 7465 7374 5f6f 7574 7075 7473 2c0a 2020  test_outputs,.  
-00012df0: 2020 2020 2020 6665 6564 6261 636b 733d        feedbacks=
-00012e00: 4e6f 6e65 2c0a 2020 2020 2020 2020 7469  None,.        ti
-00012e10: 6d65 7374 616d 7073 3d74 6573 745f 7469  mestamps=test_ti
-00012e20: 6d65 7374 616d 7073 2c0a 2020 2020 2020  mestamps,.      
-00012e30: 2020 736f 7274 5f6f 6e5f 7469 6d65 7374    sort_on_timest
-00012e40: 616d 703d 5472 7565 2c0a 2020 2020 2020  amp=True,.      
-00012e50: 2020 7461 6773 3d74 6167 732c 0a20 2020    tags=tags,.   
-00012e60: 2020 2020 2072 6f77 5f74 6167 733d 726f       row_tags=ro
-00012e70: 775f 7461 6773 2c0a 2020 2020 2020 2020  w_tags,.        
-00012e80: 676c 6f62 616c 5f74 6167 733d 676c 6f62  global_tags=glob
-00012e90: 616c 5f74 6167 732c 0a20 2020 2020 2020  al_tags,.       
-00012ea0: 202a 2a6b 7761 7267 732c 0a20 2020 2029   **kwargs,.    )
-00012eb0: 203d 3d20 284e 6f6e 652c 205b 2231 3233   == (None, ["123
-00012ec0: 3435 222c 2022 3637 3839 3022 5d29 0a0a  45", "67890"])..
-00012ed0: 2020 2020 6d6f 636b 5f70 7265 6473 5f61      mock_preds_a
-00012ee0: 6e64 5f66 6565 6462 6163 6b2e 6173 7365  nd_feedback.asse
-00012ef0: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00012f00: 2020 2020 6d6f 636b 5f70 7265 6473 2e61      mock_preds.a
-00012f10: 7373 6572 745f 6361 6c6c 6564 5f6f 6e63  ssert_called_onc
-00012f20: 655f 7769 7468 280a 2020 2020 2020 2020  e_with(.        
-00012f30: 6170 706c 6963 6174 696f 6e3d 2266 6f6f  application="foo
-00012f40: 6261 7222 2c0a 2020 2020 2020 2020 696e  bar",.        in
-00012f50: 7075 7473 3d5b 7b22 4122 3a20 3130 307d  puts=[{"A": 100}
-00012f60: 2c20 7b22 4122 3a20 3130 317d 5d2c 0a20  , {"A": 101}],. 
-00012f70: 2020 2020 2020 206f 7574 7075 7473 3d5b         outputs=[
-00012f80: 7b22 4222 3a20 3330 307d 2c20 7b22 4222  {"B": 300}, {"B"
-00012f90: 3a20 3330 317d 5d2c 0a20 2020 2020 2020  : 301}],.       
-00012fa0: 206a 6f69 6e5f 6b65 7973 3d5b 2231 3233   join_keys=["123
-00012fb0: 3435 222c 2022 3637 3839 3022 5d20 6966  45", "67890"] if
-00012fc0: 206b 7761 7267 7320 656c 7365 205b 2236   kwargs else ["6
-00012fd0: 3738 3930 222c 2022 3132 3334 3522 5d2c  7890", "12345"],
-00012fe0: 0a20 2020 2020 2020 2076 6572 7369 6f6e  .        version
-00012ff0: 3d76 6572 7369 6f6e 2c0a 2020 2020 2020  =version,.      
-00013000: 2020 6967 6e6f 7265 5f69 6e70 7574 733d    ignore_inputs=
-00013010: 4e6f 6e65 2c0a 2020 2020 2020 2020 7469  None,.        ti
-00013020: 6d65 7374 616d 7073 3d74 6573 745f 7469  mestamps=test_ti
-00013030: 6d65 7374 616d 7073 5f6c 6973 742c 0a20  mestamps_list,. 
-00013040: 2020 2020 2020 2073 6f72 745f 6f6e 5f74         sort_on_t
-00013050: 696d 6573 7461 6d70 3d54 7275 652c 0a20  imestamp=True,. 
-00013060: 2020 2020 2020 2061 735f 6261 7463 683d         as_batch=
-00013070: 4661 6c73 652c 0a20 2020 2020 2020 2074  False,.        t
-00013080: 6167 733d 6578 7065 6374 6564 5f74 6167  ags=expected_tag
-00013090: 735f 7061 7261 6d2c 0a20 2020 2029 0a20  s_param,.    ). 
-000130a0: 2020 206d 6f63 6b5f 6665 6564 6261 636b     mock_feedback
-000130b0: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-000130c0: 6564 2829 0a0a 2020 2020 6d6f 636b 5f73  ed()..    mock_s
-000130d0: 616d 706c 655f 7265 636f 7264 732e 6173  ample_records.as
-000130e0: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
-000130f0: 5f77 6974 6828 0a20 2020 2020 2020 2032  _with(.        2
-00013100: 2c0a 2020 2020 2020 2020 312c 0a20 2020  ,.        1,.   
-00013110: 2020 2020 205b 7b22 4122 3a20 3130 307d       [{"A": 100}
-00013120: 2c20 7b22 4122 3a20 3130 317d 5d2c 0a20  , {"A": 101}],. 
-00013130: 2020 2020 2020 205b 7b22 4222 3a20 3330         [{"B": 30
-00013140: 307d 2c20 7b22 4222 3a20 3330 317d 5d2c  0}, {"B": 301}],
-00013150: 0a20 2020 2020 2020 204e 6f6e 652c 0a20  .        None,. 
-00013160: 2020 2020 2020 2063 6c69 656e 742e 5f72         client._r
-00013170: 6573 6f6c 7665 5f6a 6f69 6e5f 6b65 7973  esolve_join_keys
-00013180: 282a 2a6b 7761 7267 7329 2c0a 2020 2020  (**kwargs),.    
-00013190: 2020 2020 7465 7374 5f74 696d 6573 7461      test_timesta
-000131a0: 6d70 735f 6c69 7374 2c0a 2020 2020 2020  mps_list,.      
-000131b0: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
-000131c0: 7061 7261 6d2c 0a20 2020 2029 0a0a 2020  param,.    )..  
-000131d0: 2020 6966 206b 7761 7267 733a 0a20 2020    if kwargs:.   
-000131e0: 2020 2020 206d 6f63 6b5f 6a6f 696e 5f6b       mock_join_k
-000131f0: 6579 5f67 656e 2e61 7373 6572 745f 6e6f  ey_gen.assert_no
-00013200: 745f 6361 6c6c 6564 2829 0a20 2020 2065  t_called().    e
-00013210: 6c73 653a 0a20 2020 2020 2020 206d 6f63  lse:.        moc
-00013220: 6b5f 6a6f 696e 5f6b 6579 5f67 656e 2e61  k_join_key_gen.a
-00013230: 7373 6572 745f 6361 6c6c 6564 2829 0a0a  ssert_called()..
-00013240: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
-00013250: 7261 6d65 7472 697a 6528 0a20 2020 2022  rametrize(.    "
-00013260: 7465 7374 5f74 696d 6573 7461 6d70 732c  test_timestamps,
-00013270: 2074 6573 745f 7469 6d65 7374 616d 7073   test_timestamps
-00013280: 5f6c 6973 7422 2c0a 2020 2020 5b0a 2020  _list",.    [.  
-00013290: 2020 2020 2020 284e 6f6e 652c 204e 6f6e        (None, Non
-000132a0: 6529 2c0a 2020 2020 2020 2020 285b 4355  e),.        ([CU
-000132b0: 5252 454e 545f 5449 4d45 5d20 2a20 322c  RRENT_TIME] * 2,
-000132c0: 205b 4355 5252 454e 545f 5449 4d45 5d20   [CURRENT_TIME] 
-000132d0: 2a20 3229 2c0a 2020 2020 2020 2020 286e  * 2),.        (n
-000132e0: 702e 6172 7261 7928 5b43 5552 5245 4e54  p.array([CURRENT
-000132f0: 5f54 494d 455d 202a 2032 292c 205b 4355  _TIME] * 2), [CU
-00013300: 5252 454e 545f 5449 4d45 5d20 2a20 3229  RRENT_TIME] * 2)
-00013310: 2c0a 2020 2020 5d2c 0a29 0a40 7079 7465  ,.    ],.).@pyte
-00013320: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-00013330: 697a 6528 0a20 2020 2022 6b77 6172 6773  ize(.    "kwargs
-00013340: 222c 0a20 2020 205b 0a20 2020 2020 2020  ",.    [.       
-00013350: 207b 2266 6565 6462 6163 6b5f 6b65 7973   {"feedback_keys
-00013360: 223a 205b 2241 225d 7d2c 0a20 2020 2020  ": ["A"]},.     
-00013370: 2020 207b 2266 6565 6462 6163 6b5f 6964     {"feedback_id
-00013380: 7322 3a20 5b22 3132 3334 3522 2c20 2236  s": ["12345", "6
-00013390: 3738 3930 225d 7d2c 0a20 2020 2020 2020  7890"]},.       
-000133a0: 207b 226a 6f69 6e5f 6b65 7973 223a 205b   {"join_keys": [
-000133b0: 2235 3433 3231 222c 2022 3637 3839 3022  "54321", "67890"
-000133c0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6a6f  ]},.        {"jo
-000133d0: 696e 5f6b 6579 7322 3a20 7064 2e53 6572  in_keys": pd.Ser
-000133e0: 6965 7328 5b22 3534 3332 3122 2c20 2236  ies(["54321", "6
-000133f0: 3738 3930 225d 297d 2c0a 2020 2020 2020  7890"])},.      
-00013400: 2020 7b7d 2c0a 2020 2020 5d2c 0a29 0a40    {},.    ],.).@
-00013410: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-00013420: 6d65 7472 697a 6528 0a20 2020 2028 2274  metrize(.    ("t
-00013430: 6573 745f 6f75 7470 7574 7322 2c20 2274  est_outputs", "t
-00013440: 6573 745f 696e 7075 7473 2229 2c0a 2020  est_inputs"),.  
-00013450: 2020 6c69 7374 287a 6970 2854 4553 545f    list(zip(TEST_
-00013460: 4f55 5450 5554 532c 2054 4553 545f 494e  OUTPUTS, TEST_IN
-00013470: 5055 5453 2929 2c0a 290a 4070 7974 6573  PUTS)),.).@pytes
-00013480: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00013490: 7a65 2822 7665 7273 696f 6e22 2c20 5b4e  ze("version", [N
-000134a0: 6f6e 652c 2031 302c 2022 312e 322e 3322  one, 10, "1.2.3"
-000134b0: 5d29 0a40 7079 7465 7374 2e6d 6172 6b2e  ]).@pytest.mark.
-000134c0: 7061 7261 6d65 7472 697a 6528 2274 6167  parametrize("tag
-000134d0: 732c 2072 6f77 5f74 6167 732c 2067 6c6f  s, row_tags, glo
-000134e0: 6261 6c5f 7461 6773 2c20 6578 7065 6374  bal_tags, expect
-000134f0: 6564 5f74 6167 735f 7061 7261 6d22 2c20  ed_tags_param", 
-00013500: 5445 5354 5f54 4147 5329 0a40 6d6f 636b  TEST_TAGS).@mock
-00013510: 2e70 6174 6368 2822 6761 6e74 7279 2e6c  .patch("gantry.l
-00013520: 6f67 6765 722e 636c 6965 6e74 2e5f 7265  ogger.client._re
-00013530: 736f 6c76 655f 6a6f 696e 5f6b 6579 7322  solve_join_keys"
-00013540: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-00013550: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00013560: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
-00013570: 7072 6564 6963 7469 6f6e 5f61 6e64 5f66  prediction_and_f
-00013580: 6565 6462 6163 6b5f 6576 656e 7473 2229  eedback_events")
-00013590: 0a40 6d6f 636b 2e70 6174 6368 280a 2020  .@mock.patch(.  
-000135a0: 2020 2267 616e 7472 792e 6c6f 6767 6572    "gantry.logger
-000135b0: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-000135c0: 6c6f 675f 7072 6564 6963 7469 6f6e 5f65  log_prediction_e
-000135d0: 7665 6e74 7322 2c20 7265 7475 726e 5f76  vents", return_v
-000135e0: 616c 7565 3d28 4e6f 6e65 2c20 5b22 3132  alue=(None, ["12
-000135f0: 3334 3522 2c20 2236 3738 3930 225d 290a  345", "67890"]).
-00013600: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-00013610: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00013620: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
-00013630: 6665 6564 6261 636b 5f65 7665 6e74 7322  feedback_events"
-00013640: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-00013650: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00013660: 656e 742e 5f73 616d 706c 655f 7265 636f  ent._sample_reco
-00013670: 7264 7322 2c20 7369 6465 5f65 6666 6563  rds", side_effec
-00013680: 743d 636c 6965 6e74 2e5f 7361 6d70 6c65  t=client._sample
-00013690: 5f72 6563 6f72 6473 290a 406d 6f63 6b2e  _records).@mock.
+00012b50: 6e74 2e5f 7361 6d70 6c65 5f72 6563 6f72  nt._sample_recor
+00012b60: 6473 222c 2073 6964 655f 6566 6665 6374  ds", side_effect
+00012b70: 3d63 6c69 656e 742e 5f73 616d 706c 655f  =client._sample_
+00012b80: 7265 636f 7264 7329 0a40 6d6f 636b 2e70  records).@mock.p
+00012b90: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
+00012ba0: 6765 722e 636c 6965 6e74 2e5f 6465 6661  ger.client._defa
+00012bb0: 756c 745f 6a6f 696e 5f6b 6579 5f67 656e  ult_join_key_gen
+00012bc0: 2229 0a64 6566 2074 6573 745f 6c6f 675f  ").def test_log_
+00012bd0: 7265 636f 7264 735f 7072 6564 735f 6f6e  records_preds_on
+00012be0: 6c79 280a 2020 2020 6d6f 636b 5f6a 6f69  ly(.    mock_joi
+00012bf0: 6e5f 6b65 795f 6765 6e2c 0a20 2020 206d  n_key_gen,.    m
+00012c00: 6f63 6b5f 7361 6d70 6c65 5f72 6563 6f72  ock_sample_recor
+00012c10: 6473 2c0a 2020 2020 6d6f 636b 5f66 6565  ds,.    mock_fee
+00012c20: 6462 6163 6b2c 0a20 2020 206d 6f63 6b5f  dback,.    mock_
+00012c30: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
+00012c40: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+00012c50: 636b 2c0a 2020 2020 6d6f 636b 5f72 6573  ck,.    mock_res
+00012c60: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2c0a  olve_join_keys,.
+00012c70: 2020 2020 7665 7273 696f 6e2c 0a20 2020      version,.   
+00012c80: 2074 6167 732c 0a20 2020 2072 6f77 5f74   tags,.    row_t
+00012c90: 6167 732c 0a20 2020 2067 6c6f 6261 6c5f  ags,.    global_
+00012ca0: 7461 6773 2c0a 2020 2020 6578 7065 6374  tags,.    expect
+00012cb0: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
+00012cc0: 2020 2074 6573 745f 7469 6d65 7374 616d     test_timestam
+00012cd0: 7073 2c0a 2020 2020 7465 7374 5f74 696d  ps,.    test_tim
+00012ce0: 6573 7461 6d70 735f 6c69 7374 2c0a 2020  estamps_list,.  
+00012cf0: 2020 7465 7374 5f69 6e70 7574 732c 0a20    test_inputs,. 
+00012d00: 2020 2074 6573 745f 6f75 7470 7574 732c     test_outputs,
+00012d10: 0a20 2020 206b 7761 7267 732c 0a20 2020  .    kwargs,.   
+00012d20: 2063 6c69 5f6f 626a 2c0a 293a 0a20 2020   cli_obj,.):.   
+00012d30: 206d 6f63 6b5f 6a6f 696e 5f6b 6579 5f67   mock_join_key_g
+00012d40: 656e 2e73 6964 655f 6566 6665 6374 203d  en.side_effect =
+00012d50: 205b 2236 3738 3930 222c 2022 3132 3334   ["67890", "1234
+00012d60: 3522 5d0a 2020 2020 6d6f 636b 5f72 6573  5"].    mock_res
+00012d70: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2e72  olve_join_keys.r
+00012d80: 6574 7572 6e5f 7661 6c75 6520 3d20 5b22  eturn_value = ["
+00012d90: 3132 3334 3522 2c20 2236 3738 3930 225d  12345", "67890"]
+00012da0: 2069 6620 6b77 6172 6773 2065 6c73 6520   if kwargs else 
+00012db0: 4e6f 6e65 0a20 2020 2061 7373 6572 7420  None.    assert 
+00012dc0: 636c 695f 6f62 6a2e 6c6f 675f 7265 636f  cli_obj.log_reco
+00012dd0: 7264 7328 0a20 2020 2020 2020 2061 7070  rds(.        app
+00012de0: 6c69 6361 7469 6f6e 3d22 666f 6f62 6172  lication="foobar
+00012df0: 222c 0a20 2020 2020 2020 2076 6572 7369  ",.        versi
+00012e00: 6f6e 3d76 6572 7369 6f6e 2c0a 2020 2020  on=version,.    
+00012e10: 2020 2020 696e 7075 7473 3d74 6573 745f      inputs=test_
+00012e20: 696e 7075 7473 2c0a 2020 2020 2020 2020  inputs,.        
+00012e30: 6f75 7470 7574 733d 7465 7374 5f6f 7574  outputs=test_out
+00012e40: 7075 7473 2c0a 2020 2020 2020 2020 6665  puts,.        fe
+00012e50: 6564 6261 636b 733d 4e6f 6e65 2c0a 2020  edbacks=None,.  
+00012e60: 2020 2020 2020 7469 6d65 7374 616d 7073        timestamps
+00012e70: 3d74 6573 745f 7469 6d65 7374 616d 7073  =test_timestamps
+00012e80: 2c0a 2020 2020 2020 2020 736f 7274 5f6f  ,.        sort_o
+00012e90: 6e5f 7469 6d65 7374 616d 703d 5472 7565  n_timestamp=True
+00012ea0: 2c0a 2020 2020 2020 2020 7461 6773 3d74  ,.        tags=t
+00012eb0: 6167 732c 0a20 2020 2020 2020 2072 6f77  ags,.        row
+00012ec0: 5f74 6167 733d 726f 775f 7461 6773 2c0a  _tags=row_tags,.
+00012ed0: 2020 2020 2020 2020 676c 6f62 616c 5f74          global_t
+00012ee0: 6167 733d 676c 6f62 616c 5f74 6167 732c  ags=global_tags,
+00012ef0: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
+00012f00: 732c 0a20 2020 2029 203d 3d20 284e 6f6e  s,.    ) == (Non
+00012f10: 652c 205b 2231 3233 3435 222c 2022 3637  e, ["12345", "67
+00012f20: 3839 3022 5d29 0a0a 2020 2020 6d6f 636b  890"])..    mock
+00012f30: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
+00012f40: 6163 6b2e 6173 7365 7274 5f6e 6f74 5f63  ack.assert_not_c
+00012f50: 616c 6c65 6428 290a 2020 2020 6d6f 636b  alled().    mock
+00012f60: 5f70 7265 6473 2e61 7373 6572 745f 6361  _preds.assert_ca
+00012f70: 6c6c 6564 5f6f 6e63 655f 7769 7468 280a  lled_once_with(.
+00012f80: 2020 2020 2020 2020 6170 706c 6963 6174          applicat
+00012f90: 696f 6e3d 2266 6f6f 6261 7222 2c0a 2020  ion="foobar",.  
+00012fa0: 2020 2020 2020 696e 7075 7473 3d5b 7b22        inputs=[{"
+00012fb0: 4122 3a20 3130 307d 2c20 7b22 4122 3a20  A": 100}, {"A": 
+00012fc0: 3130 317d 5d2c 0a20 2020 2020 2020 206f  101}],.        o
+00012fd0: 7574 7075 7473 3d5b 7b22 4222 3a20 3330  utputs=[{"B": 30
+00012fe0: 307d 2c20 7b22 4222 3a20 3330 317d 5d2c  0}, {"B": 301}],
+00012ff0: 0a20 2020 2020 2020 206a 6f69 6e5f 6b65  .        join_ke
+00013000: 7973 3d5b 2231 3233 3435 222c 2022 3637  ys=["12345", "67
+00013010: 3839 3022 5d20 6966 206b 7761 7267 7320  890"] if kwargs 
+00013020: 656c 7365 205b 2236 3738 3930 222c 2022  else ["67890", "
+00013030: 3132 3334 3522 5d2c 0a20 2020 2020 2020  12345"],.       
+00013040: 2076 6572 7369 6f6e 3d76 6572 7369 6f6e   version=version
+00013050: 2c0a 2020 2020 2020 2020 6967 6e6f 7265  ,.        ignore
+00013060: 5f69 6e70 7574 733d 4e6f 6e65 2c0a 2020  _inputs=None,.  
+00013070: 2020 2020 2020 7469 6d65 7374 616d 7073        timestamps
+00013080: 3d74 6573 745f 7469 6d65 7374 616d 7073  =test_timestamps
+00013090: 5f6c 6973 742c 0a20 2020 2020 2020 2073  _list,.        s
+000130a0: 6f72 745f 6f6e 5f74 696d 6573 7461 6d70  ort_on_timestamp
+000130b0: 3d54 7275 652c 0a20 2020 2020 2020 2061  =True,.        a
+000130c0: 735f 6261 7463 683d 4661 6c73 652c 0a20  s_batch=False,. 
+000130d0: 2020 2020 2020 2074 6167 733d 6578 7065         tags=expe
+000130e0: 6374 6564 5f74 6167 735f 7061 7261 6d2c  cted_tags_param,
+000130f0: 0a20 2020 2029 0a20 2020 206d 6f63 6b5f  .    ).    mock_
+00013100: 6665 6564 6261 636b 2e61 7373 6572 745f  feedback.assert_
+00013110: 6e6f 745f 6361 6c6c 6564 2829 0a0a 2020  not_called()..  
+00013120: 2020 6d6f 636b 5f73 616d 706c 655f 7265    mock_sample_re
+00013130: 636f 7264 732e 6173 7365 7274 5f63 616c  cords.assert_cal
+00013140: 6c65 645f 6f6e 6365 5f77 6974 6828 0a20  led_once_with(. 
+00013150: 2020 2020 2020 2032 2c0a 2020 2020 2020         2,.      
+00013160: 2020 312c 0a20 2020 2020 2020 205b 7b22    1,.        [{"
+00013170: 4122 3a20 3130 307d 2c20 7b22 4122 3a20  A": 100}, {"A": 
+00013180: 3130 317d 5d2c 0a20 2020 2020 2020 205b  101}],.        [
+00013190: 7b22 4222 3a20 3330 307d 2c20 7b22 4222  {"B": 300}, {"B"
+000131a0: 3a20 3330 317d 5d2c 0a20 2020 2020 2020  : 301}],.       
+000131b0: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
+000131c0: 6c69 656e 742e 5f72 6573 6f6c 7665 5f6a  lient._resolve_j
+000131d0: 6f69 6e5f 6b65 7973 282a 2a6b 7761 7267  oin_keys(**kwarg
+000131e0: 7329 2c0a 2020 2020 2020 2020 7465 7374  s),.        test
+000131f0: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
+00013200: 2c0a 2020 2020 2020 2020 6578 7065 6374  ,.        expect
+00013210: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
+00013220: 2020 2029 0a0a 2020 2020 6966 206b 7761     )..    if kwa
+00013230: 7267 733a 0a20 2020 2020 2020 206d 6f63  rgs:.        moc
+00013240: 6b5f 6a6f 696e 5f6b 6579 5f67 656e 2e61  k_join_key_gen.a
+00013250: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
+00013260: 2829 0a20 2020 2065 6c73 653a 0a20 2020  ().    else:.   
+00013270: 2020 2020 206d 6f63 6b5f 6a6f 696e 5f6b       mock_join_k
+00013280: 6579 5f67 656e 2e61 7373 6572 745f 6361  ey_gen.assert_ca
+00013290: 6c6c 6564 2829 0a0a 0a40 7079 7465 7374  lled()...@pytest
+000132a0: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+000132b0: 6528 0a20 2020 2022 7465 7374 5f74 696d  e(.    "test_tim
+000132c0: 6573 7461 6d70 732c 2074 6573 745f 7469  estamps, test_ti
+000132d0: 6d65 7374 616d 7073 5f6c 6973 7422 2c0a  mestamps_list",.
+000132e0: 2020 2020 5b0a 2020 2020 2020 2020 284e      [.        (N
+000132f0: 6f6e 652c 204e 6f6e 6529 2c0a 2020 2020  one, None),.    
+00013300: 2020 2020 285b 4355 5252 454e 545f 5449      ([CURRENT_TI
+00013310: 4d45 5d20 2a20 322c 205b 4355 5252 454e  ME] * 2, [CURREN
+00013320: 545f 5449 4d45 5d20 2a20 3229 2c0a 2020  T_TIME] * 2),.  
+00013330: 2020 2020 2020 286e 702e 6172 7261 7928        (np.array(
+00013340: 5b43 5552 5245 4e54 5f54 494d 455d 202a  [CURRENT_TIME] *
+00013350: 2032 292c 205b 4355 5252 454e 545f 5449   2), [CURRENT_TI
+00013360: 4d45 5d20 2a20 3229 2c0a 2020 2020 5d2c  ME] * 2),.    ],
+00013370: 0a29 0a40 7079 7465 7374 2e6d 6172 6b2e  .).@pytest.mark.
+00013380: 7061 7261 6d65 7472 697a 6528 0a20 2020  parametrize(.   
+00013390: 2022 6b77 6172 6773 222c 0a20 2020 205b   "kwargs",.    [
+000133a0: 0a20 2020 2020 2020 207b 2266 6565 6462  .        {"feedb
+000133b0: 6163 6b5f 6b65 7973 223a 205b 2241 225d  ack_keys": ["A"]
+000133c0: 7d2c 0a20 2020 2020 2020 207b 2266 6565  },.        {"fee
+000133d0: 6462 6163 6b5f 6964 7322 3a20 5b22 3132  dback_ids": ["12
+000133e0: 3334 3522 2c20 2236 3738 3930 225d 7d2c  345", "67890"]},
+000133f0: 0a20 2020 2020 2020 207b 226a 6f69 6e5f  .        {"join_
+00013400: 6b65 7973 223a 205b 2235 3433 3231 222c  keys": ["54321",
+00013410: 2022 3637 3839 3022 5d7d 2c0a 2020 2020   "67890"]},.    
+00013420: 2020 2020 7b22 6a6f 696e 5f6b 6579 7322      {"join_keys"
+00013430: 3a20 7064 2e53 6572 6965 7328 5b22 3534  : pd.Series(["54
+00013440: 3332 3122 2c20 2236 3738 3930 225d 297d  321", "67890"])}
+00013450: 2c0a 2020 2020 2020 2020 7b7d 2c0a 2020  ,.        {},.  
+00013460: 2020 5d2c 0a29 0a40 7079 7465 7374 2e6d    ],.).@pytest.m
+00013470: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00013480: 0a20 2020 2028 2274 6573 745f 6f75 7470  .    ("test_outp
+00013490: 7574 7322 2c20 2274 6573 745f 696e 7075  uts", "test_inpu
+000134a0: 7473 2229 2c0a 2020 2020 6c69 7374 287a  ts"),.    list(z
+000134b0: 6970 2854 4553 545f 4f55 5450 5554 532c  ip(TEST_OUTPUTS,
+000134c0: 2054 4553 545f 494e 5055 5453 2929 2c0a   TEST_INPUTS)),.
+000134d0: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
+000134e0: 6172 616d 6574 7269 7a65 2822 7665 7273  arametrize("vers
+000134f0: 696f 6e22 2c20 5b4e 6f6e 652c 2031 302c  ion", [None, 10,
+00013500: 2022 312e 322e 3322 5d29 0a40 7079 7465   "1.2.3"]).@pyte
+00013510: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
+00013520: 697a 6528 2274 6167 732c 2072 6f77 5f74  ize("tags, row_t
+00013530: 6167 732c 2067 6c6f 6261 6c5f 7461 6773  ags, global_tags
+00013540: 2c20 6578 7065 6374 6564 5f74 6167 735f  , expected_tags_
+00013550: 7061 7261 6d22 2c20 5445 5354 5f54 4147  param", TEST_TAG
+00013560: 5329 0a40 6d6f 636b 2e70 6174 6368 2822  S).@mock.patch("
+00013570: 6761 6e74 7279 2e6c 6f67 6765 722e 636c  gantry.logger.cl
+00013580: 6965 6e74 2e5f 7265 736f 6c76 655f 6a6f  ient._resolve_jo
+00013590: 696e 5f6b 6579 7322 290a 406d 6f63 6b2e  in_keys").@mock.
+000135a0: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+000135b0: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
+000135c0: 7279 2e5f 6c6f 675f 7072 6564 6963 7469  ry._log_predicti
+000135d0: 6f6e 5f61 6e64 5f66 6565 6462 6163 6b5f  on_and_feedback_
+000135e0: 6576 656e 7473 2229 0a40 6d6f 636b 2e70  events").@mock.p
+000135f0: 6174 6368 280a 2020 2020 2267 616e 7472  atch(.    "gantr
+00013600: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+00013610: 4761 6e74 7279 2e5f 6c6f 675f 7072 6564  Gantry._log_pred
+00013620: 6963 7469 6f6e 5f65 7665 6e74 7322 2c20  iction_events", 
+00013630: 7265 7475 726e 5f76 616c 7565 3d28 4e6f  return_value=(No
+00013640: 6e65 2c20 5b22 3132 3334 3522 2c20 2236  ne, ["12345", "6
+00013650: 3738 3930 225d 290a 290a 406d 6f63 6b2e  7890"]).).@mock.
+00013660: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+00013670: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
+00013680: 7279 2e5f 6c6f 675f 6665 6564 6261 636b  ry._log_feedback
+00013690: 5f65 7665 6e74 7322 290a 406d 6f63 6b2e  _events").@mock.
 000136a0: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-000136b0: 6767 6572 2e63 6c69 656e 742e 5f64 6566  gger.client._def
-000136c0: 6175 6c74 5f6a 6f69 6e5f 6b65 795f 6765  ault_join_key_ge
-000136d0: 6e22 290a 6465 6620 7465 7374 5f73 696e  n").def test_sin
-000136e0: 676c 655f 6c6f 675f 7265 636f 7264 735f  gle_log_records_
-000136f0: 7072 6564 735f 6f6e 6c79 280a 2020 2020  preds_only(.    
-00013700: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
-00013710: 6e2c 0a20 2020 206d 6f63 6b5f 7361 6d70  n,.    mock_samp
-00013720: 6c65 5f72 6563 6f72 6473 2c0a 2020 2020  le_records,.    
-00013730: 6d6f 636b 5f66 6565 6462 6163 6b2c 0a20  mock_feedback,. 
-00013740: 2020 206d 6f63 6b5f 7072 6564 732c 0a20     mock_preds,. 
-00013750: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
-00013760: 645f 6665 6564 6261 636b 2c0a 2020 2020  d_feedback,.    
-00013770: 6d6f 636b 5f72 6573 6f6c 7665 5f6a 6f69  mock_resolve_joi
-00013780: 6e5f 6b65 7973 2c0a 2020 2020 7665 7273  n_keys,.    vers
-00013790: 696f 6e2c 0a20 2020 2074 6167 732c 0a20  ion,.    tags,. 
-000137a0: 2020 2072 6f77 5f74 6167 732c 0a20 2020     row_tags,.   
-000137b0: 2067 6c6f 6261 6c5f 7461 6773 2c0a 2020   global_tags,.  
-000137c0: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
-000137d0: 7061 7261 6d2c 0a20 2020 2074 6573 745f  param,.    test_
-000137e0: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
-000137f0: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
-00013800: 6c69 7374 2c0a 2020 2020 7465 7374 5f69  list,.    test_i
-00013810: 6e70 7574 732c 0a20 2020 2074 6573 745f  nputs,.    test_
-00013820: 6f75 7470 7574 732c 0a20 2020 206b 7761  outputs,.    kwa
-00013830: 7267 732c 0a20 2020 2063 6c69 5f6f 626a  rgs,.    cli_obj
-00013840: 2c0a 293a 0a20 2020 206d 6f63 6b5f 6a6f  ,.):.    mock_jo
-00013850: 696e 5f6b 6579 5f67 656e 2e73 6964 655f  in_key_gen.side_
-00013860: 6566 6665 6374 203d 205b 2236 3738 3930  effect = ["67890
-00013870: 222c 2022 3132 3334 3522 5d0a 2020 2020  ", "12345"].    
-00013880: 6d6f 636b 5f72 6573 6f6c 7665 5f6a 6f69  mock_resolve_joi
-00013890: 6e5f 6b65 7973 2e72 6574 7572 6e5f 7661  n_keys.return_va
-000138a0: 6c75 6520 3d20 5b22 3132 3334 3522 2c20  lue = ["12345", 
-000138b0: 2236 3738 3930 225d 2069 6620 6b77 6172  "67890"] if kwar
-000138c0: 6773 2065 6c73 6520 4e6f 6e65 0a20 2020  gs else None.   
-000138d0: 2061 7373 6572 7420 636c 695f 6f62 6a2e   assert cli_obj.
-000138e0: 7369 6e67 6c65 5f6c 6f67 5f72 6563 6f72  single_log_recor
-000138f0: 6473 280a 2020 2020 2020 2020 6170 706c  ds(.        appl
-00013900: 6963 6174 696f 6e3d 2266 6f6f 6261 7222  ication="foobar"
-00013910: 2c0a 2020 2020 2020 2020 7665 7273 696f  ,.        versio
-00013920: 6e3d 7665 7273 696f 6e2c 0a20 2020 2020  n=version,.     
-00013930: 2020 2069 6e70 7574 733d 7465 7374 5f69     inputs=test_i
-00013940: 6e70 7574 732c 0a20 2020 2020 2020 206f  nputs,.        o
-00013950: 7574 7075 7473 3d74 6573 745f 6f75 7470  utputs=test_outp
-00013960: 7574 732c 0a20 2020 2020 2020 2066 6565  uts,.        fee
-00013970: 6462 6163 6b73 3d4e 6f6e 652c 0a20 2020  dbacks=None,.   
-00013980: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
-00013990: 7465 7374 5f74 696d 6573 7461 6d70 732c  test_timestamps,
-000139a0: 0a20 2020 2020 2020 2073 6f72 745f 6f6e  .        sort_on
-000139b0: 5f74 696d 6573 7461 6d70 3d54 7275 652c  _timestamp=True,
-000139c0: 0a20 2020 2020 2020 2074 6167 733d 7461  .        tags=ta
-000139d0: 6773 2c0a 2020 2020 2020 2020 726f 775f  gs,.        row_
-000139e0: 7461 6773 3d72 6f77 5f74 6167 732c 0a20  tags=row_tags,. 
-000139f0: 2020 2020 2020 2067 6c6f 6261 6c5f 7461         global_ta
-00013a00: 6773 3d67 6c6f 6261 6c5f 7461 6773 2c0a  gs=global_tags,.
-00013a10: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00013a20: 2c0a 2020 2020 2920 3d3d 2028 4e6f 6e65  ,.    ) == (None
-00013a30: 2c20 5b22 3132 3334 3522 2c20 2236 3738  , ["12345", "678
-00013a40: 3930 225d 290a 0a20 2020 206d 6f63 6b5f  90"])..    mock_
-00013a50: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-00013a60: 636b 2e61 7373 6572 745f 6e6f 745f 6361  ck.assert_not_ca
-00013a70: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
-00013a80: 7072 6564 732e 6173 7365 7274 5f63 616c  preds.assert_cal
-00013a90: 6c65 645f 6f6e 6365 5f77 6974 6828 0a20  led_once_with(. 
-00013aa0: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
-00013ab0: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
-00013ac0: 2020 2020 2069 6e70 7574 733d 5b7b 2241       inputs=[{"A
-00013ad0: 223a 2031 3030 7d2c 207b 2241 223a 2031  ": 100}, {"A": 1
-00013ae0: 3031 7d5d 2c0a 2020 2020 2020 2020 6f75  01}],.        ou
-00013af0: 7470 7574 733d 5b7b 2242 223a 2033 3030  tputs=[{"B": 300
-00013b00: 7d2c 207b 2242 223a 2033 3031 7d5d 2c0a  }, {"B": 301}],.
-00013b10: 2020 2020 2020 2020 6a6f 696e 5f6b 6579          join_key
-00013b20: 733d 5b22 3132 3334 3522 2c20 2236 3738  s=["12345", "678
-00013b30: 3930 225d 2069 6620 6b77 6172 6773 2065  90"] if kwargs e
-00013b40: 6c73 6520 5b22 3637 3839 3022 2c20 2231  lse ["67890", "1
-00013b50: 3233 3435 225d 2c0a 2020 2020 2020 2020  2345"],.        
-00013b60: 7665 7273 696f 6e3d 7665 7273 696f 6e2c  version=version,
-00013b70: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
-00013b80: 696e 7075 7473 3d4e 6f6e 652c 0a20 2020  inputs=None,.   
-00013b90: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
-00013ba0: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
-00013bb0: 6c69 7374 2c0a 2020 2020 2020 2020 736f  list,.        so
-00013bc0: 7274 5f6f 6e5f 7469 6d65 7374 616d 703d  rt_on_timestamp=
-00013bd0: 5472 7565 2c0a 2020 2020 2020 2020 6173  True,.        as
-00013be0: 5f62 6174 6368 3d46 616c 7365 2c0a 2020  _batch=False,.  
-00013bf0: 2020 2020 2020 7461 6773 3d65 7870 6563        tags=expec
-00013c00: 7465 645f 7461 6773 5f70 6172 616d 2c0a  ted_tags_param,.
-00013c10: 2020 2020 290a 2020 2020 6d6f 636b 5f66      ).    mock_f
-00013c20: 6565 6462 6163 6b2e 6173 7365 7274 5f6e  eedback.assert_n
-00013c30: 6f74 5f63 616c 6c65 6428 290a 0a20 2020  ot_called()..   
-00013c40: 206d 6f63 6b5f 7361 6d70 6c65 5f72 6563   mock_sample_rec
-00013c50: 6f72 6473 2e61 7373 6572 745f 6361 6c6c  ords.assert_call
-00013c60: 6564 5f6f 6e63 655f 7769 7468 280a 2020  ed_once_with(.  
-00013c70: 2020 2020 2020 322c 0a20 2020 2020 2020        2,.       
-00013c80: 2031 2c0a 2020 2020 2020 2020 5b7b 2241   1,.        [{"A
-00013c90: 223a 2031 3030 7d2c 207b 2241 223a 2031  ": 100}, {"A": 1
-00013ca0: 3031 7d5d 2c0a 2020 2020 2020 2020 5b7b  01}],.        [{
-00013cb0: 2242 223a 2033 3030 7d2c 207b 2242 223a  "B": 300}, {"B":
-00013cc0: 2033 3031 7d5d 2c0a 2020 2020 2020 2020   301}],.        
-00013cd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 636c  None,.        cl
-00013ce0: 6965 6e74 2e5f 7265 736f 6c76 655f 6a6f  ient._resolve_jo
-00013cf0: 696e 5f6b 6579 7328 2a2a 6b77 6172 6773  in_keys(**kwargs
-00013d00: 292c 0a20 2020 2020 2020 2074 6573 745f  ),.        test_
-00013d10: 7469 6d65 7374 616d 7073 5f6c 6973 742c  timestamps_list,
-00013d20: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-00013d30: 645f 7461 6773 5f70 6172 616d 2c0a 2020  d_tags_param,.  
-00013d40: 2020 290a 0a20 2020 2069 6620 6b77 6172    )..    if kwar
-00013d50: 6773 3a0a 2020 2020 2020 2020 6d6f 636b  gs:.        mock
-00013d60: 5f6a 6f69 6e5f 6b65 795f 6765 6e2e 6173  _join_key_gen.as
-00013d70: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
-00013d80: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00013d90: 2020 2020 6d6f 636b 5f6a 6f69 6e5f 6b65      mock_join_ke
-00013da0: 795f 6765 6e2e 6173 7365 7274 5f63 616c  y_gen.assert_cal
-00013db0: 6c65 6428 290a 0a0a 4070 7974 6573 742e  led()...@pytest.
-00013dc0: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-00013dd0: 280a 2020 2020 2274 6573 745f 7469 6d65  (.    "test_time
-00013de0: 7374 616d 7073 2c20 7465 7374 5f74 696d  stamps, test_tim
-00013df0: 6573 7461 6d70 735f 6c69 7374 222c 0a20  estamps_list",. 
-00013e00: 2020 205b 0a20 2020 2020 2020 2028 4e6f     [.        (No
-00013e10: 6e65 2c20 4e6f 6e65 292c 0a20 2020 2020  ne, None),.     
-00013e20: 2020 2028 5b43 5552 5245 4e54 5f54 494d     ([CURRENT_TIM
-00013e30: 455d 202a 2032 2c20 5b43 5552 5245 4e54  E] * 2, [CURRENT
-00013e40: 5f54 494d 455d 202a 2032 292c 0a20 2020  _TIME] * 2),.   
-00013e50: 2020 2020 2028 6e70 2e61 7272 6179 285b       (np.array([
-00013e60: 4355 5252 454e 545f 5449 4d45 5d20 2a20  CURRENT_TIME] * 
-00013e70: 3229 2c20 5b43 5552 5245 4e54 5f54 494d  2), [CURRENT_TIM
-00013e80: 455d 202a 2032 292c 0a20 2020 205d 2c0a  E] * 2),.    ],.
-00013e90: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
-00013ea0: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
-00013eb0: 226b 7761 7267 7322 2c0a 2020 2020 5b0a  "kwargs",.    [.
-00013ec0: 2020 2020 2020 2020 7b22 6a6f 696e 5f6b          {"join_k
-00013ed0: 6579 7322 3a20 5b22 3534 3332 3122 2c20  eys": ["54321", 
-00013ee0: 2236 3738 3930 225d 7d2c 0a20 2020 2020  "67890"]},.     
-00013ef0: 2020 207b 226a 6f69 6e5f 6b65 7973 223a     {"join_keys":
-00013f00: 2070 642e 5365 7269 6573 285b 2235 3433   pd.Series(["543
-00013f10: 3231 222c 2022 3637 3839 3022 5d29 7d2c  21", "67890"])},
-00013f20: 0a20 2020 2020 2020 207b 7d2c 0a20 2020  .        {},.   
-00013f30: 205d 2c0a 290a 4070 7974 6573 742e 6d61   ],.).@pytest.ma
-00013f40: 726b 2e70 6172 616d 6574 7269 7a65 280a  rk.parametrize(.
-00013f50: 2020 2020 2822 7465 7374 5f6f 7574 7075      ("test_outpu
-00013f60: 7473 222c 2022 7465 7374 5f69 6e70 7574  ts", "test_input
-00013f70: 7322 292c 0a20 2020 206c 6973 7428 7a69  s"),.    list(zi
-00013f80: 7028 5445 5354 5f4f 5554 5055 5453 2c20  p(TEST_OUTPUTS, 
-00013f90: 5445 5354 5f49 4e50 5554 5329 292c 0a29  TEST_INPUTS)),.)
-00013fa0: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
-00013fb0: 7261 6d65 7472 697a 6528 2276 6572 7369  rametrize("versi
-00013fc0: 6f6e 222c 205b 4e6f 6e65 2c20 3130 2c20  on", [None, 10, 
-00013fd0: 2231 2e32 2e33 225d 290a 4070 7974 6573  "1.2.3"]).@pytes
-00013fe0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00013ff0: 7a65 2822 7461 6773 2c20 726f 775f 7461  ze("tags, row_ta
-00014000: 6773 2c20 676c 6f62 616c 5f74 6167 732c  gs, global_tags,
-00014010: 2065 7870 6563 7465 645f 7461 6773 5f70   expected_tags_p
-00014020: 6172 616d 222c 2054 4553 545f 5441 4753  aram", TEST_TAGS
-00014030: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-00014040: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00014050: 656e 742e 5f72 6573 6f6c 7665 5f6a 6f69  ent._resolve_joi
-00014060: 6e5f 6b65 7973 2229 0a40 6d6f 636b 2e70  n_keys").@mock.p
-00014070: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
-00014080: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-00014090: 792e 5f67 656e 6572 6174 655f 7072 6564  y._generate_pred
-000140a0: 6963 7469 6f6e 5f61 6e64 5f66 6565 6462  iction_and_feedb
-000140b0: 6163 6b5f 6576 656e 7473 2229 0a40 6d6f  ack_events").@mo
-000140c0: 636b 2e70 6174 6368 280a 2020 2020 2267  ck.patch(.    "g
-000140d0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-000140e0: 656e 742e 4761 6e74 7279 2e5f 6765 6e65  ent.Gantry._gene
-000140f0: 7261 7465 5f70 7265 6469 6374 696f 6e5f  rate_prediction_
-00014100: 6576 656e 7473 222c 0a20 2020 2072 6574  events",.    ret
-00014110: 7572 6e5f 7661 6c75 653d 285b 7b22 6576  urn_value=([{"ev
-00014120: 656e 7422 3a20 2270 6c61 6365 5f68 6f6c  ent": "place_hol
-00014130: 6465 7222 7d5d 2c20 5b22 3132 3334 3522  der"}], ["12345"
-00014140: 2c20 2236 3738 3930 225d 292c 0a29 0a40  , "67890"]),.).@
-00014150: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
-00014160: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
-00014170: 2e47 616e 7472 792e 5f67 656e 6572 6174  .Gantry._generat
-00014180: 655f 6665 6564 6261 636b 5f65 7665 6e74  e_feedback_event
-00014190: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
-000141a0: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
-000141b0: 6c69 656e 742e 5f73 616d 706c 655f 7265  lient._sample_re
-000141c0: 636f 7264 7322 2c20 7369 6465 5f65 6666  cords", side_eff
-000141d0: 6563 743d 636c 6965 6e74 2e5f 7361 6d70  ect=client._samp
-000141e0: 6c65 5f72 6563 6f72 6473 290a 406d 6f63  le_records).@moc
+000136b0: 6767 6572 2e63 6c69 656e 742e 5f73 616d  gger.client._sam
+000136c0: 706c 655f 7265 636f 7264 7322 2c20 7369  ple_records", si
+000136d0: 6465 5f65 6666 6563 743d 636c 6965 6e74  de_effect=client
+000136e0: 2e5f 7361 6d70 6c65 5f72 6563 6f72 6473  ._sample_records
+000136f0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+00013700: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+00013710: 656e 742e 5f64 6566 6175 6c74 5f6a 6f69  ent._default_joi
+00013720: 6e5f 6b65 795f 6765 6e22 290a 6465 6620  n_key_gen").def 
+00013730: 7465 7374 5f73 696e 676c 655f 6c6f 675f  test_single_log_
+00013740: 7265 636f 7264 735f 7072 6564 735f 6f6e  records_preds_on
+00013750: 6c79 280a 2020 2020 6d6f 636b 5f6a 6f69  ly(.    mock_joi
+00013760: 6e5f 6b65 795f 6765 6e2c 0a20 2020 206d  n_key_gen,.    m
+00013770: 6f63 6b5f 7361 6d70 6c65 5f72 6563 6f72  ock_sample_recor
+00013780: 6473 2c0a 2020 2020 6d6f 636b 5f66 6565  ds,.    mock_fee
+00013790: 6462 6163 6b2c 0a20 2020 206d 6f63 6b5f  dback,.    mock_
+000137a0: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
+000137b0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+000137c0: 636b 2c0a 2020 2020 6d6f 636b 5f72 6573  ck,.    mock_res
+000137d0: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2c0a  olve_join_keys,.
+000137e0: 2020 2020 7665 7273 696f 6e2c 0a20 2020      version,.   
+000137f0: 2074 6167 732c 0a20 2020 2072 6f77 5f74   tags,.    row_t
+00013800: 6167 732c 0a20 2020 2067 6c6f 6261 6c5f  ags,.    global_
+00013810: 7461 6773 2c0a 2020 2020 6578 7065 6374  tags,.    expect
+00013820: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
+00013830: 2020 2074 6573 745f 7469 6d65 7374 616d     test_timestam
+00013840: 7073 2c0a 2020 2020 7465 7374 5f74 696d  ps,.    test_tim
+00013850: 6573 7461 6d70 735f 6c69 7374 2c0a 2020  estamps_list,.  
+00013860: 2020 7465 7374 5f69 6e70 7574 732c 0a20    test_inputs,. 
+00013870: 2020 2074 6573 745f 6f75 7470 7574 732c     test_outputs,
+00013880: 0a20 2020 206b 7761 7267 732c 0a20 2020  .    kwargs,.   
+00013890: 2063 6c69 5f6f 626a 2c0a 293a 0a20 2020   cli_obj,.):.   
+000138a0: 206d 6f63 6b5f 6a6f 696e 5f6b 6579 5f67   mock_join_key_g
+000138b0: 656e 2e73 6964 655f 6566 6665 6374 203d  en.side_effect =
+000138c0: 205b 2236 3738 3930 222c 2022 3132 3334   ["67890", "1234
+000138d0: 3522 5d0a 2020 2020 6d6f 636b 5f72 6573  5"].    mock_res
+000138e0: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2e72  olve_join_keys.r
+000138f0: 6574 7572 6e5f 7661 6c75 6520 3d20 5b22  eturn_value = ["
+00013900: 3132 3334 3522 2c20 2236 3738 3930 225d  12345", "67890"]
+00013910: 2069 6620 6b77 6172 6773 2065 6c73 6520   if kwargs else 
+00013920: 4e6f 6e65 0a20 2020 2061 7373 6572 7420  None.    assert 
+00013930: 636c 695f 6f62 6a2e 7369 6e67 6c65 5f6c  cli_obj.single_l
+00013940: 6f67 5f72 6563 6f72 6473 280a 2020 2020  og_records(.    
+00013950: 2020 2020 6170 706c 6963 6174 696f 6e3d      application=
+00013960: 2266 6f6f 6261 7222 2c0a 2020 2020 2020  "foobar",.      
+00013970: 2020 7665 7273 696f 6e3d 7665 7273 696f    version=versio
+00013980: 6e2c 0a20 2020 2020 2020 2069 6e70 7574  n,.        input
+00013990: 733d 7465 7374 5f69 6e70 7574 732c 0a20  s=test_inputs,. 
+000139a0: 2020 2020 2020 206f 7574 7075 7473 3d74         outputs=t
+000139b0: 6573 745f 6f75 7470 7574 732c 0a20 2020  est_outputs,.   
+000139c0: 2020 2020 2066 6565 6462 6163 6b73 3d4e       feedbacks=N
+000139d0: 6f6e 652c 0a20 2020 2020 2020 2074 696d  one,.        tim
+000139e0: 6573 7461 6d70 733d 7465 7374 5f74 696d  estamps=test_tim
+000139f0: 6573 7461 6d70 732c 0a20 2020 2020 2020  estamps,.       
+00013a00: 2073 6f72 745f 6f6e 5f74 696d 6573 7461   sort_on_timesta
+00013a10: 6d70 3d54 7275 652c 0a20 2020 2020 2020  mp=True,.       
+00013a20: 2074 6167 733d 7461 6773 2c0a 2020 2020   tags=tags,.    
+00013a30: 2020 2020 726f 775f 7461 6773 3d72 6f77      row_tags=row
+00013a40: 5f74 6167 732c 0a20 2020 2020 2020 2067  _tags,.        g
+00013a50: 6c6f 6261 6c5f 7461 6773 3d67 6c6f 6261  lobal_tags=globa
+00013a60: 6c5f 7461 6773 2c0a 2020 2020 2020 2020  l_tags,.        
+00013a70: 2a2a 6b77 6172 6773 2c0a 2020 2020 2920  **kwargs,.    ) 
+00013a80: 3d3d 2028 4e6f 6e65 2c20 5b22 3132 3334  == (None, ["1234
+00013a90: 3522 2c20 2236 3738 3930 225d 290a 0a20  5", "67890"]).. 
+00013aa0: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
+00013ab0: 645f 6665 6564 6261 636b 2e61 7373 6572  d_feedback.asser
+00013ac0: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
+00013ad0: 2020 206d 6f63 6b5f 7072 6564 732e 6173     mock_preds.as
+00013ae0: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+00013af0: 5f77 6974 6828 0a20 2020 2020 2020 2061  _with(.        a
+00013b00: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
+00013b10: 6172 222c 0a20 2020 2020 2020 2069 6e70  ar",.        inp
+00013b20: 7574 733d 5b7b 2241 223a 2031 3030 7d2c  uts=[{"A": 100},
+00013b30: 207b 2241 223a 2031 3031 7d5d 2c0a 2020   {"A": 101}],.  
+00013b40: 2020 2020 2020 6f75 7470 7574 733d 5b7b        outputs=[{
+00013b50: 2242 223a 2033 3030 7d2c 207b 2242 223a  "B": 300}, {"B":
+00013b60: 2033 3031 7d5d 2c0a 2020 2020 2020 2020   301}],.        
+00013b70: 6a6f 696e 5f6b 6579 733d 5b22 3132 3334  join_keys=["1234
+00013b80: 3522 2c20 2236 3738 3930 225d 2069 6620  5", "67890"] if 
+00013b90: 6b77 6172 6773 2065 6c73 6520 5b22 3637  kwargs else ["67
+00013ba0: 3839 3022 2c20 2231 3233 3435 225d 2c0a  890", "12345"],.
+00013bb0: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
+00013bc0: 7665 7273 696f 6e2c 0a20 2020 2020 2020  version,.       
+00013bd0: 2069 676e 6f72 655f 696e 7075 7473 3d4e   ignore_inputs=N
+00013be0: 6f6e 652c 0a20 2020 2020 2020 2074 696d  one,.        tim
+00013bf0: 6573 7461 6d70 733d 7465 7374 5f74 696d  estamps=test_tim
+00013c00: 6573 7461 6d70 735f 6c69 7374 2c0a 2020  estamps_list,.  
+00013c10: 2020 2020 2020 736f 7274 5f6f 6e5f 7469        sort_on_ti
+00013c20: 6d65 7374 616d 703d 5472 7565 2c0a 2020  mestamp=True,.  
+00013c30: 2020 2020 2020 6173 5f62 6174 6368 3d46        as_batch=F
+00013c40: 616c 7365 2c0a 2020 2020 2020 2020 7461  alse,.        ta
+00013c50: 6773 3d65 7870 6563 7465 645f 7461 6773  gs=expected_tags
+00013c60: 5f70 6172 616d 2c0a 2020 2020 290a 2020  _param,.    ).  
+00013c70: 2020 6d6f 636b 5f66 6565 6462 6163 6b2e    mock_feedback.
+00013c80: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
+00013c90: 6428 290a 0a20 2020 206d 6f63 6b5f 7361  d()..    mock_sa
+00013ca0: 6d70 6c65 5f72 6563 6f72 6473 2e61 7373  mple_records.ass
+00013cb0: 6572 745f 6361 6c6c 6564 5f6f 6e63 655f  ert_called_once_
+00013cc0: 7769 7468 280a 2020 2020 2020 2020 322c  with(.        2,
+00013cd0: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
+00013ce0: 2020 2020 5b7b 2241 223a 2031 3030 7d2c      [{"A": 100},
+00013cf0: 207b 2241 223a 2031 3031 7d5d 2c0a 2020   {"A": 101}],.  
+00013d00: 2020 2020 2020 5b7b 2242 223a 2033 3030        [{"B": 300
+00013d10: 7d2c 207b 2242 223a 2033 3031 7d5d 2c0a  }, {"B": 301}],.
+00013d20: 2020 2020 2020 2020 4e6f 6e65 2c0a 2020          None,.  
+00013d30: 2020 2020 2020 636c 6965 6e74 2e5f 7265        client._re
+00013d40: 736f 6c76 655f 6a6f 696e 5f6b 6579 7328  solve_join_keys(
+00013d50: 2a2a 6b77 6172 6773 292c 0a20 2020 2020  **kwargs),.     
+00013d60: 2020 2074 6573 745f 7469 6d65 7374 616d     test_timestam
+00013d70: 7073 5f6c 6973 742c 0a20 2020 2020 2020  ps_list,.       
+00013d80: 2065 7870 6563 7465 645f 7461 6773 5f70   expected_tags_p
+00013d90: 6172 616d 2c0a 2020 2020 290a 0a20 2020  aram,.    )..   
+00013da0: 2069 6620 6b77 6172 6773 3a0a 2020 2020   if kwargs:.    
+00013db0: 2020 2020 6d6f 636b 5f6a 6f69 6e5f 6b65      mock_join_ke
+00013dc0: 795f 6765 6e2e 6173 7365 7274 5f6e 6f74  y_gen.assert_not
+00013dd0: 5f63 616c 6c65 6428 290a 2020 2020 656c  _called().    el
+00013de0: 7365 3a0a 2020 2020 2020 2020 6d6f 636b  se:.        mock
+00013df0: 5f6a 6f69 6e5f 6b65 795f 6765 6e2e 6173  _join_key_gen.as
+00013e00: 7365 7274 5f63 616c 6c65 6428 290a 0a0a  sert_called()...
+00013e10: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
+00013e20: 616d 6574 7269 7a65 280a 2020 2020 2274  ametrize(.    "t
+00013e30: 6573 745f 7469 6d65 7374 616d 7073 2c20  est_timestamps, 
+00013e40: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
+00013e50: 6c69 7374 222c 0a20 2020 205b 0a20 2020  list",.    [.   
+00013e60: 2020 2020 2028 4e6f 6e65 2c20 4e6f 6e65       (None, None
+00013e70: 292c 0a20 2020 2020 2020 2028 5b43 5552  ),.        ([CUR
+00013e80: 5245 4e54 5f54 494d 455d 202a 2032 2c20  RENT_TIME] * 2, 
+00013e90: 5b43 5552 5245 4e54 5f54 494d 455d 202a  [CURRENT_TIME] *
+00013ea0: 2032 292c 0a20 2020 2020 2020 2028 6e70   2),.        (np
+00013eb0: 2e61 7272 6179 285b 4355 5252 454e 545f  .array([CURRENT_
+00013ec0: 5449 4d45 5d20 2a20 3229 2c20 5b43 5552  TIME] * 2), [CUR
+00013ed0: 5245 4e54 5f54 494d 455d 202a 2032 292c  RENT_TIME] * 2),
+00013ee0: 0a20 2020 205d 2c0a 290a 4070 7974 6573  .    ],.).@pytes
+00013ef0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+00013f00: 7a65 280a 2020 2020 226b 7761 7267 7322  ze(.    "kwargs"
+00013f10: 2c0a 2020 2020 5b0a 2020 2020 2020 2020  ,.    [.        
+00013f20: 7b22 6a6f 696e 5f6b 6579 7322 3a20 5b22  {"join_keys": ["
+00013f30: 3534 3332 3122 2c20 2236 3738 3930 225d  54321", "67890"]
+00013f40: 7d2c 0a20 2020 2020 2020 207b 226a 6f69  },.        {"joi
+00013f50: 6e5f 6b65 7973 223a 2070 642e 5365 7269  n_keys": pd.Seri
+00013f60: 6573 285b 2235 3433 3231 222c 2022 3637  es(["54321", "67
+00013f70: 3839 3022 5d29 7d2c 0a20 2020 2020 2020  890"])},.       
+00013f80: 207b 7d2c 0a20 2020 205d 2c0a 290a 4070   {},.    ],.).@p
+00013f90: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
+00013fa0: 6574 7269 7a65 280a 2020 2020 2822 7465  etrize(.    ("te
+00013fb0: 7374 5f6f 7574 7075 7473 222c 2022 7465  st_outputs", "te
+00013fc0: 7374 5f69 6e70 7574 7322 292c 0a20 2020  st_inputs"),.   
+00013fd0: 206c 6973 7428 7a69 7028 5445 5354 5f4f   list(zip(TEST_O
+00013fe0: 5554 5055 5453 2c20 5445 5354 5f49 4e50  UTPUTS, TEST_INP
+00013ff0: 5554 5329 292c 0a29 0a40 7079 7465 7374  UTS)),.).@pytest
+00014000: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00014010: 6528 2276 6572 7369 6f6e 222c 205b 4e6f  e("version", [No
+00014020: 6e65 2c20 3130 2c20 2231 2e32 2e33 225d  ne, 10, "1.2.3"]
+00014030: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
+00014040: 6172 616d 6574 7269 7a65 2822 7461 6773  arametrize("tags
+00014050: 2c20 726f 775f 7461 6773 2c20 676c 6f62  , row_tags, glob
+00014060: 616c 5f74 6167 732c 2065 7870 6563 7465  al_tags, expecte
+00014070: 645f 7461 6773 5f70 6172 616d 222c 2054  d_tags_param", T
+00014080: 4553 545f 5441 4753 290a 406d 6f63 6b2e  EST_TAGS).@mock.
+00014090: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+000140a0: 6767 6572 2e63 6c69 656e 742e 5f72 6573  gger.client._res
+000140b0: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2229  olve_join_keys")
+000140c0: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
+000140d0: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+000140e0: 6e74 2e47 616e 7472 792e 5f67 656e 6572  nt.Gantry._gener
+000140f0: 6174 655f 7072 6564 6963 7469 6f6e 5f61  ate_prediction_a
+00014100: 6e64 5f66 6565 6462 6163 6b5f 6576 656e  nd_feedback_even
+00014110: 7473 2229 0a40 6d6f 636b 2e70 6174 6368  ts").@mock.patch
+00014120: 280a 2020 2020 2267 616e 7472 792e 6c6f  (.    "gantry.lo
+00014130: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
+00014140: 7279 2e5f 6765 6e65 7261 7465 5f70 7265  ry._generate_pre
+00014150: 6469 6374 696f 6e5f 6576 656e 7473 222c  diction_events",
+00014160: 0a20 2020 2072 6574 7572 6e5f 7661 6c75  .    return_valu
+00014170: 653d 285b 7b22 6576 656e 7422 3a20 2270  e=([{"event": "p
+00014180: 6c61 6365 5f68 6f6c 6465 7222 7d5d 2c20  lace_holder"}], 
+00014190: 5b22 3132 3334 3522 2c20 2236 3738 3930  ["12345", "67890
+000141a0: 225d 292c 0a29 0a40 6d6f 636b 2e70 6174  "]),.).@mock.pat
+000141b0: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
+000141c0: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
+000141d0: 5f67 656e 6572 6174 655f 6665 6564 6261  _generate_feedba
+000141e0: 636b 5f65 7665 6e74 7322 290a 406d 6f63  ck_events").@moc
 000141f0: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-00014200: 6c6f 6767 6572 2e63 6c69 656e 742e 5f64  logger.client._d
-00014210: 6566 6175 6c74 5f6a 6f69 6e5f 6b65 795f  efault_join_key_
-00014220: 6765 6e22 290a 6465 6620 7465 7374 5f67  gen").def test_g
-00014230: 656e 6572 6174 655f 7265 636f 7264 735f  enerate_records_
-00014240: 7072 6564 735f 6f6e 6c79 280a 2020 2020  preds_only(.    
-00014250: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
-00014260: 6e2c 0a20 2020 206d 6f63 6b5f 7361 6d70  n,.    mock_samp
-00014270: 6c65 5f72 6563 6f72 6473 2c0a 2020 2020  le_records,.    
-00014280: 6d6f 636b 5f67 656e 6572 6174 655f 6665  mock_generate_fe
-00014290: 6564 6261 636b 2c0a 2020 2020 6d6f 636b  edback,.    mock
-000142a0: 5f67 656e 6572 6174 655f 7072 6564 732c  _generate_preds,
-000142b0: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
-000142c0: 7465 5f70 7265 6473 5f61 6e64 5f66 6565  te_preds_and_fee
-000142d0: 6462 6163 6b2c 0a20 2020 206d 6f63 6b5f  dback,.    mock_
-000142e0: 7265 736f 6c76 655f 6a6f 696e 5f6b 6579  resolve_join_key
-000142f0: 732c 0a20 2020 2076 6572 7369 6f6e 2c0a  s,.    version,.
-00014300: 2020 2020 7461 6773 2c0a 2020 2020 726f      tags,.    ro
-00014310: 775f 7461 6773 2c0a 2020 2020 676c 6f62  w_tags,.    glob
-00014320: 616c 5f74 6167 732c 0a20 2020 2065 7870  al_tags,.    exp
-00014330: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
-00014340: 2c0a 2020 2020 7465 7374 5f74 696d 6573  ,.    test_times
-00014350: 7461 6d70 732c 0a20 2020 2074 6573 745f  tamps,.    test_
-00014360: 7469 6d65 7374 616d 7073 5f6c 6973 742c  timestamps_list,
-00014370: 0a20 2020 2074 6573 745f 696e 7075 7473  .    test_inputs
-00014380: 2c0a 2020 2020 7465 7374 5f6f 7574 7075  ,.    test_outpu
-00014390: 7473 2c0a 2020 2020 6b77 6172 6773 2c0a  ts,.    kwargs,.
-000143a0: 2020 2020 636c 695f 6f62 6a2c 0a29 3a0a      cli_obj,.):.
-000143b0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000143c0: 6528 7461 6773 2c20 6c69 7374 293a 0a20  e(tags, list):. 
-000143d0: 2020 2020 2020 2070 7974 6573 742e 736b         pytest.sk
-000143e0: 6970 2822 5468 6973 2074 6573 7420 6973  ip("This test is
-000143f0: 206e 6f74 2061 7070 6c69 6361 626c 6520   not applicable 
-00014400: 746f 206c 6973 7420 7461 6773 2229 0a0a  to list tags")..
-00014410: 2020 2020 6d6f 636b 5f6a 6f69 6e5f 6b65      mock_join_ke
-00014420: 795f 6765 6e2e 7369 6465 5f65 6666 6563  y_gen.side_effec
-00014430: 7420 3d20 5b22 3637 3839 3022 2c20 2231  t = ["67890", "1
-00014440: 3233 3435 225d 0a20 2020 206d 6f63 6b5f  2345"].    mock_
-00014450: 7265 736f 6c76 655f 6a6f 696e 5f6b 6579  resolve_join_key
-00014460: 732e 7265 7475 726e 5f76 616c 7565 203d  s.return_value =
-00014470: 205b 2231 3233 3435 222c 2022 3637 3839   ["12345", "6789
-00014480: 3022 5d20 6966 206b 7761 7267 7320 656c  0"] if kwargs el
-00014490: 7365 204e 6f6e 650a 2020 2020 7275 6e5f  se None.    run_
-000144a0: 6964 203d 2073 7472 2875 7569 642e 7575  id = str(uuid.uu
-000144b0: 6964 3428 2929 0a20 2020 2072 756e 5f74  id4()).    run_t
-000144c0: 6167 7320 3d20 4e6f 6e65 0a20 2020 2069  ags = None.    i
-000144d0: 6620 7461 6773 2061 6e64 2067 6c6f 6261  f tags and globa
-000144e0: 6c5f 7461 6773 3a0a 2020 2020 2020 2020  l_tags:.        
-000144f0: 7275 6e5f 7461 6773 203d 207b 2a2a 7461  run_tags = {**ta
-00014500: 6773 2c20 2a2a 676c 6f62 616c 5f74 6167  gs, **global_tag
-00014510: 737d 0a20 2020 2065 6c69 6620 7461 6773  s}.    elif tags
-00014520: 3a0a 2020 2020 2020 2020 7275 6e5f 7461  :.        run_ta
-00014530: 6773 203d 2074 6167 730a 2020 2020 656c  gs = tags.    el
-00014540: 6966 2067 6c6f 6261 6c5f 7461 6773 3a0a  if global_tags:.
-00014550: 2020 2020 2020 2020 7275 6e5f 7461 6773          run_tags
-00014560: 203d 2067 6c6f 6261 6c5f 7461 6773 0a20   = global_tags. 
-00014570: 2020 2061 7373 6572 7420 636c 695f 6f62     assert cli_ob
-00014580: 6a2e 6c6f 6728 0a20 2020 2020 2020 2061  j.log(.        a
-00014590: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
-000145a0: 6172 222c 0a20 2020 2020 2020 2076 6572  ar",.        ver
-000145b0: 7369 6f6e 3d76 6572 7369 6f6e 2c0a 2020  sion=version,.  
-000145c0: 2020 2020 2020 696e 7075 7473 3d74 6573        inputs=tes
-000145d0: 745f 696e 7075 7473 2c0a 2020 2020 2020  t_inputs,.      
-000145e0: 2020 6f75 7470 7574 733d 7465 7374 5f6f    outputs=test_o
-000145f0: 7574 7075 7473 2c0a 2020 2020 2020 2020  utputs,.        
-00014600: 6665 6564 6261 636b 733d 4e6f 6e65 2c0a  feedbacks=None,.
-00014610: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
-00014620: 7073 3d74 6573 745f 7469 6d65 7374 616d  ps=test_timestam
-00014630: 7073 2c0a 2020 2020 2020 2020 736f 7274  ps,.        sort
-00014640: 5f6f 6e5f 7469 6d65 7374 616d 703d 5472  _on_timestamp=Tr
-00014650: 7565 2c0a 2020 2020 2020 2020 7275 6e5f  ue,.        run_
-00014660: 7461 6773 3d72 756e 5f74 6167 732c 0a20  tags=run_tags,. 
-00014670: 2020 2020 2020 2072 6f77 5f74 6167 733d         row_tags=
-00014680: 726f 775f 7461 6773 2c0a 2020 2020 2020  row_tags,.      
-00014690: 2020 7275 6e5f 6964 3d72 756e 5f69 642c    run_id=run_id,
-000146a0: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
-000146b0: 732c 0a20 2020 2029 203d 3d20 5b7b 2265  s,.    ) == [{"e
-000146c0: 7665 6e74 223a 2022 706c 6163 655f 686f  vent": "place_ho
-000146d0: 6c64 6572 227d 5d0a 0a20 2020 206d 6f63  lder"}]..    moc
-000146e0: 6b5f 6765 6e65 7261 7465 5f70 7265 6473  k_generate_preds
-000146f0: 5f61 6e64 5f66 6565 6462 6163 6b2e 6173  _and_feedback.as
-00014700: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
-00014710: 290a 2020 2020 6d6f 636b 5f67 656e 6572  ).    mock_gener
-00014720: 6174 655f 7072 6564 732e 6173 7365 7274  ate_preds.assert
-00014730: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
-00014740: 6828 0a20 2020 2020 2020 2061 7070 6c69  h(.        appli
-00014750: 6361 7469 6f6e 3d22 666f 6f62 6172 222c  cation="foobar",
-00014760: 0a20 2020 2020 2020 2069 6e70 7574 733d  .        inputs=
-00014770: 5b7b 2241 223a 2031 3030 7d2c 207b 2241  [{"A": 100}, {"A
-00014780: 223a 2031 3031 7d5d 2c0a 2020 2020 2020  ": 101}],.      
-00014790: 2020 6f75 7470 7574 733d 5b7b 2242 223a    outputs=[{"B":
-000147a0: 2033 3030 7d2c 207b 2242 223a 2033 3031   300}, {"B": 301
-000147b0: 7d5d 2c0a 2020 2020 2020 2020 6a6f 696e  }],.        join
-000147c0: 5f6b 6579 733d 5b22 3132 3334 3522 2c20  _keys=["12345", 
-000147d0: 2236 3738 3930 225d 2069 6620 6b77 6172  "67890"] if kwar
-000147e0: 6773 2065 6c73 6520 5b22 3637 3839 3022  gs else ["67890"
-000147f0: 2c20 2231 3233 3435 225d 2c0a 2020 2020  , "12345"],.    
-00014800: 2020 2020 7665 7273 696f 6e3d 7665 7273      version=vers
-00014810: 696f 6e2c 0a20 2020 2020 2020 2069 676e  ion,.        ign
-00014820: 6f72 655f 696e 7075 7473 3d4e 6f6e 652c  ore_inputs=None,
-00014830: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
-00014840: 6d70 733d 7465 7374 5f74 696d 6573 7461  mps=test_timesta
-00014850: 6d70 735f 6c69 7374 2c0a 2020 2020 2020  mps_list,.      
-00014860: 2020 736f 7274 5f6f 6e5f 7469 6d65 7374    sort_on_timest
-00014870: 616d 703d 5472 7565 2c0a 2020 2020 2020  amp=True,.      
-00014880: 2020 7275 6e5f 6964 3d72 756e 5f69 642c    run_id=run_id,
-00014890: 0a20 2020 2020 2020 2074 6167 733d 6578  .        tags=ex
-000148a0: 7065 6374 6564 5f74 6167 735f 7061 7261  pected_tags_para
-000148b0: 6d2c 0a20 2020 2029 0a20 2020 206d 6f63  m,.    ).    moc
-000148c0: 6b5f 6765 6e65 7261 7465 5f66 6565 6462  k_generate_feedb
-000148d0: 6163 6b2e 6173 7365 7274 5f6e 6f74 5f63  ack.assert_not_c
-000148e0: 616c 6c65 6428 290a 0a20 2020 206d 6f63  alled()..    moc
-000148f0: 6b5f 7361 6d70 6c65 5f72 6563 6f72 6473  k_sample_records
-00014900: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
-00014910: 6e63 655f 7769 7468 280a 2020 2020 2020  nce_with(.      
-00014920: 2020 322c 0a20 2020 2020 2020 2031 2c0a    2,.        1,.
-00014930: 2020 2020 2020 2020 5b7b 2241 223a 2031          [{"A": 1
-00014940: 3030 7d2c 207b 2241 223a 2031 3031 7d5d  00}, {"A": 101}]
-00014950: 2c0a 2020 2020 2020 2020 5b7b 2242 223a  ,.        [{"B":
-00014960: 2033 3030 7d2c 207b 2242 223a 2033 3031   300}, {"B": 301
-00014970: 7d5d 2c0a 2020 2020 2020 2020 4e6f 6e65  }],.        None
-00014980: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
-00014990: 2e5f 7265 736f 6c76 655f 6a6f 696e 5f6b  ._resolve_join_k
-000149a0: 6579 7328 2a2a 6b77 6172 6773 292c 0a20  eys(**kwargs),. 
-000149b0: 2020 2020 2020 2074 6573 745f 7469 6d65         test_time
-000149c0: 7374 616d 7073 5f6c 6973 742c 0a20 2020  stamps_list,.   
-000149d0: 2020 2020 2065 7870 6563 7465 645f 7461       expected_ta
-000149e0: 6773 5f70 6172 616d 2c0a 2020 2020 290a  gs_param,.    ).
-000149f0: 0a20 2020 2069 6620 6b77 6172 6773 3a0a  .    if kwargs:.
-00014a00: 2020 2020 2020 2020 6d6f 636b 5f6a 6f69          mock_joi
-00014a10: 6e5f 6b65 795f 6765 6e2e 6173 7365 7274  n_key_gen.assert
-00014a20: 5f6e 6f74 5f63 616c 6c65 6428 290a 2020  _not_called().  
-00014a30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014a40: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
-00014a50: 6e2e 6173 7365 7274 5f63 616c 6c65 6428  n.assert_called(
-00014a60: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-00014a70: 2e70 6172 616d 6574 7269 7a65 280a 2020  .parametrize(.  
-00014a80: 2020 2274 6573 745f 7469 6d65 7374 616d    "test_timestam
-00014a90: 7073 2c20 7465 7374 5f74 696d 6573 7461  ps, test_timesta
-00014aa0: 6d70 735f 6c69 7374 222c 0a20 2020 205b  mps_list",.    [
-00014ab0: 0a20 2020 2020 2020 2028 4e6f 6e65 2c20  .        (None, 
-00014ac0: 4e6f 6e65 292c 0a20 2020 2020 2020 2028  None),.        (
-00014ad0: 5b43 5552 5245 4e54 5f54 494d 455d 202a  [CURRENT_TIME] *
-00014ae0: 2032 2c20 5b43 5552 5245 4e54 5f54 494d   2, [CURRENT_TIM
-00014af0: 455d 202a 2032 292c 0a20 2020 2020 2020  E] * 2),.       
-00014b00: 2028 6e70 2e61 7272 6179 285b 4355 5252   (np.array([CURR
-00014b10: 454e 545f 5449 4d45 5d20 2a20 3229 2c20  ENT_TIME] * 2), 
-00014b20: 5b43 5552 5245 4e54 5f54 494d 455d 202a  [CURRENT_TIME] *
-00014b30: 2032 292c 0a20 2020 205d 2c0a 290a 4070   2),.    ],.).@p
-00014b40: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-00014b50: 6574 7269 7a65 280a 2020 2020 226b 7761  etrize(.    "kwa
-00014b60: 7267 7322 2c0a 2020 2020 5b0a 2020 2020  rgs",.    [.    
-00014b70: 2020 2020 7b22 6665 6564 6261 636b 5f6b      {"feedback_k
-00014b80: 6579 7322 3a20 5b22 4122 5d7d 2c0a 2020  eys": ["A"]},.  
-00014b90: 2020 2020 2020 7b22 6665 6564 6261 636b        {"feedback
-00014ba0: 5f69 6473 223a 205b 2231 3233 3435 222c  _ids": ["12345",
-00014bb0: 2022 3637 3839 3022 5d7d 2c0a 2020 2020   "67890"]},.    
-00014bc0: 2020 2020 7b22 6a6f 696e 5f6b 6579 7322      {"join_keys"
-00014bd0: 3a20 5b22 3534 3332 3122 2c20 2236 3738  : ["54321", "678
-00014be0: 3930 225d 7d2c 0a20 2020 2020 2020 207b  90"]},.        {
-00014bf0: 226a 6f69 6e5f 6b65 7973 223a 2070 642e  "join_keys": pd.
-00014c00: 5365 7269 6573 285b 2235 3433 3231 222c  Series(["54321",
-00014c10: 2022 3637 3839 3022 5d29 7d2c 0a20 2020   "67890"])},.   
-00014c20: 205d 2c0a 290a 4070 7974 6573 742e 6d61   ],.).@pytest.ma
-00014c30: 726b 2e70 6172 616d 6574 7269 7a65 2822  rk.parametrize("
-00014c40: 7465 7374 5f66 6565 6462 6163 6b73 222c  test_feedbacks",
-00014c50: 2054 4553 545f 4645 4544 4241 434b 5329   TEST_FEEDBACKS)
-00014c60: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
-00014c70: 7261 6d65 7472 697a 6528 2276 6572 7369  rametrize("versi
-00014c80: 6f6e 222c 205b 4e6f 6e65 2c20 3130 2c20  on", [None, 10, 
-00014c90: 2231 2e32 2e33 225d 290a 4070 7974 6573  "1.2.3"]).@pytes
-00014ca0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00014cb0: 7a65 2822 7461 6773 2c20 726f 775f 7461  ze("tags, row_ta
-00014cc0: 6773 2c20 676c 6f62 616c 5f74 6167 732c  gs, global_tags,
-00014cd0: 2065 7870 6563 7465 645f 7461 6773 5f70   expected_tags_p
-00014ce0: 6172 616d 222c 2054 4553 545f 5441 4753  aram", TEST_TAGS
-00014cf0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-00014d00: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00014d10: 656e 742e 5f72 6573 6f6c 7665 5f6a 6f69  ent._resolve_joi
-00014d20: 6e5f 6b65 7973 222c 2072 6574 7572 6e5f  n_keys", return_
-00014d30: 7661 6c75 653d 5b22 3132 3334 3522 2c20  value=["12345", 
-00014d40: 2235 3433 3231 225d 290a 406d 6f63 6b2e  "54321"]).@mock.
+00014200: 6c6f 6767 6572 2e63 6c69 656e 742e 5f73  logger.client._s
+00014210: 616d 706c 655f 7265 636f 7264 7322 2c20  ample_records", 
+00014220: 7369 6465 5f65 6666 6563 743d 636c 6965  side_effect=clie
+00014230: 6e74 2e5f 7361 6d70 6c65 5f72 6563 6f72  nt._sample_recor
+00014240: 6473 290a 406d 6f63 6b2e 7061 7463 6828  ds).@mock.patch(
+00014250: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
+00014260: 6c69 656e 742e 5f64 6566 6175 6c74 5f6a  lient._default_j
+00014270: 6f69 6e5f 6b65 795f 6765 6e22 290a 6465  oin_key_gen").de
+00014280: 6620 7465 7374 5f67 656e 6572 6174 655f  f test_generate_
+00014290: 7265 636f 7264 735f 7072 6564 735f 6f6e  records_preds_on
+000142a0: 6c79 280a 2020 2020 6d6f 636b 5f6a 6f69  ly(.    mock_joi
+000142b0: 6e5f 6b65 795f 6765 6e2c 0a20 2020 206d  n_key_gen,.    m
+000142c0: 6f63 6b5f 7361 6d70 6c65 5f72 6563 6f72  ock_sample_recor
+000142d0: 6473 2c0a 2020 2020 6d6f 636b 5f67 656e  ds,.    mock_gen
+000142e0: 6572 6174 655f 6665 6564 6261 636b 2c0a  erate_feedback,.
+000142f0: 2020 2020 6d6f 636b 5f67 656e 6572 6174      mock_generat
+00014300: 655f 7072 6564 732c 0a20 2020 206d 6f63  e_preds,.    moc
+00014310: 6b5f 6765 6e65 7261 7465 5f70 7265 6473  k_generate_preds
+00014320: 5f61 6e64 5f66 6565 6462 6163 6b2c 0a20  _and_feedback,. 
+00014330: 2020 206d 6f63 6b5f 7265 736f 6c76 655f     mock_resolve_
+00014340: 6a6f 696e 5f6b 6579 732c 0a20 2020 2076  join_keys,.    v
+00014350: 6572 7369 6f6e 2c0a 2020 2020 7461 6773  ersion,.    tags
+00014360: 2c0a 2020 2020 726f 775f 7461 6773 2c0a  ,.    row_tags,.
+00014370: 2020 2020 676c 6f62 616c 5f74 6167 732c      global_tags,
+00014380: 0a20 2020 2065 7870 6563 7465 645f 7461  .    expected_ta
+00014390: 6773 5f70 6172 616d 2c0a 2020 2020 7465  gs_param,.    te
+000143a0: 7374 5f74 696d 6573 7461 6d70 732c 0a20  st_timestamps,. 
+000143b0: 2020 2074 6573 745f 7469 6d65 7374 616d     test_timestam
+000143c0: 7073 5f6c 6973 742c 0a20 2020 2074 6573  ps_list,.    tes
+000143d0: 745f 696e 7075 7473 2c0a 2020 2020 7465  t_inputs,.    te
+000143e0: 7374 5f6f 7574 7075 7473 2c0a 2020 2020  st_outputs,.    
+000143f0: 6b77 6172 6773 2c0a 2020 2020 636c 695f  kwargs,.    cli_
+00014400: 6f62 6a2c 0a29 3a0a 2020 2020 6966 2069  obj,.):.    if i
+00014410: 7369 6e73 7461 6e63 6528 7461 6773 2c20  sinstance(tags, 
+00014420: 6c69 7374 293a 0a20 2020 2020 2020 2070  list):.        p
+00014430: 7974 6573 742e 736b 6970 2822 5468 6973  ytest.skip("This
+00014440: 2074 6573 7420 6973 206e 6f74 2061 7070   test is not app
+00014450: 6c69 6361 626c 6520 746f 206c 6973 7420  licable to list 
+00014460: 7461 6773 2229 0a0a 2020 2020 6d6f 636b  tags")..    mock
+00014470: 5f6a 6f69 6e5f 6b65 795f 6765 6e2e 7369  _join_key_gen.si
+00014480: 6465 5f65 6666 6563 7420 3d20 5b22 3637  de_effect = ["67
+00014490: 3839 3022 2c20 2231 3233 3435 225d 0a20  890", "12345"]. 
+000144a0: 2020 206d 6f63 6b5f 7265 736f 6c76 655f     mock_resolve_
+000144b0: 6a6f 696e 5f6b 6579 732e 7265 7475 726e  join_keys.return
+000144c0: 5f76 616c 7565 203d 205b 2231 3233 3435  _value = ["12345
+000144d0: 222c 2022 3637 3839 3022 5d20 6966 206b  ", "67890"] if k
+000144e0: 7761 7267 7320 656c 7365 204e 6f6e 650a  wargs else None.
+000144f0: 2020 2020 7275 6e5f 6964 203d 2073 7472      run_id = str
+00014500: 2875 7569 642e 7575 6964 3428 2929 0a20  (uuid.uuid4()). 
+00014510: 2020 2072 756e 5f74 6167 7320 3d20 4e6f     run_tags = No
+00014520: 6e65 0a20 2020 2069 6620 7461 6773 2061  ne.    if tags a
+00014530: 6e64 2067 6c6f 6261 6c5f 7461 6773 3a0a  nd global_tags:.
+00014540: 2020 2020 2020 2020 7275 6e5f 7461 6773          run_tags
+00014550: 203d 207b 2a2a 7461 6773 2c20 2a2a 676c   = {**tags, **gl
+00014560: 6f62 616c 5f74 6167 737d 0a20 2020 2065  obal_tags}.    e
+00014570: 6c69 6620 7461 6773 3a0a 2020 2020 2020  lif tags:.      
+00014580: 2020 7275 6e5f 7461 6773 203d 2074 6167    run_tags = tag
+00014590: 730a 2020 2020 656c 6966 2067 6c6f 6261  s.    elif globa
+000145a0: 6c5f 7461 6773 3a0a 2020 2020 2020 2020  l_tags:.        
+000145b0: 7275 6e5f 7461 6773 203d 2067 6c6f 6261  run_tags = globa
+000145c0: 6c5f 7461 6773 0a20 2020 2061 7373 6572  l_tags.    asser
+000145d0: 7420 636c 695f 6f62 6a2e 6c6f 6728 0a20  t cli_obj.log(. 
+000145e0: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
+000145f0: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
+00014600: 2020 2020 2076 6572 7369 6f6e 3d76 6572       version=ver
+00014610: 7369 6f6e 2c0a 2020 2020 2020 2020 696e  sion,.        in
+00014620: 7075 7473 3d74 6573 745f 696e 7075 7473  puts=test_inputs
+00014630: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
+00014640: 733d 7465 7374 5f6f 7574 7075 7473 2c0a  s=test_outputs,.
+00014650: 2020 2020 2020 2020 6665 6564 6261 636b          feedback
+00014660: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+00014670: 7469 6d65 7374 616d 7073 3d74 6573 745f  timestamps=test_
+00014680: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
+00014690: 2020 2020 736f 7274 5f6f 6e5f 7469 6d65      sort_on_time
+000146a0: 7374 616d 703d 5472 7565 2c0a 2020 2020  stamp=True,.    
+000146b0: 2020 2020 7275 6e5f 7461 6773 3d72 756e      run_tags=run
+000146c0: 5f74 6167 732c 0a20 2020 2020 2020 2072  _tags,.        r
+000146d0: 6f77 5f74 6167 733d 726f 775f 7461 6773  ow_tags=row_tags
+000146e0: 2c0a 2020 2020 2020 2020 7275 6e5f 6964  ,.        run_id
+000146f0: 3d72 756e 5f69 642c 0a20 2020 2020 2020  =run_id,.       
+00014700: 202a 2a6b 7761 7267 732c 0a20 2020 2029   **kwargs,.    )
+00014710: 203d 3d20 5b7b 2265 7665 6e74 223a 2022   == [{"event": "
+00014720: 706c 6163 655f 686f 6c64 6572 227d 5d0a  place_holder"}].
+00014730: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
+00014740: 7465 5f70 7265 6473 5f61 6e64 5f66 6565  te_preds_and_fee
+00014750: 6462 6163 6b2e 6173 7365 7274 5f6e 6f74  dback.assert_not
+00014760: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
+00014770: 636b 5f67 656e 6572 6174 655f 7072 6564  ck_generate_pred
+00014780: 732e 6173 7365 7274 5f63 616c 6c65 645f  s.assert_called_
+00014790: 6f6e 6365 5f77 6974 6828 0a20 2020 2020  once_with(.     
+000147a0: 2020 2061 7070 6c69 6361 7469 6f6e 3d22     application="
+000147b0: 666f 6f62 6172 222c 0a20 2020 2020 2020  foobar",.       
+000147c0: 2069 6e70 7574 733d 5b7b 2241 223a 2031   inputs=[{"A": 1
+000147d0: 3030 7d2c 207b 2241 223a 2031 3031 7d5d  00}, {"A": 101}]
+000147e0: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
+000147f0: 733d 5b7b 2242 223a 2033 3030 7d2c 207b  s=[{"B": 300}, {
+00014800: 2242 223a 2033 3031 7d5d 2c0a 2020 2020  "B": 301}],.    
+00014810: 2020 2020 6a6f 696e 5f6b 6579 733d 5b22      join_keys=["
+00014820: 3132 3334 3522 2c20 2236 3738 3930 225d  12345", "67890"]
+00014830: 2069 6620 6b77 6172 6773 2065 6c73 6520   if kwargs else 
+00014840: 5b22 3637 3839 3022 2c20 2231 3233 3435  ["67890", "12345
+00014850: 225d 2c0a 2020 2020 2020 2020 7665 7273  "],.        vers
+00014860: 696f 6e3d 7665 7273 696f 6e2c 0a20 2020  ion=version,.   
+00014870: 2020 2020 2069 676e 6f72 655f 696e 7075       ignore_inpu
+00014880: 7473 3d4e 6f6e 652c 0a20 2020 2020 2020  ts=None,.       
+00014890: 2074 696d 6573 7461 6d70 733d 7465 7374   timestamps=test
+000148a0: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
+000148b0: 2c0a 2020 2020 2020 2020 736f 7274 5f6f  ,.        sort_o
+000148c0: 6e5f 7469 6d65 7374 616d 703d 5472 7565  n_timestamp=True
+000148d0: 2c0a 2020 2020 2020 2020 7275 6e5f 6964  ,.        run_id
+000148e0: 3d72 756e 5f69 642c 0a20 2020 2020 2020  =run_id,.       
+000148f0: 2074 6167 733d 6578 7065 6374 6564 5f74   tags=expected_t
+00014900: 6167 735f 7061 7261 6d2c 0a20 2020 2029  ags_param,.    )
+00014910: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
+00014920: 7465 5f66 6565 6462 6163 6b2e 6173 7365  te_feedback.asse
+00014930: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
+00014940: 0a20 2020 206d 6f63 6b5f 7361 6d70 6c65  .    mock_sample
+00014950: 5f72 6563 6f72 6473 2e61 7373 6572 745f  _records.assert_
+00014960: 6361 6c6c 6564 5f6f 6e63 655f 7769 7468  called_once_with
+00014970: 280a 2020 2020 2020 2020 322c 0a20 2020  (.        2,.   
+00014980: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
+00014990: 5b7b 2241 223a 2031 3030 7d2c 207b 2241  [{"A": 100}, {"A
+000149a0: 223a 2031 3031 7d5d 2c0a 2020 2020 2020  ": 101}],.      
+000149b0: 2020 5b7b 2242 223a 2033 3030 7d2c 207b    [{"B": 300}, {
+000149c0: 2242 223a 2033 3031 7d5d 2c0a 2020 2020  "B": 301}],.    
+000149d0: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
+000149e0: 2020 636c 6965 6e74 2e5f 7265 736f 6c76    client._resolv
+000149f0: 655f 6a6f 696e 5f6b 6579 7328 2a2a 6b77  e_join_keys(**kw
+00014a00: 6172 6773 292c 0a20 2020 2020 2020 2074  args),.        t
+00014a10: 6573 745f 7469 6d65 7374 616d 7073 5f6c  est_timestamps_l
+00014a20: 6973 742c 0a20 2020 2020 2020 2065 7870  ist,.        exp
+00014a30: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
+00014a40: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
+00014a50: 6b77 6172 6773 3a0a 2020 2020 2020 2020  kwargs:.        
+00014a60: 6d6f 636b 5f6a 6f69 6e5f 6b65 795f 6765  mock_join_key_ge
+00014a70: 6e2e 6173 7365 7274 5f6e 6f74 5f63 616c  n.assert_not_cal
+00014a80: 6c65 6428 290a 2020 2020 656c 7365 3a0a  led().    else:.
+00014a90: 2020 2020 2020 2020 6d6f 636b 5f6a 6f69          mock_joi
+00014aa0: 6e5f 6b65 795f 6765 6e2e 6173 7365 7274  n_key_gen.assert
+00014ab0: 5f63 616c 6c65 6428 290a 0a0a 4070 7974  _called()...@pyt
+00014ac0: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
+00014ad0: 7269 7a65 280a 2020 2020 2274 6573 745f  rize(.    "test_
+00014ae0: 7469 6d65 7374 616d 7073 2c20 7465 7374  timestamps, test
+00014af0: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
+00014b00: 222c 0a20 2020 205b 0a20 2020 2020 2020  ",.    [.       
+00014b10: 2028 4e6f 6e65 2c20 4e6f 6e65 292c 0a20   (None, None),. 
+00014b20: 2020 2020 2020 2028 5b43 5552 5245 4e54         ([CURRENT
+00014b30: 5f54 494d 455d 202a 2032 2c20 5b43 5552  _TIME] * 2, [CUR
+00014b40: 5245 4e54 5f54 494d 455d 202a 2032 292c  RENT_TIME] * 2),
+00014b50: 0a20 2020 2020 2020 2028 6e70 2e61 7272  .        (np.arr
+00014b60: 6179 285b 4355 5252 454e 545f 5449 4d45  ay([CURRENT_TIME
+00014b70: 5d20 2a20 3229 2c20 5b43 5552 5245 4e54  ] * 2), [CURRENT
+00014b80: 5f54 494d 455d 202a 2032 292c 0a20 2020  _TIME] * 2),.   
+00014b90: 205d 2c0a 290a 4070 7974 6573 742e 6d61   ],.).@pytest.ma
+00014ba0: 726b 2e70 6172 616d 6574 7269 7a65 280a  rk.parametrize(.
+00014bb0: 2020 2020 226b 7761 7267 7322 2c0a 2020      "kwargs",.  
+00014bc0: 2020 5b0a 2020 2020 2020 2020 7b22 6665    [.        {"fe
+00014bd0: 6564 6261 636b 5f6b 6579 7322 3a20 5b22  edback_keys": ["
+00014be0: 4122 5d7d 2c0a 2020 2020 2020 2020 7b22  A"]},.        {"
+00014bf0: 6665 6564 6261 636b 5f69 6473 223a 205b  feedback_ids": [
+00014c00: 2231 3233 3435 222c 2022 3637 3839 3022  "12345", "67890"
+00014c10: 5d7d 2c0a 2020 2020 2020 2020 7b22 6a6f  ]},.        {"jo
+00014c20: 696e 5f6b 6579 7322 3a20 5b22 3534 3332  in_keys": ["5432
+00014c30: 3122 2c20 2236 3738 3930 225d 7d2c 0a20  1", "67890"]},. 
+00014c40: 2020 2020 2020 207b 226a 6f69 6e5f 6b65         {"join_ke
+00014c50: 7973 223a 2070 642e 5365 7269 6573 285b  ys": pd.Series([
+00014c60: 2235 3433 3231 222c 2022 3637 3839 3022  "54321", "67890"
+00014c70: 5d29 7d2c 0a20 2020 205d 2c0a 290a 4070  ])},.    ],.).@p
+00014c80: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
+00014c90: 6574 7269 7a65 2822 7465 7374 5f66 6565  etrize("test_fee
+00014ca0: 6462 6163 6b73 222c 2054 4553 545f 4645  dbacks", TEST_FE
+00014cb0: 4544 4241 434b 5329 0a40 7079 7465 7374  EDBACKS).@pytest
+00014cc0: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00014cd0: 6528 2276 6572 7369 6f6e 222c 205b 4e6f  e("version", [No
+00014ce0: 6e65 2c20 3130 2c20 2231 2e32 2e33 225d  ne, 10, "1.2.3"]
+00014cf0: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
+00014d00: 6172 616d 6574 7269 7a65 2822 7461 6773  arametrize("tags
+00014d10: 2c20 726f 775f 7461 6773 2c20 676c 6f62  , row_tags, glob
+00014d20: 616c 5f74 6167 732c 2065 7870 6563 7465  al_tags, expecte
+00014d30: 645f 7461 6773 5f70 6172 616d 222c 2054  d_tags_param", T
+00014d40: 4553 545f 5441 4753 290a 406d 6f63 6b2e  EST_TAGS).@mock.
 00014d50: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-00014d60: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-00014d70: 7279 2e5f 6c6f 675f 7072 6564 6963 7469  ry._log_predicti
-00014d80: 6f6e 5f61 6e64 5f66 6565 6462 6163 6b5f  on_and_feedback_
-00014d90: 6576 656e 7473 2229 0a40 6d6f 636b 2e70  events").@mock.p
-00014da0: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
-00014db0: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-00014dc0: 792e 5f6c 6f67 5f70 7265 6469 6374 696f  y._log_predictio
-00014dd0: 6e5f 6576 656e 7473 2229 0a40 6d6f 636b  n_events").@mock
-00014de0: 2e70 6174 6368 280a 2020 2020 2267 616e  .patch(.    "gan
-00014df0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-00014e00: 742e 4761 6e74 7279 2e5f 6c6f 675f 6665  t.Gantry._log_fe
-00014e10: 6564 6261 636b 5f65 7665 6e74 7322 2c20  edback_events", 
-00014e20: 7265 7475 726e 5f76 616c 7565 3d28 4e6f  return_value=(No
-00014e30: 6e65 2c20 5b22 3132 3334 3522 2c20 2236  ne, ["12345", "6
-00014e40: 3738 3930 225d 290a 290a 406d 6f63 6b2e  7890"]).).@mock.
-00014e50: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-00014e60: 6767 6572 2e63 6c69 656e 742e 5f73 616d  gger.client._sam
-00014e70: 706c 655f 7265 636f 7264 7322 2c20 7369  ple_records", si
-00014e80: 6465 5f65 6666 6563 743d 636c 6965 6e74  de_effect=client
-00014e90: 2e5f 7361 6d70 6c65 5f72 6563 6f72 6473  ._sample_records
-00014ea0: 290a 6465 6620 7465 7374 5f6c 6f67 5f72  ).def test_log_r
-00014eb0: 6563 6f72 6473 5f66 6565 6462 6163 6b5f  ecords_feedback_
-00014ec0: 6f6e 6c79 280a 2020 2020 6d6f 636b 5f73  only(.    mock_s
-00014ed0: 616d 706c 655f 7265 636f 7264 732c 0a20  ample_records,. 
-00014ee0: 2020 206d 6f63 6b5f 6665 6564 6261 636b     mock_feedback
-00014ef0: 2c0a 2020 2020 6d6f 636b 5f70 7265 6473  ,.    mock_preds
-00014f00: 2c0a 2020 2020 6d6f 636b 5f70 7265 6473  ,.    mock_preds
-00014f10: 5f61 6e64 5f66 6565 6462 6163 6b2c 0a20  _and_feedback,. 
-00014f20: 2020 206d 6f63 6b5f 7265 736f 6c76 655f     mock_resolve_
-00014f30: 6a6f 696e 5f6b 6579 732c 0a20 2020 2076  join_keys,.    v
-00014f40: 6572 7369 6f6e 2c0a 2020 2020 7461 6773  ersion,.    tags
-00014f50: 2c0a 2020 2020 726f 775f 7461 6773 2c0a  ,.    row_tags,.
-00014f60: 2020 2020 676c 6f62 616c 5f74 6167 732c      global_tags,
-00014f70: 0a20 2020 2065 7870 6563 7465 645f 7461  .    expected_ta
-00014f80: 6773 5f70 6172 616d 2c0a 2020 2020 7465  gs_param,.    te
-00014f90: 7374 5f66 6565 6462 6163 6b73 2c0a 2020  st_feedbacks,.  
-00014fa0: 2020 7465 7374 5f74 696d 6573 7461 6d70    test_timestamp
-00014fb0: 732c 0a20 2020 2074 6573 745f 7469 6d65  s,.    test_time
-00014fc0: 7374 616d 7073 5f6c 6973 742c 0a20 2020  stamps_list,.   
-00014fd0: 206b 7761 7267 732c 0a20 2020 2063 6c69   kwargs,.    cli
-00014fe0: 5f6f 626a 2c0a 293a 0a20 2020 2061 7373  _obj,.):.    ass
-00014ff0: 6572 7420 636c 695f 6f62 6a2e 6c6f 675f  ert cli_obj.log_
-00015000: 7265 636f 7264 7328 0a20 2020 2020 2020  records(.       
-00015010: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
-00015020: 6f62 6172 222c 0a20 2020 2020 2020 2076  obar",.        v
-00015030: 6572 7369 6f6e 3d76 6572 7369 6f6e 2c0a  ersion=version,.
-00015040: 2020 2020 2020 2020 696e 7075 7473 3d4e          inputs=N
-00015050: 6f6e 652c 0a20 2020 2020 2020 206f 7574  one,.        out
-00015060: 7075 7473 3d4e 6f6e 652c 0a20 2020 2020  puts=None,.     
-00015070: 2020 2066 6565 6462 6163 6b73 3d74 6573     feedbacks=tes
-00015080: 745f 6665 6564 6261 636b 732c 0a20 2020  t_feedbacks,.   
-00015090: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
-000150a0: 7465 7374 5f74 696d 6573 7461 6d70 732c  test_timestamps,
-000150b0: 0a20 2020 2020 2020 2073 6f72 745f 6f6e  .        sort_on
-000150c0: 5f74 696d 6573 7461 6d70 3d54 7275 652c  _timestamp=True,
-000150d0: 0a20 2020 2020 2020 2074 6167 733d 7461  .        tags=ta
-000150e0: 6773 2c0a 2020 2020 2020 2020 726f 775f  gs,.        row_
-000150f0: 7461 6773 3d72 6f77 5f74 6167 732c 0a20  tags=row_tags,. 
-00015100: 2020 2020 2020 2067 6c6f 6261 6c5f 7461         global_ta
-00015110: 6773 3d67 6c6f 6261 6c5f 7461 6773 2c0a  gs=global_tags,.
-00015120: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00015130: 2c0a 2020 2020 2920 3d3d 2028 4e6f 6e65  ,.    ) == (None
-00015140: 2c20 5b22 3132 3334 3522 2c20 2236 3738  , ["12345", "678
-00015150: 3930 225d 290a 0a20 2020 206d 6f63 6b5f  90"])..    mock_
-00015160: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-00015170: 636b 2e61 7373 6572 745f 6e6f 745f 6361  ck.assert_not_ca
-00015180: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
-00015190: 7072 6564 732e 6173 7365 7274 5f6e 6f74  preds.assert_not
-000151a0: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
-000151b0: 636b 5f66 6565 6462 6163 6b2e 6173 7365  ck_feedback.asse
-000151c0: 7274 5f63 616c 6c65 645f 6f6e 6365 5f77  rt_called_once_w
-000151d0: 6974 6828 0a20 2020 2020 2020 2022 666f  ith(.        "fo
-000151e0: 6f62 6172 222c 0a20 2020 2020 2020 205b  obar",.        [
-000151f0: 7b22 4122 3a20 3230 307d 2c20 7b22 4122  {"A": 200}, {"A"
-00015200: 3a20 3230 317d 5d2c 0a20 2020 2020 2020  : 201}],.       
-00015210: 205b 2231 3233 3435 222c 2022 3534 3332   ["12345", "5432
-00015220: 3122 5d2c 0a20 2020 2020 2020 2076 6572  1"],.        ver
-00015230: 7369 6f6e 2c0a 2020 2020 2020 2020 7465  sion,.        te
-00015240: 7374 5f74 696d 6573 7461 6d70 735f 6c69  st_timestamps_li
-00015250: 7374 2c0a 2020 2020 2020 2020 5472 7565  st,.        True
-00015260: 2c0a 2020 2020 2020 2020 4661 6c73 652c  ,.        False,
-00015270: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-00015280: 645f 7461 6773 5f70 6172 616d 2c0a 2020  d_tags_param,.  
-00015290: 2020 290a 0a20 2020 206d 6f63 6b5f 7361    )..    mock_sa
-000152a0: 6d70 6c65 5f72 6563 6f72 6473 2e61 7373  mple_records.ass
-000152b0: 6572 745f 6361 6c6c 6564 5f6f 6e63 655f  ert_called_once_
-000152c0: 7769 7468 280a 2020 2020 2020 2020 322c  with(.        2,
-000152d0: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
-000152e0: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
-000152f0: 2020 4e6f 6e65 2c0a 2020 2020 2020 2020    None,.        
-00015300: 5b7b 2241 223a 2032 3030 7d2c 207b 2241  [{"A": 200}, {"A
-00015310: 223a 2032 3031 7d5d 2c0a 2020 2020 2020  ": 201}],.      
-00015320: 2020 636c 6965 6e74 2e5f 7265 736f 6c76    client._resolv
-00015330: 655f 6a6f 696e 5f6b 6579 7328 2a2a 6b77  e_join_keys(**kw
-00015340: 6172 6773 292c 0a20 2020 2020 2020 2074  args),.        t
-00015350: 6573 745f 7469 6d65 7374 616d 7073 5f6c  est_timestamps_l
-00015360: 6973 742c 0a20 2020 2020 2020 2065 7870  ist,.        exp
-00015370: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
-00015380: 2c0a 2020 2020 290a 0a0a 4070 7974 6573  ,.    )...@pytes
-00015390: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-000153a0: 7a65 280a 2020 2020 2274 6573 745f 7469  ze(.    "test_ti
-000153b0: 6d65 7374 616d 7073 2c20 7465 7374 5f74  mestamps, test_t
-000153c0: 696d 6573 7461 6d70 735f 6c69 7374 222c  imestamps_list",
-000153d0: 0a20 2020 205b 0a20 2020 2020 2020 2028  .    [.        (
-000153e0: 4e6f 6e65 2c20 4e6f 6e65 292c 0a20 2020  None, None),.   
-000153f0: 2020 2020 2028 5b43 5552 5245 4e54 5f54       ([CURRENT_T
-00015400: 494d 455d 202a 2032 2c20 5b43 5552 5245  IME] * 2, [CURRE
-00015410: 4e54 5f54 494d 455d 202a 2032 292c 0a20  NT_TIME] * 2),. 
-00015420: 2020 2020 2020 2028 6e70 2e61 7272 6179         (np.array
-00015430: 285b 4355 5252 454e 545f 5449 4d45 5d20  ([CURRENT_TIME] 
-00015440: 2a20 3229 2c20 5b43 5552 5245 4e54 5f54  * 2), [CURRENT_T
-00015450: 494d 455d 202a 2032 292c 0a20 2020 205d  IME] * 2),.    ]
-00015460: 2c0a 290a 4070 7974 6573 742e 6d61 726b  ,.).@pytest.mark
-00015470: 2e70 6172 616d 6574 7269 7a65 280a 2020  .parametrize(.  
-00015480: 2020 226b 7761 7267 7322 2c0a 2020 2020    "kwargs",.    
-00015490: 5b0a 2020 2020 2020 2020 7b22 6665 6564  [.        {"feed
-000154a0: 6261 636b 5f6b 6579 7322 3a20 5b22 4122  back_keys": ["A"
-000154b0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6665  ]},.        {"fe
-000154c0: 6564 6261 636b 5f69 6473 223a 205b 2231  edback_ids": ["1
-000154d0: 3233 3435 222c 2022 3637 3839 3022 5d7d  2345", "67890"]}
-000154e0: 2c0a 2020 2020 2020 2020 7b22 6a6f 696e  ,.        {"join
-000154f0: 5f6b 6579 7322 3a20 5b22 3534 3332 3122  _keys": ["54321"
-00015500: 2c20 2236 3738 3930 225d 7d2c 0a20 2020  , "67890"]},.   
-00015510: 2020 2020 207b 226a 6f69 6e5f 6b65 7973       {"join_keys
-00015520: 223a 2070 642e 5365 7269 6573 285b 2235  ": pd.Series(["5
-00015530: 3433 3231 222c 2022 3637 3839 3022 5d29  4321", "67890"])
-00015540: 7d2c 0a20 2020 205d 2c0a 290a 4070 7974  },.    ],.).@pyt
-00015550: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
-00015560: 7269 7a65 2822 7465 7374 5f66 6565 6462  rize("test_feedb
-00015570: 6163 6b73 222c 2054 4553 545f 4645 4544  acks", TEST_FEED
-00015580: 4241 434b 5329 0a40 7079 7465 7374 2e6d  BACKS).@pytest.m
-00015590: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
-000155a0: 2276 6572 7369 6f6e 222c 205b 4e6f 6e65  "version", [None
-000155b0: 2c20 3130 2c20 2231 2e32 2e33 225d 290a  , 10, "1.2.3"]).
-000155c0: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
-000155d0: 616d 6574 7269 7a65 2822 7461 6773 2c20  ametrize("tags, 
-000155e0: 726f 775f 7461 6773 2c20 676c 6f62 616c  row_tags, global
-000155f0: 5f74 6167 732c 2065 7870 6563 7465 645f  _tags, expected_
-00015600: 7461 6773 5f70 6172 616d 222c 2054 4553  tags_param", TES
-00015610: 545f 5441 4753 290a 406d 6f63 6b2e 7061  T_TAGS).@mock.pa
-00015620: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
-00015630: 6572 2e63 6c69 656e 742e 5f72 6573 6f6c  er.client._resol
-00015640: 7665 5f6a 6f69 6e5f 6b65 7973 222c 2072  ve_join_keys", r
-00015650: 6574 7572 6e5f 7661 6c75 653d 5b22 3132  eturn_value=["12
-00015660: 3334 3522 2c20 2235 3433 3231 225d 290a  345", "54321"]).
+00014d60: 6767 6572 2e63 6c69 656e 742e 5f72 6573  gger.client._res
+00014d70: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 222c  olve_join_keys",
+00014d80: 2072 6574 7572 6e5f 7661 6c75 653d 5b22   return_value=["
+00014d90: 3132 3334 3522 2c20 2235 3433 3231 225d  12345", "54321"]
+00014da0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+00014db0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+00014dc0: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
+00014dd0: 7072 6564 6963 7469 6f6e 5f61 6e64 5f66  prediction_and_f
+00014de0: 6565 6462 6163 6b5f 6576 656e 7473 2229  eedback_events")
+00014df0: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
+00014e00: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+00014e10: 6e74 2e47 616e 7472 792e 5f6c 6f67 5f70  nt.Gantry._log_p
+00014e20: 7265 6469 6374 696f 6e5f 6576 656e 7473  rediction_events
+00014e30: 2229 0a40 6d6f 636b 2e70 6174 6368 280a  ").@mock.patch(.
+00014e40: 2020 2020 2267 616e 7472 792e 6c6f 6767      "gantry.logg
+00014e50: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
+00014e60: 2e5f 6c6f 675f 6665 6564 6261 636b 5f65  ._log_feedback_e
+00014e70: 7665 6e74 7322 2c20 7265 7475 726e 5f76  vents", return_v
+00014e80: 616c 7565 3d28 4e6f 6e65 2c20 5b22 3132  alue=(None, ["12
+00014e90: 3334 3522 2c20 2236 3738 3930 225d 290a  345", "67890"]).
+00014ea0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+00014eb0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+00014ec0: 656e 742e 5f73 616d 706c 655f 7265 636f  ent._sample_reco
+00014ed0: 7264 7322 2c20 7369 6465 5f65 6666 6563  rds", side_effec
+00014ee0: 743d 636c 6965 6e74 2e5f 7361 6d70 6c65  t=client._sample
+00014ef0: 5f72 6563 6f72 6473 290a 6465 6620 7465  _records).def te
+00014f00: 7374 5f6c 6f67 5f72 6563 6f72 6473 5f66  st_log_records_f
+00014f10: 6565 6462 6163 6b5f 6f6e 6c79 280a 2020  eedback_only(.  
+00014f20: 2020 6d6f 636b 5f73 616d 706c 655f 7265    mock_sample_re
+00014f30: 636f 7264 732c 0a20 2020 206d 6f63 6b5f  cords,.    mock_
+00014f40: 6665 6564 6261 636b 2c0a 2020 2020 6d6f  feedback,.    mo
+00014f50: 636b 5f70 7265 6473 2c0a 2020 2020 6d6f  ck_preds,.    mo
+00014f60: 636b 5f70 7265 6473 5f61 6e64 5f66 6565  ck_preds_and_fee
+00014f70: 6462 6163 6b2c 0a20 2020 206d 6f63 6b5f  dback,.    mock_
+00014f80: 7265 736f 6c76 655f 6a6f 696e 5f6b 6579  resolve_join_key
+00014f90: 732c 0a20 2020 2076 6572 7369 6f6e 2c0a  s,.    version,.
+00014fa0: 2020 2020 7461 6773 2c0a 2020 2020 726f      tags,.    ro
+00014fb0: 775f 7461 6773 2c0a 2020 2020 676c 6f62  w_tags,.    glob
+00014fc0: 616c 5f74 6167 732c 0a20 2020 2065 7870  al_tags,.    exp
+00014fd0: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
+00014fe0: 2c0a 2020 2020 7465 7374 5f66 6565 6462  ,.    test_feedb
+00014ff0: 6163 6b73 2c0a 2020 2020 7465 7374 5f74  acks,.    test_t
+00015000: 696d 6573 7461 6d70 732c 0a20 2020 2074  imestamps,.    t
+00015010: 6573 745f 7469 6d65 7374 616d 7073 5f6c  est_timestamps_l
+00015020: 6973 742c 0a20 2020 206b 7761 7267 732c  ist,.    kwargs,
+00015030: 0a20 2020 2063 6c69 5f6f 626a 2c0a 293a  .    cli_obj,.):
+00015040: 0a20 2020 2061 7373 6572 7420 636c 695f  .    assert cli_
+00015050: 6f62 6a2e 6c6f 675f 7265 636f 7264 7328  obj.log_records(
+00015060: 0a20 2020 2020 2020 2061 7070 6c69 6361  .        applica
+00015070: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
+00015080: 2020 2020 2020 2076 6572 7369 6f6e 3d76         version=v
+00015090: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
+000150a0: 696e 7075 7473 3d4e 6f6e 652c 0a20 2020  inputs=None,.   
+000150b0: 2020 2020 206f 7574 7075 7473 3d4e 6f6e       outputs=Non
+000150c0: 652c 0a20 2020 2020 2020 2066 6565 6462  e,.        feedb
+000150d0: 6163 6b73 3d74 6573 745f 6665 6564 6261  acks=test_feedba
+000150e0: 636b 732c 0a20 2020 2020 2020 2074 696d  cks,.        tim
+000150f0: 6573 7461 6d70 733d 7465 7374 5f74 696d  estamps=test_tim
+00015100: 6573 7461 6d70 732c 0a20 2020 2020 2020  estamps,.       
+00015110: 2073 6f72 745f 6f6e 5f74 696d 6573 7461   sort_on_timesta
+00015120: 6d70 3d54 7275 652c 0a20 2020 2020 2020  mp=True,.       
+00015130: 2074 6167 733d 7461 6773 2c0a 2020 2020   tags=tags,.    
+00015140: 2020 2020 726f 775f 7461 6773 3d72 6f77      row_tags=row
+00015150: 5f74 6167 732c 0a20 2020 2020 2020 2067  _tags,.        g
+00015160: 6c6f 6261 6c5f 7461 6773 3d67 6c6f 6261  lobal_tags=globa
+00015170: 6c5f 7461 6773 2c0a 2020 2020 2020 2020  l_tags,.        
+00015180: 2a2a 6b77 6172 6773 2c0a 2020 2020 2920  **kwargs,.    ) 
+00015190: 3d3d 2028 4e6f 6e65 2c20 5b22 3132 3334  == (None, ["1234
+000151a0: 3522 2c20 2236 3738 3930 225d 290a 0a20  5", "67890"]).. 
+000151b0: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
+000151c0: 645f 6665 6564 6261 636b 2e61 7373 6572  d_feedback.asser
+000151d0: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
+000151e0: 2020 206d 6f63 6b5f 7072 6564 732e 6173     mock_preds.as
+000151f0: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
+00015200: 290a 2020 2020 6d6f 636b 5f66 6565 6462  ).    mock_feedb
+00015210: 6163 6b2e 6173 7365 7274 5f63 616c 6c65  ack.assert_calle
+00015220: 645f 6f6e 6365 5f77 6974 6828 0a20 2020  d_once_with(.   
+00015230: 2020 2020 2022 666f 6f62 6172 222c 0a20       "foobar",. 
+00015240: 2020 2020 2020 205b 7b22 4122 3a20 3230         [{"A": 20
+00015250: 307d 2c20 7b22 4122 3a20 3230 317d 5d2c  0}, {"A": 201}],
+00015260: 0a20 2020 2020 2020 205b 2231 3233 3435  .        ["12345
+00015270: 222c 2022 3534 3332 3122 5d2c 0a20 2020  ", "54321"],.   
+00015280: 2020 2020 2076 6572 7369 6f6e 2c0a 2020       version,.  
+00015290: 2020 2020 2020 7465 7374 5f74 696d 6573        test_times
+000152a0: 7461 6d70 735f 6c69 7374 2c0a 2020 2020  tamps_list,.    
+000152b0: 2020 2020 5472 7565 2c0a 2020 2020 2020      True,.      
+000152c0: 2020 4661 6c73 652c 0a20 2020 2020 2020    False,.       
+000152d0: 2065 7870 6563 7465 645f 7461 6773 5f70   expected_tags_p
+000152e0: 6172 616d 2c0a 2020 2020 290a 0a20 2020  aram,.    )..   
+000152f0: 206d 6f63 6b5f 7361 6d70 6c65 5f72 6563   mock_sample_rec
+00015300: 6f72 6473 2e61 7373 6572 745f 6361 6c6c  ords.assert_call
+00015310: 6564 5f6f 6e63 655f 7769 7468 280a 2020  ed_once_with(.  
+00015320: 2020 2020 2020 322c 0a20 2020 2020 2020        2,.       
+00015330: 2031 2c0a 2020 2020 2020 2020 4e6f 6e65   1,.        None
+00015340: 2c0a 2020 2020 2020 2020 4e6f 6e65 2c0a  ,.        None,.
+00015350: 2020 2020 2020 2020 5b7b 2241 223a 2032          [{"A": 2
+00015360: 3030 7d2c 207b 2241 223a 2032 3031 7d5d  00}, {"A": 201}]
+00015370: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
+00015380: 2e5f 7265 736f 6c76 655f 6a6f 696e 5f6b  ._resolve_join_k
+00015390: 6579 7328 2a2a 6b77 6172 6773 292c 0a20  eys(**kwargs),. 
+000153a0: 2020 2020 2020 2074 6573 745f 7469 6d65         test_time
+000153b0: 7374 616d 7073 5f6c 6973 742c 0a20 2020  stamps_list,.   
+000153c0: 2020 2020 2065 7870 6563 7465 645f 7461       expected_ta
+000153d0: 6773 5f70 6172 616d 2c0a 2020 2020 290a  gs_param,.    ).
+000153e0: 0a0a 4070 7974 6573 742e 6d61 726b 2e70  ..@pytest.mark.p
+000153f0: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
+00015400: 2274 6573 745f 7469 6d65 7374 616d 7073  "test_timestamps
+00015410: 2c20 7465 7374 5f74 696d 6573 7461 6d70  , test_timestamp
+00015420: 735f 6c69 7374 222c 0a20 2020 205b 0a20  s_list",.    [. 
+00015430: 2020 2020 2020 2028 4e6f 6e65 2c20 4e6f         (None, No
+00015440: 6e65 292c 0a20 2020 2020 2020 2028 5b43  ne),.        ([C
+00015450: 5552 5245 4e54 5f54 494d 455d 202a 2032  URRENT_TIME] * 2
+00015460: 2c20 5b43 5552 5245 4e54 5f54 494d 455d  , [CURRENT_TIME]
+00015470: 202a 2032 292c 0a20 2020 2020 2020 2028   * 2),.        (
+00015480: 6e70 2e61 7272 6179 285b 4355 5252 454e  np.array([CURREN
+00015490: 545f 5449 4d45 5d20 2a20 3229 2c20 5b43  T_TIME] * 2), [C
+000154a0: 5552 5245 4e54 5f54 494d 455d 202a 2032  URRENT_TIME] * 2
+000154b0: 292c 0a20 2020 205d 2c0a 290a 4070 7974  ),.    ],.).@pyt
+000154c0: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
+000154d0: 7269 7a65 280a 2020 2020 226b 7761 7267  rize(.    "kwarg
+000154e0: 7322 2c0a 2020 2020 5b0a 2020 2020 2020  s",.    [.      
+000154f0: 2020 7b22 6665 6564 6261 636b 5f6b 6579    {"feedback_key
+00015500: 7322 3a20 5b22 4122 5d7d 2c0a 2020 2020  s": ["A"]},.    
+00015510: 2020 2020 7b22 6665 6564 6261 636b 5f69      {"feedback_i
+00015520: 6473 223a 205b 2231 3233 3435 222c 2022  ds": ["12345", "
+00015530: 3637 3839 3022 5d7d 2c0a 2020 2020 2020  67890"]},.      
+00015540: 2020 7b22 6a6f 696e 5f6b 6579 7322 3a20    {"join_keys": 
+00015550: 5b22 3534 3332 3122 2c20 2236 3738 3930  ["54321", "67890
+00015560: 225d 7d2c 0a20 2020 2020 2020 207b 226a  "]},.        {"j
+00015570: 6f69 6e5f 6b65 7973 223a 2070 642e 5365  oin_keys": pd.Se
+00015580: 7269 6573 285b 2235 3433 3231 222c 2022  ries(["54321", "
+00015590: 3637 3839 3022 5d29 7d2c 0a20 2020 205d  67890"])},.    ]
+000155a0: 2c0a 290a 4070 7974 6573 742e 6d61 726b  ,.).@pytest.mark
+000155b0: 2e70 6172 616d 6574 7269 7a65 2822 7465  .parametrize("te
+000155c0: 7374 5f66 6565 6462 6163 6b73 222c 2054  st_feedbacks", T
+000155d0: 4553 545f 4645 4544 4241 434b 5329 0a40  EST_FEEDBACKS).@
+000155e0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+000155f0: 6d65 7472 697a 6528 2276 6572 7369 6f6e  metrize("version
+00015600: 222c 205b 4e6f 6e65 2c20 3130 2c20 2231  ", [None, 10, "1
+00015610: 2e32 2e33 225d 290a 4070 7974 6573 742e  .2.3"]).@pytest.
+00015620: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+00015630: 2822 7461 6773 2c20 726f 775f 7461 6773  ("tags, row_tags
+00015640: 2c20 676c 6f62 616c 5f74 6167 732c 2065  , global_tags, e
+00015650: 7870 6563 7465 645f 7461 6773 5f70 6172  xpected_tags_par
+00015660: 616d 222c 2054 4553 545f 5441 4753 290a  am", TEST_TAGS).
 00015670: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
 00015680: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-00015690: 742e 4761 6e74 7279 2e5f 6c6f 675f 7072  t.Gantry._log_pr
-000156a0: 6564 6963 7469 6f6e 5f61 6e64 5f66 6565  ediction_and_fee
-000156b0: 6462 6163 6b5f 6576 656e 7473 2229 0a40  dback_events").@
-000156c0: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
-000156d0: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
-000156e0: 2e47 616e 7472 792e 5f6c 6f67 5f70 7265  .Gantry._log_pre
-000156f0: 6469 6374 696f 6e5f 6576 656e 7473 2229  diction_events")
-00015700: 0a40 6d6f 636b 2e70 6174 6368 280a 2020  .@mock.patch(.  
-00015710: 2020 2267 616e 7472 792e 6c6f 6767 6572    "gantry.logger
-00015720: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-00015730: 6c6f 675f 6665 6564 6261 636b 5f65 7665  log_feedback_eve
-00015740: 6e74 7322 2c20 7265 7475 726e 5f76 616c  nts", return_val
-00015750: 7565 3d28 4e6f 6e65 2c20 5b22 3132 3334  ue=(None, ["1234
-00015760: 3522 2c20 2236 3738 3930 225d 290a 290a  5", "67890"]).).
-00015770: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
-00015780: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-00015790: 742e 5f73 616d 706c 655f 7265 636f 7264  t._sample_record
-000157a0: 7322 2c20 7369 6465 5f65 6666 6563 743d  s", side_effect=
-000157b0: 636c 6965 6e74 2e5f 7361 6d70 6c65 5f72  client._sample_r
-000157c0: 6563 6f72 6473 290a 6465 6620 7465 7374  ecords).def test
-000157d0: 5f73 696e 676c 655f 6c6f 675f 7265 636f  _single_log_reco
-000157e0: 7264 735f 6665 6564 6261 636b 5f6f 6e6c  rds_feedback_onl
-000157f0: 7928 0a20 2020 206d 6f63 6b5f 7361 6d70  y(.    mock_samp
-00015800: 6c65 5f72 6563 6f72 6473 2c0a 2020 2020  le_records,.    
-00015810: 6d6f 636b 5f66 6565 6462 6163 6b2c 0a20  mock_feedback,. 
-00015820: 2020 206d 6f63 6b5f 7072 6564 732c 0a20     mock_preds,. 
-00015830: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
-00015840: 645f 6665 6564 6261 636b 2c0a 2020 2020  d_feedback,.    
-00015850: 6d6f 636b 5f72 6573 6f6c 7665 5f6a 6f69  mock_resolve_joi
-00015860: 6e5f 6b65 7973 2c0a 2020 2020 7665 7273  n_keys,.    vers
-00015870: 696f 6e2c 0a20 2020 2074 6167 732c 0a20  ion,.    tags,. 
-00015880: 2020 2072 6f77 5f74 6167 732c 0a20 2020     row_tags,.   
-00015890: 2067 6c6f 6261 6c5f 7461 6773 2c0a 2020   global_tags,.  
-000158a0: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
-000158b0: 7061 7261 6d2c 0a20 2020 2074 6573 745f  param,.    test_
-000158c0: 6665 6564 6261 636b 732c 0a20 2020 2074  feedbacks,.    t
-000158d0: 6573 745f 7469 6d65 7374 616d 7073 2c0a  est_timestamps,.
-000158e0: 2020 2020 7465 7374 5f74 696d 6573 7461      test_timesta
-000158f0: 6d70 735f 6c69 7374 2c0a 2020 2020 6b77  mps_list,.    kw
-00015900: 6172 6773 2c0a 2020 2020 636c 695f 6f62  args,.    cli_ob
-00015910: 6a2c 0a29 3a0a 2020 2020 6173 7365 7274  j,.):.    assert
-00015920: 2063 6c69 5f6f 626a 2e73 696e 676c 655f   cli_obj.single_
-00015930: 6c6f 675f 7265 636f 7264 7328 0a20 2020  log_records(.   
-00015940: 2020 2020 2061 7070 6c69 6361 7469 6f6e       application
-00015950: 3d22 666f 6f62 6172 222c 0a20 2020 2020  ="foobar",.     
-00015960: 2020 2076 6572 7369 6f6e 3d76 6572 7369     version=versi
-00015970: 6f6e 2c0a 2020 2020 2020 2020 696e 7075  on,.        inpu
-00015980: 7473 3d4e 6f6e 652c 0a20 2020 2020 2020  ts=None,.       
-00015990: 206f 7574 7075 7473 3d4e 6f6e 652c 0a20   outputs=None,. 
-000159a0: 2020 2020 2020 2066 6565 6462 6163 6b73         feedbacks
-000159b0: 3d74 6573 745f 6665 6564 6261 636b 732c  =test_feedbacks,
-000159c0: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
-000159d0: 6d70 733d 7465 7374 5f74 696d 6573 7461  mps=test_timesta
-000159e0: 6d70 732c 0a20 2020 2020 2020 2073 6f72  mps,.        sor
-000159f0: 745f 6f6e 5f74 696d 6573 7461 6d70 3d54  t_on_timestamp=T
-00015a00: 7275 652c 0a20 2020 2020 2020 2074 6167  rue,.        tag
-00015a10: 733d 7461 6773 2c0a 2020 2020 2020 2020  s=tags,.        
-00015a20: 726f 775f 7461 6773 3d72 6f77 5f74 6167  row_tags=row_tag
-00015a30: 732c 0a20 2020 2020 2020 2067 6c6f 6261  s,.        globa
-00015a40: 6c5f 7461 6773 3d67 6c6f 6261 6c5f 7461  l_tags=global_ta
-00015a50: 6773 2c0a 2020 2020 2020 2020 2a2a 6b77  gs,.        **kw
-00015a60: 6172 6773 2c0a 2020 2020 2920 3d3d 2028  args,.    ) == (
-00015a70: 4e6f 6e65 2c20 5b22 3132 3334 3522 2c20  None, ["12345", 
-00015a80: 2236 3738 3930 225d 290a 0a20 2020 206d  "67890"])..    m
-00015a90: 6f63 6b5f 7072 6564 735f 616e 645f 6665  ock_preds_and_fe
-00015aa0: 6564 6261 636b 2e61 7373 6572 745f 6e6f  edback.assert_no
-00015ab0: 745f 6361 6c6c 6564 2829 0a20 2020 206d  t_called().    m
-00015ac0: 6f63 6b5f 7072 6564 732e 6173 7365 7274  ock_preds.assert
-00015ad0: 5f6e 6f74 5f63 616c 6c65 6428 290a 2020  _not_called().  
-00015ae0: 2020 6d6f 636b 5f66 6565 6462 6163 6b2e    mock_feedback.
-00015af0: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
-00015b00: 6365 5f77 6974 6828 0a20 2020 2020 2020  ce_with(.       
-00015b10: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
-00015b20: 6f62 6172 222c 0a20 2020 2020 2020 2066  obar",.        f
-00015b30: 6565 6462 6163 6b73 3d5b 7b22 4122 3a20  eedbacks=[{"A": 
-00015b40: 3230 307d 2c20 7b22 4122 3a20 3230 317d  200}, {"A": 201}
-00015b50: 5d2c 0a20 2020 2020 2020 206a 6f69 6e5f  ],.        join_
-00015b60: 6b65 7973 3d5b 2231 3233 3435 222c 2022  keys=["12345", "
-00015b70: 3534 3332 3122 5d2c 0a20 2020 2020 2020  54321"],.       
-00015b80: 2066 6565 6462 6163 6b5f 7665 7273 696f   feedback_versio
-00015b90: 6e3d 7665 7273 696f 6e2c 0a20 2020 2020  n=version,.     
-00015ba0: 2020 2074 696d 6573 7461 6d70 733d 7465     timestamps=te
-00015bb0: 7374 5f74 696d 6573 7461 6d70 735f 6c69  st_timestamps_li
-00015bc0: 7374 2c0a 2020 2020 2020 2020 736f 7274  st,.        sort
-00015bd0: 5f6f 6e5f 7469 6d65 7374 616d 703d 5472  _on_timestamp=Tr
-00015be0: 7565 2c0a 2020 2020 2020 2020 6173 5f62  ue,.        as_b
-00015bf0: 6174 6368 3d46 616c 7365 2c0a 2020 2020  atch=False,.    
-00015c00: 2020 2020 7461 6773 3d65 7870 6563 7465      tags=expecte
-00015c10: 645f 7461 6773 5f70 6172 616d 2c0a 2020  d_tags_param,.  
-00015c20: 2020 290a 0a20 2020 206d 6f63 6b5f 7361    )..    mock_sa
-00015c30: 6d70 6c65 5f72 6563 6f72 6473 2e61 7373  mple_records.ass
-00015c40: 6572 745f 6361 6c6c 6564 5f6f 6e63 655f  ert_called_once_
-00015c50: 7769 7468 280a 2020 2020 2020 2020 322c  with(.        2,
-00015c60: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
-00015c70: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
-00015c80: 2020 4e6f 6e65 2c0a 2020 2020 2020 2020    None,.        
-00015c90: 5b7b 2241 223a 2032 3030 7d2c 207b 2241  [{"A": 200}, {"A
-00015ca0: 223a 2032 3031 7d5d 2c0a 2020 2020 2020  ": 201}],.      
-00015cb0: 2020 636c 6965 6e74 2e5f 7265 736f 6c76    client._resolv
-00015cc0: 655f 6a6f 696e 5f6b 6579 7328 2a2a 6b77  e_join_keys(**kw
-00015cd0: 6172 6773 292c 0a20 2020 2020 2020 2074  args),.        t
-00015ce0: 6573 745f 7469 6d65 7374 616d 7073 5f6c  est_timestamps_l
-00015cf0: 6973 742c 0a20 2020 2020 2020 2065 7870  ist,.        exp
-00015d00: 6563 7465 645f 7461 6773 5f70 6172 616d  ected_tags_param
-00015d10: 2c0a 2020 2020 290a 0a0a 4070 7974 6573  ,.    )...@pytes
-00015d20: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00015d30: 7a65 280a 2020 2020 2274 6573 745f 7469  ze(.    "test_ti
-00015d40: 6d65 7374 616d 7073 2c20 7465 7374 5f74  mestamps, test_t
-00015d50: 696d 6573 7461 6d70 735f 6c69 7374 222c  imestamps_list",
-00015d60: 0a20 2020 205b 0a20 2020 2020 2020 2028  .    [.        (
-00015d70: 4e6f 6e65 2c20 4e6f 6e65 292c 0a20 2020  None, None),.   
-00015d80: 2020 2020 2028 5b43 5552 5245 4e54 5f54       ([CURRENT_T
-00015d90: 494d 455d 202a 2032 2c20 5b43 5552 5245  IME] * 2, [CURRE
-00015da0: 4e54 5f54 494d 455d 202a 2032 292c 0a20  NT_TIME] * 2),. 
-00015db0: 2020 2020 2020 2028 6e70 2e61 7272 6179         (np.array
-00015dc0: 285b 4355 5252 454e 545f 5449 4d45 5d20  ([CURRENT_TIME] 
-00015dd0: 2a20 3229 2c20 5b43 5552 5245 4e54 5f54  * 2), [CURRENT_T
-00015de0: 494d 455d 202a 2032 292c 0a20 2020 205d  IME] * 2),.    ]
-00015df0: 2c0a 290a 4070 7974 6573 742e 6d61 726b  ,.).@pytest.mark
-00015e00: 2e70 6172 616d 6574 7269 7a65 280a 2020  .parametrize(.  
-00015e10: 2020 226b 7761 7267 7322 2c0a 2020 2020    "kwargs",.    
-00015e20: 5b0a 2020 2020 2020 2020 7b22 6a6f 696e  [.        {"join
-00015e30: 5f6b 6579 7322 3a20 5b22 3534 3332 3122  _keys": ["54321"
-00015e40: 2c20 2236 3738 3930 225d 7d2c 0a20 2020  , "67890"]},.   
-00015e50: 2020 2020 207b 226a 6f69 6e5f 6b65 7973       {"join_keys
-00015e60: 223a 2070 642e 5365 7269 6573 285b 2235  ": pd.Series(["5
-00015e70: 3433 3231 222c 2022 3637 3839 3022 5d29  4321", "67890"])
-00015e80: 7d2c 0a20 2020 205d 2c0a 290a 4070 7974  },.    ],.).@pyt
-00015e90: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
-00015ea0: 7269 7a65 2822 7465 7374 5f66 6565 6462  rize("test_feedb
-00015eb0: 6163 6b73 222c 2054 4553 545f 4645 4544  acks", TEST_FEED
-00015ec0: 4241 434b 5329 0a40 7079 7465 7374 2e6d  BACKS).@pytest.m
-00015ed0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
-00015ee0: 2276 6572 7369 6f6e 222c 205b 4e6f 6e65  "version", [None
-00015ef0: 2c20 3130 2c20 2231 2e32 2e33 225d 290a  , 10, "1.2.3"]).
-00015f00: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
-00015f10: 616d 6574 7269 7a65 2822 7461 6773 2c20  ametrize("tags, 
-00015f20: 726f 775f 7461 6773 2c20 676c 6f62 616c  row_tags, global
-00015f30: 5f74 6167 732c 2065 7870 6563 7465 645f  _tags, expected_
-00015f40: 7461 6773 5f70 6172 616d 222c 2054 4553  tags_param", TES
-00015f50: 545f 5441 4753 290a 406d 6f63 6b2e 7061  T_TAGS).@mock.pa
-00015f60: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
-00015f70: 6572 2e63 6c69 656e 742e 5f72 6573 6f6c  er.client._resol
-00015f80: 7665 5f6a 6f69 6e5f 6b65 7973 222c 2072  ve_join_keys", r
-00015f90: 6574 7572 6e5f 7661 6c75 653d 5b22 3132  eturn_value=["12
-00015fa0: 3334 3522 2c20 2235 3433 3231 225d 290a  345", "54321"]).
+00015690: 742e 5f72 6573 6f6c 7665 5f6a 6f69 6e5f  t._resolve_join_
+000156a0: 6b65 7973 222c 2072 6574 7572 6e5f 7661  keys", return_va
+000156b0: 6c75 653d 5b22 3132 3334 3522 2c20 2235  lue=["12345", "5
+000156c0: 3433 3231 225d 290a 406d 6f63 6b2e 7061  4321"]).@mock.pa
+000156d0: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
+000156e0: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
+000156f0: 2e5f 6c6f 675f 7072 6564 6963 7469 6f6e  ._log_prediction
+00015700: 5f61 6e64 5f66 6565 6462 6163 6b5f 6576  _and_feedback_ev
+00015710: 656e 7473 2229 0a40 6d6f 636b 2e70 6174  ents").@mock.pat
+00015720: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
+00015730: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
+00015740: 5f6c 6f67 5f70 7265 6469 6374 696f 6e5f  _log_prediction_
+00015750: 6576 656e 7473 2229 0a40 6d6f 636b 2e70  events").@mock.p
+00015760: 6174 6368 280a 2020 2020 2267 616e 7472  atch(.    "gantr
+00015770: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+00015780: 4761 6e74 7279 2e5f 6c6f 675f 6665 6564  Gantry._log_feed
+00015790: 6261 636b 5f65 7665 6e74 7322 2c20 7265  back_events", re
+000157a0: 7475 726e 5f76 616c 7565 3d28 4e6f 6e65  turn_value=(None
+000157b0: 2c20 5b22 3132 3334 3522 2c20 2236 3738  , ["12345", "678
+000157c0: 3930 225d 290a 290a 406d 6f63 6b2e 7061  90"]).).@mock.pa
+000157d0: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
+000157e0: 6572 2e63 6c69 656e 742e 5f73 616d 706c  er.client._sampl
+000157f0: 655f 7265 636f 7264 7322 2c20 7369 6465  e_records", side
+00015800: 5f65 6666 6563 743d 636c 6965 6e74 2e5f  _effect=client._
+00015810: 7361 6d70 6c65 5f72 6563 6f72 6473 290a  sample_records).
+00015820: 6465 6620 7465 7374 5f73 696e 676c 655f  def test_single_
+00015830: 6c6f 675f 7265 636f 7264 735f 6665 6564  log_records_feed
+00015840: 6261 636b 5f6f 6e6c 7928 0a20 2020 206d  back_only(.    m
+00015850: 6f63 6b5f 7361 6d70 6c65 5f72 6563 6f72  ock_sample_recor
+00015860: 6473 2c0a 2020 2020 6d6f 636b 5f66 6565  ds,.    mock_fee
+00015870: 6462 6163 6b2c 0a20 2020 206d 6f63 6b5f  dback,.    mock_
+00015880: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
+00015890: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+000158a0: 636b 2c0a 2020 2020 6d6f 636b 5f72 6573  ck,.    mock_res
+000158b0: 6f6c 7665 5f6a 6f69 6e5f 6b65 7973 2c0a  olve_join_keys,.
+000158c0: 2020 2020 7665 7273 696f 6e2c 0a20 2020      version,.   
+000158d0: 2074 6167 732c 0a20 2020 2072 6f77 5f74   tags,.    row_t
+000158e0: 6167 732c 0a20 2020 2067 6c6f 6261 6c5f  ags,.    global_
+000158f0: 7461 6773 2c0a 2020 2020 6578 7065 6374  tags,.    expect
+00015900: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
+00015910: 2020 2074 6573 745f 6665 6564 6261 636b     test_feedback
+00015920: 732c 0a20 2020 2074 6573 745f 7469 6d65  s,.    test_time
+00015930: 7374 616d 7073 2c0a 2020 2020 7465 7374  stamps,.    test
+00015940: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
+00015950: 2c0a 2020 2020 6b77 6172 6773 2c0a 2020  ,.    kwargs,.  
+00015960: 2020 636c 695f 6f62 6a2c 0a29 3a0a 2020    cli_obj,.):.  
+00015970: 2020 6173 7365 7274 2063 6c69 5f6f 626a    assert cli_obj
+00015980: 2e73 696e 676c 655f 6c6f 675f 7265 636f  .single_log_reco
+00015990: 7264 7328 0a20 2020 2020 2020 2061 7070  rds(.        app
+000159a0: 6c69 6361 7469 6f6e 3d22 666f 6f62 6172  lication="foobar
+000159b0: 222c 0a20 2020 2020 2020 2076 6572 7369  ",.        versi
+000159c0: 6f6e 3d76 6572 7369 6f6e 2c0a 2020 2020  on=version,.    
+000159d0: 2020 2020 696e 7075 7473 3d4e 6f6e 652c      inputs=None,
+000159e0: 0a20 2020 2020 2020 206f 7574 7075 7473  .        outputs
+000159f0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2066  =None,.        f
+00015a00: 6565 6462 6163 6b73 3d74 6573 745f 6665  eedbacks=test_fe
+00015a10: 6564 6261 636b 732c 0a20 2020 2020 2020  edbacks,.       
+00015a20: 2074 696d 6573 7461 6d70 733d 7465 7374   timestamps=test
+00015a30: 5f74 696d 6573 7461 6d70 732c 0a20 2020  _timestamps,.   
+00015a40: 2020 2020 2073 6f72 745f 6f6e 5f74 696d       sort_on_tim
+00015a50: 6573 7461 6d70 3d54 7275 652c 0a20 2020  estamp=True,.   
+00015a60: 2020 2020 2074 6167 733d 7461 6773 2c0a       tags=tags,.
+00015a70: 2020 2020 2020 2020 726f 775f 7461 6773          row_tags
+00015a80: 3d72 6f77 5f74 6167 732c 0a20 2020 2020  =row_tags,.     
+00015a90: 2020 2067 6c6f 6261 6c5f 7461 6773 3d67     global_tags=g
+00015aa0: 6c6f 6261 6c5f 7461 6773 2c0a 2020 2020  lobal_tags,.    
+00015ab0: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
+00015ac0: 2020 2920 3d3d 2028 4e6f 6e65 2c20 5b22    ) == (None, ["
+00015ad0: 3132 3334 3522 2c20 2236 3738 3930 225d  12345", "67890"]
+00015ae0: 290a 0a20 2020 206d 6f63 6b5f 7072 6564  )..    mock_pred
+00015af0: 735f 616e 645f 6665 6564 6261 636b 2e61  s_and_feedback.a
+00015b00: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
+00015b10: 2829 0a20 2020 206d 6f63 6b5f 7072 6564  ().    mock_pred
+00015b20: 732e 6173 7365 7274 5f6e 6f74 5f63 616c  s.assert_not_cal
+00015b30: 6c65 6428 290a 2020 2020 6d6f 636b 5f66  led().    mock_f
+00015b40: 6565 6462 6163 6b2e 6173 7365 7274 5f63  eedback.assert_c
+00015b50: 616c 6c65 645f 6f6e 6365 5f77 6974 6828  alled_once_with(
+00015b60: 0a20 2020 2020 2020 2061 7070 6c69 6361  .        applica
+00015b70: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
+00015b80: 2020 2020 2020 2066 6565 6462 6163 6b73         feedbacks
+00015b90: 3d5b 7b22 4122 3a20 3230 307d 2c20 7b22  =[{"A": 200}, {"
+00015ba0: 4122 3a20 3230 317d 5d2c 0a20 2020 2020  A": 201}],.     
+00015bb0: 2020 206a 6f69 6e5f 6b65 7973 3d5b 2231     join_keys=["1
+00015bc0: 3233 3435 222c 2022 3534 3332 3122 5d2c  2345", "54321"],
+00015bd0: 0a20 2020 2020 2020 2066 6565 6462 6163  .        feedbac
+00015be0: 6b5f 7665 7273 696f 6e3d 7665 7273 696f  k_version=versio
+00015bf0: 6e2c 0a20 2020 2020 2020 2074 696d 6573  n,.        times
+00015c00: 7461 6d70 733d 7465 7374 5f74 696d 6573  tamps=test_times
+00015c10: 7461 6d70 735f 6c69 7374 2c0a 2020 2020  tamps_list,.    
+00015c20: 2020 2020 736f 7274 5f6f 6e5f 7469 6d65      sort_on_time
+00015c30: 7374 616d 703d 5472 7565 2c0a 2020 2020  stamp=True,.    
+00015c40: 2020 2020 6173 5f62 6174 6368 3d46 616c      as_batch=Fal
+00015c50: 7365 2c0a 2020 2020 2020 2020 7461 6773  se,.        tags
+00015c60: 3d65 7870 6563 7465 645f 7461 6773 5f70  =expected_tags_p
+00015c70: 6172 616d 2c0a 2020 2020 290a 0a20 2020  aram,.    )..   
+00015c80: 206d 6f63 6b5f 7361 6d70 6c65 5f72 6563   mock_sample_rec
+00015c90: 6f72 6473 2e61 7373 6572 745f 6361 6c6c  ords.assert_call
+00015ca0: 6564 5f6f 6e63 655f 7769 7468 280a 2020  ed_once_with(.  
+00015cb0: 2020 2020 2020 322c 0a20 2020 2020 2020        2,.       
+00015cc0: 2031 2c0a 2020 2020 2020 2020 4e6f 6e65   1,.        None
+00015cd0: 2c0a 2020 2020 2020 2020 4e6f 6e65 2c0a  ,.        None,.
+00015ce0: 2020 2020 2020 2020 5b7b 2241 223a 2032          [{"A": 2
+00015cf0: 3030 7d2c 207b 2241 223a 2032 3031 7d5d  00}, {"A": 201}]
+00015d00: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
+00015d10: 2e5f 7265 736f 6c76 655f 6a6f 696e 5f6b  ._resolve_join_k
+00015d20: 6579 7328 2a2a 6b77 6172 6773 292c 0a20  eys(**kwargs),. 
+00015d30: 2020 2020 2020 2074 6573 745f 7469 6d65         test_time
+00015d40: 7374 616d 7073 5f6c 6973 742c 0a20 2020  stamps_list,.   
+00015d50: 2020 2020 2065 7870 6563 7465 645f 7461       expected_ta
+00015d60: 6773 5f70 6172 616d 2c0a 2020 2020 290a  gs_param,.    ).
+00015d70: 0a0a 4070 7974 6573 742e 6d61 726b 2e70  ..@pytest.mark.p
+00015d80: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
+00015d90: 2274 6573 745f 7469 6d65 7374 616d 7073  "test_timestamps
+00015da0: 2c20 7465 7374 5f74 696d 6573 7461 6d70  , test_timestamp
+00015db0: 735f 6c69 7374 222c 0a20 2020 205b 0a20  s_list",.    [. 
+00015dc0: 2020 2020 2020 2028 4e6f 6e65 2c20 4e6f         (None, No
+00015dd0: 6e65 292c 0a20 2020 2020 2020 2028 5b43  ne),.        ([C
+00015de0: 5552 5245 4e54 5f54 494d 455d 202a 2032  URRENT_TIME] * 2
+00015df0: 2c20 5b43 5552 5245 4e54 5f54 494d 455d  , [CURRENT_TIME]
+00015e00: 202a 2032 292c 0a20 2020 2020 2020 2028   * 2),.        (
+00015e10: 6e70 2e61 7272 6179 285b 4355 5252 454e  np.array([CURREN
+00015e20: 545f 5449 4d45 5d20 2a20 3229 2c20 5b43  T_TIME] * 2), [C
+00015e30: 5552 5245 4e54 5f54 494d 455d 202a 2032  URRENT_TIME] * 2
+00015e40: 292c 0a20 2020 205d 2c0a 290a 4070 7974  ),.    ],.).@pyt
+00015e50: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
+00015e60: 7269 7a65 280a 2020 2020 226b 7761 7267  rize(.    "kwarg
+00015e70: 7322 2c0a 2020 2020 5b0a 2020 2020 2020  s",.    [.      
+00015e80: 2020 7b22 6a6f 696e 5f6b 6579 7322 3a20    {"join_keys": 
+00015e90: 5b22 3534 3332 3122 2c20 2236 3738 3930  ["54321", "67890
+00015ea0: 225d 7d2c 0a20 2020 2020 2020 207b 226a  "]},.        {"j
+00015eb0: 6f69 6e5f 6b65 7973 223a 2070 642e 5365  oin_keys": pd.Se
+00015ec0: 7269 6573 285b 2235 3433 3231 222c 2022  ries(["54321", "
+00015ed0: 3637 3839 3022 5d29 7d2c 0a20 2020 205d  67890"])},.    ]
+00015ee0: 2c0a 290a 4070 7974 6573 742e 6d61 726b  ,.).@pytest.mark
+00015ef0: 2e70 6172 616d 6574 7269 7a65 2822 7465  .parametrize("te
+00015f00: 7374 5f66 6565 6462 6163 6b73 222c 2054  st_feedbacks", T
+00015f10: 4553 545f 4645 4544 4241 434b 5329 0a40  EST_FEEDBACKS).@
+00015f20: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+00015f30: 6d65 7472 697a 6528 2276 6572 7369 6f6e  metrize("version
+00015f40: 222c 205b 4e6f 6e65 2c20 3130 2c20 2231  ", [None, 10, "1
+00015f50: 2e32 2e33 225d 290a 4070 7974 6573 742e  .2.3"]).@pytest.
+00015f60: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+00015f70: 2822 7461 6773 2c20 726f 775f 7461 6773  ("tags, row_tags
+00015f80: 2c20 676c 6f62 616c 5f74 6167 732c 2065  , global_tags, e
+00015f90: 7870 6563 7465 645f 7461 6773 5f70 6172  xpected_tags_par
+00015fa0: 616d 222c 2054 4553 545f 5441 4753 290a  am", TEST_TAGS).
 00015fb0: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
 00015fc0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-00015fd0: 742e 4761 6e74 7279 2e5f 6765 6e65 7261  t.Gantry._genera
-00015fe0: 7465 5f70 7265 6469 6374 696f 6e5f 616e  te_prediction_an
-00015ff0: 645f 6665 6564 6261 636b 5f65 7665 6e74  d_feedback_event
-00016000: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
-00016010: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
-00016020: 6c69 656e 742e 4761 6e74 7279 2e5f 6765  lient.Gantry._ge
-00016030: 6e65 7261 7465 5f70 7265 6469 6374 696f  nerate_predictio
-00016040: 6e5f 6576 656e 7473 2229 0a40 6d6f 636b  n_events").@mock
-00016050: 2e70 6174 6368 280a 2020 2020 2267 616e  .patch(.    "gan
-00016060: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
-00016070: 742e 4761 6e74 7279 2e5f 6765 6e65 7261  t.Gantry._genera
-00016080: 7465 5f66 6565 6462 6163 6b5f 6576 656e  te_feedback_even
-00016090: 7473 222c 0a20 2020 2072 6574 7572 6e5f  ts",.    return_
-000160a0: 7661 6c75 653d 285b 7b22 6576 656e 7422  value=([{"event"
-000160b0: 3a20 2270 6c61 6365 5f68 6f6c 6465 7222  : "place_holder"
-000160c0: 7d5d 2c20 5b22 3132 3334 3522 2c20 2236  }], ["12345", "6
-000160d0: 3738 3930 225d 292c 0a29 0a40 6d6f 636b  7890"]),.).@mock
-000160e0: 2e70 6174 6368 2822 6761 6e74 7279 2e6c  .patch("gantry.l
-000160f0: 6f67 6765 722e 636c 6965 6e74 2e5f 7361  ogger.client._sa
-00016100: 6d70 6c65 5f72 6563 6f72 6473 222c 2073  mple_records", s
-00016110: 6964 655f 6566 6665 6374 3d63 6c69 656e  ide_effect=clien
-00016120: 742e 5f73 616d 706c 655f 7265 636f 7264  t._sample_record
-00016130: 7329 0a64 6566 2074 6573 745f 6765 6e65  s).def test_gene
-00016140: 7261 7465 5f72 6563 6f72 6473 5f66 6565  rate_records_fee
-00016150: 6462 6163 6b5f 6f6e 6c79 280a 2020 2020  dback_only(.    
-00016160: 6d6f 636b 5f73 616d 706c 655f 7265 636f  mock_sample_reco
-00016170: 7264 732c 0a20 2020 206d 6f63 6b5f 6765  rds,.    mock_ge
-00016180: 6e65 7261 7465 5f66 6565 6462 6163 6b2c  nerate_feedback,
-00016190: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
-000161a0: 7465 5f70 7265 6473 2c0a 2020 2020 6d6f  te_preds,.    mo
-000161b0: 636b 5f67 656e 6572 6174 655f 7072 6564  ck_generate_pred
-000161c0: 735f 616e 645f 6665 6564 6261 636b 2c0a  s_and_feedback,.
-000161d0: 2020 2020 6d6f 636b 5f72 6573 6f6c 7665      mock_resolve
-000161e0: 5f6a 6f69 6e5f 6b65 7973 2c0a 2020 2020  _join_keys,.    
-000161f0: 7665 7273 696f 6e2c 0a20 2020 2074 6167  version,.    tag
-00016200: 732c 0a20 2020 2072 6f77 5f74 6167 732c  s,.    row_tags,
-00016210: 0a20 2020 2067 6c6f 6261 6c5f 7461 6773  .    global_tags
-00016220: 2c0a 2020 2020 6578 7065 6374 6564 5f74  ,.    expected_t
-00016230: 6167 735f 7061 7261 6d2c 0a20 2020 2074  ags_param,.    t
-00016240: 6573 745f 6665 6564 6261 636b 732c 0a20  est_feedbacks,. 
-00016250: 2020 2074 6573 745f 7469 6d65 7374 616d     test_timestam
-00016260: 7073 2c0a 2020 2020 7465 7374 5f74 696d  ps,.    test_tim
-00016270: 6573 7461 6d70 735f 6c69 7374 2c0a 2020  estamps_list,.  
-00016280: 2020 6b77 6172 6773 2c0a 2020 2020 636c    kwargs,.    cl
-00016290: 695f 6f62 6a2c 0a29 3a0a 2020 2020 6966  i_obj,.):.    if
-000162a0: 2069 7369 6e73 7461 6e63 6528 7461 6773   isinstance(tags
-000162b0: 2c20 6c69 7374 293a 0a20 2020 2020 2020  , list):.       
-000162c0: 2070 7974 6573 742e 736b 6970 2822 5468   pytest.skip("Th
-000162d0: 6973 2074 6573 7420 6973 206e 6f74 2061  is test is not a
-000162e0: 7070 6c69 6361 626c 6520 746f 206c 6973  pplicable to lis
-000162f0: 7420 7461 6773 2229 0a0a 2020 2020 7275  t tags")..    ru
-00016300: 6e5f 6964 203d 2073 7472 2875 7569 642e  n_id = str(uuid.
-00016310: 7575 6964 3428 2929 0a20 2020 2072 756e  uuid4()).    run
-00016320: 5f74 6167 7320 3d20 4e6f 6e65 0a20 2020  _tags = None.   
-00016330: 2069 6620 7461 6773 2061 6e64 2067 6c6f   if tags and glo
-00016340: 6261 6c5f 7461 6773 3a0a 2020 2020 2020  bal_tags:.      
-00016350: 2020 7275 6e5f 7461 6773 203d 207b 2a2a    run_tags = {**
-00016360: 7461 6773 2c20 2a2a 676c 6f62 616c 5f74  tags, **global_t
-00016370: 6167 737d 0a20 2020 2065 6c69 6620 7461  ags}.    elif ta
-00016380: 6773 3a0a 2020 2020 2020 2020 7275 6e5f  gs:.        run_
-00016390: 7461 6773 203d 2074 6167 730a 2020 2020  tags = tags.    
-000163a0: 656c 6966 2067 6c6f 6261 6c5f 7461 6773  elif global_tags
-000163b0: 3a0a 2020 2020 2020 2020 7275 6e5f 7461  :.        run_ta
-000163c0: 6773 203d 2067 6c6f 6261 6c5f 7461 6773  gs = global_tags
-000163d0: 0a20 2020 2061 7373 6572 7420 636c 695f  .    assert cli_
-000163e0: 6f62 6a2e 6c6f 6728 0a20 2020 2020 2020  obj.log(.       
-000163f0: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
-00016400: 6f62 6172 222c 0a20 2020 2020 2020 2076  obar",.        v
-00016410: 6572 7369 6f6e 3d76 6572 7369 6f6e 2c0a  ersion=version,.
-00016420: 2020 2020 2020 2020 696e 7075 7473 3d4e          inputs=N
-00016430: 6f6e 652c 0a20 2020 2020 2020 206f 7574  one,.        out
-00016440: 7075 7473 3d4e 6f6e 652c 0a20 2020 2020  puts=None,.     
-00016450: 2020 2066 6565 6462 6163 6b73 3d74 6573     feedbacks=tes
-00016460: 745f 6665 6564 6261 636b 732c 0a20 2020  t_feedbacks,.   
-00016470: 2020 2020 2074 696d 6573 7461 6d70 733d       timestamps=
-00016480: 7465 7374 5f74 696d 6573 7461 6d70 732c  test_timestamps,
-00016490: 0a20 2020 2020 2020 2073 6f72 745f 6f6e  .        sort_on
-000164a0: 5f74 696d 6573 7461 6d70 3d54 7275 652c  _timestamp=True,
-000164b0: 0a20 2020 2020 2020 2072 6f77 5f74 6167  .        row_tag
-000164c0: 733d 726f 775f 7461 6773 2c0a 2020 2020  s=row_tags,.    
-000164d0: 2020 2020 7275 6e5f 7461 6773 3d72 756e      run_tags=run
-000164e0: 5f74 6167 732c 0a20 2020 2020 2020 2072  _tags,.        r
-000164f0: 756e 5f69 643d 7275 6e5f 6964 2c0a 2020  un_id=run_id,.  
-00016500: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
-00016510: 2020 2020 2920 3d3d 205b 7b22 6576 656e      ) == [{"even
-00016520: 7422 3a20 2270 6c61 6365 5f68 6f6c 6465  t": "place_holde
-00016530: 7222 7d5d 0a0a 2020 2020 6d6f 636b 5f67  r"}]..    mock_g
-00016540: 656e 6572 6174 655f 7072 6564 735f 616e  enerate_preds_an
-00016550: 645f 6665 6564 6261 636b 2e61 7373 6572  d_feedback.asser
-00016560: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
-00016570: 2020 206d 6f63 6b5f 6765 6e65 7261 7465     mock_generate
-00016580: 5f70 7265 6473 2e61 7373 6572 745f 6e6f  _preds.assert_no
-00016590: 745f 6361 6c6c 6564 2829 0a20 2020 206d  t_called().    m
-000165a0: 6f63 6b5f 6765 6e65 7261 7465 5f66 6565  ock_generate_fee
-000165b0: 6462 6163 6b2e 6173 7365 7274 5f63 616c  dback.assert_cal
-000165c0: 6c65 645f 6f6e 6365 5f77 6974 6828 0a20  led_once_with(. 
-000165d0: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
-000165e0: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
-000165f0: 2020 2020 2066 6565 6462 6163 6b73 3d5b       feedbacks=[
-00016600: 7b22 4122 3a20 3230 307d 2c20 7b22 4122  {"A": 200}, {"A"
-00016610: 3a20 3230 317d 5d2c 0a20 2020 2020 2020  : 201}],.       
-00016620: 206a 6f69 6e5f 6b65 7973 3d5b 2231 3233   join_keys=["123
-00016630: 3435 222c 2022 3534 3332 3122 5d2c 0a20  45", "54321"],. 
-00016640: 2020 2020 2020 2066 6565 6462 6163 6b5f         feedback_
-00016650: 7665 7273 696f 6e3d 7665 7273 696f 6e2c  version=version,
-00016660: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
-00016670: 6d70 733d 7465 7374 5f74 696d 6573 7461  mps=test_timesta
-00016680: 6d70 735f 6c69 7374 2c0a 2020 2020 2020  mps_list,.      
-00016690: 2020 736f 7274 5f6f 6e5f 7469 6d65 7374    sort_on_timest
-000166a0: 616d 703d 5472 7565 2c0a 2020 2020 2020  amp=True,.      
-000166b0: 2020 7275 6e5f 6964 3d72 756e 5f69 642c    run_id=run_id,
-000166c0: 0a20 2020 2020 2020 2074 6167 733d 6578  .        tags=ex
-000166d0: 7065 6374 6564 5f74 6167 735f 7061 7261  pected_tags_para
-000166e0: 6d2c 0a20 2020 2029 0a0a 2020 2020 6d6f  m,.    )..    mo
-000166f0: 636b 5f73 616d 706c 655f 7265 636f 7264  ck_sample_record
-00016700: 732e 6173 7365 7274 5f63 616c 6c65 645f  s.assert_called_
-00016710: 6f6e 6365 5f77 6974 6828 0a20 2020 2020  once_with(.     
-00016720: 2020 2032 2c0a 2020 2020 2020 2020 312c     2,.        1,
-00016730: 0a20 2020 2020 2020 204e 6f6e 652c 0a20  .        None,. 
-00016740: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
-00016750: 2020 2020 205b 7b22 4122 3a20 3230 307d       [{"A": 200}
-00016760: 2c20 7b22 4122 3a20 3230 317d 5d2c 0a20  , {"A": 201}],. 
-00016770: 2020 2020 2020 2063 6c69 656e 742e 5f72         client._r
-00016780: 6573 6f6c 7665 5f6a 6f69 6e5f 6b65 7973  esolve_join_keys
-00016790: 282a 2a6b 7761 7267 7329 2c0a 2020 2020  (**kwargs),.    
-000167a0: 2020 2020 7465 7374 5f74 696d 6573 7461      test_timesta
-000167b0: 6d70 735f 6c69 7374 2c0a 2020 2020 2020  mps_list,.      
-000167c0: 2020 6578 7065 6374 6564 5f74 6167 735f    expected_tags_
-000167d0: 7061 7261 6d2c 0a20 2020 2029 0a0a 0a40  param,.    )...@
-000167e0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-000167f0: 6d65 7472 697a 6528 2274 6573 745f 6665  metrize("test_fe
-00016800: 6564 6261 636b 7322 2c20 5445 5354 5f46  edbacks", TEST_F
-00016810: 4545 4442 4143 4b53 290a 4070 7974 6573  EEDBACKS).@pytes
-00016820: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00016830: 7a65 2822 7665 7273 696f 6e22 2c20 5b4e  ze("version", [N
-00016840: 6f6e 652c 2031 302c 2022 312e 322e 3322  one, 10, "1.2.3"
-00016850: 5d29 0a40 6d6f 636b 2e70 6174 6368 2822  ]).@mock.patch("
-00016860: 6761 6e74 7279 2e6c 6f67 6765 722e 636c  gantry.logger.cl
-00016870: 6965 6e74 2e47 616e 7472 792e 5f6c 6f67  ient.Gantry._log
-00016880: 5f70 7265 6469 6374 696f 6e5f 616e 645f  _prediction_and_
-00016890: 6665 6564 6261 636b 5f65 7665 6e74 7322  feedback_events"
-000168a0: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-000168b0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-000168c0: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
-000168d0: 7072 6564 6963 7469 6f6e 5f65 7665 6e74  prediction_event
-000168e0: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
-000168f0: 0a20 2020 2022 6761 6e74 7279 2e6c 6f67  .    "gantry.log
-00016900: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-00016910: 792e 5f6c 6f67 5f66 6565 6462 6163 6b5f  y._log_feedback_
-00016920: 6576 656e 7473 222c 2072 6574 7572 6e5f  events", return_
-00016930: 7661 6c75 653d 284e 6f6e 652c 205b 2231  value=(None, ["1
-00016940: 3233 3435 222c 2022 3637 3839 3022 5d29  2345", "67890"])
-00016950: 0a29 0a64 6566 2074 6573 745f 6c6f 675f  .).def test_log_
-00016960: 7265 636f 7264 735f 6665 6564 6261 636b  records_feedback
-00016970: 5f6f 6e6c 795f 6e6f 5f6a 6f69 6e5f 6b65  _only_no_join_ke
-00016980: 7973 280a 2020 2020 6d6f 636b 5f66 6565  ys(.    mock_fee
-00016990: 6462 6163 6b2c 0a20 2020 206d 6f63 6b5f  dback,.    mock_
-000169a0: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
-000169b0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-000169c0: 636b 2c0a 2020 2020 7665 7273 696f 6e2c  ck,.    version,
-000169d0: 0a20 2020 2074 6573 745f 6665 6564 6261  .    test_feedba
-000169e0: 636b 732c 0a20 2020 2063 6c69 5f6f 626a  cks,.    cli_obj
-000169f0: 2c0a 293a 0a20 2020 2061 7373 6572 7420  ,.):.    assert 
-00016a00: 280a 2020 2020 2020 2020 636c 695f 6f62  (.        cli_ob
-00016a10: 6a2e 6c6f 675f 7265 636f 7264 7328 0a20  j.log_records(. 
-00016a20: 2020 2020 2020 2020 2020 2061 7070 6c69             appli
-00016a30: 6361 7469 6f6e 3d22 666f 6f62 6172 222c  cation="foobar",
-00016a40: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
-00016a50: 7369 6f6e 3d76 6572 7369 6f6e 2c0a 2020  sion=version,.  
-00016a60: 2020 2020 2020 2020 2020 696e 7075 7473            inputs
-00016a70: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00016a80: 2020 206f 7574 7075 7473 3d4e 6f6e 652c     outputs=None,
-00016a90: 0a20 2020 2020 2020 2020 2020 2066 6565  .            fee
-00016aa0: 6462 6163 6b73 3d74 6573 745f 6665 6564  dbacks=test_feed
-00016ab0: 6261 636b 732c 0a20 2020 2020 2020 2020  backs,.         
-00016ac0: 2020 2074 696d 6573 7461 6d70 733d 4e6f     timestamps=No
-00016ad0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00016ae0: 736f 7274 5f6f 6e5f 7469 6d65 7374 616d  sort_on_timestam
-00016af0: 703d 5472 7565 2c0a 2020 2020 2020 2020  p=True,.        
-00016b00: 290a 2020 2020 2020 2020 6973 204e 6f6e  ).        is Non
-00016b10: 650a 2020 2020 290a 0a20 2020 206d 6f63  e.    )..    moc
-00016b20: 6b5f 7072 6564 735f 616e 645f 6665 6564  k_preds_and_feed
-00016b30: 6261 636b 2e61 7373 6572 745f 6e6f 745f  back.assert_not_
-00016b40: 6361 6c6c 6564 2829 0a20 2020 206d 6f63  called().    moc
-00016b50: 6b5f 7072 6564 732e 6173 7365 7274 5f6e  k_preds.assert_n
-00016b60: 6f74 5f63 616c 6c65 6428 290a 2020 2020  ot_called().    
-00016b70: 6d6f 636b 5f66 6565 6462 6163 6b2e 6173  mock_feedback.as
-00016b80: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
-00016b90: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-00016ba0: 2e70 6172 616d 6574 7269 7a65 2822 7465  .parametrize("te
-00016bb0: 7374 5f66 6565 6462 6163 6b73 222c 2054  st_feedbacks", T
-00016bc0: 4553 545f 4645 4544 4241 434b 5329 0a40  EST_FEEDBACKS).@
-00016bd0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-00016be0: 6d65 7472 697a 6528 2276 6572 7369 6f6e  metrize("version
-00016bf0: 222c 205b 4e6f 6e65 2c20 3130 2c20 2231  ", [None, 10, "1
-00016c00: 2e32 2e33 225d 290a 406d 6f63 6b2e 7061  .2.3"]).@mock.pa
-00016c10: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
-00016c20: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
-00016c30: 2e5f 6765 6e65 7261 7465 5f70 7265 6469  ._generate_predi
-00016c40: 6374 696f 6e5f 616e 645f 6665 6564 6261  ction_and_feedba
-00016c50: 636b 5f65 7665 6e74 7322 290a 406d 6f63  ck_events").@moc
-00016c60: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-00016c70: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
-00016c80: 6e74 7279 2e5f 6765 6e65 7261 7465 5f70  ntry._generate_p
-00016c90: 7265 6469 6374 696f 6e5f 6576 656e 7473  rediction_events
-00016ca0: 2229 0a40 6d6f 636b 2e70 6174 6368 280a  ").@mock.patch(.
-00016cb0: 2020 2020 2267 616e 7472 792e 6c6f 6767      "gantry.logg
-00016cc0: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
-00016cd0: 2e5f 6765 6e65 7261 7465 5f66 6565 6462  ._generate_feedb
-00016ce0: 6163 6b5f 6576 656e 7473 222c 2072 6574  ack_events", ret
-00016cf0: 7572 6e5f 7661 6c75 653d 284e 6f6e 652c  urn_value=(None,
-00016d00: 205b 2231 3233 3435 222c 2022 3637 3839   ["12345", "6789
-00016d10: 3022 5d29 0a29 0a64 6566 2074 6573 745f  0"]).).def test_
-00016d20: 6765 6e65 7261 7465 5f72 6563 6f72 6473  generate_records
-00016d30: 5f66 6565 6462 6163 6b5f 6f6e 6c79 5f6e  _feedback_only_n
-00016d40: 6f5f 6a6f 696e 5f6b 6579 7328 0a20 2020  o_join_keys(.   
-00016d50: 206d 6f63 6b5f 6665 6564 6261 636b 2c0a   mock_feedback,.
-00016d60: 2020 2020 6d6f 636b 5f70 7265 6473 2c0a      mock_preds,.
-00016d70: 2020 2020 6d6f 636b 5f70 7265 6473 5f61      mock_preds_a
-00016d80: 6e64 5f66 6565 6462 6163 6b2c 0a20 2020  nd_feedback,.   
-00016d90: 2076 6572 7369 6f6e 2c0a 2020 2020 7465   version,.    te
-00016da0: 7374 5f66 6565 6462 6163 6b73 2c0a 2020  st_feedbacks,.  
-00016db0: 2020 636c 695f 6f62 6a2c 0a29 3a0a 2020    cli_obj,.):.  
-00016dc0: 2020 6173 7365 7274 2028 0a20 2020 2020    assert (.     
-00016dd0: 2020 2063 6c69 5f6f 626a 2e67 656e 6572     cli_obj.gener
-00016de0: 6174 655f 7265 636f 7264 7328 0a20 2020  ate_records(.   
-00016df0: 2020 2020 2020 2020 2061 7070 6c69 6361           applica
-00016e00: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
-00016e10: 2020 2020 2020 2020 2020 2076 6572 7369             versi
-00016e20: 6f6e 3d76 6572 7369 6f6e 2c0a 2020 2020  on=version,.    
-00016e30: 2020 2020 2020 2020 696e 7075 7473 3d4e          inputs=N
-00016e40: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00016e50: 206f 7574 7075 7473 3d4e 6f6e 652c 0a20   outputs=None,. 
-00016e60: 2020 2020 2020 2020 2020 2066 6565 6462             feedb
-00016e70: 6163 6b73 3d74 6573 745f 6665 6564 6261  acks=test_feedba
-00016e80: 636b 732c 0a20 2020 2020 2020 2020 2020  cks,.           
-00016e90: 2074 696d 6573 7461 6d70 733d 4e6f 6e65   timestamps=None
-00016ea0: 2c0a 2020 2020 2020 2020 2020 2020 736f  ,.            so
-00016eb0: 7274 5f6f 6e5f 7469 6d65 7374 616d 703d  rt_on_timestamp=
-00016ec0: 5472 7565 2c0a 2020 2020 2020 2020 290a  True,.        ).
-00016ed0: 2020 2020 2020 2020 6973 204e 6f6e 650a          is None.
-00016ee0: 2020 2020 290a 0a20 2020 206d 6f63 6b5f      )..    mock_
-00016ef0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-00016f00: 636b 2e61 7373 6572 745f 6e6f 745f 6361  ck.assert_not_ca
-00016f10: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
-00016f20: 7072 6564 732e 6173 7365 7274 5f6e 6f74  preds.assert_not
-00016f30: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
-00016f40: 636b 5f66 6565 6462 6163 6b2e 6173 7365  ck_feedback.asse
-00016f50: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00016f60: 0a0a 4070 7974 6573 742e 6d61 726b 2e70  ..@pytest.mark.p
-00016f70: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
-00016f80: 2822 7465 7374 5f66 6565 6462 6163 6b73  ("test_feedbacks
-00016f90: 222c 2022 7465 7374 5f6f 7574 7075 7473  ", "test_outputs
-00016fa0: 222c 2022 7465 7374 5f69 6e70 7574 7322  ", "test_inputs"
-00016fb0: 292c 0a20 2020 205b 0a20 2020 2020 2020  ),.    [.       
-00016fc0: 2028 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f   (None, None, No
-00016fd0: 6e65 292c 0a20 2020 2020 2020 2028 7064  ne),.        (pd
-00016fe0: 2e44 6174 6146 7261 6d65 2829 2c20 7064  .DataFrame(), pd
-00016ff0: 2e44 6174 6146 7261 6d65 2829 2c20 7064  .DataFrame(), pd
-00017000: 2e44 6174 6146 7261 6d65 2829 292c 0a20  .DataFrame()),. 
-00017010: 2020 2020 2020 2028 5b5d 2c20 5b5d 2c20         ([], [], 
-00017020: 5b5d 292c 0a20 2020 2020 2020 2028 7064  []),.        (pd
-00017030: 2e53 6572 6965 7328 292c 2070 642e 5365  .Series(), pd.Se
-00017040: 7269 6573 2829 2c20 7064 2e53 6572 6965  ries(), pd.Serie
-00017050: 7328 2929 2c0a 2020 2020 2020 2020 286e  s()),.        (n
-00017060: 702e 6172 7261 7928 5b5d 292c 206e 702e  p.array([]), np.
-00017070: 6172 7261 7928 5b5d 292c 206e 702e 6172  array([]), np.ar
-00017080: 7261 7928 5b5d 2929 2c0a 2020 2020 5d2c  ray([])),.    ],
-00017090: 0a29 0a40 7079 7465 7374 2e6d 6172 6b2e  .).@pytest.mark.
-000170a0: 7061 7261 6d65 7472 697a 6528 2276 6572  parametrize("ver
-000170b0: 7369 6f6e 222c 205b 4e6f 6e65 2c20 3130  sion", [None, 10
-000170c0: 2c20 2231 2e32 2e33 225d 290a 406d 6f63  , "1.2.3"]).@moc
-000170d0: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-000170e0: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
-000170f0: 6e74 7279 2e5f 6c6f 675f 7072 6564 6963  ntry._log_predic
-00017100: 7469 6f6e 5f61 6e64 5f66 6565 6462 6163  tion_and_feedbac
-00017110: 6b5f 6576 656e 7473 2229 0a40 6d6f 636b  k_events").@mock
-00017120: 2e70 6174 6368 2822 6761 6e74 7279 2e6c  .patch("gantry.l
-00017130: 6f67 6765 722e 636c 6965 6e74 2e47 616e  ogger.client.Gan
-00017140: 7472 792e 5f6c 6f67 5f70 7265 6469 6374  try._log_predict
-00017150: 696f 6e5f 6576 656e 7473 2229 0a40 6d6f  ion_events").@mo
-00017160: 636b 2e70 6174 6368 2822 6761 6e74 7279  ck.patch("gantry
-00017170: 2e6c 6f67 6765 722e 636c 6965 6e74 2e47  .logger.client.G
-00017180: 616e 7472 792e 5f6c 6f67 5f66 6565 6462  antry._log_feedb
-00017190: 6163 6b5f 6576 656e 7473 2229 0a64 6566  ack_events").def
-000171a0: 2074 6573 745f 6c6f 675f 7265 636f 7264   test_log_record
-000171b0: 735f 6e6f 5f64 6174 6128 0a20 2020 206d  s_no_data(.    m
-000171c0: 6f63 6b5f 6665 6564 6261 636b 2c0a 2020  ock_feedback,.  
-000171d0: 2020 6d6f 636b 5f70 7265 6473 2c0a 2020    mock_preds,.  
-000171e0: 2020 6d6f 636b 5f70 7265 6473 5f61 6e64    mock_preds_and
-000171f0: 5f66 6565 6462 6163 6b2c 0a20 2020 2076  _feedback,.    v
-00017200: 6572 7369 6f6e 2c0a 2020 2020 7465 7374  ersion,.    test
-00017210: 5f69 6e70 7574 732c 0a20 2020 2074 6573  _inputs,.    tes
-00017220: 745f 6f75 7470 7574 732c 0a20 2020 2074  t_outputs,.    t
-00017230: 6573 745f 6665 6564 6261 636b 732c 0a20  est_feedbacks,. 
-00017240: 2020 2063 6c69 5f6f 626a 2c0a 293a 0a20     cli_obj,.):. 
-00017250: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
-00017260: 2020 2020 636c 695f 6f62 6a2e 6c6f 675f      cli_obj.log_
-00017270: 7265 636f 7264 7328 0a20 2020 2020 2020  records(.       
-00017280: 2020 2020 2061 7070 6c69 6361 7469 6f6e       application
-00017290: 3d22 666f 6f62 6172 222c 0a20 2020 2020  ="foobar",.     
-000172a0: 2020 2020 2020 2076 6572 7369 6f6e 3d76         version=v
-000172b0: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
-000172c0: 2020 2020 696e 7075 7473 3d74 6573 745f      inputs=test_
-000172d0: 696e 7075 7473 2c0a 2020 2020 2020 2020  inputs,.        
-000172e0: 2020 2020 6f75 7470 7574 733d 7465 7374      outputs=test
-000172f0: 5f6f 7574 7075 7473 2c0a 2020 2020 2020  _outputs,.      
-00017300: 2020 2020 2020 6665 6564 6261 636b 733d        feedbacks=
-00017310: 7465 7374 5f66 6565 6462 6163 6b73 2c0a  test_feedbacks,.
-00017320: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00017330: 7374 616d 7073 3d4e 6f6e 652c 0a20 2020  stamps=None,.   
-00017340: 2020 2020 2020 2020 2073 6f72 745f 6f6e           sort_on
-00017350: 5f74 696d 6573 7461 6d70 3d54 7275 652c  _timestamp=True,
-00017360: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00017370: 2020 2069 7320 4e6f 6e65 0a20 2020 2029     is None.    )
-00017380: 0a0a 2020 2020 6d6f 636b 5f70 7265 6473  ..    mock_preds
-00017390: 5f61 6e64 5f66 6565 6462 6163 6b2e 6173  _and_feedback.as
-000173a0: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
-000173b0: 290a 2020 2020 6d6f 636b 5f70 7265 6473  ).    mock_preds
-000173c0: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-000173d0: 6564 2829 0a20 2020 206d 6f63 6b5f 6665  ed().    mock_fe
-000173e0: 6564 6261 636b 2e61 7373 6572 745f 6e6f  edback.assert_no
-000173f0: 745f 6361 6c6c 6564 2829 0a0a 0a40 7079  t_called()...@py
-00017400: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
-00017410: 7472 697a 6528 0a20 2020 2028 2274 6573  trize(.    ("tes
-00017420: 745f 6665 6564 6261 636b 7322 2c20 2274  t_feedbacks", "t
-00017430: 6573 745f 6f75 7470 7574 7322 2c20 2274  est_outputs", "t
-00017440: 6573 745f 696e 7075 7473 2229 2c0a 2020  est_inputs"),.  
-00017450: 2020 5b0a 2020 2020 2020 2020 284e 6f6e    [.        (Non
-00017460: 652c 204e 6f6e 652c 204e 6f6e 6529 2c0a  e, None, None),.
-00017470: 2020 2020 2020 2020 2870 642e 4461 7461          (pd.Data
-00017480: 4672 616d 6528 292c 2070 642e 4461 7461  Frame(), pd.Data
-00017490: 4672 616d 6528 292c 2070 642e 4461 7461  Frame(), pd.Data
-000174a0: 4672 616d 6528 2929 2c0a 2020 2020 2020  Frame()),.      
-000174b0: 2020 285b 5d2c 205b 5d2c 205b 5d29 2c0a    ([], [], []),.
-000174c0: 2020 2020 2020 2020 2870 642e 5365 7269          (pd.Seri
-000174d0: 6573 2829 2c20 7064 2e53 6572 6965 7328  es(), pd.Series(
-000174e0: 292c 2070 642e 5365 7269 6573 2829 292c  ), pd.Series()),
-000174f0: 0a20 2020 2020 2020 2028 6e70 2e61 7272  .        (np.arr
-00017500: 6179 285b 5d29 2c20 6e70 2e61 7272 6179  ay([]), np.array
-00017510: 285b 5d29 2c20 6e70 2e61 7272 6179 285b  ([]), np.array([
-00017520: 5d29 292c 0a20 2020 205d 2c0a 290a 4070  ])),.    ],.).@p
-00017530: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-00017540: 6574 7269 7a65 2822 7665 7273 696f 6e22  etrize("version"
-00017550: 2c20 5b4e 6f6e 652c 2031 302c 2022 312e  , [None, 10, "1.
-00017560: 322e 3322 5d29 0a40 6d6f 636b 2e70 6174  2.3"]).@mock.pat
-00017570: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
-00017580: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
-00017590: 5f67 656e 6572 6174 655f 7072 6564 6963  _generate_predic
-000175a0: 7469 6f6e 5f61 6e64 5f66 6565 6462 6163  tion_and_feedbac
-000175b0: 6b5f 6576 656e 7473 2229 0a40 6d6f 636b  k_events").@mock
-000175c0: 2e70 6174 6368 2822 6761 6e74 7279 2e6c  .patch("gantry.l
-000175d0: 6f67 6765 722e 636c 6965 6e74 2e47 616e  ogger.client.Gan
-000175e0: 7472 792e 5f67 656e 6572 6174 655f 7072  try._generate_pr
-000175f0: 6564 6963 7469 6f6e 5f65 7665 6e74 7322  ediction_events"
-00017600: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
-00017610: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
-00017620: 656e 742e 4761 6e74 7279 2e5f 6765 6e65  ent.Gantry._gene
-00017630: 7261 7465 5f66 6565 6462 6163 6b5f 6576  rate_feedback_ev
-00017640: 656e 7473 2229 0a64 6566 2074 6573 745f  ents").def test_
-00017650: 6765 6e65 7261 7465 5f72 6563 6f72 6473  generate_records
-00017660: 5f6e 6f5f 6461 7461 280a 2020 2020 6d6f  _no_data(.    mo
-00017670: 636b 5f67 656e 6572 6174 655f 6665 6564  ck_generate_feed
-00017680: 6261 636b 2c0a 2020 2020 6d6f 636b 5f67  back,.    mock_g
-00017690: 656e 6572 6174 655f 7072 6564 732c 0a20  enerate_preds,. 
-000176a0: 2020 206d 6f63 6b5f 6765 6e65 7261 7465     mock_generate
-000176b0: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
-000176c0: 6163 6b2c 0a20 2020 2076 6572 7369 6f6e  ack,.    version
-000176d0: 2c0a 2020 2020 7465 7374 5f69 6e70 7574  ,.    test_input
-000176e0: 732c 0a20 2020 2074 6573 745f 6f75 7470  s,.    test_outp
-000176f0: 7574 732c 0a20 2020 2074 6573 745f 6665  uts,.    test_fe
-00017700: 6564 6261 636b 732c 0a20 2020 2063 6c69  edbacks,.    cli
-00017710: 5f6f 626a 2c0a 293a 0a20 2020 2061 7373  _obj,.):.    ass
-00017720: 6572 7420 280a 2020 2020 2020 2020 636c  ert (.        cl
-00017730: 695f 6f62 6a2e 6765 6e65 7261 7465 5f72  i_obj.generate_r
-00017740: 6563 6f72 6473 280a 2020 2020 2020 2020  ecords(.        
-00017750: 2020 2020 6170 706c 6963 6174 696f 6e3d      application=
-00017760: 2266 6f6f 6261 7222 2c0a 2020 2020 2020  "foobar",.      
-00017770: 2020 2020 2020 7665 7273 696f 6e3d 7665        version=ve
-00017780: 7273 696f 6e2c 0a20 2020 2020 2020 2020  rsion,.         
-00017790: 2020 2069 6e70 7574 733d 7465 7374 5f69     inputs=test_i
-000177a0: 6e70 7574 732c 0a20 2020 2020 2020 2020  nputs,.         
-000177b0: 2020 206f 7574 7075 7473 3d74 6573 745f     outputs=test_
-000177c0: 6f75 7470 7574 732c 0a20 2020 2020 2020  outputs,.       
-000177d0: 2020 2020 2066 6565 6462 6163 6b73 3d74       feedbacks=t
-000177e0: 6573 745f 6665 6564 6261 636b 732c 0a20  est_feedbacks,. 
-000177f0: 2020 2020 2020 2020 2020 2074 696d 6573             times
-00017800: 7461 6d70 733d 4e6f 6e65 2c0a 2020 2020  tamps=None,.    
-00017810: 2020 2020 2020 2020 736f 7274 5f6f 6e5f          sort_on_
-00017820: 7469 6d65 7374 616d 703d 5472 7565 2c0a  timestamp=True,.
-00017830: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017840: 2020 6973 204e 6f6e 650a 2020 2020 290a    is None.    ).
-00017850: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
-00017860: 7465 5f70 7265 6473 5f61 6e64 5f66 6565  te_preds_and_fee
-00017870: 6462 6163 6b2e 6173 7365 7274 5f6e 6f74  dback.assert_not
-00017880: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
-00017890: 636b 5f67 656e 6572 6174 655f 7072 6564  ck_generate_pred
-000178a0: 732e 6173 7365 7274 5f6e 6f74 5f63 616c  s.assert_not_cal
-000178b0: 6c65 6428 290a 2020 2020 6d6f 636b 5f67  led().    mock_g
-000178c0: 656e 6572 6174 655f 6665 6564 6261 636b  enerate_feedback
-000178d0: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-000178e0: 6564 2829 0a0a 0a40 7079 7465 7374 2e6d  ed()...@pytest.m
-000178f0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
-00017900: 0a20 2020 2022 7465 7374 5f66 6565 6462  .    "test_feedb
-00017910: 6163 6b73 222c 0a20 2020 205b 4e6f 6e65  acks",.    [None
-00017920: 2c20 7064 2e44 6174 6146 7261 6d65 2829  , pd.DataFrame()
-00017930: 2c20 5b7b 2241 223a 2033 7d2c 207b 2241  , [{"A": 3}, {"A
-00017940: 223a 2033 7d5d 2c20 7064 2e53 6572 6965  ": 3}], pd.Serie
-00017950: 7328 295d 2c0a 290a 406d 6f63 6b2e 7061  s()],.).@mock.pa
-00017960: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
-00017970: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
-00017980: 2e5f 6c6f 675f 7072 6564 6963 7469 6f6e  ._log_prediction
-00017990: 5f61 6e64 5f66 6565 6462 6163 6b5f 6576  _and_feedback_ev
-000179a0: 656e 7473 2229 0a40 6d6f 636b 2e70 6174  ents").@mock.pat
-000179b0: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
-000179c0: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
-000179d0: 5f6c 6f67 5f70 7265 6469 6374 696f 6e5f  _log_prediction_
-000179e0: 6576 656e 7473 2229 0a40 6d6f 636b 2e70  events").@mock.p
-000179f0: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
-00017a00: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-00017a10: 792e 5f6c 6f67 5f66 6565 6462 6163 6b5f  y._log_feedback_
-00017a20: 6576 656e 7473 2229 0a64 6566 2074 6573  events").def tes
-00017a30: 745f 6c6f 675f 7265 636f 7264 735f 696e  t_log_records_in
-00017a40: 636f 6d70 6c65 7465 5f70 7265 6473 280a  complete_preds(.
-00017a50: 2020 2020 6d6f 636b 5f66 6565 6462 6163      mock_feedbac
-00017a60: 6b2c 0a20 2020 206d 6f63 6b5f 7072 6564  k,.    mock_pred
-00017a70: 732c 0a20 2020 206d 6f63 6b5f 7072 6564  s,.    mock_pred
-00017a80: 735f 616e 645f 6665 6564 6261 636b 2c0a  s_and_feedback,.
-00017a90: 2020 2020 7465 7374 5f66 6565 6462 6163      test_feedbac
-00017aa0: 6b73 2c0a 2020 2020 636c 695f 6f62 6a2c  ks,.    cli_obj,
-00017ab0: 0a29 3a0a 2020 2020 7276 203d 2063 6c69  .):.    rv = cli
-00017ac0: 5f6f 626a 2e6c 6f67 5f72 6563 6f72 6473  _obj.log_records
-00017ad0: 280a 2020 2020 2020 2020 6170 706c 6963  (.        applic
-00017ae0: 6174 696f 6e3d 2266 6f6f 6261 7222 2c0a  ation="foobar",.
-00017af0: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
-00017b00: 2232 2e30 2e31 222c 0a20 2020 2020 2020  "2.0.1",.       
-00017b10: 2069 6e70 7574 733d 5b5d 2c0a 2020 2020   inputs=[],.    
-00017b20: 2020 2020 6f75 7470 7574 733d 5b7b 2241      outputs=[{"A
-00017b30: 223a 2031 7d2c 207b 2241 223a 2032 7d5d  ": 1}, {"A": 2}]
-00017b40: 2c0a 2020 2020 2020 2020 6665 6564 6261  ,.        feedba
-00017b50: 636b 733d 7465 7374 5f66 6565 6462 6163  cks=test_feedbac
-00017b60: 6b73 2c0a 2020 2020 2020 2020 7469 6d65  ks,.        time
-00017b70: 7374 616d 7073 3d4e 6f6e 652c 0a20 2020  stamps=None,.   
-00017b80: 2020 2020 2073 6f72 745f 6f6e 5f74 696d       sort_on_tim
-00017b90: 6573 7461 6d70 3d54 7275 652c 0a20 2020  estamp=True,.   
-00017ba0: 2029 0a20 2020 2061 7373 6572 7420 7276   ).    assert rv
-00017bb0: 2069 7320 4e6f 6e65 0a0a 2020 2020 6d6f   is None..    mo
-00017bc0: 636b 5f70 7265 6473 5f61 6e64 5f66 6565  ck_preds_and_fee
-00017bd0: 6462 6163 6b2e 6173 7365 7274 5f6e 6f74  dback.assert_not
-00017be0: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
-00017bf0: 636b 5f70 7265 6473 2e61 7373 6572 745f  ck_preds.assert_
-00017c00: 6e6f 745f 6361 6c6c 6564 2829 0a20 2020  not_called().   
-00017c10: 206d 6f63 6b5f 6665 6564 6261 636b 2e61   mock_feedback.a
-00017c20: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
-00017c30: 2829 0a0a 0a40 7079 7465 7374 2e6d 6172  ()...@pytest.mar
-00017c40: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
-00017c50: 2020 2022 7465 7374 5f66 6565 6462 6163     "test_feedbac
-00017c60: 6b73 222c 0a20 2020 205b 4e6f 6e65 2c20  ks",.    [None, 
-00017c70: 7064 2e44 6174 6146 7261 6d65 2829 2c20  pd.DataFrame(), 
-00017c80: 5b7b 2241 223a 2033 7d2c 207b 2241 223a  [{"A": 3}, {"A":
-00017c90: 2033 7d5d 2c20 7064 2e53 6572 6965 7328   3}], pd.Series(
-00017ca0: 295d 2c0a 290a 406d 6f63 6b2e 7061 7463  )],.).@mock.patc
-00017cb0: 6828 2267 616e 7472 792e 6c6f 6767 6572  h("gantry.logger
-00017cc0: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-00017cd0: 6765 6e65 7261 7465 5f70 7265 6469 6374  generate_predict
-00017ce0: 696f 6e5f 616e 645f 6665 6564 6261 636b  ion_and_feedback
-00017cf0: 5f65 7665 6e74 7322 290a 406d 6f63 6b2e  _events").@mock.
-00017d00: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-00017d10: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-00017d20: 7279 2e5f 6765 6e65 7261 7465 5f70 7265  ry._generate_pre
-00017d30: 6469 6374 696f 6e5f 6576 656e 7473 2229  diction_events")
-00017d40: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
-00017d50: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
-00017d60: 6e74 2e47 616e 7472 792e 5f67 656e 6572  nt.Gantry._gener
-00017d70: 6174 655f 6665 6564 6261 636b 5f65 7665  ate_feedback_eve
-00017d80: 6e74 7322 290a 6465 6620 7465 7374 5f67  nts").def test_g
-00017d90: 656e 6572 6174 655f 7265 636f 7264 735f  enerate_records_
-00017da0: 696e 636f 6d70 6c65 7465 5f70 7265 6473  incomplete_preds
-00017db0: 280a 2020 2020 6d6f 636b 5f67 656e 6572  (.    mock_gener
-00017dc0: 6174 655f 6665 6564 6261 636b 2c0a 2020  ate_feedback,.  
-00017dd0: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
-00017de0: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
-00017df0: 6765 6e65 7261 7465 5f70 7265 6473 5f61  generate_preds_a
-00017e00: 6e64 5f66 6565 6462 6163 6b2c 0a20 2020  nd_feedback,.   
-00017e10: 2074 6573 745f 6665 6564 6261 636b 732c   test_feedbacks,
-00017e20: 0a20 2020 2063 6c69 5f6f 626a 2c0a 293a  .    cli_obj,.):
-00017e30: 0a20 2020 2072 7620 3d20 636c 695f 6f62  .    rv = cli_ob
-00017e40: 6a2e 6765 6e65 7261 7465 5f72 6563 6f72  j.generate_recor
-00017e50: 6473 280a 2020 2020 2020 2020 6170 706c  ds(.        appl
-00017e60: 6963 6174 696f 6e3d 2266 6f6f 6261 7222  ication="foobar"
-00017e70: 2c0a 2020 2020 2020 2020 7665 7273 696f  ,.        versio
-00017e80: 6e3d 2232 2e30 2e31 222c 0a20 2020 2020  n="2.0.1",.     
-00017e90: 2020 2069 6e70 7574 733d 5b5d 2c0a 2020     inputs=[],.  
-00017ea0: 2020 2020 2020 6f75 7470 7574 733d 5b7b        outputs=[{
-00017eb0: 2241 223a 2031 7d2c 207b 2241 223a 2032  "A": 1}, {"A": 2
-00017ec0: 7d5d 2c0a 2020 2020 2020 2020 6665 6564  }],.        feed
-00017ed0: 6261 636b 733d 7465 7374 5f66 6565 6462  backs=test_feedb
-00017ee0: 6163 6b73 2c0a 2020 2020 2020 2020 7469  acks,.        ti
-00017ef0: 6d65 7374 616d 7073 3d4e 6f6e 652c 0a20  mestamps=None,. 
-00017f00: 2020 2020 2020 2073 6f72 745f 6f6e 5f74         sort_on_t
-00017f10: 696d 6573 7461 6d70 3d54 7275 652c 0a20  imestamp=True,. 
-00017f20: 2020 2029 0a20 2020 2061 7373 6572 7420     ).    assert 
-00017f30: 7276 2069 7320 4e6f 6e65 0a0a 2020 2020  rv is None..    
-00017f40: 6d6f 636b 5f67 656e 6572 6174 655f 7072  mock_generate_pr
-00017f50: 6564 735f 616e 645f 6665 6564 6261 636b  eds_and_feedback
-00017f60: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
-00017f70: 6564 2829 0a20 2020 206d 6f63 6b5f 6765  ed().    mock_ge
-00017f80: 6e65 7261 7465 5f70 7265 6473 2e61 7373  nerate_preds.ass
-00017f90: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
-00017fa0: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
-00017fb0: 7465 5f66 6565 6462 6163 6b2e 6173 7365  te_feedback.asse
-00017fc0: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00017fd0: 0a0a 4070 7974 6573 742e 6d61 726b 2e70  ..@pytest.mark.p
-00017fe0: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
-00017ff0: 2274 6573 745f 696e 7075 7473 222c 0a20  "test_inputs",. 
-00018000: 2020 205b 5b7b 2241 223a 2031 3030 7d2c     [[{"A": 100},
-00018010: 207b 2241 223a 2031 3031 7d5d 5d2c 0a29   {"A": 101}]],.)
-00018020: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
-00018030: 6e74 7279 2e6c 6f67 6765 722e 7574 696c  ntry.logger.util
-00018040: 732e 6765 745f 6669 6c65 5f6c 696e 6563  s.get_file_linec
-00018050: 6f75 6e74 2229 0a64 6566 2074 6573 745f  ount").def test_
-00018060: 6c6f 675f 6669 6c65 286d 6f63 6b5f 6c69  log_file(mock_li
-00018070: 6e65 5f63 6f75 6e74 2c20 7465 7374 5f69  ne_count, test_i
-00018080: 6e70 7574 7329 3a0a 2020 2020 6c6f 675f  nputs):.    log_
-00018090: 7374 6f72 6520 3d20 6d6f 636b 2e4d 6167  store = mock.Mag
-000180a0: 6963 4d6f 636b 2829 0a20 2020 2067 616e  icMock().    gan
-000180b0: 7472 7920 3d20 636c 6965 6e74 2e47 616e  try = client.Gan
-000180c0: 7472 7928 6c6f 675f 7374 6f72 653d 6c6f  try(log_store=lo
-000180d0: 675f 7374 6f72 652c 2065 6e76 6972 6f6e  g_store, environ
-000180e0: 6d65 6e74 3d22 7465 7374 2229 0a20 2020  ment="test").   
-000180f0: 206d 6f63 6b5f 6c69 6e65 5f63 6f75 6e74   mock_line_count
-00018100: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
-00018110: 350a 0a20 2020 2067 616e 7472 792e 6c6f  5..    gantry.lo
-00018120: 675f 6669 6c65 280a 2020 2020 2020 2020  g_file(.        
-00018130: 2266 6f6f 6261 7222 2c0a 2020 2020 2020  "foobar",.      
-00018140: 2020 2264 6972 2f63 7376 5f77 6974 685f    "dir/csv_with_
-00018150: 6865 6164 6572 732e 6373 7622 2c0a 2020  headers.csv",.  
-00018160: 2020 2020 2020 7665 7273 696f 6e3d 2232        version="2
-00018170: 2e30 2e31 222c 0a20 2020 2029 0a0a 2020  .0.1",.    )..  
-00018180: 2020 6c6f 675f 7374 6f72 652e 6c6f 675f    log_store.log_
-00018190: 6261 7463 682e 6173 7365 7274 5f6e 6f74  batch.assert_not
-000181a0: 5f63 616c 6c65 6428 290a 0a0a 406d 6f63  _called()...@moc
-000181b0: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
-000181c0: 6c6f 6767 6572 2e63 6c69 656e 742e 7575  logger.client.uu
-000181d0: 6964 2e75 7569 6434 222c 2072 6574 7572  id.uuid4", retur
-000181e0: 6e5f 7661 6c75 653d 2241 4243 2229 0a40  n_value="ABC").@
-000181f0: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
-00018200: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
-00018210: 2e47 616e 7472 792e 5f68 616e 646c 655f  .Gantry._handle_
-00018220: 7570 6c6f 6164 2229 0a64 6566 2074 6573  upload").def tes
-00018230: 745f 736d 6172 745f 6669 6c65 7265 6164  t_smart_fileread
-00018240: 286d 6f63 6b5f 6861 6e64 6c65 5f75 706c  (mock_handle_upl
-00018250: 6f61 642c 206d 6f63 6b5f 7575 6964 2c20  oad, mock_uuid, 
-00018260: 636c 695f 6f62 6a29 3a0a 2020 2020 6461  cli_obj):.    da
-00018270: 7461 5f6c 696e 6b20 3d20 6d6f 636b 2e4d  ta_link = mock.M
-00018280: 6f63 6b28 290a 2020 2020 636c 695f 6f62  ock().    cli_ob
-00018290: 6a2e 5f73 6d61 7274 5f66 696c 655f 7265  j._smart_file_re
-000182a0: 6164 280a 2020 2020 2020 2020 6461 7461  ad(.        data
-000182b0: 5f6c 696e 6b3d 6461 7461 5f6c 696e 6b2c  _link=data_link,
-000182c0: 0a20 2020 2020 2020 206f 626a 6563 745f  .        object_
-000182d0: 7369 7a65 3d31 302c 0a20 2020 2020 2020  size=10,.       
-000182e0: 2070 6174 685f 6e61 6d65 3d22 666f 6f62   path_name="foob
-000182f0: 6172 222c 0a20 2020 2020 2020 2066 696c  ar",.        fil
-00018300: 653d 696f 2e53 7472 696e 6749 4f28 22f0  e=io.StringIO(".
-00018310: 9f98 8ef0 9f98 8e22 292c 0a20 2020 2020  ......."),.     
-00018320: 2020 2063 6875 6e6b 5f73 697a 653d 3230     chunk_size=20
-00018330: 302c 0a20 2020 2029 0a0a 2020 2020 6172  0,.    )..    ar
-00018340: 6773 2c20 6b77 6172 6773 203d 206d 6f63  gs, kwargs = moc
-00018350: 6b5f 6861 6e64 6c65 5f75 706c 6f61 642e  k_handle_upload.
-00018360: 6361 6c6c 5f61 7267 730a 0a20 2020 2061  call_args..    a
-00018370: 7373 6572 7420 6c69 7374 2861 7267 735b  ssert list(args[
-00018380: 305d 2920 3d3d 205b 6222 5c78 6630 5c78  0]) == [b"\xf0\x
-00018390: 3966 5c78 3938 5c78 3865 5c78 6630 5c78  9f\x98\x8e\xf0\x
-000183a0: 3966 5c78 3938 5c78 3865 225d 2020 2320  9f\x98\x8e"]  # 
-000183b0: 7465 7374 2055 5446 2d38 2073 7570 706f  test UTF-8 suppo
-000183c0: 7274 0a20 2020 2061 7373 6572 7420 6172  rt.    assert ar
-000183d0: 6773 5b31 5d20 3d3d 2064 6174 615f 6c69  gs[1] == data_li
-000183e0: 6e6b 0a20 2020 2061 7373 6572 7420 6172  nk.    assert ar
-000183f0: 6773 5b32 5d20 3d3d 2031 300a 2020 2020  gs[2] == 10.    
-00018400: 6173 7365 7274 2061 7267 735b 335d 203d  assert args[3] =
-00018410: 3d20 2241 4243 5f66 6f6f 6261 7222 0a0a  = "ABC_foobar"..
-00018420: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
-00018430: 7261 6d65 7472 697a 6528 0a20 2020 205b  rametrize(.    [
-00018440: 2269 6e70 7574 7322 2c20 226f 7574 7075  "inputs", "outpu
-00018450: 7473 222c 2022 6665 6564 6261 636b 7322  ts", "feedbacks"
-00018460: 2c20 226a 6f69 6e5f 6b65 7973 222c 2022  , "join_keys", "
-00018470: 7469 6d65 7374 616d 7073 225d 2c0a 2020  timestamps"],.  
-00018480: 2020 5b0a 2020 2020 2020 2020 285b 7b22    [.        ([{"
-00018490: 4122 3a20 3130 7d5d 202a 2031 302c 205b  A": 10}] * 10, [
-000184a0: 7b22 4122 3a20 3130 7d5d 202a 2039 2c20  {"A": 10}] * 9, 
-000184b0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-000184c0: 292c 0a20 2020 2020 2020 2028 5b7b 2241  ),.        ([{"A
-000184d0: 223a 2031 307d 5d20 2a20 3130 2c20 5b7b  ": 10}] * 10, [{
-000184e0: 2241 223a 2031 307d 5d20 2a20 392c 205b  "A": 10}] * 9, [
-000184f0: 7b22 4122 3a20 3131 7d5d 202a 2031 302c  {"A": 11}] * 10,
-00018500: 205b 2266 6f6f 6261 7222 5d20 2a20 3130   ["foobar"] * 10
-00018510: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
-00018520: 2028 5b7b 2241 223a 2031 307d 5d20 2a20   ([{"A": 10}] * 
-00018530: 392c 205b 7b22 4122 3a20 3130 7d5d 202a  9, [{"A": 10}] *
-00018540: 2038 2c20 5b7b 2241 223a 2031 317d 5d20   8, [{"A": 11}] 
-00018550: 2a20 3130 2c20 5b22 666f 6f62 6172 225d  * 10, ["foobar"]
-00018560: 202a 2031 302c 204e 6f6e 6529 2c0a 2020   * 10, None),.  
-00018570: 2020 2020 2020 285b 7b22 4122 3a20 3130        ([{"A": 10
-00018580: 7d5d 202a 2039 2c20 4e6f 6e65 2c20 5b7b  }] * 9, None, [{
-00018590: 2241 223a 2031 317d 5d20 2a20 3130 2c20  "A": 11}] * 10, 
-000185a0: 5b22 666f 6f62 6172 225d 202a 2031 302c  ["foobar"] * 10,
-000185b0: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
-000185c0: 284e 6f6e 652c 204e 6f6e 652c 205b 7b22  (None, None, [{"
-000185d0: 4122 3a20 3131 7d5d 202a 2031 312c 205b  A": 11}] * 11, [
-000185e0: 2266 6f6f 6261 7222 5d20 2a20 3130 2c20  "foobar"] * 10, 
-000185f0: 4e6f 6e65 292c 0a20 2020 2020 2020 2028  None),.        (
-00018600: 4e6f 6e65 2c20 4e6f 6e65 2c20 5b7b 2241  None, None, [{"A
-00018610: 223a 2031 317d 5d20 2a20 3131 2c20 5b22  ": 11}] * 11, ["
-00018620: 666f 6f62 6172 225d 202a 2031 302c 205b  foobar"] * 10, [
-00018630: 4355 5252 454e 545f 5449 4d45 5d20 2a20  CURRENT_TIME] * 
-00018640: 3130 292c 0a20 2020 2020 2020 2028 4e6f  10),.        (No
-00018650: 6e65 2c20 4e6f 6e65 2c20 5b7b 2241 223a  ne, None, [{"A":
-00018660: 2031 317d 5d20 2a20 3131 2c20 5b22 666f   11}] * 11, ["fo
-00018670: 6f62 6172 225d 202a 2031 302c 206e 702e  obar"] * 10, np.
-00018680: 6172 7261 7928 5b43 5552 5245 4e54 5f54  array([CURRENT_T
-00018690: 494d 455d 202a 2031 3029 292c 0a20 2020  IME] * 10)),.   
-000186a0: 205d 2c0a 290a 406d 6f63 6b2e 7061 7463   ],.).@mock.patc
-000186b0: 6828 2267 616e 7472 792e 6c6f 6767 6572  h("gantry.logger
-000186c0: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-000186d0: 6c6f 675f 7072 6564 6963 7469 6f6e 5f61  log_prediction_a
-000186e0: 6e64 5f66 6565 6462 6163 6b5f 6576 656e  nd_feedback_even
-000186f0: 7473 2229 0a40 6d6f 636b 2e70 6174 6368  ts").@mock.patch
-00018700: 2822 6761 6e74 7279 2e6c 6f67 6765 722e  ("gantry.logger.
-00018710: 636c 6965 6e74 2e47 616e 7472 792e 5f6c  client.Gantry._l
-00018720: 6f67 5f70 7265 6469 6374 696f 6e5f 6576  og_prediction_ev
-00018730: 656e 7473 2229 0a40 6d6f 636b 2e70 6174  ents").@mock.pat
-00018740: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
-00018750: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
-00018760: 5f6c 6f67 5f66 6565 6462 6163 6b5f 6576  _log_feedback_ev
-00018770: 656e 7473 2229 0a64 6566 2074 6573 745f  ents").def test_
-00018780: 6c6f 675f 7265 636f 7264 735f 7369 7a65  log_records_size
-00018790: 5f6d 6973 6d61 7463 6828 0a20 2020 206d  _mismatch(.    m
-000187a0: 6f63 6b5f 6665 6564 6261 636b 732c 0a20  ock_feedbacks,. 
-000187b0: 2020 206d 6f63 6b5f 7072 6564 732c 0a20     mock_preds,. 
-000187c0: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
-000187d0: 645f 6665 6564 6261 636b 2c0a 2020 2020  d_feedback,.    
-000187e0: 696e 7075 7473 2c0a 2020 2020 6f75 7470  inputs,.    outp
-000187f0: 7574 732c 0a20 2020 2066 6565 6462 6163  uts,.    feedbac
-00018800: 6b73 2c0a 2020 2020 7469 6d65 7374 616d  ks,.    timestam
-00018810: 7073 2c0a 2020 2020 6a6f 696e 5f6b 6579  ps,.    join_key
-00018820: 732c 0a20 2020 2063 6c69 5f6f 626a 2c0a  s,.    cli_obj,.
-00018830: 293a 0a20 2020 2061 7373 6572 7420 280a  ):.    assert (.
-00018840: 2020 2020 2020 2020 636c 695f 6f62 6a2e          cli_obj.
-00018850: 6c6f 675f 7265 636f 7264 7328 0a20 2020  log_records(.   
-00018860: 2020 2020 2020 2020 2061 7070 6c69 6361           applica
-00018870: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
-00018880: 2020 2020 2020 2020 2020 2076 6572 7369             versi
-00018890: 6f6e 3d22 322e 302e 3122 2c0a 2020 2020  on="2.0.1",.    
-000188a0: 2020 2020 2020 2020 696e 7075 7473 3d69          inputs=i
-000188b0: 6e70 7574 732c 0a20 2020 2020 2020 2020  nputs,.         
-000188c0: 2020 206f 7574 7075 7473 3d6f 7574 7075     outputs=outpu
-000188d0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-000188e0: 6665 6564 6261 636b 733d 6665 6564 6261  feedbacks=feedba
-000188f0: 636b 732c 0a20 2020 2020 2020 2020 2020  cks,.           
-00018900: 2074 696d 6573 7461 6d70 733d 7469 6d65   timestamps=time
-00018910: 7374 616d 7073 2c0a 2020 2020 2020 2020  stamps,.        
-00018920: 2020 2020 736f 7274 5f6f 6e5f 7469 6d65      sort_on_time
-00018930: 7374 616d 703d 5472 7565 2c0a 2020 2020  stamp=True,.    
-00018940: 2020 2020 2020 2020 6a6f 696e 5f6b 6579          join_key
-00018950: 733d 6a6f 696e 5f6b 6579 732c 0a20 2020  s=join_keys,.   
-00018960: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-00018970: 7320 4e6f 6e65 0a20 2020 2029 0a0a 2020  s None.    )..  
-00018980: 2020 6d6f 636b 5f70 7265 6473 5f61 6e64    mock_preds_and
-00018990: 5f66 6565 6462 6163 6b2e 6173 7365 7274  _feedback.assert
-000189a0: 5f6e 6f74 5f63 616c 6c65 6428 290a 2020  _not_called().  
-000189b0: 2020 6d6f 636b 5f70 7265 6473 2e61 7373    mock_preds.ass
-000189c0: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
-000189d0: 0a20 2020 206d 6f63 6b5f 6665 6564 6261  .    mock_feedba
-000189e0: 636b 732e 6173 7365 7274 5f6e 6f74 5f63  cks.assert_not_c
-000189f0: 616c 6c65 6428 290a 0a0a 4070 7974 6573  alled()...@pytes
-00018a00: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00018a10: 7a65 280a 2020 2020 5b22 696e 7075 7473  ze(.    ["inputs
-00018a20: 222c 2022 6f75 7470 7574 7322 2c20 2266  ", "outputs", "f
-00018a30: 6565 6462 6163 6b73 222c 2022 6a6f 696e  eedbacks", "join
-00018a40: 5f6b 6579 7322 2c20 2274 696d 6573 7461  _keys", "timesta
-00018a50: 6d70 7322 5d2c 0a20 2020 205b 0a20 2020  mps"],.    [.   
-00018a60: 2020 2020 2028 5b7b 2241 223a 2031 307d       ([{"A": 10}
-00018a70: 5d20 2a20 3130 2c20 5b7b 2241 223a 2031  ] * 10, [{"A": 1
-00018a80: 307d 5d20 2a20 392c 204e 6f6e 652c 204e  0}] * 9, None, N
-00018a90: 6f6e 652c 204e 6f6e 6529 2c0a 2020 2020  one, None),.    
-00018aa0: 2020 2020 285b 7b22 4122 3a20 3130 7d5d      ([{"A": 10}]
-00018ab0: 202a 2031 302c 205b 7b22 4122 3a20 3130   * 10, [{"A": 10
-00018ac0: 7d5d 202a 2039 2c20 5b7b 2241 223a 2031  }] * 9, [{"A": 1
-00018ad0: 317d 5d20 2a20 3130 2c20 5b22 666f 6f62  1}] * 10, ["foob
-00018ae0: 6172 225d 202a 2031 302c 204e 6f6e 6529  ar"] * 10, None)
-00018af0: 2c0a 2020 2020 2020 2020 285b 7b22 4122  ,.        ([{"A"
-00018b00: 3a20 3130 7d5d 202a 2039 2c20 5b7b 2241  : 10}] * 9, [{"A
-00018b10: 223a 2031 307d 5d20 2a20 382c 205b 7b22  ": 10}] * 8, [{"
-00018b20: 4122 3a20 3131 7d5d 202a 2031 302c 205b  A": 11}] * 10, [
-00018b30: 2266 6f6f 6261 7222 5d20 2a20 3130 2c20  "foobar"] * 10, 
-00018b40: 4e6f 6e65 292c 0a20 2020 2020 2020 2028  None),.        (
-00018b50: 5b7b 2241 223a 2031 307d 5d20 2a20 392c  [{"A": 10}] * 9,
-00018b60: 204e 6f6e 652c 205b 7b22 4122 3a20 3131   None, [{"A": 11
-00018b70: 7d5d 202a 2031 302c 205b 2266 6f6f 6261  }] * 10, ["fooba
-00018b80: 7222 5d20 2a20 3130 2c20 4e6f 6e65 292c  r"] * 10, None),
-00018b90: 0a20 2020 2020 2020 2028 4e6f 6e65 2c20  .        (None, 
-00018ba0: 4e6f 6e65 2c20 5b7b 2241 223a 2031 317d  None, [{"A": 11}
-00018bb0: 5d20 2a20 3131 2c20 5b22 666f 6f62 6172  ] * 11, ["foobar
-00018bc0: 225d 202a 2031 302c 204e 6f6e 6529 2c0a  "] * 10, None),.
-00018bd0: 2020 2020 2020 2020 284e 6f6e 652c 204e          (None, N
-00018be0: 6f6e 652c 205b 7b22 4122 3a20 3131 7d5d  one, [{"A": 11}]
-00018bf0: 202a 2031 312c 205b 2266 6f6f 6261 7222   * 11, ["foobar"
-00018c00: 5d20 2a20 3130 2c20 5b43 5552 5245 4e54  ] * 10, [CURRENT
-00018c10: 5f54 494d 455d 202a 2031 3029 2c0a 2020  _TIME] * 10),.  
-00018c20: 2020 2020 2020 284e 6f6e 652c 204e 6f6e        (None, Non
-00018c30: 652c 205b 7b22 4122 3a20 3131 7d5d 202a  e, [{"A": 11}] *
-00018c40: 2031 312c 205b 2266 6f6f 6261 7222 5d20   11, ["foobar"] 
-00018c50: 2a20 3130 2c20 6e70 2e61 7272 6179 285b  * 10, np.array([
-00018c60: 4355 5252 454e 545f 5449 4d45 5d20 2a20  CURRENT_TIME] * 
-00018c70: 3130 2929 2c0a 2020 2020 5d2c 0a29 0a40  10)),.    ],.).@
-00018c80: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
-00018c90: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
-00018ca0: 2e47 616e 7472 792e 5f67 656e 6572 6174  .Gantry._generat
-00018cb0: 655f 7072 6564 6963 7469 6f6e 5f61 6e64  e_prediction_and
-00018cc0: 5f66 6565 6462 6163 6b5f 6576 656e 7473  _feedback_events
-00018cd0: 2229 0a40 6d6f 636b 2e70 6174 6368 2822  ").@mock.patch("
-00018ce0: 6761 6e74 7279 2e6c 6f67 6765 722e 636c  gantry.logger.cl
-00018cf0: 6965 6e74 2e47 616e 7472 792e 5f67 656e  ient.Gantry._gen
-00018d00: 6572 6174 655f 7072 6564 6963 7469 6f6e  erate_prediction
-00018d10: 5f65 7665 6e74 7322 290a 406d 6f63 6b2e  _events").@mock.
-00018d20: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
-00018d30: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-00018d40: 7279 2e5f 6765 6e65 7261 7465 5f66 6565  ry._generate_fee
-00018d50: 6462 6163 6b5f 6576 656e 7473 2229 0a64  dback_events").d
-00018d60: 6566 2074 6573 745f 6765 6e65 7261 7465  ef test_generate
-00018d70: 5f72 6563 6f72 6473 5f73 697a 655f 6d69  _records_size_mi
-00018d80: 736d 6174 6368 280a 2020 2020 6d6f 636b  smatch(.    mock
-00018d90: 5f67 656e 6572 6174 655f 6665 6564 6261  _generate_feedba
-00018da0: 636b 732c 0a20 2020 206d 6f63 6b5f 6765  cks,.    mock_ge
-00018db0: 6e65 7261 7465 5f70 7265 6473 2c0a 2020  nerate_preds,.  
-00018dc0: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
-00018dd0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
-00018de0: 636b 2c0a 2020 2020 696e 7075 7473 2c0a  ck,.    inputs,.
-00018df0: 2020 2020 6f75 7470 7574 732c 0a20 2020      outputs,.   
-00018e00: 2066 6565 6462 6163 6b73 2c0a 2020 2020   feedbacks,.    
-00018e10: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
-00018e20: 6a6f 696e 5f6b 6579 732c 0a20 2020 2063  join_keys,.    c
-00018e30: 6c69 5f6f 626a 2c0a 293a 0a20 2020 2061  li_obj,.):.    a
-00018e40: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-00018e50: 636c 695f 6f62 6a2e 6765 6e65 7261 7465  cli_obj.generate
-00018e60: 5f72 6563 6f72 6473 280a 2020 2020 2020  _records(.      
-00018e70: 2020 2020 2020 6170 706c 6963 6174 696f        applicatio
-00018e80: 6e3d 2266 6f6f 6261 7222 2c0a 2020 2020  n="foobar",.    
-00018e90: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
-00018ea0: 2232 2e30 2e31 222c 0a20 2020 2020 2020  "2.0.1",.       
-00018eb0: 2020 2020 2069 6e70 7574 733d 696e 7075       inputs=inpu
-00018ec0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-00018ed0: 6f75 7470 7574 733d 6f75 7470 7574 732c  outputs=outputs,
-00018ee0: 0a20 2020 2020 2020 2020 2020 2066 6565  .            fee
-00018ef0: 6462 6163 6b73 3d66 6565 6462 6163 6b73  dbacks=feedbacks
-00018f00: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-00018f10: 6d65 7374 616d 7073 3d74 696d 6573 7461  mestamps=timesta
-00018f20: 6d70 732c 0a20 2020 2020 2020 2020 2020  mps,.           
-00018f30: 2073 6f72 745f 6f6e 5f74 696d 6573 7461   sort_on_timesta
-00018f40: 6d70 3d54 7275 652c 0a20 2020 2020 2020  mp=True,.       
-00018f50: 2020 2020 206a 6f69 6e5f 6b65 7973 3d6a       join_keys=j
-00018f60: 6f69 6e5f 6b65 7973 2c0a 2020 2020 2020  oin_keys,.      
-00018f70: 2020 290a 2020 2020 2020 2020 6973 204e    ).        is N
-00018f80: 6f6e 650a 2020 2020 290a 0a20 2020 206d  one.    )..    m
-00018f90: 6f63 6b5f 6765 6e65 7261 7465 5f70 7265  ock_generate_pre
-00018fa0: 6473 5f61 6e64 5f66 6565 6462 6163 6b2e  ds_and_feedback.
-00018fb0: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
-00018fc0: 6428 290a 2020 2020 6d6f 636b 5f67 656e  d().    mock_gen
-00018fd0: 6572 6174 655f 7072 6564 732e 6173 7365  erate_preds.asse
-00018fe0: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00018ff0: 2020 2020 6d6f 636b 5f67 656e 6572 6174      mock_generat
-00019000: 655f 6665 6564 6261 636b 732e 6173 7365  e_feedbacks.asse
-00019010: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00019020: 0a0a 4070 7974 6573 742e 6d61 726b 2e70  ..@pytest.mark.p
-00019030: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
-00019040: 5b22 696e 7075 7473 222c 2022 6f75 7470  ["inputs", "outp
-00019050: 7574 7322 2c20 2266 6565 6462 6163 6b73  uts", "feedbacks
-00019060: 222c 2022 6a6f 696e 5f6b 6579 7322 2c20  ", "join_keys", 
-00019070: 2274 696d 6573 7461 6d70 7322 5d2c 0a20  "timestamps"],. 
-00019080: 2020 205b 0a20 2020 2020 2020 2028 5b7b     [.        ([{
-00019090: 2241 223a 2031 307d 5d20 2a20 3130 2c20  "A": 10}] * 10, 
-000190a0: 5b7b 2241 223a 2031 307d 5d20 2a20 3130  [{"A": 10}] * 10
-000190b0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
-000190c0: 6e65 292c 0a20 2020 2020 2020 2028 5b7b  ne),.        ([{
-000190d0: 2241 223a 2031 307d 5d20 2a20 3130 2c20  "A": 10}] * 10, 
-000190e0: 5b7b 2241 223a 2031 307d 5d20 2a20 3130  [{"A": 10}] * 10
-000190f0: 2c20 5b7b 2241 223a 2031 317d 5d20 2a20  , [{"A": 11}] * 
-00019100: 3130 2c20 5b22 666f 6f62 6172 225d 202a  10, ["foobar"] *
-00019110: 2031 302c 204e 6f6e 6529 2c0a 2020 2020   10, None),.    
-00019120: 2020 2020 285b 7b22 4122 3a20 3130 7d5d      ([{"A": 10}]
-00019130: 202a 2031 302c 205b 7b22 4122 3a20 3130   * 10, [{"A": 10
-00019140: 7d5d 202a 2031 302c 205b 7b22 4122 3a20  }] * 10, [{"A": 
-00019150: 3131 7d5d 202a 2031 302c 205b 2266 6f6f  11}] * 10, ["foo
-00019160: 6261 7222 5d20 2a20 3130 2c20 4e6f 6e65  bar"] * 10, None
-00019170: 292c 0a20 2020 2020 2020 2028 4e6f 6e65  ),.        (None
-00019180: 2c20 4e6f 6e65 2c20 5b7b 2241 223a 2031  , None, [{"A": 1
-00019190: 317d 5d20 2a20 3130 2c20 5b22 666f 6f62  1}] * 10, ["foob
-000191a0: 6172 225d 202a 2031 302c 204e 6f6e 6529  ar"] * 10, None)
-000191b0: 2c0a 2020 2020 2020 2020 284e 6f6e 652c  ,.        (None,
-000191c0: 204e 6f6e 652c 205b 7b22 4122 3a20 3131   None, [{"A": 11
-000191d0: 7d5d 202a 2031 302c 205b 2266 6f6f 6261  }] * 10, ["fooba
-000191e0: 7222 5d20 2a20 3130 2c20 5b43 5552 5245  r"] * 10, [CURRE
-000191f0: 4e54 5f54 494d 455d 202a 2031 3029 2c0a  NT_TIME] * 10),.
-00019200: 2020 2020 2020 2020 284e 6f6e 652c 204e          (None, N
-00019210: 6f6e 652c 205b 7b22 4122 3a20 3131 7d5d  one, [{"A": 11}]
-00019220: 202a 2031 302c 205b 2266 6f6f 6261 7222   * 10, ["foobar"
-00019230: 5d20 2a20 3130 2c20 6e70 2e61 7272 6179  ] * 10, np.array
-00019240: 285b 4355 5252 454e 545f 5449 4d45 5d20  ([CURRENT_TIME] 
-00019250: 2a20 3130 2929 2c0a 2020 2020 5d2c 0a29  * 10)),.    ],.)
-00019260: 0a40 6d6f 636b 2e70 6174 6368 280a 2020  .@mock.patch(.  
-00019270: 2020 2267 616e 7472 792e 6c6f 6767 6572    "gantry.logger
-00019280: 2e63 6c69 656e 742e 4761 6e74 7279 2e5f  .client.Gantry._
-00019290: 6c6f 675f 7072 6564 6963 7469 6f6e 5f61  log_prediction_a
-000192a0: 6e64 5f66 6565 6462 6163 6b5f 6576 656e  nd_feedback_even
-000192b0: 7473 222c 0a20 2020 2072 6574 7572 6e5f  ts",.    return_
-000192c0: 7661 6c75 653d 284e 6f6e 652c 205b 2231  value=(None, ["1
-000192d0: 3233 3435 222c 2022 3637 3839 3022 5d29  2345", "67890"])
-000192e0: 2c0a 290a 406d 6f63 6b2e 7061 7463 6828  ,.).@mock.patch(
-000192f0: 0a20 2020 2022 6761 6e74 7279 2e6c 6f67  .    "gantry.log
-00019300: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-00019310: 792e 5f6c 6f67 5f70 7265 6469 6374 696f  y._log_predictio
-00019320: 6e5f 6576 656e 7473 222c 2072 6574 7572  n_events", retur
-00019330: 6e5f 7661 6c75 653d 284e 6f6e 652c 205b  n_value=(None, [
-00019340: 2231 3233 3435 222c 2022 3637 3839 3022  "12345", "67890"
-00019350: 5d29 0a29 0a40 6d6f 636b 2e70 6174 6368  ]).).@mock.patch
-00019360: 280a 2020 2020 2267 616e 7472 792e 6c6f  (.    "gantry.lo
-00019370: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
-00019380: 7279 2e5f 6c6f 675f 6665 6564 6261 636b  ry._log_feedback
-00019390: 5f65 7665 6e74 7322 2c20 7265 7475 726e  _events", return
-000193a0: 5f76 616c 7565 3d28 4e6f 6e65 2c20 5b22  _value=(None, ["
-000193b0: 3132 3334 3522 2c20 2236 3738 3930 225d  12345", "67890"]
-000193c0: 290a 290a 6465 6620 7465 7374 5f6c 6f67  ).).def test_log
-000193d0: 5f72 6563 6f72 6473 5f73 697a 655f 6d61  _records_size_ma
-000193e0: 7463 6828 0a20 2020 206d 6f63 6b5f 6665  tch(.    mock_fe
-000193f0: 6564 6261 636b 732c 0a20 2020 206d 6f63  edbacks,.    moc
-00019400: 6b5f 7072 6564 732c 0a20 2020 206d 6f63  k_preds,.    moc
-00019410: 6b5f 7072 6564 735f 616e 645f 6665 6564  k_preds_and_feed
-00019420: 6261 636b 2c0a 2020 2020 696e 7075 7473  back,.    inputs
-00019430: 2c0a 2020 2020 6f75 7470 7574 732c 0a20  ,.    outputs,. 
-00019440: 2020 2066 6565 6462 6163 6b73 2c0a 2020     feedbacks,.  
-00019450: 2020 7469 6d65 7374 616d 7073 2c0a 2020    timestamps,.  
-00019460: 2020 6a6f 696e 5f6b 6579 732c 0a20 2020    join_keys,.   
-00019470: 2063 6c69 5f6f 626a 2c0a 293a 0a20 2020   cli_obj,.):.   
-00019480: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
-00019490: 2020 636c 695f 6f62 6a2e 6c6f 675f 7265    cli_obj.log_re
-000194a0: 636f 7264 7328 0a20 2020 2020 2020 2020  cords(.         
-000194b0: 2020 2061 7070 6c69 6361 7469 6f6e 3d22     application="
-000194c0: 666f 6f62 6172 222c 0a20 2020 2020 2020  foobar",.       
-000194d0: 2020 2020 2076 6572 7369 6f6e 3d22 322e       version="2.
-000194e0: 302e 3122 2c0a 2020 2020 2020 2020 2020  0.1",.          
-000194f0: 2020 696e 7075 7473 3d69 6e70 7574 732c    inputs=inputs,
-00019500: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00019510: 7075 7473 3d6f 7574 7075 7473 2c0a 2020  puts=outputs,.  
-00019520: 2020 2020 2020 2020 2020 6665 6564 6261            feedba
-00019530: 636b 733d 6665 6564 6261 636b 732c 0a20  cks=feedbacks,. 
-00019540: 2020 2020 2020 2020 2020 2074 696d 6573             times
-00019550: 7461 6d70 733d 7469 6d65 7374 616d 7073  tamps=timestamps
-00019560: 2c0a 2020 2020 2020 2020 2020 2020 736f  ,.            so
-00019570: 7274 5f6f 6e5f 7469 6d65 7374 616d 703d  rt_on_timestamp=
-00019580: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00019590: 2020 6a6f 696e 5f6b 6579 733d 6a6f 696e    join_keys=join
-000195a0: 5f6b 6579 732c 0a20 2020 2020 2020 2029  _keys,.        )
-000195b0: 0a20 2020 2020 2020 2069 7320 6e6f 7420  .        is not 
-000195c0: 4e6f 6e65 0a20 2020 2029 0a0a 0a40 7079  None.    )...@py
-000195d0: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
-000195e0: 7472 697a 6528 0a20 2020 205b 2269 6e70  trize(.    ["inp
-000195f0: 7574 7322 2c20 226f 7574 7075 7473 222c  uts", "outputs",
-00019600: 2022 6665 6564 6261 636b 7322 2c20 226a   "feedbacks", "j
-00019610: 6f69 6e5f 6b65 7973 222c 2022 7469 6d65  oin_keys", "time
-00019620: 7374 616d 7073 225d 2c0a 2020 2020 5b0a  stamps"],.    [.
-00019630: 2020 2020 2020 2020 285b 7b22 4122 3a20          ([{"A": 
-00019640: 3130 7d5d 202a 2031 302c 205b 7b22 4122  10}] * 10, [{"A"
-00019650: 3a20 3130 7d5d 202a 2031 302c 204e 6f6e  : 10}] * 10, Non
-00019660: 652c 204e 6f6e 652c 204e 6f6e 6529 2c0a  e, None, None),.
-00019670: 2020 2020 2020 2020 285b 7b22 4122 3a20          ([{"A": 
-00019680: 3130 7d5d 202a 2031 302c 205b 7b22 4122  10}] * 10, [{"A"
-00019690: 3a20 3130 7d5d 202a 2031 302c 205b 7b22  : 10}] * 10, [{"
-000196a0: 4122 3a20 3131 7d5d 202a 2031 302c 205b  A": 11}] * 10, [
-000196b0: 2266 6f6f 6261 7222 5d20 2a20 3130 2c20  "foobar"] * 10, 
-000196c0: 4e6f 6e65 292c 0a20 2020 2020 2020 2028  None),.        (
-000196d0: 5b7b 2241 223a 2031 307d 5d20 2a20 3130  [{"A": 10}] * 10
-000196e0: 2c20 5b7b 2241 223a 2031 307d 5d20 2a20  , [{"A": 10}] * 
-000196f0: 3130 2c20 5b7b 2241 223a 2031 317d 5d20  10, [{"A": 11}] 
-00019700: 2a20 3130 2c20 5b22 666f 6f62 6172 225d  * 10, ["foobar"]
-00019710: 202a 2031 302c 204e 6f6e 6529 2c0a 2020   * 10, None),.  
-00019720: 2020 2020 2020 284e 6f6e 652c 204e 6f6e        (None, Non
-00019730: 652c 205b 7b22 4122 3a20 3131 7d5d 202a  e, [{"A": 11}] *
-00019740: 2031 302c 205b 2266 6f6f 6261 7222 5d20   10, ["foobar"] 
-00019750: 2a20 3130 2c20 4e6f 6e65 292c 0a20 2020  * 10, None),.   
-00019760: 2020 2020 2028 4e6f 6e65 2c20 4e6f 6e65       (None, None
-00019770: 2c20 5b7b 2241 223a 2031 317d 5d20 2a20  , [{"A": 11}] * 
-00019780: 3130 2c20 5b22 666f 6f62 6172 225d 202a  10, ["foobar"] *
-00019790: 2031 302c 205b 4355 5252 454e 545f 5449   10, [CURRENT_TI
-000197a0: 4d45 5d20 2a20 3130 292c 0a20 2020 2020  ME] * 10),.     
-000197b0: 2020 2028 4e6f 6e65 2c20 4e6f 6e65 2c20     (None, None, 
-000197c0: 5b7b 2241 223a 2031 317d 5d20 2a20 3130  [{"A": 11}] * 10
-000197d0: 2c20 5b22 666f 6f62 6172 225d 202a 2031  , ["foobar"] * 1
-000197e0: 302c 206e 702e 6172 7261 7928 5b43 5552  0, np.array([CUR
-000197f0: 5245 4e54 5f54 494d 455d 202a 2031 3029  RENT_TIME] * 10)
-00019800: 292c 0a20 2020 205d 2c0a 290a 406d 6f63  ),.    ],.).@moc
-00019810: 6b2e 7061 7463 6828 0a20 2020 2022 6761  k.patch(.    "ga
-00019820: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
-00019830: 6e74 2e47 616e 7472 792e 5f67 656e 6572  nt.Gantry._gener
-00019840: 6174 655f 7072 6564 6963 7469 6f6e 5f61  ate_prediction_a
-00019850: 6e64 5f66 6565 6462 6163 6b5f 6576 656e  nd_feedback_even
-00019860: 7473 222c 0a20 2020 2072 6574 7572 6e5f  ts",.    return_
-00019870: 7661 6c75 653d 284e 6f6e 652c 205b 2231  value=(None, ["1
-00019880: 3233 3435 222c 2022 3637 3839 3022 5d29  2345", "67890"])
-00019890: 2c0a 290a 406d 6f63 6b2e 7061 7463 6828  ,.).@mock.patch(
-000198a0: 0a20 2020 2022 6761 6e74 7279 2e6c 6f67  .    "gantry.log
-000198b0: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
-000198c0: 792e 5f67 656e 6572 6174 655f 7072 6564  y._generate_pred
-000198d0: 6963 7469 6f6e 5f65 7665 6e74 7322 2c0a  iction_events",.
-000198e0: 2020 2020 7265 7475 726e 5f76 616c 7565      return_value
-000198f0: 3d28 4e6f 6e65 2c20 5b22 3132 3334 3522  =(None, ["12345"
-00019900: 2c20 2236 3738 3930 225d 292c 0a29 0a40  , "67890"]),.).@
-00019910: 6d6f 636b 2e70 6174 6368 280a 2020 2020  mock.patch(.    
-00019920: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
-00019930: 6c69 656e 742e 4761 6e74 7279 2e5f 6765  lient.Gantry._ge
-00019940: 6e65 7261 7465 5f66 6565 6462 6163 6b5f  nerate_feedback_
-00019950: 6576 656e 7473 222c 2072 6574 7572 6e5f  events", return_
-00019960: 7661 6c75 653d 284e 6f6e 652c 205b 2231  value=(None, ["1
-00019970: 3233 3435 222c 2022 3637 3839 3022 5d29  2345", "67890"])
-00019980: 0a29 0a64 6566 2074 6573 745f 6765 6e65  .).def test_gene
-00019990: 7261 7465 5f72 6563 6f72 6473 5f73 697a  rate_records_siz
-000199a0: 655f 6d61 7463 6828 0a20 2020 206d 6f63  e_match(.    moc
-000199b0: 6b5f 6765 6e65 7261 7465 5f66 6565 6462  k_generate_feedb
-000199c0: 6163 6b73 2c0a 2020 2020 6d6f 636b 5f67  acks,.    mock_g
-000199d0: 656e 6572 6174 655f 7072 6564 732c 0a20  enerate_preds,. 
-000199e0: 2020 206d 6f63 6b5f 6765 6e65 7261 7465     mock_generate
-000199f0: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
-00019a00: 6163 6b2c 0a20 2020 2069 6e70 7574 732c  ack,.    inputs,
-00019a10: 0a20 2020 206f 7574 7075 7473 2c0a 2020  .    outputs,.  
-00019a20: 2020 6665 6564 6261 636b 732c 0a20 2020    feedbacks,.   
-00019a30: 2074 696d 6573 7461 6d70 732c 0a20 2020   timestamps,.   
-00019a40: 206a 6f69 6e5f 6b65 7973 2c0a 2020 2020   join_keys,.    
-00019a50: 636c 695f 6f62 6a2c 0a29 3a0a 2020 2020  cli_obj,.):.    
-00019a60: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
-00019a70: 2063 6c69 5f6f 626a 2e67 656e 6572 6174   cli_obj.generat
-00019a80: 655f 7265 636f 7264 7328 0a20 2020 2020  e_records(.     
-00019a90: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
-00019aa0: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
-00019ab0: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
-00019ac0: 3d22 322e 302e 3122 2c0a 2020 2020 2020  ="2.0.1",.      
-00019ad0: 2020 2020 2020 696e 7075 7473 3d69 6e70        inputs=inp
-00019ae0: 7574 732c 0a20 2020 2020 2020 2020 2020  uts,.           
-00019af0: 206f 7574 7075 7473 3d6f 7574 7075 7473   outputs=outputs
-00019b00: 2c0a 2020 2020 2020 2020 2020 2020 6665  ,.            fe
-00019b10: 6564 6261 636b 733d 6665 6564 6261 636b  edbacks=feedback
-00019b20: 732c 0a20 2020 2020 2020 2020 2020 2074  s,.            t
-00019b30: 696d 6573 7461 6d70 733d 7469 6d65 7374  imestamps=timest
-00019b40: 616d 7073 2c0a 2020 2020 2020 2020 2020  amps,.          
-00019b50: 2020 736f 7274 5f6f 6e5f 7469 6d65 7374    sort_on_timest
-00019b60: 616d 703d 5472 7565 2c0a 2020 2020 2020  amp=True,.      
-00019b70: 2020 2020 2020 6a6f 696e 5f6b 6579 733d        join_keys=
-00019b80: 6a6f 696e 5f6b 6579 732c 0a20 2020 2020  join_keys,.     
-00019b90: 2020 2029 0a20 2020 2020 2020 2069 7320     ).        is 
-00019ba0: 6e6f 7420 4e6f 6e65 0a20 2020 2029 0a0a  not None.    )..
-00019bb0: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
-00019bc0: 7261 6d65 7472 697a 6528 0a20 2020 2028  rametrize(.    (
-00019bd0: 2274 696d 6573 7461 6d70 222c 2022 696e  "timestamp", "in
-00019be0: 7075 7473 222c 2022 6f75 7470 7574 7322  puts", "outputs"
-00019bf0: 2c20 2266 6565 6462 6163 6b73 222c 2022  , "feedbacks", "
-00019c00: 6a6f 696e 5f6b 6579 222c 2022 676c 6f62  join_key", "glob
-00019c10: 616c 5f74 6167 7322 2c20 2272 6f77 5f74  al_tags", "row_t
-00019c20: 6167 7322 292c 0a20 2020 205b 2020 2320  ags"),.    [  # 
-00019c30: 5465 7374 2061 6c6c 2063 6f6d 6269 6e61  Test all combina
-00019c40: 7469 6f6e 7320 6f66 2069 6e70 7574 732c  tions of inputs,
-00019c50: 206f 7574 7075 7473 2c20 6665 6564 6261   outputs, feedba
-00019c60: 636b 732c 2061 6e64 206a 6f69 6e5f 6b65  cks, and join_ke
-00019c70: 790a 2020 2020 2020 2020 2822 5422 2c20  y.        ("T", 
-00019c80: 5b22 4122 2c20 2242 225d 2c20 5b22 4322  ["A", "B"], ["C"
-00019c90: 2c20 2244 225d 2c20 5b22 4822 2c20 2249  , "D"], ["H", "I
-00019ca0: 225d 2c20 2245 222c 207b 2276 6572 7369  "], "E", {"versi
-00019cb0: 6f6e 223a 2022 7465 7374 5f76 6572 7369  on": "test_versi
-00019cc0: 6f6e 227d 2c20 5b22 4722 5d29 2c0a 2020  on"}, ["G"]),.  
-00019cd0: 2020 2020 2020 2320 5465 7374 2077 6974        # Test wit
-00019ce0: 686f 7574 2066 6565 6462 6163 6b73 2061  hout feedbacks a
-00019cf0: 6e64 2072 6f77 5f74 6167 730a 2020 2020  nd row_tags.    
-00019d00: 2020 2020 2822 5422 2c20 5b22 4122 2c20      ("T", ["A", 
-00019d10: 2242 225d 2c20 5b22 4422 5d2c 204e 6f6e  "B"], ["D"], Non
-00019d20: 652c 2022 4522 2c20 7b22 7665 7273 696f  e, "E", {"versio
-00019d30: 6e22 3a20 2274 6573 745f 7665 7273 696f  n": "test_versio
-00019d40: 6e22 7d2c 204e 6f6e 6529 2c0a 2020 2020  n"}, None),.    
-00019d50: 2020 2020 2320 5465 7374 2077 6974 686f      # Test witho
-00019d60: 7574 2069 6e70 7574 7320 616e 6420 7469  ut inputs and ti
-00019d70: 6d65 7374 616d 700a 2020 2020 2020 2020  mestamp.        
-00019d80: 284e 6f6e 652c 204e 6f6e 652c 204e 6f6e  (None, None, Non
-00019d90: 652c 205b 2248 222c 2022 4922 5d2c 2022  e, ["H", "I"], "
-00019da0: 4522 2c20 7b22 7665 7273 696f 6e22 3a20  E", {"version": 
-00019db0: 2274 6573 745f 7665 7273 696f 6e22 7d2c  "test_version"},
-00019dc0: 205b 2247 225d 292c 0a20 2020 2020 2020   ["G"]),.       
-00019dd0: 2023 2054 6573 7420 6f6e 6c79 2077 6974   # Test only wit
-00019de0: 6820 6665 6564 6261 636b 7320 616e 6420  h feedbacks and 
-00019df0: 6a6f 696e 5f6b 6579 0a20 2020 2020 2020  join_key.       
-00019e00: 2028 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f   (None, None, No
-00019e10: 6e65 2c20 5b22 4822 2c20 2249 225d 2c20  ne, ["H", "I"], 
-00019e20: 2245 222c 204e 6f6e 652c 204e 6f6e 6529  "E", None, None)
-00019e30: 2c0a 2020 2020 2020 2020 2320 5465 7374  ,.        # Test
-00019e40: 206f 6e6c 7920 7769 7468 2069 6e70 7574   only with input
-00019e50: 7320 616e 6420 676c 6f62 616c 2074 6167  s and global tag
-00019e60: 730a 2020 2020 2020 2020 2822 5422 2c20  s.        ("T", 
-00019e70: 5b22 4122 2c20 2242 225d 2c20 5b22 4322  ["A", "B"], ["C"
-00019e80: 2c20 2244 225d 2c20 4e6f 6e65 2c20 4e6f  , "D"], None, No
-00019e90: 6e65 2c20 7b22 7665 7273 696f 6e22 3a20  ne, {"version": 
-00019ea0: 2274 6573 745f 7665 7273 696f 6e22 7d2c  "test_version"},
-00019eb0: 204e 6f6e 6529 2c0a 2020 2020 5d2c 0a29   None),.    ],.)
-00019ec0: 0a64 6566 2074 6573 745f 6c6f 675f 6672  .def test_log_fr
-00019ed0: 6f6d 5f64 6174 615f 636f 6e6e 6563 746f  om_data_connecto
-00019ee0: 7228 0a20 2020 2074 696d 6573 7461 6d70  r(.    timestamp
-00019ef0: 3a20 7374 722c 0a20 2020 2069 6e70 7574  : str,.    input
-00019f00: 733a 204c 6973 745b 7374 725d 2c0a 2020  s: List[str],.  
-00019f10: 2020 6f75 7470 7574 733a 204c 6973 745b    outputs: List[
-00019f20: 7374 725d 2c0a 2020 2020 6665 6564 6261  str],.    feedba
-00019f30: 636b 733a 204c 6973 745b 7374 725d 2c0a  cks: List[str],.
-00019f40: 2020 2020 6a6f 696e 5f6b 6579 3a20 7374      join_key: st
-00019f50: 722c 0a20 2020 2072 6f77 5f74 6167 733a  r,.    row_tags:
-00019f60: 204c 6973 745b 7374 725d 2c0a 2020 2020   List[str],.    
-00019f70: 676c 6f62 616c 5f74 6167 733a 2044 6963  global_tags: Dic
-00019f80: 745b 7374 722c 2073 7472 5d2c 0a20 2020  t[str, str],.   
-00019f90: 2063 6c69 5f6f 626a 2c0a 293a 0a20 2020   cli_obj,.):.   
-00019fa0: 2022 2222 0a20 2020 2054 6573 7473 2074   """.    Tests t
-00019fb0: 6861 7420 7468 6520 6c6f 675f 6672 6f6d  hat the log_from
-00019fc0: 5f64 6174 615f 636f 6e6e 6563 746f 7220  _data_connector 
-00019fd0: 6675 6e63 7469 6f6e 2063 616c 6c73 2074  function calls t
-00019fe0: 6865 206c 6f67 5f66 726f 6d5f 6461 7461  he log_from_data
-00019ff0: 5f63 6f6e 6e65 6374 6f72 5f61 7379 6e63  _connector_async
-0001a000: 0a20 2020 2066 756e 6374 696f 6e20 7769  .    function wi
-0001a010: 7468 2063 6f72 7265 6374 2070 6172 616d  th correct param
-0001a020: 6574 6572 730a 2020 2020 2222 220a 2020  eters.    """.  
-0001a030: 2020 636c 695f 6f62 6a2e 6c6f 675f 7374    cli_obj.log_st
-0001a040: 6f72 6520 3d20 6d6f 636b 2e4d 6f63 6b28  ore = mock.Mock(
-0001a050: 290a 2020 2020 636c 695f 6f62 6a2e 6c6f  ).    cli_obj.lo
-0001a060: 675f 6672 6f6d 5f64 6174 615f 636f 6e6e  g_from_data_conn
-0001a070: 6563 746f 7228 0a20 2020 2020 2020 2061  ector(.        a
-0001a080: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
-0001a090: 6172 222c 0a20 2020 2020 2020 2073 6f75  ar",.        sou
-0001a0a0: 7263 655f 6461 7461 5f63 6f6e 6e65 6374  rce_data_connect
-0001a0b0: 6f72 5f6e 616d 653d 2274 6573 742d 636f  or_name="test-co
-0001a0c0: 6e6e 6563 746f 7222 2c0a 2020 2020 2020  nnector",.      
-0001a0d0: 2020 7469 6d65 7374 616d 703d 7469 6d65    timestamp=time
-0001a0e0: 7374 616d 702c 0a20 2020 2020 2020 2069  stamp,.        i
-0001a0f0: 6e70 7574 733d 696e 7075 7473 2c0a 2020  nputs=inputs,.  
-0001a100: 2020 2020 2020 6f75 7470 7574 733d 6f75        outputs=ou
-0001a110: 7470 7574 732c 0a20 2020 2020 2020 2066  tputs,.        f
-0001a120: 6565 6462 6163 6b73 3d66 6565 6462 6163  eedbacks=feedbac
-0001a130: 6b73 2c0a 2020 2020 2020 2020 6a6f 696e  ks,.        join
-0001a140: 5f6b 6579 3d6a 6f69 6e5f 6b65 792c 0a20  _key=join_key,. 
-0001a150: 2020 2020 2020 2072 6f77 5f74 6167 733d         row_tags=
-0001a160: 726f 775f 7461 6773 2c0a 2020 2020 2020  row_tags,.      
-0001a170: 2020 676c 6f62 616c 5f74 6167 733d 676c    global_tags=gl
-0001a180: 6f62 616c 5f74 6167 732c 0a20 2020 2029  obal_tags,.    )
-0001a190: 0a0a 2020 2020 6361 6c6c 5f61 7267 7320  ..    call_args 
-0001a1a0: 3d20 636c 695f 6f62 6a2e 6c6f 675f 7374  = cli_obj.log_st
-0001a1b0: 6f72 652e 6c6f 675f 6672 6f6d 5f64 6174  ore.log_from_dat
-0001a1c0: 615f 636f 6e6e 6563 746f 725f 6173 796e  a_connector_asyn
-0001a1d0: 632e 6361 6c6c 5f61 7267 730a 2020 2020  c.call_args.    
-0001a1e0: 6173 7365 7274 2063 616c 6c5f 6172 6773  assert call_args
-0001a1f0: 2e6b 7761 7267 7320 3d3d 207b 0a20 2020  .kwargs == {.   
-0001a200: 2020 2020 2022 7265 7175 6573 7422 3a20       "request": 
-0001a210: 496e 6765 7374 4672 6f6d 4461 7461 436f  IngestFromDataCo
-0001a220: 6e6e 6563 746f 7252 6571 7565 7374 280a  nnectorRequest(.
-0001a230: 2020 2020 2020 2020 2020 2020 6170 706c              appl
-0001a240: 6963 6174 696f 6e3d 2266 6f6f 6261 7222  ication="foobar"
-0001a250: 2c0a 2020 2020 2020 2020 2020 2020 736f  ,.            so
-0001a260: 7572 6365 5f64 6174 615f 636f 6e6e 6563  urce_data_connec
-0001a270: 746f 725f 6e61 6d65 3d22 7465 7374 2d63  tor_name="test-c
-0001a280: 6f6e 6e65 6374 6f72 222c 0a20 2020 2020  onnector",.     
-0001a290: 2020 2020 2020 2074 696d 6573 7461 6d70         timestamp
-0001a2a0: 3d74 696d 6573 7461 6d70 2c0a 2020 2020  =timestamp,.    
-0001a2b0: 2020 2020 2020 2020 696e 7075 7473 3d69          inputs=i
-0001a2c0: 6e70 7574 732c 0a20 2020 2020 2020 2020  nputs,.         
-0001a2d0: 2020 206f 7574 7075 7473 3d6f 7574 7075     outputs=outpu
-0001a2e0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-0001a2f0: 6665 6564 6261 636b 733d 6665 6564 6261  feedbacks=feedba
-0001a300: 636b 732c 0a20 2020 2020 2020 2020 2020  cks,.           
-0001a310: 206a 6f69 6e5f 6b65 793d 6a6f 696e 5f6b   join_key=join_k
-0001a320: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
-0001a330: 726f 775f 7461 6773 3d72 6f77 5f74 6167  row_tags=row_tag
-0001a340: 732c 0a20 2020 2020 2020 2020 2020 2067  s,.            g
-0001a350: 6c6f 6261 6c5f 7461 6773 3d67 6c6f 6261  lobal_tags=globa
-0001a360: 6c5f 7461 6773 2c0a 2020 2020 2020 2020  l_tags,.        
-0001a370: 2020 2020 7363 6865 6475 6c65 3d4e 6f6e      schedule=Non
-0001a380: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
-0001a390: 6970 656c 696e 655f 6e61 6d65 3d4e 6f6e  ipeline_name=Non
-0001a3a0: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
-0001a3b0: 207d 0a0a 0a40 7079 7465 7374 2e6d 6172   }...@pytest.mar
-0001a3c0: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
-0001a3d0: 2020 2028 2273 7461 7274 5f6f 6e22 2c20     ("start_on", 
-0001a3e0: 2266 7265 7175 656e 6379 222c 2022 7479  "frequency", "ty
-0001a3f0: 7065 222c 2022 6f70 7469 6f6e 7322 292c  pe", "options"),
-0001a400: 0a20 2020 205b 0a20 2020 2020 2020 2028  .    [.        (
-0001a410: 0a20 2020 2020 2020 2020 2020 2022 3230  .            "20
-0001a420: 3233 2d30 322d 3031 5430 303a 3030 3a30  23-02-01T00:00:0
-0001a430: 302e 3030 3030 3030 222c 0a20 2020 2020  0.000000",.     
-0001a440: 2020 2020 2020 2053 6368 6564 756c 6546         ScheduleF
-0001a450: 7265 7175 656e 6379 2e45 5645 5259 5f48  requency.EVERY_H
-0001a460: 4f55 522c 0a20 2020 2020 2020 2020 2020  OUR,.           
-0001a470: 2053 6368 6564 756c 6554 7970 652e 494e   ScheduleType.IN
-0001a480: 4352 454d 454e 5441 4c5f 4150 5045 4e44  CREMENTAL_APPEND
-0001a490: 2c0a 2020 2020 2020 2020 2020 2020 7b22  ,.            {"
-0001a4a0: 7761 7465 726d 6172 6b5f 6b65 7922 3a20  watermark_key": 
-0001a4b0: 2275 7064 6174 6564 5f61 7422 7d2c 0a20  "updated_at"},. 
-0001a4c0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-0001a4d0: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-0001a4e0: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-0001a4f0: 652e 7574 636e 6f77 2829 2c0a 2020 2020  e.utcnow(),.    
-0001a500: 2020 2020 2020 2020 5363 6865 6475 6c65          Schedule
-0001a510: 4672 6571 7565 6e63 792e 4556 4552 595f  Frequency.EVERY_
-0001a520: 325f 484f 5552 532c 0a20 2020 2020 2020  2_HOURS,.       
-0001a530: 2020 2020 2053 6368 6564 756c 6554 7970       ScheduleTyp
-0001a540: 652e 494e 4352 454d 454e 5441 4c5f 4150  e.INCREMENTAL_AP
-0001a550: 5045 4e44 2c0a 2020 2020 2020 2020 2020  PEND,.          
-0001a560: 2020 7b22 7761 7465 726d 6172 6b5f 6b65    {"watermark_ke
-0001a570: 7922 3a20 4e6f 6e65 7d2c 0a20 2020 2020  y": None},.     
-0001a580: 2020 2029 2c0a 2020 2020 2020 2020 280a     ),.        (.
-0001a590: 2020 2020 2020 2020 2020 2020 6461 7465              date
-0001a5a0: 7469 6d65 2e64 6174 6574 696d 652e 7574  time.datetime.ut
-0001a5b0: 636e 6f77 2829 2c0a 2020 2020 2020 2020  cnow(),.        
-0001a5c0: 2020 2020 5363 6865 6475 6c65 4672 6571      ScheduleFreq
-0001a5d0: 7565 6e63 792e 4556 4552 595f 345f 484f  uency.EVERY_4_HO
-0001a5e0: 5552 532c 0a20 2020 2020 2020 2020 2020  URS,.           
-0001a5f0: 2053 6368 6564 756c 6554 7970 652e 494e   ScheduleType.IN
-0001a600: 4352 454d 454e 5441 4c5f 4150 5045 4e44  CREMENTAL_APPEND
-0001a610: 2c0a 2020 2020 2020 2020 2020 2020 7b22  ,.            {"
-0001a620: 7761 7465 726d 6172 6b5f 6b65 7922 3a20  watermark_key": 
-0001a630: 2275 7064 6174 6564 5f61 7422 7d2c 0a20  "updated_at"},. 
-0001a640: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-0001a650: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-0001a660: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-0001a670: 652e 7574 636e 6f77 2829 2c0a 2020 2020  e.utcnow(),.    
-0001a680: 2020 2020 2020 2020 5363 6865 6475 6c65          Schedule
-0001a690: 4672 6571 7565 6e63 792e 4556 4552 595f  Frequency.EVERY_
-0001a6a0: 345f 484f 5552 532c 0a20 2020 2020 2020  4_HOURS,.       
-0001a6b0: 2020 2020 2053 6368 6564 756c 6554 7970       ScheduleTyp
-0001a6c0: 652e 494e 4352 454d 454e 5441 4c5f 4150  e.INCREMENTAL_AP
-0001a6d0: 5045 4e44 2c0a 2020 2020 2020 2020 2020  PEND,.          
-0001a6e0: 2020 7b22 6465 6c61 795f 7469 6d65 223a    {"delay_time":
-0001a6f0: 2033 3030 2c20 2277 6174 6572 6d61 726b   300, "watermark
-0001a700: 5f6b 6579 223a 2022 7570 6461 7465 645f  _key": "updated_
-0001a710: 6174 227d 2c0a 2020 2020 2020 2020 292c  at"},.        ),
-0001a720: 0a20 2020 205d 2c0a 290a 6465 6620 7465  .    ],.).def te
-0001a730: 7374 5f6c 6f67 5f66 726f 6d5f 6461 7461  st_log_from_data
-0001a740: 5f63 6f6e 6e65 6374 6f72 5f77 6974 685f  _connector_with_
-0001a750: 7363 6865 6475 6c65 280a 2020 2020 7374  schedule(.    st
-0001a760: 6172 745f 6f6e 3a20 556e 696f 6e5b 6461  art_on: Union[da
-0001a770: 7465 7469 6d65 2e64 6174 6574 696d 652c  tetime.datetime,
-0001a780: 2073 7472 5d2c 0a20 2020 2066 7265 7175   str],.    frequ
-0001a790: 656e 6379 3a20 5363 6865 6475 6c65 4672  ency: ScheduleFr
-0001a7a0: 6571 7565 6e63 792c 0a20 2020 2074 7970  equency,.    typ
-0001a7b0: 653a 2053 6368 6564 756c 6554 7970 652c  e: ScheduleType,
-0001a7c0: 0a20 2020 206f 7074 696f 6e73 3a20 4469  .    options: Di
-0001a7d0: 6374 5b73 7472 2c20 7374 725d 2c0a 2020  ct[str, str],.  
-0001a7e0: 2020 636c 695f 6f62 6a2c 0a29 3a0a 2020    cli_obj,.):.  
-0001a7f0: 2020 2222 220a 2020 2020 5465 7374 7320    """.    Tests 
-0001a800: 7468 6174 2074 6865 206c 6f67 5f66 726f  that the log_fro
-0001a810: 6d5f 6461 7461 5f63 6f6e 6e65 6374 6f72  m_data_connector
-0001a820: 2066 756e 6374 696f 6e20 6361 6c6c 7320   function calls 
-0001a830: 7468 6520 6c6f 675f 6672 6f6d 5f64 6174  the log_from_dat
-0001a840: 615f 636f 6e6e 6563 746f 725f 6173 796e  a_connector_asyn
-0001a850: 630a 2020 2020 6675 6e63 7469 6f6e 2077  c.    function w
-0001a860: 6974 6820 636f 7272 6563 7420 7061 7261  ith correct para
-0001a870: 6d65 7465 7273 0a20 2020 2022 2222 0a20  meters.    """. 
-0001a880: 2020 2063 6c69 5f6f 626a 2e6c 6f67 5f73     cli_obj.log_s
-0001a890: 746f 7265 203d 206d 6f63 6b2e 4d6f 636b  tore = mock.Mock
-0001a8a0: 2829 0a20 2020 2063 6c69 5f6f 626a 2e6c  ().    cli_obj.l
-0001a8b0: 6f67 5f66 726f 6d5f 6461 7461 5f63 6f6e  og_from_data_con
-0001a8c0: 6e65 6374 6f72 280a 2020 2020 2020 2020  nector(.        
-0001a8d0: 6170 706c 6963 6174 696f 6e3d 2266 6f6f  application="foo
-0001a8e0: 6261 7222 2c0a 2020 2020 2020 2020 736f  bar",.        so
-0001a8f0: 7572 6365 5f64 6174 615f 636f 6e6e 6563  urce_data_connec
-0001a900: 746f 725f 6e61 6d65 3d22 7465 7374 2d63  tor_name="test-c
-0001a910: 6f6e 6e65 6374 6f72 222c 0a20 2020 2020  onnector",.     
-0001a920: 2020 2074 696d 6573 7461 6d70 3d22 5422     timestamp="T"
-0001a930: 2c0a 2020 2020 2020 2020 696e 7075 7473  ,.        inputs
-0001a940: 3d5b 2241 222c 2022 4222 5d2c 0a20 2020  =["A", "B"],.   
-0001a950: 2020 2020 206f 7574 7075 7473 3d5b 2243       outputs=["C
-0001a960: 222c 2022 4422 5d2c 0a20 2020 2020 2020  ", "D"],.       
-0001a970: 2066 6565 6462 6163 6b73 3d5b 2245 222c   feedbacks=["E",
-0001a980: 2022 4622 5d2c 0a20 2020 2020 2020 206a   "F"],.        j
-0001a990: 6f69 6e5f 6b65 793d 2248 222c 0a20 2020  oin_key="H",.   
-0001a9a0: 2020 2020 2072 6f77 5f74 6167 733d 5b22       row_tags=["
-0001a9b0: 4922 2c20 224a 225d 2c0a 2020 2020 2020  I", "J"],.      
-0001a9c0: 2020 676c 6f62 616c 5f74 6167 733d 7b22    global_tags={"
-0001a9d0: 7665 7273 696f 6e22 3a20 2274 6573 745f  version": "test_
-0001a9e0: 7665 7273 696f 6e22 7d2c 0a20 2020 2020  version"},.     
-0001a9f0: 2020 2073 6368 6564 756c 653d 5363 6865     schedule=Sche
-0001aa00: 6475 6c65 280a 2020 2020 2020 2020 2020  dule(.          
-0001aa10: 2020 7374 6172 745f 6f6e 3d73 7461 7274    start_on=start
-0001aa20: 5f6f 6e2c 0a20 2020 2020 2020 2020 2020  _on,.           
-0001aa30: 2066 7265 7175 656e 6379 3d66 7265 7175   frequency=frequ
-0001aa40: 656e 6379 2c0a 2020 2020 2020 2020 2020  ency,.          
-0001aa50: 2020 7479 7065 3d74 7970 652c 0a20 2020    type=type,.   
-0001aa60: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-0001aa70: 3d53 6368 6564 756c 654f 7074 696f 6e73  =ScheduleOptions
-0001aa80: 282a 2a6f 7074 696f 6e73 292c 2020 2320  (**options),  # 
-0001aa90: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-0001aaa0: 2020 2020 2029 2c0a 2020 2020 290a 0a20       ),.    ).. 
-0001aab0: 2020 2063 616c 6c5f 6172 6773 203d 2063     call_args = c
-0001aac0: 6c69 5f6f 626a 2e6c 6f67 5f73 746f 7265  li_obj.log_store
-0001aad0: 2e6c 6f67 5f66 726f 6d5f 6461 7461 5f63  .log_from_data_c
-0001aae0: 6f6e 6e65 6374 6f72 5f61 7379 6e63 2e63  onnector_async.c
-0001aaf0: 616c 6c5f 6172 6773 0a20 2020 2061 7373  all_args.    ass
-0001ab00: 6572 7420 6361 6c6c 5f61 7267 732e 6b77  ert call_args.kw
-0001ab10: 6172 6773 203d 3d20 7b0a 2020 2020 2020  args == {.      
-0001ab20: 2020 2272 6571 7565 7374 223a 2049 6e67    "request": Ing
-0001ab30: 6573 7446 726f 6d44 6174 6143 6f6e 6e65  estFromDataConne
-0001ab40: 6374 6f72 5265 7175 6573 7428 0a20 2020  ctorRequest(.   
-0001ab50: 2020 2020 2020 2020 2061 7070 6c69 6361           applica
-0001ab60: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
-0001ab70: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-0001ab80: 655f 6461 7461 5f63 6f6e 6e65 6374 6f72  e_data_connector
-0001ab90: 5f6e 616d 653d 2274 6573 742d 636f 6e6e  _name="test-conn
-0001aba0: 6563 746f 7222 2c0a 2020 2020 2020 2020  ector",.        
-0001abb0: 2020 2020 7469 6d65 7374 616d 703d 2254      timestamp="T
-0001abc0: 222c 0a20 2020 2020 2020 2020 2020 2069  ",.            i
-0001abd0: 6e70 7574 733d 5b22 4122 2c20 2242 225d  nputs=["A", "B"]
-0001abe0: 2c0a 2020 2020 2020 2020 2020 2020 6f75  ,.            ou
-0001abf0: 7470 7574 733d 5b22 4322 2c20 2244 225d  tputs=["C", "D"]
-0001ac00: 2c0a 2020 2020 2020 2020 2020 2020 6665  ,.            fe
-0001ac10: 6564 6261 636b 733d 5b22 4522 2c20 2246  edbacks=["E", "F
-0001ac20: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-0001ac30: 6a6f 696e 5f6b 6579 3d22 4822 2c0a 2020  join_key="H",.  
-0001ac40: 2020 2020 2020 2020 2020 726f 775f 7461            row_ta
-0001ac50: 6773 3d5b 2249 222c 2022 4a22 5d2c 0a20  gs=["I", "J"],. 
-0001ac60: 2020 2020 2020 2020 2020 2067 6c6f 6261             globa
-0001ac70: 6c5f 7461 6773 3d7b 2276 6572 7369 6f6e  l_tags={"version
-0001ac80: 223a 2022 7465 7374 5f76 6572 7369 6f6e  ": "test_version
-0001ac90: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
-0001aca0: 7363 6865 6475 6c65 3d53 6368 6564 756c  schedule=Schedul
-0001acb0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0001acc0: 2020 2073 7461 7274 5f6f 6e3d 7374 6172     start_on=star
-0001acd0: 745f 6f6e 2e69 736f 666f 726d 6174 2829  t_on.isoformat()
-0001ace0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001acf0: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-0001ad00: 7461 7274 5f6f 6e2c 2064 6174 6574 696d  tart_on, datetim
-0001ad10: 652e 6461 7465 7469 6d65 290a 2020 2020  e.datetime).    
-0001ad20: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001ad30: 2073 7461 7274 5f6f 6e2c 0a20 2020 2020   start_on,.     
-0001ad40: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
-0001ad50: 656e 6379 3d66 7265 7175 656e 6379 2c0a  ency=frequency,.
-0001ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad70: 7479 7065 3d74 7970 652c 0a20 2020 2020  type=type,.     
-0001ad80: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-0001ad90: 6e73 3d53 6368 6564 756c 654f 7074 696f  ns=ScheduleOptio
-0001ada0: 6e73 282a 2a6f 7074 696f 6e73 292c 2020  ns(**options),  
-0001adb0: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
-0001adc0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-0001add0: 2020 2020 2020 2020 2020 7069 7065 6c69            pipeli
-0001ade0: 6e65 5f6e 616d 653d 4e6f 6e65 2c0a 2020  ne_name=None,.  
-0001adf0: 2020 2020 2020 290a 2020 2020 7d0a             ).    }.
+00015fd0: 742e 5f72 6573 6f6c 7665 5f6a 6f69 6e5f  t._resolve_join_
+00015fe0: 6b65 7973 222c 2072 6574 7572 6e5f 7661  keys", return_va
+00015ff0: 6c75 653d 5b22 3132 3334 3522 2c20 2235  lue=["12345", "5
+00016000: 3433 3231 225d 290a 406d 6f63 6b2e 7061  4321"]).@mock.pa
+00016010: 7463 6828 2267 616e 7472 792e 6c6f 6767  tch("gantry.logg
+00016020: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
+00016030: 2e5f 6765 6e65 7261 7465 5f70 7265 6469  ._generate_predi
+00016040: 6374 696f 6e5f 616e 645f 6665 6564 6261  ction_and_feedba
+00016050: 636b 5f65 7665 6e74 7322 290a 406d 6f63  ck_events").@moc
+00016060: 6b2e 7061 7463 6828 2267 616e 7472 792e  k.patch("gantry.
+00016070: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
+00016080: 6e74 7279 2e5f 6765 6e65 7261 7465 5f70  ntry._generate_p
+00016090: 7265 6469 6374 696f 6e5f 6576 656e 7473  rediction_events
+000160a0: 2229 0a40 6d6f 636b 2e70 6174 6368 280a  ").@mock.patch(.
+000160b0: 2020 2020 2267 616e 7472 792e 6c6f 6767      "gantry.logg
+000160c0: 6572 2e63 6c69 656e 742e 4761 6e74 7279  er.client.Gantry
+000160d0: 2e5f 6765 6e65 7261 7465 5f66 6565 6462  ._generate_feedb
+000160e0: 6163 6b5f 6576 656e 7473 222c 0a20 2020  ack_events",.   
+000160f0: 2072 6574 7572 6e5f 7661 6c75 653d 285b   return_value=([
+00016100: 7b22 6576 656e 7422 3a20 2270 6c61 6365  {"event": "place
+00016110: 5f68 6f6c 6465 7222 7d5d 2c20 5b22 3132  _holder"}], ["12
+00016120: 3334 3522 2c20 2236 3738 3930 225d 292c  345", "67890"]),
+00016130: 0a29 0a40 6d6f 636b 2e70 6174 6368 2822  .).@mock.patch("
+00016140: 6761 6e74 7279 2e6c 6f67 6765 722e 636c  gantry.logger.cl
+00016150: 6965 6e74 2e5f 7361 6d70 6c65 5f72 6563  ient._sample_rec
+00016160: 6f72 6473 222c 2073 6964 655f 6566 6665  ords", side_effe
+00016170: 6374 3d63 6c69 656e 742e 5f73 616d 706c  ct=client._sampl
+00016180: 655f 7265 636f 7264 7329 0a64 6566 2074  e_records).def t
+00016190: 6573 745f 6765 6e65 7261 7465 5f72 6563  est_generate_rec
+000161a0: 6f72 6473 5f66 6565 6462 6163 6b5f 6f6e  ords_feedback_on
+000161b0: 6c79 280a 2020 2020 6d6f 636b 5f73 616d  ly(.    mock_sam
+000161c0: 706c 655f 7265 636f 7264 732c 0a20 2020  ple_records,.   
+000161d0: 206d 6f63 6b5f 6765 6e65 7261 7465 5f66   mock_generate_f
+000161e0: 6565 6462 6163 6b2c 0a20 2020 206d 6f63  eedback,.    moc
+000161f0: 6b5f 6765 6e65 7261 7465 5f70 7265 6473  k_generate_preds
+00016200: 2c0a 2020 2020 6d6f 636b 5f67 656e 6572  ,.    mock_gener
+00016210: 6174 655f 7072 6564 735f 616e 645f 6665  ate_preds_and_fe
+00016220: 6564 6261 636b 2c0a 2020 2020 6d6f 636b  edback,.    mock
+00016230: 5f72 6573 6f6c 7665 5f6a 6f69 6e5f 6b65  _resolve_join_ke
+00016240: 7973 2c0a 2020 2020 7665 7273 696f 6e2c  ys,.    version,
+00016250: 0a20 2020 2074 6167 732c 0a20 2020 2072  .    tags,.    r
+00016260: 6f77 5f74 6167 732c 0a20 2020 2067 6c6f  ow_tags,.    glo
+00016270: 6261 6c5f 7461 6773 2c0a 2020 2020 6578  bal_tags,.    ex
+00016280: 7065 6374 6564 5f74 6167 735f 7061 7261  pected_tags_para
+00016290: 6d2c 0a20 2020 2074 6573 745f 6665 6564  m,.    test_feed
+000162a0: 6261 636b 732c 0a20 2020 2074 6573 745f  backs,.    test_
+000162b0: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
+000162c0: 7465 7374 5f74 696d 6573 7461 6d70 735f  test_timestamps_
+000162d0: 6c69 7374 2c0a 2020 2020 6b77 6172 6773  list,.    kwargs
+000162e0: 2c0a 2020 2020 636c 695f 6f62 6a2c 0a29  ,.    cli_obj,.)
+000162f0: 3a0a 2020 2020 6966 2069 7369 6e73 7461  :.    if isinsta
+00016300: 6e63 6528 7461 6773 2c20 6c69 7374 293a  nce(tags, list):
+00016310: 0a20 2020 2020 2020 2070 7974 6573 742e  .        pytest.
+00016320: 736b 6970 2822 5468 6973 2074 6573 7420  skip("This test 
+00016330: 6973 206e 6f74 2061 7070 6c69 6361 626c  is not applicabl
+00016340: 6520 746f 206c 6973 7420 7461 6773 2229  e to list tags")
+00016350: 0a0a 2020 2020 7275 6e5f 6964 203d 2073  ..    run_id = s
+00016360: 7472 2875 7569 642e 7575 6964 3428 2929  tr(uuid.uuid4())
+00016370: 0a20 2020 2072 756e 5f74 6167 7320 3d20  .    run_tags = 
+00016380: 4e6f 6e65 0a20 2020 2069 6620 7461 6773  None.    if tags
+00016390: 2061 6e64 2067 6c6f 6261 6c5f 7461 6773   and global_tags
+000163a0: 3a0a 2020 2020 2020 2020 7275 6e5f 7461  :.        run_ta
+000163b0: 6773 203d 207b 2a2a 7461 6773 2c20 2a2a  gs = {**tags, **
+000163c0: 676c 6f62 616c 5f74 6167 737d 0a20 2020  global_tags}.   
+000163d0: 2065 6c69 6620 7461 6773 3a0a 2020 2020   elif tags:.    
+000163e0: 2020 2020 7275 6e5f 7461 6773 203d 2074      run_tags = t
+000163f0: 6167 730a 2020 2020 656c 6966 2067 6c6f  ags.    elif glo
+00016400: 6261 6c5f 7461 6773 3a0a 2020 2020 2020  bal_tags:.      
+00016410: 2020 7275 6e5f 7461 6773 203d 2067 6c6f    run_tags = glo
+00016420: 6261 6c5f 7461 6773 0a20 2020 2061 7373  bal_tags.    ass
+00016430: 6572 7420 636c 695f 6f62 6a2e 6c6f 6728  ert cli_obj.log(
+00016440: 0a20 2020 2020 2020 2061 7070 6c69 6361  .        applica
+00016450: 7469 6f6e 3d22 666f 6f62 6172 222c 0a20  tion="foobar",. 
+00016460: 2020 2020 2020 2076 6572 7369 6f6e 3d76         version=v
+00016470: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
+00016480: 696e 7075 7473 3d4e 6f6e 652c 0a20 2020  inputs=None,.   
+00016490: 2020 2020 206f 7574 7075 7473 3d4e 6f6e       outputs=Non
+000164a0: 652c 0a20 2020 2020 2020 2066 6565 6462  e,.        feedb
+000164b0: 6163 6b73 3d74 6573 745f 6665 6564 6261  acks=test_feedba
+000164c0: 636b 732c 0a20 2020 2020 2020 2074 696d  cks,.        tim
+000164d0: 6573 7461 6d70 733d 7465 7374 5f74 696d  estamps=test_tim
+000164e0: 6573 7461 6d70 732c 0a20 2020 2020 2020  estamps,.       
+000164f0: 2073 6f72 745f 6f6e 5f74 696d 6573 7461   sort_on_timesta
+00016500: 6d70 3d54 7275 652c 0a20 2020 2020 2020  mp=True,.       
+00016510: 2072 6f77 5f74 6167 733d 726f 775f 7461   row_tags=row_ta
+00016520: 6773 2c0a 2020 2020 2020 2020 7275 6e5f  gs,.        run_
+00016530: 7461 6773 3d72 756e 5f74 6167 732c 0a20  tags=run_tags,. 
+00016540: 2020 2020 2020 2072 756e 5f69 643d 7275         run_id=ru
+00016550: 6e5f 6964 2c0a 2020 2020 2020 2020 2a2a  n_id,.        **
+00016560: 6b77 6172 6773 2c0a 2020 2020 2920 3d3d  kwargs,.    ) ==
+00016570: 205b 7b22 6576 656e 7422 3a20 2270 6c61   [{"event": "pla
+00016580: 6365 5f68 6f6c 6465 7222 7d5d 0a0a 2020  ce_holder"}]..  
+00016590: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
+000165a0: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+000165b0: 636b 2e61 7373 6572 745f 6e6f 745f 6361  ck.assert_not_ca
+000165c0: 6c6c 6564 2829 0a20 2020 206d 6f63 6b5f  lled().    mock_
+000165d0: 6765 6e65 7261 7465 5f70 7265 6473 2e61  generate_preds.a
+000165e0: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
+000165f0: 2829 0a20 2020 206d 6f63 6b5f 6765 6e65  ().    mock_gene
+00016600: 7261 7465 5f66 6565 6462 6163 6b2e 6173  rate_feedback.as
+00016610: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+00016620: 5f77 6974 6828 0a20 2020 2020 2020 2061  _with(.        a
+00016630: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
+00016640: 6172 222c 0a20 2020 2020 2020 2066 6565  ar",.        fee
+00016650: 6462 6163 6b73 3d5b 7b22 4122 3a20 3230  dbacks=[{"A": 20
+00016660: 307d 2c20 7b22 4122 3a20 3230 317d 5d2c  0}, {"A": 201}],
+00016670: 0a20 2020 2020 2020 206a 6f69 6e5f 6b65  .        join_ke
+00016680: 7973 3d5b 2231 3233 3435 222c 2022 3534  ys=["12345", "54
+00016690: 3332 3122 5d2c 0a20 2020 2020 2020 2066  321"],.        f
+000166a0: 6565 6462 6163 6b5f 7665 7273 696f 6e3d  eedback_version=
+000166b0: 7665 7273 696f 6e2c 0a20 2020 2020 2020  version,.       
+000166c0: 2074 696d 6573 7461 6d70 733d 7465 7374   timestamps=test
+000166d0: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
+000166e0: 2c0a 2020 2020 2020 2020 736f 7274 5f6f  ,.        sort_o
+000166f0: 6e5f 7469 6d65 7374 616d 703d 5472 7565  n_timestamp=True
+00016700: 2c0a 2020 2020 2020 2020 7275 6e5f 6964  ,.        run_id
+00016710: 3d72 756e 5f69 642c 0a20 2020 2020 2020  =run_id,.       
+00016720: 2074 6167 733d 6578 7065 6374 6564 5f74   tags=expected_t
+00016730: 6167 735f 7061 7261 6d2c 0a20 2020 2029  ags_param,.    )
+00016740: 0a0a 2020 2020 6d6f 636b 5f73 616d 706c  ..    mock_sampl
+00016750: 655f 7265 636f 7264 732e 6173 7365 7274  e_records.assert
+00016760: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+00016770: 6828 0a20 2020 2020 2020 2032 2c0a 2020  h(.        2,.  
+00016780: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+00016790: 204e 6f6e 652c 0a20 2020 2020 2020 204e   None,.        N
+000167a0: 6f6e 652c 0a20 2020 2020 2020 205b 7b22  one,.        [{"
+000167b0: 4122 3a20 3230 307d 2c20 7b22 4122 3a20  A": 200}, {"A": 
+000167c0: 3230 317d 5d2c 0a20 2020 2020 2020 2063  201}],.        c
+000167d0: 6c69 656e 742e 5f72 6573 6f6c 7665 5f6a  lient._resolve_j
+000167e0: 6f69 6e5f 6b65 7973 282a 2a6b 7761 7267  oin_keys(**kwarg
+000167f0: 7329 2c0a 2020 2020 2020 2020 7465 7374  s),.        test
+00016800: 5f74 696d 6573 7461 6d70 735f 6c69 7374  _timestamps_list
+00016810: 2c0a 2020 2020 2020 2020 6578 7065 6374  ,.        expect
+00016820: 6564 5f74 6167 735f 7061 7261 6d2c 0a20  ed_tags_param,. 
+00016830: 2020 2029 0a0a 0a40 7079 7465 7374 2e6d     )...@pytest.m
+00016840: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00016850: 2274 6573 745f 6665 6564 6261 636b 7322  "test_feedbacks"
+00016860: 2c20 5445 5354 5f46 4545 4442 4143 4b53  , TEST_FEEDBACKS
+00016870: 290a 4070 7974 6573 742e 6d61 726b 2e70  ).@pytest.mark.p
+00016880: 6172 616d 6574 7269 7a65 2822 7665 7273  arametrize("vers
+00016890: 696f 6e22 2c20 5b4e 6f6e 652c 2031 302c  ion", [None, 10,
+000168a0: 2022 312e 322e 3322 5d29 0a40 6d6f 636b   "1.2.3"]).@mock
+000168b0: 2e70 6174 6368 2822 6761 6e74 7279 2e6c  .patch("gantry.l
+000168c0: 6f67 6765 722e 636c 6965 6e74 2e47 616e  ogger.client.Gan
+000168d0: 7472 792e 5f6c 6f67 5f70 7265 6469 6374  try._log_predict
+000168e0: 696f 6e5f 616e 645f 6665 6564 6261 636b  ion_and_feedback
+000168f0: 5f65 7665 6e74 7322 290a 406d 6f63 6b2e  _events").@mock.
+00016900: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+00016910: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
+00016920: 7279 2e5f 6c6f 675f 7072 6564 6963 7469  ry._log_predicti
+00016930: 6f6e 5f65 7665 6e74 7322 290a 406d 6f63  on_events").@moc
+00016940: 6b2e 7061 7463 6828 0a20 2020 2022 6761  k.patch(.    "ga
+00016950: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+00016960: 6e74 2e47 616e 7472 792e 5f6c 6f67 5f66  nt.Gantry._log_f
+00016970: 6565 6462 6163 6b5f 6576 656e 7473 222c  eedback_events",
+00016980: 2072 6574 7572 6e5f 7661 6c75 653d 284e   return_value=(N
+00016990: 6f6e 652c 205b 2231 3233 3435 222c 2022  one, ["12345", "
+000169a0: 3637 3839 3022 5d29 0a29 0a64 6566 2074  67890"]).).def t
+000169b0: 6573 745f 6c6f 675f 7265 636f 7264 735f  est_log_records_
+000169c0: 6665 6564 6261 636b 5f6f 6e6c 795f 6e6f  feedback_only_no
+000169d0: 5f6a 6f69 6e5f 6b65 7973 280a 2020 2020  _join_keys(.    
+000169e0: 6d6f 636b 5f66 6565 6462 6163 6b2c 0a20  mock_feedback,. 
+000169f0: 2020 206d 6f63 6b5f 7072 6564 732c 0a20     mock_preds,. 
+00016a00: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
+00016a10: 645f 6665 6564 6261 636b 2c0a 2020 2020  d_feedback,.    
+00016a20: 7665 7273 696f 6e2c 0a20 2020 2074 6573  version,.    tes
+00016a30: 745f 6665 6564 6261 636b 732c 0a20 2020  t_feedbacks,.   
+00016a40: 2063 6c69 5f6f 626a 2c0a 293a 0a20 2020   cli_obj,.):.   
+00016a50: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
+00016a60: 2020 636c 695f 6f62 6a2e 6c6f 675f 7265    cli_obj.log_re
+00016a70: 636f 7264 7328 0a20 2020 2020 2020 2020  cords(.         
+00016a80: 2020 2061 7070 6c69 6361 7469 6f6e 3d22     application="
+00016a90: 666f 6f62 6172 222c 0a20 2020 2020 2020  foobar",.       
+00016aa0: 2020 2020 2076 6572 7369 6f6e 3d76 6572       version=ver
+00016ab0: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+00016ac0: 2020 696e 7075 7473 3d4e 6f6e 652c 0a20    inputs=None,. 
+00016ad0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00016ae0: 7473 3d4e 6f6e 652c 0a20 2020 2020 2020  ts=None,.       
+00016af0: 2020 2020 2066 6565 6462 6163 6b73 3d74       feedbacks=t
+00016b00: 6573 745f 6665 6564 6261 636b 732c 0a20  est_feedbacks,. 
+00016b10: 2020 2020 2020 2020 2020 2074 696d 6573             times
+00016b20: 7461 6d70 733d 4e6f 6e65 2c0a 2020 2020  tamps=None,.    
+00016b30: 2020 2020 2020 2020 736f 7274 5f6f 6e5f          sort_on_
+00016b40: 7469 6d65 7374 616d 703d 5472 7565 2c0a  timestamp=True,.
+00016b50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00016b60: 2020 6973 204e 6f6e 650a 2020 2020 290a    is None.    ).
+00016b70: 0a20 2020 206d 6f63 6b5f 7072 6564 735f  .    mock_preds_
+00016b80: 616e 645f 6665 6564 6261 636b 2e61 7373  and_feedback.ass
+00016b90: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
+00016ba0: 0a20 2020 206d 6f63 6b5f 7072 6564 732e  .    mock_preds.
+00016bb0: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
+00016bc0: 6428 290a 2020 2020 6d6f 636b 5f66 6565  d().    mock_fee
+00016bd0: 6462 6163 6b2e 6173 7365 7274 5f6e 6f74  dback.assert_not
+00016be0: 5f63 616c 6c65 6428 290a 0a0a 4070 7974  _called()...@pyt
+00016bf0: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
+00016c00: 7269 7a65 2822 7465 7374 5f66 6565 6462  rize("test_feedb
+00016c10: 6163 6b73 222c 2054 4553 545f 4645 4544  acks", TEST_FEED
+00016c20: 4241 434b 5329 0a40 7079 7465 7374 2e6d  BACKS).@pytest.m
+00016c30: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00016c40: 2276 6572 7369 6f6e 222c 205b 4e6f 6e65  "version", [None
+00016c50: 2c20 3130 2c20 2231 2e32 2e33 225d 290a  , 10, "1.2.3"]).
+00016c60: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
+00016c70: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
+00016c80: 742e 4761 6e74 7279 2e5f 6765 6e65 7261  t.Gantry._genera
+00016c90: 7465 5f70 7265 6469 6374 696f 6e5f 616e  te_prediction_an
+00016ca0: 645f 6665 6564 6261 636b 5f65 7665 6e74  d_feedback_event
+00016cb0: 7322 290a 406d 6f63 6b2e 7061 7463 6828  s").@mock.patch(
+00016cc0: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
+00016cd0: 6c69 656e 742e 4761 6e74 7279 2e5f 6765  lient.Gantry._ge
+00016ce0: 6e65 7261 7465 5f70 7265 6469 6374 696f  nerate_predictio
+00016cf0: 6e5f 6576 656e 7473 2229 0a40 6d6f 636b  n_events").@mock
+00016d00: 2e70 6174 6368 280a 2020 2020 2267 616e  .patch(.    "gan
+00016d10: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
+00016d20: 742e 4761 6e74 7279 2e5f 6765 6e65 7261  t.Gantry._genera
+00016d30: 7465 5f66 6565 6462 6163 6b5f 6576 656e  te_feedback_even
+00016d40: 7473 222c 2072 6574 7572 6e5f 7661 6c75  ts", return_valu
+00016d50: 653d 284e 6f6e 652c 205b 2231 3233 3435  e=(None, ["12345
+00016d60: 222c 2022 3637 3839 3022 5d29 0a29 0a64  ", "67890"]).).d
+00016d70: 6566 2074 6573 745f 6765 6e65 7261 7465  ef test_generate
+00016d80: 5f72 6563 6f72 6473 5f66 6565 6462 6163  _records_feedbac
+00016d90: 6b5f 6f6e 6c79 5f6e 6f5f 6a6f 696e 5f6b  k_only_no_join_k
+00016da0: 6579 7328 0a20 2020 206d 6f63 6b5f 6665  eys(.    mock_fe
+00016db0: 6564 6261 636b 2c0a 2020 2020 6d6f 636b  edback,.    mock
+00016dc0: 5f70 7265 6473 2c0a 2020 2020 6d6f 636b  _preds,.    mock
+00016dd0: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
+00016de0: 6163 6b2c 0a20 2020 2076 6572 7369 6f6e  ack,.    version
+00016df0: 2c0a 2020 2020 7465 7374 5f66 6565 6462  ,.    test_feedb
+00016e00: 6163 6b73 2c0a 2020 2020 636c 695f 6f62  acks,.    cli_ob
+00016e10: 6a2c 0a29 3a0a 2020 2020 6173 7365 7274  j,.):.    assert
+00016e20: 2028 0a20 2020 2020 2020 2063 6c69 5f6f   (.        cli_o
+00016e30: 626a 2e67 656e 6572 6174 655f 7265 636f  bj.generate_reco
+00016e40: 7264 7328 0a20 2020 2020 2020 2020 2020  rds(.           
+00016e50: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
+00016e60: 6f62 6172 222c 0a20 2020 2020 2020 2020  obar",.         
+00016e70: 2020 2076 6572 7369 6f6e 3d76 6572 7369     version=versi
+00016e80: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00016e90: 696e 7075 7473 3d4e 6f6e 652c 0a20 2020  inputs=None,.   
+00016ea0: 2020 2020 2020 2020 206f 7574 7075 7473           outputs
+00016eb0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00016ec0: 2020 2066 6565 6462 6163 6b73 3d74 6573     feedbacks=tes
+00016ed0: 745f 6665 6564 6261 636b 732c 0a20 2020  t_feedbacks,.   
+00016ee0: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
+00016ef0: 6d70 733d 4e6f 6e65 2c0a 2020 2020 2020  mps=None,.      
+00016f00: 2020 2020 2020 736f 7274 5f6f 6e5f 7469        sort_on_ti
+00016f10: 6d65 7374 616d 703d 5472 7565 2c0a 2020  mestamp=True,.  
+00016f20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00016f30: 6973 204e 6f6e 650a 2020 2020 290a 0a20  is None.    ).. 
+00016f40: 2020 206d 6f63 6b5f 7072 6564 735f 616e     mock_preds_an
+00016f50: 645f 6665 6564 6261 636b 2e61 7373 6572  d_feedback.asser
+00016f60: 745f 6e6f 745f 6361 6c6c 6564 2829 0a20  t_not_called(). 
+00016f70: 2020 206d 6f63 6b5f 7072 6564 732e 6173     mock_preds.as
+00016f80: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
+00016f90: 290a 2020 2020 6d6f 636b 5f66 6565 6462  ).    mock_feedb
+00016fa0: 6163 6b2e 6173 7365 7274 5f6e 6f74 5f63  ack.assert_not_c
+00016fb0: 616c 6c65 6428 290a 0a0a 4070 7974 6573  alled()...@pytes
+00016fc0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+00016fd0: 7a65 280a 2020 2020 2822 7465 7374 5f66  ze(.    ("test_f
+00016fe0: 6565 6462 6163 6b73 222c 2022 7465 7374  eedbacks", "test
+00016ff0: 5f6f 7574 7075 7473 222c 2022 7465 7374  _outputs", "test
+00017000: 5f69 6e70 7574 7322 292c 0a20 2020 205b  _inputs"),.    [
+00017010: 0a20 2020 2020 2020 2028 4e6f 6e65 2c20  .        (None, 
+00017020: 4e6f 6e65 2c20 4e6f 6e65 292c 0a20 2020  None, None),.   
+00017030: 2020 2020 2028 7064 2e44 6174 6146 7261       (pd.DataFra
+00017040: 6d65 2829 2c20 7064 2e44 6174 6146 7261  me(), pd.DataFra
+00017050: 6d65 2829 2c20 7064 2e44 6174 6146 7261  me(), pd.DataFra
+00017060: 6d65 2829 292c 0a20 2020 2020 2020 2028  me()),.        (
+00017070: 5b5d 2c20 5b5d 2c20 5b5d 292c 0a20 2020  [], [], []),.   
+00017080: 2020 2020 2028 7064 2e53 6572 6965 7328       (pd.Series(
+00017090: 292c 2070 642e 5365 7269 6573 2829 2c20  ), pd.Series(), 
+000170a0: 7064 2e53 6572 6965 7328 2929 2c0a 2020  pd.Series()),.  
+000170b0: 2020 2020 2020 286e 702e 6172 7261 7928        (np.array(
+000170c0: 5b5d 292c 206e 702e 6172 7261 7928 5b5d  []), np.array([]
+000170d0: 292c 206e 702e 6172 7261 7928 5b5d 2929  ), np.array([]))
+000170e0: 2c0a 2020 2020 5d2c 0a29 0a40 7079 7465  ,.    ],.).@pyte
+000170f0: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
+00017100: 697a 6528 2276 6572 7369 6f6e 222c 205b  ize("version", [
+00017110: 4e6f 6e65 2c20 3130 2c20 2231 2e32 2e33  None, 10, "1.2.3
+00017120: 225d 290a 406d 6f63 6b2e 7061 7463 6828  "]).@mock.patch(
+00017130: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
+00017140: 6c69 656e 742e 4761 6e74 7279 2e5f 6c6f  lient.Gantry._lo
+00017150: 675f 7072 6564 6963 7469 6f6e 5f61 6e64  g_prediction_and
+00017160: 5f66 6565 6462 6163 6b5f 6576 656e 7473  _feedback_events
+00017170: 2229 0a40 6d6f 636b 2e70 6174 6368 2822  ").@mock.patch("
+00017180: 6761 6e74 7279 2e6c 6f67 6765 722e 636c  gantry.logger.cl
+00017190: 6965 6e74 2e47 616e 7472 792e 5f6c 6f67  ient.Gantry._log
+000171a0: 5f70 7265 6469 6374 696f 6e5f 6576 656e  _prediction_even
+000171b0: 7473 2229 0a40 6d6f 636b 2e70 6174 6368  ts").@mock.patch
+000171c0: 2822 6761 6e74 7279 2e6c 6f67 6765 722e  ("gantry.logger.
+000171d0: 636c 6965 6e74 2e47 616e 7472 792e 5f6c  client.Gantry._l
+000171e0: 6f67 5f66 6565 6462 6163 6b5f 6576 656e  og_feedback_even
+000171f0: 7473 2229 0a64 6566 2074 6573 745f 6c6f  ts").def test_lo
+00017200: 675f 7265 636f 7264 735f 6e6f 5f64 6174  g_records_no_dat
+00017210: 6128 0a20 2020 206d 6f63 6b5f 6665 6564  a(.    mock_feed
+00017220: 6261 636b 2c0a 2020 2020 6d6f 636b 5f70  back,.    mock_p
+00017230: 7265 6473 2c0a 2020 2020 6d6f 636b 5f70  reds,.    mock_p
+00017240: 7265 6473 5f61 6e64 5f66 6565 6462 6163  reds_and_feedbac
+00017250: 6b2c 0a20 2020 2076 6572 7369 6f6e 2c0a  k,.    version,.
+00017260: 2020 2020 7465 7374 5f69 6e70 7574 732c      test_inputs,
+00017270: 0a20 2020 2074 6573 745f 6f75 7470 7574  .    test_output
+00017280: 732c 0a20 2020 2074 6573 745f 6665 6564  s,.    test_feed
+00017290: 6261 636b 732c 0a20 2020 2063 6c69 5f6f  backs,.    cli_o
+000172a0: 626a 2c0a 293a 0a20 2020 2061 7373 6572  bj,.):.    asser
+000172b0: 7420 280a 2020 2020 2020 2020 636c 695f  t (.        cli_
+000172c0: 6f62 6a2e 6c6f 675f 7265 636f 7264 7328  obj.log_records(
+000172d0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+000172e0: 6c69 6361 7469 6f6e 3d22 666f 6f62 6172  lication="foobar
+000172f0: 222c 0a20 2020 2020 2020 2020 2020 2076  ",.            v
+00017300: 6572 7369 6f6e 3d76 6572 7369 6f6e 2c0a  ersion=version,.
+00017310: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+00017320: 7473 3d74 6573 745f 696e 7075 7473 2c0a  ts=test_inputs,.
+00017330: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00017340: 7574 733d 7465 7374 5f6f 7574 7075 7473  uts=test_outputs
+00017350: 2c0a 2020 2020 2020 2020 2020 2020 6665  ,.            fe
+00017360: 6564 6261 636b 733d 7465 7374 5f66 6565  edbacks=test_fee
+00017370: 6462 6163 6b73 2c0a 2020 2020 2020 2020  dbacks,.        
+00017380: 2020 2020 7469 6d65 7374 616d 7073 3d4e      timestamps=N
+00017390: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000173a0: 2073 6f72 745f 6f6e 5f74 696d 6573 7461   sort_on_timesta
+000173b0: 6d70 3d54 7275 652c 0a20 2020 2020 2020  mp=True,.       
+000173c0: 2029 0a20 2020 2020 2020 2069 7320 4e6f   ).        is No
+000173d0: 6e65 0a20 2020 2029 0a0a 2020 2020 6d6f  ne.    )..    mo
+000173e0: 636b 5f70 7265 6473 5f61 6e64 5f66 6565  ck_preds_and_fee
+000173f0: 6462 6163 6b2e 6173 7365 7274 5f6e 6f74  dback.assert_not
+00017400: 5f63 616c 6c65 6428 290a 2020 2020 6d6f  _called().    mo
+00017410: 636b 5f70 7265 6473 2e61 7373 6572 745f  ck_preds.assert_
+00017420: 6e6f 745f 6361 6c6c 6564 2829 0a20 2020  not_called().   
+00017430: 206d 6f63 6b5f 6665 6564 6261 636b 2e61   mock_feedback.a
+00017440: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
+00017450: 2829 0a0a 0a40 7079 7465 7374 2e6d 6172  ()...@pytest.mar
+00017460: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
+00017470: 2020 2028 2274 6573 745f 6665 6564 6261     ("test_feedba
+00017480: 636b 7322 2c20 2274 6573 745f 6f75 7470  cks", "test_outp
+00017490: 7574 7322 2c20 2274 6573 745f 696e 7075  uts", "test_inpu
+000174a0: 7473 2229 2c0a 2020 2020 5b0a 2020 2020  ts"),.    [.    
+000174b0: 2020 2020 284e 6f6e 652c 204e 6f6e 652c      (None, None,
+000174c0: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
+000174d0: 2870 642e 4461 7461 4672 616d 6528 292c  (pd.DataFrame(),
+000174e0: 2070 642e 4461 7461 4672 616d 6528 292c   pd.DataFrame(),
+000174f0: 2070 642e 4461 7461 4672 616d 6528 2929   pd.DataFrame())
+00017500: 2c0a 2020 2020 2020 2020 285b 5d2c 205b  ,.        ([], [
+00017510: 5d2c 205b 5d29 2c0a 2020 2020 2020 2020  ], []),.        
+00017520: 2870 642e 5365 7269 6573 2829 2c20 7064  (pd.Series(), pd
+00017530: 2e53 6572 6965 7328 292c 2070 642e 5365  .Series(), pd.Se
+00017540: 7269 6573 2829 292c 0a20 2020 2020 2020  ries()),.       
+00017550: 2028 6e70 2e61 7272 6179 285b 5d29 2c20   (np.array([]), 
+00017560: 6e70 2e61 7272 6179 285b 5d29 2c20 6e70  np.array([]), np
+00017570: 2e61 7272 6179 285b 5d29 292c 0a20 2020  .array([])),.   
+00017580: 205d 2c0a 290a 4070 7974 6573 742e 6d61   ],.).@pytest.ma
+00017590: 726b 2e70 6172 616d 6574 7269 7a65 2822  rk.parametrize("
+000175a0: 7665 7273 696f 6e22 2c20 5b4e 6f6e 652c  version", [None,
+000175b0: 2031 302c 2022 312e 322e 3322 5d29 0a40   10, "1.2.3"]).@
+000175c0: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
+000175d0: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
+000175e0: 2e47 616e 7472 792e 5f67 656e 6572 6174  .Gantry._generat
+000175f0: 655f 7072 6564 6963 7469 6f6e 5f61 6e64  e_prediction_and
+00017600: 5f66 6565 6462 6163 6b5f 6576 656e 7473  _feedback_events
+00017610: 2229 0a40 6d6f 636b 2e70 6174 6368 2822  ").@mock.patch("
+00017620: 6761 6e74 7279 2e6c 6f67 6765 722e 636c  gantry.logger.cl
+00017630: 6965 6e74 2e47 616e 7472 792e 5f67 656e  ient.Gantry._gen
+00017640: 6572 6174 655f 7072 6564 6963 7469 6f6e  erate_prediction
+00017650: 5f65 7665 6e74 7322 290a 406d 6f63 6b2e  _events").@mock.
+00017660: 7061 7463 6828 2267 616e 7472 792e 6c6f  patch("gantry.lo
+00017670: 6767 6572 2e63 6c69 656e 742e 4761 6e74  gger.client.Gant
+00017680: 7279 2e5f 6765 6e65 7261 7465 5f66 6565  ry._generate_fee
+00017690: 6462 6163 6b5f 6576 656e 7473 2229 0a64  dback_events").d
+000176a0: 6566 2074 6573 745f 6765 6e65 7261 7465  ef test_generate
+000176b0: 5f72 6563 6f72 6473 5f6e 6f5f 6461 7461  _records_no_data
+000176c0: 280a 2020 2020 6d6f 636b 5f67 656e 6572  (.    mock_gener
+000176d0: 6174 655f 6665 6564 6261 636b 2c0a 2020  ate_feedback,.  
+000176e0: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
+000176f0: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
+00017700: 6765 6e65 7261 7465 5f70 7265 6473 5f61  generate_preds_a
+00017710: 6e64 5f66 6565 6462 6163 6b2c 0a20 2020  nd_feedback,.   
+00017720: 2076 6572 7369 6f6e 2c0a 2020 2020 7465   version,.    te
+00017730: 7374 5f69 6e70 7574 732c 0a20 2020 2074  st_inputs,.    t
+00017740: 6573 745f 6f75 7470 7574 732c 0a20 2020  est_outputs,.   
+00017750: 2074 6573 745f 6665 6564 6261 636b 732c   test_feedbacks,
+00017760: 0a20 2020 2063 6c69 5f6f 626a 2c0a 293a  .    cli_obj,.):
+00017770: 0a20 2020 2061 7373 6572 7420 280a 2020  .    assert (.  
+00017780: 2020 2020 2020 636c 695f 6f62 6a2e 6765        cli_obj.ge
+00017790: 6e65 7261 7465 5f72 6563 6f72 6473 280a  nerate_records(.
+000177a0: 2020 2020 2020 2020 2020 2020 6170 706c              appl
+000177b0: 6963 6174 696f 6e3d 2266 6f6f 6261 7222  ication="foobar"
+000177c0: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+000177d0: 7273 696f 6e3d 7665 7273 696f 6e2c 0a20  rsion=version,. 
+000177e0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+000177f0: 733d 7465 7374 5f69 6e70 7574 732c 0a20  s=test_inputs,. 
+00017800: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00017810: 7473 3d74 6573 745f 6f75 7470 7574 732c  ts=test_outputs,
+00017820: 0a20 2020 2020 2020 2020 2020 2066 6565  .            fee
+00017830: 6462 6163 6b73 3d74 6573 745f 6665 6564  dbacks=test_feed
+00017840: 6261 636b 732c 0a20 2020 2020 2020 2020  backs,.         
+00017850: 2020 2074 696d 6573 7461 6d70 733d 4e6f     timestamps=No
+00017860: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00017870: 736f 7274 5f6f 6e5f 7469 6d65 7374 616d  sort_on_timestam
+00017880: 703d 5472 7565 2c0a 2020 2020 2020 2020  p=True,.        
+00017890: 290a 2020 2020 2020 2020 6973 204e 6f6e  ).        is Non
+000178a0: 650a 2020 2020 290a 0a20 2020 206d 6f63  e.    )..    moc
+000178b0: 6b5f 6765 6e65 7261 7465 5f70 7265 6473  k_generate_preds
+000178c0: 5f61 6e64 5f66 6565 6462 6163 6b2e 6173  _and_feedback.as
+000178d0: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
+000178e0: 290a 2020 2020 6d6f 636b 5f67 656e 6572  ).    mock_gener
+000178f0: 6174 655f 7072 6564 732e 6173 7365 7274  ate_preds.assert
+00017900: 5f6e 6f74 5f63 616c 6c65 6428 290a 2020  _not_called().  
+00017910: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
+00017920: 6665 6564 6261 636b 2e61 7373 6572 745f  feedback.assert_
+00017930: 6e6f 745f 6361 6c6c 6564 2829 0a0a 0a40  not_called()...@
+00017940: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+00017950: 6d65 7472 697a 6528 0a20 2020 2022 7465  metrize(.    "te
+00017960: 7374 5f66 6565 6462 6163 6b73 222c 0a20  st_feedbacks",. 
+00017970: 2020 205b 4e6f 6e65 2c20 7064 2e44 6174     [None, pd.Dat
+00017980: 6146 7261 6d65 2829 2c20 5b7b 2241 223a  aFrame(), [{"A":
+00017990: 2033 7d2c 207b 2241 223a 2033 7d5d 2c20   3}, {"A": 3}], 
+000179a0: 7064 2e53 6572 6965 7328 295d 2c0a 290a  pd.Series()],.).
+000179b0: 406d 6f63 6b2e 7061 7463 6828 2267 616e  @mock.patch("gan
+000179c0: 7472 792e 6c6f 6767 6572 2e63 6c69 656e  try.logger.clien
+000179d0: 742e 4761 6e74 7279 2e5f 6c6f 675f 7072  t.Gantry._log_pr
+000179e0: 6564 6963 7469 6f6e 5f61 6e64 5f66 6565  ediction_and_fee
+000179f0: 6462 6163 6b5f 6576 656e 7473 2229 0a40  dback_events").@
+00017a00: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
+00017a10: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
+00017a20: 2e47 616e 7472 792e 5f6c 6f67 5f70 7265  .Gantry._log_pre
+00017a30: 6469 6374 696f 6e5f 6576 656e 7473 2229  diction_events")
+00017a40: 0a40 6d6f 636b 2e70 6174 6368 2822 6761  .@mock.patch("ga
+00017a50: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+00017a60: 6e74 2e47 616e 7472 792e 5f6c 6f67 5f66  nt.Gantry._log_f
+00017a70: 6565 6462 6163 6b5f 6576 656e 7473 2229  eedback_events")
+00017a80: 0a64 6566 2074 6573 745f 6c6f 675f 7265  .def test_log_re
+00017a90: 636f 7264 735f 696e 636f 6d70 6c65 7465  cords_incomplete
+00017aa0: 5f70 7265 6473 280a 2020 2020 6d6f 636b  _preds(.    mock
+00017ab0: 5f66 6565 6462 6163 6b2c 0a20 2020 206d  _feedback,.    m
+00017ac0: 6f63 6b5f 7072 6564 732c 0a20 2020 206d  ock_preds,.    m
+00017ad0: 6f63 6b5f 7072 6564 735f 616e 645f 6665  ock_preds_and_fe
+00017ae0: 6564 6261 636b 2c0a 2020 2020 7465 7374  edback,.    test
+00017af0: 5f66 6565 6462 6163 6b73 2c0a 2020 2020  _feedbacks,.    
+00017b00: 636c 695f 6f62 6a2c 0a29 3a0a 2020 2020  cli_obj,.):.    
+00017b10: 7276 203d 2063 6c69 5f6f 626a 2e6c 6f67  rv = cli_obj.log
+00017b20: 5f72 6563 6f72 6473 280a 2020 2020 2020  _records(.      
+00017b30: 2020 6170 706c 6963 6174 696f 6e3d 2266    application="f
+00017b40: 6f6f 6261 7222 2c0a 2020 2020 2020 2020  oobar",.        
+00017b50: 7665 7273 696f 6e3d 2232 2e30 2e31 222c  version="2.0.1",
+00017b60: 0a20 2020 2020 2020 2069 6e70 7574 733d  .        inputs=
+00017b70: 5b5d 2c0a 2020 2020 2020 2020 6f75 7470  [],.        outp
+00017b80: 7574 733d 5b7b 2241 223a 2031 7d2c 207b  uts=[{"A": 1}, {
+00017b90: 2241 223a 2032 7d5d 2c0a 2020 2020 2020  "A": 2}],.      
+00017ba0: 2020 6665 6564 6261 636b 733d 7465 7374    feedbacks=test
+00017bb0: 5f66 6565 6462 6163 6b73 2c0a 2020 2020  _feedbacks,.    
+00017bc0: 2020 2020 7469 6d65 7374 616d 7073 3d4e      timestamps=N
+00017bd0: 6f6e 652c 0a20 2020 2020 2020 2073 6f72  one,.        sor
+00017be0: 745f 6f6e 5f74 696d 6573 7461 6d70 3d54  t_on_timestamp=T
+00017bf0: 7275 652c 0a20 2020 2029 0a20 2020 2061  rue,.    ).    a
+00017c00: 7373 6572 7420 7276 2069 7320 4e6f 6e65  ssert rv is None
+00017c10: 0a0a 2020 2020 6d6f 636b 5f70 7265 6473  ..    mock_preds
+00017c20: 5f61 6e64 5f66 6565 6462 6163 6b2e 6173  _and_feedback.as
+00017c30: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
+00017c40: 290a 2020 2020 6d6f 636b 5f70 7265 6473  ).    mock_preds
+00017c50: 2e61 7373 6572 745f 6e6f 745f 6361 6c6c  .assert_not_call
+00017c60: 6564 2829 0a20 2020 206d 6f63 6b5f 6665  ed().    mock_fe
+00017c70: 6564 6261 636b 2e61 7373 6572 745f 6e6f  edback.assert_no
+00017c80: 745f 6361 6c6c 6564 2829 0a0a 0a40 7079  t_called()...@py
+00017c90: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+00017ca0: 7472 697a 6528 0a20 2020 2022 7465 7374  trize(.    "test
+00017cb0: 5f66 6565 6462 6163 6b73 222c 0a20 2020  _feedbacks",.   
+00017cc0: 205b 4e6f 6e65 2c20 7064 2e44 6174 6146   [None, pd.DataF
+00017cd0: 7261 6d65 2829 2c20 5b7b 2241 223a 2033  rame(), [{"A": 3
+00017ce0: 7d2c 207b 2241 223a 2033 7d5d 2c20 7064  }, {"A": 3}], pd
+00017cf0: 2e53 6572 6965 7328 295d 2c0a 290a 406d  .Series()],.).@m
+00017d00: 6f63 6b2e 7061 7463 6828 2267 616e 7472  ock.patch("gantr
+00017d10: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+00017d20: 4761 6e74 7279 2e5f 6765 6e65 7261 7465  Gantry._generate
+00017d30: 5f70 7265 6469 6374 696f 6e5f 616e 645f  _prediction_and_
+00017d40: 6665 6564 6261 636b 5f65 7665 6e74 7322  feedback_events"
+00017d50: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+00017d60: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+00017d70: 656e 742e 4761 6e74 7279 2e5f 6765 6e65  ent.Gantry._gene
+00017d80: 7261 7465 5f70 7265 6469 6374 696f 6e5f  rate_prediction_
+00017d90: 6576 656e 7473 2229 0a40 6d6f 636b 2e70  events").@mock.p
+00017da0: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
+00017db0: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
+00017dc0: 792e 5f67 656e 6572 6174 655f 6665 6564  y._generate_feed
+00017dd0: 6261 636b 5f65 7665 6e74 7322 290a 6465  back_events").de
+00017de0: 6620 7465 7374 5f67 656e 6572 6174 655f  f test_generate_
+00017df0: 7265 636f 7264 735f 696e 636f 6d70 6c65  records_incomple
+00017e00: 7465 5f70 7265 6473 280a 2020 2020 6d6f  te_preds(.    mo
+00017e10: 636b 5f67 656e 6572 6174 655f 6665 6564  ck_generate_feed
+00017e20: 6261 636b 2c0a 2020 2020 6d6f 636b 5f67  back,.    mock_g
+00017e30: 656e 6572 6174 655f 7072 6564 732c 0a20  enerate_preds,. 
+00017e40: 2020 206d 6f63 6b5f 6765 6e65 7261 7465     mock_generate
+00017e50: 5f70 7265 6473 5f61 6e64 5f66 6565 6462  _preds_and_feedb
+00017e60: 6163 6b2c 0a20 2020 2074 6573 745f 6665  ack,.    test_fe
+00017e70: 6564 6261 636b 732c 0a20 2020 2063 6c69  edbacks,.    cli
+00017e80: 5f6f 626a 2c0a 293a 0a20 2020 2072 7620  _obj,.):.    rv 
+00017e90: 3d20 636c 695f 6f62 6a2e 6765 6e65 7261  = cli_obj.genera
+00017ea0: 7465 5f72 6563 6f72 6473 280a 2020 2020  te_records(.    
+00017eb0: 2020 2020 6170 706c 6963 6174 696f 6e3d      application=
+00017ec0: 2266 6f6f 6261 7222 2c0a 2020 2020 2020  "foobar",.      
+00017ed0: 2020 7665 7273 696f 6e3d 2232 2e30 2e31    version="2.0.1
+00017ee0: 222c 0a20 2020 2020 2020 2069 6e70 7574  ",.        input
+00017ef0: 733d 5b5d 2c0a 2020 2020 2020 2020 6f75  s=[],.        ou
+00017f00: 7470 7574 733d 5b7b 2241 223a 2031 7d2c  tputs=[{"A": 1},
+00017f10: 207b 2241 223a 2032 7d5d 2c0a 2020 2020   {"A": 2}],.    
+00017f20: 2020 2020 6665 6564 6261 636b 733d 7465      feedbacks=te
+00017f30: 7374 5f66 6565 6462 6163 6b73 2c0a 2020  st_feedbacks,.  
+00017f40: 2020 2020 2020 7469 6d65 7374 616d 7073        timestamps
+00017f50: 3d4e 6f6e 652c 0a20 2020 2020 2020 2073  =None,.        s
+00017f60: 6f72 745f 6f6e 5f74 696d 6573 7461 6d70  ort_on_timestamp
+00017f70: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00017f80: 2061 7373 6572 7420 7276 2069 7320 4e6f   assert rv is No
+00017f90: 6e65 0a0a 2020 2020 6d6f 636b 5f67 656e  ne..    mock_gen
+00017fa0: 6572 6174 655f 7072 6564 735f 616e 645f  erate_preds_and_
+00017fb0: 6665 6564 6261 636b 2e61 7373 6572 745f  feedback.assert_
+00017fc0: 6e6f 745f 6361 6c6c 6564 2829 0a20 2020  not_called().   
+00017fd0: 206d 6f63 6b5f 6765 6e65 7261 7465 5f70   mock_generate_p
+00017fe0: 7265 6473 2e61 7373 6572 745f 6e6f 745f  reds.assert_not_
+00017ff0: 6361 6c6c 6564 2829 0a20 2020 206d 6f63  called().    moc
+00018000: 6b5f 6765 6e65 7261 7465 5f66 6565 6462  k_generate_feedb
+00018010: 6163 6b2e 6173 7365 7274 5f6e 6f74 5f63  ack.assert_not_c
+00018020: 616c 6c65 6428 290a 0a0a 4070 7974 6573  alled()...@pytes
+00018030: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+00018040: 7a65 280a 2020 2020 2274 6573 745f 696e  ze(.    "test_in
+00018050: 7075 7473 222c 0a20 2020 205b 5b7b 2241  puts",.    [[{"A
+00018060: 223a 2031 3030 7d2c 207b 2241 223a 2031  ": 100}, {"A": 1
+00018070: 3031 7d5d 5d2c 0a29 0a40 6d6f 636b 2e70  01}]],.).@mock.p
+00018080: 6174 6368 2822 6761 6e74 7279 2e6c 6f67  atch("gantry.log
+00018090: 6765 722e 7574 696c 732e 6765 745f 6669  ger.utils.get_fi
+000180a0: 6c65 5f6c 696e 6563 6f75 6e74 2229 0a64  le_linecount").d
+000180b0: 6566 2074 6573 745f 6c6f 675f 6669 6c65  ef test_log_file
+000180c0: 286d 6f63 6b5f 6c69 6e65 5f63 6f75 6e74  (mock_line_count
+000180d0: 2c20 7465 7374 5f69 6e70 7574 7329 3a0a  , test_inputs):.
+000180e0: 2020 2020 6c6f 675f 7374 6f72 6520 3d20      log_store = 
+000180f0: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2829  mock.MagicMock()
+00018100: 0a20 2020 2067 616e 7472 7920 3d20 636c  .    gantry = cl
+00018110: 6965 6e74 2e47 616e 7472 7928 6c6f 675f  ient.Gantry(log_
+00018120: 7374 6f72 653d 6c6f 675f 7374 6f72 652c  store=log_store,
+00018130: 2065 6e76 6972 6f6e 6d65 6e74 3d22 7465   environment="te
+00018140: 7374 2229 0a20 2020 206d 6f63 6b5f 6c69  st").    mock_li
+00018150: 6e65 5f63 6f75 6e74 2e72 6574 7572 6e5f  ne_count.return_
+00018160: 7661 6c75 6520 3d20 350a 0a20 2020 2067  value = 5..    g
+00018170: 616e 7472 792e 6c6f 675f 6669 6c65 280a  antry.log_file(.
+00018180: 2020 2020 2020 2020 2266 6f6f 6261 7222          "foobar"
+00018190: 2c0a 2020 2020 2020 2020 2264 6972 2f63  ,.        "dir/c
+000181a0: 7376 5f77 6974 685f 6865 6164 6572 732e  sv_with_headers.
+000181b0: 6373 7622 2c0a 2020 2020 2020 2020 7665  csv",.        ve
+000181c0: 7273 696f 6e3d 2232 2e30 2e31 222c 0a20  rsion="2.0.1",. 
+000181d0: 2020 2029 0a0a 2020 2020 6c6f 675f 7374     )..    log_st
+000181e0: 6f72 652e 6c6f 675f 6261 7463 682e 6173  ore.log_batch.as
+000181f0: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
+00018200: 290a 0a0a 406d 6f63 6b2e 7061 7463 6828  )...@mock.patch(
+00018210: 2267 616e 7472 792e 6c6f 6767 6572 2e63  "gantry.logger.c
+00018220: 6c69 656e 742e 7575 6964 2e75 7569 6434  lient.uuid.uuid4
+00018230: 222c 2072 6574 7572 6e5f 7661 6c75 653d  ", return_value=
+00018240: 2241 4243 2229 0a40 6d6f 636b 2e70 6174  "ABC").@mock.pat
+00018250: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
+00018260: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
+00018270: 5f68 616e 646c 655f 7570 6c6f 6164 2229  _handle_upload")
+00018280: 0a64 6566 2074 6573 745f 736d 6172 745f  .def test_smart_
+00018290: 6669 6c65 7265 6164 286d 6f63 6b5f 6861  fileread(mock_ha
+000182a0: 6e64 6c65 5f75 706c 6f61 642c 206d 6f63  ndle_upload, moc
+000182b0: 6b5f 7575 6964 2c20 636c 695f 6f62 6a29  k_uuid, cli_obj)
+000182c0: 3a0a 2020 2020 6461 7461 5f6c 696e 6b20  :.    data_link 
+000182d0: 3d20 6d6f 636b 2e4d 6f63 6b28 290a 2020  = mock.Mock().  
+000182e0: 2020 636c 695f 6f62 6a2e 5f73 6d61 7274    cli_obj._smart
+000182f0: 5f66 696c 655f 7265 6164 280a 2020 2020  _file_read(.    
+00018300: 2020 2020 6461 7461 5f6c 696e 6b3d 6461      data_link=da
+00018310: 7461 5f6c 696e 6b2c 0a20 2020 2020 2020  ta_link,.       
+00018320: 206f 626a 6563 745f 7369 7a65 3d31 302c   object_size=10,
+00018330: 0a20 2020 2020 2020 2070 6174 685f 6e61  .        path_na
+00018340: 6d65 3d22 666f 6f62 6172 222c 0a20 2020  me="foobar",.   
+00018350: 2020 2020 2066 696c 653d 696f 2e53 7472       file=io.Str
+00018360: 696e 6749 4f28 22f0 9f98 8ef0 9f98 8e22  ingIO("........"
+00018370: 292c 0a20 2020 2020 2020 2063 6875 6e6b  ),.        chunk
+00018380: 5f73 697a 653d 3230 302c 0a20 2020 2029  _size=200,.    )
+00018390: 0a0a 2020 2020 6172 6773 2c20 6b77 6172  ..    args, kwar
+000183a0: 6773 203d 206d 6f63 6b5f 6861 6e64 6c65  gs = mock_handle
+000183b0: 5f75 706c 6f61 642e 6361 6c6c 5f61 7267  _upload.call_arg
+000183c0: 730a 0a20 2020 2061 7373 6572 7420 6c69  s..    assert li
+000183d0: 7374 2861 7267 735b 305d 2920 3d3d 205b  st(args[0]) == [
+000183e0: 6222 5c78 6630 5c78 3966 5c78 3938 5c78  b"\xf0\x9f\x98\x
+000183f0: 3865 5c78 6630 5c78 3966 5c78 3938 5c78  8e\xf0\x9f\x98\x
+00018400: 3865 225d 2020 2320 7465 7374 2055 5446  8e"]  # test UTF
+00018410: 2d38 2073 7570 706f 7274 0a20 2020 2061  -8 support.    a
+00018420: 7373 6572 7420 6172 6773 5b31 5d20 3d3d  ssert args[1] ==
+00018430: 2064 6174 615f 6c69 6e6b 0a20 2020 2061   data_link.    a
+00018440: 7373 6572 7420 6172 6773 5b32 5d20 3d3d  ssert args[2] ==
+00018450: 2031 300a 2020 2020 6173 7365 7274 2061   10.    assert a
+00018460: 7267 735b 335d 203d 3d20 2241 4243 5f66  rgs[3] == "ABC_f
+00018470: 6f6f 6261 7222 0a0a 0a40 7079 7465 7374  oobar"...@pytest
+00018480: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00018490: 6528 0a20 2020 205b 2269 6e70 7574 7322  e(.    ["inputs"
+000184a0: 2c20 226f 7574 7075 7473 222c 2022 6665  , "outputs", "fe
+000184b0: 6564 6261 636b 7322 2c20 226a 6f69 6e5f  edbacks", "join_
+000184c0: 6b65 7973 222c 2022 7469 6d65 7374 616d  keys", "timestam
+000184d0: 7073 225d 2c0a 2020 2020 5b0a 2020 2020  ps"],.    [.    
+000184e0: 2020 2020 285b 7b22 4122 3a20 3130 7d5d      ([{"A": 10}]
+000184f0: 202a 2031 302c 205b 7b22 4122 3a20 3130   * 10, [{"A": 10
+00018500: 7d5d 202a 2039 2c20 4e6f 6e65 2c20 4e6f  }] * 9, None, No
+00018510: 6e65 2c20 4e6f 6e65 292c 0a20 2020 2020  ne, None),.     
+00018520: 2020 2028 5b7b 2241 223a 2031 307d 5d20     ([{"A": 10}] 
+00018530: 2a20 3130 2c20 5b7b 2241 223a 2031 307d  * 10, [{"A": 10}
+00018540: 5d20 2a20 392c 205b 7b22 4122 3a20 3131  ] * 9, [{"A": 11
+00018550: 7d5d 202a 2031 302c 205b 2266 6f6f 6261  }] * 10, ["fooba
+00018560: 7222 5d20 2a20 3130 2c20 4e6f 6e65 292c  r"] * 10, None),
+00018570: 0a20 2020 2020 2020 2028 5b7b 2241 223a  .        ([{"A":
+00018580: 2031 307d 5d20 2a20 392c 205b 7b22 4122   10}] * 9, [{"A"
+00018590: 3a20 3130 7d5d 202a 2038 2c20 5b7b 2241  : 10}] * 8, [{"A
+000185a0: 223a 2031 317d 5d20 2a20 3130 2c20 5b22  ": 11}] * 10, ["
+000185b0: 666f 6f62 6172 225d 202a 2031 302c 204e  foobar"] * 10, N
+000185c0: 6f6e 6529 2c0a 2020 2020 2020 2020 285b  one),.        ([
+000185d0: 7b22 4122 3a20 3130 7d5d 202a 2039 2c20  {"A": 10}] * 9, 
+000185e0: 4e6f 6e65 2c20 5b7b 2241 223a 2031 317d  None, [{"A": 11}
+000185f0: 5d20 2a20 3130 2c20 5b22 666f 6f62 6172  ] * 10, ["foobar
+00018600: 225d 202a 2031 302c 204e 6f6e 6529 2c0a  "] * 10, None),.
+00018610: 2020 2020 2020 2020 284e 6f6e 652c 204e          (None, N
+00018620: 6f6e 652c 205b 7b22 4122 3a20 3131 7d5d  one, [{"A": 11}]
+00018630: 202a 2031 312c 205b 2266 6f6f 6261 7222   * 11, ["foobar"
+00018640: 5d20 2a20 3130 2c20 4e6f 6e65 292c 0a20  ] * 10, None),. 
+00018650: 2020 2020 2020 2028 4e6f 6e65 2c20 4e6f         (None, No
+00018660: 6e65 2c20 5b7b 2241 223a 2031 317d 5d20  ne, [{"A": 11}] 
+00018670: 2a20 3131 2c20 5b22 666f 6f62 6172 225d  * 11, ["foobar"]
+00018680: 202a 2031 302c 205b 4355 5252 454e 545f   * 10, [CURRENT_
+00018690: 5449 4d45 5d20 2a20 3130 292c 0a20 2020  TIME] * 10),.   
+000186a0: 2020 2020 2028 4e6f 6e65 2c20 4e6f 6e65       (None, None
+000186b0: 2c20 5b7b 2241 223a 2031 317d 5d20 2a20  , [{"A": 11}] * 
+000186c0: 3131 2c20 5b22 666f 6f62 6172 225d 202a  11, ["foobar"] *
+000186d0: 2031 302c 206e 702e 6172 7261 7928 5b43   10, np.array([C
+000186e0: 5552 5245 4e54 5f54 494d 455d 202a 2031  URRENT_TIME] * 1
+000186f0: 3029 292c 0a20 2020 205d 2c0a 290a 406d  0)),.    ],.).@m
+00018700: 6f63 6b2e 7061 7463 6828 2267 616e 7472  ock.patch("gantr
+00018710: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+00018720: 4761 6e74 7279 2e5f 6c6f 675f 7072 6564  Gantry._log_pred
+00018730: 6963 7469 6f6e 5f61 6e64 5f66 6565 6462  iction_and_feedb
+00018740: 6163 6b5f 6576 656e 7473 2229 0a40 6d6f  ack_events").@mo
+00018750: 636b 2e70 6174 6368 2822 6761 6e74 7279  ck.patch("gantry
+00018760: 2e6c 6f67 6765 722e 636c 6965 6e74 2e47  .logger.client.G
+00018770: 616e 7472 792e 5f6c 6f67 5f70 7265 6469  antry._log_predi
+00018780: 6374 696f 6e5f 6576 656e 7473 2229 0a40  ction_events").@
+00018790: 6d6f 636b 2e70 6174 6368 2822 6761 6e74  mock.patch("gant
+000187a0: 7279 2e6c 6f67 6765 722e 636c 6965 6e74  ry.logger.client
+000187b0: 2e47 616e 7472 792e 5f6c 6f67 5f66 6565  .Gantry._log_fee
+000187c0: 6462 6163 6b5f 6576 656e 7473 2229 0a64  dback_events").d
+000187d0: 6566 2074 6573 745f 6c6f 675f 7265 636f  ef test_log_reco
+000187e0: 7264 735f 7369 7a65 5f6d 6973 6d61 7463  rds_size_mismatc
+000187f0: 6828 0a20 2020 206d 6f63 6b5f 6665 6564  h(.    mock_feed
+00018800: 6261 636b 732c 0a20 2020 206d 6f63 6b5f  backs,.    mock_
+00018810: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
+00018820: 7072 6564 735f 616e 645f 6665 6564 6261  preds_and_feedba
+00018830: 636b 2c0a 2020 2020 696e 7075 7473 2c0a  ck,.    inputs,.
+00018840: 2020 2020 6f75 7470 7574 732c 0a20 2020      outputs,.   
+00018850: 2066 6565 6462 6163 6b73 2c0a 2020 2020   feedbacks,.    
+00018860: 7469 6d65 7374 616d 7073 2c0a 2020 2020  timestamps,.    
+00018870: 6a6f 696e 5f6b 6579 732c 0a20 2020 2063  join_keys,.    c
+00018880: 6c69 5f6f 626a 2c0a 293a 0a20 2020 2061  li_obj,.):.    a
+00018890: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
+000188a0: 636c 695f 6f62 6a2e 6c6f 675f 7265 636f  cli_obj.log_reco
+000188b0: 7264 7328 0a20 2020 2020 2020 2020 2020  rds(.           
+000188c0: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
+000188d0: 6f62 6172 222c 0a20 2020 2020 2020 2020  obar",.         
+000188e0: 2020 2076 6572 7369 6f6e 3d22 322e 302e     version="2.0.
+000188f0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+00018900: 696e 7075 7473 3d69 6e70 7574 732c 0a20  inputs=inputs,. 
+00018910: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00018920: 7473 3d6f 7574 7075 7473 2c0a 2020 2020  ts=outputs,.    
+00018930: 2020 2020 2020 2020 6665 6564 6261 636b          feedback
+00018940: 733d 6665 6564 6261 636b 732c 0a20 2020  s=feedbacks,.   
+00018950: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
+00018960: 6d70 733d 7469 6d65 7374 616d 7073 2c0a  mps=timestamps,.
+00018970: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+00018980: 5f6f 6e5f 7469 6d65 7374 616d 703d 5472  _on_timestamp=Tr
+00018990: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000189a0: 6a6f 696e 5f6b 6579 733d 6a6f 696e 5f6b  join_keys=join_k
+000189b0: 6579 732c 0a20 2020 2020 2020 2029 0a20  eys,.        ). 
+000189c0: 2020 2020 2020 2069 7320 4e6f 6e65 0a20         is None. 
+000189d0: 2020 2029 0a0a 2020 2020 6d6f 636b 5f70     )..    mock_p
+000189e0: 7265 6473 5f61 6e64 5f66 6565 6462 6163  reds_and_feedbac
+000189f0: 6b2e 6173 7365 7274 5f6e 6f74 5f63 616c  k.assert_not_cal
+00018a00: 6c65 6428 290a 2020 2020 6d6f 636b 5f70  led().    mock_p
+00018a10: 7265 6473 2e61 7373 6572 745f 6e6f 745f  reds.assert_not_
+00018a20: 6361 6c6c 6564 2829 0a20 2020 206d 6f63  called().    moc
+00018a30: 6b5f 6665 6564 6261 636b 732e 6173 7365  k_feedbacks.asse
+00018a40: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
+00018a50: 0a0a 4070 7974 6573 742e 6d61 726b 2e70  ..@pytest.mark.p
+00018a60: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
+00018a70: 5b22 696e 7075 7473 222c 2022 6f75 7470  ["inputs", "outp
+00018a80: 7574 7322 2c20 2266 6565 6462 6163 6b73  uts", "feedbacks
+00018a90: 222c 2022 6a6f 696e 5f6b 6579 7322 2c20  ", "join_keys", 
+00018aa0: 2274 696d 6573 7461 6d70 7322 5d2c 0a20  "timestamps"],. 
+00018ab0: 2020 205b 0a20 2020 2020 2020 2028 5b7b     [.        ([{
+00018ac0: 2241 223a 2031 307d 5d20 2a20 3130 2c20  "A": 10}] * 10, 
+00018ad0: 5b7b 2241 223a 2031 307d 5d20 2a20 392c  [{"A": 10}] * 9,
+00018ae0: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
+00018af0: 6529 2c0a 2020 2020 2020 2020 285b 7b22  e),.        ([{"
+00018b00: 4122 3a20 3130 7d5d 202a 2031 302c 205b  A": 10}] * 10, [
+00018b10: 7b22 4122 3a20 3130 7d5d 202a 2039 2c20  {"A": 10}] * 9, 
+00018b20: 5b7b 2241 223a 2031 317d 5d20 2a20 3130  [{"A": 11}] * 10
+00018b30: 2c20 5b22 666f 6f62 6172 225d 202a 2031  , ["foobar"] * 1
+00018b40: 302c 204e 6f6e 6529 2c0a 2020 2020 2020  0, None),.      
+00018b50: 2020 285b 7b22 4122 3a20 3130 7d5d 202a    ([{"A": 10}] *
+00018b60: 2039 2c20 5b7b 2241 223a 2031 307d 5d20   9, [{"A": 10}] 
+00018b70: 2a20 382c 205b 7b22 4122 3a20 3131 7d5d  * 8, [{"A": 11}]
+00018b80: 202a 2031 302c 205b 2266 6f6f 6261 7222   * 10, ["foobar"
+00018b90: 5d20 2a20 3130 2c20 4e6f 6e65 292c 0a20  ] * 10, None),. 
+00018ba0: 2020 2020 2020 2028 5b7b 2241 223a 2031         ([{"A": 1
+00018bb0: 307d 5d20 2a20 392c 204e 6f6e 652c 205b  0}] * 9, None, [
+00018bc0: 7b22 4122 3a20 3131 7d5d 202a 2031 302c  {"A": 11}] * 10,
+00018bd0: 205b 2266 6f6f 6261 7222 5d20 2a20 3130   ["foobar"] * 10
+00018be0: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
+00018bf0: 2028 4e6f 6e65 2c20 4e6f 6e65 2c20 5b7b   (None, None, [{
+00018c00: 2241 223a 2031 317d 5d20 2a20 3131 2c20  "A": 11}] * 11, 
+00018c10: 5b22 666f 6f62 6172 225d 202a 2031 302c  ["foobar"] * 10,
+00018c20: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
+00018c30: 284e 6f6e 652c 204e 6f6e 652c 205b 7b22  (None, None, [{"
+00018c40: 4122 3a20 3131 7d5d 202a 2031 312c 205b  A": 11}] * 11, [
+00018c50: 2266 6f6f 6261 7222 5d20 2a20 3130 2c20  "foobar"] * 10, 
+00018c60: 5b43 5552 5245 4e54 5f54 494d 455d 202a  [CURRENT_TIME] *
+00018c70: 2031 3029 2c0a 2020 2020 2020 2020 284e   10),.        (N
+00018c80: 6f6e 652c 204e 6f6e 652c 205b 7b22 4122  one, None, [{"A"
+00018c90: 3a20 3131 7d5d 202a 2031 312c 205b 2266  : 11}] * 11, ["f
+00018ca0: 6f6f 6261 7222 5d20 2a20 3130 2c20 6e70  oobar"] * 10, np
+00018cb0: 2e61 7272 6179 285b 4355 5252 454e 545f  .array([CURRENT_
+00018cc0: 5449 4d45 5d20 2a20 3130 2929 2c0a 2020  TIME] * 10)),.  
+00018cd0: 2020 5d2c 0a29 0a40 6d6f 636b 2e70 6174    ],.).@mock.pat
+00018ce0: 6368 2822 6761 6e74 7279 2e6c 6f67 6765  ch("gantry.logge
+00018cf0: 722e 636c 6965 6e74 2e47 616e 7472 792e  r.client.Gantry.
+00018d00: 5f67 656e 6572 6174 655f 7072 6564 6963  _generate_predic
+00018d10: 7469 6f6e 5f61 6e64 5f66 6565 6462 6163  tion_and_feedbac
+00018d20: 6b5f 6576 656e 7473 2229 0a40 6d6f 636b  k_events").@mock
+00018d30: 2e70 6174 6368 2822 6761 6e74 7279 2e6c  .patch("gantry.l
+00018d40: 6f67 6765 722e 636c 6965 6e74 2e47 616e  ogger.client.Gan
+00018d50: 7472 792e 5f67 656e 6572 6174 655f 7072  try._generate_pr
+00018d60: 6564 6963 7469 6f6e 5f65 7665 6e74 7322  ediction_events"
+00018d70: 290a 406d 6f63 6b2e 7061 7463 6828 2267  ).@mock.patch("g
+00018d80: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+00018d90: 656e 742e 4761 6e74 7279 2e5f 6765 6e65  ent.Gantry._gene
+00018da0: 7261 7465 5f66 6565 6462 6163 6b5f 6576  rate_feedback_ev
+00018db0: 656e 7473 2229 0a64 6566 2074 6573 745f  ents").def test_
+00018dc0: 6765 6e65 7261 7465 5f72 6563 6f72 6473  generate_records
+00018dd0: 5f73 697a 655f 6d69 736d 6174 6368 280a  _size_mismatch(.
+00018de0: 2020 2020 6d6f 636b 5f67 656e 6572 6174      mock_generat
+00018df0: 655f 6665 6564 6261 636b 732c 0a20 2020  e_feedbacks,.   
+00018e00: 206d 6f63 6b5f 6765 6e65 7261 7465 5f70   mock_generate_p
+00018e10: 7265 6473 2c0a 2020 2020 6d6f 636b 5f67  reds,.    mock_g
+00018e20: 656e 6572 6174 655f 7072 6564 735f 616e  enerate_preds_an
+00018e30: 645f 6665 6564 6261 636b 2c0a 2020 2020  d_feedback,.    
+00018e40: 696e 7075 7473 2c0a 2020 2020 6f75 7470  inputs,.    outp
+00018e50: 7574 732c 0a20 2020 2066 6565 6462 6163  uts,.    feedbac
+00018e60: 6b73 2c0a 2020 2020 7469 6d65 7374 616d  ks,.    timestam
+00018e70: 7073 2c0a 2020 2020 6a6f 696e 5f6b 6579  ps,.    join_key
+00018e80: 732c 0a20 2020 2063 6c69 5f6f 626a 2c0a  s,.    cli_obj,.
+00018e90: 293a 0a20 2020 2061 7373 6572 7420 280a  ):.    assert (.
+00018ea0: 2020 2020 2020 2020 636c 695f 6f62 6a2e          cli_obj.
+00018eb0: 6765 6e65 7261 7465 5f72 6563 6f72 6473  generate_records
+00018ec0: 280a 2020 2020 2020 2020 2020 2020 6170  (.            ap
+00018ed0: 706c 6963 6174 696f 6e3d 2266 6f6f 6261  plication="fooba
+00018ee0: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00018ef0: 7665 7273 696f 6e3d 2232 2e30 2e31 222c  version="2.0.1",
+00018f00: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
+00018f10: 7574 733d 696e 7075 7473 2c0a 2020 2020  uts=inputs,.    
+00018f20: 2020 2020 2020 2020 6f75 7470 7574 733d          outputs=
+00018f30: 6f75 7470 7574 732c 0a20 2020 2020 2020  outputs,.       
+00018f40: 2020 2020 2066 6565 6462 6163 6b73 3d66       feedbacks=f
+00018f50: 6565 6462 6163 6b73 2c0a 2020 2020 2020  eedbacks,.      
+00018f60: 2020 2020 2020 7469 6d65 7374 616d 7073        timestamps
+00018f70: 3d74 696d 6573 7461 6d70 732c 0a20 2020  =timestamps,.   
+00018f80: 2020 2020 2020 2020 2073 6f72 745f 6f6e           sort_on
+00018f90: 5f74 696d 6573 7461 6d70 3d54 7275 652c  _timestamp=True,
+00018fa0: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
+00018fb0: 6e5f 6b65 7973 3d6a 6f69 6e5f 6b65 7973  n_keys=join_keys
+00018fc0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00018fd0: 2020 2020 6973 204e 6f6e 650a 2020 2020      is None.    
+00018fe0: 290a 0a20 2020 206d 6f63 6b5f 6765 6e65  )..    mock_gene
+00018ff0: 7261 7465 5f70 7265 6473 5f61 6e64 5f66  rate_preds_and_f
+00019000: 6565 6462 6163 6b2e 6173 7365 7274 5f6e  eedback.assert_n
+00019010: 6f74 5f63 616c 6c65 6428 290a 2020 2020  ot_called().    
+00019020: 6d6f 636b 5f67 656e 6572 6174 655f 7072  mock_generate_pr
+00019030: 6564 732e 6173 7365 7274 5f6e 6f74 5f63  eds.assert_not_c
+00019040: 616c 6c65 6428 290a 2020 2020 6d6f 636b  alled().    mock
+00019050: 5f67 656e 6572 6174 655f 6665 6564 6261  _generate_feedba
+00019060: 636b 732e 6173 7365 7274 5f6e 6f74 5f63  cks.assert_not_c
+00019070: 616c 6c65 6428 290a 0a0a 4070 7974 6573  alled()...@pytes
+00019080: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+00019090: 7a65 280a 2020 2020 5b22 696e 7075 7473  ze(.    ["inputs
+000190a0: 222c 2022 6f75 7470 7574 7322 2c20 2266  ", "outputs", "f
+000190b0: 6565 6462 6163 6b73 222c 2022 6a6f 696e  eedbacks", "join
+000190c0: 5f6b 6579 7322 2c20 2274 696d 6573 7461  _keys", "timesta
+000190d0: 6d70 7322 5d2c 0a20 2020 205b 0a20 2020  mps"],.    [.   
+000190e0: 2020 2020 2028 5b7b 2241 223a 2031 307d       ([{"A": 10}
+000190f0: 5d20 2a20 3130 2c20 5b7b 2241 223a 2031  ] * 10, [{"A": 1
+00019100: 307d 5d20 2a20 3130 2c20 4e6f 6e65 2c20  0}] * 10, None, 
+00019110: 4e6f 6e65 2c20 4e6f 6e65 292c 0a20 2020  None, None),.   
+00019120: 2020 2020 2028 5b7b 2241 223a 2031 307d       ([{"A": 10}
+00019130: 5d20 2a20 3130 2c20 5b7b 2241 223a 2031  ] * 10, [{"A": 1
+00019140: 307d 5d20 2a20 3130 2c20 5b7b 2241 223a  0}] * 10, [{"A":
+00019150: 2031 317d 5d20 2a20 3130 2c20 5b22 666f   11}] * 10, ["fo
+00019160: 6f62 6172 225d 202a 2031 302c 204e 6f6e  obar"] * 10, Non
+00019170: 6529 2c0a 2020 2020 2020 2020 285b 7b22  e),.        ([{"
+00019180: 4122 3a20 3130 7d5d 202a 2031 302c 205b  A": 10}] * 10, [
+00019190: 7b22 4122 3a20 3130 7d5d 202a 2031 302c  {"A": 10}] * 10,
+000191a0: 205b 7b22 4122 3a20 3131 7d5d 202a 2031   [{"A": 11}] * 1
+000191b0: 302c 205b 2266 6f6f 6261 7222 5d20 2a20  0, ["foobar"] * 
+000191c0: 3130 2c20 4e6f 6e65 292c 0a20 2020 2020  10, None),.     
+000191d0: 2020 2028 4e6f 6e65 2c20 4e6f 6e65 2c20     (None, None, 
+000191e0: 5b7b 2241 223a 2031 317d 5d20 2a20 3130  [{"A": 11}] * 10
+000191f0: 2c20 5b22 666f 6f62 6172 225d 202a 2031  , ["foobar"] * 1
+00019200: 302c 204e 6f6e 6529 2c0a 2020 2020 2020  0, None),.      
+00019210: 2020 284e 6f6e 652c 204e 6f6e 652c 205b    (None, None, [
+00019220: 7b22 4122 3a20 3131 7d5d 202a 2031 302c  {"A": 11}] * 10,
+00019230: 205b 2266 6f6f 6261 7222 5d20 2a20 3130   ["foobar"] * 10
+00019240: 2c20 5b43 5552 5245 4e54 5f54 494d 455d  , [CURRENT_TIME]
+00019250: 202a 2031 3029 2c0a 2020 2020 2020 2020   * 10),.        
+00019260: 284e 6f6e 652c 204e 6f6e 652c 205b 7b22  (None, None, [{"
+00019270: 4122 3a20 3131 7d5d 202a 2031 302c 205b  A": 11}] * 10, [
+00019280: 2266 6f6f 6261 7222 5d20 2a20 3130 2c20  "foobar"] * 10, 
+00019290: 6e70 2e61 7272 6179 285b 4355 5252 454e  np.array([CURREN
+000192a0: 545f 5449 4d45 5d20 2a20 3130 2929 2c0a  T_TIME] * 10)),.
+000192b0: 2020 2020 5d2c 0a29 0a40 6d6f 636b 2e70      ],.).@mock.p
+000192c0: 6174 6368 280a 2020 2020 2267 616e 7472  atch(.    "gantr
+000192d0: 792e 6c6f 6767 6572 2e63 6c69 656e 742e  y.logger.client.
+000192e0: 4761 6e74 7279 2e5f 6c6f 675f 7072 6564  Gantry._log_pred
+000192f0: 6963 7469 6f6e 5f61 6e64 5f66 6565 6462  iction_and_feedb
+00019300: 6163 6b5f 6576 656e 7473 222c 0a20 2020  ack_events",.   
+00019310: 2072 6574 7572 6e5f 7661 6c75 653d 284e   return_value=(N
+00019320: 6f6e 652c 205b 2231 3233 3435 222c 2022  one, ["12345", "
+00019330: 3637 3839 3022 5d29 2c0a 290a 406d 6f63  67890"]),.).@moc
+00019340: 6b2e 7061 7463 6828 0a20 2020 2022 6761  k.patch(.    "ga
+00019350: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+00019360: 6e74 2e47 616e 7472 792e 5f6c 6f67 5f70  nt.Gantry._log_p
+00019370: 7265 6469 6374 696f 6e5f 6576 656e 7473  rediction_events
+00019380: 222c 2072 6574 7572 6e5f 7661 6c75 653d  ", return_value=
+00019390: 284e 6f6e 652c 205b 2231 3233 3435 222c  (None, ["12345",
+000193a0: 2022 3637 3839 3022 5d29 0a29 0a40 6d6f   "67890"]).).@mo
+000193b0: 636b 2e70 6174 6368 280a 2020 2020 2267  ck.patch(.    "g
+000193c0: 616e 7472 792e 6c6f 6767 6572 2e63 6c69  antry.logger.cli
+000193d0: 656e 742e 4761 6e74 7279 2e5f 6c6f 675f  ent.Gantry._log_
+000193e0: 6665 6564 6261 636b 5f65 7665 6e74 7322  feedback_events"
+000193f0: 2c20 7265 7475 726e 5f76 616c 7565 3d28  , return_value=(
+00019400: 4e6f 6e65 2c20 5b22 3132 3334 3522 2c20  None, ["12345", 
+00019410: 2236 3738 3930 225d 290a 290a 6465 6620  "67890"]).).def 
+00019420: 7465 7374 5f6c 6f67 5f72 6563 6f72 6473  test_log_records
+00019430: 5f73 697a 655f 6d61 7463 6828 0a20 2020  _size_match(.   
+00019440: 206d 6f63 6b5f 6665 6564 6261 636b 732c   mock_feedbacks,
+00019450: 0a20 2020 206d 6f63 6b5f 7072 6564 732c  .    mock_preds,
+00019460: 0a20 2020 206d 6f63 6b5f 7072 6564 735f  .    mock_preds_
+00019470: 616e 645f 6665 6564 6261 636b 2c0a 2020  and_feedback,.  
+00019480: 2020 696e 7075 7473 2c0a 2020 2020 6f75    inputs,.    ou
+00019490: 7470 7574 732c 0a20 2020 2066 6565 6462  tputs,.    feedb
+000194a0: 6163 6b73 2c0a 2020 2020 7469 6d65 7374  acks,.    timest
+000194b0: 616d 7073 2c0a 2020 2020 6a6f 696e 5f6b  amps,.    join_k
+000194c0: 6579 732c 0a20 2020 2063 6c69 5f6f 626a  eys,.    cli_obj
+000194d0: 2c0a 293a 0a20 2020 2061 7373 6572 7420  ,.):.    assert 
+000194e0: 280a 2020 2020 2020 2020 636c 695f 6f62  (.        cli_ob
+000194f0: 6a2e 6c6f 675f 7265 636f 7264 7328 0a20  j.log_records(. 
+00019500: 2020 2020 2020 2020 2020 2061 7070 6c69             appli
+00019510: 6361 7469 6f6e 3d22 666f 6f62 6172 222c  cation="foobar",
+00019520: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
+00019530: 7369 6f6e 3d22 322e 302e 3122 2c0a 2020  sion="2.0.1",.  
+00019540: 2020 2020 2020 2020 2020 696e 7075 7473            inputs
+00019550: 3d69 6e70 7574 732c 0a20 2020 2020 2020  =inputs,.       
+00019560: 2020 2020 206f 7574 7075 7473 3d6f 7574       outputs=out
+00019570: 7075 7473 2c0a 2020 2020 2020 2020 2020  puts,.          
+00019580: 2020 6665 6564 6261 636b 733d 6665 6564    feedbacks=feed
+00019590: 6261 636b 732c 0a20 2020 2020 2020 2020  backs,.         
+000195a0: 2020 2074 696d 6573 7461 6d70 733d 7469     timestamps=ti
+000195b0: 6d65 7374 616d 7073 2c0a 2020 2020 2020  mestamps,.      
+000195c0: 2020 2020 2020 736f 7274 5f6f 6e5f 7469        sort_on_ti
+000195d0: 6d65 7374 616d 703d 5472 7565 2c0a 2020  mestamp=True,.  
+000195e0: 2020 2020 2020 2020 2020 6a6f 696e 5f6b            join_k
+000195f0: 6579 733d 6a6f 696e 5f6b 6579 732c 0a20  eys=join_keys,. 
+00019600: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00019610: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+00019620: 2029 0a0a 0a40 7079 7465 7374 2e6d 6172   )...@pytest.mar
+00019630: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
+00019640: 2020 205b 2269 6e70 7574 7322 2c20 226f     ["inputs", "o
+00019650: 7574 7075 7473 222c 2022 6665 6564 6261  utputs", "feedba
+00019660: 636b 7322 2c20 226a 6f69 6e5f 6b65 7973  cks", "join_keys
+00019670: 222c 2022 7469 6d65 7374 616d 7073 225d  ", "timestamps"]
+00019680: 2c0a 2020 2020 5b0a 2020 2020 2020 2020  ,.    [.        
+00019690: 285b 7b22 4122 3a20 3130 7d5d 202a 2031  ([{"A": 10}] * 1
+000196a0: 302c 205b 7b22 4122 3a20 3130 7d5d 202a  0, [{"A": 10}] *
+000196b0: 2031 302c 204e 6f6e 652c 204e 6f6e 652c   10, None, None,
+000196c0: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
+000196d0: 285b 7b22 4122 3a20 3130 7d5d 202a 2031  ([{"A": 10}] * 1
+000196e0: 302c 205b 7b22 4122 3a20 3130 7d5d 202a  0, [{"A": 10}] *
+000196f0: 2031 302c 205b 7b22 4122 3a20 3131 7d5d   10, [{"A": 11}]
+00019700: 202a 2031 302c 205b 2266 6f6f 6261 7222   * 10, ["foobar"
+00019710: 5d20 2a20 3130 2c20 4e6f 6e65 292c 0a20  ] * 10, None),. 
+00019720: 2020 2020 2020 2028 5b7b 2241 223a 2031         ([{"A": 1
+00019730: 307d 5d20 2a20 3130 2c20 5b7b 2241 223a  0}] * 10, [{"A":
+00019740: 2031 307d 5d20 2a20 3130 2c20 5b7b 2241   10}] * 10, [{"A
+00019750: 223a 2031 317d 5d20 2a20 3130 2c20 5b22  ": 11}] * 10, ["
+00019760: 666f 6f62 6172 225d 202a 2031 302c 204e  foobar"] * 10, N
+00019770: 6f6e 6529 2c0a 2020 2020 2020 2020 284e  one),.        (N
+00019780: 6f6e 652c 204e 6f6e 652c 205b 7b22 4122  one, None, [{"A"
+00019790: 3a20 3131 7d5d 202a 2031 302c 205b 2266  : 11}] * 10, ["f
+000197a0: 6f6f 6261 7222 5d20 2a20 3130 2c20 4e6f  oobar"] * 10, No
+000197b0: 6e65 292c 0a20 2020 2020 2020 2028 4e6f  ne),.        (No
+000197c0: 6e65 2c20 4e6f 6e65 2c20 5b7b 2241 223a  ne, None, [{"A":
+000197d0: 2031 317d 5d20 2a20 3130 2c20 5b22 666f   11}] * 10, ["fo
+000197e0: 6f62 6172 225d 202a 2031 302c 205b 4355  obar"] * 10, [CU
+000197f0: 5252 454e 545f 5449 4d45 5d20 2a20 3130  RRENT_TIME] * 10
+00019800: 292c 0a20 2020 2020 2020 2028 4e6f 6e65  ),.        (None
+00019810: 2c20 4e6f 6e65 2c20 5b7b 2241 223a 2031  , None, [{"A": 1
+00019820: 317d 5d20 2a20 3130 2c20 5b22 666f 6f62  1}] * 10, ["foob
+00019830: 6172 225d 202a 2031 302c 206e 702e 6172  ar"] * 10, np.ar
+00019840: 7261 7928 5b43 5552 5245 4e54 5f54 494d  ray([CURRENT_TIM
+00019850: 455d 202a 2031 3029 292c 0a20 2020 205d  E] * 10)),.    ]
+00019860: 2c0a 290a 406d 6f63 6b2e 7061 7463 6828  ,.).@mock.patch(
+00019870: 0a20 2020 2022 6761 6e74 7279 2e6c 6f67  .    "gantry.log
+00019880: 6765 722e 636c 6965 6e74 2e47 616e 7472  ger.client.Gantr
+00019890: 792e 5f67 656e 6572 6174 655f 7072 6564  y._generate_pred
+000198a0: 6963 7469 6f6e 5f61 6e64 5f66 6565 6462  iction_and_feedb
+000198b0: 6163 6b5f 6576 656e 7473 222c 0a20 2020  ack_events",.   
+000198c0: 2072 6574 7572 6e5f 7661 6c75 653d 284e   return_value=(N
+000198d0: 6f6e 652c 205b 2231 3233 3435 222c 2022  one, ["12345", "
+000198e0: 3637 3839 3022 5d29 2c0a 290a 406d 6f63  67890"]),.).@moc
+000198f0: 6b2e 7061 7463 6828 0a20 2020 2022 6761  k.patch(.    "ga
+00019900: 6e74 7279 2e6c 6f67 6765 722e 636c 6965  ntry.logger.clie
+00019910: 6e74 2e47 616e 7472 792e 5f67 656e 6572  nt.Gantry._gener
+00019920: 6174 655f 7072 6564 6963 7469 6f6e 5f65  ate_prediction_e
+00019930: 7665 6e74 7322 2c0a 2020 2020 7265 7475  vents",.    retu
+00019940: 726e 5f76 616c 7565 3d28 4e6f 6e65 2c20  rn_value=(None, 
+00019950: 5b22 3132 3334 3522 2c20 2236 3738 3930  ["12345", "67890
+00019960: 225d 292c 0a29 0a40 6d6f 636b 2e70 6174  "]),.).@mock.pat
+00019970: 6368 280a 2020 2020 2267 616e 7472 792e  ch(.    "gantry.
+00019980: 6c6f 6767 6572 2e63 6c69 656e 742e 4761  logger.client.Ga
+00019990: 6e74 7279 2e5f 6765 6e65 7261 7465 5f66  ntry._generate_f
+000199a0: 6565 6462 6163 6b5f 6576 656e 7473 222c  eedback_events",
+000199b0: 2072 6574 7572 6e5f 7661 6c75 653d 284e   return_value=(N
+000199c0: 6f6e 652c 205b 2231 3233 3435 222c 2022  one, ["12345", "
+000199d0: 3637 3839 3022 5d29 0a29 0a64 6566 2074  67890"]).).def t
+000199e0: 6573 745f 6765 6e65 7261 7465 5f72 6563  est_generate_rec
+000199f0: 6f72 6473 5f73 697a 655f 6d61 7463 6828  ords_size_match(
+00019a00: 0a20 2020 206d 6f63 6b5f 6765 6e65 7261  .    mock_genera
+00019a10: 7465 5f66 6565 6462 6163 6b73 2c0a 2020  te_feedbacks,.  
+00019a20: 2020 6d6f 636b 5f67 656e 6572 6174 655f    mock_generate_
+00019a30: 7072 6564 732c 0a20 2020 206d 6f63 6b5f  preds,.    mock_
+00019a40: 6765 6e65 7261 7465 5f70 7265 6473 5f61  generate_preds_a
+00019a50: 6e64 5f66 6565 6462 6163 6b2c 0a20 2020  nd_feedback,.   
+00019a60: 2069 6e70 7574 732c 0a20 2020 206f 7574   inputs,.    out
+00019a70: 7075 7473 2c0a 2020 2020 6665 6564 6261  puts,.    feedba
+00019a80: 636b 732c 0a20 2020 2074 696d 6573 7461  cks,.    timesta
+00019a90: 6d70 732c 0a20 2020 206a 6f69 6e5f 6b65  mps,.    join_ke
+00019aa0: 7973 2c0a 2020 2020 636c 695f 6f62 6a2c  ys,.    cli_obj,
+00019ab0: 0a29 3a0a 2020 2020 6173 7365 7274 2028  .):.    assert (
+00019ac0: 0a20 2020 2020 2020 2063 6c69 5f6f 626a  .        cli_obj
+00019ad0: 2e67 656e 6572 6174 655f 7265 636f 7264  .generate_record
+00019ae0: 7328 0a20 2020 2020 2020 2020 2020 2061  s(.            a
+00019af0: 7070 6c69 6361 7469 6f6e 3d22 666f 6f62  pplication="foob
+00019b00: 6172 222c 0a20 2020 2020 2020 2020 2020  ar",.           
+00019b10: 2076 6572 7369 6f6e 3d22 322e 302e 3122   version="2.0.1"
+00019b20: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+00019b30: 7075 7473 3d69 6e70 7574 732c 0a20 2020  puts=inputs,.   
+00019b40: 2020 2020 2020 2020 206f 7574 7075 7473           outputs
+00019b50: 3d6f 7574 7075 7473 2c0a 2020 2020 2020  =outputs,.      
+00019b60: 2020 2020 2020 6665 6564 6261 636b 733d        feedbacks=
+00019b70: 6665 6564 6261 636b 732c 0a20 2020 2020  feedbacks,.     
+00019b80: 2020 2020 2020 2074 696d 6573 7461 6d70         timestamp
+00019b90: 733d 7469 6d65 7374 616d 7073 2c0a 2020  s=timestamps,.  
+00019ba0: 2020 2020 2020 2020 2020 736f 7274 5f6f            sort_o
+00019bb0: 6e5f 7469 6d65 7374 616d 703d 5472 7565  n_timestamp=True
+00019bc0: 2c0a 2020 2020 2020 2020 2020 2020 6a6f  ,.            jo
+00019bd0: 696e 5f6b 6579 733d 6a6f 696e 5f6b 6579  in_keys=join_key
+00019be0: 732c 0a20 2020 2020 2020 2029 0a20 2020  s,.        ).   
+00019bf0: 2020 2020 2069 7320 6e6f 7420 4e6f 6e65       is not None
+00019c00: 0a20 2020 2029 0a0a 0a40 7079 7465 7374  .    )...@pytest
+00019c10: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00019c20: 6528 0a20 2020 2028 2274 696d 6573 7461  e(.    ("timesta
+00019c30: 6d70 222c 2022 696e 7075 7473 222c 2022  mp", "inputs", "
+00019c40: 6f75 7470 7574 7322 2c20 2266 6565 6462  outputs", "feedb
+00019c50: 6163 6b73 222c 2022 6a6f 696e 5f6b 6579  acks", "join_key
+00019c60: 222c 2022 676c 6f62 616c 5f74 6167 7322  ", "global_tags"
+00019c70: 2c20 2272 6f77 5f74 6167 7322 292c 0a20  , "row_tags"),. 
+00019c80: 2020 205b 2020 2320 5465 7374 2061 6c6c     [  # Test all
+00019c90: 2063 6f6d 6269 6e61 7469 6f6e 7320 6f66   combinations of
+00019ca0: 2069 6e70 7574 732c 206f 7574 7075 7473   inputs, outputs
+00019cb0: 2c20 6665 6564 6261 636b 732c 2061 6e64  , feedbacks, and
+00019cc0: 206a 6f69 6e5f 6b65 790a 2020 2020 2020   join_key.      
+00019cd0: 2020 2822 5422 2c20 5b22 4122 2c20 2242    ("T", ["A", "B
+00019ce0: 225d 2c20 5b22 4322 2c20 2244 225d 2c20  "], ["C", "D"], 
+00019cf0: 5b22 4822 2c20 2249 225d 2c20 2245 222c  ["H", "I"], "E",
+00019d00: 207b 2276 6572 7369 6f6e 223a 2022 7465   {"version": "te
+00019d10: 7374 5f76 6572 7369 6f6e 227d 2c20 5b22  st_version"}, ["
+00019d20: 4722 5d29 2c0a 2020 2020 2020 2020 2320  G"]),.        # 
+00019d30: 5465 7374 2077 6974 686f 7574 2066 6565  Test without fee
+00019d40: 6462 6163 6b73 2061 6e64 2072 6f77 5f74  dbacks and row_t
+00019d50: 6167 730a 2020 2020 2020 2020 2822 5422  ags.        ("T"
+00019d60: 2c20 5b22 4122 2c20 2242 225d 2c20 5b22  , ["A", "B"], ["
+00019d70: 4422 5d2c 204e 6f6e 652c 2022 4522 2c20  D"], None, "E", 
+00019d80: 7b22 7665 7273 696f 6e22 3a20 2274 6573  {"version": "tes
+00019d90: 745f 7665 7273 696f 6e22 7d2c 204e 6f6e  t_version"}, Non
+00019da0: 6529 2c0a 2020 2020 2020 2020 2320 5465  e),.        # Te
+00019db0: 7374 2077 6974 686f 7574 2069 6e70 7574  st without input
+00019dc0: 7320 616e 6420 7469 6d65 7374 616d 700a  s and timestamp.
+00019dd0: 2020 2020 2020 2020 284e 6f6e 652c 204e          (None, N
+00019de0: 6f6e 652c 204e 6f6e 652c 205b 2248 222c  one, None, ["H",
+00019df0: 2022 4922 5d2c 2022 4522 2c20 7b22 7665   "I"], "E", {"ve
+00019e00: 7273 696f 6e22 3a20 2274 6573 745f 7665  rsion": "test_ve
+00019e10: 7273 696f 6e22 7d2c 205b 2247 225d 292c  rsion"}, ["G"]),
+00019e20: 0a20 2020 2020 2020 2023 2054 6573 7420  .        # Test 
+00019e30: 6f6e 6c79 2077 6974 6820 6665 6564 6261  only with feedba
+00019e40: 636b 7320 616e 6420 6a6f 696e 5f6b 6579  cks and join_key
+00019e50: 0a20 2020 2020 2020 2028 4e6f 6e65 2c20  .        (None, 
+00019e60: 4e6f 6e65 2c20 4e6f 6e65 2c20 5b22 4822  None, None, ["H"
+00019e70: 2c20 2249 225d 2c20 2245 222c 204e 6f6e  , "I"], "E", Non
+00019e80: 652c 204e 6f6e 6529 2c0a 2020 2020 2020  e, None),.      
+00019e90: 2020 2320 5465 7374 206f 6e6c 7920 7769    # Test only wi
+00019ea0: 7468 2069 6e70 7574 7320 616e 6420 676c  th inputs and gl
+00019eb0: 6f62 616c 2074 6167 730a 2020 2020 2020  obal tags.      
+00019ec0: 2020 2822 5422 2c20 5b22 4122 2c20 2242    ("T", ["A", "B
+00019ed0: 225d 2c20 5b22 4322 2c20 2244 225d 2c20  "], ["C", "D"], 
+00019ee0: 4e6f 6e65 2c20 4e6f 6e65 2c20 7b22 7665  None, None, {"ve
+00019ef0: 7273 696f 6e22 3a20 2274 6573 745f 7665  rsion": "test_ve
+00019f00: 7273 696f 6e22 7d2c 204e 6f6e 6529 2c0a  rsion"}, None),.
+00019f10: 2020 2020 5d2c 0a29 0a64 6566 2074 6573      ],.).def tes
+00019f20: 745f 6c6f 675f 6672 6f6d 5f64 6174 615f  t_log_from_data_
+00019f30: 636f 6e6e 6563 746f 7228 0a20 2020 2074  connector(.    t
+00019f40: 696d 6573 7461 6d70 3a20 7374 722c 0a20  imestamp: str,. 
+00019f50: 2020 2069 6e70 7574 733a 204c 6973 745b     inputs: List[
+00019f60: 7374 725d 2c0a 2020 2020 6f75 7470 7574  str],.    output
+00019f70: 733a 204c 6973 745b 7374 725d 2c0a 2020  s: List[str],.  
+00019f80: 2020 6665 6564 6261 636b 733a 204c 6973    feedbacks: Lis
+00019f90: 745b 7374 725d 2c0a 2020 2020 6a6f 696e  t[str],.    join
+00019fa0: 5f6b 6579 3a20 7374 722c 0a20 2020 2072  _key: str,.    r
+00019fb0: 6f77 5f74 6167 733a 204c 6973 745b 7374  ow_tags: List[st
+00019fc0: 725d 2c0a 2020 2020 676c 6f62 616c 5f74  r],.    global_t
+00019fd0: 6167 733a 2044 6963 745b 7374 722c 2073  ags: Dict[str, s
+00019fe0: 7472 5d2c 0a20 2020 2063 6c69 5f6f 626a  tr],.    cli_obj
+00019ff0: 2c0a 293a 0a20 2020 2022 2222 0a20 2020  ,.):.    """.   
+0001a000: 2054 6573 7473 2074 6861 7420 7468 6520   Tests that the 
+0001a010: 6c6f 675f 6672 6f6d 5f64 6174 615f 636f  log_from_data_co
+0001a020: 6e6e 6563 746f 7220 6675 6e63 7469 6f6e  nnector function
+0001a030: 2063 616c 6c73 2074 6865 206c 6f67 5f66   calls the log_f
+0001a040: 726f 6d5f 6461 7461 5f63 6f6e 6e65 6374  rom_data_connect
+0001a050: 6f72 5f61 7379 6e63 0a20 2020 2066 756e  or_async.    fun
+0001a060: 6374 696f 6e20 7769 7468 2063 6f72 7265  ction with corre
+0001a070: 6374 2070 6172 616d 6574 6572 730a 2020  ct parameters.  
+0001a080: 2020 2222 220a 2020 2020 636c 695f 6f62    """.    cli_ob
+0001a090: 6a2e 6c6f 675f 7374 6f72 6520 3d20 6d6f  j.log_store = mo
+0001a0a0: 636b 2e4d 6f63 6b28 290a 2020 2020 636c  ck.Mock().    cl
+0001a0b0: 695f 6f62 6a2e 6c6f 675f 6672 6f6d 5f64  i_obj.log_from_d
+0001a0c0: 6174 615f 636f 6e6e 6563 746f 7228 0a20  ata_connector(. 
+0001a0d0: 2020 2020 2020 2061 7070 6c69 6361 7469         applicati
+0001a0e0: 6f6e 3d22 666f 6f62 6172 222c 0a20 2020  on="foobar",.   
+0001a0f0: 2020 2020 2073 6f75 7263 655f 6461 7461       source_data
+0001a100: 5f63 6f6e 6e65 6374 6f72 5f6e 616d 653d  _connector_name=
+0001a110: 2274 6573 742d 636f 6e6e 6563 746f 7222  "test-connector"
+0001a120: 2c0a 2020 2020 2020 2020 7469 6d65 7374  ,.        timest
+0001a130: 616d 703d 7469 6d65 7374 616d 702c 0a20  amp=timestamp,. 
+0001a140: 2020 2020 2020 2069 6e70 7574 733d 696e         inputs=in
+0001a150: 7075 7473 2c0a 2020 2020 2020 2020 6f75  puts,.        ou
+0001a160: 7470 7574 733d 6f75 7470 7574 732c 0a20  tputs=outputs,. 
+0001a170: 2020 2020 2020 2066 6565 6462 6163 6b73         feedbacks
+0001a180: 3d66 6565 6462 6163 6b73 2c0a 2020 2020  =feedbacks,.    
+0001a190: 2020 2020 6a6f 696e 5f6b 6579 3d6a 6f69      join_key=joi
+0001a1a0: 6e5f 6b65 792c 0a20 2020 2020 2020 2072  n_key,.        r
+0001a1b0: 6f77 5f74 6167 733d 726f 775f 7461 6773  ow_tags=row_tags
+0001a1c0: 2c0a 2020 2020 2020 2020 676c 6f62 616c  ,.        global
+0001a1d0: 5f74 6167 733d 676c 6f62 616c 5f74 6167  _tags=global_tag
+0001a1e0: 732c 0a20 2020 2029 0a0a 2020 2020 6361  s,.    )..    ca
+0001a1f0: 6c6c 5f61 7267 7320 3d20 636c 695f 6f62  ll_args = cli_ob
+0001a200: 6a2e 6c6f 675f 7374 6f72 652e 6c6f 675f  j.log_store.log_
+0001a210: 6672 6f6d 5f64 6174 615f 636f 6e6e 6563  from_data_connec
+0001a220: 746f 725f 6173 796e 632e 6361 6c6c 5f61  tor_async.call_a
+0001a230: 7267 730a 2020 2020 6173 7365 7274 2063  rgs.    assert c
+0001a240: 616c 6c5f 6172 6773 2e6b 7761 7267 7320  all_args.kwargs 
+0001a250: 3d3d 207b 0a20 2020 2020 2020 2022 7265  == {.        "re
+0001a260: 7175 6573 7422 3a20 496e 6765 7374 4672  quest": IngestFr
+0001a270: 6f6d 4461 7461 436f 6e6e 6563 746f 7252  omDataConnectorR
+0001a280: 6571 7565 7374 280a 2020 2020 2020 2020  equest(.        
+0001a290: 2020 2020 6170 706c 6963 6174 696f 6e3d      application=
+0001a2a0: 2266 6f6f 6261 7222 2c0a 2020 2020 2020  "foobar",.      
+0001a2b0: 2020 2020 2020 736f 7572 6365 5f64 6174        source_dat
+0001a2c0: 615f 636f 6e6e 6563 746f 725f 6e61 6d65  a_connector_name
+0001a2d0: 3d22 7465 7374 2d63 6f6e 6e65 6374 6f72  ="test-connector
+0001a2e0: 222c 0a20 2020 2020 2020 2020 2020 2074  ",.            t
+0001a2f0: 696d 6573 7461 6d70 3d74 696d 6573 7461  imestamp=timesta
+0001a300: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
+0001a310: 696e 7075 7473 3d69 6e70 7574 732c 0a20  inputs=inputs,. 
+0001a320: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0001a330: 7473 3d6f 7574 7075 7473 2c0a 2020 2020  ts=outputs,.    
+0001a340: 2020 2020 2020 2020 6665 6564 6261 636b          feedback
+0001a350: 733d 6665 6564 6261 636b 732c 0a20 2020  s=feedbacks,.   
+0001a360: 2020 2020 2020 2020 206a 6f69 6e5f 6b65           join_ke
+0001a370: 793d 6a6f 696e 5f6b 6579 2c0a 2020 2020  y=join_key,.    
+0001a380: 2020 2020 2020 2020 726f 775f 7461 6773          row_tags
+0001a390: 3d72 6f77 5f74 6167 732c 0a20 2020 2020  =row_tags,.     
+0001a3a0: 2020 2020 2020 2067 6c6f 6261 6c5f 7461         global_ta
+0001a3b0: 6773 3d67 6c6f 6261 6c5f 7461 6773 2c0a  gs=global_tags,.
+0001a3c0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+0001a3d0: 6475 6c65 3d4e 6f6e 652c 0a20 2020 2020  dule=None,.     
+0001a3e0: 2020 2020 2020 2070 6970 656c 696e 655f         pipeline_
+0001a3f0: 6e61 6d65 3d4e 6f6e 652c 0a20 2020 2020  name=None,.     
+0001a400: 2020 2029 0a20 2020 207d 0a0a 0a40 7079     ).    }...@py
+0001a410: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+0001a420: 7472 697a 6528 0a20 2020 2028 2273 7461  trize(.    ("sta
+0001a430: 7274 5f6f 6e22 2c20 2266 7265 7175 656e  rt_on", "frequen
+0001a440: 6379 222c 2022 7479 7065 222c 2022 6f70  cy", "type", "op
+0001a450: 7469 6f6e 7322 292c 0a20 2020 205b 0a20  tions"),.    [. 
+0001a460: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
+0001a470: 2020 2020 2022 3230 3233 2d30 322d 3031       "2023-02-01
+0001a480: 5430 303a 3030 3a30 302e 3030 3030 3030  T00:00:00.000000
+0001a490: 222c 0a20 2020 2020 2020 2020 2020 2053  ",.            S
+0001a4a0: 6368 6564 756c 6546 7265 7175 656e 6379  cheduleFrequency
+0001a4b0: 2e45 5645 5259 5f48 4f55 522c 0a20 2020  .EVERY_HOUR,.   
+0001a4c0: 2020 2020 2020 2020 2053 6368 6564 756c           Schedul
+0001a4d0: 6554 7970 652e 494e 4352 454d 454e 5441  eType.INCREMENTA
+0001a4e0: 4c5f 4150 5045 4e44 2c0a 2020 2020 2020  L_APPEND,.      
+0001a4f0: 2020 2020 2020 7b22 7761 7465 726d 6172        {"watermar
+0001a500: 6b5f 6b65 7922 3a20 2275 7064 6174 6564  k_key": "updated
+0001a510: 5f61 7422 7d2c 0a20 2020 2020 2020 2029  _at"},.        )
+0001a520: 2c0a 2020 2020 2020 2020 280a 2020 2020  ,.        (.    
+0001a530: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
+0001a540: 2e64 6174 6574 696d 652e 7574 636e 6f77  .datetime.utcnow
+0001a550: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0001a560: 5363 6865 6475 6c65 4672 6571 7565 6e63  ScheduleFrequenc
+0001a570: 792e 4556 4552 595f 325f 484f 5552 532c  y.EVERY_2_HOURS,
+0001a580: 0a20 2020 2020 2020 2020 2020 2053 6368  .            Sch
+0001a590: 6564 756c 6554 7970 652e 494e 4352 454d  eduleType.INCREM
+0001a5a0: 454e 5441 4c5f 4150 5045 4e44 2c0a 2020  ENTAL_APPEND,.  
+0001a5b0: 2020 2020 2020 2020 2020 7b22 7761 7465            {"wate
+0001a5c0: 726d 6172 6b5f 6b65 7922 3a20 4e6f 6e65  rmark_key": None
+0001a5d0: 7d2c 0a20 2020 2020 2020 2029 2c0a 2020  },.        ),.  
+0001a5e0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+0001a5f0: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
+0001a600: 6574 696d 652e 7574 636e 6f77 2829 2c0a  etime.utcnow(),.
+0001a610: 2020 2020 2020 2020 2020 2020 5363 6865              Sche
+0001a620: 6475 6c65 4672 6571 7565 6e63 792e 4556  duleFrequency.EV
+0001a630: 4552 595f 345f 484f 5552 532c 0a20 2020  ERY_4_HOURS,.   
+0001a640: 2020 2020 2020 2020 2053 6368 6564 756c           Schedul
+0001a650: 6554 7970 652e 494e 4352 454d 454e 5441  eType.INCREMENTA
+0001a660: 4c5f 4150 5045 4e44 2c0a 2020 2020 2020  L_APPEND,.      
+0001a670: 2020 2020 2020 7b22 7761 7465 726d 6172        {"watermar
+0001a680: 6b5f 6b65 7922 3a20 2275 7064 6174 6564  k_key": "updated
+0001a690: 5f61 7422 7d2c 0a20 2020 2020 2020 2029  _at"},.        )
+0001a6a0: 2c0a 2020 2020 2020 2020 280a 2020 2020  ,.        (.    
+0001a6b0: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
+0001a6c0: 2e64 6174 6574 696d 652e 7574 636e 6f77  .datetime.utcnow
+0001a6d0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0001a6e0: 5363 6865 6475 6c65 4672 6571 7565 6e63  ScheduleFrequenc
+0001a6f0: 792e 4556 4552 595f 345f 484f 5552 532c  y.EVERY_4_HOURS,
+0001a700: 0a20 2020 2020 2020 2020 2020 2053 6368  .            Sch
+0001a710: 6564 756c 6554 7970 652e 494e 4352 454d  eduleType.INCREM
+0001a720: 454e 5441 4c5f 4150 5045 4e44 2c0a 2020  ENTAL_APPEND,.  
+0001a730: 2020 2020 2020 2020 2020 7b22 6465 6c61            {"dela
+0001a740: 795f 7469 6d65 223a 2033 3030 2c20 2277  y_time": 300, "w
+0001a750: 6174 6572 6d61 726b 5f6b 6579 223a 2022  atermark_key": "
+0001a760: 7570 6461 7465 645f 6174 227d 2c0a 2020  updated_at"},.  
+0001a770: 2020 2020 2020 292c 0a20 2020 205d 2c0a        ),.    ],.
+0001a780: 290a 6465 6620 7465 7374 5f6c 6f67 5f66  ).def test_log_f
+0001a790: 726f 6d5f 6461 7461 5f63 6f6e 6e65 6374  rom_data_connect
+0001a7a0: 6f72 5f77 6974 685f 7363 6865 6475 6c65  or_with_schedule
+0001a7b0: 280a 2020 2020 7374 6172 745f 6f6e 3a20  (.    start_on: 
+0001a7c0: 556e 696f 6e5b 6461 7465 7469 6d65 2e64  Union[datetime.d
+0001a7d0: 6174 6574 696d 652c 2073 7472 5d2c 0a20  atetime, str],. 
+0001a7e0: 2020 2066 7265 7175 656e 6379 3a20 5363     frequency: Sc
+0001a7f0: 6865 6475 6c65 4672 6571 7565 6e63 792c  heduleFrequency,
+0001a800: 0a20 2020 2074 7970 653a 2053 6368 6564  .    type: Sched
+0001a810: 756c 6554 7970 652c 0a20 2020 206f 7074  uleType,.    opt
+0001a820: 696f 6e73 3a20 4469 6374 5b73 7472 2c20  ions: Dict[str, 
+0001a830: 7374 725d 2c0a 2020 2020 636c 695f 6f62  str],.    cli_ob
+0001a840: 6a2c 0a29 3a0a 2020 2020 2222 220a 2020  j,.):.    """.  
+0001a850: 2020 5465 7374 7320 7468 6174 2074 6865    Tests that the
+0001a860: 206c 6f67 5f66 726f 6d5f 6461 7461 5f63   log_from_data_c
+0001a870: 6f6e 6e65 6374 6f72 2066 756e 6374 696f  onnector functio
+0001a880: 6e20 6361 6c6c 7320 7468 6520 6c6f 675f  n calls the log_
+0001a890: 6672 6f6d 5f64 6174 615f 636f 6e6e 6563  from_data_connec
+0001a8a0: 746f 725f 6173 796e 630a 2020 2020 6675  tor_async.    fu
+0001a8b0: 6e63 7469 6f6e 2077 6974 6820 636f 7272  nction with corr
+0001a8c0: 6563 7420 7061 7261 6d65 7465 7273 0a20  ect parameters. 
+0001a8d0: 2020 2022 2222 0a20 2020 2063 6c69 5f6f     """.    cli_o
+0001a8e0: 626a 2e6c 6f67 5f73 746f 7265 203d 206d  bj.log_store = m
+0001a8f0: 6f63 6b2e 4d6f 636b 2829 0a20 2020 2063  ock.Mock().    c
+0001a900: 6c69 5f6f 626a 2e6c 6f67 5f66 726f 6d5f  li_obj.log_from_
+0001a910: 6461 7461 5f63 6f6e 6e65 6374 6f72 280a  data_connector(.
+0001a920: 2020 2020 2020 2020 6170 706c 6963 6174          applicat
+0001a930: 696f 6e3d 2266 6f6f 6261 7222 2c0a 2020  ion="foobar",.  
+0001a940: 2020 2020 2020 736f 7572 6365 5f64 6174        source_dat
+0001a950: 615f 636f 6e6e 6563 746f 725f 6e61 6d65  a_connector_name
+0001a960: 3d22 7465 7374 2d63 6f6e 6e65 6374 6f72  ="test-connector
+0001a970: 222c 0a20 2020 2020 2020 2074 696d 6573  ",.        times
+0001a980: 7461 6d70 3d22 5422 2c0a 2020 2020 2020  tamp="T",.      
+0001a990: 2020 696e 7075 7473 3d5b 2241 222c 2022    inputs=["A", "
+0001a9a0: 4222 5d2c 0a20 2020 2020 2020 206f 7574  B"],.        out
+0001a9b0: 7075 7473 3d5b 2243 222c 2022 4422 5d2c  puts=["C", "D"],
+0001a9c0: 0a20 2020 2020 2020 2066 6565 6462 6163  .        feedbac
+0001a9d0: 6b73 3d5b 2245 222c 2022 4622 5d2c 0a20  ks=["E", "F"],. 
+0001a9e0: 2020 2020 2020 206a 6f69 6e5f 6b65 793d         join_key=
+0001a9f0: 2248 222c 0a20 2020 2020 2020 2072 6f77  "H",.        row
+0001aa00: 5f74 6167 733d 5b22 4922 2c20 224a 225d  _tags=["I", "J"]
+0001aa10: 2c0a 2020 2020 2020 2020 676c 6f62 616c  ,.        global
+0001aa20: 5f74 6167 733d 7b22 7665 7273 696f 6e22  _tags={"version"
+0001aa30: 3a20 2274 6573 745f 7665 7273 696f 6e22  : "test_version"
+0001aa40: 7d2c 0a20 2020 2020 2020 2073 6368 6564  },.        sched
+0001aa50: 756c 653d 5363 6865 6475 6c65 280a 2020  ule=Schedule(.  
+0001aa60: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0001aa70: 6f6e 3d73 7461 7274 5f6f 6e2c 0a20 2020  on=start_on,.   
+0001aa80: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
+0001aa90: 6379 3d66 7265 7175 656e 6379 2c0a 2020  cy=frequency,.  
+0001aaa0: 2020 2020 2020 2020 2020 7479 7065 3d74            type=t
+0001aab0: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+0001aac0: 206f 7074 696f 6e73 3d53 6368 6564 756c   options=Schedul
+0001aad0: 654f 7074 696f 6e73 282a 2a6f 7074 696f  eOptions(**optio
+0001aae0: 6e73 292c 2020 2320 7479 7065 3a20 6967  ns),  # type: ig
+0001aaf0: 6e6f 7265 0a20 2020 2020 2020 2029 2c0a  nore.        ),.
+0001ab00: 2020 2020 290a 0a20 2020 2063 616c 6c5f      )..    call_
+0001ab10: 6172 6773 203d 2063 6c69 5f6f 626a 2e6c  args = cli_obj.l
+0001ab20: 6f67 5f73 746f 7265 2e6c 6f67 5f66 726f  og_store.log_fro
+0001ab30: 6d5f 6461 7461 5f63 6f6e 6e65 6374 6f72  m_data_connector
+0001ab40: 5f61 7379 6e63 2e63 616c 6c5f 6172 6773  _async.call_args
+0001ab50: 0a20 2020 2061 7373 6572 7420 6361 6c6c  .    assert call
+0001ab60: 5f61 7267 732e 6b77 6172 6773 203d 3d20  _args.kwargs == 
+0001ab70: 7b0a 2020 2020 2020 2020 2272 6571 7565  {.        "reque
+0001ab80: 7374 223a 2049 6e67 6573 7446 726f 6d44  st": IngestFromD
+0001ab90: 6174 6143 6f6e 6e65 6374 6f72 5265 7175  ataConnectorRequ
+0001aba0: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
+0001abb0: 2061 7070 6c69 6361 7469 6f6e 3d22 666f   application="fo
+0001abc0: 6f62 6172 222c 0a20 2020 2020 2020 2020  obar",.         
+0001abd0: 2020 2073 6f75 7263 655f 6461 7461 5f63     source_data_c
+0001abe0: 6f6e 6e65 6374 6f72 5f6e 616d 653d 2274  onnector_name="t
+0001abf0: 6573 742d 636f 6e6e 6563 746f 7222 2c0a  est-connector",.
+0001ac00: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0001ac10: 7374 616d 703d 2254 222c 0a20 2020 2020  stamp="T",.     
+0001ac20: 2020 2020 2020 2069 6e70 7574 733d 5b22         inputs=["
+0001ac30: 4122 2c20 2242 225d 2c0a 2020 2020 2020  A", "B"],.      
+0001ac40: 2020 2020 2020 6f75 7470 7574 733d 5b22        outputs=["
+0001ac50: 4322 2c20 2244 225d 2c0a 2020 2020 2020  C", "D"],.      
+0001ac60: 2020 2020 2020 6665 6564 6261 636b 733d        feedbacks=
+0001ac70: 5b22 4522 2c20 2246 225d 2c0a 2020 2020  ["E", "F"],.    
+0001ac80: 2020 2020 2020 2020 6a6f 696e 5f6b 6579          join_key
+0001ac90: 3d22 4822 2c0a 2020 2020 2020 2020 2020  ="H",.          
+0001aca0: 2020 726f 775f 7461 6773 3d5b 2249 222c    row_tags=["I",
+0001acb0: 2022 4a22 5d2c 0a20 2020 2020 2020 2020   "J"],.         
+0001acc0: 2020 2067 6c6f 6261 6c5f 7461 6773 3d7b     global_tags={
+0001acd0: 2276 6572 7369 6f6e 223a 2022 7465 7374  "version": "test
+0001ace0: 5f76 6572 7369 6f6e 227d 2c0a 2020 2020  _version"},.    
+0001acf0: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+0001ad00: 3d53 6368 6564 756c 6528 0a20 2020 2020  =Schedule(.     
+0001ad10: 2020 2020 2020 2020 2020 2073 7461 7274             start
+0001ad20: 5f6f 6e3d 7374 6172 745f 6f6e 2e69 736f  _on=start_on.iso
+0001ad30: 666f 726d 6174 2829 0a20 2020 2020 2020  format().       
+0001ad40: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0001ad50: 7374 616e 6365 2873 7461 7274 5f6f 6e2c  stance(start_on,
+0001ad60: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+0001ad70: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+0001ad80: 2020 2020 656c 7365 2073 7461 7274 5f6f      else start_o
+0001ad90: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0001ada0: 2020 2066 7265 7175 656e 6379 3d66 7265     frequency=fre
+0001adb0: 7175 656e 6379 2c0a 2020 2020 2020 2020  quency,.        
+0001adc0: 2020 2020 2020 2020 7479 7065 3d74 7970          type=typ
+0001add0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001ade0: 2020 206f 7074 696f 6e73 3d53 6368 6564     options=Sched
+0001adf0: 756c 654f 7074 696f 6e73 282a 2a6f 7074  uleOptions(**opt
+0001ae00: 696f 6e73 292c 2020 2320 7479 7065 3a20  ions),  # type: 
+0001ae10: 6967 6e6f 7265 0a20 2020 2020 2020 2020  ignore.         
+0001ae20: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+0001ae30: 2020 7069 7065 6c69 6e65 5f6e 616d 653d    pipeline_name=
+0001ae40: 4e6f 6e65 2c0a 2020 2020 2020 2020 290a  None,.        ).
+0001ae50: 2020 2020 7d0a                               }.
```

### Comparing `gantry-0.6.6/tests/logger/test_consumer.py` & `gantry-0.6.7/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/logger/test_event_builder.py` & `gantry-0.6.7/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/logger/test_main.py` & `gantry-0.6.7/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/logger/test_stores.py` & `gantry-0.6.7/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/logger/test_utils.py` & `gantry-0.6.7/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/conftest.py` & `gantry-0.6.7/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/core/test_dataframe.py` & `gantry-0.6.7/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/core/test_distance.py` & `gantry-0.6.7/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/core/test_filters.py` & `gantry-0.6.7/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/core/test_metric.py` & `gantry-0.6.7/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/core/test_queryframe.py` & `gantry-0.6.7/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/core/test_series.py` & `gantry-0.6.7/tests/query/core/test_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,32 +80,32 @@
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_count(mock_query, num_points_kwargs, series_obj):
     mock_query.return_value = 100
     assert series_obj.count(**num_points_kwargs) == 100
     mock_query.assert_called_once_with(
-        "total", num_points=num_points_kwargs.get("num_points", 1), group_by=None
+        "total", num_points=num_points_kwargs.get("num_points", 1), group_by=None, limit_buckets=20
     )
 
 
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_len(mock_query, series_obj):
     mock_query.return_value = 100
     assert len(series_obj) == 100
-    mock_query.assert_called_once_with("total", num_points=1, group_by=None)
+    mock_query.assert_called_once_with("total", num_points=1, group_by=None, limit_buckets=20)
 
 
 @pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_count_error(mock_query, error, series_obj):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj.count()
-    mock_query.assert_called_once_with("total", num_points=1, group_by=None)
+    mock_query.assert_called_once_with("total", num_points=1, group_by=None, limit_buckets=20)
 
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @pytest.mark.parametrize("datatype", ["int", "float"])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_min(mock_query, datatype, num_points_kwargs, series_obj_factory):
     series_obj = series_obj_factory(datatype)
@@ -258,32 +258,32 @@
     [
         (None, "str"),
         ("proj_datanode", "intC"),
         ("feed_datanode", "intB"),
         ("column-missing-from-schema", None),
     ],
 )
-@mock.patch("gantry.query.core.dataframe._raw_query_cached_request")
+@mock.patch("gantry.query.core.dataframe._raw_query_request")
 def test_aggregate_query(
     mock_query_data, series_obj_factory_with_filters_and_tags, filters, tags, group_by_info
 ):
     group_by = group_by_info[0]
     group_by_type = group_by_info[1]
     content_dict = {
         "start_time": "2008-09-03T20:56:35",
         "end_time": "2008-09-10T23:58:23",
         "version": "1.2.3",
         "num_points": 1,
         "queries": {
             "query": {
-                "query_type": "feature",
+                "query_type": "features",
                 "model_node_id": "ABCD1234",
                 "stat": "some-attribute",
                 "stat_kwargs": {"some-attribute": {"a": 10}},
-                "feature": "series_name",
+                "features": [{"name": "series_name", "dtype": None}],
                 "filters": filters,
                 "tags": tags,
             }
         },
     }
     if group_by is not None:
         content_dict["queries"]["query"]["group_by"] = [
@@ -322,44 +322,43 @@
         with pytest.raises(ValueError, match=f"Cannot find column {group_by} in dataframe."):
             result = series_obj._aggregate_query("some-attribute", a=10, group_by=group_by)
 
 
 @pytest.mark.parametrize("num_points", [2, 5, 10])
 @pytest.mark.parametrize("tags", [{}, {"foo": "bar"}])
 @pytest.mark.parametrize("filters", [[], [{"some": "filter"}]])
-@mock.patch("gantry.query.core.dataframe._raw_query_cached_request")
+@mock.patch("gantry.query.core.dataframe._raw_query_request")
 def test_aggregate_query_num_points(
     mock_query_data, series_obj_factory_with_filters_and_tags, filters, tags, num_points
 ):
     content = json.dumps(
         {
             "start_time": "2008-09-03T20:56:35",
             "end_time": "2008-09-10T23:58:23",
             "version": "1.2.3",
             "num_points": num_points,
             "queries": {
                 "query": {
-                    "query_type": "feature",
+                    "query_type": "features",
                     "model_node_id": "ABCD1234",
                     "stat": "some-attribute",
                     "stat_kwargs": {"some-attribute": {"a": 10}},
-                    "feature": "series_name",
+                    "features": [{"name": "series_name", "dtype": None}],
                     "filters": filters,
                     "tags": tags,
                 }
             },
         },
         default=lambda x: x.isoformat(),
     )
     series_obj = series_obj_factory_with_filters_and_tags("int", filters=filters, tags=tags)
     mock_query_data.return_value = {
         "response": "ok",
         "data": {"query": {"points": [{"A": 10, "B": 10}, {"A": 20, "B": 20}]}},
     }
-
     res = series_obj._aggregate_query("some-attribute", num_points=num_points, a=10)
     assert_frame_equal(res, pd.DataFrame([{"A": 10, "B": 10}, {"A": 20, "B": 20}]))
 
     mock_query_data.assert_called_with(series_obj.api_client, content, resource="time_series")
 
 
 @pytest.mark.parametrize("tags", [{}, {"foo": "bar"}])
@@ -386,37 +385,37 @@
     series_obj = series_obj_factory("int")
     with pytest.raises(
         ValueError,
     ):
         _ = series_obj._aggregate_query("some-attribute", num_points=invalid_num_points, a=10)
 
 
-def test_raw_query_cached_request_default_resource(api_client_obj):
+def test_raw_query_request_default_resource(api_client_obj):
     with responses.RequestsMock() as rsps:
         rsps.add(
             responses.POST,
             "{}/api/v1/aggregate/query".format(ORIGIN),
             json={"response": "ok", "data": "100"},
             match=[matchers.json_params_matcher({"foo": "bar"})],
         )
-        assert dataframe._raw_query_cached_request(api_client_obj, '{"foo": "bar"}') == {
+        assert dataframe._raw_query_request(api_client_obj, '{"foo": "bar"}') == {
             "response": "ok",
             "data": "100",
         }
 
 
-def test_raw_query_cached_request_provided_resource(api_client_obj):
+def test_raw_query_request_provided_resource(api_client_obj):
     with responses.RequestsMock() as rsps:
         rsps.add(
             responses.POST,
             "{}/api/v1/foobar/query".format(ORIGIN),
             json={"response": "ok", "data": "100"},
             match=[matchers.json_params_matcher({"foo": "bar"})],
         )
-        assert dataframe._raw_query_cached_request(
+        assert dataframe._raw_query_request(
             api_client_obj, '{"foo": "bar"}', resource="foobar"
         ) == {
             "response": "ok",
             "data": "100",
         }
```

### Comparing `gantry-0.6.6/tests/query/core/test_utils.py` & `gantry-0.6.7/tests/query/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/distance/test_main.py` & `gantry-0.6.7/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/metric/test_main.py` & `gantry-0.6.7/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/test_client.py` & `gantry-0.6.7/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/query/test_main.py` & `gantry-0.6.7/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/test_api_client.py` & `gantry-0.6.7/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/test_init.py` & `gantry-0.6.7/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/test_utils.py` & `gantry-0.6.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.6/tests/test_validator.py` & `gantry-0.6.7/tests/test_validator.py`

 * *Files identical despite different names*

