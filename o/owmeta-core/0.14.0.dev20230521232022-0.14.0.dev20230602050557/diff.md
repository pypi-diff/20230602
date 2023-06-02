# Comparing `tmp/owmeta-core-0.14.0.dev20230521232022.tar.gz` & `tmp/owmeta-core-0.14.0.dev20230602050557.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owmeta-core-0.14.0.dev20230521232022.tar", last modified: Sun May 21 23:20:24 2023, max compression
+gzip compressed data, was "owmeta-core-0.14.0.dev20230602050557.tar", last modified: Fri Jun  2 05:05:58 2023, max compression
```

## Comparing `owmeta-core-0.14.0.dev20230521232022.tar` & `owmeta-core-0.14.0.dev20230602050557.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:20:24.531183 owmeta-core-0.14.0.dev20230521232022/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-21 23:20:24.531183 owmeta-core-0.14.0.dev20230521232022/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:20:24.527183 owmeta-core-0.14.0.dev20230521232022/owmeta_core/
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-05-21 23:20:22.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/agg_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bittorrent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:20:24.527183 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:20:24.531183 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24779 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle_dependency_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/capability.py
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/capability_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/capable_configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli_command_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)   115314 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/command_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:20:24.531183 owmeta-core-0.14.0.dev20230521232022/owmeta_core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/commands/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/context_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/context_dataobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/context_mapped_class_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/context_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/contextualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/custom_dataobject_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:20:24.531183 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/common_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/context_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/csv_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/excel_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/file_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/http_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/local_file_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    31191 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/dataobject_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    35750 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/datasource_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/default.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/file_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/graph_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/graph_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/identifier_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/inverse_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    25718 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/mapped_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/property_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/property_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/ranged_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_query_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_query_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_type_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/requests_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:20:24.527183 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-21 23:20:24.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-21 23:20:24.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:20:24.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-21 23:20:24.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:20:24.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 23:20:24.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 23:20:24.000000 owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-21 23:20:24.531183 owmeta-core-0.14.0.dev20230521232022/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-21 23:20:16.000000 owmeta-core-0.14.0.dev20230521232022/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:05:58.976227 owmeta-core-0.14.0.dev20230602050557/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-02 05:05:58.976227 owmeta-core-0.14.0.dev20230602050557/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:05:58.972227 owmeta-core-0.14.0.dev20230602050557/owmeta_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-02 05:05:57.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/agg_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bittorrent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:05:58.972227 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:05:58.972227 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24779 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle_dependency_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/capability_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/capable_configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli_command_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115314 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/command_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:05:58.976227 owmeta-core-0.14.0.dev20230602050557/owmeta_core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/commands/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/context_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/context_dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/context_mapped_class_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/context_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/contextualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/custom_dataobject_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:05:58.976227 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/common_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/context_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/csv_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/excel_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/file_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/http_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/local_file_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31191 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/dataobject_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35750 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/datasource_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/default.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/file_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/graph_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/graph_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/identifier_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/inverse_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25718 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/mapped_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/property_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/property_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/ranged_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_query_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_query_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_type_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/requests_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:05:58.972227 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-02 05:05:58.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-02 05:05:58.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:05:58.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-02 05:05:58.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:05:58.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-02 05:05:58.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 05:05:58.000000 owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 05:05:58.976227 owmeta-core-0.14.0.dev20230602050557/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-02 05:05:45.000000 owmeta-core-0.14.0.dev20230602050557/setup.py
```

### Comparing `owmeta-core-0.14.0.dev20230521232022/LICENSE.txt` & `owmeta-core-0.14.0.dev20230602050557/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/PKG-INFO` & `owmeta-core-0.14.0.dev20230602050557/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owmeta-core
-Version: 0.14.0.dev20230521232022
+Version: 0.14.0.dev20230602050557
 Summary: owmeta-core is a platform for sharing relational data over the internet.
 Home-page: https://owmeta-core.readthedocs.io/en/latest/
 Author: OpenWorm.org authors and contributors
 Author-email: info@openworm.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `owmeta-core-0.14.0.dev20230521232022/README.md` & `owmeta-core-0.14.0.dev20230602050557/README.md`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/__init__.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 owmeta_core
 ===========
 owmeta-core is a platform for sharing relational data over the internet.
 """
 
 from __future__ import print_function
-__version__ = '0.14.0.dev20230521232022'
+__version__ = '0.14.0.dev20230602050557'
 __author__ = 'OpenWorm.org authors and contributors'
 
 import sys
 import os
 import logging
 import uuid
 from os.path import join as pth_join
```

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/agg_store.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/agg_store.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/__init__.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/archive.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/archive.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/common.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/common.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/exceptions.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/exceptions.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/__init__.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/http.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/http.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/local.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/local.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle/loaders/sftp.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle/loaders/sftp.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/bundle_dependency_store.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/bundle_dependency_store.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/capabilities.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/capabilities.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/capability.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/capability.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/capability_providers.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/capability_providers.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/capable_configurable.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/capable_configurable.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli_command_wrapper.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli_command_wrapper.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli_common.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli_common.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/cli_hints.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/cli_hints.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/collections.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/collections.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/command.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/command.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/command_util.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/command_util.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/commands/bundle.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/commands/bundle.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/configure.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/configure.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/context.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/context.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/context_dataobject.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/context_dataobject.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/context_mapped_class_util.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/context_mapped_class_util.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/context_store.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/context_store.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/contextualize.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/contextualize.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/custom_dataobject_property.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/custom_dataobject_property.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/data.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/data.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/common_data.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/common_data.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/context_datasource.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/context_datasource.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/csv_ds.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/csv_ds.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/file_ds.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/file_ds.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/data_trans/local_file_ds.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/data_trans/local_file_ds.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/dataobject.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/dataobject.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/dataobject_property.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/dataobject_property.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/datasource.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/datasource.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/datasource_loader.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/datasource_loader.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/docscrape.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/docscrape.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/file_lock.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/file_lock.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/file_match.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/file_match.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/file_utils.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/file_utils.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/git_repo.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/git_repo.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/graph_object.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/graph_object.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/graph_serialization.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/graph_serialization.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/identifier_mixin.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/identifier_mixin.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/inverse_property.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/inverse_property.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/json_schema.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/json_schema.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/mapped_class.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/mapped_class.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/mapper.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/mapper.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/property_mixins.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/property_mixins.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/property_value.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/property_value.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/quantity.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/quantity.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/ranged_objects.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/ranged_objects.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_query_modifiers.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_query_modifiers.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_query_util.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_query_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,23 +51,25 @@
         t = grouped_types.get(ident, None)
         if t is None:
             ids_missing_types.remove(ident)
             grouped_types[ident] = set([rdf_type])
         else:
             t.add(rdf_type)
     if ids_missing_types:
-        raise MissingRDFTypeException('Could not recover a type declaration for'
-                                      f' {ids_missing_types}')
+        L.debug('Could not recover type declarations for %r. Defaulting to %s',
+                ids_missing_types, rdflib.RDFS.Resource)
+        for ident in ids_missing_types:
+            grouped_types[ident] = set([rdflib.RDFS.Resource])
 
     for ident, types in grouped_types.items():
         the_type = resolver.type_resolver(graph, types, base=target_type)
         if the_type is None:
             raise MissingRDFTypeException(
-                    f'The type resolver could not recover a type for {ident}'
-                    f' from {types} constrained to {target_type}')
+                    f'The type resolver could not recover an RDF type for {ident}'
+                    f' from {types} in {graph} constrained to sub-classes of {target_type}')
         yield resolver.id2ob(ident, the_type, context)
 
 
 def load_terms(graph, start, target_type):
     '''
     Loads a set of terms based on the object graph starting from `start`
```

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_type_resolver.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_type_resolver.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/rdf_utils.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/rdf_utils.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/requests_sessions.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/requests_sessions.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/statement.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/statement.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/text_util.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/text_util.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/utils.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/utils.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core/variable.py` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core/variable.py`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/PKG-INFO` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owmeta-core
-Version: 0.14.0.dev20230521232022
+Version: 0.14.0.dev20230602050557
 Summary: owmeta-core is a platform for sharing relational data over the internet.
 Home-page: https://owmeta-core.readthedocs.io/en/latest/
 Author: OpenWorm.org authors and contributors
 Author-email: info@openworm.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/SOURCES.txt` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/entry_points.txt` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/owmeta_core.egg-info/requires.txt` & `owmeta-core-0.14.0.dev20230602050557/owmeta_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `owmeta-core-0.14.0.dev20230521232022/setup.py` & `owmeta-core-0.14.0.dev20230602050557/setup.py`

 * *Files identical despite different names*

