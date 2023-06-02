# Comparing `tmp/lesscode_database-0.0.1.tar.gz` & `tmp/lesscode_database-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_database-0.0.1.tar", last modified: Thu Jun  1 15:04:43 2023, max compression
+gzip compressed data, was "dist/lesscode_database-0.0.2.tar", last modified: Fri Jun  2 01:24:03 2023, max compression
```

## Comparing `lesscode_database-0.0.1.tar` & `lesscode_database-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/
--rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-06-01 13:04:22.000000 lesscode_database-0.0.1/LICENSE
--rw-r--r--   0 navy      (1000) navy      (1000)      412 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)       46 2023-06-01 13:04:45.000000 lesscode_database-0.0.1/README.md
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/lesscode_database/
--rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-06-01 13:04:45.000000 lesscode_database-0.0.1/lesscode_database/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)    20703 2023-06-01 14:36:51.000000 lesscode_database-0.0.1/lesscode_database/connect_pool.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1085 2023-06-01 13:04:45.000000 lesscode_database-0.0.1/lesscode_database/connection_info.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1900 2023-06-01 13:32:42.000000 lesscode_database-0.0.1/lesscode_database/options.py
--rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-06-01 15:03:29.000000 lesscode_database-0.0.1/lesscode_database/version.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/lesscode_database.egg-info/
--rw-r--r--   0 navy      (1000) navy      (1000)      412 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/lesscode_database.egg-info/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)      349 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/lesscode_database.egg-info/SOURCES.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/lesscode_database.egg-info/dependency_links.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       18 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/lesscode_database.egg-info/top_level.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-06-01 15:04:43.000000 lesscode_database-0.0.1/setup.cfg
--rw-r--r--   0 navy      (1000) navy      (1000)     1194 2023-06-01 13:04:45.000000 lesscode_database-0.0.1/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/
+-rw-r--r--   0 baai       (501) staff       (20)    11357 2023-06-01 01:18:51.000000 lesscode_database-0.0.2/LICENSE
+-rw-r--r--   0 baai       (501) staff       (20)     6062 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)     5696 2023-06-02 01:23:39.000000 lesscode_database-0.0.2/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-01 01:20:17.000000 lesscode_database-0.0.2/lesscode_database/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)    23749 2023-06-02 00:50:57.000000 lesscode_database-0.0.2/lesscode_database/connect_pool.py
+-rw-r--r--   0 baai       (501) staff       (20)     1109 2023-06-02 00:50:57.000000 lesscode_database-0.0.2/lesscode_database/connection_info.py
+-rw-r--r--   0 baai       (501) staff       (20)     1900 2023-06-02 00:50:57.000000 lesscode_database-0.0.2/lesscode_database/options.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-02 01:23:39.000000 lesscode_database-0.0.2/lesscode_database/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)     6062 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      349 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       18 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1194 2023-06-01 01:27:32.000000 lesscode_database-0.0.2/setup.py
```

### Comparing `lesscode_database-0.0.1/LICENSE` & `lesscode_database-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.1/lesscode_database/connect_pool.py` & `lesscode_database-0.0.2/lesscode_database/connect_pool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import importlib
 import ssl
+from inspect import iscoroutine
 
 from lesscode_database.connection_info import ConnectionInfo
 
 
 class Pool:
     """
     Elasticsearch 数据库链接创建类
@@ -24,15 +25,15 @@
         if conn_info.params:
             if conn_info.params.get('protocol', 'http'):
                 protocol = conn_info.params.get('protocol', 'http')
         hosts = [f"{protocol}://{conn_info.user}:{conn_info.password}@{host}:{conn_info.port}" for host in host_arr]
         try:
             elasticsearch = importlib.import_module("elasticsearch")
         except ImportError:
-            raise Exception(f"elasticsearch is not exist,run:pip install elasticsearch")
+            raise Exception(f"elasticsearch is not exist,run:pip install elasticsearch[async]")
         pool = elasticsearch.AsyncElasticsearch(hosts=hosts)
         return pool
 
     @staticmethod
     def sync_create_es_pool(conn_info):
         """
         创建elasticsearch 同步连接池
@@ -349,14 +350,60 @@
                                                   skip_full_coverage_check=skip_full_coverage_check,
                                                   nodemanager_follow_cluster=nodemanager_follow_cluster,
                                                   host_port_remap=host_port_remap, db=conn_info.db_name,
                                                   username=conn_info.user, password=conn_info.password)
         return pool
 
     @staticmethod
+    def create_sqlalchemy_pool(conn_info):
+        """
+        创建sqlalchemy同步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        db_type = "mysql"
+        if conn_info.params:
+            if conn_info.params.get("db_type"):
+                db_type = conn_info.params.pop("db_type")
+        if db_type == "mysql":
+            url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                conn_info.db_name)
+        elif db_type == "postgresql":
+            url = 'postgresql+aiopg://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                conn_info.db_name)
+        elif db_type == "tidb":
+            url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                conn_info.db_name)
+        elif db_type == "ocean_base":
+            url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                conn_info.db_name)
+        else:
+            raise Exception("UNSUPPORTED DB TYPE")
+        try:
+            sqlalchemy = importlib.import_module("sqlalchemy.ext.asyncio")
+        except ImportError:
+            raise Exception(f"sqlalchemy is not exist,run:pip install sqlalchemy")
+        engine = sqlalchemy.create_async_engine(url, echo=conn_info.params.get("echo",
+                                                                               True) if conn_info.params else True,
+                                                pool_size=conn_info.min_size,
+                                                pool_recycle=conn_info.params.get("pool_recycle",
+                                                                                  3600) if conn_info.params else 3600,
+                                                max_overflow=conn_info.params.get("max_overflow",
+                                                                                  0) if conn_info.params else 0,
+                                                pool_timeout=conn_info.params.get("pool_timeout",
+                                                                                  10) if conn_info.params else 10,
+                                                pool_pre_ping=conn_info.params.get("pool_pre_ping",
+                                                                                   True) if conn_info.params else True)
+        return engine
+
+    @staticmethod
     def sync_create_sqlalchemy_pool(conn_info):
         """
         创建sqlalchemy同步连接池
         :param conn_info: 连接信息
         :return:
         """
         db_type = "mysql"
@@ -395,65 +442,71 @@
                                           pool_timeout=conn_info.params.get("pool_timeout",
                                                                             10) if conn_info.params else 10,
                                           pool_pre_ping=conn_info.params.get("pool_pre_ping",
                                                                              True) if conn_info.params else True)
         return engine
 
 
-def run_sync(future_func):
-    loop = asyncio.get_event_loop()
-    future = asyncio.ensure_future(future_func)
-    loop.run_until_complete(future)
-    return future.result()
+def run_sync(func_instance):
+    if iscoroutine(func_instance):
+        loop = asyncio.get_event_loop()
+        future = asyncio.ensure_future(func_instance)
+        loop.run_until_complete(future)
+        return future.result()
+    else:
+        return func_instance
 
 
 def get_pool(conn_info: ConnectionInfo):
     if conn_info.dialect == "elasticsearch":
         if conn_info.async_enable:
             return run_sync(Pool.create_es_pool(conn_info))
         else:
-            return Pool.sync_create_es_pool(conn_info)
+            return run_sync(Pool.sync_create_es_pool(conn_info))
 
     elif conn_info.dialect == "mongo":
         if conn_info.async_enable:
-            return Pool.create_mongo_pool(conn_info)
+            return run_sync(Pool.create_mongo_pool(conn_info))
         else:
-            return Pool.sync_create_mongo_pool(conn_info)
+            return run_sync(Pool.sync_create_mongo_pool(conn_info))
 
     elif conn_info.dialect == "mysql":
         if conn_info.async_enable:
             return run_sync(Pool.create_mysql_pool(conn_info))
         else:
-            return Pool.sync_create_mysql_pool(conn_info)
+            return run_sync(Pool.sync_create_mysql_pool(conn_info))
 
     elif conn_info.dialect == "nebula3":
-        return Pool.sync_create_nebula3_pool(conn_info)
+        return run_sync(Pool.sync_create_nebula3_pool(conn_info))
 
     elif conn_info.dialect == "neo4j":
         if conn_info.async_enable:
             return run_sync(Pool.create_neo4j_pool(conn_info))
         else:
-            return Pool.sync_create_neo4j_pool(conn_info)
+            return run_sync(Pool.sync_create_neo4j_pool(conn_info))
 
     elif conn_info.dialect == "postgresql":
         if conn_info.async_enable:
             return run_sync(Pool.create_postgresql_pool(conn_info))
         else:
-            return Pool.sync_create_postgresql_pool(conn_info)
+            return run_sync(Pool.sync_create_postgresql_pool(conn_info))
 
     elif conn_info.dialect == "redis":
         if conn_info.async_enable:
             return run_sync(Pool.create_redis_pool(conn_info))
         else:
-            return Pool.sync_create_redis_pool(conn_info)
+            return run_sync(Pool.sync_create_redis_pool(conn_info))
 
     elif conn_info.dialect == "redis_cluster":
         if conn_info.async_enable:
             return run_sync(Pool.create_redis_cluster_pool(conn_info))
         else:
-            return Pool.sync_create_redis_cluster_pool(conn_info)
+            return run_sync(Pool.sync_create_redis_cluster_pool(conn_info))
 
     elif conn_info.dialect == "sqlalchemy":
-        return Pool.sync_create_sqlalchemy_pool(conn_info)
+        if conn_info.async_enable:
+            return run_sync(Pool.create_sqlalchemy_pool(conn_info))
+        else:
+            return run_sync(Pool.sync_create_sqlalchemy_pool(conn_info))
 
     else:
         raise Exception(f"conn_info.dialect={conn_info.dialect} is not supported")
```

### Comparing `lesscode_database-0.0.1/lesscode_database/connection_info.py` & `lesscode_database-0.0.2/lesscode_database/connection_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
+from typing import Any
+
 
 class ConnectionInfo:
     """
     数据库连接信息对象
     """
 
     def __init__(self, dialect: str, host: str, port: int, user: str = None, password: str = None,
-                 db_name: str = None, name: str = None, params: dict = None, min_size: int = 3, max_size: int = 10,
+                 db_name: Any = None, name: str = None, params: dict = None, min_size: int = 3, max_size: int = 10,
                  enable: bool = True, async_enable: bool = False):
         # 数据库dialect类型
         self.dialect = dialect
         # 连接池名称
         if name:
             self.name = name
         else:
```

### Comparing `lesscode_database-0.0.1/lesscode_database/options.py` & `lesscode_database-0.0.2/lesscode_database/options.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.1/setup.py` & `lesscode_database-0.0.2/setup.py`

 * *Files identical despite different names*

