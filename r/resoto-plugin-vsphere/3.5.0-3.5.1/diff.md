# Comparing `tmp/resoto-plugin-vsphere-3.5.0.tar.gz` & `tmp/resoto-plugin-vsphere-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-vsphere-3.5.0.tar", last modified: Fri May 26 18:26:34 2023, max compression
+gzip compressed data, was "resoto-plugin-vsphere-3.5.1.tar", last modified: Fri Jun  2 14:52:32 2023, max compression
```

## Comparing `resoto-plugin-vsphere-3.5.0.tar` & `resoto-plugin-vsphere-3.5.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:34.565657 resoto-plugin-vsphere-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-26 18:26:34.565657 resoto-plugin-vsphere-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:34.565657 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/vsphere_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:34.565657 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-26 18:26:34.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 18:26:34.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:34.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 18:26:34.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:34.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 18:26:34.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 18:26:34.000000 resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:26:34.565657 resoto-plugin-vsphere-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:34.565657 resoto-plugin-vsphere-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-26 18:24:12.000000 resoto-plugin-vsphere-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:32.894988 resoto-plugin-vsphere-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-02 14:52:32.894988 resoto-plugin-vsphere-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:32.890988 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/vsphere_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:32.894988 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-02 14:52:32.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-02 14:52:32.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:32.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 14:52:32.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:53.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 14:52:32.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 14:52:32.000000 resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:32.894988 resoto-plugin-vsphere-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:32.894988 resoto-plugin-vsphere-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-02 14:49:38.000000 resoto-plugin-vsphere-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-vsphere-3.5.0/PKG-INFO` & `resoto-plugin-vsphere-3.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto VSphere Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/vsphere
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/vsphere
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
 
 # resoto-plugin-vsphere
 VMWare VSphere Collector Plugin for Resoto (Alpha)
```

### Comparing `resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/__init__.py` & `resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/config.py` & `resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/resources.py` & `resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere/vsphere_client.py` & `resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere/vsphere_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/PKG-INFO` & `resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto VSphere Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/vsphere
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/vsphere
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
 
 # resoto-plugin-vsphere
 VMWare VSphere Collector Plugin for Resoto (Alpha)
```

### Comparing `resoto-plugin-vsphere-3.5.0/resoto_plugin_vsphere.egg-info/SOURCES.txt` & `resoto-plugin-vsphere-3.5.1/resoto_plugin_vsphere.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_vsphere/__init__.py
 resoto_plugin_vsphere/config.py
 resoto_plugin_vsphere/resources.py
 resoto_plugin_vsphere/vsphere_client.py
 resoto_plugin_vsphere.egg-info/PKG-INFO
 resoto_plugin_vsphere.egg-info/SOURCES.txt
 resoto_plugin_vsphere.egg-info/dependency_links.txt
```

### Comparing `resoto-plugin-vsphere-3.5.0/setup.py` & `resoto-plugin-vsphere-3.5.1/pyproject.toml`

 * *Files 26% similar despite different names*

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
-    name="resoto-plugin-vsphere",
-    version="3.5.0",
-    description="Resoto VSphere Collector Plugin",
-    license="Apache 2.0",
-    packages=find_packages(),
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    entry_points={"resoto.plugins": ["vsphere = resoto_plugin_vsphere:VSphereCollectorPlugin"]},
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
-    url="https://github.com/someengineering/resoto/tree/main/plugins/vsphere",
-)
+[project]
+name = "resoto-plugin-vsphere"
+description = "Resoto VSphere Collector Plugin"
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
+    "pyvmomi",
+]
+
+[project.entry-points."resoto.plugins"]
+vsphere = "resoto_plugin_vsphere:VSphereCollectorPlugin"
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/plugins/vsphere"
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
+
```

