# Comparing `tmp/datoso-0.2.9.tar.gz` & `tmp/datoso-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.9.tar", last modified: Sun May 21 15:58:54 2023, max compression
+gzip compressed data, was "datoso-0.3.0.tar", last modified: Fri Jun  2 05:14:32 2023, max compression
```

## Comparing `datoso-0.2.9.tar` & `datoso-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.487207 datoso-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 15:58:42.000000 datoso-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-21 15:58:42.000000 datoso-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-21 15:58:54.487207 datoso-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-21 15:58:42.000000 datoso-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-21 15:58:42.000000 datoso-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-21 15:58:54.487207 datoso-0.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.479207 datoso-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.487207 datoso-0.2.9/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.487207 datoso-0.2.9/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42443 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.865323 datoso-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 05:14:20.000000 datoso-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 05:14:20.000000 datoso-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-02 05:14:32.865323 datoso-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-02 05:14:20.000000 datoso-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-02 05:14:20.000000 datoso-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 05:14:32.865323 datoso-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.853323 datoso-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.857323 datoso-0.3.0/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.865323 datoso-0.3.0/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42565 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.857323 datoso-0.3.0/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.9/LICENSE` & `datoso-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/PKG-INFO` & `datoso-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.9/README.md` & `datoso-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/pyproject.toml` & `datoso-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/__main__.py` & `datoso-0.3.0/src/datoso/__main__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/actions/processor.py` & `datoso-0.3.0/src/datoso/actions/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,20 @@
         """ Load a dat file. """
         from datoso.database.models.datfile import Dat
 
         # If there is a factory method, use it to create the class
         if getattr(self, '_factory', None) and self._factory:
             self._class = self._factory(self.file)
 
-        self._dat = self._class(file=self.file)
+        try:
+            self._dat = self._class(file=self.file)
+        except Exception:
+            self._dat = None
+            self.status = "Error"
+            return "Error"
         self._dat.load()
         self.database = Dat(seed=self.seed, **self._dat.dict())
         self.output = self.database.dict()
         return "Loaded"
 
 
 class DeleteOld(Process):
@@ -113,19 +118,22 @@
                 if old_file != new_file or config.getboolean('GENERAL', 'Overwrite', fallback=False) or not os.path.exists(destination):
                     if not old_file:
                         result = "Created"
                     elif old_file != new_file:
                         result = "Updated"
                     elif config.getboolean('GENERAL', 'Overwrite', fallback=False):
                         result = "Overwritten"
-                    if parser.parse(self.database.date, fuzzy=True) > parser.parse(self.previous['date'], fuzzy=True):
-                        result = "No Action Taken, Newer Found"
-                    else:
-                        self.previous['new_file'] = destination
-                        FileUtils.copy(origin, destination)
+                    try:
+                        if getattr(self.database, 'date', None) and self.previous.get('date', None) and parser.parse(self.database.date, fuzzy=True) > parser.parse(self.previous['date'], fuzzy=True):
+                            result = "No Action Taken, Newer Found"
+                        else:
+                            self.previous['new_file'] = destination
+                            FileUtils.copy(origin, destination)
+                    except ValueError:
+                        pass
                 else:
                     result = "Exists"
             else:
                 self.previous['new_file'] = None
                 result = "Ignored"
         else:
             FileUtils.copy(origin, destination)
```

### Comparing `datoso-0.2.9/src/datoso/commands/doctor.py` & `datoso-0.3.0/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/commands/seed.py` & `datoso-0.3.0/src/datoso/commands/seed.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,21 @@
                     continue
 
                 if not config.getboolean('COMMAND', 'Quiet', fallback=False):
                     delete_line(line)
                     line = f'Processing {Bcolors.OKCYAN}{file}{Bcolors.ENDC}'
                     print(line, end=' ', flush=True)
                 procesor = Processor(seed=self.name, file=f'{new_path}/{file}', actions=actions)
-                output = [x for x in procesor.process() if (x in self.status_to_show or Command.verbose)]
+                # output = [x for x in procesor.process() if (x in self.status_to_show or Command.verbose)]
+                output = []
+                for process in procesor.process():
+                    if process in self.status_to_show or Command.verbose:
+                        output.append(process)
+                    if process == 'Error':
+                        break
                 if 'Deleted' in output and 'Ignored' in output:
                     output.append('Disabled')
                 if not config.getboolean('COMMAND', 'Quiet', fallback=False):
                     # [print('\b \b', end='') for x in range(0, len(line))]
                     delete_line(line)
                     line = f'Processed {Bcolors.OKCYAN}{file}{Bcolors.ENDC}'
                     print(line, end=' ', flush=True)
```

### Comparing `datoso-0.2.9/src/datoso/configuration/folder_helper.py` & `datoso-0.3.0/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/configuration/logger.py` & `datoso-0.3.0/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/database/__init__.py` & `datoso-0.3.0/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/database/models/datfile.py` & `datoso-0.3.0/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/database/seeds/dat_repos.py` & `datoso-0.3.0/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/database/seeds/dat_rules.py` & `datoso-0.3.0/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/datoso.ini` & `datoso-0.3.0/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/helpers/__init__.py` & `datoso-0.3.0/src/datoso/helpers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     """ Color class. """
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
+    ERROR = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
     BOLDBLUE = '\e[1;34m'
     BOLDCYAN = '\e[1;36m'
     BOLDGREEN = '\e[1;32m'
     BOLDRED = '\e[1;31m'
@@ -127,7 +128,10 @@
     def move(origin, destination):
         """ Move file to destination. """
         os.makedirs(os.path.dirname(destination), exist_ok=True)
         try:
             shutil.move(origin, destination)
         except shutil.Error:
             FileUtils.remove(origin)
+
+class RequestUtils:
+    pass
```

### Comparing `datoso-0.2.9/src/datoso/helpers/executor.py` & `datoso-0.3.0/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/helpers/plugins.py` & `datoso-0.3.0/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/repositories/dat.py` & `datoso-0.3.0/src/datoso/repositories/dat.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,15 @@
     """ Base class for dat files. """
     def get_header(self) -> dict:
         """ Get the header from the dat file. """
         return { 'name': os.path.basename(self.file), 'description': self.file }
 
     def load(self) -> None:
         """ Load the data from a ClrMamePro file. """
+        self.main_key = 'datafile'
         self.games = []
         self.header = self.get_header()
 
         self.data = {
             self.main_key: {
                 'header':  self.header,
                 'game': self.games
@@ -320,14 +321,15 @@
     """ Base class for dat files. """
     def get_header(self) -> dict:
         """ Get the header from the dat file. """
         return { 'name': self.name, 'description': self.file }
 
     def load(self) -> None:
         """ Load the data from a ClrMamePro file. """
+        self.main_key = 'datafile'
         self.games = []
         for file in os.listdir(self.file):
             if file.endswith(('.xml', '.dat')):
                 self.games.append({ 'rom': { '@name': file } })
 
         self.name = os.path.basename(self.file)
```

### Comparing `datoso-0.2.9/src/datoso/repositories/dedupe.py` & `datoso-0.3.0/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/seeds/unknown_seed.py` & `datoso-0.3.0/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/seeds.txt` & `datoso-0.3.0/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso/systems.json` & `datoso-0.3.0/src/datoso/systems.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962546816479401%*

 * *Differences: {'insert': "[(46, OrderedDict([('company', 'Digital Media Cartridge'), ('system', 'Firecore'), "*

 * *           "('system_type', 'Console')]))]"}*

```diff
@@ -307,14 +307,19 @@
     },
     {
         "company": "Commodore",
         "system": "VIC-20",
         "system_type": "Computer"
     },
     {
+        "company": "Digital Media Cartridge",
+        "system": "Firecore",
+        "system_type": "Console"
+    },
+    {
         "company": "Emerson",
         "system": "Arcadia 2001",
         "system_type": "Console"
     },
     {
         "company": "Entex",
         "system": "Adventure Vision",
```

### Comparing `datoso-0.2.9/src/datoso.egg-info/PKG-INFO` & `datoso-0.3.0/src/datoso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.9/src/datoso.egg-info/SOURCES.txt` & `datoso-0.3.0/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.9/src/datoso.egg-info/requires.txt` & `datoso-0.3.0/src/datoso.egg-info/requires.txt`

 * *Files identical despite different names*

