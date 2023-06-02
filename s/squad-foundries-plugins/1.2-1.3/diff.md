# Comparing `tmp/squad-foundries-plugins-1.2.tar.gz` & `tmp/squad-foundries-plugins-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squad-foundries-plugins-1.2.tar", last modified: Fri Apr 28 10:58:35 2023, max compression
+gzip compressed data, was "squad-foundries-plugins-1.3.tar", last modified: Fri Jun  2 08:51:39 2023, max compression
```

## Comparing `squad-foundries-plugins-1.2.tar` & `squad-foundries-plugins-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-28 10:58:35.367530 squad-foundries-plugins-1.2/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)    26526 2023-04-24 10:54:53.000000 squad-foundries-plugins-1.2/LICENSE
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-04-28 10:58:35.367530 squad-foundries-plugins-1.2/PKG-INFO
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       73 2023-04-24 10:55:55.000000 squad-foundries-plugins-1.2/README
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-28 10:58:35.367530 squad-foundries-plugins-1.2/mcu/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)     2549 2023-04-28 08:34:43.000000 squad-foundries-plugins-1.2/mcu/__init__.py
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       38 2023-04-28 10:58:35.367530 squad-foundries-plugins-1.2/setup.cfg
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      661 2023-04-28 08:34:50.000000 squad-foundries-plugins-1.2/setup.py
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-28 10:58:35.367530 squad-foundries-plugins-1.2/squad_foundries_plugins.egg-info/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-04-28 10:58:35.000000 squad-foundries-plugins-1.2/squad_foundries_plugins.egg-info/PKG-INFO
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      340 2023-04-28 10:58:35.000000 squad-foundries-plugins-1.2/squad_foundries_plugins.egg-info/SOURCES.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)        1 2023-04-28 10:58:35.000000 squad-foundries-plugins-1.2/squad_foundries_plugins.egg-info/dependency_links.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       37 2023-04-28 10:58:35.000000 squad-foundries-plugins-1.2/squad_foundries_plugins.egg-info/entry_points.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       31 2023-04-28 10:58:35.000000 squad-foundries-plugins-1.2/squad_foundries_plugins.egg-info/requires.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)        4 2023-04-28 10:58:35.000000 squad-foundries-plugins-1.2/squad_foundries_plugins.egg-info/top_level.txt
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-28 10:58:35.367530 squad-foundries-plugins-1.2/test/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)     9150 2023-04-24 10:51:01.000000 squad-foundries-plugins-1.2/test/test_mcu.py
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-06-02 08:51:39.651184 squad-foundries-plugins-1.3/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)    26526 2023-04-24 10:54:53.000000 squad-foundries-plugins-1.3/LICENSE
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-06-02 08:51:39.651184 squad-foundries-plugins-1.3/PKG-INFO
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       73 2023-04-24 10:55:55.000000 squad-foundries-plugins-1.3/README
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-06-02 08:51:39.651184 squad-foundries-plugins-1.3/mcu/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)     2571 2023-06-02 08:48:59.000000 squad-foundries-plugins-1.3/mcu/__init__.py
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       38 2023-06-02 08:51:39.651184 squad-foundries-plugins-1.3/setup.cfg
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      661 2023-06-02 08:49:31.000000 squad-foundries-plugins-1.3/setup.py
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-06-02 08:51:39.651184 squad-foundries-plugins-1.3/squad_foundries_plugins.egg-info/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-06-02 08:51:39.000000 squad-foundries-plugins-1.3/squad_foundries_plugins.egg-info/PKG-INFO
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      340 2023-06-02 08:51:39.000000 squad-foundries-plugins-1.3/squad_foundries_plugins.egg-info/SOURCES.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)        1 2023-06-02 08:51:39.000000 squad-foundries-plugins-1.3/squad_foundries_plugins.egg-info/dependency_links.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       37 2023-06-02 08:51:39.000000 squad-foundries-plugins-1.3/squad_foundries_plugins.egg-info/entry_points.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       31 2023-06-02 08:51:39.000000 squad-foundries-plugins-1.3/squad_foundries_plugins.egg-info/requires.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)        4 2023-06-02 08:51:39.000000 squad-foundries-plugins-1.3/squad_foundries_plugins.egg-info/top_level.txt
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-06-02 08:51:39.651184 squad-foundries-plugins-1.3/test/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)     9150 2023-04-24 10:51:01.000000 squad-foundries-plugins-1.3/test/test_mcu.py
```

### Comparing `squad-foundries-plugins-1.2/LICENSE` & `squad-foundries-plugins-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `squad-foundries-plugins-1.2/mcu/__init__.py` & `squad-foundries-plugins-1.3/mcu/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class MCUResults(BasePlugin):
     name = "MCU test results"
 
     def postprocess_testrun(self, testrun):
         has_test_results = False
-        regex = re.compile("TEST (?P<test_unit>.*) (?P<test_case_id>.*)=(?P<measurement>.*)")
+        regex = re.compile("TEST (?P<test_unit>.*)\/REVISION=v([0-9]{9}) (?P<test_case_id>.*)=(?P<measurement>.*)")
         issues = defaultdict(list)
         for issue in KnownIssue.active_by_environment(testrun.environment):
             issues[issue.test_name].append(issue)
         for line in  testrun.log_file.split('\n'):
             result = regex.search(line)
             if result:
                 suite_slug = result.group("test_unit")
```

### Comparing `squad-foundries-plugins-1.2/setup.py` & `squad-foundries-plugins-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='squad-foundries-plugins',
-    version='1.2',
+    version='1.3',
     author='Milosz Wasilewski',
     author_email='milosz.wasilewski@foundries.io',
     url='https://github.com/foundries/squadplugins',
     packages=['mcu'],
     entry_points={
         'squad_plugins': [
             'mcu=mcu:MCUResults',
```

### Comparing `squad-foundries-plugins-1.2/test/test_mcu.py` & `squad-foundries-plugins-1.3/test/test_mcu.py`

 * *Files identical despite different names*

