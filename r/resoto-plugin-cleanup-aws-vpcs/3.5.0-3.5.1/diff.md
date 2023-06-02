# Comparing `tmp/resoto-plugin-cleanup-aws-vpcs-3.5.0.tar.gz` & `tmp/resoto-plugin-cleanup-aws-vpcs-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.5.0.tar", last modified: Fri May 26 18:24:14 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.5.1.tar", last modified: Fri Jun  2 14:55:46 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0.tar` & `resoto-plugin-cleanup-aws-vpcs-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:14.444069 resoto-plugin-cleanup-aws-vpcs-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:41.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 18:24:14.444069 resoto-plugin-cleanup-aws-vpcs-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-26 18:21:41.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 18:21:41.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:14.444069 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-26 18:21:41.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-26 18:21:41.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:14.444069 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 18:24:14.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 18:24:14.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:14.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 18:24:14.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:14.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 18:24:14.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 18:24:14.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:24:14.448069 resoto-plugin-cleanup-aws-vpcs-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-26 18:21:41.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:14.444069 resoto-plugin-cleanup-aws-vpcs-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-26 18:21:41.000000 resoto-plugin-cleanup-aws-vpcs-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:46.346669 resoto-plugin-cleanup-aws-vpcs-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:52:13.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-02 14:55:46.346669 resoto-plugin-cleanup-aws-vpcs-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-02 14:52:13.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-02 14:52:13.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:46.346669 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-02 14:52:13.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 14:52:13.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:46.346669 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-02 14:55:46.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-02 14:55:46.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:55:46.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 14:55:46.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:53:46.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 14:55:46.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 14:55:46.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:55:46.350669 resoto-plugin-cleanup-aws-vpcs-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:46.346669 resoto-plugin-cleanup-aws-vpcs-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-02 14:52:13.000000 resoto-plugin-cleanup-aws-vpcs-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.5.0
+Version: 3.5.1
 Summary: AWS VPC Cleaner Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-cleanup-aws-vpcs
 AWS VPC Cleanup Plugin for Resoto
 
 This plugin marks all VPC dependencies for cleanup. The VPC must have been previously marked for cleanup by another cleanup plugin.
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0/README.md` & `resoto-plugin-cleanup-aws-vpcs-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs/__init__.py` & `resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs/config.py` & `resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.5.0
+Version: 3.5.1
 Summary: AWS VPC Cleaner Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-cleanup-aws-vpcs
 AWS VPC Cleanup Plugin for Resoto
 
 This plugin marks all VPC dependencies for cleanup. The VPC must have been previously marked for cleanup by another cleanup plugin.
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-vpcs-3.5.1/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_cleanup_aws_vpcs/__init__.py
 resoto_plugin_cleanup_aws_vpcs/config.py
 resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
 resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
 resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
 resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
 resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.0/setup.py` & `resoto-plugin-cleanup-aws-vpcs-3.5.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-import os
-import pkg_resources
-from setuptools import setup, find_packages
-
-
-def read(file_name: str) -> str:
-    with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
-        return of.read()
-
-
-setup(
-    name="resoto-plugin-cleanup-aws-vpcs",
-    version="3.5.0",
-    description="AWS VPC Cleaner Plugin",
-    license="Apache 2.0",
-    packages=find_packages(),
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    entry_points={"resoto.plugins": ["cleanup_aws_vpcs = resoto_plugin_cleanup_aws_vpcs:CleanupAWSVPCsPlugin"]},
-    include_package_data=True,
-    zip_safe=False,
-    install_requires=[str(requirement) for requirement in pkg_resources.parse_requirements(read("requirements.txt"))],
-    setup_requires=["pytest-runner"],
-    tests_require=["pytest"],
-    classifiers=[
-        # Current project status
-        "Development Status :: 4 - Beta",
-        # Audience
-        "Intended Audience :: System Administrators",
-        "Intended Audience :: Information Technology",
-        # License information
-        "License :: OSI Approved :: Apache Software License",
-        # Supported python versions
-        "Programming Language :: Python :: 3.9",
-        # Supported OS's
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Unix",
-        # Extra metadata
-        "Environment :: Console",
-        "Natural Language :: English",
-        "Topic :: Security",
-        "Topic :: Utilities",
-    ],
-    keywords="cloud security",
-    url="https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs",
-)
+[project]
+name = "resoto-plugin-cleanup-aws-vpcs"
+description = "AWS VPC Cleaner Plugin"
+version = "3.5.1"
+authors = [{name="Some Engineering Inc."}]
+license = {file="LICENSE"}
+requires-python = ">=3.9"
+classifiers = [
+    # Current project status
+    "Development Status :: 4 - Beta",
+    # Audience
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Information Technology",
+    # License information
+    "License :: OSI Approved :: Apache Software License",
+    # Supported python versions
+    "Programming Language :: Python :: 3.9",
+    # Supported OS's
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Unix",
+    # Extra metadata
+    "Environment :: Console",
+    "Natural Language :: English",
+    "Topic :: Security",
+    "Topic :: Utilities",
+]
+readme = {file="README.md", content-type="text/markdown"}
+
+dependencies = [
+    "resotolib==3.5.1",
+    "resoto-plugin-aws==3.5.1"
+]
+
+[project.entry-points."resoto.plugins"]
+cleanup_aws_vpcs = "resoto_plugin_cleanup_aws_vpcs:CleanupAWSVPCsPlugin"
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs"
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
+
```

