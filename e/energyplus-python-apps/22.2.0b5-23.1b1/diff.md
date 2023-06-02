# Comparing `tmp/energyplus_python_apps-22.2.0b5.tar.gz` & `tmp/energyplus_python_apps-23.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_python_apps-22.2.0b5.tar", last modified: Tue Nov 22 14:01:17 2022, max compression
+gzip compressed data, was "energyplus_python_apps-23.1b1.tar", last modified: Fri Jun  2 21:39:29 2023, max compression
```

## Comparing `energyplus_python_apps-22.2.0b5.tar` & `energyplus_python_apps-23.1b1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:01:17.738038 energyplus_python_apps-22.2.0b5/
--rw-r--r--   0 runner    (1001) docker     (122)     3099 2022-11-22 14:01:17.738038 energyplus_python_apps-22.2.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2476 2022-11-22 14:01:13.000000 energyplus_python_apps-22.2.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:01:17.738038 energyplus_python_apps-22.2.0b5/energyplus_python_apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 14:01:13.000000 energyplus_python_apps-22.2.0b5/energyplus_python_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:01:17.738038 energyplus_python_apps-22.2.0b5/energyplus_python_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3099 2022-11-22 14:01:17.000000 energyplus_python_apps-22.2.0b5/energyplus_python_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      282 2022-11-22 14:01:17.000000 energyplus_python_apps-22.2.0b5/energyplus_python_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 14:01:17.000000 energyplus_python_apps-22.2.0b5/energyplus_python_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2022-11-22 14:01:17.000000 energyplus_python_apps-22.2.0b5/energyplus_python_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-11-22 14:01:17.000000 energyplus_python_apps-22.2.0b5/energyplus_python_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 14:01:17.738038 energyplus_python_apps-22.2.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      946 2022-11-22 14:01:13.000000 energyplus_python_apps-22.2.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/energyplus_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/energyplus_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      763 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/energyplus_python_apps/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 21:39:29.000000 energyplus_python_apps-23.1b1/energyplus_python_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 21:39:29.796290 energyplus_python_apps-23.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-06-02 21:39:26.000000 energyplus_python_apps-23.1b1/setup.py
```

### Comparing `energyplus_python_apps-22.2.0b5/PKG-INFO` & `energyplus_python_apps-23.1b1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-Metadata-Version: 2.1
-Name: energyplus_python_apps
-Version: 22.2.0b5
-Summary: Meta-package collecting all official EnergyPlus Python utilities
-Home-page: https://github.com/Myoldmopar/EnergyPlusPythonApps
-Author: Edwin Lee, for NREL, for United States Department of Energy
-Author-email: a@a.a
-License: UnlicensedForNow
-Description: # EnergyPlus Python Apps
-        
-        This is a meta-project which simply depends on all the EnergyPlus "Official" Python utilities.
-        This project itself does not create any new utilities, or contain any code.
-        This really just pins the dependencies at specific versions and ensures compatability in the installation dependencies.
-        
-        ## Releases
-        
-        [![PyPIRelease](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/release.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/release.yml)
-        
-        I think long term, this "project" itself will be tagged with versions in sync with EnergyPlus itself.
-        To install all EnergyPlus Python utilities, simply execute, for example,  `pip install energyplus_python_apps==22.2.0`.
-        
-        ## Current Repos
-        
-        This project is currently linking to the following packages:
-        
-        | PyPi Project Name            | Project Description                                                                  | Repository                                                   |
-        |------------------------------|--------------------------------------------------------------------------------------|--------------------------------------------------------------|
-        | energyplus-launch            | A graphical interface and workflow manager for EnergyPlus                            | https://github.com/NREL/EP-Launch                            |
-        | energyplus-ruleset-model     | A utility for generating ruleset model reports from EnergyPlus inputs and outputs    | https://github.com/jasonglazer/createrulesetmodeldescription |
-        | energyplus-transition-tools  | A lightweight interface for automatically transitioning EnergyPlus input files       | https://github.com/Myoldmopar/EnergyPlusTransitionTools      |
-        | energyplus-pet               | A library and graphical tool for generating input coefficients for EnergyPlus models | https://github.com/Myoldmopar/energypluspet                  |
-        | energyplus-idd-idf-utilities | A lightweight library for processing and querying idd and idf files                  | https://github.com/Myoldmopar/py-idd-idf                     |
-        | energyplus-regressions       | A tool for comparing results from two EnergyPlus builds, for E+ developer usage      | https://github.com/NREL/EnergyPlusRegressionTool             |
-        | energyplus-api-helpers       | A set of helper classes and demos for interacting with the EnergyPlus API            | https://github.com/Myoldmopar/EnergyPlusAPIDemos             |
-        
-        
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# EnergyPlus Python Apps
+
+This is a meta-project which simply depends on all the EnergyPlus "Official" Python utilities.
+This project itself does not create any new utilities, or contain any code.
+This really just pins the dependencies at specific versions and ensures compatability in the installation dependencies.
+
+## Releases
+
+[![DevelopmentTest](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/test.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/test.yml)
+[![PyPIRelease](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/release.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/release.yml)
+
+I think long term, this "project" itself will be tagged with versions in sync with EnergyPlus itself.
+To install all EnergyPlus Python utilities, simply execute, for example,  `pip install energyplus_python_apps==22.2.0`.
+
+## Current Repos
+
+This project is currently linking to the following packages:
+
+| PyPi Project Name            | Project Description                                                                  | Repository                                                   |
+|------------------------------|--------------------------------------------------------------------------------------|--------------------------------------------------------------|
+| energyplus-launch            | A graphical interface and workflow manager for EnergyPlus                            | https://github.com/NREL/EP-Launch                            |
+| energyplus-ruleset-model     | A utility for generating ruleset model reports from EnergyPlus inputs and outputs    | https://github.com/jasonglazer/createrulesetmodeldescription |
+| energyplus-transition-tools  | A lightweight interface for automatically transitioning EnergyPlus input files       | https://github.com/Myoldmopar/EnergyPlusTransitionTools      |
+| energyplus-pet               | A library and graphical tool for generating input coefficients for EnergyPlus models | https://github.com/Myoldmopar/energypluspet                  |
+| energyplus-idd-idf-utilities | A lightweight library for processing and querying idd and idf files                  | https://github.com/Myoldmopar/py-idd-idf                     |
+| energyplus-regressions       | A tool for comparing results from two EnergyPlus builds, for E+ developer usage      | https://github.com/NREL/EnergyPlusRegressionTool             |
+| energyplus-api-helpers       | A set of helper classes and demos for interacting with the EnergyPlus API            | https://github.com/Myoldmopar/EnergyPlusAPIHelper            |
+| energyplus-diff-analysis     | Tools for plotting and comparing csv data from two separate EnergyPlus runs          | https://github.com/mitchute/energyplus-diff-analysis         |
+
+## Usage
+
+Cover a few topics here:
+ - Installation
+ - Running the configuration script after install
+ - Accessing all the tools, including the dev tools
+ - Updating
```

### Comparing `energyplus_python_apps-22.2.0b5/energyplus_python_apps.egg-info/PKG-INFO` & `energyplus_python_apps-23.1b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: energyplus-python-apps
-Version: 22.2.0b5
+Name: energyplus_python_apps
+Version: 23.1b1
 Summary: Meta-package collecting all official EnergyPlus Python utilities
 Home-page: https://github.com/Myoldmopar/EnergyPlusPythonApps
 Author: Edwin Lee, for NREL, for United States Department of Energy
-Author-email: a@a.a
-License: UnlicensedForNow
+License: ModifiedBSD
 Description: # EnergyPlus Python Apps
         
         This is a meta-project which simply depends on all the EnergyPlus "Official" Python utilities.
         This project itself does not create any new utilities, or contain any code.
         This really just pins the dependencies at specific versions and ensures compatability in the installation dependencies.
         
         ## Releases
         
+        [![DevelopmentTest](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/test.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/test.yml)
         [![PyPIRelease](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/release.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusPythonApps/actions/workflows/release.yml)
         
         I think long term, this "project" itself will be tagged with versions in sync with EnergyPlus itself.
         To install all EnergyPlus Python utilities, simply execute, for example,  `pip install energyplus_python_apps==22.2.0`.
         
         ## Current Repos
         
@@ -27,14 +27,19 @@
         |------------------------------|--------------------------------------------------------------------------------------|--------------------------------------------------------------|
         | energyplus-launch            | A graphical interface and workflow manager for EnergyPlus                            | https://github.com/NREL/EP-Launch                            |
         | energyplus-ruleset-model     | A utility for generating ruleset model reports from EnergyPlus inputs and outputs    | https://github.com/jasonglazer/createrulesetmodeldescription |
         | energyplus-transition-tools  | A lightweight interface for automatically transitioning EnergyPlus input files       | https://github.com/Myoldmopar/EnergyPlusTransitionTools      |
         | energyplus-pet               | A library and graphical tool for generating input coefficients for EnergyPlus models | https://github.com/Myoldmopar/energypluspet                  |
         | energyplus-idd-idf-utilities | A lightweight library for processing and querying idd and idf files                  | https://github.com/Myoldmopar/py-idd-idf                     |
         | energyplus-regressions       | A tool for comparing results from two EnergyPlus builds, for E+ developer usage      | https://github.com/NREL/EnergyPlusRegressionTool             |
-        | energyplus-api-helpers       | A set of helper classes and demos for interacting with the EnergyPlus API            | https://github.com/Myoldmopar/EnergyPlusAPIDemos             |
-        
-        
+        | energyplus-api-helpers       | A set of helper classes and demos for interacting with the EnergyPlus API            | https://github.com/Myoldmopar/EnergyPlusAPIHelper            |
+        | energyplus-diff-analysis     | Tools for plotting and comparing csv data from two separate EnergyPlus runs          | https://github.com/mitchute/energyplus-diff-analysis         |
         
+        ## Usage
         
+        Cover a few topics here:
+         - Installation
+         - Running the configuration script after install
+         - Accessing all the tools, including the dev tools
+         - Updating
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `energyplus_python_apps-22.2.0b5/setup.py` & `energyplus_python_apps-23.1b1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import pathlib
 from setuptools import setup
 
+from energyplus_python_apps import NAME, VERSION
+
 readme_file = pathlib.Path(__file__).parent.resolve() / 'README.md'
 readme_contents = readme_file.read_text()
 
 setup(
-    name="energyplus_python_apps",
-    version="22.2.0-Beta5",
+    name=NAME,
+    version=VERSION,
     packages=['energyplus_python_apps'],
     description="Meta-package collecting all official EnergyPlus Python utilities",
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     author='Edwin Lee, for NREL, for United States Department of Energy',
-    author_email='a@a.a',
     url='https://github.com/Myoldmopar/EnergyPlusPythonApps',
-    license='UnlicensedForNow',
+    license='ModifiedBSD',
     install_requires=[
-        'energyplus-launch==3.5.3',
-        'energyplus-ruleset-model==0.2',
-        'energyplus-transition-tools==2.0.3',
-        'energyplus-pet==0.43',
-        'energyplus-idd-idf-utilities==0.86',
-        'energyplus-regressions==1.9.7',
-        'energyplus-api-helpers==0.2',
-    ]
+        'energyplus-launch==3.6.9',
+        'energyplus-ruleset-model==0.5',
+        'energyplus-transition-tools==2.0.8',
+        'energyplus-pet==0.49',
+        'energyplus-idd-idf-utilities==0.88',
+        'energyplus-regressions==2.0.3',
+        'energyplus-api-helpers==0.4',
+        'energyplus-diff-analysis==0.2',
+        # 'energyplus-expand-objects==blah',
+        # 'energyplus-epjson-editor==blah',
+    ],
+    entry_points={
+        'console_scripts': [
+            'energyplus_python_configure=energyplus_python_apps.configure:configure_cli',
+        ]
+    }
 )
```

