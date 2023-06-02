# Comparing `tmp/edx-arch-experiments-1.2.0.tar.gz` & `tmp/edx-arch-experiments-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-arch-experiments-1.2.0.tar", last modified: Tue May  9 16:31:34 2023, max compression
+gzip compressed data, was "edx-arch-experiments-2.0.0.tar", last modified: Fri Jun  2 16:03:22 2023, max compression
```

## Comparing `edx-arch-experiments-1.2.0.tar` & `edx-arch-experiments-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6769 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4463 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.781480 edx-arch-experiments-1.2.0/edx_arch_experiments/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/tests/test_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6769 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5475 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:03:22.320599 edx-arch-experiments-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6868 2023-06-02 16:03:22.320599 edx-arch-experiments-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4463 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:03:22.316599 edx-arch-experiments-2.0.0/edx_arch_experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/edx_arch_experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/edx_arch_experiments/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:03:22.320599 edx-arch-experiments-2.0.0/edx_arch_experiments/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/edx_arch_experiments/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/edx_arch_experiments/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/edx_arch_experiments/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:03:22.320599 edx-arch-experiments-2.0.0/edx_arch_experiments/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/edx_arch_experiments/tests/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:03:22.320599 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6868 2023-06-02 16:03:22.000000 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-06-02 16:03:22.000000 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 16:03:22.000000 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-02 16:03:22.000000 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 16:03:22.000000 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-02 16:03:22.000000 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-02 16:03:22.000000 edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:03:22.320599 edx-arch-experiments-2.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-02 16:03:22.320599 edx-arch-experiments-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5196 2023-06-02 16:03:13.000000 edx-arch-experiments-2.0.0/setup.py
```

### Comparing `edx-arch-experiments-1.2.0/CHANGELOG.rst` & `edx-arch-experiments-2.0.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 *
 
+[2.0.0] - 2023-06-01
+~~~~~~~~~~~~~~~~~~~~
+
+* Removes summary hook aside, now in the ai-aside repo
+
 [1.2.0] - 2023-05-08
 ~~~~~~~~~~~~~~~~~~~~
 
 * Update summary hook to trigger on videos
 * Remove text selection data key from summary hook html
 
 [1.1.4] - 2023-04-14
```

### Comparing `edx-arch-experiments-1.2.0/LICENSE.txt` & `edx-arch-experiments-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.2.0/PKG-INFO` & `edx-arch-experiments-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-arch-experiments
-Version: 1.2.0
+Version: 2.0.0
 Summary: A plugin to include applications under development by the architecture team at edx
 Home-page: https://github.com/edx/edx-arch-experiments
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -160,14 +160,19 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 *
 
+[2.0.0] - 2023-06-01
+~~~~~~~~~~~~~~~~~~~~
+
+* Removes summary hook aside, now in the ai-aside repo
+
 [1.2.0] - 2023-05-08
 ~~~~~~~~~~~~~~~~~~~~
 
 * Update summary hook to trigger on videos
 * Remove text selection data key from summary hook html
 
 [1.1.4] - 2023-04-14
```

### Comparing `edx-arch-experiments-1.2.0/README.rst` & `edx-arch-experiments-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.2.0/edx_arch_experiments/apps.py` & `edx-arch-experiments-2.0.0/edx_arch_experiments/apps.py`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/PKG-INFO` & `edx-arch-experiments-2.0.0/edx_arch_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-arch-experiments
-Version: 1.2.0
+Version: 2.0.0
 Summary: A plugin to include applications under development by the architecture team at edx
 Home-page: https://github.com/edx/edx-arch-experiments
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -160,14 +160,19 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 *
 
+[2.0.0] - 2023-06-01
+~~~~~~~~~~~~~~~~~~~~
+
+* Removes summary hook aside, now in the ai-aside repo
+
 [1.2.0] - 2023-05-08
 ~~~~~~~~~~~~~~~~~~~~
 
 * Update summary hook to trigger on videos
 * Remove text selection data key from summary hook html
 
 [1.1.4] - 2023-04-14
```

### Comparing `edx-arch-experiments-1.2.0/requirements/constraints.txt` & `edx-arch-experiments-2.0.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.2.0/setup.py` & `edx-arch-experiments-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -106,15 +106,14 @@
     description='A plugin to include applications under development by the architecture team at edx',
     long_description=f"{README}\n\n{CHANGELOG}",
     author='edX',
     author_email='oscm@edx.org',
     url='https://github.com/edx/edx-arch-experiments',
     packages=[
         'edx_arch_experiments',
-        'edx_arch_experiments.summaryhook_aside',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     python_requires=">=3.8",
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Python edx',
@@ -127,14 +126,10 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
         "lms.djangoapp": [
             "arch_experiments = edx_arch_experiments.apps:EdxArchExperimentsConfig",
-            "summaryhook = edx_arch_experiments.summaryhook_aside.apps:SummaryHookConfig",
-        ],
-        "xblock_asides.v1": [
-            "summaryhook_aside = edx_arch_experiments.summaryhook_aside.block:SummaryHookAside",
         ],
     },
 )
```

