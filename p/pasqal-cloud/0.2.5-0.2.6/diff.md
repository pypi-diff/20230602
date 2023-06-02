# Comparing `tmp/pasqal-cloud-0.2.5.tar.gz` & `tmp/pasqal-cloud-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.2.5.tar", last modified: Mon Apr 24 13:05:37 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.2.6.tar", last modified: Fri Jun  2 14:10:18 2023, max compression
```

## Comparing `pasqal-cloud-0.2.5.tar` & `pasqal-cloud-0.2.6.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_doubles/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_project_renaming_compatibility.py
```

### Comparing `pasqal-cloud-0.2.5/LICENSE` & `pasqal-cloud-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/PKG-INFO` & `pasqal-cloud-0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.5
+Version: 0.2.6
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -64,19 +64,19 @@
 
 Once you have serialized your sequence, you can send it with the SDK with the following code
 
 ```python
 from pasqal_cloud import SDK
 from pulser import devices, Register, Sequence
 
-group_id="your_group_id" # Replace this value by your group_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 
-sdk = SDK(username=username, password=password, group_id=group_id)
+sdk = SDK(username=username, password=password, project_id=project_id)
 
 # When creating a job, select a number of runs and set the desired values for the variables
 # defined in the sequence
 job1 = {"runs": 20, "variables": {"omega_max": 6} }
 job2 = {"runs": 50, "variables": {"omega_max": 10.5} }
 
 # Send the batch of jobs to the QPU and wait for the results
@@ -98,41 +98,45 @@
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
 from pasqal_cloud import SDK
 
-group_id="your_group_id" # Replace this value by your group_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 # Ideally, do not write this password in a script but provide in through the command-line or as a secret environment variable.
 
 """ Method 1: Username + Password
     If you know your credentials, you can pass them to the SDK instance on creation.
 """
-sdk = SDK(username=username, password=password, group_id=group_id)
+sdk = SDK(username=username, password=password, project_id=project_id)
 
 """ Method 2: Username only
     If you only want to insert your username, but want a solution to have your password being secret
     you can run the SDK without password. A prompt will then ask for your password
 """
-sdk = SDK(username=username, group_id=group_id)
+sdk = SDK(username=username, project_id=project_id)
 > Please, enter your password:
 
 """ Method 3: Use a custom token provider
     You can define a custom class to provide the token.
     For example, if you know your token, you can use that token to authenticate directly to our APIs as follows.
 """
 class CustomTokenProvider(TokenProvider):
     def get_token(self):
         return "your-token" # Replace this value with your token
 
 
-sdk = SDK(token_provider=CustomTokenProvider(), group_id=group_id)
+sdk = SDK(token_provider=CustomTokenProvider(), project_id=project_id)
+
+""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a 
+    custom _query_token method which fetches your token. See Auth0TokenProvider implementation for an example.
+"""
 ```
 
 ### Extra emulator configuration (Soon publicly available)
 
 Some emulators, such as EMU_TN and EMU_FREE, accept further configuration to control the emulation.
 This is because these emulators are more advanced numerical simulation of the quantum system.
```

### Comparing `pasqal-cloud-0.2.5/README.md` & `pasqal-cloud-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -49,19 +49,19 @@
 
 Once you have serialized your sequence, you can send it with the SDK with the following code
 
 ```python
 from pasqal_cloud import SDK
 from pulser import devices, Register, Sequence
 
-group_id="your_group_id" # Replace this value by your group_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 
-sdk = SDK(username=username, password=password, group_id=group_id)
+sdk = SDK(username=username, password=password, project_id=project_id)
 
 # When creating a job, select a number of runs and set the desired values for the variables
 # defined in the sequence
 job1 = {"runs": 20, "variables": {"omega_max": 6} }
 job2 = {"runs": 50, "variables": {"omega_max": 10.5} }
 
 # Send the batch of jobs to the QPU and wait for the results
@@ -83,41 +83,45 @@
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
 from pasqal_cloud import SDK
 
-group_id="your_group_id" # Replace this value by your group_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 # Ideally, do not write this password in a script but provide in through the command-line or as a secret environment variable.
 
 """ Method 1: Username + Password
     If you know your credentials, you can pass them to the SDK instance on creation.
 """
-sdk = SDK(username=username, password=password, group_id=group_id)
+sdk = SDK(username=username, password=password, project_id=project_id)
 
 """ Method 2: Username only
     If you only want to insert your username, but want a solution to have your password being secret
     you can run the SDK without password. A prompt will then ask for your password
 """
-sdk = SDK(username=username, group_id=group_id)
+sdk = SDK(username=username, project_id=project_id)
 > Please, enter your password:
 
 """ Method 3: Use a custom token provider
     You can define a custom class to provide the token.
     For example, if you know your token, you can use that token to authenticate directly to our APIs as follows.
 """
 class CustomTokenProvider(TokenProvider):
     def get_token(self):
         return "your-token" # Replace this value with your token
 
 
-sdk = SDK(token_provider=CustomTokenProvider(), group_id=group_id)
+sdk = SDK(token_provider=CustomTokenProvider(), project_id=project_id)
+
+""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a 
+    custom _query_token method which fetches your token. See Auth0TokenProvider implementation for an example.
+"""
 ```
 
 ### Extra emulator configuration (Soon publicly available)
 
 Some emulators, such as EMU_TN and EMU_FREE, accept further configuration to control the emulation.
 This is because these emulators are more advanced numerical simulation of the quantum system.
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/__init__.py` & `pasqal-cloud-0.2.6/pasqal_cloud/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from pasqal_cloud.authentication import TokenProvider
 from pasqal_cloud.batch import Batch, RESULT_POLLING_INTERVAL
 from pasqal_cloud.client import Client
 from pasqal_cloud.device import BaseConfig
 from pasqal_cloud.device import EmulatorType
 from pasqal_cloud.endpoints import Auth0Conf, Endpoints
@@ -25,30 +26,42 @@
 
 
 class SDK:
     _client: Client
 
     def __init__(
         self,
-        group_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         token_provider: Optional[TokenProvider] = None,
         endpoints: Optional[Endpoints] = None,
         auth0: Optional[Auth0Conf] = None,
         webhook: Optional[str] = None,
+        group_id: Optional[str] = None,
+        project_id: Optional[str] = None
     ):
         """This class provides helper methods to call the PASQAL Cloud endpoints.
 
         To authenticate to PASQAL Cloud, you have to provide either an
         email/password combination or a TokenProvider instance.
         You may omit the password, you will then be prompted to enter one.
         """
+
+        # Ticket (#622), to be removed, used to avoid a breaking change during the group to project renaming
+        if not project_id:
+            if not group_id:
+                raise TypeError("Either a group_id or project_id has to be given as argument")
+            warn('The parameter group_id is deprecated, from now use project_id instead',
+                 DeprecationWarning,
+                 stacklevel=2
+                 )
+            project_id = group_id
+
         self._client = Client(
-            group_id=group_id,
+            project_id=project_id,
             username=username,
             password=password,
             token_provider=token_provider,
             endpoints=endpoints,
             auth0=auth0,
         )
         self.batches: Dict[str, Batch] = {}
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/_version.py` & `pasqal-cloud-0.2.6/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/authentication.py` & `pasqal-cloud-0.2.6/pasqal_cloud/authentication.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,22 +34,36 @@
 
     @abstractmethod
     def get_token(self) -> str:
         raise NotImplementedError
 
 
 class ExpiringTokenProvider(TokenProvider, ABC):
+    """TokenProvider class which caches a token up to its expiry date.
+
+    This is an abstract class. Create your custom TokenProvider by inheriting from
+    this class and defining your own `_query_token` method. See Auth0TokenProvider for
+    an implementation example.
+    """
     __token_cache: Optional[tuple[datetime, str]] = None
     expiry_window: timedelta = timedelta(minutes=1.0)
 
     @abstractmethod
     def _query_token(self) -> dict[str, Any]:
+        """Return a dictionnary mapping the key 'access_token' to the token value.
+
+        Optionally, your dictionnary may include an 'expires_in' key mapped to the
+        duration before expiration of your token (in seconds).
+        """
         raise NotImplementedError
 
     def get_token(self) -> str:
+        """Returns the token stored in the cache. If token has expired, first refresh
+        the cache by calling the _query_token method.
+        """
         if self.__token_cache:
             expiry, token = self.__token_cache
             if expiry - self.expiry_window > datetime.now(tz=timezone.utc):
                 return token
 
         self.__token_cache = self._refresh_token_cache()
         return self.__token_cache[1]
@@ -99,15 +113,24 @@
         except DecodeError:
             # The token is not in a format that could be parsed as a JWT
             pass
         return None
 
 
 class Auth0TokenProvider(ExpiringTokenProvider):
+    """ExpiringTokenProvider implementation which fetches a token from auth0."""
     def __init__(self, username: str, password: str, auth0: Auth0Conf):
+        """Initializes the token provider with user credentials and
+        an auth0 configuration object
+
+        Args:
+            username: name of the user to log in as
+            password: password of the user to log in as
+            auth0: auth0 configuration object to target the proper auth0 tenant and app
+        """
         self.username = username
         self.password = password
         self.auth0 = auth0
 
         # Makes a call in order to check the credentials at creation
         self.get_token()
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/batch.py` & `pasqal-cloud-0.2.6/pasqal_cloud/batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from dataclasses import dataclass, field
 from typing import Any, Dict, Optional, Type, Union
+from warnings import warn
 
 from pasqal_cloud.client import Client
 from pasqal_cloud.job import Job
 from pasqal_cloud.device.configuration import BaseConfig, EmuTNConfig, EmuFreeConfig
 from pasqal_cloud.device import EmulatorType
 
 RESULT_POLLING_INTERVAL = 2  # seconds
@@ -19,50 +20,53 @@
     device until all its jobs are done and declared complete.
 
     Attributes:
         - complete: Whether the batch has been declared as complete.
         - created_at: Timestamp of the creation of the batch.
         - updated_at: Timestamp of the last update of the batch.
         - device_type: Type of device to run the batch on.
-        - group_id: ID of the owner group of the batch.
+        - project_id: ID of the owner project of the batch.
         - id: Unique identifier for the batch.
         - user_id: Unique identifier of the user that created the batch.
         - priority: Level of priority of the batch.
         - status: Status of the batch. Possible values are: PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
         - webhook: Webhook where the job results are automatically sent to.
         - _client: A Client instance to connect to PCS.
         - sequence_builder: Pulser sequence of the batch.
         - start_datetime: Timestamp of the time the batch was sent to the QPU.
         - end_datetime: Timestamp of when the batch process was finished.
         - device_status: Status of the device where the batch is running.
         - jobs: Dictionary of all the jobs added to the batch.
         - jobs_count: Number of jobs added to the batch.
         - jobs_count_per_status: Number of jobs per status.
         - configuration: Further configuration for certain emulators.
+        - group_id: This parameter is deprecated, use project_id instead.
     """
 
     complete: bool
     created_at: str
     updated_at: str
     device_type: str
-    group_id: str
+    project_id: str
     id: str
     user_id: int
     priority: int
     status: str
     webhook: str
     _client: Client
     sequence_builder: str
     start_datetime: Optional[str] = None
     end_datetime: Optional[str] = None
     device_status: Optional[str] = None
     jobs: Dict[str, Job] = field(default_factory=dict)
     jobs_count: int = 0
     jobs_count_per_status: Dict[str, int] = field(default_factory=dict)
     configuration: Optional[Union[BaseConfig, dict]] = None
+    # Ticket (#622)
+    group_id: Optional[str] = None
 
     def __post_init__(self) -> None:
         """Post init method to convert the configuration to a BaseConfig object."""
         if not isinstance(self.configuration, dict):
             return
         conf_class: Type[BaseConfig] = BaseConfig
         if self.device_type == EmulatorType.EMU_TN.value:
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/client.py` & `pasqal-cloud-0.2.6/pasqal_cloud/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 
 
 class Client:
     authenticator: AuthBase
 
     def __init__(
         self,
-        group_id: str,
+        project_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         token_provider: Optional[TokenProvider] = None,
         endpoints: Optional[Endpoints] = None,
-        auth0: Optional[Auth0Conf] = None,
+        auth0: Optional[Auth0Conf] = None
     ):
         if not username and not token_provider:
             raise ValueError(
                 "At least a username or TokenProvider object should be provided."
             )
         if token_provider is not None:
             self._check_token_provider(token_provider)
@@ -53,15 +53,15 @@
         self.endpoints = self._make_endpoints(endpoints)
 
         if username:
             auth0 = self._make_auth0(auth0)
             token_provider = self._credential_login(username, password, auth0)
 
         self.authenticator = HTTPBearerAuthenticator(token_provider)
-        self.group_id = group_id
+        self.project_id = project_id
 
     @staticmethod
     def _make_endpoints(endpoints: Optional[Endpoints]) -> Endpoints:
         if endpoints is None:
             return Endpoints()
 
         if not isinstance(endpoints, Endpoints):
@@ -113,15 +113,15 @@
             raise HTTPError(data)
 
         return data
 
     def _send_batch(
         self, batch_data: Dict[str, Any]
     ) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
-        batch_data.update({"group_id": self.group_id})
+        batch_data.update({"project_id": self.project_id})
         batch_data = self._request(
             "POST",
             f"{self.endpoints.core}/api/v1/batches",
             batch_data,
         )["data"]
         jobs_data = batch_data.pop("jobs", [])
         return batch_data, jobs_data
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.2.6/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/errors.py` & `pasqal-cloud-0.2.6/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/job.py` & `pasqal-cloud-0.2.6/pasqal_cloud/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from pasqal_cloud.client import Client
 
 
 @dataclass
 class Job:
     """Class for job data.
 
     Attributes:
         - runs: Number of times the job should be run.
-        - created_at: Timestamp of the creation of the job.
-        - updated_at: Timestamp of the last update of the job.
-        - start_timestamp: The timestamp of when the job began processing.
-        - end_timestamp: The timestamp of when the job finished processing.
         - batch_id: ID of the batch which the job belongs to.
-        - errors: Error messages that occurred while processing job.
         - id: Unique identifier for the job.
-        - group_id: ID of the group which the users scheduling the job belong to.
+        - project_id: ID of the project which the users scheduling the job belong to.
         - status: Status of the job. Possible values are: PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
         - _client: A Client instance to connect to PCS.
+        - created_at: Timestamp of the creation of the job.
+        - updated_at: Timestamp of the last update of the job.
+        - errors: Error messages that occurred while processing job.
+        - start_timestamp: The timestamp of when the job began processing.
+        - end_timestamp: The timestamp of when the job finished processing.
         - result: Result of the job.
         - variables: Dictionary of variables of the job.
           None if the associated batch is non-parametrized.
+        - group_id: This parameter is deprecated, use project_id instead.
     """
 
     runs: int
     batch_id: str
     id: str
-    group_id: str
+    project_id: str
     status: str
-    _client : Client
+    _client: Client
     created_at: str
     updated_at: str
     errors: List[str]
     start_timestamp: Optional[str] = None
     end_timestamp: Optional[str] = None
     result: Optional[Dict[str, Any]] = None
     variables: Optional[Dict[str, Any]] = None
+    # Ticket (#622)
+    group_id: Optional[str] = None
 
     def cancel(self) -> Dict[str, Any]:
         """Cancel the current job on the PCS."""
         job_rsp = self._client._cancel_job(self.id)
         self.status = job_rsp.get("status", "CANCELED")
         return job_rsp
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.2.6/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.2.6/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.5
+Version: 0.2.6
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -64,19 +64,19 @@
 
 Once you have serialized your sequence, you can send it with the SDK with the following code
 
 ```python
 from pasqal_cloud import SDK
 from pulser import devices, Register, Sequence
 
-group_id="your_group_id" # Replace this value by your group_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 
-sdk = SDK(username=username, password=password, group_id=group_id)
+sdk = SDK(username=username, password=password, project_id=project_id)
 
 # When creating a job, select a number of runs and set the desired values for the variables
 # defined in the sequence
 job1 = {"runs": 20, "variables": {"omega_max": 6} }
 job2 = {"runs": 50, "variables": {"omega_max": 10.5} }
 
 # Send the batch of jobs to the QPU and wait for the results
@@ -98,41 +98,45 @@
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
 from pasqal_cloud import SDK
 
-group_id="your_group_id" # Replace this value by your group_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 # Ideally, do not write this password in a script but provide in through the command-line or as a secret environment variable.
 
 """ Method 1: Username + Password
     If you know your credentials, you can pass them to the SDK instance on creation.
 """
-sdk = SDK(username=username, password=password, group_id=group_id)
+sdk = SDK(username=username, password=password, project_id=project_id)
 
 """ Method 2: Username only
     If you only want to insert your username, but want a solution to have your password being secret
     you can run the SDK without password. A prompt will then ask for your password
 """
-sdk = SDK(username=username, group_id=group_id)
+sdk = SDK(username=username, project_id=project_id)
 > Please, enter your password:
 
 """ Method 3: Use a custom token provider
     You can define a custom class to provide the token.
     For example, if you know your token, you can use that token to authenticate directly to our APIs as follows.
 """
 class CustomTokenProvider(TokenProvider):
     def get_token(self):
         return "your-token" # Replace this value with your token
 
 
-sdk = SDK(token_provider=CustomTokenProvider(), group_id=group_id)
+sdk = SDK(token_provider=CustomTokenProvider(), project_id=project_id)
+
+""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a 
+    custom _query_token method which fetches your token. See Auth0TokenProvider implementation for an example.
+"""
 ```
 
 ### Extra emulator configuration (Soon publicly available)
 
 Some emulators, such as EMU_TN and EMU_FREE, accept further configuration to control the emulation.
 This is because these emulators are more advanced numerical simulation of the quantum system.
```

### Comparing `pasqal-cloud-0.2.5/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.2.6/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,9 +35,10 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_batch.py
 tests/test_client.py
 tests/test_cloud_sdk_import.py
 tests/test_config.py
 tests/test_device_specs.py
+tests/test_project_renaming_compatibility.py
 tests/test_doubles/__init__.py
 tests/test_doubles/authentication.py
```

### Comparing `pasqal-cloud-0.2.5/sdk/setup.py` & `pasqal-cloud-0.2.6/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/setup.py` & `pasqal-cloud-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/tests/conftest.py` & `pasqal-cloud-0.2.6/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,29 @@
     request_mock.stop()
 
 
 @pytest.fixture
 @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
 def pasqal_client_mock():
     client = Client(
-        group_id="00000000-0000-0000-0000-000000000002",
+        project_id="00000000-0000-0000-0000-000000000002",
         username="00000000-0000-0000-0000-000000000001",
         password="password",
     )
     return client
 
 
 @pytest.fixture
 def batch(pasqal_client_mock):
     batch_data = {
         "complete": False,
         "created_at": "2022-12-31T23:59:59.999Z",
         "updated_at": "2023-01-01T00:00:00.000Z",
         "device_type": "qpu",
-        "group_id": "00000000-0000-0000-0000-000000000002",
+        "project_id": "00000000-0000-0000-0000-000000000002",
         "id": "00000000-0000-0000-0000-000000000001",
         "user_id": 1,
         "priority": 0,
         "status": "PENDING",
         "webhook": "https://example.com/webhook",
         "_client": pasqal_client_mock,
         "sequence_builder": "pulser",
@@ -91,15 +91,15 @@
 
 @pytest.fixture
 def job(pasqal_client_mock):
     job_data = {
         "runs": 50,
         "batch_id": "00000000-0000-0000-0000-000000000001",
         "id": "00000000-0000-0000-0000-000000022010",
-        "group_id": "00000000-0000-0000-0000-000000000001",
+        "project_id": "00000000-0000-0000-0000-000000000001",
         "status": "PENDING",
         "_client": pasqal_client_mock,
         "created_at": "2022-12-31T23:59:59.999Z",
         "updated_at": "2023-01-01T00:00:00.000Z",
         "errors": [],
         "variables": {
             "param1": 1,
```

### Comparing `pasqal-cloud-0.2.5/tests/test_batch.py` & `pasqal-cloud-0.2.6/tests/test_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class TestBatch:
     @pytest.fixture(autouse=True)
     @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
     def init_sdk(self, start_mock_request):
         self.sdk = SDK(
-            username="me@test.com", password="password", group_id=str(uuid4())
+            username="me@test.com", password="password", project_id=str(uuid4())
         )
         self.pulser_sequence = "pulser_test_sequence"
         self.batch_id = "00000000-0000-0000-0000-000000000001"
         self.job_result = {"1001": 12, "0110": 35, "1111": 1}
         self.n_job_runs = 50
         self.job_id = "00000000-0000-0000-0000-000000022010"
         self.job_variables = {"Omega_max": 14.4, "last_target": "q1", "ts": [200, 500]}
```

### Comparing `pasqal-cloud-0.2.5/tests/test_client.py` & `pasqal-cloud-0.2.6/tests/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,137 +9,137 @@
     FakeAuth0AuthenticationFailure,
     FakeAuth0AuthenticationSuccess,
 )
 
 
 @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
 class TestAuthSuccess:
-    group_id = "random_group_id"
+    project_id = "random_project_id"
     username = "random_username"
     password = "random_password"
     new_core_endpoint = "random_endpoint"
 
     @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_success(self, getpass):
         getpass.return_value = self.password
-        SDK(group_id=self.group_id, username=self.username)
+        SDK(project_id=self.project_id, username=self.username)
         getpass.assert_called_once()
 
     def test_authentication_success(self):
-        SDK(group_id=self.group_id, username=self.username, password=self.password)
+        SDK(project_id=self.project_id, username=self.username, password=self.password)
 
     def test_good_token_provider(self):
         SDK(
-            group_id=self.group_id,
+            project_id=self.project_id,
             token_provider=FakeAuth0AuthenticationSuccess("username", "password", None),
         )
 
     def test_custom_token_provider(self):
         """Test that the custom provider suggested in the readme is working"""
         class CustomTokenProvider(TokenProvider):
             def get_token(self):
                 return "your-token" # Replace this value with your token
-        SDK(token_provider=CustomTokenProvider(), group_id="group_id")
+        SDK(token_provider=CustomTokenProvider(), project_id="project_id")
 
     def test_correct_endpoints(self):
         sdk = SDK(
-            group_id=self.group_id,
+            project_id=self.project_id,
             username=self.username,
             password=self.password,
             endpoints=Endpoints(core=self.new_core_endpoint),
         )
         assert sdk._client.endpoints.core == self.new_core_endpoint
 
     def test_correct_new_auth0(self):
         new_auth0 = Auth0Conf(domain="new_domain")
         SDK(
-            group_id=self.group_id,
+            project_id=self.project_id,
             username=self.username,
             password=self.password,
             auth0=new_auth0,
         )
 
 
 @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationFailure)
 class TestAuthFailure:
-    group_id = "random_group_id"
+    project_id = "random_project_id"
     username = "random_username"
     no_username = ""
     password = "random_password"
     no_password = ""
 
     @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_bad_password(self, getpass):
         getpass.return_value = self.password
 
         with pytest.raises(Auth0Error):
-            SDK(group_id=self.group_id, username=self.username)
+            SDK(project_id=self.project_id, username=self.username)
 
         getpass.assert_called_once()
 
     def test_module_bad_password(self):
         with pytest.raises(Auth0Error):
-            SDK(group_id=self.group_id, username=self.username, password=self.password)
+            SDK(project_id=self.project_id, username=self.username, password=self.password)
 
 
 class TestAuthInvalidClient:
-    group_id = "random_group_id"
+    project_id = "random_project_id"
     username = "random_username"
     no_username = ""
     password = "random_password"
     no_password = ""
 
     def test_module_no_user_with_password(self):
         with pytest.raises(ValueError):
             SDK(
-                group_id=self.group_id,
+                project_id=self.project_id,
                 username=self.no_username,
                 password=self.password,
             )
 
     @patch("pasqal_cloud.client.getpass")
     def test_module_no_password(self, getpass):
         getpass.return_value = ""
         with pytest.raises(ValueError):
             SDK(
-                group_id=self.group_id,
+                project_id=self.project_id,
                 username=self.username,
                 password=self.no_password,
             )
 
     @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_no_password(self, getpass):
         getpass.return_value = self.no_password
 
         with pytest.raises(ValueError):
-            SDK(group_id=self.group_id, username=self.username)
+            SDK(project_id=self.project_id, username=self.username)
 
         getpass.assert_called_once()
 
     def test_bad_token_provider(self):
         with pytest.raises(TypeError):
-            SDK(group_id=self.group_id, token_provider="token")
+            SDK(project_id=self.project_id, token_provider="token")
 
     def test_bad_auth0(self):
         with pytest.raises(TypeError):
             SDK(
-                group_id=self.group_id,
+                project_id=self.project_id,
                 username=self.username,
                 password=self.password,
                 auth0="",
             )
 
     def test_authentication_no_credentials_provided(self):
         with pytest.raises(ValueError):
-            SDK(group_id=self.group_id)
+            SDK(project_id=self.project_id)
 
     def test_bad_endpoints(self):
         with pytest.raises(TypeError):
             SDK(
-                group_id=self.group_id,
+                project_id=self.project_id,
                 username=self.username,
                 password=self.password,
                 endpoints={
                     "core": "",
                     "account": "",
                 },
             )
```

### Comparing `pasqal-cloud-0.2.5/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.2.6/tests/test_cloud_sdk_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-import warnings
 
 import pytest
 
 """
 Tests written to verify if the backward compatibility is working between the new name of the package `pasqal-cloud` 
 and its main folder renamed to `pasqal_cloud` and the previous package name that was `pasqal-cloud` 
 with the former folder called `sdk`.
```

### Comparing `pasqal-cloud-0.2.5/tests/test_config.py` & `pasqal-cloud-0.2.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.5/tests/test_device_specs.py` & `pasqal-cloud-0.2.6/tests/test_device_specs.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class TestDeviceSpecs:
     @pytest.fixture(autouse=True)
     @patch("sdk.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
     def init_sdk(self, start_mock_request):
         self.sdk = SDK(
-            username="me@test.com", password="password", group_id=str(uuid4())
+            username="me@test.com", password="password", project_id=str(uuid4())
         )
 
     def test_get_device_specs_success(self):
         device_specs_dict = self.sdk.get_device_specs_dict()
         assert type(device_specs_dict) == dict
         specs = device_specs_dict["FRESNEL"]
         json.loads(specs)
```

### Comparing `pasqal-cloud-0.2.5/tests/test_doubles/authentication.py` & `pasqal-cloud-0.2.6/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

