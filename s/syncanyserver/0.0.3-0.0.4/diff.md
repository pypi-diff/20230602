# Comparing `tmp/syncanyserver-0.0.3.tar.gz` & `tmp/syncanyserver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanyserver-0.0.3.tar", last modified: Mon May 29 10:05:27 2023, max compression
+gzip compressed data, was "syncanyserver-0.0.4.tar", last modified: Fri Jun  2 10:53:32 2023, max compression
```

## Comparing `syncanyserver-0.0.3.tar` & `syncanyserver-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:05:27.562142 syncanyserver-0.0.3/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.3/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-29 10:05:27.564115 syncanyserver-0.0.3/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.3/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-29 10:05:27.574114 syncanyserver-0.0.3/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2010 2023-05-27 14:13:18.000000 syncanyserver-0.0.3/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:05:27.215169 syncanyserver-0.0.3/syncanyserver/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-05-27 14:13:18.000000 syncanyserver-0.0.3/syncanyserver/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4121 2023-05-12 08:47:17.000000 syncanyserver-0.0.3/syncanyserver/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2464 2023-05-26 07:20:59.000000 syncanyserver-0.0.3/syncanyserver/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    31204 2023-05-26 09:48:39.000000 syncanyserver-0.0.3/syncanyserver/server.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1868 2023-05-12 04:09:15.000000 syncanyserver-0.0.3/syncanyserver/table.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2325 2023-05-26 07:20:59.000000 syncanyserver-0.0.3/syncanyserver/user.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:05:27.515717 syncanyserver-0.0.3/syncanyserver.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.3/syncanyserver.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      363 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:32.528340 syncanyserver-0.0.4/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.4/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-06-02 10:53:32.529955 syncanyserver-0.0.4/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.4/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-06-02 10:53:32.539965 syncanyserver-0.0.4/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2010 2023-05-31 05:37:53.000000 syncanyserver-0.0.4/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:32.189211 syncanyserver-0.0.4/syncanyserver/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-05-31 05:37:53.000000 syncanyserver-0.0.4/syncanyserver/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4121 2023-05-12 08:47:17.000000 syncanyserver-0.0.4/syncanyserver/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2464 2023-05-26 07:20:59.000000 syncanyserver-0.0.4/syncanyserver/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    30117 2023-06-02 04:45:20.000000 syncanyserver-0.0.4/syncanyserver/server.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1868 2023-05-12 04:09:15.000000 syncanyserver-0.0.4/syncanyserver/table.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2325 2023-05-26 07:20:59.000000 syncanyserver-0.0.4/syncanyserver/user.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:32.482379 syncanyserver-0.0.4/syncanyserver.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.4/syncanyserver.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      363 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/top_level.txt
```

### Comparing `syncanyserver-0.0.3/LICENSE` & `syncanyserver-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.3/PKG-INFO` & `syncanyserver-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```

### Comparing `syncanyserver-0.0.3/setup.py` & `syncanyserver-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.3"
+version = "0.0.4"
 
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
-        "syncanysql>=0.1.5",
+        "syncanysql>=0.1.6",
         "mysql-mimic>=2.2.3"
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
         "openpyxl": ["openpyxl>=2.5.0"],
         "postgresql": ["psycopg2>=2.8.6"],
```

### Comparing `syncanyserver-0.0.3/syncanyserver/database.py` & `syncanyserver-0.0.4/syncanyserver/database.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.3/syncanyserver/main.py` & `syncanyserver-0.0.4/syncanyserver/main.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.3/syncanyserver/server.py` & `syncanyserver-0.0.4/syncanyserver/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from mysql_mimic.errors import MysqlError, ErrorCode
 from mysql_mimic.intercept import expression_to_value
 from syncany.logger import get_logger
 from syncany.taskers.manager import TaskerManager
 from syncany.database.memory import MemoryDBCollection
 from syncanysql.compiler import Compiler
 from syncanysql.taskers.query import QueryTasker
-from syncanysql import ScriptEngine, Executor, ExecuterContext, SqlSegment, SqlParser, ExecuterError
+from syncanysql import ScriptEngine, Executor, ExecuterContext, SqlSegment, SqlParser
 from syncanysql.parser import FileParser
 from .user import UserIdentityProvider
 from .database import DatabaseManager, Database
 
 
 class ServerSessionExecuterContext(ExecuterContext):
     def __init__(self, *args, **kwargs):
@@ -42,36 +42,27 @@
         if isinstance(sql, str):
             sql_parser = SqlParser(sql)
             sqls = sql_parser.split()
         else:
             sqls = [sql] if not isinstance(sql, list) else sql
         with self.executor as executor:
             executor.run("session[%d-%d]" % (id(self.session), self.session.execute_index), sqls)
-            exit_code = executor.execute()
-            if exit_code is not None and exit_code != 0:
-                raise ExecuterError(exit_code)
-        return 0
+            executor.execute()
 
     def execute_segments(self, sql_segments):
         with self.executor as executor:
             executor.run("session[%d-%d]" % (id(self.session), self.session.execute_index), sql_segments)
-            exit_code = executor.execute()
-            if exit_code is not None and exit_code != 0:
-                raise ExecuterError(exit_code)
-        return 0
+            executor.execute()
 
     def execute_file(self, filename):
         sql_parser = FileParser(filename)
         sqls = sql_parser.load()
         with self.executor as executor:
             executor.run("session[%s-%d]%s" % (id(self.session), self.session.execute_index, filename), sqls)
-            exit_code = executor.execute()
-            if exit_code is not None and exit_code != 0:
-                raise ExecuterError(exit_code)
-        return 0
+            executor.execute()
 
     def execute_expression(self, expression, output_name=None):
         with self.executor as executor:
             config = executor.session_config.get()
             config["name"] = "session[%s-%d]" % (id(self.session), self.session.execute_index)
             try:
                 compiler = Compiler(config, executor.env_variables)
@@ -87,18 +78,15 @@
                 tasker = compiler.compile_expression(expression, arguments)
             finally:
                 config["name"] = ""
             if output_name and isinstance(tasker, QueryTasker):
                 tasker.config["output"] = "&." + output_name + "::" + tasker.config["output"].split("::")[-1]
             executor.runners.extend(tasker.start(config["name"], executor, executor.session_config, executor.manager,
                                                  arguments))
-            exit_code = executor.execute()
-            if exit_code is not None and exit_code != 0:
-                raise ExecuterError(exit_code)
-        return 0
+            executor.execute()
 
 
 class ServerSession(Session):
     def __init__(self, config_path, executer_context, identity_provider, thread_pool_executor, databases,
                  executor_wait_timeout, *args, **kwargs):
         super(ServerSession, self).__init__(*args, **kwargs)
 
@@ -164,17 +152,15 @@
             self.variables.set(name, value)
         if self.executer_context:
             with self.executer_context as executer_context:
                 try:
                     with executer_context.executor as executor:
                         executor.run("session[%d-%d]" % (id(self), self.execute_index),
                                      [SqlSegment("set " + str(setitem), 1)])
-                        exit_code = executor.execute()
-                        if exit_code is not None and exit_code != 0:
-                            raise ExecuterError(exit_code)
+                        executor.execute()
                 except Exception as e:
                     raise MysqlError(str(e), code=ErrorCode.NOT_SUPPORTED_YET)
         else:
             raise MysqlError(
                 f"Cannot SET variable {name} with scope {scope}",
                 code=ErrorCode.NOT_SUPPORTED_YET,
             )
@@ -272,24 +258,20 @@
                 continue
             with Executor(executer_context.engine.manager, executer_context.executor.session_config.session(),
                           executer_context.executor) as executor:
                 table_variable_sqls = variable_sqls.get((database_name, table_name))
                 if table_variable_sqls:
                     executor.run("session[%d-%d]" % (id(self), self.execute_index),
                                  [SqlSegment(table_variable_sqls[i], i + 1) for i in range(len(table_variable_sqls))])
-                    exit_code = executor.execute()
-                    if exit_code is not None and exit_code != 0:
-                        raise ExecuterError(exit_code)
+                    executor.execute()
 
                 sql_parser = FileParser(table.filename)
                 sqls = sql_parser.load()
                 executor.run("session[%s-%d]%s" % (id(self), self.execute_index, table.filename), sqls)
-                exit_code = executor.execute()
-                if exit_code is not None and exit_code != 0:
-                    raise ExecuterError(exit_code)
+                executor.execute()
 
             for table_expression in table_expressions:
                 table_expression.args["db"] = None
 
     def parse_primary_tables(self, expression, tables):
         if isinstance(expression, sqlglot_expressions.Select):
             from_expression = expression.args.get("from")
@@ -518,17 +500,15 @@
         self.script_engine.config.load_extensions()
         self.script_engine.manager = TaskerManager(DatabaseManager())
         self.script_engine.executor = Executor(self.script_engine.manager, self.script_engine.config.session())
         if init_execute_files:
             self.script_engine.executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1)
                                                      for i in range(len(init_execute_files))])
             with self.script_engine.executor as executor:
-                exit_code = executor.execute()
-                if exit_code is not None and exit_code != 0:
-                    raise ExecuterError(exit_code)
+                executor.execute()
         self.thread_pool_executor = ThreadPoolExecutor(self.executor_max_workers)
         self.identity_provider.load_users()
         Database.scan_databases(self.config_path, self.script_engine, self.databases)
 
     async def start_server(self, **kwargs):
         self.setup_script_engine()
         await super(Server, self).start_server(host=self.host, port=self.port,
```

### Comparing `syncanyserver-0.0.3/syncanyserver/table.py` & `syncanyserver-0.0.4/syncanyserver/table.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.3/syncanyserver/user.py` & `syncanyserver-0.0.4/syncanyserver/user.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.3/syncanyserver.egg-info/PKG-INFO` & `syncanyserver-0.0.4/syncanyserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```

