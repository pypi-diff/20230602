# Comparing `tmp/neo4cdisc-1.0.4.0.tar.gz` & `tmp/neo4cdisc-1.0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4cdisc-1.0.4.0.tar", last modified: Fri Feb  3 09:50:37 2023, max compression
+gzip compressed data, was "neo4cdisc-1.0.5.0.tar", last modified: Fri Jun  2 14:29:44 2023, max compression
```

## Comparing `neo4cdisc-1.0.4.0.tar` & `neo4cdisc-1.0.5.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-02-03 09:50:37.015704 neo4cdisc-1.0.4.0/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    11357 2023-01-18 16:45:48.000000 neo4cdisc-1.0.4.0/LICENSE
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    13355 2023-02-03 09:50:37.015704 neo4cdisc-1.0.4.0/PKG-INFO
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1088 2023-02-03 08:40:07.000000 neo4cdisc-1.0.4.0/README.md
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-02-03 09:50:37.007703 neo4cdisc-1.0.4.0/cdisc_data_providers/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       69 2023-01-18 16:45:48.000000 neo4cdisc-1.0.4.0/cdisc_data_providers/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    11169 2023-01-18 16:45:48.000000 neo4cdisc-1.0.4.0/cdisc_data_providers/sdtm_data_provider.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-02-03 09:50:37.011704 neo4cdisc-1.0.4.0/cdisc_model_managers/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      126 2023-02-03 08:40:07.000000 neo4cdisc-1.0.4.0/cdisc_model_managers/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1044 2023-02-03 08:40:07.000000 neo4cdisc-1.0.4.0/cdisc_model_managers/cdisc_api.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    21929 2023-02-03 08:40:07.000000 neo4cdisc-1.0.4.0/cdisc_model_managers/cdisc_model_manager.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    18806 2023-01-18 16:45:48.000000 neo4cdisc-1.0.4.0/cdisc_model_managers/cdisc_standard_loader.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-02-03 09:50:37.015704 neo4cdisc-1.0.4.0/neo4cdisc.egg-info/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    13355 2023-02-03 09:50:36.000000 neo4cdisc-1.0.4.0/neo4cdisc.egg-info/PKG-INFO
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      440 2023-02-03 09:50:36.000000 neo4cdisc-1.0.4.0/neo4cdisc.egg-info/SOURCES.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)        1 2023-02-03 09:50:36.000000 neo4cdisc-1.0.4.0/neo4cdisc.egg-info/dependency_links.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       17 2023-02-03 09:50:36.000000 neo4cdisc-1.0.4.0/neo4cdisc.egg-info/requires.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       42 2023-02-03 09:50:36.000000 neo4cdisc-1.0.4.0/neo4cdisc.egg-info/top_level.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       17 2023-02-03 09:47:58.000000 neo4cdisc-1.0.4.0/requirements.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       38 2023-02-03 09:50:37.015704 neo4cdisc-1.0.4.0/setup.cfg
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     2172 2023-02-03 08:40:07.000000 neo4cdisc-1.0.4.0/setup.py
+drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:29:44.470901 neo4cdisc-1.0.5.0/
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    11357 2023-01-18 16:45:48.000000 neo4cdisc-1.0.5.0/LICENSE
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    13355 2023-06-02 14:29:44.466901 neo4cdisc-1.0.5.0/PKG-INFO
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1088 2023-02-03 08:40:07.000000 neo4cdisc-1.0.5.0/README.md
+drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:29:44.442901 neo4cdisc-1.0.5.0/cdisc_data_providers/
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       69 2023-01-18 16:45:48.000000 neo4cdisc-1.0.5.0/cdisc_data_providers/__init__.py
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    11169 2023-01-18 16:45:48.000000 neo4cdisc-1.0.5.0/cdisc_data_providers/sdtm_data_provider.py
+drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:29:44.450901 neo4cdisc-1.0.5.0/cdisc_model_managers/
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      126 2023-02-03 08:40:07.000000 neo4cdisc-1.0.5.0/cdisc_model_managers/__init__.py
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1044 2023-02-03 08:40:07.000000 neo4cdisc-1.0.5.0/cdisc_model_managers/cdisc_api.py
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    21929 2023-02-03 08:40:07.000000 neo4cdisc-1.0.5.0/cdisc_model_managers/cdisc_model_manager.py
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    18806 2023-01-18 16:45:48.000000 neo4cdisc-1.0.5.0/cdisc_model_managers/cdisc_standard_loader.py
+drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:29:44.466901 neo4cdisc-1.0.5.0/neo4cdisc.egg-info/
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    13355 2023-06-02 14:29:44.000000 neo4cdisc-1.0.5.0/neo4cdisc.egg-info/PKG-INFO
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      548 2023-06-02 14:29:44.000000 neo4cdisc-1.0.5.0/neo4cdisc.egg-info/SOURCES.txt
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)        1 2023-06-02 14:29:44.000000 neo4cdisc-1.0.5.0/neo4cdisc.egg-info/dependency_links.txt
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       17 2023-06-02 14:29:44.000000 neo4cdisc-1.0.5.0/neo4cdisc.egg-info/requires.txt
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       42 2023-06-02 14:29:44.000000 neo4cdisc-1.0.5.0/neo4cdisc.egg-info/top_level.txt
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       17 2023-06-02 10:54:27.000000 neo4cdisc-1.0.5.0/requirements.txt
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       38 2023-06-02 14:29:44.470901 neo4cdisc-1.0.5.0/setup.cfg
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     2172 2023-06-02 10:54:20.000000 neo4cdisc-1.0.5.0/setup.py
+drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:29:44.466901 neo4cdisc-1.0.5.0/tests/
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     2360 2023-01-18 16:45:48.000000 neo4cdisc-1.0.5.0/tests/test_cdisc_model_manager.py
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     7150 2023-01-18 16:45:48.000000 neo4cdisc-1.0.5.0/tests/test_sdtm_data_provider.py
+-rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      659 2023-01-18 16:45:48.000000 neo4cdisc-1.0.5.0/tests/test_sdtm_data_provider_dfcheck.py
```

### Comparing `neo4cdisc-1.0.4.0/LICENSE` & `neo4cdisc-1.0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.4.0/PKG-INFO` & `neo4cdisc-1.0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4cdisc
-Version: 1.0.4.0
+Version: 1.0.5.0
 Summary: Clinical Linked Data: Example of loading the FDA CDISC pilot study into Neo4J using the tab2neo python package
 Author: Alexey Kuznetsov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `neo4cdisc-1.0.4.0/README.md` & `neo4cdisc-1.0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.4.0/cdisc_data_providers/sdtm_data_provider.py` & `neo4cdisc-1.0.5.0/cdisc_data_providers/sdtm_data_provider.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.4.0/cdisc_model_managers/cdisc_api.py` & `neo4cdisc-1.0.5.0/cdisc_model_managers/cdisc_api.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.4.0/cdisc_model_managers/cdisc_model_manager.py` & `neo4cdisc-1.0.5.0/cdisc_model_managers/cdisc_model_manager.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.4.0/cdisc_model_managers/cdisc_standard_loader.py` & `neo4cdisc-1.0.5.0/cdisc_model_managers/cdisc_standard_loader.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.4.0/neo4cdisc.egg-info/PKG-INFO` & `neo4cdisc-1.0.5.0/neo4cdisc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4cdisc
-Version: 1.0.4.0
+Version: 1.0.5.0
 Summary: Clinical Linked Data: Example of loading the FDA CDISC pilot study into Neo4J using the tab2neo python package
 Author: Alexey Kuznetsov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `neo4cdisc-1.0.4.0/setup.py` & `neo4cdisc-1.0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             print('Dependency to a git repository should have the format:')
             print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
     else:
         required.append(line)
 
 setuptools.setup(
     name="neo4cdisc",                           # This is the name of the package
-    version="1.0.4.0",                      # Release.Major Feature.Minor Feature.Bug Fix
+    version="1.0.5.0",                      # Release.Major Feature.Minor Feature.Bug Fix
     author="Alexey Kuznetsov",              # Full name of the author
     description="Clinical Linked Data: Example of loading the FDA CDISC pilot study into Neo4J using the tab2neo python package",
     #long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=[
         "cdisc_model_managers",
         "cdisc_data_providers",
```

