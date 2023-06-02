# Comparing `tmp/cdktf-cdktf-provider-external-6.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-external-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-external-6.0.0.tar", last modified: Tue Apr 18 20:37:46 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-external-6.0.1.tar", last modified: Fri Jun  2 14:01:00 2023, max compression
```

## Comparing `cdktf-cdktf-provider-external-6.0.0.tar` & `cdktf-cdktf-provider-external-6.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39509 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/_jsii/provider-external@6.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/data_external/
--rw-r--r--   0 runner    (1001) docker     (123)    21802 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/data_external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:01:00.072732 cdktf-cdktf-provider-external-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21622 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/_jsii/provider-external@6.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/data_external/
+-rw-r--r--   0 runner    (1001) docker     (123)    21802 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/data_external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:00:47.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:01:00.068731 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-02 14:01:00.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 14:01:00.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:01:00.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:01:00.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 14:01:00.000000 cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-external-6.0.0/LICENSE` & `cdktf-cdktf-provider-external-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-external-6.0.0/PKG-INFO` & `cdktf-cdktf-provider-external-6.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-external
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt external Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-external.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-external.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform external Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform external Provider](https://github.com/terraform-providers/terraform-provider-external)
+* [Terraform external Provider](https://registry.terraform.io/providers/hashicorp/external/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-external/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-external-6.0.0/README.md` & `cdktf-cdktf-provider-external-6.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform external Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform external Provider](https://github.com/terraform-providers/terraform-provider-external)
+* [Terraform external Provider](https://registry.terraform.io/providers/hashicorp/external/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-external/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-external-6.0.0/setup.py` & `cdktf-cdktf-provider-external-6.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-external",
-    "version": "6.0.0",
+    "version": "6.0.1",
     "description": "Prebuilt external Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-external.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -24,25 +24,25 @@
         "cdktf_cdktf_provider_external",
         "cdktf_cdktf_provider_external._jsii",
         "cdktf_cdktf_provider_external.data_external",
         "cdktf_cdktf_provider_external.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_external._jsii": [
-            "provider-external@6.0.0.jsii.tgz"
+            "provider-external@6.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_external": [
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

### Comparing `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/__init__.py` & `cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform external Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform external Provider](https://github.com/terraform-providers/terraform-provider-external)
+* [Terraform external Provider](https://registry.terraform.io/providers/hashicorp/external/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-external/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/data_external/__init__.py` & `cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/data_external/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/provider/__init__.py` & `cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO` & `cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-external
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt external Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-external.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-external.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform external Provider version 1:1. In fact, it always tracks `latest` of `~> 2.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform external Provider](https://github.com/terraform-providers/terraform-provider-external)
+* [Terraform external Provider](https://registry.terraform.io/providers/hashicorp/external/2.1.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-external/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-external-6.0.1/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/cdktf_cdktf_provider_external/py.typed
 src/cdktf_cdktf_provider_external.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_external.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_external.egg-info/requires.txt
 src/cdktf_cdktf_provider_external.egg-info/top_level.txt
 src/cdktf_cdktf_provider_external/_jsii/__init__.py
-src/cdktf_cdktf_provider_external/_jsii/provider-external@6.0.0.jsii.tgz
+src/cdktf_cdktf_provider_external/_jsii/provider-external@6.0.1.jsii.tgz
 src/cdktf_cdktf_provider_external/data_external/__init__.py
 src/cdktf_cdktf_provider_external/provider/__init__.py
```

