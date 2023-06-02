# Comparing `tmp/granica-sdk-2.1.8.tar.gz` & `tmp/granica-sdk-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granica-sdk-2.1.8.tar", last modified: Fri Jun  2 02:39:19 2023, max compression
+gzip compressed data, was "granica-sdk-2.1.9.tar", last modified: Fri Jun  2 03:13:09 2023, max compression
```

## Comparing `granica-sdk-2.1.8.tar` & `granica-sdk-2.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:19.524455 granica-sdk-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-02 02:39:09.000000 granica-sdk-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-02 02:39:19.524455 granica-sdk-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-02 02:39:09.000000 granica-sdk-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:19.520455 granica-sdk-2.1.8/granica/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4595 2023-06-02 02:39:09.000000 granica-sdk-2.1.8/granica/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10059 2023-06-02 02:39:09.000000 granica-sdk-2.1.8/granica/bolt_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:19.520455 granica-sdk-2.1.8/granica_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-02 02:39:19.000000 granica-sdk-2.1.8/granica_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 02:39:19.000000 granica-sdk-2.1.8/granica_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:39:19.000000 granica-sdk-2.1.8/granica_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 02:39:19.000000 granica-sdk-2.1.8/granica_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 02:39:19.000000 granica-sdk-2.1.8/granica_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 02:39:19.524455 granica-sdk-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-02 02:39:09.000000 granica-sdk-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:13:09.801947 granica-sdk-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-02 03:13:01.000000 granica-sdk-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-02 03:13:09.801947 granica-sdk-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-02 03:13:01.000000 granica-sdk-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:13:09.801947 granica-sdk-2.1.9/granica/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4595 2023-06-02 03:13:01.000000 granica-sdk-2.1.9/granica/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10059 2023-06-02 03:13:01.000000 granica-sdk-2.1.9/granica/bolt_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:13:09.801947 granica-sdk-2.1.9/granica_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-02 03:13:09.000000 granica-sdk-2.1.9/granica_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 03:13:09.000000 granica-sdk-2.1.9/granica_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:13:09.000000 granica-sdk-2.1.9/granica_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 03:13:09.000000 granica-sdk-2.1.9/granica_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 03:13:09.000000 granica-sdk-2.1.9/granica_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:13:09.801947 granica-sdk-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-02 03:13:01.000000 granica-sdk-2.1.9/setup.py
```

### Comparing `granica-sdk-2.1.8/LICENSE` & `granica-sdk-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `granica-sdk-2.1.8/PKG-INFO` & `granica-sdk-2.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: granica-sdk
-Version: 2.1.8
+Version: 2.1.9
 Summary: Granica Python SDK
 Home-page: https://gitlab.com/projectn-oss/projectn-bolt-python
 Author: Project N
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Granica SDK
 
-This SDK provides an authentication solution for programatically interacting with Granica. It wraps the boto3 interface so project wide integration is as easy as refactoring `import boto3` to `import bolt as boto3`.
+This SDK provides an authentication solution for programatically interacting with Granica. It wraps the boto3 interface so project wide integration is as easy as refactoring `import boto3` to `import granica as boto3`.
 
 The package affects the signing and routing protocol of the boto3 S3 client, therefore any non S3 clients created through this SDK will be un-affected by the wrapper.
 
 ## Prerequisites
 
 The minimum supported version of Python is version 3.
 
@@ -50,13 +50,23 @@
 
 ## Debugging
 
 Import the default logger and set its level to DEBUG
 
 `logging.getLogger().setLevel(logging.DEBUG)`
 
+## Example S3 GetObject
+
+```python
+import granica as boto3
+
+s3_client = boto3.client('s3')
+response = s3_client.get_object(Bucket='MyBucket', Key='MyKey.csv')
+obj = response['Body'].read()
+
+```
 
 ## Tests
 Basic integration tests are provided for the modified Session/Client interfaces. They must be run in an environment with a properly configured Granica deployment accessible.
 ```bash
 python3 tests/tests.py
 ```
```

### Comparing `granica-sdk-2.1.8/README.md` & `granica-sdk-2.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Granica SDK
 
-This SDK provides an authentication solution for programatically interacting with Granica. It wraps the boto3 interface so project wide integration is as easy as refactoring `import boto3` to `import bolt as boto3`.
+This SDK provides an authentication solution for programatically interacting with Granica. It wraps the boto3 interface so project wide integration is as easy as refactoring `import boto3` to `import granica as boto3`.
 
 The package affects the signing and routing protocol of the boto3 S3 client, therefore any non S3 clients created through this SDK will be un-affected by the wrapper.
 
 ## Prerequisites
 
 The minimum supported version of Python is version 3.
 
@@ -36,13 +36,23 @@
 
 ## Debugging
 
 Import the default logger and set its level to DEBUG
 
 `logging.getLogger().setLevel(logging.DEBUG)`
 
+## Example S3 GetObject
+
+```python
+import granica as boto3
+
+s3_client = boto3.client('s3')
+response = s3_client.get_object(Bucket='MyBucket', Key='MyKey.csv')
+obj = response['Body'].read()
+
+```
 
 ## Tests
 Basic integration tests are provided for the modified Session/Client interfaces. They must be run in an environment with a properly configured Granica deployment accessible.
 ```bash
 python3 tests/tests.py
 ```
```

### Comparing `granica-sdk-2.1.8/granica/__init__.py` & `granica-sdk-2.1.9/granica/__init__.py`

 * *Files identical despite different names*

### Comparing `granica-sdk-2.1.8/granica/bolt_router.py` & `granica-sdk-2.1.9/granica/bolt_router.py`

 * *Files identical despite different names*

### Comparing `granica-sdk-2.1.8/granica_sdk.egg-info/PKG-INFO` & `granica-sdk-2.1.9/granica_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: granica-sdk
-Version: 2.1.8
+Version: 2.1.9
 Summary: Granica Python SDK
 Home-page: https://gitlab.com/projectn-oss/projectn-bolt-python
 Author: Project N
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Granica SDK
 
-This SDK provides an authentication solution for programatically interacting with Granica. It wraps the boto3 interface so project wide integration is as easy as refactoring `import boto3` to `import bolt as boto3`.
+This SDK provides an authentication solution for programatically interacting with Granica. It wraps the boto3 interface so project wide integration is as easy as refactoring `import boto3` to `import granica as boto3`.
 
 The package affects the signing and routing protocol of the boto3 S3 client, therefore any non S3 clients created through this SDK will be un-affected by the wrapper.
 
 ## Prerequisites
 
 The minimum supported version of Python is version 3.
 
@@ -50,13 +50,23 @@
 
 ## Debugging
 
 Import the default logger and set its level to DEBUG
 
 `logging.getLogger().setLevel(logging.DEBUG)`
 
+## Example S3 GetObject
+
+```python
+import granica as boto3
+
+s3_client = boto3.client('s3')
+response = s3_client.get_object(Bucket='MyBucket', Key='MyKey.csv')
+obj = response['Body'].read()
+
+```
 
 ## Tests
 Basic integration tests are provided for the modified Session/Client interfaces. They must be run in an environment with a properly configured Granica deployment accessible.
 ```bash
 python3 tests/tests.py
 ```
```

### Comparing `granica-sdk-2.1.8/setup.py` & `granica-sdk-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='granica-sdk',
     packages=setuptools.find_packages(),
-    version='2.1.8',
+    version='2.1.9',
     description='Granica Python SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Project N',
     install_requires=requires,
     classifiers=[
         "Programming Language :: Python :: 3",
```

