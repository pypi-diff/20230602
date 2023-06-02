# Comparing `tmp/xoa-core-1.0.8.tar.gz` & `tmp/xoa-core-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-core-1.0.8.tar", last modified: Thu Feb 16 09:22:05 2023, max compression
+gzip compressed data, was "xoa-core-2.0.0.tar", last modified: Fri Jun  2 07:25:54 2023, max compression
```

## Comparing `xoa-core-1.0.8.tar` & `xoa-core-2.0.0.tar`

### file list

```diff
@@ -1,70 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.319819 xoa-core-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-02-16 09:21:46.000000 xoa-core-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-02-16 09:22:05.319819 xoa-core-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-02-16 09:21:46.000000 xoa-core-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-16 09:21:46.000000 xoa-core-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-16 09:22:05.319819 xoa-core-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-16 09:21:46.000000 xoa-core-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.315819 xoa-core-1.0.8/xoa_core/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.315819 xoa-core-1.0.8/xoa_core/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.315819 xoa-core-1.0.8/xoa_core/core/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/executors/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/executors/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/executors/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/executors/executor_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/executors/executor_state_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/executors/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/generic_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.315819 xoa-core-1.0.8/xoa_core/core/messanger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/messanger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/messanger/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/messanger/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/messanger/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/plugin_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.319819 xoa-core-1.0.8/xoa_core/core/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.319819 xoa-core-1.0.8/xoa_core/core/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.319819 xoa-core-1.0.8/xoa_core/core/resources/datasets/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/external/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/external/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/external/port.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/external/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.319819 xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/resources_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/resources/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.319819 xoa-core-1.0.8/xoa_core/core/test_suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/test_suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/test_suites/_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/test_suites/controler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/test_suites/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.319819 xoa-core-1.0.8/xoa_core/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/utils/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/core/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-16 09:21:46.000000 xoa-core-1.0.8/xoa_core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:22:05.315819 xoa-core-1.0.8/xoa_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-02-16 09:22:05.000000 xoa-core-1.0.8/xoa_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-02-16 09:22:05.000000 xoa-core-1.0.8/xoa_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 09:22:05.000000 xoa-core-1.0.8/xoa_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-16 09:22:05.000000 xoa-core-1.0.8/xoa_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-16 09:22:05.000000 xoa-core-1.0.8/xoa_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-02 07:25:44.000000 xoa-core-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-02 07:25:54.068522 xoa-core-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-02 07:25:44.000000 xoa-core-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 07:25:44.000000 xoa-core-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 07:25:54.068522 xoa-core-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 07:25:44.000000 xoa-core-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor_state_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/generic_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/messenger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/plugin_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/resources/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/xoa_core/core/resources/resource/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/__decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/xoa_core/core/test_suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/xoa_core/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/utils/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/top_level.txt
```

### Comparing `xoa-core-1.0.8/LICENSE` & `xoa-core-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-core-1.0.8/PKG-INFO` & `xoa-core-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 Metadata-Version: 2.1
 Name: xoa-core
-Version: 1.0.8
+Version: 2.0.0
 Summary: Xena Open Automation framework for Xena test suite execution, integration, and development.
 Home-page: https://github.com/xenanetworks/open-automation-core
-Author: Artem Constantinov, Frank Chen
-Author-email: aco@xenanetworks.com, fch@xenanewtorks.com
+Author: Artem Constantinov, Leonard Yu
+Author-email: aco@xenanetworks.com, hyu@xenanewtorks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-core) [![PyPI](https://img.shields.io/pypi/v/xoa-core)](https://pypi.python.org/pypi/xoa-core) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-core) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-core/badge/?version=latest)](https://xena-openautomation-core.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-core) [![PyPI](https://img.shields.io/pypi/v/xoa-core)](https://pypi.python.org/pypi/xoa-core) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-core) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-core/badge/?version=stable)](https://xena-openautomation-core.readthedocs.io/en/stable/?badge=stable)
 
 # Xena OpenAutomation Core
-Xena OpenAutomation (XOA) Core is the framework that provides a standardized way for developers and test specialists to execute, develop, and integrate test suites, as well as managing Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
+Xena OpenAutomation Core (XOA Core) is an open-source test suite framework for network automation and testing. It is designed to host various [XOA Test Suites](https://github.com/xenanetworks/open-automation-test-suites) as plugins, allowing users to create, manage, and run test cases for different network scenarios. The XOA Core framework serves as the foundation for building and executing test suites in the XOA ecosystem.
+
+Key features of XOA Core include:
+
+1. Modular architecture: The test suite framework employs a modular architecture, enabling users to develop and run different test suites as plugins.
 
-We open the source code of XOA Core to the public to empower our users with the freedom to tailor the code to their unique needs, develop and integrate their own test suites, so that XOA Core not only works with Xena-developed test suites.
+2. Test Suite execution: XOA Core supports both local and remote test suite execution. Users can execute test suites on their local machines or on remote testbeds through the XOA CLI or Web GUI.
 
-All of Xena-developed test suites are in this repository: [XOA Test Suites](https://github.com/xenanetworks/open-automation-test-suites).
+3. Test Case management: XOA Core provides tools for managing test cases, including creating, updating, and deleting them. Users can also organize test cases using tags and execute them in parallel or sequentially.
 
-XOA Core uses [XOA Python API](https://github.com/xenanetworks/open-automation-python-api) as the driver to administer Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
+4. Extensibility: The framework is designed to be extensible, allowing users to develop custom test suites and plugins to address specific testing requirements.
+
+5. Logging and reporting: XOA Core offers built-in logging and reporting functionality, generating detailed test reports to help users analyze test results and identify issues.
+Xena OpenAutomation (XOA) Core is the framework that provides a standardized way for developers and test specialists to execute, develop, and integrate test suites, as well as managing Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
 
 ## Documentation
 The user documentation is hosted:
-[Xena OpenAutomation Core Documentation](https://docs.xoa-core.xenanetworks.com/)
+[Xena OpenAutomation Core Documentation](https://docs.xenanetworks.com/projects/xoa-core)
 
 ## Installation
 
 ### Install Using `pip`
 Make sure Python `pip` is installed on you system. If you are using virtualenv, then pip is already installed into environments created by virtualenv, and using sudo is not needed. If you do not have pip installed, download this file: https://bootstrap.pypa.io/get-pip.py and run `python get-pip.py`.
 
 To install the latest, use pip to install from pypi:
```

### Comparing `xoa-core-1.0.8/README.md` & `xoa-core-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-core) [![PyPI](https://img.shields.io/pypi/v/xoa-core)](https://pypi.python.org/pypi/xoa-core) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-core) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-core/badge/?version=latest)](https://xena-openautomation-core.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-core) [![PyPI](https://img.shields.io/pypi/v/xoa-core)](https://pypi.python.org/pypi/xoa-core) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-core) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-core/badge/?version=stable)](https://xena-openautomation-core.readthedocs.io/en/stable/?badge=stable)
 
 # Xena OpenAutomation Core
-Xena OpenAutomation (XOA) Core is the framework that provides a standardized way for developers and test specialists to execute, develop, and integrate test suites, as well as managing Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
+Xena OpenAutomation Core (XOA Core) is an open-source test suite framework for network automation and testing. It is designed to host various [XOA Test Suites](https://github.com/xenanetworks/open-automation-test-suites) as plugins, allowing users to create, manage, and run test cases for different network scenarios. The XOA Core framework serves as the foundation for building and executing test suites in the XOA ecosystem.
+
+Key features of XOA Core include:
+
+1. Modular architecture: The test suite framework employs a modular architecture, enabling users to develop and run different test suites as plugins.
 
-We open the source code of XOA Core to the public to empower our users with the freedom to tailor the code to their unique needs, develop and integrate their own test suites, so that XOA Core not only works with Xena-developed test suites.
+2. Test Suite execution: XOA Core supports both local and remote test suite execution. Users can execute test suites on their local machines or on remote testbeds through the XOA CLI or Web GUI.
 
-All of Xena-developed test suites are in this repository: [XOA Test Suites](https://github.com/xenanetworks/open-automation-test-suites).
+3. Test Case management: XOA Core provides tools for managing test cases, including creating, updating, and deleting them. Users can also organize test cases using tags and execute them in parallel or sequentially.
 
-XOA Core uses [XOA Python API](https://github.com/xenanetworks/open-automation-python-api) as the driver to administer Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
+4. Extensibility: The framework is designed to be extensible, allowing users to develop custom test suites and plugins to address specific testing requirements.
+
+5. Logging and reporting: XOA Core offers built-in logging and reporting functionality, generating detailed test reports to help users analyze test results and identify issues.
+Xena OpenAutomation (XOA) Core is the framework that provides a standardized way for developers and test specialists to execute, develop, and integrate test suites, as well as managing Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
 
 ## Documentation
 The user documentation is hosted:
-[Xena OpenAutomation Core Documentation](https://docs.xoa-core.xenanetworks.com/)
+[Xena OpenAutomation Core Documentation](https://docs.xenanetworks.com/projects/xoa-core)
 
 ## Installation
 
 ### Install Using `pip`
 Make sure Python `pip` is installed on you system. If you are using virtualenv, then pip is already installed into environments created by virtualenv, and using sudo is not needed. If you do not have pip installed, download this file: https://bootstrap.pypa.io/get-pip.py and run `python get-pip.py`.
 
 To install the latest, use pip to install from pypi:
@@ -212,8 +219,8 @@
 
 > Note:
 > ``_filter`` argument is optional. If it is not provided, all message types will be returned from this test suite execution.
 
 
 ***
 
-FOR TESTING BEYOND THE STANDARD.
+FOR TESTING BEYOND THE STANDARD.
```

### Comparing `xoa-core-1.0.8/setup.py` & `xoa-core-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,31 @@
         long_description = fh.read()
 
     setuptools.setup(
         name="xoa-core",
         description="Xena Open Automation framework for Xena test suite execution, integration, and development.",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        author="Artem Constantinov, Frank Chen",
-        author_email="aco@xenanetworks.com, fch@xenanewtorks.com",
+        author="Artem Constantinov, Leonard Yu",
+        author_email="aco@xenanetworks.com, hyu@xenanewtorks.com",
         maintainer="Xena Networks",
         maintainer_email="support@xenanetworks.com",
         url="https://github.com/xenanetworks/open-automation-core",
         packages=setuptools.find_packages(),
         license='Apache 2.0',
-        install_requires=["xoa_driver>=1.0.12", "pydantic", "semver", "oyaml", "loguru"],
+        install_requires=["xoa_driver>=2.0", "pydantic", "semver", "oyaml", "loguru"],
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
-            "Topic :: Software Development :: Build Tools",
+            "Topic :: Software Development :: Libraries :: Application Frameworks",
             "License :: OSI Approved :: Apache Software License",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
         ],
         python_requires=">=3.8.9",
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `xoa-core-1.0.8/xoa_core/core/exceptions.py` & `xoa-core-2.0.0/xoa_core/core/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from xoa_core import __version__
 
+
 class TestSuiteNotExistError(Exception):
     def __init__(self, name: str) -> None:
         self.name = name
         self.msg = f"Test Suite: <{self.name}> is not exist."
         super().__init__(self.msg)
 
+
 class TestSuiteVersionError(Exception):
     def __init__(self, name: str, required_version: str) -> None:
         self.name = name
         self.required_version = required_version
         self.msg = f"Test Suite: <{self.name}> require framework version of <{self.required_version}> current is: <{__version__}>"
         super().__init__(self.msg)
 
+
 class MultiModeError(Exception):
     def __init__(self) -> None:
         self.msg = "Only single Test suite execution is permited."
         super().__init__(self.msg)
 
+
 class InvalidPluginError(ValueError):
     def __init__(self, value, expected) -> None:
         self.value = value
         self.expected = expected
         self.msg = f"Invalid plugin. Plugin Entry Class {self.value} must be a subclass of {self.expected}."
         super().__init__(self.msg)
-
-
-
```

### Comparing `xoa-core-1.0.8/xoa_core/core/executors/executor.py` & `xoa-core-2.0.0/xoa_core/core/executors/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import asyncio
 import contextlib
 import uuid
 import typing
 from xoa_core.core.generic_types import (
     TObserver,
     TMesagesPipe,
-    PipeFacade
 )
 if typing.TYPE_CHECKING:
     from xoa_core.types import PluginAbstract
+    from xoa_core.core.plugin_abstract import (
+        PStateConditionsFacade,
+        PPipeFacade
+    )
 
+from .executor_info import ExecutorInfo
 from . import exceptions
 from ._events import Event
 from .executor_state import ExecutorState
-from .executor_state_conditions import (
-    StateConditions,
-    StateConditionsFacade
-)
+from .executor_state_conditions import StateConditions
 
 
 class PPlugin(typing.Protocol):
-    def create_test_suite(self, state_conditions: "StateConditionsFacade", xoa_out: "PipeFacade") -> "PluginAbstract":
-        ...
-
-# TODO: Need to improve attributes creation in this class
+    def create_test_suite(self, state_conditions: "PStateConditionsFacade", xoa_out: "PPipeFacade") -> "PluginAbstract": ...  # noqa: E704
 
 
 class SuiteExecutor:
     __slots__ = ("suite_name", "state", "__id", "__observer", "__msg_pipe", "__test_suite", "__task", "state_conditions",)
 
     def __init__(self, suite_name: str) -> None:
         self.__id = str(uuid.uuid4())
@@ -47,22 +45,29 @@
         with contextlib.suppress(asyncio.CancelledError, exceptions.StopPlugin):
             e = task.exception()
             if e is None:
                 return None
             self.__observer.emit(Event.ERROR, task.get_name(), e)
             raise e
 
+    def get_info(self) -> ExecutorInfo:
+        return ExecutorInfo(
+            id=self.__id,
+            suite_name=self.suite_name,
+            state=self.state.current_state,
+        )
+
     def assign_pipe(self, pipe: "TMesagesPipe") -> None:
         self.__msg_pipe = pipe
         self.state.assign_senders(pipe.get_state_facade())
 
     def assign_plugin(self, plugin: PPlugin) -> None:
         self.__test_suite = plugin.create_test_suite(
             state_conditions=self.state_conditions.get_facade(),
-            xoa_out=self.__msg_pipe.get_facade()
+            xoa_out=self.__msg_pipe.get_facade(self.suite_name)
         )
 
     def run(self, observer: TObserver) -> None:
         self.__observer = observer
         self.state.set_run()
         self.__task = asyncio.create_task(
             self.__test_suite.start(),
```

### Comparing `xoa-core-1.0.8/xoa_core/core/executors/executor_state.py` & `xoa-core-2.0.0/xoa_core/core/executors/executor_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,32 @@
 
 
 def no_sender(status: Optional[str], old_status: Optional[str]) -> None:
     return None
 
 
 class ExecutorState:
-    __slots__ = ("__state", "__sender", "__sender_is_set",)
+    __slots__ = ("__state", "__sender", "__sender_is_set")
 
     def __init__(self) -> None:
         self.__state = EState.STOPPED
         self.__sender = no_sender
         self.__sender_is_set = False
 
     def assign_senders(self, sender: "SenderType") -> None:
         if self.__sender_is_set:
             return None
         self.__sender = sender
         self.__sender_is_set = True
 
     @property
+    def current_state(self) -> str:
+        return self.__state.value
+
+    @property
     def is_stoped(self) -> bool:
         return self.__state is EState.STOPPED
 
     @property
     def is_paused(self) -> bool:
         return self.__state is EState.PAUSED
```

### Comparing `xoa-core-1.0.8/xoa_core/core/executors/executor_state_conditions.py` & `xoa-core-2.0.0/xoa_core/core/executors/executor_state_conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from . import exceptions
 
 
 class StateConditionsFacade:
-    __slots__ = ("__wait_if_paused", "__stop_if_stopped",)
+    __slots__ = ("__wait_if_paused", "__stop_if_stopped")
 
-    def __init__(self, wait_if_paused, stop_if_stopped) -> None:
+    def __init__(self, wait_if_paused, stop_if_stopped) -> None:  # TODO: Add type notations
         self.__wait_if_paused = wait_if_paused
         self.__stop_if_stopped = stop_if_stopped
 
     async def wait_if_paused(self) -> None:
         await self.__wait_if_paused()
 
     async def stop_if_stopped(self) -> None:
```

### Comparing `xoa-core-1.0.8/xoa_core/core/executors/manager.py` & `xoa-core-2.0.0/xoa_core/core/executors/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
 import typing
 from xoa_core.core.utils import observer
 from xoa_core.core import exceptions
-
+from .executor_info import ExecutorInfo
 from .executor import SuiteExecutor
 from ._events import Event
 
 from xoa_core.core.generic_types import TMesagesPipe
 
 
 class ExecutorsManager:
@@ -22,25 +23,34 @@
         self.__observer.subscribe(Event.ERROR, self.__on_execution_error)
 
     async def __on_execution_stopped(self, exec_id: str) -> None:
         del self.__executors[exec_id]
         self.__msg_pipe.transmit(f"Test Suite stopped: {exec_id}")
 
     async def __on_execution_error(self, suite_name: str, error: Exception) -> None:
-        # print(suite_name, error)
         self.__msg_pipe.transmit(f"Test Suite Error: {suite_name}, {error}")
 
     def run(self, executor: "SuiteExecutor") -> str:
         if self.__mono and len(self.__executors) > 1:
             raise exceptions.MultiModeError()
         self.__executors[executor.id] = executor
         executor.run(self.__observer)
         self.__msg_pipe.transmit(f"Test Suite Started: {executor.id}")
         return executor.id
 
+    def get_executors_info(self) -> list[ExecutorInfo]:
+        return [
+            ex.get_info()
+            for ex in self.__executors.values()
+        ]
+
+    def get_state(self, exec_id: str) -> str | None:
+        if ex := self.__executors.get(exec_id):
+            return ex.state.current_state
+
     async def stop(self, exec_id: str) -> None:
         if ex := self.__executors.get(exec_id):
             await ex.stop()
 
     async def toggle_pause(self, exec_id: str) -> None:
         if ex := self.__executors.get(exec_id):
             await ex.toggle_pause()
```

### Comparing `xoa-core-1.0.8/xoa_core/core/generic_types.py` & `xoa-core-2.0.0/xoa_core/core/generic_types.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,48 +12,50 @@
 
 if TYPE_CHECKING:
     import asyncio
     # from xoa_driver import testers
     from functools import partialmethod
     # from valhalla_core.core.test_suites.datasets import PluginData
 
-from xoa_core.core.messanger.misc import EMsgType, Message, PipeFacade, PipeStateFacade
+from xoa_core.core.messenger.misc import EMsgType, Message, PipeFacade, PipeStateFacade
 
 
 # region Execution Manager
 
 # TTesterReceaver = Callable[[str, str], Optional["testers.GenericAnyTester"]]
 
 # endregion
 
 # region Utils SimpleObserver
 
 TCallback = Callable[..., Coroutine[Any, None, None]]
 
+
 class TObserver(Protocol):
-    def subscribe(self, evt: int, func: TCallback) -> None: ...
-    def emit(self, evt: int, *args, **kwargs) -> None: ...
+    def subscribe(self, evt: int, func: TCallback) -> None: ...  # noqa: E704
+    def emit(self, evt: int, *args, **kwargs) -> None: ...  # noqa: E704
 
 # endregion
 
 
 # region Messanger
 
 
 class TMesagesPipe(Protocol):
-    async def _add_stream(self, key: str, queue: "asyncio.Queue") -> None: ...
-    async def _free_stream(self, key: str) -> None: ...
-    async def disable(self) -> None: ...
-    def transmit(self, msg: Any, *, msg_type: EMsgType = EMsgType.DATA) -> None: ...
-    def get_facade(self) -> PipeFacade: ...
-    def get_state_facade(self) -> PipeStateFacade: ...
+    async def _add_stream(self, key: str, queue: "asyncio.Queue") -> None: ...  # noqa: E704
+    async def _free_stream(self, key: str) -> None: ...  # noqa: E704
+    async def disable(self) -> None: ...  # noqa: E704
+    def transmit(self, msg: Any, *, msg_type: EMsgType = EMsgType.DATA) -> None: ...  # noqa: E704
+    def get_facade(self, suite_name: str) -> PipeFacade: ...  # noqa: E704
+    def get_state_facade(self) -> PipeStateFacade: ...  # noqa: E704
     transmit_warn: "partialmethod"
     transmit_err: "partialmethod"
 
+
 class TMessagesHandler(Protocol):
-    def get_pipe(self, name: str) -> "TMesagesPipe": ...
-    async def disable_pipe(self, name: str) -> None: ...
-    def avaliable_pipes(self) -> Tuple[str, ...]: ...
-    async def changes(self, *names: str) -> AsyncGenerator["Message", None]: ...
+    def get_pipe(self, name: str) -> "TMesagesPipe": ...  # noqa: E704
+    async def disable_pipe(self, name: str) -> None: ...  # noqa: E704
+    def avaliable_pipes(self) -> Tuple[str, ...]: ...  # noqa: E704
+    async def changes(self, *names: str) -> AsyncGenerator["Message", None]: ...  # noqa: E704
 
 
-# endregion
+# endregion
```

### Comparing `xoa-core-1.0.8/xoa_core/core/messanger/handler.py` & `xoa-core-2.0.0/xoa_core/core/messenger/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+from __future__ import annotations
 import asyncio
 import uuid
 import contextlib
 from typing import (
-    Optional,
-    Tuple,
-    Dict,
     Set,
     AsyncGenerator
 )
 from xoa_core.core.utils import observer
 from .pipe import MesagesPipe
 from . import misc
 
 
-async def _get_from_queue(queue: "asyncio.Queue[Optional[misc.Message]]") -> AsyncGenerator[Optional[misc.Message], None]:
+async def _get_from_queue(queue: asyncio.Queue[misc.Message | None]) -> AsyncGenerator[misc.Message | None, None]:
     while True:
         msg = await queue.get()
         try:
             yield msg
         finally:
             queue.task_done()
 
 
 class OutMessagesHandler:
     __slots__ = ("__pipes", "__senders", "__observer",)
 
     def __init__(self) -> None:
-        self.__pipes: Dict[str, MesagesPipe] = dict()
+        self.__pipes: dict[str, MesagesPipe] = dict()
         self.__observer = observer.SimpleObserver()
         self.__observer.subscribe(misc.DISABLED, self.__on_pipe_disabled)
 
     def get_pipe(self, name: str) -> "MesagesPipe":
         if name in self.__pipes:
             return self.__pipes[name]
         self.__pipes[name] = pipe = MesagesPipe(
@@ -40,34 +38,34 @@
         return pipe
 
     async def disable_pipe(self, name: str) -> None:
         if name not in self.__pipes:
             return None
         await self.__pipes[name].disable()
 
-    def avaliable_pipes(self) -> Tuple[str, ...]:
+    def avaliable_pipes(self) -> tuple[str, ...]:
         return tuple(self.__pipes.keys())
 
     async def __on_pipe_disabled(self, name: str) -> None:
         del self.__pipes[name]
 
     @contextlib.asynccontextmanager
-    async def __user_stream(self, queue: "asyncio.Queue[Optional[misc.Message]]", *names: str) -> AsyncGenerator[None, None]:
+    async def __user_stream(self, queue: asyncio.Queue[misc.Message | None], *names: str) -> AsyncGenerator[None, None]:
         key = str(uuid.uuid4())
         pipes = (self.__pipes[name] for name in names)
         await asyncio.gather(*[pipe._add_stream(key, queue) for pipe in pipes])
         try:
             yield
         finally:
             await asyncio.gather(*[pipe._free_stream(key) for pipe in pipes])
 
-    async def changes(self, *names: str, _filter: Optional[Set["misc.EMsgType"]] = None) -> AsyncGenerator[misc.Message, None]:
+    async def changes(self, *names: str, _filter: Set["misc.EMsgType"] | None = None) -> AsyncGenerator[misc.Message, None]:
         if not all((self.__pipes.get(name) for name in names)):
             return
-        msg_queue: asyncio.Queue[Optional["misc.Message"]] = asyncio.Queue()
+        msg_queue: asyncio.Queue["misc.Message" | None] = asyncio.Queue()
         async with self.__user_stream(msg_queue, *names):
             async for msg in _get_from_queue(msg_queue):
                 if msg is None:
                     break
                 if _filter and msg.type not in _filter:
                     continue
                 yield msg
```

### Comparing `xoa-core-1.0.8/xoa_core/core/messanger/pipe.py` & `xoa-core-2.0.0/xoa_core/core/messenger/pipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+from __future__ import annotations
 import asyncio
 import contextlib
 from functools import partialmethod
 from typing import (
     Any,
     Final,
-    Dict,
-    Optional,
 )
 
 from xoa_core.core.generic_types import TObserver
 from . import misc
 
 
 class MesagesPipe:
@@ -17,15 +16,15 @@
 
     def __init__(self, name: str, observer: "TObserver") -> None:
         self.name: Final[str] = name
         self.__evt = asyncio.Event()
         self.__queue: "asyncio.Queue[misc.Message]" = asyncio.Queue()
         self.__observer = observer
         self.__lock = asyncio.Lock()
-        self.__push_streams: Dict[str, asyncio.Queue[Optional["misc.Message"]]] = {}
+        self.__push_streams: dict[str, asyncio.Queue["misc.Message" | None]] = {}
         self.__procesor = asyncio.create_task(
             self.__worker(),
             name=f"MessagesPipe[{self.name}]"
         )
 
     async def _add_stream(self, key: str, queue: asyncio.Queue) -> None:
         async with self.__lock:
@@ -54,26 +53,26 @@
         self.__procesor.cancel()
         with contextlib.suppress(asyncio.CancelledError):
             await self.__procesor
         for stm in self.__push_streams.values():
             stm.put_nowait(None)  # Inform to stop watching
         self.__observer.emit(misc.DISABLED, self.name)
 
-    def transmit(self, msg: Any, *, msg_type: misc.EMsgType = misc.EMsgType.DATA) -> None:
+    def transmit(self, msg: Any, *, msg_type: misc.EMsgType = misc.EMsgType.DATA, **meta: Any) -> None:
         """Unblocable function"""
         assert not self.__evt.is_set(), "Message pipe is closed"
         message = misc.Message(
             pipe_name=self.name,
-            destenation=None,
+            meta=meta,
             type=msg_type,
             payload=msg
         )
         self.__queue.put_nowait(message)
 
-    def get_facade(self) -> misc.PipeFacade:
-        return misc.PipeFacade(self.transmit)
+    def get_facade(self, suite_name: str) -> misc.PipeFacade:
+        return misc.PipeFacade(self.transmit, suite_name)
 
     def get_state_facade(self) -> misc.PipeStateFacade:
         return misc.PipeStateFacade(self.transmit)
 
     transmit_warn = partialmethod(transmit, msg_type=misc.EMsgType.WARNING)
     transmit_err = partialmethod(transmit, msg_type=misc.EMsgType.ERROR)
```

### Comparing `xoa-core-1.0.8/xoa_core/core/plugin_abstract.py` & `xoa-core-2.0.0/xoa_core/core/plugin_abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import typing
-from abc import ABC, abstractmethod
+from abc import (
+    ABC,
+    abstractmethod,
+)
 
 if typing.TYPE_CHECKING:
     from enum import Enum
 
     from pydantic import BaseModel
     from xoa_driver import testers as driver_testers
 
@@ -11,28 +14,29 @@
 
 
 TestersType = typing.Dict[str, "driver_testers.GenericAnyTester"]
 DT = typing.TypeVar("DT", bound="BaseModel")
 
 
 class TransmitFunc(typing.Protocol):
-    def __call__(self, msg: typing.Any, *, msg_type: "Enum") -> None:
-        ...
+    def __call__(self, msg: typing.Any, *, msg_type: "Enum", **meta) -> None: ...  # noqa: E704
 
 
 class PPipeFacade(typing.Protocol):
-    def __init__(self, transmit: "TransmitFunc") -> None:
-        ...
+    def __init__(self, transmit: "TransmitFunc", suite_name: str) -> None: ...  # noqa: E704
 
     def send_statistics(self, data: typing.Union[typing.Dict, "BaseModel"]) -> None:
         """Method used for push statistics data into the messages pipe for future distribution"""
-    def send_progress(self, progress: int) -> None:
+
+    def send_progress(self, current: int, total: int) -> None:
         """Method used for push current progress value into the messages pipe for future distribution"""
-    def send_warning(self, worning: Exception) -> None:
+
+    def send_warning(self, warning: Exception) -> None:
         """Method used for push warning exceptions into the messages pipe for future distribution"""
+
     def send_error(self, error: Exception) -> None:
         """Method used for push error exceptions into the messages pipe for future distribution"""
 
 
 class PStateConditionsFacade(typing.Protocol):
     async def wait_if_paused(self) -> None:
         """
@@ -51,27 +55,27 @@
 class PluginAbstract(ABC, typing.Generic[DT]):
     """TestSuitePlugin abstraction class, all test suite must be inherited from it."""
 
     __slots__ = {
         "state_conditions": """Facade contains methods which can help pause or stop Plugin execution.""",
         "xoa_out": """Facade for transmit messages to user.""",
         "testers": """Dictionary of <TESTER_ID>: <TESTER_INSTANCE>""",
-        "port_identities": """PortIdentities a dictionary of <SLOT_ID>: <PortIdentity>""",
+        "port_identities": """PortIdentities a list where positional index is <SLOT_ID> and item is <PortIdentity>""",
         "cfg": """Test-Suite configuration model defined by plugin."""
     }
 
     def __init__(self, state_conditions: "PStateConditionsFacade", xoa_out: "PPipeFacade", testers: TestersType, params: "TestParameters") -> None:
         self.state_conditions = state_conditions
         """Facade contains methods which can help pause or stop Plugin execution."""
         self.xoa_out = xoa_out
         """Facade for transmit messages to user."""
         self.testers = testers
         """Dictionary of <TESTER_ID>: <TESTER_INSTANCE>"""
         self.port_identities = params.port_identities
-        """PortIdentities a dictionary of <SLOT_ID>: <PortIdentity>"""
+        """PortIdentities a list where positional index is <SLOT_ID> and item is <PortIdentity>"""
         self.cfg: DT = typing.cast(DT, params.config)
         """Test configuration model defined by plugin."""
         self.prepare()
 
     def prepare(self) -> None:
         """Optional method used for declare plugins attributes."""
         pass
```

### Comparing `xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/module.py` & `xoa-core-2.0.0/xoa_core/core/resources/resource/models/module.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,98 @@
+from __future__ import annotations
+
 import asyncio
+from dataclasses import dataclass
 from typing import (
-    Tuple,
-    Optional,
+    Any,
     Callable,
-    TypeVar,
     Type,
-    Dict,
-    Any,
+    Tuple,
+    Optional,
+)
+from pydantic import BaseModel
+from typing_extensions import Self
+from xoa_driver import (
+    enums,
+    modules,
 )
-from dataclasses import dataclass
-from xoa_driver import enums
-from xoa_driver import modules
-
-from xoa_core.core.utils import decorators
-from .port import PortModel
-
 
-M = TypeVar("M", bound="ModuleModel")
+from .__decorator import post_notify
+from .types import (
+    ModuleID,
+    TesterID,
+)
+from .port import (
+    PortModel,
+    PortInfoModel,
+)
 
 
 @dataclass
 class ModuleModel:
-    id: int
+    id: ModuleID
+    index: int
     model: str
     reserved_by: str
-    ports: Tuple[PortModel, ...]
+    ports: tuple[PortModel, ...]
+    serial_number: int
     name: str = " - "
     can_media_config: bool = False
     is_chimera: bool = False
     can_local_time_adjust: bool = False
-    max_clock_ppm: Optional[int] = None
+    max_clock_ppm: int | None = None
 
     async def on_evt_reserved_by(self, _, value) -> None:
         self.reserved_by = value.username
 
+    async def on_serial_number_change(self, _, value) -> None:
+        self.serial_number = value.serial_number
+
     @classmethod
-    async def from_module(cls: Type[M], module: "modules.GenericAnyModule", notifier: Callable) -> M:
+    async def from_module(cls: Type[Self], tester_id: TesterID, module: "modules.GenericAnyModule", notifier: Callable) -> Self:
+        module_id = ModuleID(f"{tester_id}-{module.module_id}")
         inst = cls(
-            id=module.module_id,
+            id=module_id,
+            index=module.module_id,
             model=module.info.model,
             reserved_by=module.info.reserved_by,
             **await _prepare_values(module),
+            serial_number=(await module.serial_number.get()).serial_number,
             ports=tuple(
                 await asyncio.gather(*[
-                    PortModel.from_port(port, notifier)
+                    PortModel.from_port(module_id, port, notifier)
                     for port in module.ports
                 ])
             )
         )
-        module.on_reserved_by_change(decorators.post_notify(notifier)(inst.on_evt_reserved_by))
+        module.on_reserved_by_change(post_notify(notifier)(inst.on_evt_reserved_by))
+        module.on_serial_number_change(post_notify(notifier)(inst.on_serial_number_change))
         return inst
 
 
-async def _prepare_values(module: "modules.GenericAnyModule") -> Dict[str, Any]:
+async def _prepare_values(module: "modules.GenericAnyModule") -> dict[str, Any]:
     m_cpb = dict()
     if not isinstance(module, (modules.ModuleL47, modules.ModuleL47VE)):
         cpb = await module.capabilities.get()
         m_cpb["can_media_config"] = cpb.can_media_config is enums.YesNo.YES
         m_cpb["is_chimera"] = cpb.is_chimera is enums.YesNo.YES
         m_cpb["can_local_time_adjust"] = cpb.can_local_time_adjust is enums.YesNo.YES
         m_cpb["max_clock_ppm"] = cpb.max_clock_ppm
 
     if m_name := getattr(module, "name", None):
         mn = await m_name.get()
         m_cpb["name"] = mn.name
     return m_cpb
+
+
+class ModuleInfoModel(BaseModel):
+    id: ModuleID
+    index: int
+    model: str
+    reserved_by: str
+    ports: Tuple[PortInfoModel, ...]
+    name: str
+    can_media_config: bool
+    is_chimera: bool
+    can_local_time_adjust: bool
+    max_clock_ppm: Optional[int]
+    serial_number: int
```

### Comparing `xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/port.py` & `xoa-core-2.0.0/xoa_core/core/resources/resource/models/port.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,93 @@
+from __future__ import annotations
+
+from dataclasses import (
+    dataclass,
+    field,
+)
 from typing import (
-    Tuple,
-    Optional,
+    Any,
     Callable,
-    TypeVar,
+    Optional,
+    Tuple,
     Type,
-    Dict,
-    Any,
 )
-from dataclasses import (
-    dataclass,
-    field,
+from pydantic import BaseModel
+from typing_extensions import Self
+from xoa_driver import (
+    enums,
+    ports,
+    utils,
 )
-from xoa_driver import ports
-from xoa_driver import enums
-from xoa_driver import utils
-
-from xoa_core.core.utils import decorators
-
-P = TypeVar("P", bound="PortModel")
+from .types import ModuleID, PortID
+from .__decorator import post_notify
 
 
 @dataclass
 class PortModel:
-    id: int
+    id: PortID
+    index: int
     model: str
     reserved_by: str
-    sync_status: Optional[bool] = None
-    traffic_state: Optional[enums.TrafficOnOff] = None
-    max_speed: Optional[int] = None
-    max_speed_reduction: Optional[int] = None
-    min_interframe_gap: Optional[int] = None
-    max_interframe_gap: Optional[int] = None
-    max_streams_per_port: Optional[int] = None
-    packet_limit: Optional[int] = None
-    min_packet_length: Optional[int] = None
-    max_packet_length: Optional[int] = None
-    max_header_length: Optional[int] = None
-    max_protocol_segments: Optional[int] = None
-    max_repeat: Optional[int] = None
+    sync_status: bool | None = None
+    traffic_state: enums.TrafficOnOff | None = None
+    max_speed: int | None = None
+    max_speed_reduction: int | None = None
+    min_interframe_gap: int | None = None
+    max_interframe_gap: int | None = None
+    max_streams_per_port: int | None = None
+    packet_limit: int | None = None
+    min_packet_length: int | None = None
+    max_packet_length: int | None = None
+    max_header_length: int | None = None
+    max_protocol_segments: int | None = None
+    max_repeat: int | None = None
     can_set_autoneg: bool = False
     can_tcp_checksum: bool = False
     can_udp_checksum: bool = False
     can_micro_tpld: bool = False
     can_mdi_mdix: bool = False
     can_sync_traffic_start: bool = False
     can_fec: bool = False
     can_anlt: bool = False
     is_chimera: bool = False
     can_brr: bool = False
-    speed_modes_supported: Tuple["enums.PortSpeedMode", ...] = field(default_factory=tuple)
-    speed_mode_current: Optional[enums.PortSpeedMode] = None
-    speed_current: Optional[int] = None
-    speed_reduction: Optional[int] = None
+    speed_modes_supported: tuple["enums.PortSpeedMode", ...] = field(default_factory=tuple)
+    speed_mode_current: enums.PortSpeedMode | None = None
+    speed_current: int | None = None
+    speed_reduction: int | None = None
 
     async def on_evt_traffic_state(self, _, value) -> None:
         self.traffic_state = enums.TrafficOnOff(value.on_off)
 
     async def on_evt_sync_status(self, _, value) -> None:
         self.sync_status = enums.SyncStatus(value.sync_status) is enums.SyncStatus.IN_SYNC
 
     async def on_evt_reserved_by(self, _, value) -> None:
         self.reserved_by = value.username
 
     @classmethod
-    async def from_port(cls: Type[P], port: "ports.GenericAnyPort", notifier: Callable) -> P:
+    async def from_port(cls: Type[Self], module_id: ModuleID, port: "ports.GenericAnyPort", notifier: Callable) -> Self:
         inst = cls(
-            id=port.kind.port_id,
+            id=PortID(f"{module_id}-{port.kind.port_id}"),
+            index=port.kind.port_id,
             model=port.info.interface,
             reserved_by=port.info.reserved_by,
             sync_status=getattr(port.info, "sync_status", None),
             traffic_state=getattr(port.info, "traffic_state", None),
             **await _prepare_values(port),
         )
-        port.on_reserved_by_change(decorators.post_notify(notifier)(inst.on_evt_reserved_by))
+        port.on_reserved_by_change(post_notify(notifier)(inst.on_evt_reserved_by))
         if on_traffic_change := getattr(port, 'on_traffic_change', None):
-            on_traffic_change(decorators.post_notify(notifier)(inst.on_evt_traffic_state))
-        port.on_receive_sync_change(decorators.post_notify(notifier)(inst.on_evt_sync_status))
+            on_traffic_change(post_notify(notifier)(inst.on_evt_traffic_state))
+        port.on_receive_sync_change(post_notify(notifier)(inst.on_evt_sync_status))
         return inst
 
 
-async def _prepare_values(port: "ports.GenericAnyPort") -> Dict[str, Any]:
+async def _prepare_values(port: "ports.GenericAnyPort") -> dict[str, Any]:
     p_vals = dict()
     if not isinstance(port, (ports.PortL47, ports.PortL23VE)):
         if not isinstance(port, ports.PortChimera):
             ms, cur, red, tx_pl = await utils.apply(
                 port.speed.mode.selection.get(),
                 port.speed.current.get(),
                 port.speed.reduction.get(),
@@ -109,11 +113,45 @@
         p_vals["can_set_autoneg"] = bool(cpb.can_set_autoneg)
         p_vals["can_tcp_checksum"] = bool(cpb.can_tcp_checksum)
         p_vals["can_udp_checksum"] = bool(cpb.can_udp_checksum)
         p_vals["can_micro_tpld"] = bool(cpb.can_micro_tpld)
         p_vals["can_mdi_mdix"] = bool(cpb.can_mdi_mdix)
         p_vals["can_sync_traffic_start"] = bool(cpb.can_sync_traffic_start)
         p_vals["can_fec"] = bool(cpb.can_fec)
-        p_vals["can_anlt"] = cpb.can_set_link_train and cpb.can_auto_neg_base_r
+        p_vals["can_anlt"] = bool(cpb.can_set_link_train and cpb.can_auto_neg_base_r)
         p_vals["is_chimera"] = bool(cpb.is_chimera)
         p_vals["can_brr"] = getattr(port, "is_brr_mode_supported", False)
     return p_vals
+
+
+class PortInfoModel(BaseModel):
+    id: PortID
+    index: int
+    model: str
+    reserved_by: str
+    sync_status: Optional[bool]
+    traffic_state: Optional[enums.TrafficOnOff]
+    max_speed: Optional[int]
+    max_speed_reduction: Optional[int]
+    min_interframe_gap: Optional[int]
+    max_interframe_gap: Optional[int]
+    max_streams_per_port: Optional[int]
+    packet_limit: Optional[int]
+    min_packet_length: Optional[int]
+    max_packet_length: Optional[int]
+    max_header_length: Optional[int]
+    max_protocol_segments: Optional[int]
+    max_repeat: Optional[int]
+    can_set_autoneg: bool
+    can_tcp_checksum: bool
+    can_udp_checksum: bool
+    can_micro_tpld: bool
+    can_mdi_mdix: bool
+    can_sync_traffic_start: bool
+    can_fec: bool
+    can_anlt: bool
+    is_chimera: bool
+    can_brr: bool
+    speed_modes_supported: Tuple["enums.PortSpeedMode", ...]
+    speed_mode_current: Optional[enums.PortSpeedMode]
+    speed_current: Optional[int]
+    speed_reduction: Optional[int]
```

### Comparing `xoa-core-1.0.8/xoa_core/core/resources/datasets/internal/tester.py` & `xoa-core-2.0.0/xoa_core/core/resources/resource/models/tester.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,97 @@
+from __future__ import annotations
+
 import asyncio
+from dataclasses import (
+    dataclass,
+    field,
+)
 from typing import (
     TYPE_CHECKING,
-    Tuple,
     Callable,
-    TypeVar,
-    Type,
+    Tuple,
+)
+
+from pydantic import (
+    BaseModel,
+    SecretStr,
 )
-from pydantic import SecretStr
-from dataclasses import dataclass, field
 if TYPE_CHECKING:
     from xoa_driver import testers
+
 from xoa_driver import utils
-from xoa_core.core.utils import decorators
-from xoa_core.core.resources.datasets import enums
-from .module import ModuleModel
 
-T = TypeVar("T", bound="TesterModel")
+from .__decorator import post_notify
+from .module import (
+    ModuleModel,
+    ModuleInfoModel,
+)
+from .types import (
+    EProductType,
+    TesterID,
+)
 
 
 @dataclass
 class TesterModel:
-    product: enums.EProductType
+    id: TesterID
+    product: EProductType
     host: str
     port: int
     password: SecretStr
     name: str = " - "
     reserved_by: str = ""
     is_connected: bool = False
-    modules: Tuple[ModuleModel, ...] = field(default_factory=tuple)
-    id: str = None  # type: ignore
+    modules: tuple[ModuleModel, ...] = field(default_factory=tuple)
     keep_disconnected: bool = False
     max_name_len: int = 0
     max_comment_len: int = 0
     max_password_len: int = 0
+    serial_number: int = 0
 
     async def on_evt_reserved_by(self, _, value) -> None:
         self.reserved_by = value.username
 
     async def on_evt_disconnected(self, *_) -> None:
         self.is_connected = False
         self.modules = tuple()
 
-    @classmethod
-    async def from_tester(cls: Type[T], resource_id: str, product: "enums.EProductType", tester: "testers.GenericAnyTester", notifier: Callable) -> T:
+    async def sync(self, tester: "testers.GenericAnyTester", notifier: Callable) -> None:
         tn, cpb = await utils.apply(
             tester.name.get(),
             tester.capabilities.get()
         )
-        inst = cls(
-            id=resource_id,
-            product=product,
-            host=tester.info.host,
-            port=tester.info.port,
-            password=SecretStr(tester.session.pwd),
-            name=str(tn.chassis_name),
-            reserved_by=tester.info.reserved_by,
-            is_connected=tester.session.is_online,
-            keep_disconnected=False,
-            max_name_len=cpb.max_name_len,
-            max_comment_len=cpb.max_name_len,
-            max_password_len=cpb.max_name_len,
-            modules=tuple(
-                await asyncio.gather(*[
-                    ModuleModel.from_module(module, notifier)
-                    for module in tester.modules
-                ])
-            )
+
+        self.name = str(tn.chassis_name)
+        self.reserved_by = tester.info.reserved_by
+        self.is_connected = tester.session.is_online
+        self.keep_disconnected = False
+        self.max_name_len = cpb.max_name_len
+        self.max_comment_len = cpb.max_name_len
+        self.max_password_len = cpb.max_name_len
+        self.serial_number = tester.info.serial_number
+        self.modules = tuple(
+            await asyncio.gather(*[
+                ModuleModel.from_module(self.id, module, notifier)
+                for module in tester.modules
+            ])
         )
-        tester.on_reserved_by_change(decorators.post_notify(notifier)(inst.on_evt_reserved_by))
-        tester.on_disconnected(decorators.post_notify(notifier)(inst.on_evt_disconnected))
-        return inst
+
+        tester.on_reserved_by_change(post_notify(notifier)(self.on_evt_reserved_by))
+        tester.on_disconnected(self.on_evt_disconnected)
+
+
+class TesterInfoModel(BaseModel):
+    id: TesterID
+    product: EProductType
+    host: str
+    port: int
+    password: SecretStr
+    name: str
+    reserved_by: str
+    is_connected: bool
+    modules: Tuple[ModuleInfoModel, ...] = tuple()
+    keep_disconnected: bool
+    max_name_len: int
+    max_comment_len: int
+    max_password_len: int
+    serial_number: int
```

### Comparing `xoa-core-1.0.8/xoa_core/core/resources/manager.py` & `xoa-core-2.0.0/xoa_core/core/resources/resource/facade.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,155 @@
+from __future__ import annotations
+
 import asyncio
+from dataclasses import asdict
+
+from functools import lru_cache
 from typing import (
-    TYPE_CHECKING,
-    Iterable,
-    Generator,
-    TypeVar,
-    Union,
-    Dict,
     Any,
+    Callable,
+    Coroutine,
 )
-if TYPE_CHECKING:
-    from xoa_driver import testers
-    from xoa_core.core.generic_types import TMesagesPipe
-from .datasets.external.tester import TesterExternalModel
-
-
-from xoa_core.core.utils import observer
+from xoa_driver.testers import GenericAnyTester
+from xoa_core.core.utils.observer import SimpleObserver
 
-from .resources_pool import ResourcesPool
+from . import const
+from . import (
+    exceptions,
+    misc,
+)
+from .models.tester import TesterModel, TesterInfoModel
+from .models.types import (
+    TesterID,
+    StorageResource,
+)
 
-from . import storage
 
-from .datasets import enums
-from .datasets.external import credentials
-from .datasets.internal.credentials import CredentialsModel
+EventCallback = Callable[[TesterInfoModel, str], Coroutine[None, None, None]]
 
 
-from . import misc
-from .exceptions import (
-    InvalidTesterTypeError,
-    TesterCommunicationError,
-    ResourceNotAvaliableError
-)
+class Events:
+    __slots__ = ("__observer",)
 
-AllTesterTypes = Union["CredentialsModel", "TesterExternalModel"]
+    def __init__(self, observer: SimpleObserver) -> None:
+        self.__observer = observer
 
-RM = TypeVar("RM", bound="ResourcesManager")
+    def reset(self) -> None:
+        self.__observer.reset()
 
+    def on_connected(self, func: EventCallback) -> None:
+        self.__observer.subscribe(const.CONNECTED, func)
 
-class ResourcesManager:
-    __slots__ = ("_msg_pipe", "__precision_storage", "__observer", "_pool", )
+    def on_disconnected(self, func: EventCallback) -> None:
+        self.__observer.subscribe(const.DISCONNECTED, func)
 
-    def __init__(self, msg_pipe: "TMesagesPipe", data_storage_path: str) -> None:
-        self._msg_pipe = msg_pipe
-        self.__precision_storage = storage.PrecisionStorage(data_storage_path)
-        self.__observer = observer.SimpleObserver()
-        self._pool = ResourcesPool(self.__observer)
+    def on_changed(self, func: EventCallback) -> None:
+        self.__observer.subscribe(const.CHANGED, func)
 
-        self.__observer.subscribe(enums.EResourcesEvents.ADDED, self.__tester_added)
-        self.__observer.subscribe(enums.EResourcesEvents.EXCLUDED, self.__tester_excluded)
-        self.__observer.subscribe(enums.EResourcesEvents.INFO_CHANGE_TESTER, self.__tester_info_change)
 
-    def __await__(self: RM) -> Generator[Any, None, RM]:
-        return self.__setup().__await__()
+class Resource:
+    __slots__ = ("tester", "dataset", "__observer")
 
-    async def __setup(self: RM) -> RM:
-        known_testers = await self.__precision_storage.get_all()
-        tasks = tuple(
-            self._pool.add(tester)
-            for tester in known_testers.values()
-            if not tester.keep_disconnected
+    def __init__(self, credentials: misc.Credentials, *, name: str | None = None, keep_disconnected: bool | None = None) -> None:
+        self.__observer: SimpleObserver[str] = SimpleObserver(pass_event=True)
+        self.dataset = TesterModel(
+            id=misc.make_resource_id(credentials.host, credentials.port),
+            product=credentials.product,
+            host=credentials.host,
+            port=credentials.port,
+            password=credentials.password,
+            name=name or " - "
         )
-        exceptions = filter(
-            None,
-            await asyncio.gather(*tasks, return_exceptions=True)
-        )
-        for err in exceptions:
-            await self.__precision_storage.keep_disconnected(err.props.id)
-            self._msg_pipe.transmit_err(err)
-        return self
-
-    async def add_tester(self, params: "credentials.Credentials") -> bool:
-        if not await self.__precision_storage.is_registered(params.id):
-            credentials = CredentialsModel.from_external(params)
-            try:
-                await self._pool.add(credentials)
-            except (InvalidTesterTypeError, TesterCommunicationError) as err:
-                self._msg_pipe.transmit_err(err)
-            else:
-                self.__precision_storage.remember(credentials)
-                return True
-        return False
-
-    async def remove_tester(self, id: str):
-        self.__precision_storage.forget(id)
-        await self._pool.suspend(id)
-
-    async def update_tester(self):
-        """ User Apply Changes """
-        pass
-
-    async def get_all_testers(self) -> Dict[str, "AllTesterTypes"]:
-        known_testers = await self.__precision_storage.get_all()
-        all_credentials = {tid: TesterExternalModel.parse_obj(credentials) for tid, credentials in known_testers.items()}
-        return {**all_credentials, **self._pool.avaliable_resources}
-
-    async def connect(self, id: str) -> None:
-        if id in self._pool.res_identifiers:
+        if keep_disconnected is not None:
+            self.dataset.keep_disconnected = keep_disconnected
+        self.tester = self.__get_tester_inst()
+
+    def __get_tester_inst(self) -> GenericAnyTester:
+        if tester_ := misc.get_tester_inst(self.credentials):
+            return tester_
+        raise exceptions.InvalidTesterTypeError(self.credentials)
+
+    async def __on_tester_loose_connection(self, _) -> None:
+        self.__observer.emit(const.DISCONNECTED, self.info())
+        if self.keep_disconnected:
             return None
-        if obj := await self.__precision_storage.get(id):
+        self.tester = self.__get_tester_inst()
+        for retry in range(5):
+            await asyncio.sleep(delay=retry * 2)
             try:
-                await self._pool.add(obj)
-            except (InvalidTesterTypeError, TesterCommunicationError) as err:
-                self._msg_pipe.transmit_err(err)
+                await self.connect()
+            except Exception:
+                continue
             else:
-                await self.__precision_storage.keep_connected(id)
-
-    async def disconnect(self, id: str) -> None:
-        await self.__precision_storage.keep_disconnected(id)
-        await self._pool.suspend(id)
-
-    def get_testers_by_id(self, testers_ids: Iterable[str], username: str, debug=False) -> Dict[str, "testers.GenericAnyTester"]:
-        testers = {}
-        for tester_id in testers_ids:
-            resource = self._pool.use_resource(tester_id)
-            if resource is None:
-                raise ResourceNotAvaliableError(tester_id)
-            tester = misc.get_tester_inst(resource.credentials, username, debug)
-            if tester is None:
-                raise InvalidTesterTypeError(resource.credentials)
-            testers[tester_id] = tester
-        return testers
-
-    async def __tester_added(self, data: "TesterExternalModel") -> None:
-        self._msg_pipe.transmit(data)
-
-    async def __tester_excluded(self, id: str) -> None:
-        if obj := await self.__precision_storage.get(id):
-            self._msg_pipe.transmit(TesterExternalModel.parse_obj(obj))
-            if obj.keep_disconnected:
                 return None
-            await self.connect(id)
+        self.dataset.keep_disconnected = True
+
+    def __on_data_changed(self) -> None:
+        self.__observer.emit(const.CHANGED, self.info())
 
-    async def __tester_info_change(self, data: "TesterExternalModel") -> None:
-        self._msg_pipe.transmit(data)
+    @property
+    def is_connected(self) -> bool:
+        return self.tester is not None and self.tester.session.is_online
+
+    async def connect(self) -> None:
+        if self.tester.session.is_online:
+            raise exceptions.IsConnectedError(self.id)
+        self.dataset.keep_disconnected = False
+        try:
+            await self.tester
+        except Exception as e:
+            raise exceptions.TesterCommunicationError(self.credentials, e) from None
+        else:
+            # IMPORTANT: To keep order of next functions call
+            # 1 - sync which can emit CHANGED event
+            # 2 - Emit CONNECTED
+            # 3 - Subscribe on tester disconnected
+            await self.dataset.sync(self.tester, self.__on_data_changed)
+            self.__observer.emit(const.CONNECTED, self.info())
+            self.tester.on_disconnected(self.__on_tester_loose_connection)
+
+    async def disconnect(self) -> None:
+        if not self.tester.session.is_online:
+            raise exceptions.IsDisconnectedError(self.id)
+        self.dataset.keep_disconnected = True
+        await self.tester.session.logoff()
+        self.tester = self.__get_tester_inst()
+
+    async def configure(self, config: dict[str, Any]) -> None:
+        raise NotImplementedError()
+
+    def prepare_session(self, username: str, debug: bool = False) -> GenericAnyTester:
+        if tester_ := misc.get_tester_inst(self.credentials, username=username, debug=debug):
+            return tester_
+        raise exceptions.InvalidTesterTypeError(self.credentials)
+
+    @property
+    def id(self) -> TesterID:
+        return self.dataset.id
+
+    @property
+    def keep_disconnected(self) -> bool:
+        return self.dataset.keep_disconnected
+
+    @property
+    def store_data(self) -> StorageResource:
+        return {
+            "id": self.dataset.id,
+            "product": self.dataset.product,
+            "host": self.dataset.host,
+            "port": self.dataset.port,
+            "password": self.dataset.password,
+            "name": self.dataset.name,
+            "keep_disconnected": self.dataset.keep_disconnected
+        }
+
+    @property
+    @lru_cache
+    def credentials(self) -> misc.Credentials:
+        return misc.Credentials.parse_obj(self.store_data)
+
+    def info(self) -> TesterInfoModel:
+        return TesterInfoModel.parse_obj(asdict(self.dataset))
+
+    @property
+    def events(self) -> Events:
+        return Events(self.__observer)
```

### Comparing `xoa-core-1.0.8/xoa_core/core/test_suites/_loader.py` & `xoa-core-2.0.0/xoa_core/core/test_suites/_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,53 @@
+from __future__ import annotations
 import os
+from pathlib import Path
 import sys
 import oyaml as yaml
 import importlib.util
 from typing import (
     TYPE_CHECKING,
-    Optional, 
+    Optional,
     Type,
     Generator,
 )
 
 from pydantic import BaseModel
 from xoa_core.core.exceptions import InvalidPluginError
 if TYPE_CHECKING:
     from types import ModuleType
 
 from .datasets import (
-    PluginMeta, 
+    PluginMeta,
     PluginData,
     build_test_params
 )
 
 from ..plugin_abstract import PluginAbstract
 
 
 META_FILE_NAME = 'meta.yml'
 
+
 def __load_module(path: str) -> Generator["ModuleType", None, None]:
     """Load module from path to the var"""
     for child in os.listdir(path):
         ilename, _ = os.path.splitext(child)
         module_name = f"{os.path.split(path)[-1]}.{ilename}"
         spec = importlib.util.spec_from_file_location(
             module_name,
             os.path.join(path, child),
         )
-        if not spec or not spec.loader: 
+        if not spec or not spec.loader:
             continue
         mod = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(mod)
         yield mod
 
+
 def __make_plugin(module_path: str, meta: PluginMeta) -> Optional["PluginData"]:
     """Create plugin model."""
     entry_class: Optional[Type["PluginAbstract"]] = None
     model_class: Optional[Type["BaseModel"]] = None
     for module in __load_module(module_path):
         if entry_class is None:
             entry_class = getattr(module, meta.entry_object, None)
@@ -52,28 +56,35 @@
     if not (entry_class and model_class):
         return None
     if not issubclass(entry_class, PluginAbstract):
         raise InvalidPluginError(entry_class, PluginAbstract)
     if not issubclass(model_class, BaseModel):
         raise InvalidPluginError(model_class, BaseModel)
     return PluginData(
-        meta=meta, 
-        entry_class=entry_class, 
+        meta=meta,
+        entry_class=entry_class,
         model_class=build_test_params(model_class)
     )
 
 
 def __read_meta(path: str) -> "PluginMeta":
     """Read metafile"""
     with open(path, "r") as outfile:
         data = yaml.load(outfile, Loader=yaml.SafeLoader)
         return PluginMeta(**data)
 
-def load_plugin(path: str) -> Generator[PluginData, None, None]:
-    sys.path.append(path)
+def __register_path(path: str | Path) -> None:
+    str_path = str(path)
+    if str_path in sys.path:
+        return None
+    sys.path.append(str_path)
+
+
+def load_plugin(path: str | Path) -> Generator[PluginData, None, None]:
+    __register_path(path)
     for child in os.listdir(path):
         child_path = os.path.abspath(os.path.join(path, child))
         if not os.path.isdir(child_path):
             continue
         meta_path = os.path.join(child_path, META_FILE_NAME)
         if not os.path.exists(meta_path):
             continue
```

### Comparing `xoa-core-1.0.8/xoa_core/core/test_suites/controler.py` & `xoa-core-2.0.0/xoa_core/core/test_suites/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+from __future__ import annotations
 import os
+from pathlib import Path
 from typing import (
     Generator,
     Optional,
     Dict,
     Tuple,
     List,
 )
 
 from xoa_core.core import exceptions
-from . import datasets #import PluginData, Plugin
+from . import datasets
 from . import _loader as loader
 
 
 class PluginController:
     __slots__ = ("__paths", "__test_suites")
 
     def __init__(self) -> None:
-        self.__paths: Tuple[str, ...] = tuple()
+        self.__paths: Tuple[str | Path, ...] = tuple()
         self.__test_suites: Dict[str, "datasets.PluginData"] = dict()
 
-    def register_path(self, path: str) -> None:
+    def register_path(self, path: str | Path) -> None:
         """Register custom path of plugins"""
-        self.__paths += (
-            os.path.abspath(path)
-            if not os.path.isabs(path)
-            else path,
-        )
+        if not os.path.isabs(path):
+            path = os.path.abspath(path)
+        if path in self.__paths:
+            return None
+        self.__paths += (path,)
         self.__init_plugins()
 
     def available_test_suites(self) -> List[str]:
         return list(self.__test_suites.keys())
 
     def suite_info(self, name: str) -> Optional[Dict]:
         suite = self.__test_suites.get(name, None)
@@ -44,15 +46,15 @@
         plugin_data = self.__test_suites.get(name, None)
         if plugin_data is None:
             raise exceptions.TestSuiteNotExistError(name)
         elif not plugin_data.meta.is_supported:
             raise exceptions.TestSuiteVersionError(name, plugin_data.meta.core_version)
         return plugin_data
 
-    def get_plugin(self, name: str, debug: bool=False) -> "datasets.Plugin":
+    def get_plugin(self, name: str, debug: bool = False) -> "datasets.Plugin":
         plugin_data = self.get_plugin_data(name)
         return datasets.Plugin(plugin_data, debug)
 
     def __read_plugins(self) -> Generator["datasets.PluginData", None, None]:
         """Read plugins from provided paths."""
         for path in self.__paths:
             yield from loader.load_plugin(path)
@@ -60,8 +62,7 @@
     def __init_plugins(self) -> None:
         """Read plugins in to the local storage"""
         self.__test_suites.clear()
         self.__test_suites = dict(
             (plugin.meta.name, plugin)
             for plugin in self.__read_plugins()
         )
-
```

### Comparing `xoa-core-1.0.8/xoa_core/core/test_suites/datasets.py` & `xoa-core-2.0.0/xoa_core/core/test_suites/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from operator import attrgetter
 from typing import (
     TYPE_CHECKING,
     Optional,
     Type,
     List,
     Dict,
@@ -13,36 +14,38 @@
 import semver
 
 if TYPE_CHECKING:
     from ..plugin_abstract import PluginAbstract, PStateConditionsFacade, PPipeFacade
 
 from xoa_core import __version__
 
+
 class PortIdentity(BaseModel):
     tester_id: str
-    tester_index: int
     module_index: int
     port_index: int
-    
+
     @property
     def name(self) -> str:
-        return f"P-{self.tester_index}-{self.module_index}-{self.port_index}"
+        return f"P-{self.tester_id}-{self.module_index}-{self.port_index}"
 
 
 class TestParameters(BaseModel):
     username: str
-    port_identities: Dict[str, PortIdentity]
+    port_identities: List[PortIdentity]
     config: BaseModel
-    
+
     @property
     def get_testers_ids(self) -> Set[str]:
-        return set(map(
-            attrgetter("tester_id"), 
-            self.port_identities.values()
-        ))
+        return set(
+            map(
+                attrgetter("tester_id"),
+                self.port_identities
+            )
+        )
 
 
 class PluginMeta(BaseModel):
     name: str
     version: str
     core_version: str
     author: Optional[List[str]] = None
@@ -52,41 +55,46 @@
     @property
     def is_supported(self) -> bool:
         return semver.match(__version__, self.core_version)
 
 
 class PluginData(NamedTuple):
     """
-    A test suit container. 
+    A test suit container.
     Contain references to starting points and metadata of the plugin
     """
+
     meta: PluginMeta
     entry_class: Type["PluginAbstract"]
     model_class: Type["TestParameters"]
 
 
 class Plugin:
     def __init__(self, plugin_data: PluginData, debug: bool = False) -> None:
         self.plugin_data = plugin_data
         self.debug = debug
 
     def parse_config(self, config: Dict[str, Any]) -> None:
-        self.params = self.plugin_data.model_class.parse_obj(config) # can raise ValidationError
+        self.params = self.plugin_data.model_class.parse_obj(config)  # can raise ValidationError
 
     def assign_testers(self, tester_getter) -> None:
-        self.testers = tester_getter(self.params.get_testers_ids, self.params.username, self.debug)
+        self.testers = tester_getter(
+            self.params.get_testers_ids,
+            self.params.username,
+            self.debug
+        )
 
-    def create_test_suite(self, state_conditions: "PStateConditionsFacade",  xoa_out: "PPipeFacade") -> "PluginAbstract":
+    def create_test_suite(self, state_conditions: "PStateConditionsFacade", xoa_out: "PPipeFacade") -> "PluginAbstract":
         return self.plugin_data.entry_class(
-            state_conditions=state_conditions, 
-            xoa_out=xoa_out, 
-            testers=self.testers, 
-            params=self.params
+            state_conditions=state_conditions,
+            xoa_out=xoa_out,
+            testers=self.testers,
+            params=self.params,
         )
 
 
 def build_test_params(_test_config: Type["BaseModel"]) -> Type["TestParameters"]:
     class TP(TestParameters):
         config: _test_config
 
     TP.update_forward_refs(_test_config=_test_config)
-    return TP
+    return TP
```

### Comparing `xoa-core-1.0.8/xoa_core/core/utils/observer.py` & `xoa-core-2.0.0/xoa_core/core/utils/observer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import asyncio
 import collections
+from contextlib import suppress
 from typing import (
     Dict,
+    Generic,
     List,
     Callable,
     Any,
     Coroutine,
+    TypeVar,
 )
+import warnings
 CB = Callable[..., Coroutine[Any, None, None]]
+T = TypeVar("T")
 
 
-class SimpleObserver:
-    __slots__ = ("__events", "__loop",)
+class SimpleObserver(Generic[T]):
+    __slots__ = ("__events", "__pass_event")
 
-    def __init__(self) -> None:
-        self.__events: Dict[int, List[CB]] = collections.defaultdict(list)
-        self.__loop = asyncio.get_event_loop()
+    def __init__(self, *, pass_event: bool = False) -> None:
+        self.__pass_event = pass_event
+        self.reset()
 
     def __handle_exceptions(self, task: "asyncio.Task") -> None:
-        if e := task.exception():
-            print(e)
+        with suppress(asyncio.CancelledError):
+            if e := task.exception():
+                warnings.warn(str(e))
 
-    def subscribe(self, evt: int, func: CB) -> None:
+    def reset(self) -> None:
+        self.__events: Dict[T, List[CB]] = collections.defaultdict(list)
+
+    def subscribe(self, evt: T, func: CB) -> None:
         self.__events[evt].append(func)
 
-    def emit(self, evt: int, *args, **kwargs) -> None:
+    def emit(self, evt: T, *args, **kwargs) -> None:
+        kwargs_ = {**kwargs, "event": evt} if self.__pass_event else kwargs
         for action in self.__events[evt]:
-            task = self.__loop.create_task(action(*args, **kwargs))
+            task = asyncio.create_task(action(*args, **kwargs_))
             task.add_done_callback(self.__handle_exceptions)
```

### Comparing `xoa-core-1.0.8/xoa_core/core/utils/validators.py` & `xoa-core-2.0.0/xoa_core/core/utils/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from xoa_driver import ports
 
 
 def is_tester(inst) -> bool:
     cmp_types = (
         testers.L23Tester,
         testers.L47Tester,
-        testers.L47VeTester,
+        testers.L47VeTester
     )
     return isinstance(inst, cmp_types)
 
 
 def is_module(inst) -> bool:
     cmp_types = (
         modules.ModuleL23,
```

### Comparing `xoa-core-1.0.8/xoa_core.egg-info/PKG-INFO` & `xoa-core-2.0.0/xoa_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 Metadata-Version: 2.1
 Name: xoa-core
-Version: 1.0.8
+Version: 2.0.0
 Summary: Xena Open Automation framework for Xena test suite execution, integration, and development.
 Home-page: https://github.com/xenanetworks/open-automation-core
-Author: Artem Constantinov, Frank Chen
-Author-email: aco@xenanetworks.com, fch@xenanewtorks.com
+Author: Artem Constantinov, Leonard Yu
+Author-email: aco@xenanetworks.com, hyu@xenanewtorks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-core) [![PyPI](https://img.shields.io/pypi/v/xoa-core)](https://pypi.python.org/pypi/xoa-core) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-core) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-core/badge/?version=latest)](https://xena-openautomation-core.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-core) [![PyPI](https://img.shields.io/pypi/v/xoa-core)](https://pypi.python.org/pypi/xoa-core) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-core) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-core/badge/?version=stable)](https://xena-openautomation-core.readthedocs.io/en/stable/?badge=stable)
 
 # Xena OpenAutomation Core
-Xena OpenAutomation (XOA) Core is the framework that provides a standardized way for developers and test specialists to execute, develop, and integrate test suites, as well as managing Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
+Xena OpenAutomation Core (XOA Core) is an open-source test suite framework for network automation and testing. It is designed to host various [XOA Test Suites](https://github.com/xenanetworks/open-automation-test-suites) as plugins, allowing users to create, manage, and run test cases for different network scenarios. The XOA Core framework serves as the foundation for building and executing test suites in the XOA ecosystem.
+
+Key features of XOA Core include:
+
+1. Modular architecture: The test suite framework employs a modular architecture, enabling users to develop and run different test suites as plugins.
 
-We open the source code of XOA Core to the public to empower our users with the freedom to tailor the code to their unique needs, develop and integrate their own test suites, so that XOA Core not only works with Xena-developed test suites.
+2. Test Suite execution: XOA Core supports both local and remote test suite execution. Users can execute test suites on their local machines or on remote testbeds through the XOA CLI or Web GUI.
 
-All of Xena-developed test suites are in this repository: [XOA Test Suites](https://github.com/xenanetworks/open-automation-test-suites).
+3. Test Case management: XOA Core provides tools for managing test cases, including creating, updating, and deleting them. Users can also organize test cases using tags and execute them in parallel or sequentially.
 
-XOA Core uses [XOA Python API](https://github.com/xenanetworks/open-automation-python-api) as the driver to administer Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
+4. Extensibility: The framework is designed to be extensible, allowing users to develop custom test suites and plugins to address specific testing requirements.
+
+5. Logging and reporting: XOA Core offers built-in logging and reporting functionality, generating detailed test reports to help users analyze test results and identify issues.
+Xena OpenAutomation (XOA) Core is the framework that provides a standardized way for developers and test specialists to execute, develop, and integrate test suites, as well as managing Xena's physical and virtual Traffic Generation and Analysis (TGA) testers.
 
 ## Documentation
 The user documentation is hosted:
-[Xena OpenAutomation Core Documentation](https://docs.xoa-core.xenanetworks.com/)
+[Xena OpenAutomation Core Documentation](https://docs.xenanetworks.com/projects/xoa-core)
 
 ## Installation
 
 ### Install Using `pip`
 Make sure Python `pip` is installed on you system. If you are using virtualenv, then pip is already installed into environments created by virtualenv, and using sudo is not needed. If you do not have pip installed, download this file: https://bootstrap.pypa.io/get-pip.py and run `python get-pip.py`.
 
 To install the latest, use pip to install from pypi:
```

### Comparing `xoa-core-1.0.8/xoa_core.egg-info/SOURCES.txt` & `xoa-core-2.0.0/xoa_core.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -17,41 +17,38 @@
 xoa_core/core/exceptions.py
 xoa_core/core/generic_types.py
 xoa_core/core/plugin_abstract.py
 xoa_core/core/executors/__init__.py
 xoa_core/core/executors/_events.py
 xoa_core/core/executors/exceptions.py
 xoa_core/core/executors/executor.py
+xoa_core/core/executors/executor_info.py
 xoa_core/core/executors/executor_state.py
 xoa_core/core/executors/executor_state_conditions.py
 xoa_core/core/executors/manager.py
-xoa_core/core/messanger/__init__.py
-xoa_core/core/messanger/handler.py
-xoa_core/core/messanger/misc.py
-xoa_core/core/messanger/pipe.py
+xoa_core/core/messenger/__init__.py
+xoa_core/core/messenger/handler.py
+xoa_core/core/messenger/misc.py
+xoa_core/core/messenger/pipe.py
 xoa_core/core/resources/__init__.py
-xoa_core/core/resources/exceptions.py
-xoa_core/core/resources/manager.py
-xoa_core/core/resources/misc.py
-xoa_core/core/resources/resource.py
-xoa_core/core/resources/resources_pool.py
+xoa_core/core/resources/controller.py
+xoa_core/core/resources/pool.py
 xoa_core/core/resources/storage.py
-xoa_core/core/resources/datasets/__init__.py
-xoa_core/core/resources/datasets/enums.py
-xoa_core/core/resources/datasets/external/__init__.py
-xoa_core/core/resources/datasets/external/credentials.py
-xoa_core/core/resources/datasets/external/module.py
-xoa_core/core/resources/datasets/external/port.py
-xoa_core/core/resources/datasets/external/tester.py
-xoa_core/core/resources/datasets/internal/__init__.py
-xoa_core/core/resources/datasets/internal/credentials.py
-xoa_core/core/resources/datasets/internal/module.py
-xoa_core/core/resources/datasets/internal/port.py
-xoa_core/core/resources/datasets/internal/tester.py
+xoa_core/core/resources/types.py
+xoa_core/core/resources/resource/__init__.py
+xoa_core/core/resources/resource/const.py
+xoa_core/core/resources/resource/exceptions.py
+xoa_core/core/resources/resource/facade.py
+xoa_core/core/resources/resource/misc.py
+xoa_core/core/resources/resource/models/__decorator.py
+xoa_core/core/resources/resource/models/__init__.py
+xoa_core/core/resources/resource/models/module.py
+xoa_core/core/resources/resource/models/port.py
+xoa_core/core/resources/resource/models/tester.py
+xoa_core/core/resources/resource/models/types.py
 xoa_core/core/test_suites/__init__.py
 xoa_core/core/test_suites/_loader.py
-xoa_core/core/test_suites/controler.py
+xoa_core/core/test_suites/controller.py
 xoa_core/core/test_suites/datasets.py
 xoa_core/core/utils/__init__.py
-xoa_core/core/utils/decorators.py
 xoa_core/core/utils/observer.py
 xoa_core/core/utils/validators.py
```

