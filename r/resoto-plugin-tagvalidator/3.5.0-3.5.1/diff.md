# Comparing `tmp/resoto-plugin-tagvalidator-3.5.0.tar.gz` & `tmp/resoto-plugin-tagvalidator-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-tagvalidator-3.5.0.tar", last modified: Fri May 26 18:26:57 2023, max compression
+gzip compressed data, was "resoto-plugin-tagvalidator-3.5.1.tar", last modified: Fri Jun  2 14:52:09 2023, max compression
```

## Comparing `resoto-plugin-tagvalidator-3.5.0.tar` & `resoto-plugin-tagvalidator-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:57.749038 resoto-plugin-tagvalidator-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:14.000000 resoto-plugin-tagvalidator-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-26 18:26:57.749038 resoto-plugin-tagvalidator-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-26 18:24:14.000000 resoto-plugin-tagvalidator-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:24:14.000000 resoto-plugin-tagvalidator-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:57.749038 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator/
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-26 18:24:14.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-26 18:24:14.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:57.749038 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-26 18:26:57.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 18:26:57.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:57.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 18:26:57.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:57.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:26:57.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 18:26:57.000000 resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:26:57.749038 resoto-plugin-tagvalidator-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 18:24:14.000000 resoto-plugin-tagvalidator-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:57.749038 resoto-plugin-tagvalidator-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-26 18:24:14.000000 resoto-plugin-tagvalidator-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:09.145630 resoto-plugin-tagvalidator-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:48:37.000000 resoto-plugin-tagvalidator-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-02 14:52:09.145630 resoto-plugin-tagvalidator-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-02 14:48:37.000000 resoto-plugin-tagvalidator-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-02 14:48:37.000000 resoto-plugin-tagvalidator-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:09.145630 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-02 14:48:37.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-02 14:48:37.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:09.145630 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-02 14:52:09.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 14:52:09.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:09.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 14:52:09.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:49:45.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:52:09.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 14:52:09.000000 resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:09.145630 resoto-plugin-tagvalidator-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:09.145630 resoto-plugin-tagvalidator-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-02 14:48:37.000000 resoto-plugin-tagvalidator-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-tagvalidator-3.5.0/PKG-INFO` & `resoto-plugin-tagvalidator-3.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Tag Validator Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
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
 
 # resoto-plugin-tagvalidator
 Tag Validator plugin for Resoto
 
 This plugin validates the contents of expiration tags. With it you can enforce a max. expiration length for certain resources in an account. For instance you could have an org policy that says in our "dev" account compute instances are only allowed to exist for 2 days max. Then this plugin can ensure that the expiration tag on those instances is set to no more than 2 days. If it is set to e.g. 50h it would be corrected down to 48h.
```

### Comparing `resoto-plugin-tagvalidator-3.5.0/README.md` & `resoto-plugin-tagvalidator-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator/__init__.py` & `resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator/config.py` & `resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.5.0/resoto_plugin_tagvalidator.egg-info/PKG-INFO` & `resoto-plugin-tagvalidator-3.5.1/resoto_plugin_tagvalidator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Tag Validator Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
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
 
 # resoto-plugin-tagvalidator
 Tag Validator plugin for Resoto
 
 This plugin validates the contents of expiration tags. With it you can enforce a max. expiration length for certain resources in an account. For instance you could have an org policy that says in our "dev" account compute instances are only allowed to exist for 2 days max. Then this plugin can ensure that the expiration tag on those instances is set to no more than 2 days. If it is set to e.g. 50h it would be corrected down to 48h.
```

### Comparing `resoto-plugin-tagvalidator-3.5.0/setup.py` & `resoto-plugin-tagvalidator-3.5.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,44 @@
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
-    name="resoto-plugin-tagvalidator",
-    version="3.5.0",
-    description="Resoto Tag Validator Plugin",
-    license="Apache 2.0",
-    packages=find_packages(),
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    entry_points={"resoto.plugins": ["tagvalidator = resoto_plugin_tagvalidator:TagValidatorPlugin"]},
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
-    url="https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator",
-)
+[project]
+name = "resoto-plugin-tagvalidator"
+description = "Resoto Tag Validator Plugin"
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
+]
+
+[project.entry-points."resoto.plugins"]
+tagvalidator = "resoto_plugin_tagvalidator:TagValidatorPlugin"
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator"
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
+
```

### Comparing `resoto-plugin-tagvalidator-3.5.0/test/test_config.py` & `resoto-plugin-tagvalidator-3.5.1/test/test_config.py`

 * *Files identical despite different names*

