# Comparing `tmp/red-postgres-0.1.0.tar.gz` & `tmp/red-postgres-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red-postgres-0.1.0.tar", last modified: Fri Jun  2 14:21:56 2023, max compression
+gzip compressed data, was "red-postgres-0.1.1.tar", last modified: Fri Jun  2 15:00:58 2023, max compression
```

## Comparing `red-postgres-0.1.0.tar` & `red-postgres-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 14:21:56.154644 red-postgres-0.1.0/
--rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6017 2023-06-02 14:21:56.153645 red-postgres-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5480 2023-06-02 14:21:00.000000 red-postgres-0.1.0/README.md
--rw-rw-rw-   0        0        0     1630 2023-06-02 14:12:43.000000 red-postgres-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-02 14:21:56.135645 red-postgres-0.1.0/red_postgres/
--rw-rw-rw-   0        0        0      180 2023-05-29 17:18:29.000000 red-postgres-0.1.0/red_postgres/__init__.py
--rw-rw-rw-   0        0        0     4903 2023-06-02 14:03:49.000000 red-postgres-0.1.0/red_postgres/engine.py
-drwxrwxrwx   0        0        0        0 2023-06-02 14:21:56.152644 red-postgres-0.1.0/red_postgres.egg-info/
--rw-rw-rw-   0        0        0     6017 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 14:21:56.000000 red-postgres-0.1.0/red_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 14:21:56.154644 red-postgres-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 15:00:58.138639 red-postgres-0.1.1/
+-rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6287 2023-06-02 15:00:58.137639 red-postgres-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5750 2023-06-02 15:00:17.000000 red-postgres-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1630 2023-06-02 14:57:44.000000 red-postgres-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-02 15:00:58.125639 red-postgres-0.1.1/red_postgres/
+-rw-rw-rw-   0        0        0      180 2023-05-29 17:18:29.000000 red-postgres-0.1.1/red_postgres/__init__.py
+-rw-rw-rw-   0        0        0     5377 2023-06-02 14:57:37.000000 red-postgres-0.1.1/red_postgres/engine.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:00:58.136639 red-postgres-0.1.1/red_postgres.egg-info/
+-rw-rw-rw-   0        0        0     6287 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 15:00:58.138639 red-postgres-0.1.1/setup.cfg
```

### Comparing `red-postgres-0.1.0/LICENSE` & `red-postgres-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `red-postgres-0.1.0/PKG-INFO` & `red-postgres-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.1.0
+Version: 0.1.1
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
 
     async def cog_load(self):
         asyncio.create_task(self.setup())
 
     async def setup(self):
         await self.bot.wait_until_red_ready()
         config = await self.bot.get_shared_api_tokens("piccolo")
-        self.db, migration_result_message = await register_cog(self, config, [MyTable])
+        self.db = await register_cog(self, config, [MyTable])
 
     async def cog_unload(self):
         if self.db:
             await self.db.close_connection_pool()
 ```
 
 The shared api token config for piccolo should be the following:
@@ -79,27 +79,31 @@
   "host": "host ip (127.0.0.1)",
   "port": "port (5432)",
   "user": "user123",
   "password": "password123"
 }
 ```
 
+> Note: database name in your config should normally be the default "postgres", this library will automatically handle connecting your cogs to their own database
+
 The register method connects to the database specified in config, creates the a new database with the name of the registering cog, registers any tables, runs any migrations, sets the new engine object to all tables, and returns the raw engine object.
 
+- The name of the database will be the the name of the cog's folder, not the name of the main cog.py file
+
 You can then use your piccolo table methods like so:
 
 ```python
 count = await MyTable.count()
 or
 objects = await MyTable.objects().where(MyTable.text == "Hello World")
 ```
 
 The engine associated with your tables after registering the cog is connected to the database named the same as the cog that registered them, thus using this integration with multiple cogs will not interfere, as each cog will create its own database.
 
-- _If your cog's name is `MyCog` then the database will be named `my_cog`_
+- _If your cog's folder name is `MyCog` then the database will be named `my_cog`_
 
 # Piccolo Configuration Files
 
 Your piccolo configuration files must be setup like so. This is really only used for migrations.
 
 - _When migrations are run, the os environment variables are mocked in subprocess, so there should be no conflicts_
 
@@ -189,8 +193,8 @@
 
 if __name__ == "__main__":
     make()
     run()
 
 ```
 
-You would have a similar file for each cog of your cogs, here you would create the migrations to include in your cog folder for users to run when the load up the cog.
+You would have a similar file in the root of each of your cog folders, here you would create the migrations to include in your cog folder for users to run when they load up the cog.
```

### Comparing `red-postgres-0.1.0/README.md` & `red-postgres-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     async def cog_load(self):
         asyncio.create_task(self.setup())
 
     async def setup(self):
         await self.bot.wait_until_red_ready()
         config = await self.bot.get_shared_api_tokens("piccolo")
-        self.db, migration_result_message = await register_cog(self, config, [MyTable])
+        self.db = await register_cog(self, config, [MyTable])
 
     async def cog_unload(self):
         if self.db:
             await self.db.close_connection_pool()
 ```
 
 The shared api token config for piccolo should be the following:
@@ -65,27 +65,31 @@
   "host": "host ip (127.0.0.1)",
   "port": "port (5432)",
   "user": "user123",
   "password": "password123"
 }
 ```
 
+> Note: database name in your config should normally be the default "postgres", this library will automatically handle connecting your cogs to their own database
+
 The register method connects to the database specified in config, creates the a new database with the name of the registering cog, registers any tables, runs any migrations, sets the new engine object to all tables, and returns the raw engine object.
 
+- The name of the database will be the the name of the cog's folder, not the name of the main cog.py file
+
 You can then use your piccolo table methods like so:
 
 ```python
 count = await MyTable.count()
 or
 objects = await MyTable.objects().where(MyTable.text == "Hello World")
 ```
 
 The engine associated with your tables after registering the cog is connected to the database named the same as the cog that registered them, thus using this integration with multiple cogs will not interfere, as each cog will create its own database.
 
-- _If your cog's name is `MyCog` then the database will be named `my_cog`_
+- _If your cog's folder name is `MyCog` then the database will be named `my_cog`_
 
 # Piccolo Configuration Files
 
 Your piccolo configuration files must be setup like so. This is really only used for migrations.
 
 - _When migrations are run, the os environment variables are mocked in subprocess, so there should be no conflicts_
 
@@ -175,8 +179,8 @@
 
 if __name__ == "__main__":
     make()
     run()
 
 ```
 
-You would have a similar file for each cog of your cogs, here you would create the migrations to include in your cog folder for users to run when the load up the cog.
+You would have a similar file in the root of each of your cog folders, here you would create the migrations to include in your cog folder for users to run when they load up the cog.
```

### Comparing `red-postgres-0.1.0/pyproject.toml` & `red-postgres-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "discord.py>=2.2.3", "piccolo[postgres]>=0.113.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "red-postgres"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Vertyco" },
 ]
 description = "Piccolo Postgres integration for Red"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `red-postgres-0.1.0/red_postgres/engine.py` & `red-postgres-0.1.1/red_postgres/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,40 @@
 from discord.ext.commands import Cog
 from piccolo.engine.postgres import PostgresEngine
 from piccolo.table import Table, create_db_tables
 
 log = logging.getLogger("red.red-postgres.engine")
 
 
-async def create_database(cog: Cog, config: dict) -> None:
+async def create_database(cog: Cog, config: dict) -> bool:
     """Create cog's database if it doesnt exist
 
     Args:
         cog (Cog): Cog instance
         config (dict): Postgres connection information
+
+    Returns:
+        bool: whether a new database was created
     """
     engine = await asyncio.to_thread(_acquire_db_engine, config)
     await engine.start_connection_pool()
 
     # Check if the database exists
+    created = False
+    database_name = _root(cog).name.lower()
     databases = await engine._run_in_pool("SELECT datname FROM pg_database;")
-    cog_name = cog.__class__.__name__.lower()
-    if cog_name not in [db["datname"] for db in databases]:
+    if database_name not in [db["datname"] for db in databases]:
         # Create the database
-        log.info(f"First time running {cog_name}! Creating new database!")
-        await engine._run_in_pool(f"CREATE DATABASE {cog_name};")
+        log.info(f"First time running {database_name}! Creating new database!")
+        await engine._run_in_pool(f"CREATE DATABASE {database_name};")
+        created = True
 
     # Close old database connection
     await engine.close_connection_pool()
+    return created
 
 
 async def create_tables(
     cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
 ) -> PostgresEngine:
     """Connect to postgres, create database/tables and return engine
 
@@ -44,108 +50,121 @@
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
         max_size (int): maximum number of database connections, 20 by default
 
     Returns:
         PostgresEngine instance
     """
-    # Connect to the new database
-    config["database"] = cog.__class__.__name__.lower()
-    engine = await asyncio.to_thread(_acquire_db_engine, config)
+    temp_config = config.copy()
+    temp_config["database"] = _root(cog).name.lower()
+    engine = await asyncio.to_thread(_acquire_db_engine, temp_config)
     await engine.start_connection_pool(max_size=max_size)
 
     # Update table engines
     for table_class in tables:
         table_class._meta.db = engine
 
     # Create any tables that don't already exist
     await create_db_tables(*tables, if_not_exists=True)
     return engine
 
 
-async def run_migrations(cog: Cog, config: dict):
+async def run_migrations(cog: Cog, config: dict) -> str:
     """
     Run any existing migrations programatically.
 
     There might be a better way to do this that subprocess, but haven't tested yet.
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
-        make (bool): automatically make new migrations, False by default
 
     Returns:
         str: Results of the migration
     """
 
     def run():
-        root = Path(inspect.getfile(cog.__class__)).parent
+        root = _root(cog)
+        temp_config = config.copy()
+        temp_config["database"] = root.name.lower()
         return subprocess.run(
-            ["piccolo", "migrations", "forward", root.name],
-            env=_get_env(cog, config),
+            ["piccolo", "migrations", "forward", root.name.lower()],
+            env=_get_env(temp_config),
             cwd=root,
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         ).stdout.decode()
 
     return await asyncio.to_thread(run)
 
 
-async def diagnose(cog: Cog, config: dict):
+async def diagnose(cog: Cog, config: dict) -> str:
     """
     Diagnose any issues with Piccolo
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
     """
 
     def run():
+        root = _root(cog)
+        temp_config = config.copy()
+        temp_config["database"] = root.name.lower()
         return subprocess.run(
             ["piccolo", "--diagnose"],
-            env=_get_env(cog, config),
-            cwd=Path(inspect.getfile(cog.__class__)).parent,
+            env=_get_env(temp_config),
+            cwd=root,
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         ).stdout.decode()
 
     return await asyncio.to_thread(run)
 
 
 async def register_cog(
     cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
-) -> tuple[PostgresEngine, str]:
+) -> PostgresEngine:
     """Registers a cog by creating a database for it and initializing any tables it has
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
         max_size (int): maximum number of database connections, 20 by default
         make (bool): automatically make new migrations, False by default
 
     Returns:
-        Tuple[PostgresEngine, str]: Postgres Engine instance, migration results
+        PostgresEngine
     """
+    # Create databse under root folder name
     await create_database(cog, config)
+    # Run any migrations
     result = await run_migrations(cog, config)
-    engine = await create_tables(cog, config, tables, max_size)
-    return engine, result
+    log.info(result)
+    # Create any tables and fetch postgres engine
+    return await create_tables(cog, config, tables, max_size)
 
 
 def _acquire_db_engine(config: dict) -> PostgresEngine:
     """This is ran in executor since it blocks if connection info is bad"""
     return PostgresEngine(config=config)
 
 
-def _get_env(cog: Cog, config: dict):
+def _get_env(config: dict) -> dict:
+    """Create mock environment for subprocess"""
     env = os.environ.copy()
     env["PICCOLO_CONF"] = "db.piccolo_conf"
     env["POSTGRES_HOST"] = config.get("host")
     env["POSTGRES_PORT"] = config.get("port")
     env["POSTGRES_USER"] = config.get("user")
     env["POSTGRES_PASSWORD"] = config.get("password")
-    env["POSTGRES_DATABASE"] = cog.__class__.__name__.lower()
+    env["POSTGRES_DATABASE"] = config.get("database")
     env["PYTHONIOENCODING"] = "utf-8"
     return env
+
+
+def _root(cog: Cog) -> Path:
+    """Get root directory of cog, used for path and database name"""
+    return Path(inspect.getfile(cog.__class__)).parent
```

### Comparing `red-postgres-0.1.0/red_postgres.egg-info/PKG-INFO` & `red-postgres-0.1.1/red_postgres.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.1.0
+Version: 0.1.1
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
 
     async def cog_load(self):
         asyncio.create_task(self.setup())
 
     async def setup(self):
         await self.bot.wait_until_red_ready()
         config = await self.bot.get_shared_api_tokens("piccolo")
-        self.db, migration_result_message = await register_cog(self, config, [MyTable])
+        self.db = await register_cog(self, config, [MyTable])
 
     async def cog_unload(self):
         if self.db:
             await self.db.close_connection_pool()
 ```
 
 The shared api token config for piccolo should be the following:
@@ -79,27 +79,31 @@
   "host": "host ip (127.0.0.1)",
   "port": "port (5432)",
   "user": "user123",
   "password": "password123"
 }
 ```
 
+> Note: database name in your config should normally be the default "postgres", this library will automatically handle connecting your cogs to their own database
+
 The register method connects to the database specified in config, creates the a new database with the name of the registering cog, registers any tables, runs any migrations, sets the new engine object to all tables, and returns the raw engine object.
 
+- The name of the database will be the the name of the cog's folder, not the name of the main cog.py file
+
 You can then use your piccolo table methods like so:
 
 ```python
 count = await MyTable.count()
 or
 objects = await MyTable.objects().where(MyTable.text == "Hello World")
 ```
 
 The engine associated with your tables after registering the cog is connected to the database named the same as the cog that registered them, thus using this integration with multiple cogs will not interfere, as each cog will create its own database.
 
-- _If your cog's name is `MyCog` then the database will be named `my_cog`_
+- _If your cog's folder name is `MyCog` then the database will be named `my_cog`_
 
 # Piccolo Configuration Files
 
 Your piccolo configuration files must be setup like so. This is really only used for migrations.
 
 - _When migrations are run, the os environment variables are mocked in subprocess, so there should be no conflicts_
 
@@ -189,8 +193,8 @@
 
 if __name__ == "__main__":
     make()
     run()
 
 ```
 
-You would have a similar file for each cog of your cogs, here you would create the migrations to include in your cog folder for users to run when the load up the cog.
+You would have a similar file in the root of each of your cog folders, here you would create the migrations to include in your cog folder for users to run when they load up the cog.
```

