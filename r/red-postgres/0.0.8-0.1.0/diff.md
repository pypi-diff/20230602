# Comparing `tmp/red-postgres-0.0.8.tar.gz` & `tmp/red-postgres-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red-postgres-0.0.8.tar", last modified: Mon May 29 19:20:18 2023, max compression
+gzip compressed data, was "red-postgres-0.1.0.tar", last modified: Fri Jun  2 14:21:56 2023, max compression
```

## Comparing `red-postgres-0.0.8.tar` & `red-postgres-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 19:20:18.766191 red-postgres-0.0.8/
--rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4680 2023-05-29 19:20:18.766191 red-postgres-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4143 2023-05-29 17:36:29.000000 red-postgres-0.0.8/README.md
--rw-rw-rw-   0        0        0     1630 2023-05-29 19:19:53.000000 red-postgres-0.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-29 19:20:18.750188 red-postgres-0.0.8/red_postgres/
--rw-rw-rw-   0        0        0      180 2023-05-29 17:18:29.000000 red-postgres-0.0.8/red_postgres/__init__.py
--rw-rw-rw-   0        0        0     4306 2023-05-29 19:20:03.000000 red-postgres-0.0.8/red_postgres/engine.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:20:18.765191 red-postgres-0.0.8/red_postgres.egg-info/
--rw-rw-rw-   0        0        0     4680 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 19:20:18.767197 red-postgres-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 14:21:56.154644 red-postgres-0.1.0/
+-rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6017 2023-06-02 14:21:56.153645 red-postgres-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-06-02 14:21:00.000000 red-postgres-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1630 2023-06-02 14:12:43.000000 red-postgres-0.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-02 14:21:56.135645 red-postgres-0.1.0/red_postgres/
+-rw-rw-rw-   0        0        0      180 2023-05-29 17:18:29.000000 red-postgres-0.1.0/red_postgres/__init__.py
+-rw-rw-rw-   0        0        0     4903 2023-06-02 14:03:49.000000 red-postgres-0.1.0/red_postgres/engine.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:21:56.152644 red-postgres-0.1.0/red_postgres.egg-info/
+-rw-rw-rw-   0        0        0     6017 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 14:21:56.154644 red-postgres-0.1.0/setup.cfg
```

### Comparing `red-postgres-0.0.8/LICENSE` & `red-postgres-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `red-postgres-0.0.8/PKG-INFO` & `red-postgres-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: red-postgres
-Version: 0.0.8
-Summary: Piccolo Postgres integration for Red
-Author: Vertyco
-Project-URL: Homepage, https://github.com/vertyco/red-postgres
-Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # red-postgres
 
 Piccolo Postgres integration for Red-DiscordBot, although it could be used with any dpy bot as an easy wrapper for making postgres with cogs more modular.
 
 ![Py](https://img.shields.io/badge/python-v3.11-yellow?style=for-the-badge)
 ![black](https://img.shields.io/badge/style-black-000000?style=for-the-badge&?link=https://github.com/psf/black)
 ![license](https://img.shields.io/github/license/Vertyco/red-postgres?style=for-the-badge)
@@ -138,7 +124,59 @@
     app_name="cog_name",
     table_classes=table_finder(["db.tables"]),
     migrations_folder_path=os.path.join(CURRENT_DIRECTORY, "migrations"),
 )
 ```
 
 for `table_classes` add in the list of tables you're using
+
+# Local development and making migrations
+
+Handing migrations is up to you, but one way to do it is to make migrations locally like so:
+
+```python
+import os
+import subprocess
+from pathlib import Path
+
+root = Path(__file__).parent
+env = os.environ.copy()
+env["PICCOLO_CONF"] = "db.piccolo_conf"
+env["POSTGRES_HOST"] = "localhost"
+env["POSTGRES_PORT"] = "5432"
+env["POSTGRES_USER"] = "user"
+env["POSTGRES_PASSWORD"] = "password123!"
+env["POSTGRES_DATABASE"] = "templatecog"
+env["PYTHONIOENCODING"] = "utf-8"
+
+
+def make():
+    migration_result = subprocess.run(
+        ["piccolo", "migrations", "new", root.name, "--auto"],
+        env=env,
+        cwd=root,
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    ).stdout.decode()
+    print(migration_result)
+
+
+def run():
+    run_result = subprocess.run(
+        ["piccolo", "migrations", "forward", root.name],
+        env=env,
+        cwd=root,
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    ).stdout.decode()
+    print(run_result)
+
+
+if __name__ == "__main__":
+    make()
+    run()
+
+```
+
+You would have a similar file for each cog of your cogs, here you would create the migrations to include in your cog folder for users to run when the load up the cog.
```

### Comparing `red-postgres-0.0.8/README.md` & `red-postgres-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: red-postgres
+Version: 0.1.0
+Summary: Piccolo Postgres integration for Red
+Author: Vertyco
+Project-URL: Homepage, https://github.com/vertyco/red-postgres
+Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # red-postgres
 
 Piccolo Postgres integration for Red-DiscordBot, although it could be used with any dpy bot as an easy wrapper for making postgres with cogs more modular.
 
 ![Py](https://img.shields.io/badge/python-v3.11-yellow?style=for-the-badge)
 ![black](https://img.shields.io/badge/style-black-000000?style=for-the-badge&?link=https://github.com/psf/black)
 ![license](https://img.shields.io/github/license/Vertyco/red-postgres?style=for-the-badge)
@@ -124,7 +138,59 @@
     app_name="cog_name",
     table_classes=table_finder(["db.tables"]),
     migrations_folder_path=os.path.join(CURRENT_DIRECTORY, "migrations"),
 )
 ```
 
 for `table_classes` add in the list of tables you're using
+
+# Local development and making migrations
+
+Handing migrations is up to you, but one way to do it is to make migrations locally like so:
+
+```python
+import os
+import subprocess
+from pathlib import Path
+
+root = Path(__file__).parent
+env = os.environ.copy()
+env["PICCOLO_CONF"] = "db.piccolo_conf"
+env["POSTGRES_HOST"] = "localhost"
+env["POSTGRES_PORT"] = "5432"
+env["POSTGRES_USER"] = "user"
+env["POSTGRES_PASSWORD"] = "password123!"
+env["POSTGRES_DATABASE"] = "templatecog"
+env["PYTHONIOENCODING"] = "utf-8"
+
+
+def make():
+    migration_result = subprocess.run(
+        ["piccolo", "migrations", "new", root.name, "--auto"],
+        env=env,
+        cwd=root,
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    ).stdout.decode()
+    print(migration_result)
+
+
+def run():
+    run_result = subprocess.run(
+        ["piccolo", "migrations", "forward", root.name],
+        env=env,
+        cwd=root,
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    ).stdout.decode()
+    print(run_result)
+
+
+if __name__ == "__main__":
+    make()
+    run()
+
+```
+
+You would have a similar file for each cog of your cogs, here you would create the migrations to include in your cog folder for users to run when the load up the cog.
```

### Comparing `red-postgres-0.0.8/pyproject.toml` & `red-postgres-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "discord.py>=2.2.3", "piccolo[postgres]>=0.113.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "red-postgres"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   { name="Vertyco" },
 ]
 description = "Piccolo Postgres integration for Red"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `red-postgres-0.0.8/red_postgres/engine.py` & `red-postgres-0.1.0/red_postgres/engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,51 +8,53 @@
 from discord.ext.commands import Cog
 from piccolo.engine.postgres import PostgresEngine
 from piccolo.table import Table, create_db_tables
 
 log = logging.getLogger("red.red-postgres.engine")
 
 
-def acquire_db_engine(config: dict) -> PostgresEngine:
-    """This is ran in executor since it blocks if connection info is bad"""
-    return PostgresEngine(config=config)
-
-
-async def create_database_and_tables(
-    cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
-) -> PostgresEngine:
-    """Connect to postgres, create database/tables and return engine
+async def create_database(cog: Cog, config: dict) -> None:
+    """Create cog's database if it doesnt exist
 
     Args:
         cog (Cog): Cog instance
-        config (dict): database connection info
-        tables (list[type[Table]]): list of piccolo table subclasses
-        max_size (int): maximum number of database connections, 20 by default
-
-    Returns:
-        PostgresEngine instance
+        config (dict): Postgres connection information
     """
-    log.debug("Initializing database")
-    engine = await asyncio.to_thread(acquire_db_engine, config)
+    engine = await asyncio.to_thread(_acquire_db_engine, config)
     await engine.start_connection_pool()
 
     # Check if the database exists
     databases = await engine._run_in_pool("SELECT datname FROM pg_database;")
     cog_name = cog.__class__.__name__.lower()
     if cog_name not in [db["datname"] for db in databases]:
         # Create the database
         log.info(f"First time running {cog_name}! Creating new database!")
         await engine._run_in_pool(f"CREATE DATABASE {cog_name};")
 
     # Close old database connection
     await engine.close_connection_pool()
 
+
+async def create_tables(
+    cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
+) -> PostgresEngine:
+    """Connect to postgres, create database/tables and return engine
+
+    Args:
+        cog (Cog): Cog instance
+        config (dict): database connection info
+        tables (list[type[Table]]): list of piccolo table subclasses
+        max_size (int): maximum number of database connections, 20 by default
+
+    Returns:
+        PostgresEngine instance
+    """
     # Connect to the new database
-    config["database"] = cog_name
-    engine = await asyncio.to_thread(acquire_db_engine, config)
+    config["database"] = cog.__class__.__name__.lower()
+    engine = await asyncio.to_thread(_acquire_db_engine, config)
     await engine.start_connection_pool(max_size=max_size)
 
     # Update table engines
     for table_class in tables:
         table_class._meta.db = engine
 
     # Create any tables that don't already exist
@@ -64,66 +66,86 @@
     """
     Run any existing migrations programatically.
 
     There might be a better way to do this that subprocess, but haven't tested yet.
 
     Args:
         cog (Cog): Cog instance
-        config (dict): Database connection info
+        config (dict): database connection info
+        make (bool): automatically make new migrations, False by default
 
     Returns:
         str: Results of the migration
     """
 
     def run():
         root = Path(inspect.getfile(cog.__class__)).parent
-        env = os.environ.copy()
-        env["PICCOLO_CONF"] = "db.piccolo_conf"
-        env["POSTGRES_HOST"] = config.get("host")
-        env["POSTGRES_PORT"] = config.get("port")
-        env["POSTGRES_USER"] = config.get("user")
-        env["POSTGRES_PASSWORD"] = config.get("password")
-        env["POSTGRES_DATABASE"] = cog.__class__.__name__.lower()
-        env["PYTHONIOENCODING"] = "utf-8"
-
-        migration_result = subprocess.run(
+        return subprocess.run(
             ["piccolo", "migrations", "forward", root.name],
-            env=env,
+            env=_get_env(cog, config),
             cwd=root,
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         ).stdout.decode()
-        log.debug(migration_result)
 
-        diagnose_result = subprocess.run(
+    return await asyncio.to_thread(run)
+
+
+async def diagnose(cog: Cog, config: dict):
+    """
+    Diagnose any issues with Piccolo
+
+    Args:
+        cog (Cog): Cog instance
+        config (dict): database connection info
+    """
+
+    def run():
+        return subprocess.run(
             ["piccolo", "--diagnose"],
-            env=env,
-            cwd=root,
+            env=_get_env(cog, config),
+            cwd=Path(inspect.getfile(cog.__class__)).parent,
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         ).stdout.decode()
-        log.debug(diagnose_result)
-
-        return migration_result
 
     return await asyncio.to_thread(run)
 
 
 async def register_cog(
     cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
 ) -> tuple[PostgresEngine, str]:
     """Registers a cog by creating a database for it and initializing any tables it has
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
         max_size (int): maximum number of database connections, 20 by default
+        make (bool): automatically make new migrations, False by default
 
     Returns:
         Tuple[PostgresEngine, str]: Postgres Engine instance, migration results
     """
-    engine = await create_database_and_tables(cog, config, tables, max_size)
+    await create_database(cog, config)
     result = await run_migrations(cog, config)
+    engine = await create_tables(cog, config, tables, max_size)
     return engine, result
+
+
+def _acquire_db_engine(config: dict) -> PostgresEngine:
+    """This is ran in executor since it blocks if connection info is bad"""
+    return PostgresEngine(config=config)
+
+
+def _get_env(cog: Cog, config: dict):
+    env = os.environ.copy()
+    env["PICCOLO_CONF"] = "db.piccolo_conf"
+    env["POSTGRES_HOST"] = config.get("host")
+    env["POSTGRES_PORT"] = config.get("port")
+    env["POSTGRES_USER"] = config.get("user")
+    env["POSTGRES_PASSWORD"] = config.get("password")
+    env["POSTGRES_DATABASE"] = cog.__class__.__name__.lower()
+    env["PYTHONIOENCODING"] = "utf-8"
+    return env
```

### Comparing `red-postgres-0.0.8/red_postgres.egg-info/PKG-INFO` & `red-postgres-0.1.0/red_postgres.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.0.8
+Version: 0.1.0
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
@@ -138,7 +138,59 @@
     app_name="cog_name",
     table_classes=table_finder(["db.tables"]),
     migrations_folder_path=os.path.join(CURRENT_DIRECTORY, "migrations"),
 )
 ```
 
 for `table_classes` add in the list of tables you're using
+
+# Local development and making migrations
+
+Handing migrations is up to you, but one way to do it is to make migrations locally like so:
+
+```python
+import os
+import subprocess
+from pathlib import Path
+
+root = Path(__file__).parent
+env = os.environ.copy()
+env["PICCOLO_CONF"] = "db.piccolo_conf"
+env["POSTGRES_HOST"] = "localhost"
+env["POSTGRES_PORT"] = "5432"
+env["POSTGRES_USER"] = "user"
+env["POSTGRES_PASSWORD"] = "password123!"
+env["POSTGRES_DATABASE"] = "templatecog"
+env["PYTHONIOENCODING"] = "utf-8"
+
+
+def make():
+    migration_result = subprocess.run(
+        ["piccolo", "migrations", "new", root.name, "--auto"],
+        env=env,
+        cwd=root,
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    ).stdout.decode()
+    print(migration_result)
+
+
+def run():
+    run_result = subprocess.run(
+        ["piccolo", "migrations", "forward", root.name],
+        env=env,
+        cwd=root,
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    ).stdout.decode()
+    print(run_result)
+
+
+if __name__ == "__main__":
+    make()
+    run()
+
+```
+
+You would have a similar file for each cog of your cogs, here you would create the migrations to include in your cog folder for users to run when the load up the cog.
```

