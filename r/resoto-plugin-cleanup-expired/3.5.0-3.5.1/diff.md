# Comparing `tmp/resoto-plugin-cleanup-expired-3.5.0.tar.gz` & `tmp/resoto-plugin-cleanup-expired-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-expired-3.5.0.tar", last modified: Fri May 26 18:23:22 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-expired-3.5.1.tar", last modified: Fri Jun  2 14:57:04 2023, max compression
```

## Comparing `resoto-plugin-cleanup-expired-3.5.0.tar` & `resoto-plugin-cleanup-expired-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:04.186967 resoto-plugin-cleanup-expired-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:53:32.000000 resoto-plugin-cleanup-expired-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-02 14:57:04.186967 resoto-plugin-cleanup-expired-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 14:53:32.000000 resoto-plugin-cleanup-expired-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 14:53:32.000000 resoto-plugin-cleanup-expired-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:04.182968 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-02 14:53:32.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-02 14:53:32.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:04.186967 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-02 14:57:04.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-02 14:57:04.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:57:04.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 14:57:04.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:59.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:57:04.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 14:57:04.000000 resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:57:04.186967 resoto-plugin-cleanup-expired-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:04.186967 resoto-plugin-cleanup-expired-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-02 14:53:32.000000 resoto-plugin-cleanup-expired-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-expired-3.5.0/PKG-INFO` & `resoto-plugin-cleanup-expired-3.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Expired Resource Cleanup Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
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
 
 # resoto-plugin-cleanup-expired
 Resoto plugin for cleanup of expired resources
 
 This plugin looks for resources with the tags `expiration` or `resoto:expires` and flags them for cleanup if they are expired.
```

### Comparing `resoto-plugin-cleanup-expired-3.5.0/README.md` & `resoto-plugin-cleanup-expired-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/__init__.py` & `resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/PKG-INFO` & `resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Expired Resource Cleanup Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
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
 
 # resoto-plugin-cleanup-expired
 Resoto plugin for cleanup of expired resources
 
 This plugin looks for resources with the tags `expiration` or `resoto:expires` and flags them for cleanup if they are expired.
```

### Comparing `resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-expired-3.5.1/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_cleanup_expired/__init__.py
 resoto_plugin_cleanup_expired/config.py
 resoto_plugin_cleanup_expired.egg-info/PKG-INFO
 resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
 resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
 resoto_plugin_cleanup_expired.egg-info/entry_points.txt
 resoto_plugin_cleanup_expired.egg-info/not-zip-safe
```

### Comparing `resoto-plugin-cleanup-expired-3.5.0/setup.py` & `resoto-plugin-cleanup-expired-3.5.1/pyproject.toml`

 * *Files 17% similar despite different names*

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
-    name="resoto-plugin-cleanup-expired",
-    version="3.5.0",
-    description="Resoto Expired Resource Cleanup Plugin",
-    license="Apache 2.0",
-    packages=find_packages(),
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    entry_points={"resoto.plugins": ["cleanup_expired = resoto_plugin_cleanup_expired:CleanupExpiredPlugin"]},
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
-    url="https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired",
-)
+[project]
+name = "resoto-plugin-cleanup-expired"
+description = "Resoto Expired Resource Cleanup Plugin"
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
+cleanup_expired = "resoto_plugin_cleanup_expired:CleanupExpiredPlugin"
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired"
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
+
```

