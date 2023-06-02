# Comparing `tmp/chaostoolkit-terraform-0.0.6.tar.gz` & `tmp/chaostoolkit-terraform-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaostoolkit-terraform-0.0.6.tar", last modified: Fri Jun  2 11:01:15 2023, max compression
+gzip compressed data, was "chaostoolkit-terraform-0.0.7.tar", last modified: Fri Jun  2 18:16:50 2023, max compression
```

## Comparing `chaostoolkit-terraform-0.0.6.tar` & `chaostoolkit-terraform-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/chaosterraform/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-02 11:01:09.000000 chaostoolkit-terraform-0.0.6/chaosterraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3399 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/chaosterraform/control.py
--rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/chaosterraform/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-02 11:01:09.000000 chaostoolkit-terraform-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/tests/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.939037 chaostoolkit-terraform-0.0.7/chaosterraform/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-02 18:16:45.000000 chaostoolkit-terraform-0.0.7/chaosterraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3399 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/chaosterraform/control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4606 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/chaosterraform/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-02 18:16:45.000000 chaostoolkit-terraform-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/tests/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/tests/test_version.py
```

### Comparing `chaostoolkit-terraform-0.0.6/LICENSE` & `chaostoolkit-terraform-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.6/PKG-INFO` & `chaostoolkit-terraform-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-terraform
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Chaos Toolkit module to deploy terraform stacks
 Author: Manuel Castellin
 Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chaostoolkit-terraform
```

### Comparing `chaostoolkit-terraform-0.0.6/README.md` & `chaostoolkit-terraform-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.6/chaosterraform/__init__.py` & `chaostoolkit-terraform-0.0.7/chaosterraform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from chaoslib.discovery.discover import discover_actions, discover_activities, initialize_discovery_result
 from chaoslib.types import DiscoveredActivities, Discovery
 
 name = "chaosterraform"
 __author__ = """Manuel Castellin"""
 __email__ = "manuel@castellinconsulting.com"
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __all__ = [
     "discover",
     "__version__",
 ]
 
 
 def discover(discover_system: bool = True) -> Discovery:
```

### Comparing `chaostoolkit-terraform-0.0.6/chaosterraform/control.py` & `chaostoolkit-terraform-0.0.7/chaosterraform/control.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.6/chaosterraform/driver.py` & `chaostoolkit-terraform-0.0.7/chaosterraform/driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import subprocess
 from copy import deepcopy
 from itertools import chain
 from typing import Dict, List
 
 from chaoslib.exceptions import InterruptExecution
+from logzero import logger
 
 
 def _run(*cmd: List[List[str]], capture_output: bool = False, text: bool = False):
     _cmd = list(chain(*cmd))
     return subprocess.run(_cmd, shell=False, capture_output=capture_output, text=text, check=False)
 
 
@@ -83,14 +84,16 @@
         ------
         InterruptExecution
             Interrupts the experiment execution if Terraform modules could not be initialized
         """
         if not os.path.exists(".terraform"):
             result = _run(self._terraform, ["init"], capture_output=self.silent)
             if result.returncode != 0:
+                if self.silent:
+                    logger.error(result.stderr.decode("utf-8"))
                 raise InterruptExecution("Failed to initialize terraform")
 
     def apply(self, **kwargs):
         """
         Apply the Terraform stack
 
         Parameters
@@ -108,23 +111,25 @@
         args.update(kwargs)
 
         var_overrides = []
         for key, value in args.items():
             string_value = value
             if isinstance(value, bool):
                 string_value = str(value).lower()
-            var_overrides.extend(["-var", f"{key}='{string_value}'"])
+            var_overrides.extend(["-var", f"{key}={string_value}"])
 
         result = _run(
             self._terraform,
             ["apply", "-auto-approve"],
             var_overrides,
             capture_output=self.silent,
         )
         if result.returncode != 0:
+            if self.silent:
+                logger.error(result.stderr.decode("utf-8"))
             raise InterruptExecution("Failed to apply terraform stack terraform")
 
     def output(self):
         """
         Reads Terraform stack outputs into a Python dict
 
         Returns
```

### Comparing `chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/PKG-INFO` & `chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-terraform
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Chaos Toolkit module to deploy terraform stacks
 Author: Manuel Castellin
 Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chaostoolkit-terraform
```

### Comparing `chaostoolkit-terraform-0.0.6/pyproject.toml` & `chaostoolkit-terraform-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "chaostoolkit-terraform"
 description = "A Chaos Toolkit module to deploy terraform stacks"
 readme = "README.md"
-version = "0.0.6"
+version = "0.0.7"
 authors = [ { name = "Manuel Castellin" } ]
 dependencies = [
     'chaostoolkit',
     'chaostoolkit-lib',
 ]
 
 [project.urls]
```

### Comparing `chaostoolkit-terraform-0.0.6/tests/test_control.py` & `chaostoolkit-terraform-0.0.7/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.6/tests/test_driver.py` & `chaostoolkit-terraform-0.0.7/tests/test_driver.py`

 * *Files identical despite different names*

