# Comparing `tmp/cdktf-cdktf-provider-hashicups-4.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-hashicups-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-hashicups-4.0.0.tar", last modified: Tue Apr 18 20:45:11 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-hashicups-4.0.1.tar", last modified: Fri Jun  2 14:04:48 2023, max compression
```

## Comparing `cdktf-cdktf-provider-hashicups-4.0.0.tar` & `cdktf-cdktf-provider-hashicups-4.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)    16012 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     4213 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3249 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2166 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/
--rw-r--r--   0 runner    (1000) runner    (1000)     3840 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/
--rw-r--r--   0 runner    (1000) runner    (1000)      421 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   157027 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@4.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/
--rw-r--r--   0 runner    (1000) runner    (1000)    34892 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/
--rw-r--r--   0 runner    (1000) runner    (1000)    27655 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/
--rw-r--r--   0 runner    (1000) runner    (1000)    25501 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/order/
--rw-r--r--   0 runner    (1000) runner    (1000)    40851 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/order/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.030970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/provider/
--rw-r--r--   0 runner    (1000) runner    (1000)    12334 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/provider/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-18 20:44:59.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-18 20:45:11.026970 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     4213 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      882 2023-04-18 20:45:11.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      106 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       31 2023-04-18 20:45:10.000000 cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16012 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     4384 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3420 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2166 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.951007 cdktf-cdktf-provider-hashicups-4.0.1/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.951007 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4011 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/_jsii/
+-rw-r--r--   0 runner    (1000) runner    (1000)      421 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/_jsii/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41346 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@4.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/
+-rw-r--r--   0 runner    (1000) runner    (1000)    34892 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/
+-rw-r--r--   0 runner    (1000) runner    (1000)    27655 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    25501 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/order/
+-rw-r--r--   0 runner    (1000) runner    (1000)    40851 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/order/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/provider/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12334 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/provider/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 14:04:32.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 14:04:48.955006 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4384 2023-06-02 14:04:48.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      882 2023-06-02 14:04:48.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 14:04:48.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      106 2023-06-02 14:04:48.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2023-06-02 14:04:48.000000 cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/LICENSE` & `cdktf-cdktf-provider-hashicups-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/PKG-INFO` & `cdktf-cdktf-provider-hashicups-4.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hashicups
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt hashicups Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hashicups.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hashicups.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hashicups Provider](https://github.com/terraform-providers/terraform-provider-hashicups)
+* [Terraform hashicups Provider](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hashicups/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/README.md` & `cdktf-cdktf-provider-hashicups-4.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hashicups Provider](https://github.com/terraform-providers/terraform-provider-hashicups)
+* [Terraform hashicups Provider](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hashicups/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/setup.py` & `cdktf-cdktf-provider-hashicups-4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-hashicups",
-    "version": "4.0.0",
+    "version": "4.0.1",
     "description": "Prebuilt hashicups Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-hashicups.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -27,25 +27,25 @@
         "cdktf_cdktf_provider_hashicups.data_hashicups_ingredients",
         "cdktf_cdktf_provider_hashicups.data_hashicups_order",
         "cdktf_cdktf_provider_hashicups.order",
         "cdktf_cdktf_provider_hashicups.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_hashicups._jsii": [
-            "provider-hashicups@4.0.0.jsii.tgz"
+            "provider-hashicups@4.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_hashicups": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.0, <0.17.0",
+        "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hashicups Provider](https://github.com/terraform-providers/terraform-provider-hashicups)
+* [Terraform hashicups Provider](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hashicups/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/order/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/order/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups/provider/__init__.py` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hashicups
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt hashicups Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hashicups.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hashicups.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform hashicups Provider version 1:1. In fact, it always tracks `latest` of `~> 0.3` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform hashicups Provider](https://github.com/terraform-providers/terraform-provider-hashicups)
+* [Terraform hashicups Provider](https://registry.terraform.io/providers/hashicorp/hashicups/0.3.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-hashicups/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-hashicups-4.0.0/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-hashicups-4.0.1/src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/cdktf_cdktf_provider_hashicups/py.typed
 src/cdktf_cdktf_provider_hashicups.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_hashicups.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_hashicups.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_hashicups.egg-info/requires.txt
 src/cdktf_cdktf_provider_hashicups.egg-info/top_level.txt
 src/cdktf_cdktf_provider_hashicups/_jsii/__init__.py
-src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@4.0.0.jsii.tgz
+src/cdktf_cdktf_provider_hashicups/_jsii/provider-hashicups@4.0.1.jsii.tgz
 src/cdktf_cdktf_provider_hashicups/data_hashicups_coffees/__init__.py
 src/cdktf_cdktf_provider_hashicups/data_hashicups_ingredients/__init__.py
 src/cdktf_cdktf_provider_hashicups/data_hashicups_order/__init__.py
 src/cdktf_cdktf_provider_hashicups/order/__init__.py
 src/cdktf_cdktf_provider_hashicups/provider/__init__.py
```

