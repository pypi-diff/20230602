# Comparing `tmp/syncanysql-0.1.5.tar.gz` & `tmp/syncanysql-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.5.tar", last modified: Mon May 29 10:04:48 2023, max compression
+gzip compressed data, was "syncanysql-0.1.6.tar", last modified: Fri Jun  2 10:53:06 2023, max compression
```

## Comparing `syncanysql-0.1.5.tar` & `syncanysql-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:48.583557 syncanysql-0.1.5/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.1.5/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-29 10:04:48.584557 syncanysql-0.1.5/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.5/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-29 10:04:48.594529 syncanysql-0.1.5/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2007 2023-05-27 14:11:29.000000 syncanysql-0.1.5/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:47.148615 syncanysql-0.1.5/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.5/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:47.667528 syncanysql-0.1.5/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1319 2023-05-29 09:21:36.000000 syncanysql-0.1.5/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6842 2023-05-29 09:21:36.000000 syncanysql-0.1.5/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.5/syncanysql/calculaters/env_variable_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:48.047552 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      384 2023-05-29 03:23:56.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10475 2023-05-27 08:55:29.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2860 2023-05-29 05:03:18.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/logical_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6764 2023-05-29 05:01:09.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   177108 2023-05-29 09:59:09.000000 syncanysql-0.1.5/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13459 2023-05-27 14:11:29.000000 syncanysql-0.1.5/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.5/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8633 2023-05-28 13:31:45.000000 syncanysql-0.1.5/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.5/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.5/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.5/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:48.536527 syncanysql-0.1.5/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.5/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.5/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.5/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.5/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.5/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    23474 2023-05-28 14:28:58.000000 syncanysql-0.1.5/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2890 2023-05-08 04:04:28.000000 syncanysql-0.1.5/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.5/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.5/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.5/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-27 07:49:00.000000 syncanysql-0.1.5/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:47.440030 syncanysql-0.1.5/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-05-29 10:04:46.000000 syncanysql-0.1.5/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.5/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      395 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:06.264278 syncanysql-0.1.6/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.1.6/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-02 10:53:06.266279 syncanysql-0.1.6/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3019 2023-05-30 02:47:03.000000 syncanysql-0.1.6/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-06-02 10:53:06.276278 syncanysql-0.1.6/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2007 2023-05-31 04:54:20.000000 syncanysql-0.1.6/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:04.549981 syncanysql-0.1.6/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8803 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:05.242668 syncanysql-0.1.6/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3127 2023-06-02 03:47:10.000000 syncanysql-0.1.6/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11327 2023-06-01 07:50:12.000000 syncanysql-0.1.6/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.6/syncanysql/calculaters/env_variable_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      406 2023-05-30 02:50:43.000000 syncanysql-0.1.6/syncanysql/calculaters/generate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:05.667392 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      384 2023-05-29 03:23:56.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10475 2023-05-27 08:55:29.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2982 2023-06-01 03:41:52.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/logical_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6764 2023-05-29 05:01:09.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3880 2023-06-02 03:47:10.000000 syncanysql-0.1.6/syncanysql/calculaters/window_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   194908 2023-06-02 06:40:14.000000 syncanysql-0.1.6/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13459 2023-05-27 14:11:29.000000 syncanysql-0.1.6/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      298 2023-06-02 03:32:36.000000 syncanysql-0.1.6/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8503 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4167 2023-06-02 04:35:38.000000 syncanysql-0.1.6/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.6/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7050 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:06.212462 syncanysql-0.1.6/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.6/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.6/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1601 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.6/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4120 2023-06-02 04:35:38.000000 syncanysql-0.1.6/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    23727 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2886 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2139 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1217 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.6/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-30 01:57:39.000000 syncanysql-0.1.6/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:04.862815 syncanysql-0.1.6/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1311 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.6/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      395 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.5/LICENSE` & `syncanysql-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/PKG-INFO` & `syncanysql-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
@@ -57,15 +57,15 @@
             b.name AS site_name,
             IF(c.site_amount > 0, c.site_amount, 0) AS site_amount,
             MAX(a.timeout_at) AS timeout_at,
             MAX(a.vip_timeout_at) AS vip_timeout_at,
             now() as `created_at?`
         FROM
             (SELECT
-                YIELD_DATA(sites) AS site_id,
+                YIELD_ARRAY(sites) AS site_id,
                     IF(vip_type = '2', GET_VALUE(rules, 0, 'timeout_time'), '') AS timeout_at,
                     IF(vip_type = '1', GET_VALUE(rules, 0, 'timeout_time'), '') AS vip_timeout_at
             FROM
                 `data/demo.json`
             WHERE
                 start_date >= '2021-01-01') a
                 JOIN
```

### Comparing `syncanysql-0.1.5/README.md` & `syncanysql-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     b.name AS site_name,
     IF(c.site_amount > 0, c.site_amount, 0) AS site_amount,
     MAX(a.timeout_at) AS timeout_at,
     MAX(a.vip_timeout_at) AS vip_timeout_at,
     now() as `created_at?`
 FROM
     (SELECT
-        YIELD_DATA(sites) AS site_id,
+        YIELD_ARRAY(sites) AS site_id,
             IF(vip_type = '2', GET_VALUE(rules, 0, 'timeout_time'), '') AS timeout_at,
             IF(vip_type = '1', GET_VALUE(rules, 0, 'timeout_time'), '') AS vip_timeout_at
     FROM
         `data/demo.json`
     WHERE
         start_date >= '2021-01-01') a
         JOIN
```

### Comparing `syncanysql-0.1.5/setup.py` & `syncanysql-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.5"
+version = "0.1.6"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=11.5.5,<12",
-        "syncany>=0.2.11",
+        "syncany>=0.2.12",
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
```

### Comparing `syncanysql-0.1.5/syncanysql/__init__.py` & `syncanysql-0.1.6/syncanysql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,16 @@
 from syncany.taskers.manager import TaskerManager
 from syncany.database import DatabaseManager, find_database
 from syncany.errors import DatabaseUnknownException
 from .version import version, version_info
 from .parser import SqlParser, SqlSegment
 from .config import GlobalConfig
 from .executor import Executor
-from .calculaters import AggregateCalculater, StateAggregateCalculater
-
-
-class ExecuterError(Exception):
-    def __init__(self, exit_code, *args):
-        super(ExecuterError, self).__init__(*args)
-
-        self.exit_code = exit_code
+from .calculaters import GenerateCalculater, AggregateCalculater, StateAggregateCalculater, \
+    WindowAggregateCalculater, WindowStateAggregateCalculater
 
 
 class ExecuterContext(object):
     _execute_index = 0
     _thread_local = threading.local()
 
     @classmethod
@@ -60,18 +54,15 @@
 
     def execute(self, sql):
         sql_parser = SqlParser(sql)
         sqls = sql_parser.split()
         self.__class__._execute_index += 1
         with self.executor as executor:
             executor.run("execute[%d]" % self._execute_index, sqls)
-            exit_code = executor.execute()
-            if exit_code is not None and exit_code != 0:
-                raise ExecuterError(exit_code)
-        return 0
+            executor.execute()
 
     def get_database(self, db=None):
         return self.engine.get_database(db)
 
     def get_memory_datas(self, name):
         return self.engine.get_memory_datas(name)
 
@@ -122,18 +113,15 @@
         self.config.load_extensions()
         self.manager = TaskerManager(DatabaseManager())
         self.executor = Executor(self.manager, self.config.session())
         if init_execute_files:
             self.executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in
                                        range(len(init_execute_files))])
             with self.executor as executor:
-                exit_code = executor.execute()
-                if exit_code is not None and exit_code != 0:
-                    raise ExecuterError(exit_code)
-        return 0
+                executor.execute()
 
     def get_variable(self, name, default=None):
         if self.executor is None:
             self.setup()
         if name and name[0] != "@":
             name = "@" + name
         return self.executor.env_variables.get(name, default)
```

### Comparing `syncanysql-0.1.5/syncanysql/calculaters/env_variable_calculater.py` & `syncanysql-0.1.6/syncanysql/calculaters/env_variable_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.6/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/logical_funcs.py` & `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/logical_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,8 +77,13 @@
     return 1 if not a else 0
 
 def mysql_is(a, b):
     if a is None or b is None:
         return 1 if a is b else 0
     return mysql_eq(a, b)
 
+def mysql_is_not(a, b):
+    if a is None or b is None:
+        return 0 if a is b else 1
+    return mysql_neq(a, b)
+
 funcs = {key[6:]: value for key, value in globals().items() if key.startswith("mysql_")}
```

### Comparing `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/compiler.py` & `syncanysql-0.1.6/syncanysql/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sqlglot.expressions
 from sqlglot import maybe_parse, ParseError
 from sqlglot import expressions as sqlglot_expressions
 from sqlglot.dialects import Dialect
 from sqlglot import tokens
 from syncany.taskers.core import CoreTasker
 from .errors import SyncanySqlCompileException
-from .calculaters import is_mysql_func, find_aggregate_calculater, CalculaterUnknownException
+from .calculaters import is_mysql_func, find_generate_calculater, find_aggregate_calculater, find_window_aggregate_calculater, CalculaterUnknownException
 from .config import CONST_CONFIG_KEYS
 from .parser import SqlParser
 from .taskers.delete import DeleteTasker
 from .taskers.query import QueryTasker, DEAULT_AGGREGATE
 from .taskers.into import IntoTasker
 from .taskers.explain import ExplainTasker
 from .taskers.set import SetCommandTasker
@@ -37,15 +37,15 @@
 
 
 class Compiler(object):
     ESCAPE_CHARS = ['\\\\a', '\\\\b', '\\\\f', '\\\\n', '\\\\r', '\\\\t', '\\\\v', '\\\\0']
     TYPE_FILTERS = {"int": "int", "float": "float", "str": "str", "bytes": "bytes", 'bool': 'bool', 'array': 'array', 'set': 'set',
                    'map': 'map', "objectid": "objectid", "uuid": "uuid", "datetime": "datetime", "date": "date", "time": "time",
                    "char": "str", "varchar": "str", "nchar": "str", "text": "str", "mediumtext": "str", "tinytext": "str",
-                   "bigint": "int", "mediumint": "int", "SMALLINT": "int", "tinyint": "int", "decimal": "float", "double": "float",
+                   "bigint": "int", "mediumint": "int", "smallint": "int", "tinyint": "int", "decimal": "float", "double": "float",
                    "boolean": "bool", "binary": "bytes", "varbinary": "bytes", "blob": "bytes", "timestamp": "datetime"}
 
     def __init__(self, config, env_variables):
         self.config = config
         self.env_variables = env_variables
         self.mapping = {}
 
@@ -229,15 +229,15 @@
                                         "id", " use ", update_type])
 
         if isinstance(expression.args["expression"], (sqlglot_expressions.Select, sqlglot_expressions.Union)):
             select_expression = expression.args["expression"]
             if isinstance(select_expression, sqlglot_expressions.Union):
                 self.compile_union(select_expression, config, arguments)
             else:
-                self.compile_select(select_expression, config, arguments)
+                self.compile_select(self.optimize_rewrite(select_expression, config, arguments), config, arguments)
         elif isinstance(expression.args["expression"], sqlglot_expressions.Values):
             values_expression = expression.args["expression"]
             if not values_expression.args.get("expressions"):
                 raise SyncanySqlCompileException('unkonw insert into, related sql "%s"' % self.to_sql(expression))
             datas = []
             for data_expression in values_expression.args["expressions"]:
                 data = {}
@@ -352,54 +352,70 @@
                     and isinstance(select_expression.args.get("this"), sqlglot_expressions.Star):
                 if not self.compile_select_star_column(select_expression, config, arguments, primary_table, join_tables):
                     raise SyncanySqlCompileException('unknown select * columns, related sql "%s"' % self.to_sql(expression))
                 continue
             if not isinstance(config["schema"], dict):
                 raise SyncanySqlCompileException('unknown select * columns, related sql "%s"' % self.to_sql(expression))
 
-            column_expression, aggregate_expression, calculate_expression, column_alias = None, None, None, None
+            column_expression, aggregate_expression, window_aggregate_expression, calculate_expression, column_alias = None, None, None, None, None
             if self.is_column(select_expression, config, arguments):
                 column_expression = select_expression
             elif isinstance(select_expression, sqlglot_expressions.Alias):
                 column_alias = select_expression.args["alias"].name if select_expression.args.get("alias") else None
                 if column_alias and column_alias in self.mapping:
                     column_alias = self.mapping[column_alias]
                 if self.is_const(select_expression.args["this"], config, arguments):
                     const_info = self.parse_const(select_expression.args["this"], config, arguments)
                     config["schema"][column_alias] = self.compile_const(select_expression.args["this"], config, arguments, const_info)
                     continue
                 elif self.is_column(select_expression.args["this"], config, arguments):
                     column_expression = select_expression.args["this"]
+                elif self.is_window_aggregate(select_expression.args["this"], config, arguments):
+                    window_aggregate_expression = select_expression.args["this"]
                 elif self.is_aggregate(select_expression.args["this"], config, arguments):
                     aggregate_expression = select_expression.args["this"]
                 else:
                     calculate_expression = select_expression.args["this"]
             elif self.is_const(select_expression, config, arguments):
                 const_info = self.parse_const(select_expression, config, arguments)
                 column_alias = str(select_expression)
                 config["schema"][column_alias] = self.compile_const(select_expression, config, arguments, const_info)
                 continue
+            elif self.is_window_aggregate(select_expression, config, arguments):
+                column_alias = str(select_expression)
+                window_aggregate_expression = select_expression
             elif self.is_aggregate(select_expression, config, arguments):
                 column_alias = str(select_expression)
                 aggregate_expression = select_expression
             elif self.is_calculate(select_expression, config, arguments):
                 column_alias = str(select_expression)
                 calculate_expression = select_expression
             else:
                 raise SyncanySqlCompileException('error select column, must have an alias name, related sql "%s"'
                                                  % self.to_sql(expression))
             if column_expression:
                 self.compile_select_column(column_expression, config, arguments, primary_table, column_alias,
                                            self.parse_column(column_expression, config, arguments), join_tables)
                 continue
+            if window_aggregate_expression:
+                self.compile_window_column(window_aggregate_expression, config, arguments, primary_table, column_alias,
+                                           [window_aggregate_expression], join_tables)
+                continue
             if aggregate_expression:
                 self.compile_aggregate_column(aggregate_expression, config, arguments, primary_table, column_alias,
                                               group_expression, [aggregate_expression], join_tables)
                 continue
 
+            window_aggregate_expressions = []
+            self.parse_window_aggregate(calculate_expression, config, arguments, window_aggregate_expressions)
+            if window_aggregate_expressions:
+                self.compile_window_column(calculate_expression, config, arguments, primary_table, column_alias,
+                                           window_aggregate_expressions, join_tables)
+                continue
+
             aggregate_expressions = []
             self.parse_aggregate(calculate_expression, config, arguments, aggregate_expressions)
             if aggregate_expressions:
                 self.compile_aggregate_column(calculate_expression, config, arguments, primary_table, column_alias,
                                               group_expression, aggregate_expressions, join_tables)
                 continue
             self.compile_select_calculate_column(calculate_expression, config, arguments, primary_table, column_alias,
@@ -425,15 +441,15 @@
                 config["intercepts"][0] = where_condition
             self.parse_condition_typing_filter(expression, config, arguments)
 
         having_expression = expression.args.get("having")
         if having_expression:
             having_condition = self.compile_having_condition(having_expression.args["this"], config, arguments, primary_table)
             if config.get("aggregate") and config["aggregate"]["having_columns"]:
-                if len({True if having_column in config["aggregate"]["schema"] else False
+                if len({True if having_column in config["aggregate"]["schema"] or having_column in config["aggregate"]["window_schema"] else False
                         for having_column in config["aggregate"]["having_columns"]}) != 1:
                     raise SyncanySqlCompileException(
                         'error having condition, cannot contain the values before and after the aggregate calculation at the same time, related sql "%s"'
                         % self.to_sql(expression))
             if not config["intercepts"]:
                 config["intercepts"] = [["#const", 1], ["#const", 1]]
             config["intercepts"][1] = having_condition
@@ -748,21 +764,21 @@
                         'error where condition, only "=,!=,>,>=,<,<=,in" operations executed by the database cannot be transparently transmitted,'
                         ' and it is executed with the having statement, column unkown, related sql "%s"'
                         % self.to_sql(expression))
                 left_calculater = self.compile_calculate(parse_calucate(left_expression), config, arguments,
                                                          primary_table, [])
 
             if isinstance(right_expression, list):
-                value_items = []
-                for value_expression_item in right_expression:
-                    if not self.is_const(value_expression_item, config, arguments):
-                        raise SyncanySqlCompileException('error where condition, array must be const value, related sql "%s"'
-                                                         % self.to_sql(expression))
-                    value_items.append(self.parse_const(value_expression_item, config, arguments)["value"])
-                return is_query_column, left_column, left_calculater, value_items
+                if all([self.is_const(value_expression_item, config, arguments) for value_expression_item in right_expression]):
+                    value_items = [self.parse_const(value_expression_item, config, arguments)["value"]
+                                   for value_expression_item in right_expression]
+                    return is_query_column, left_column, left_calculater, ["#const", value_items]
+                value_items = [self.compile_calculate(parse_calucate(value_expression_item), config, arguments, primary_table, [])
+                               for value_expression_item in right_expression]
+                return is_query_column, left_column, left_calculater, ["#make", value_items]
             if self.is_column(right_expression, config, arguments):
                 if not isinstance(config["schema"], dict):
                     raise SyncanySqlCompileException(
                         'error where condition, only "=,!=,>,>=,<,<=,in" operations executed by the database cannot be transparently transmitted,'
                         ' and it is executed with the having statement, column unkown, related sql "%s"'
                         % self.to_sql(expression))
                 if not left_calculater:
@@ -952,51 +968,39 @@
         }, [":#aggregate", "$.key", "$$.value"]]
         config["aggregate"]["key"] = copy.deepcopy(group_column)
         config["aggregate"]["schema"][column_alias] = aggregate_column
 
     def compile_aggregate_column(self, expression, config, arguments, primary_table, column_alias, group_expression,
                                  aggregate_expressions, join_tables):
         group_column = self.compile_aggregate_key(group_expression, config, arguments, primary_table, join_tables)
-        aggregate_value_expressions, distinct_column_index = [], -1
+        aggregate_value_expressions = []
         for i in range(len(aggregate_expressions)):
             aggregate_expression = aggregate_expressions[i]
             if isinstance(aggregate_expression, sqlglot_expressions.Anonymous):
                 if aggregate_expression.args.get("expressions") and isinstance(aggregate_expression.args["expressions"][0],
                                                                                sqlglot_expressions.Distinct):
-                    if distinct_column_index >= 0:
-                        raise SyncanySqlCompileException('error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' %
-                                                         self.to_sql(expression))
-                    distinct_column_index = i
-                    value_expressions = aggregate_expression.args["expressions"][0].args.get("expressions")
+                    raise SyncanySqlCompileException('error aggregate distinct, only be used for the count function, related sql "%s"' %
+                                                     self.to_sql(expression))
                 else:
                     value_expressions = aggregate_expression.args.get("expressions")
             else:
                 if isinstance(aggregate_expression.args["this"], sqlglot_expressions.Distinct):
-                    if distinct_column_index >= 0:
-                        raise SyncanySqlCompileException('error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' %
+                    if not isinstance(aggregate_expression, sqlglot_expressions.Count):
+                        raise SyncanySqlCompileException('error aggregate distinct, only be used for the count function, related sql "%s"' %
                                                          self.to_sql(expression))
-                    distinct_column_index = i
                     value_expressions = aggregate_expression.args.get("this").args.get("expressions")
                 else:
                     value_expressions = [aggregate_expression.args.get("this")]
             aggregate_value_expressions.append(value_expressions)
 
         if "aggregate" not in config:
             config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
         if len(aggregate_expressions) == 1 and aggregate_expressions[0] is expression:
             value_column = self.compile_aggregate_value(aggregate_expressions[0], config, arguments, primary_table, join_tables,
                                                         aggregate_value_expressions[0])
-            if distinct_column_index == 0 and value_column:
-                aggregate_distinct_keys = [copy.deepcopy(value_column[1])] if len(value_column) == 2 else copy.deepcopy(value_column[1:])
-                if not config["aggregate"]["distinct_keys"]:
-                    config["aggregate"]["distinct_keys"].extend(aggregate_distinct_keys)
-                elif config["aggregate"]["distinct_keys"] != aggregate_distinct_keys:
-                    raise SyncanySqlCompileException(
-                        'error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' % self.to_sql(expression))
-                config["aggregate"]["distinct_aggregates"].add(column_alias)
             if value_column and len(value_column) == 2:
                 value_column = value_column[1]
             aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(aggregate_expressions[0])
             aggregate_column = {
                 "key": group_column,
                 "value": value_column,
                 "calculate": [aggregate_calculate, "$." + column_alias, "$$.value"],
@@ -1005,33 +1009,23 @@
                 "final_value": [final_calculate, "$." + column_alias] if final_calculate else None
             }
         else:
             value_column, calculate_column, reduce_column = ["#make", {}], ["#make", {}], ["#make", {}]
             for i in range(len(aggregate_expressions)):
                 aggregate_value_key = "value_%d" % id(aggregate_expressions[i])
                 aggregate_value_column = self.compile_aggregate_value(aggregate_expressions[i], config, arguments, primary_table,
-                                                                                 join_tables, aggregate_value_expressions[i])
-                if distinct_column_index == i and aggregate_value_column:
-                    aggregate_distinct_keys = [copy.deepcopy(aggregate_value_column[1])] if len(aggregate_value_column) == 2 \
-                        else copy.deepcopy(aggregate_value_column[1:])
-                    if not config["aggregate"]["distinct_keys"]:
-                        config["aggregate"]["distinct_keys"].extend(aggregate_distinct_keys)
-                    elif config["aggregate"]["distinct_keys"] != aggregate_distinct_keys:
-                        raise SyncanySqlCompileException(
-                            'error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' % self.to_sql(expression))
-                    config["aggregate"]["distinct_aggregates"].add(column_alias)
+                                                                      join_tables, aggregate_value_expressions[i])
                 if aggregate_value_column and len(aggregate_value_column) == 2:
                     aggregate_value_column = aggregate_value_column[1]
                 aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(aggregate_expressions[i])
                 value_column[1][aggregate_value_key] = aggregate_value_column
                 calculate_column[1][aggregate_value_key] = [aggregate_calculate, "$." + column_alias + "." + aggregate_value_key,
-                                                                      "$$.value." + aggregate_value_key]
-                reduce_column[1][aggregate_value_key] = [reduce_calculate,
-                                                                   "$." + column_alias + "." + aggregate_value_key,
-                                                                   "$$." + column_alias + "." + aggregate_value_key]
+                                                            "$$.value." + aggregate_value_key]
+                reduce_column[1][aggregate_value_key] = [reduce_calculate, "$." + column_alias + "." + aggregate_value_key,
+                                                         "$$." + column_alias + "." + aggregate_value_key]
                 setattr(aggregate_expressions[i], "syncany_valuer",
                         [final_calculate, "$." + column_alias + "." + aggregate_value_key]
                         if final_calculate else ("$." + column_alias + "." + aggregate_value_key))
             self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias,
                                                  join_tables, False)
             aggregate_column = {
                 "key": group_column,
@@ -1121,36 +1115,212 @@
                                                       column_join_tables)
             value_column.append(self.compile_join_column(value_expression, config, arguments, primary_table,
                                                          calculate_column, column_join_tables))
         return value_column
 
     def compile_aggregate_calculate(self, expression):
         if isinstance(expression, sqlglot_expressions.Count):
+            if isinstance(expression.args.get("this"), sqlglot_expressions.Distinct):
+                return "@aggregate_distinct_count::aggregate", "@aggregate_distinct_count::reduce", "@aggregate_distinct_count::final_value"
             return "@aggregate_count::aggregate", "@aggregate_count::reduce", None
         elif isinstance(expression, sqlglot_expressions.Sum):
             return "@aggregate_sum::aggregate", "@aggregate_sum::reduce", None
         elif isinstance(expression, sqlglot_expressions.Min):
             return "@aggregate_min::aggregate", "@aggregate_min::reduce", None
         elif isinstance(expression, sqlglot_expressions.Max):
             return "@aggregate_max::aggregate", "@aggregate_max::reduce", None
         elif isinstance(expression, sqlglot_expressions.Avg):
             return "@aggregate_avg::aggregate", "@aggregate_avg::reduce", "@aggregate_avg::final_value"
         elif isinstance(expression, sqlglot_expressions.GroupConcat):
-            return "@aggregate_group_concat::aggregate", "@aggregate_group_concat::reduce", "@aggregate_group_concat::final_value"
+            return "@group_concat::aggregate", "@group_concat::reduce", "@group_concat::final_value"
+        elif isinstance(expression, sqlglot_expressions.GroupUniqArray):
+            return "@group_uniq_array::aggregate", "@group_uniq_array::reduce", "@group_uniq_array::final_value"
         elif isinstance(expression, sqlglot_expressions.Anonymous):
+            aggregate_funcs = {"grouparray": "group_array", "groupuniqarray": "group_uniq_array", "groupbitand": "group_bit_and",
+                               "groupbitor": "group_bit_or", "groupbitxor": "group_bit_xor"}
             calculater_name = expression.args["this"].lower()
+            if calculater_name in aggregate_funcs:
+                calculater_name = aggregate_funcs[calculater_name]
             try:
                 aggregate_calculater = find_aggregate_calculater(calculater_name)
                 return ("@" + calculater_name + "::aggregate",
                         "@" + calculater_name + "::reduce",
                         ("@" + calculater_name + "::final_value" if hasattr(aggregate_calculater, "final_value") else None))
             except CalculaterUnknownException:
                 raise SyncanySqlCompileException('unknown aggregate calculate, related sql "%s"' % self.to_sql(expression))
         else:
             raise SyncanySqlCompileException('unknown aggregate calculate, related sql "%s"' % self.to_sql(expression))
+
+    def compile_window_column(self, expression, config, arguments, primary_table, column_alias, window_expressions, join_tables):
+        if "aggregate" not in config:
+            config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
+        config["aggregate"]["window_schema"][column_alias] = {"aggregate": None, "final_value": None}
+        for i in range(len(window_expressions)):
+            aggregate_expression = window_expressions[i].args["this"]
+            if isinstance(aggregate_expression, sqlglot_expressions.Anonymous):
+                if aggregate_expression.args.get("expressions") and isinstance(aggregate_expression.args["expressions"][0], sqlglot_expressions.Distinct):
+                    raise SyncanySqlCompileException('error window distinct, only be used for the count function, related sql "%s"' %
+                                                     self.to_sql(expression))
+                else:
+                    value_expressions = aggregate_expression.args.get("expressions")
+            else:
+                if isinstance(aggregate_expression.args.get("this"), sqlglot_expressions.Distinct):
+                    if not isinstance(aggregate_expression, sqlglot_expressions.Count):
+                        raise SyncanySqlCompileException('error window distinct, only be used for the count function, related sql "%s"' %
+                                                         self.to_sql(expression))
+                    value_expressions = aggregate_expression.args.get("this").args.get("expressions")
+                else:
+                    if aggregate_expression.args.get("this"):
+                        value_expressions = [aggregate_expression.args.get("this")]
+                    else:
+                        value_expressions = []
+
+            partition_column = self.compile_window_key(window_expressions[i].args["partition_by"], config, arguments,
+                                                       primary_table, join_tables) if window_expressions[i].args.get("partition_by") else None
+            order_column = self.compile_window_order(window_expressions[i].args["order"], config, arguments,
+                                                     primary_table, join_tables) if window_expressions[i].args.get("order") else None
+            value_column = self.compile_window_value(window_expressions[i].args["this"], config, arguments, primary_table,
+                                                     join_tables, value_expressions) if value_expressions else None
+            if value_column and len(value_column) == 2:
+                value_column = value_column[1]
+            is_window_aggregate_calculate, aggregate_calculate, final_calculate = self.compile_window_calculate(window_expressions[i])
+            partition_calculate = "$.partition_key" if partition_column is not None else None
+            order_calculate = {"valuer": "$.order_key", "orders": order_column["orders"]} if order_column is not None else None
+            value_calculate = "$.value" if value_column is not None else None
+            if is_window_aggregate_calculate:
+                aggregate_calculate = [":#partition", partition_calculate, order_calculate, value_calculate,
+                                       [aggregate_calculate, "$.state", "$.value", "$.context"]]
+            else:
+                aggregate_calculate = [":#partition", partition_calculate, order_calculate, value_calculate,
+                                       [aggregate_calculate, "$.state", "$.value"]]
+            if final_calculate:
+                aggregate_calculate.append([":" + final_calculate, "$.*"])
+            window_aggregate_column = ["#make", {}, aggregate_calculate]
+            if partition_column is not None:
+                window_aggregate_column[1]["partition_key"] = partition_column
+            if order_column is not None:
+                window_aggregate_column[1]["order_key"] = order_column["valuer"]
+            if value_column is not None:
+                window_aggregate_column[1]["value"] = value_column
+
+            if len(window_expressions) > 1:
+                aggregate_column_alias = "__window_aggregate_value_%d__" % id(window_expressions[i])
+                config["schema"][aggregate_column_alias] = window_aggregate_column
+                setattr(window_expressions[i], "syncany_valuer", "$." + aggregate_column_alias)
+                if not isinstance(config["aggregate"]["window_schema"][column_alias]["aggregate"], dict):
+                    config["aggregate"]["window_schema"][column_alias]["aggregate"] = {}
+                config["aggregate"]["window_schema"][column_alias]["aggregate"][aggregate_column_alias] = copy.deepcopy(window_aggregate_column)
+            else:
+                config["schema"][column_alias] = window_aggregate_column
+                config["aggregate"]["window_schema"][column_alias]["aggregate"] = copy.deepcopy(window_aggregate_column)
+
+        if len(window_expressions) > 1:
+            self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias, join_tables, False)
+            config["aggregate"]["window_schema"][column_alias]["final_value"] = config["schema"].pop(column_alias, None)
+        primary_table["select_columns"][column_alias] = expression
+
+    def compile_window_key(self, expressions, config, arguments, primary_table, join_tables):
+        if not expressions:
+            return ["@aggregate_key", ["#const", "__k_g__"]]
+
+        key_column = ["@aggregate_key"]
+        for expression in expressions:
+            if self.is_column(expression, config, arguments):
+                key_expression_column = self.parse_column(expression, config, arguments)
+                if isinstance(config["schema"], dict) and not key_expression_column["table_name"] \
+                        and key_expression_column["column_name"] in config["schema"]:
+                    key_column.append(config["schema"][key_expression_column["column_name"]])
+                    continue
+                if not key_expression_column["table_name"] or key_expression_column["table_name"] == primary_table["table_name"]:
+                    key_column.append(self.compile_column(expression, config, arguments, key_expression_column))
+                    continue
+
+            calculate_fields = []
+            self.parse_calculate(expression, config, arguments, primary_table, calculate_fields)
+            calculate_fields = [calculate_field for calculate_field in calculate_fields if calculate_field["table_name"]
+                                and calculate_field["table_name"] != primary_table["table_name"]]
+            if not calculate_fields:
+                key_column.append(self.compile_calculate(expression, config, arguments, primary_table, []))
+                continue
+
+            column_join_tables = []
+            calculate_table_names = set([])
+            for calculate_field in calculate_fields:
+                if calculate_field["table_name"] not in join_tables:
+                    raise SyncanySqlCompileException('error join column, join table %s unknown, related sql "%s"' %
+                                                     (calculate_field["table_name"], self.to_sql(expression)))
+                calculate_table_names.add(calculate_field["table_name"])
+            self.compile_join_column_tables(expression, config, arguments, primary_table,
+                                            [join_tables[calculate_table_name] for calculate_table_name in calculate_table_names],
+                                            join_tables, column_join_tables)
+            calculate_column = self.compile_calculate(expression, config, arguments, primary_table, column_join_tables)
+            key_column.append(self.compile_join_column(expression, config, arguments, primary_table,
+                                                         calculate_column, column_join_tables))
+        return key_column
+
+    def compile_window_order(self, expression, config, arguments, primary_table, join_tables):
+        value_order_expressions, orders = [], []
+        for order_expression in expression.args["expressions"]:
+            order_key = str(order_expression.args["this"])
+            orders.append([order_key, order_expression.args.get("desc")])
+            value_order_expressions.append(order_expression.args["this"])
+        return {"valuer": self.compile_window_key(value_order_expressions, config, arguments,
+                                                  primary_table, join_tables), "orders": orders}
+
+    def compile_window_value(self, expression, config, arguments, primary_table, join_tables, value_expressions):
+        if isinstance(expression, sqlglot_expressions.Count) and isinstance(expression.args["this"],
+                                                                            sqlglot_expressions.Star):
+            return ["@make", ["#const", 0]]
+        if not value_expressions:
+            return ["@make", ["#const", None]]
+
+        value_column = ["@make"]
+        for value_expression in value_expressions:
+            calculate_fields = []
+            self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
+            calculate_fields = [calculate_field for calculate_field in calculate_fields if calculate_field["table_name"]
+                                and calculate_field["table_name"] != primary_table["table_name"]]
+            if not calculate_fields:
+                value_column.append(self.compile_calculate(value_expression, config, arguments, primary_table, []))
+                continue
+
+            column_join_tables = []
+            calculate_table_names = set([])
+            for calculate_field in calculate_fields:
+                if calculate_field["table_name"] not in join_tables:
+                    raise SyncanySqlCompileException('error join column, join table %s unknown, related sql "%s"' %
+                                                     (calculate_field["table_name"], self.to_sql(value_expression)))
+                calculate_table_names.add(calculate_field["table_name"])
+            self.compile_join_column_tables(value_expression, config, arguments, primary_table,
+                                            [join_tables[calculate_table_name] for calculate_table_name in
+                                             calculate_table_names], join_tables, column_join_tables)
+            calculate_column = self.compile_calculate(value_expression, config, arguments, primary_table,
+                                                      column_join_tables)
+            value_column.append(self.compile_join_column(value_expression, config, arguments, primary_table,
+                                                         calculate_column, column_join_tables))
+        return value_column
+
+    def compile_window_calculate(self, expression):
+        if isinstance(expression.args["this"], sqlglot_expressions.RowNumber):
+            return True, "@row_number::order_aggregate", None
+        elif isinstance(expression.args["this"], sqlglot_expressions.Anonymous):
+            calculater_name = expression.args["this"].args["this"].lower()
+            try:
+                aggregate_calculater = find_window_aggregate_calculater(calculater_name)
+                if expression.args.get("order"):
+                    return (True, "@" + calculater_name + "::order_aggregate",
+                            ("@" + calculater_name + "::final_value" if hasattr(aggregate_calculater, "final_value") else None))
+                return (True, "@" + calculater_name + "::aggregate",
+                        ("@" + calculater_name + "::final_value" if hasattr(aggregate_calculater, "final_value") else None))
+            except CalculaterUnknownException:
+                aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(expression.args["this"])
+                return False, aggregate_calculate, final_calculate
+        else:
+            aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(expression.args["this"])
+            return False, aggregate_calculate, final_calculate
         
     def compile_calculate(self, expression, config, arguments, primary_table, column_join_tables, join_index=-1):
         if hasattr(expression, "syncany_valuer"):
             return expression.syncany_valuer
         if isinstance(expression, sqlglot_expressions.Neg):
             return ["@neg", self.compile_calculate(expression.args["this"], config, arguments, primary_table, 
                                                    column_join_tables, join_index)]
@@ -1206,39 +1376,34 @@
                 if self.is_const(expression.args["expressions"][0], config, arguments):
                     config["defines"][define_name] = self.compile_const(expression.args["expressions"][0], config, arguments,
                                                                         self.parse_const(expression.args["expressions"][0], config, arguments))
                 else:
                     config["defines"][define_name] = self.compile_calculate(expression.args["expressions"][0], config, arguments, primary_table, column_join_tables, join_index)
                 return ["#call", define_name, "$.*"]
 
-            if calculater_name == "yield_data":
-                column = ["#yield"]
-                for arg_expression in expression.args.get("expressions", []):
-                    if self.is_const(arg_expression, config, arguments):
-                        column.append(self.compile_const(arg_expression, config, arguments,
-                                                         self.parse_const(arg_expression, config, arguments)))
-                    else:
-                        column.append(self.compile_calculate(arg_expression, config, arguments, primary_table, 
-                                                             column_join_tables, join_index))
-                return column
-
             if calculater_name not in ("add", "sub", "mul", "div", "mod") and is_mysql_func(calculater_name):
                 column = ["@mysql::" + calculater_name]
             else:
                 if calculater_name[:8] == "convert_":
                     column = ["@" + calculater_name + "|" + calculater_name[8:]]
                 else:
                     calculater_modules = calculater_name.split("$")
                     column = ["@" + calculater_modules[0] + (("::" + ".".join(calculater_modules[1:])) if len(calculater_modules) >= 2 else "")]
             for arg_expression in expression.args.get("expressions", []):
                 if self.is_const(arg_expression, config, arguments):
                     column.append(self.compile_const(arg_expression, config, arguments,
                                                      self.parse_const(arg_expression, config, arguments)))
                 else:
                     column.append(self.compile_calculate(arg_expression, config, arguments, primary_table, column_join_tables, join_index))
+
+            try:
+                find_generate_calculater(calculater_name)
+                return ["#yield", column]
+            except CalculaterUnknownException:
+                pass
             return column
         elif isinstance(expression, sqlglot_expressions.JSONExtract):
             return [
                 "@mysql::json_extract" if is_mysql_func("json_extract") else "@json_extract",
                 self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
                 self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index),
             ]
@@ -1267,17 +1432,17 @@
                 self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
             ]
         elif isinstance(expression, sqlglot_expressions.If):
             return [
                 "#if",
                 self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
                 self.compile_calculate(expression.args["true"], config, arguments, primary_table, column_join_tables, 
-                                       join_index) if expression.args.get("true") else False,
+                                       join_index) if expression.args.get("true") else ["#const", 1],
                 self.compile_calculate(expression.args["false"], config, arguments, primary_table, column_join_tables, 
-                                       join_index) if expression.args.get("false") else False,
+                                       join_index) if expression.args.get("false") else ["#const", 0],
             ]
         elif isinstance(expression, (sqlglot_expressions.IfNull, sqlglot_expressions.Coalesce)):
             condition_column = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
             if isinstance(expression, sqlglot_expressions.Coalesce):
                 def parse_coalesce(coalesce_expressions):
                     if not coalesce_expressions:
                         return None
@@ -1290,27 +1455,43 @@
                         coalesce_value_column = self.compile_calculate(coalesce_expressions[1], config, arguments, primary_table, column_join_tables, join_index)
                     return ["#if", ["@is_null", coalesce_column], coalesce_value_column, coalesce_column]
                 value_column = parse_coalesce(expression.args.get("expressions"))
             else:
                 value_column = self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
             return ["#if", ["@is_null", condition_column], value_column, condition_column]
         elif isinstance(expression, sqlglot_expressions.Case):
-            cases = {}
-            cases["#case"] = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index) \
-                                 if expression.args.get("this") else ["#const", 1]
-            if expression.args.get("ifs"):
-                for case_expression in expression.args["ifs"]:
-                    if not isinstance(case_expression, sqlglot_expressions.If) or not self.is_const(case_expression.args["this"], config, arguments):
-                        raise SyncanySqlCompileException('unknown calculate function, related sql "%s"' % self.to_sql(expression))
-                    case_value = self.parse_const(case_expression.args["this"], config, arguments)["value"]
-                    cases[(":" + str(case_value)) if isinstance(case_value, (int, float)) and not isinstance(case_value, bool) else case_value] = \
-                        self.compile_calculate(case_expression.args["true"], config, arguments, primary_table, column_join_tables, join_index)
-            cases["#end"] = self.compile_calculate(expression.args["default"], config, arguments, primary_table, column_join_tables, join_index) \
-                                if expression.args.get("default") else None
-            return cases
+            if expression.args.get("this") and all([self.is_const(case_expression.args["this"], config, arguments)
+                                                    for case_expression in expression.args.get("ifs", [])]):
+                cases = {}
+                cases["#case"] = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
+                if expression.args.get("ifs"):
+                    for case_expression in expression.args["ifs"]:
+                        case_value = self.parse_const(case_expression.args["this"], config, arguments)["value"]
+                        cases[(":" + str(case_value)) if isinstance(case_value, (int, float)) and not isinstance(case_value, bool) else case_value] = \
+                            self.compile_calculate(case_expression.args["true"], config, arguments, primary_table, column_join_tables, join_index)
+                cases["#end"] = self.compile_calculate(expression.args["default"], config, arguments, primary_table, column_join_tables, join_index) \
+                    if expression.args.get("default") else None
+                return cases
+
+            value_column = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index) \
+                if expression.args.get("this") else None
+            defaul_column = self.compile_calculate(expression.args["default"], config, arguments, primary_table, column_join_tables, join_index) \
+                if expression.args.get("default") else ["#const", 0]
+            if not expression.args.get("ifs"):
+                return defaul_column
+            def build_if(if_expression, case_expressions):
+                if_value_column = self.compile_calculate(if_expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
+                return [
+                    "#if",
+                    if_value_column if value_column is None else ["@mysql::eq", value_column, if_value_column],
+                    self.compile_calculate(if_expression.args["true"], config, arguments, primary_table, column_join_tables,
+                                           join_index) if expression.args.get("true") else ["#const", 1],
+                    build_if(case_expressions[0], case_expressions[1:]) if case_expressions else defaul_column,
+                ]
+            return build_if(expression.args["ifs"][0], expression.args["ifs"][1:])
         elif isinstance(expression, sqlglot_expressions.Func):
             func_args = {
                 "substring": ["this", "start", "length"],
             }
             func_name = expression.key.lower()
             column = ["@mysql::" + func_name] if is_mysql_func(func_name) else ["@" + func_name]
             arg_names = func_args.get(func_name) or [key for key in expression.arg_types] or ["this", "expression", "expressions"]
@@ -1339,23 +1520,36 @@
         elif self.is_column(expression, config, arguments):
             join_column = self.parse_column(expression, config, arguments)
             return self.compile_join_column_field(expression, config, arguments, primary_table, join_index, 
                                                   join_column, column_join_tables)
         elif isinstance(expression, sqlglot_expressions.Star):
             return "$.*"
         elif isinstance(expression, sqlglot_expressions.Tuple):
-            tuple_column = ["@make"]
-            for tuple_expression in expression.args["expressions"]:
-                tuple_column.append(self.compile_calculate(tuple_expression, config, arguments, primary_table,
-                                                   column_join_tables, join_index))
-            return ["@convert_array", tuple_column]
+            if all([self.is_const(tuple_expression, config, arguments) for tuple_expression in expression.args["expressions"]]):
+                value_columns = [self.parse_const(tuple_expression, config, arguments)["value"]
+                                 for tuple_expression in expression.args["expressions"]]
+                return ["#const", value_columns]
+            value_columns = [self.compile_calculate(tuple_expression, config, arguments, primary_table, column_join_tables, join_index)
+                             for tuple_expression in expression.args["expressions"]]
+            return ["#make", value_columns]
         elif isinstance(expression, sqlglot_expressions.Interval):
             return ["#const", {"value": expression.args["this"].args["this"], "unit": expression.args["unit"].args["this"]}]
         elif self.is_const(expression, config, arguments):
             return self.compile_const(expression, config, arguments, self.parse_const(expression, config, arguments))
+        elif isinstance(expression, sqlglot_expressions.Not):
+            if isinstance(expression.args["this"], sqlglot_expressions.Is):
+                return [
+                    "@mysql::is_not",
+                    self.compile_calculate(expression.args["this"].args["this"], config, arguments, primary_table,
+                                           column_join_tables, join_index),
+                    self.compile_calculate(expression.args["this"].args["expression"], config, arguments, primary_table,
+                                           column_join_tables, join_index)
+                ]
+            return ["@mysql::not", self.compile_calculate(expression.args["this"], config, arguments, primary_table,
+                                                          column_join_tables, join_index)]
         elif isinstance(expression, (sqlglot_expressions.Binary, sqlglot_expressions.Condition)):
             if isinstance(expression, sqlglot_expressions.And):
                 return [
                     "#if",
                     self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
                     self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index),
                     ["#const", 0]
@@ -1446,20 +1640,21 @@
                         continue
                     config["aggregate"]["having_columns"].add(calculate_field["column_name"])
                 left_calculater = self.compile_calculate(left_expression, config, arguments, primary_table, [])
             if not right_expression:
                 return left_calculater, None
 
             if isinstance(right_expression, list):
-                value_items = []
-                for value_expression_item in right_expression:
-                    if not self.is_const(value_expression_item, config, arguments):
-                        raise SyncanySqlCompileException('error having condition, array must be const value, related sql "%s"' % self.to_sql(expression))
-                    value_items.append(self.parse_const(value_expression_item, config, arguments)["value"])
-                return left_calculater, value_items
+                if all([self.is_const(value_expression_item, config, arguments) for value_expression_item in right_expression]):
+                    value_items = [self.parse_const(value_expression_item, config, arguments)["value"]
+                                   for value_expression_item in right_expression]
+                    return left_calculater, ["#const", value_items]
+                value_items = [self.compile_calculate(value_expression_item, config, arguments, primary_table, [])
+                               for value_expression_item in right_expression]
+                return left_calculater, ["#make", value_items]
             if self.is_column(right_expression, config, arguments):
                 right_column = self.parse_column(right_expression, config, arguments)
                 if isinstance(config["schema"], dict) and right_column["column_name"] not in config["schema"]:
                     raise SyncanySqlCompileException('unknown having condition column, column must be in the query result, related sql "%s"'
                                                      % self.to_sql(expression))
                 config["aggregate"]["having_columns"].add(right_column["column_name"])
                 return left_calculater, self.compile_column(right_expression, config, arguments, right_column)
@@ -1535,24 +1730,37 @@
                             has_column = True
                             break
                     if has_column:
                         continue
                 raise SyncanySqlCompileException('unknown order by column, the order by field must appear in the select field, related sql "%s"'
                                                  % self.to_sql(expression))
             column = self.parse_column(order_expression.args["this"], config, arguments)
-            if not isinstance(config["schema"], dict) or \
-                    (column["table_name"] and primary_table["table_name"] == column["table_name"]) or \
-                    (not column["table_name"] and column["column_name"] in primary_table["columns"]):
+            if not isinstance(config["schema"], dict) or (column["table_name"] and primary_table["table_name"] == column["table_name"]):
                 primary_sort_keys.append([column["column_name"], True if order_expression.args["desc"] else False])
+            elif not column["table_name"] and not primary_table["table_alias"]:
+                if not config.get("aggregate"):
+                    if column["column_name"] in primary_table["columns"] or column["column_name"] not in config["schema"]:
+                        primary_sort_keys.append([column["column_name"], True if order_expression.args["desc"] else False])
+                elif column["column_name"] not in config["aggregate"]["schema"] and column["column_name"] not in config["aggregate"]["window_schema"]:
+                    if column["column_name"] in primary_table["columns"] or column["column_name"] not in config["schema"]:
+                        primary_sort_keys.append([column["column_name"], True if order_expression.args["desc"] else False])
+            elif not column["table_name"] and primary_table["table_alias"]:
+                if not config.get("aggregate"):
+                    if column["column_name"] in primary_table["columns"] and column["column_name"] not in config["schema"]:
+                        primary_sort_keys.append([column["column_name"], True if order_expression.args["desc"] else False])
+                elif column["column_name"] not in config["aggregate"]["schema"] and column["column_name"] not in config["aggregate"]["window_schema"]:
+                    if column["column_name"] in primary_table["columns"] and column["column_name"] not in config["schema"]:
+                        primary_sort_keys.append([column["column_name"], True if order_expression.args["desc"] else False])
             sort_keys.append((column["column_name"], True if order_expression.args["desc"] else False))
         if sort_keys and len(primary_sort_keys) < len(sort_keys):
             if isinstance(config["schema"], dict):
                 for sort_key, _ in sort_keys:
-                    if sort_key not in config["schema"]:
-                        raise SyncanySqlCompileException('unknown order by column, related sql "%s"' % self.to_sql(expression))
+                    if sort_key in config["schema"]:
+                        continue
+                    raise SyncanySqlCompileException('unknown order by column, related sql "%s"' % self.to_sql(expression))
             config["pipelines"].append([">>@sort", "$.*|array", False, sort_keys])
         if primary_sort_keys:
             config["orders"].extend(primary_sort_keys)
         
     def compile_column(self, expression, config, arguments, column, scope_depth=1):
         if column["typing_filters"]:
             typing_filter_column = ("$" * scope_depth) + "." + column["column_name"] + "|" + column["typing_filters"][0]
@@ -1727,21 +1935,21 @@
                 value_column = self.compile_query_condition(value_expression, config, arguments, primary_table, condition_column["typing_filters"])
                 if isinstance(expression, sqlglot_expressions.In):
                     value_column = ["@convert_array", value_column]
                 else:
                     value_column = ["@convert_array", value_column, ":$.:0"]
                 return False, condition_column, value_column
             if isinstance(value_expression, list):
-                value_items = []
-                for value_expression_item in value_expression:
-                    if not self.is_const(value_expression_item, config, arguments):
-                        raise SyncanySqlCompileException('error join on condition, array must be const value, related sql "%s"'
-                                                         % self.to_sql(expression))
-                    value_items.append(self.parse_const(value_expression_item, config, arguments)["value"])
-                return False, condition_column, value_items
+                if all([self.is_const(value_expression_item, config, arguments) for value_expression_item in value_expression]):
+                    value_items = [self.parse_const(value_expression_item, config, arguments)["value"]
+                                   for value_expression_item in value_expression]
+                    return False, condition_column, ["#const", value_items]
+                value_items = [self.compile_calculate(value_expression_item, config, arguments, primary_table, [])
+                               for value_expression_item in value_expression]
+                return False, condition_column, ["#make", value_items]
             return False, condition_column, self.compile_calculate(value_expression, config, arguments, primary_table, [])
 
         if isinstance(expression, sqlglot_expressions.EQ):
             is_column, condition_column, value_column = parse(expression)
             if not is_column and condition_column:
                 if condition_column["typing_name"] not in join_table["querys"]:
                     join_table["querys"][condition_column["typing_name"]] = {}
@@ -1845,15 +2053,15 @@
         elif self.is_const(expression, config, arguments):
             pass
         else:
             if not isinstance(expression, sqlglot_expressions.Expression):
                 return
             for arg_expression in expression.args.values():
                 if isinstance(arg_expression, list):
-                    for item_arg_expression in expression.args["expressions"]:
+                    for item_arg_expression in arg_expression:
                         if not isinstance(item_arg_expression, sqlglot_expressions.Expression):
                             continue
                         if self.is_const(item_arg_expression, config, arguments):
                             continue
                         self.parse_calculate(item_arg_expression, config, arguments, primary_table, calculate_fields)
                 else:
                     if not isinstance(arg_expression, sqlglot_expressions.Expression):
@@ -1870,14 +2078,26 @@
         for _, child_expression in expression.args.items():
             if isinstance(child_expression, list):
                 for child_expression_item in child_expression:
                     self.parse_aggregate(child_expression_item, config, arguments, aggregate_expressions)
             else:
                 self.parse_aggregate(child_expression, config, arguments, aggregate_expressions)
 
+    def parse_window_aggregate(self, expression, config, arguments, window_aggregate_expressions):
+        if self.is_window_aggregate(expression, config, arguments):
+            window_aggregate_expressions.append(expression)
+        if not self.is_calculate(expression, config, arguments):
+            return
+        for _, child_expression in expression.args.items():
+            if isinstance(child_expression, list):
+                for child_expression_item in child_expression:
+                    self.parse_window_aggregate(child_expression_item, config, arguments, window_aggregate_expressions)
+            else:
+                self.parse_window_aggregate(child_expression, config, arguments, window_aggregate_expressions)
+
     def parse_table(self, expression, config, arguments):
         db_name = expression.args["db"].name if expression.args.get("db") else None
         if isinstance(expression.args["this"], sqlglot_expressions.Dot):
             def parse(expression):
                 return (parse(expression.args["this"]) if isinstance(expression.args["this"],
                                                                      sqlglot_expressions.Dot) else expression.args["this"].name) \
                        + "." + (parse(expression.args["expression"]) if isinstance(expression.args["expression"],
@@ -2166,33 +2386,43 @@
                                        sqlglot_expressions.Null, sqlglot_expressions.HexString, sqlglot_expressions.BitString,
                                        sqlglot_expressions.ByteString, sqlglot_expressions.Parameter))
 
     def is_calculate(self, expression, config, arguments):
         if isinstance(expression, sqlglot_expressions.Condition):
             return isinstance(expression, (sqlglot_expressions.EQ, sqlglot_expressions.NEQ, sqlglot_expressions.GT, sqlglot_expressions.GTE,
                                            sqlglot_expressions.LT, sqlglot_expressions.LTE, sqlglot_expressions.In, sqlglot_expressions.Not,
-                                           sqlglot_expressions.Between, sqlglot_expressions.Like, sqlglot_expressions.Func,
+                                           sqlglot_expressions.Is, sqlglot_expressions.Between, sqlglot_expressions.Like, sqlglot_expressions.Func,
                                            sqlglot_expressions.Binary))
         return isinstance(expression, (sqlglot_expressions.Neg, sqlglot_expressions.Binary, sqlglot_expressions.Select,
                                        sqlglot_expressions.Subquery, sqlglot_expressions.Union,
                                        sqlglot_expressions.BitwiseNot, sqlglot_expressions.Tuple))
 
     def is_aggregate(self, expression, config, arguments):
+        if isinstance(expression, (sqlglot_expressions.Column, sqlglot_expressions.Literal)):
+            return False
         if isinstance(expression, (sqlglot_expressions.Count, sqlglot_expressions.Sum, sqlglot_expressions.Max,
-                                   sqlglot_expressions.Min, sqlglot_expressions.Avg, sqlglot_expressions.GroupConcat)):
+                                   sqlglot_expressions.Min, sqlglot_expressions.Avg, sqlglot_expressions.GroupConcat,
+                                   sqlglot_expressions.GroupUniqArray)):
             return True
         if isinstance(expression, sqlglot_expressions.Anonymous):
+            aggregate_funcs = {"group_array", "grouparray", "group_uniq_array", "groupuniqarray", "group_bit_and", "groupbitand",
+                               "group_bit_or", "groupbitor", "group_bit_xor", "groupbitxor"}
             calculater_name = expression.args["this"].lower()
+            if calculater_name in aggregate_funcs:
+                return True
             try:
                 find_aggregate_calculater(calculater_name)
             except CalculaterUnknownException:
                 return False
             return True
         return False
 
+    def is_window_aggregate(self, expression, config, arguments):
+        return isinstance(expression, sqlglot_expressions.Window)
+
     def optimize_rewrite(self, expression, config, arguments):
         from_expression = expression.args.get("from")
         if not from_expression or not from_expression.expressions:
             return expression
         if len(from_expression.expressions) > 1:
             expression = self.optimize_rewrite_multi_select(expression, config, arguments, from_expression)
 
@@ -2210,16 +2440,18 @@
         if len(expression.args["expressions"]) == 1:
             if isinstance(expression.args["expressions"][0], sqlglot_expressions.Star):
                 return expression
         aggregate_expressions = []
         for select_expression in expression.args["expressions"]:
             if isinstance(select_expression, sqlglot_expressions.Alias):
                 self.parse_aggregate(select_expression.args["this"], config, arguments, aggregate_expressions)
+                self.parse_window_aggregate(select_expression.args["this"], config, arguments, aggregate_expressions)
             else:
                 self.parse_aggregate(select_expression, config, arguments, aggregate_expressions)
+                self.parse_window_aggregate(select_expression, config, arguments, aggregate_expressions)
         if aggregate_expressions or expression.args.get("group"):
             expression = self.optimize_rewrite_aggregate(expression, config, arguments, aggregate_expressions)
         return expression
 
     def optimize_rewrite_multi_select(self, expression, config, arguments, from_expression):
         primary_table = self.optimize_rewrite_parse_table(expression, config, arguments,
                                                           expression.args["from"].expressions[0])
@@ -2344,15 +2576,15 @@
             sql.append(str(expression.args["distinct"]))
         sql.append(", ".join([str(select_expression) for select_expression in expression.args["expressions"]]))
         sql.append("FROM " + str(selected_table["table_expression"]))
         for join_table in join_tables:
             if join_table["join_type"] == "right":
                 return expression
             sql.append("LEFT JOIN " + str(join_table["table_expression"]))
-            on_expressions = join_table["on_expressions"] + join_table["const_expressions"]
+            on_expressions = join_table["on_expressions"] + join_table["const_expressions"] + join_table["calcuate_expressions"]
             if on_expressions:
                 sql.append("ON " + " AND ".join([str(on_expression) for on_expression in on_expressions]))
 
         where_expressions = selected_table["const_expressions"] + primary_table["calcuate_expressions"] + selected_table["calcuate_expressions"]
         if where_expressions:
             sql.append("WHERE " + " AND ".join([("(" + str(where_expression) + ")")
                                                 if isinstance(where_expression, sqlglot_expressions.Or)
@@ -2407,15 +2639,15 @@
         sql.append(", ".join([str(select_expression) for select_expression in expression.args["expressions"]]))
         sql.append(str(expression.args["from"]))
         for join_expression in expression.args["joins"]:
             sql.append("LEFT JOIN " + str(join_expression.args["this"]))
             if join_expression.args.get("on"):
                 sql.append("ON " + str(join_expression.args["on"]))
 
-        inner_condition_sql = " AND ".join(["`%s`.`%s` IS NOT NULL" % (calculate_field["table_name"], calculate_field["column_name"])
+        inner_condition_sql = " AND ".join(["%s.%s IS NOT NULL" % (calculate_field["table_name"], calculate_field["column_name"])
                                             for calculate_field in inner_calculate_fields])
         if expression.args.get("where"):
             if isinstance(expression.args["where"].args["this"], sqlglot_expressions.Or):
                 sql.append("WHERE (" + str(expression.args["where"].args["this"]) + ") AND " + inner_condition_sql)
             else:
                 sql.append("WHERE " + str(expression.args["where"].args["this"]) + " AND " + inner_condition_sql)
         else:
@@ -2448,15 +2680,15 @@
         aggregate_calculate_fields = [calculate_field for calculate_field in aggregate_calculate_fields
                                       if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]]
         if not aggregate_calculate_fields:
             if not expression.args.get("group"):
                 return expression
             group_calculate_fields = []
             for group_expression in expression.args["group"].args["expressions"]:
-                self.parse_calculate(group_expression, config, arguments, primary_table, aggregate_calculate_fields)
+                self.parse_calculate(group_expression, config, arguments, primary_table, group_calculate_fields)
             group_calculate_fields = [calculate_field for calculate_field in group_calculate_fields
                                       if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]]
             if not group_calculate_fields:
                 return expression
 
         sub_sql = ["SELECT"]
         calculate_fields, sub_columns = [], []
@@ -2508,15 +2740,15 @@
                 select_column_name = self.parse_column(select_expression, config, arguments)["column_name"]
             else:
                 select_column_name = str(select_expression)
             select_sql.append("%s as `%s`" %
                               (str(self.optimize_rewrite_except_table(select_expression, config, arguments, primary_table)),
                                select_column_name))
         sql.append(", ".join(select_sql))
-        sql.append("FROM (%s) `%s`" % (" ".join(sub_sql), subquery_name))
+        sql.append("FROM (%s) %s" % (" ".join(sub_sql), subquery_name))
         if expression.args.get("group"):
             sql.append(str(self.optimize_rewrite_except_table(expression.args["group"], config, arguments, primary_table)))
         if expression.args.get("having"):
             sql.append(str(expression.args["having"]))
         if expression.args.get("order"):
             sql.append(str(self.optimize_rewrite_except_table(expression.args["order"], config, arguments, primary_table)))
         if expression.args.get("offset"):
```

### Comparing `syncanysql-0.1.5/syncanysql/config.py` & `syncanysql-0.1.6/syncanysql/config.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/executor.py` & `syncanysql-0.1.6/syncanysql/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -153,20 +153,17 @@
         self.runners.extend(tasker.start(name, self, self.session_config, self.manager, arguments))
 
     def execute(self):
         self._thread_local.current_executor = self
         while self.runners:
             self.tasker = self.runners.popleft()
             try:
-                exit_code = self.tasker.run(self, self.session_config, self.manager)
-                if exit_code is not None and exit_code != 0:
-                    return exit_code
+                self.tasker.run(self, self.session_config, self.manager)
             finally:
                 self.tasker = None
-        return 0
 
     def terminate(self):
         if not self.tasker:
             return
         self.tasker.terminate()
 
     def add_runner(self, tasker):
```

### Comparing `syncanysql-0.1.5/syncanysql/main.py` & `syncanysql-0.1.6/syncanysql/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,41 +39,49 @@
         global_config.load_extensions()
         manager = TaskerManager(DatabaseManager())
 
         try:
             with Executor(manager, global_config.session()) as executor:
                 if init_execute_files:
                     executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in range(len(init_execute_files))])
-                    exit_code = executor.execute()
-                    if exit_code is not None and exit_code != 0:
-                        return exit_code
+                    executor.execute()
 
                 if not sys.stdin.isatty() and (len(sys.argv) == 1 or (
                         len(sys.argv) >= 2 and not sys.argv[1].endswith(".sqlx") and not sys.argv[1].endswith(".sql"))):
                     start_time = time.time()
                     content = sys.stdin.read().strip()
                     if not content:
-                        exit(0)
+                        return
                     sql_parser = SqlParser(content[1:-1] if content[0] in ('"', "'") and content[-1] in ('"', "'") else content)
                     sqls = sql_parser.split()
                     executor.run("pipe", sqls)
-                    exit_code = executor.execute()
-                    get_logger().info("execute pipe sql finish with code %d %.2fms", exit_code, (time.time() - start_time) * 1000)
-                    exit(exit_code)
+                    try:
+                        executor.execute()
+                    except Exception as e:
+                        get_logger().info("execute pipe sql finish with Exception %s:%s %.2fms", e.__class__.__name__, e,
+                                          (time.time() - start_time) * 1000)
+                        raise e
+                    else:
+                        get_logger().info("execute pipe sql finish %.2fms", (time.time() - start_time) * 1000)
                 elif len(sys.argv) >= 2:
                     start_time = time.time()
                     file_parser = FileParser(sys.argv[1])
                     sqls = file_parser.load()
                     executor.run(sys.argv[1], sqls)
-                    exit_code = executor.execute()
-                    get_logger().info("execute file %s finish with code %d %.2fms", sys.argv[1], exit_code, (time.time() - start_time) * 1000)
-                    exit(exit_code)
+                    try:
+                        executor.execute()
+                    except Exception as e:
+                        get_logger().info("execute file %s finish with Exception %s:%s %.2fms", sys.argv[1], e.__class__.__name__, e,
+                                          (time.time() - start_time) * 1000)
+                        raise e
+                    else:
+                        get_logger().info("execute file %s finish %.2fms", sys.argv[1], (time.time() - start_time) * 1000)
                 else:
                     cli_prompt = CliPrompt(manager, global_config.session(), executor)
-                    exit(cli_prompt.run())
+                    cli_prompt.run()
         finally:
             manager.close()
     except SystemError:
         get_logger().error("signal exited")
         exit(130)
     except KeyboardInterrupt:
         get_logger().error("Crtl+C exited")
```

### Comparing `syncanysql-0.1.5/syncanysql/parser.py` & `syncanysql-0.1.6/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/prompt.py` & `syncanysql-0.1.6/syncanysql/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,34 +214,35 @@
             try:
                 text = session.prompt("> ", multiline=Condition(lambda: self.check_complete(session.app.current_buffer.text)),
                                       cursor=CursorShape.BEAM)
                 text = text.strip()
                 if not text:
                     continue
                 if text.lower()[:4] == "exit":
-                    return 0
+                    return
                 if text[0] == "!":
                     self.run_system_cmd(text[1:])
                     continue
                 if text[0] == "%":
                     self.run_magic_cmd(text[1:])
                     continue
                 self.executor.run("cli", [SqlSegment(text, lineno)])
                 try:
                     self.executor.execute()
+                except Exception as e:
+                    print(e.__class__.__name__ + ": " + str(e))
                 finally:
                     lineno += 1
                     self.executor.runners.clear()
             except KeyboardInterrupt:
                 continue  # Control-C pressed. Try again.
             except EOFError:
                 return 130
             except Exception as e:
                 print(e.__class__.__name__ + ": " + str(e))
-        return 0
 
     def check_complete(self, content):
         content = content.strip()
         if not content or content[:4] == "exit" or content[0] in ("!", "%"):
             return False
         sql_parser = SqlParser(content)
         try:
```

### Comparing `syncanysql-0.1.5/syncanysql/taskers/delete.py` & `syncanysql-0.1.6/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/taskers/execute.py` & `syncanysql-0.1.6/syncanysql/taskers/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 get_logger().info("execute file %s finish %.2fms", self.config["filename"], (time.time() - start_time) * 1000)
         else:
             os.system(self.config["filename"])
         return [self]
 
     def run(self, executor, session_config, manager):
         if not self.executor:
-            return 0
+            return
         with self.executor as executor:
             return executor.execute()
 
     def terminate(self):
         if not self.executor:
             return
         self.executor.terminate()
```

### Comparing `syncanysql-0.1.5/syncanysql/taskers/explain.py` & `syncanysql-0.1.6/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql/taskers/into.py` & `syncanysql-0.1.6/syncanysql/taskers/into.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     def run(self, executor, session_config, manager):
         try:
             core_tasker = self.tasker.tasker
             if not core_tasker:
                 return 1
             name = core_tasker.outputer.name
             schema_keys = tuple(core_tasker.schema.keys()) if isinstance(core_tasker.schema, dict) else None
-            exit_code = self.tasker.run(executor, session_config, manager)
-            if exit_code is not None and exit_code != 0:
-                return exit_code
+            self.tasker.run(executor, session_config, manager)
 
             try:
                 database_config = dict(**[database for database in session_config.get()["databases"]
                                           if database["name"] == "--"][0])
             except (TypeError, KeyError, IndexError):
                 raise DatabaseUnknownException("memory db is unknown")
             database_cls = find_database(database_config.pop("driver"))
@@ -73,15 +71,14 @@
                             if self.config["variables"][i] in executor.env_variables:
                                 executor.env_variables[self.config["variables"][i]] = None
                             continue
                         if isinstance(value, dict):
                             executor.env_variables[self.config["variables"][i]] = value[schema_keys[i]]
                         else:
                             executor.env_variables[self.config["variables"][i]] = [v[schema_keys[i]] for v in value]
-                return exit_code
             finally:
                 database.close()
         finally:
             self.tasker = None
 
     def terminate(self):
         if not self.tasker:
```

### Comparing `syncanysql-0.1.5/syncanysql/taskers/query.py` & `syncanysql-0.1.6/syncanysql/taskers/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from syncany.logger import get_logger
 from syncany.taskers.core import CoreTasker
 from syncany.hook import Hooker
 from syncany.taskers.tasker import _thread_local
 from syncany.main import TaskerYieldNext, warp_database_logging
 
 
-DEAULT_AGGREGATE = {"key": None, "schema": {}, "having_columns": set([]),
+DEAULT_AGGREGATE = {"key": None, "schema": {}, "window_schema": {}, "having_columns": set([]),
                     "distinct_keys": [], "distinct_aggregates": set([])}
 
 
 class ReduceHooker(Hooker):
     def __init__(self, executor, session_config, manager, arguments, tasker, config, batch, aggregate):
         self.executor = executor
         self.session_config = session_config
@@ -113,27 +113,31 @@
                 dependency_arguments.pop(key, None)
             dependency_tasker = QueryTasker(dependency_config, temporary_memory_manager=self.temporary_memory_manager)
             dependency_tasker.start(name, executor, session_config, manager, dependency_arguments)
             dependency_taskers.append(dependency_tasker)
 
         where_schema = self.config.pop("where_schema", None)
         limit, batch = int(arguments.get("@limit", 0)), int(arguments.get("@batch", 0))
-        require_reduce, reduce_intercept, sorted_limit = False, False, len(self.config.get("pipelines", [])) == 2
+        require_reduce, reduce_intercept = False, False
         if self.config.get("intercepts"):
             if aggregate and aggregate.get("schema") and aggregate.get("having_columns"):
-                if [having_column for having_column in aggregate["having_columns"] if having_column in aggregate["schema"]]:
+                if [having_column for having_column in aggregate["having_columns"]
+                    if having_column in aggregate["schema"] or having_column in aggregate["window_schema"]]:
                     require_reduce, reduce_intercept = True, True
-            if (batch > 0 or limit > 0 or sorted_limit):
+            if batch > 0:
                 require_reduce = True
-        if aggregate and aggregate.get("schema"):
-            if batch > 0 or limit > 0 or sorted_limit:
+        if aggregate and (aggregate.get("schema") or aggregate["window_schema"]):
+            if batch > 0:
                 require_reduce = True
             elif [aggregate_column["final_value"] for aggregate_column in aggregate["schema"].values()
                   if aggregate_column["final_value"]]:
                 require_reduce = True
+            elif [aggregate_column["final_value"] for aggregate_column in aggregate["window_schema"].values()
+                  if aggregate_column["final_value"]]:
+                require_reduce = True
         if where_schema:
             require_reduce = True
         if require_reduce and isinstance(self.config["schema"], dict) and not arguments.get("@streaming"):
             if not aggregate:
                 aggregate = copy.deepcopy(DEAULT_AGGREGATE)
             self.compile_reduce_config(where_schema, aggregate)
             if reduce_intercept:
@@ -164,29 +168,32 @@
             else:
                 _thread_local.current_tasker = self.tasker
             while True:
                 try:
                     value = self.tasker_generator.send(None)
                     if isinstance(value, TaskerYieldNext):
                         executor.add_runner(self)
-                        return 0
-                except StopIteration as e:
-                    exit_code = e.value
-                    if exit_code is not None and exit_code != 0:
-                        if self.sql_expression:
-                            get_logger().info("execute SQL %s finish with code %s %.2fms", self.name, exit_code,
-                                              (time.time() - self.run_start_time) * 1000)
-                        return exit_code
+                        return
+                except StopIteration:
                     break
+                except Exception as e:
+                    if self.sql_expression:
+                        get_logger().info("execute SQL %s finish with Exception %s:%s %.2fms", self.name, e.__class__.__name__, e,
+                                          (time.time() - self.run_start_time) * 1000)
+                    raise e
             if self.reduce_config:
-                exit_code = self.run_reduce(executor, session_config, manager, self.arguments, True)
-            if self.sql_expression:
-                get_logger().info("execute SQL %s finish with code %s %.2fms", self.name, exit_code,
-                                  (time.time() - self.run_start_time) * 1000)
-            return exit_code
+                try:
+                    self.run_reduce(executor, session_config, manager, self.arguments, True)
+                except Exception as e:
+                    if self.sql_expression:
+                        get_logger().info("execute SQL %s finish with Exception %s:%s %.2fms", self.name, e.__class__.__name__, e,
+                                          (time.time() - self.run_start_time) * 1000)
+                    raise e
+                if self.sql_expression:
+                    get_logger().info("execute SQL %s finish %.2fms", self.name, (time.time() - self.run_start_time) * 1000)
         finally:
             names = self.get_temporary_memory_collections()
             if names:
                 executor.clear_temporary_memory_collection(names)
 
     def run_yield(self, executor, session_config, manager, tasker, dependency_taskers):
         tasker_generator = tasker.run_yield()
@@ -194,18 +201,15 @@
                                                                             dependency_tasker.tasker, dependency_tasker.dependency_taskers))
                                         for dependency_tasker in dependency_taskers]
         while True:
             for dependency_tasker, dependency_tasker_generator in tuple(dependency_tasker_generators):
                 try:
                     _thread_local.current_tasker = dependency_tasker.tasker
                     dependency_tasker_generator.send(None)
-                except StopIteration as e:
-                    exit_code = e.value
-                    if exit_code is not None and exit_code != 0:
-                        return exit_code
+                except StopIteration:
                     if dependency_tasker.reduce_config:
                         dependency_tasker.run_reduce(executor, session_config, manager, dependency_tasker.arguments, True)
                     dependency_tasker_generators.remove((dependency_tasker, dependency_tasker_generator))
 
             try:
                 _thread_local.current_tasker = self.tasker
                 tasker_generator.send(None)
@@ -330,14 +334,19 @@
                 for key in where_schema:
                     config["schema"].pop(key, None)
             for key, column in config["schema"].items():
                 if key in aggregate["schema"] and aggregate["schema"][key]["final_value"]:
                     config["schema"][key] = aggregate["schema"][key]["final_value"]
                 else:
                     config["schema"][key] = "$." + key
+            for key, column in aggregate["window_schema"].items():
+                if isinstance(column["aggregate"], dict):
+                    for window_aggregate_key in column["aggregate"]:
+                        config["schema"].pop(window_aggregate_key, None)
+                    config["schema"][key] = column["final_value"]
             config["name"] = config["name"] + "#select@final"
         else:
             config["output"] = config["input"] + " use DI"
             config["name"] = config["name"] + "#select@reduce"
             config["intercepts"] = []
             config["pipelines"] = []
         if "intercepts" in config:
@@ -347,22 +356,18 @@
         arguments["@primary_order"] = False
         arguments["@limit"] = 0
         self.compile_tasker(arguments, tasker)
         tasker_generator = self.run_tasker(executor, session_config, manager, tasker, [])
         while True:
             try:
                 tasker_generator.send(None)
-            except StopIteration as e:
-                exit_code = e.value
-                if exit_code is not None and exit_code != 0:
-                    return exit_code
+            except StopIteration:
                 break
         if not final_reduce:
             self.tasker.status["store_count"] = tasker.status["store_count"]
-        return 0
 
     def compile_tasker(self, arguments, tasker):
         tasker.load()
         compile_arguments = {}
         compile_arguments.update({key.lower(): value for key, value in os.environ.items()})
         compile_arguments.update(arguments)
         if self.is_local_memory_database(tasker.config):
@@ -407,38 +412,34 @@
         try:
             tasker_generator = self.run_yield(executor, session_config, manager, tasker, dependency_taskers)
             while True:
                 try:
                     value = tasker_generator.send(None)
                     if isinstance(value, TaskerYieldNext):
                         yield value
-                except StopIteration as e:
-                    exit_code = e.value
-                    if exit_code is not None and exit_code != 0:
-                        return exit_code
+                except StopIteration:
                     break
-        except SystemError:
+        except SystemError as e:
             self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close(False, "signal terminaled")
             get_logger().error("signal exited")
-            return 130
-        except KeyboardInterrupt:
+            raise e
+        except KeyboardInterrupt as e:
             self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close(False, "user terminaled")
             get_logger().error("Crtl+C exited")
-            return 130
+            raise e
         except Exception as e:
             self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close(False, "Error: " + repr(e), traceback.format_exc())
             get_logger().error("tasker %s error: %s\n%s", tasker.name, e, traceback.format_exc())
-            return 1
+            raise e
         else:
             self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close()
-        return 0
 
     def execute_updater(self, executor, session_config, manager):
         for updater in self.updaters:
             updater(executor, session_config, manager)
 
         for dependency_tasker in self.dependency_taskers:
             dependency_tasker.execute_updater(executor, session_config, manager)
```

### Comparing `syncanysql-0.1.5/syncanysql/taskers/set.py` & `syncanysql-0.1.6/syncanysql/taskers/set.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,11 +61,11 @@
         value_info = value.split(".")
         if len(value_info) == 2 and (value_info[0].isdigit() or (value[0][0] == "-" and value[0][1:].isdigit())) \
                 and value_info[1].isdigit():
             return float(value)
         raise ValueError("unknown value: %s" % value)
 
     def run(self, executor, session_config, manager):
-        return 0
+        pass
 
     def terminate(self):
         pass
```

### Comparing `syncanysql-0.1.5/syncanysql/taskers/show.py` & `syncanysql-0.1.6/syncanysql/taskers/show.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         if self.config.get("key").lower() == "databases":
             self.show_databases(session_config)
         elif self.config.get("key").lower() == "imports":
             self.show_imports(session_config)
         return []
 
     def run(self, executor, session_config, manager):
-        return 0
+        pass
 
     def terminate(self):
         pass
 
     def show_databases(self, session_config):
         databases = copy.deepcopy(session_config.get().get("databases", []))
         fields, datas = ["name", "driver", "params", "virtual_views"], []
```

### Comparing `syncanysql-0.1.5/syncanysql/taskers/use.py` & `syncanysql-0.1.6/syncanysql/taskers/use.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
             if os.path.exists(use_info[0]):
                 session_config.set("sources." + use_info[0].split(".")[-1], use_info[0])
             else:
                 session_config.set("imports." + use_info[0].split(".")[-1], use_info[0])
         return []
 
     def run(self, executor, session_config, manager):
-        return 0
+        pass
 
     def terminate(self):
         pass
```

### Comparing `syncanysql-0.1.5/syncanysql/utils.py` & `syncanysql-0.1.6/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.5/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.6/syncanysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
@@ -57,15 +57,15 @@
             b.name AS site_name,
             IF(c.site_amount > 0, c.site_amount, 0) AS site_amount,
             MAX(a.timeout_at) AS timeout_at,
             MAX(a.vip_timeout_at) AS vip_timeout_at,
             now() as `created_at?`
         FROM
             (SELECT
-                YIELD_DATA(sites) AS site_id,
+                YIELD_ARRAY(sites) AS site_id,
                     IF(vip_type = '2', GET_VALUE(rules, 0, 'timeout_time'), '') AS timeout_at,
                     IF(vip_type = '1', GET_VALUE(rules, 0, 'timeout_time'), '') AS vip_timeout_at
             FROM
                 `data/demo.json`
             WHERE
                 start_date >= '2021-01-01') a
                 JOIN
```

### Comparing `syncanysql-0.1.5/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.6/syncanysql.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 syncanysql.egg-info/entry_points.txt
 syncanysql.egg-info/not-zip-safe
 syncanysql.egg-info/requires.txt
 syncanysql.egg-info/top_level.txt
 syncanysql/calculaters/__init__.py
 syncanysql/calculaters/aggregate_calculater.py
 syncanysql/calculaters/env_variable_calculater.py
+syncanysql/calculaters/generate_calculater.py
 syncanysql/calculaters/mysql_calculater.py
+syncanysql/calculaters/window_calculater.py
 syncanysql/calculaters/mysql_funcs/__init__.py
 syncanysql/calculaters/mysql_funcs/datetime_funcs.py
 syncanysql/calculaters/mysql_funcs/json_funcs.py
 syncanysql/calculaters/mysql_funcs/logical_funcs.py
 syncanysql/calculaters/mysql_funcs/number_funcs.py
 syncanysql/calculaters/mysql_funcs/string_funcs.py
 syncanysql/taskers/__init__.py
```

