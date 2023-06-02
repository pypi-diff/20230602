# Comparing `tmp/chaostoolkit-terraform-0.0.5.tar.gz` & `tmp/chaostoolkit-terraform-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaostoolkit-terraform-0.0.5.tar", last modified: Thu Jun  1 10:41:33 2023, max compression
+gzip compressed data, was "chaostoolkit-terraform-0.0.6.tar", last modified: Fri Jun  2 11:01:15 2023, max compression
```

## Comparing `chaostoolkit-terraform-0.0.5.tar` & `chaostoolkit-terraform-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4381 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/chaostf/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-01 10:41:28.000000 chaostoolkit-terraform-0.0.5/chaostf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/chaostf/actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/chaostf/control.py
--rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/chaostf/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4381 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-01 10:41:33.000000 chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-01 10:41:28.000000 chaostoolkit-terraform-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:41:33.903086 chaostoolkit-terraform-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-01 10:41:13.000000 chaostoolkit-terraform-0.0.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/chaosterraform/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-02 11:01:09.000000 chaostoolkit-terraform-0.0.6/chaosterraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3399 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/chaosterraform/control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/chaosterraform/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 11:01:15.000000 chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-02 11:01:09.000000 chaostoolkit-terraform-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 11:01:15.641268 chaostoolkit-terraform-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/tests/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-02 11:00:53.000000 chaostoolkit-terraform-0.0.6/tests/test_version.py
```

### Comparing `chaostoolkit-terraform-0.0.5/LICENSE` & `chaostoolkit-terraform-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.5/PKG-INFO` & `chaostoolkit-terraform-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: chaostoolkit-terraform
-Version: 0.0.5
-Summary: A Chaos Toolkit module to deploy terraform stacks
-Author: Manuel Castellin
-Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # chaostoolkit-terraform
 
 A [Chaos Toolkit](https://chaostoolkit.org/) driver to extend chaos experiments with [Terraform](https://www.terraform.io/)
 
 ## Package Installation
 
 ### From Python package index
@@ -27,33 +18,33 @@
 
 ```shell
 pip install -U "git+https://github.com/mcastellin/chaostoolkit-terraform.git#egg=chaostoolkit-terraform"
 ```
 
 ## Usage
 
-**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaostf.control` for your experiments
+**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaosterraform.control` for your experiments
 you need to define it in your experiment files (or settings):
 
 ```yaml
 title: My experiment
 description: ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 
 steady-state-hypothesis: {...}
 
 method: []
 ```
 
-By default the `chaostf.control` will reference the Terraform module found in the current working directory.
+By default the `chaosterraform.control` will reference the Terraform module found in the current working directory.
 
 The control will execute Terraform command in the following phases of the experiment execution:
 
 | Phase                 | Actions |
 | --------------------- | ------- |
 | **Configure control** | Initialize the Terraform driver |
 | **Before experiment** | Initialize and apply the selected Terraform module |
@@ -65,32 +56,32 @@
 
 **Configuration with control arguments**
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
       arguments:
         silent: false
         retain: true
 ```
 
 **Configuration using Ctk parameters**
 ```yaml
 configuration:
-# parameters prefixed with `tf_conf__` will configure chaostf driver
+# parameters prefixed with `tf_conf__` will configure chaosterraform driver
   tf_conf__silent: false
   tf_conf__retain: true
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 ```
 
 > When both options are supplied **configuration parameters supplied via the experiment configuration will
 > be used**.
 
 
 | Parameter Name        | Usage |
@@ -111,15 +102,15 @@
   tf__number_of_azs: 2
   ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 ```
 
 
 ## Use Terraform Outputs In Chaos Experiments
 
 If your Terraform module exports some output variables you can use them in the Chaos Toolkit experiments
 as regular experiment parameters. Such variables are added to the configuration context with the `tf_out__` prefix.
@@ -139,15 +130,15 @@
 We can use the exported DNS name in our chaos experiment like so:
 
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 
 steady-state-hypothesis:
   title: "Application is available"
   probes:
     - type: probe
       name: "should-respond-200"
       tolerance: 200
```

### Comparing `chaostoolkit-terraform-0.0.5/README.md` & `chaostoolkit-terraform-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: chaostoolkit-terraform
+Version: 0.0.6
+Summary: A Chaos Toolkit module to deploy terraform stacks
+Author: Manuel Castellin
+Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # chaostoolkit-terraform
 
 A [Chaos Toolkit](https://chaostoolkit.org/) driver to extend chaos experiments with [Terraform](https://www.terraform.io/)
 
 ## Package Installation
 
 ### From Python package index
@@ -18,33 +27,33 @@
 
 ```shell
 pip install -U "git+https://github.com/mcastellin/chaostoolkit-terraform.git#egg=chaostoolkit-terraform"
 ```
 
 ## Usage
 
-**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaostf.control` for your experiments
+**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaosterraform.control` for your experiments
 you need to define it in your experiment files (or settings):
 
 ```yaml
 title: My experiment
 description: ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 
 steady-state-hypothesis: {...}
 
 method: []
 ```
 
-By default the `chaostf.control` will reference the Terraform module found in the current working directory.
+By default the `chaosterraform.control` will reference the Terraform module found in the current working directory.
 
 The control will execute Terraform command in the following phases of the experiment execution:
 
 | Phase                 | Actions |
 | --------------------- | ------- |
 | **Configure control** | Initialize the Terraform driver |
 | **Before experiment** | Initialize and apply the selected Terraform module |
@@ -56,32 +65,32 @@
 
 **Configuration with control arguments**
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
       arguments:
         silent: false
         retain: true
 ```
 
 **Configuration using Ctk parameters**
 ```yaml
 configuration:
-# parameters prefixed with `tf_conf__` will configure chaostf driver
+# parameters prefixed with `tf_conf__` will configure chaosterraform driver
   tf_conf__silent: false
   tf_conf__retain: true
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 ```
 
 > When both options are supplied **configuration parameters supplied via the experiment configuration will
 > be used**.
 
 
 | Parameter Name        | Usage |
@@ -102,15 +111,15 @@
   tf__number_of_azs: 2
   ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 ```
 
 
 ## Use Terraform Outputs In Chaos Experiments
 
 If your Terraform module exports some output variables you can use them in the Chaos Toolkit experiments
 as regular experiment parameters. Such variables are added to the configuration context with the `tf_out__` prefix.
@@ -130,15 +139,15 @@
 We can use the exported DNS name in our chaos experiment like so:
 
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 
 steady-state-hypothesis:
   title: "Application is available"
   probes:
     - type: probe
       name: "should-respond-200"
       tolerance: 200
```

### Comparing `chaostoolkit-terraform-0.0.5/chaostf/__init__.py` & `chaostoolkit-terraform-0.0.6/chaosterraform/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-"""Top-level package for chaostf"""
+"""Top-level package for chaosterraform"""
 from typing import List
 
-from chaoslib.discovery.discover import (
-    discover_actions,
-    discover_activities,
-    discover_probes,
-    initialize_discovery_result,
-)
+from chaoslib.discovery.discover import discover_actions, discover_activities, initialize_discovery_result
 from chaoslib.types import DiscoveredActivities, Discovery
-from logzero import logger
 
-name = "chaostf"
+name = "chaosterraform"
 __author__ = """Manuel Castellin"""
 __email__ = "manuel@castellinconsulting.com"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 __all__ = [
     "discover",
     "__version__",
 ]
 
 
 def discover(discover_system: bool = True) -> Discovery:
+    """Discover chaostoolkit activities"""
     # pylint: disable=unused-argument
-    discovery = initialize_discovery_result("chaostf", __version__, "chaostf")
+    discovery = initialize_discovery_result("chaosterraform", __version__, "chaosterraform")
     discovery["activities"].extend(load_exported_activities())
     return discovery
 
 
 def load_exported_activities() -> List[DiscoveredActivities]:
     """
     Extract metadata from actions and probes exposed by this extension.
     """
     activities = []
-    activities.extend(discover_actions("chaostf.actions"))
-    activities.extend(discover_activities("chaostf.control", "control"))
+    activities.extend(discover_actions("chaosterraform.actions"))
+    activities.extend(discover_activities("chaosterraform.control", "control"))
 
     return activities
```

### Comparing `chaostoolkit-terraform-0.0.5/chaostf/control.py` & `chaostoolkit-terraform-0.0.6/chaosterraform/control.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,92 @@
-from typing import Any, Dict, List
+"""
+Terraform control module
 
-from chaoslib.exceptions import InterruptExecution
-from chaoslib.types import (
-    Activity,
-    Configuration,
-    Experiment,
-    Hypothesis,
-    Journal,
-    Run,
-    Secrets,
-    Settings,
-)
+This module allows Chaos Toolkit users to create infrastructure resources using Terraform scripts
+for the experiment execution.
+"""
+from chaoslib.types import Configuration, Experiment, Journal, Secrets, Settings
 from logzero import logger
 
 from .driver import Terraform
 
 VAR_NAME_PREFIX = "tf__"
 CONFIG_PREFIX = "tf_conf__"
 EXPORT_VAR_PREFIX = "tf_out__"
 
 
 def configure_control(
     silent: bool = True,
     retain: bool = False,
+    chdir: str = None,
     configuration: Configuration = None,
     secrets: Secrets = None,
     settings: Settings = None,
     experiment: Experiment = None,
 ):
+    """
+    Configure terraform control for the experiment execution
+
+    Parameters
+    ----------
+    silent: bool
+        suppress Terraform logs in ChaosToolkit experiment logs
+    retain: bool
+        retain created resources at the end of the experiment
+    chdir: str
+        change the Terraform working directory
+
+    Raises
+    ------
+    InterruptExecution
+        If terraform init fails we interrupt the experiment execution immediately
+    """
+    # pylint: disable=unused-argument
     tf_vars = {}
     if configuration:
         for key, value in configuration.items():
             if key.startswith(VAR_NAME_PREFIX):
                 tf_key = key.replace(VAR_NAME_PREFIX, "")
                 tf_vars[tf_key] = value
 
     for key, _ in tf_vars.items():
         configuration.pop(f"{VAR_NAME_PREFIX}{key}")
 
     params = {
         "retain": bool(configuration.get(f"{CONFIG_PREFIX}retain", retain)),
         "silent": bool(configuration.get(f"{CONFIG_PREFIX}silent", silent)),
+        "chdir": configuration.get(f"{CONFIG_PREFIX}chdir", chdir),
     }
     logger.info(
         "Terraform: retain stack after experiment completion: %s",
         str(params.get("retain")),
     )
 
-    driver = Terraform()
-    driver.configure(**params, args=tf_vars)
+    driver = Terraform(**params, args=tf_vars)
     driver.terraform_init()
 
 
 def before_experiment_control(
     context: Experiment,
     configuration: Configuration = None,
     secrets: Secrets = None,
     **kwargs,
 ):
     """
     before-control of the experiment's execution
 
-    Called by the Chaos Toolkit before the experiment's begin but after the
-    configuration and secrets have been loaded.
+    Apply the Terraform stack before the experiment execution. As the experiment did not start
+    yet, if the resources creation fails the execution is interrupted immediately.
+
+    Raises
+    ------
+    InterruptExecution
+        interrupts the experiment execution if resources creation fails
     """
+    # pylint: disable=unused-argument
     driver = Terraform()
     logger.info("Terraform: creating required resources for experiment")
     driver.apply()
     for key, value in driver.output().items():
         logger.info("Terraform: reading configuration value for [%s]", key)
         configuration[f"{EXPORT_VAR_PREFIX}{key}"] = value.get("value")
 
@@ -75,15 +94,20 @@
 def after_experiment_control(
     context: Experiment,
     state: Journal,
     configuration: Configuration = None,
     secrets: Secrets = None,
     **kwargs,
 ):
+    """
+    after-control of the experiment's execution
+
+    Destroy resources after the experiment execution unless retain specifically requested by
+    the experiment using the `retain` parameter
+    """
+    # pylint: disable=unused-argument
     driver = Terraform()
     if not driver.retain:
         logger.info("Terraform: removing experiment resources")
         driver.destroy()
     else:
-        logger.info(
-            "Terraform: stack resources will be retained after experiment completion."
-        )
+        logger.info("Terraform: stack resources will be retained after experiment completion.")
```

### Comparing `chaostoolkit-terraform-0.0.5/chaostoolkit_terraform.egg-info/PKG-INFO` & `chaostoolkit-terraform-0.0.6/chaostoolkit_terraform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-terraform
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Chaos Toolkit module to deploy terraform stacks
 Author: Manuel Castellin
 Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chaostoolkit-terraform
@@ -27,33 +27,33 @@
 
 ```shell
 pip install -U "git+https://github.com/mcastellin/chaostoolkit-terraform.git#egg=chaostoolkit-terraform"
 ```
 
 ## Usage
 
-**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaostf.control` for your experiments
+**chaostoolkit-terraform** provides a control to deploy terraform modules. To activate the `chaosterraform.control` for your experiments
 you need to define it in your experiment files (or settings):
 
 ```yaml
 title: My experiment
 description: ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 
 steady-state-hypothesis: {...}
 
 method: []
 ```
 
-By default the `chaostf.control` will reference the Terraform module found in the current working directory.
+By default the `chaosterraform.control` will reference the Terraform module found in the current working directory.
 
 The control will execute Terraform command in the following phases of the experiment execution:
 
 | Phase                 | Actions |
 | --------------------- | ------- |
 | **Configure control** | Initialize the Terraform driver |
 | **Before experiment** | Initialize and apply the selected Terraform module |
@@ -65,32 +65,32 @@
 
 **Configuration with control arguments**
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
       arguments:
         silent: false
         retain: true
 ```
 
 **Configuration using Ctk parameters**
 ```yaml
 configuration:
-# parameters prefixed with `tf_conf__` will configure chaostf driver
+# parameters prefixed with `tf_conf__` will configure chaosterraform driver
   tf_conf__silent: false
   tf_conf__retain: true
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 ```
 
 > When both options are supplied **configuration parameters supplied via the experiment configuration will
 > be used**.
 
 
 | Parameter Name        | Usage |
@@ -111,15 +111,15 @@
   tf__number_of_azs: 2
   ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 ```
 
 
 ## Use Terraform Outputs In Chaos Experiments
 
 If your Terraform module exports some output variables you can use them in the Chaos Toolkit experiments
 as regular experiment parameters. Such variables are added to the configuration context with the `tf_out__` prefix.
@@ -139,15 +139,15 @@
 We can use the exported DNS name in our chaos experiment like so:
 
 ```yaml
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
-      module: chaostf.control
+      module: chaosterraform.control
 
 steady-state-hypothesis:
   title: "Application is available"
   probes:
     - type: probe
       name: "should-respond-200"
       tolerance: 200
```

