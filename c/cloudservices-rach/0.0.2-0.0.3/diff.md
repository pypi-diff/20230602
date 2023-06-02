# Comparing `tmp/cloudservices_rach-0.0.2.tar.gz` & `tmp/cloudservices_rach-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudservices_rach-0.0.2.tar", last modified: Fri Jun  2 09:49:28 2023, max compression
+gzip compressed data, was "cloudservices_rach-0.0.3.tar", last modified: Fri Jun  2 09:55:56 2023, max compression
```

## Comparing `cloudservices_rach-0.0.2.tar` & `cloudservices_rach-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-06-02 09:49:28.918148 cloudservices_rach-0.0.2/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      605 2023-06-02 09:49:28.918148 cloudservices_rach-0.0.2/PKG-INFO
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-06-02 09:49:28.918148 cloudservices_rach-0.0.2/cloudservices_rach/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       92 2023-06-02 09:48:50.000000 cloudservices_rach-0.0.2/cloudservices_rach/__init__.py
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      565 2023-06-01 07:02:02.000000 cloudservices_rach-0.0.2/cloudservices_rach/cloud_config.py
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     5410 2023-06-02 09:46:23.000000 cloudservices_rach-0.0.2/cloudservices_rach/pubsub.py
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     4458 2023-06-02 09:41:55.000000 cloudservices_rach-0.0.2/cloudservices_rach/queue.py
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     4619 2023-06-02 09:47:01.000000 cloudservices_rach-0.0.2/cloudservices_rach/sqs.py
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     5295 2023-06-02 09:41:56.000000 cloudservices_rach-0.0.2/cloudservices_rach/storage.py
-drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-06-02 09:49:28.918148 cloudservices_rach-0.0.2/cloudservices_rach.egg-info/
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      605 2023-06-02 09:49:28.000000 cloudservices_rach-0.0.2/cloudservices_rach.egg-info/PKG-INFO
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      396 2023-06-02 09:49:28.000000 cloudservices_rach-0.0.2/cloudservices_rach.egg-info/SOURCES.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)        1 2023-06-02 09:49:28.000000 cloudservices_rach-0.0.2/cloudservices_rach.egg-info/dependency_links.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      120 2023-06-02 09:49:28.000000 cloudservices_rach-0.0.2/cloudservices_rach.egg-info/requires.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       19 2023-06-02 09:49:28.000000 cloudservices_rach-0.0.2/cloudservices_rach.egg-info/top_level.txt
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       38 2023-06-02 09:49:28.918148 cloudservices_rach-0.0.2/setup.cfg
--rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      847 2023-06-02 09:48:59.000000 cloudservices_rach-0.0.2/setup.py
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-06-02 09:55:56.579477 cloudservices_rach-0.0.3/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      605 2023-06-02 09:55:56.579477 cloudservices_rach-0.0.3/PKG-INFO
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-06-02 09:55:56.579477 cloudservices_rach-0.0.3/cloudservices_rach/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       92 2023-06-02 09:48:50.000000 cloudservices_rach-0.0.3/cloudservices_rach/__init__.py
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      565 2023-06-01 07:02:02.000000 cloudservices_rach-0.0.3/cloudservices_rach/cloud_config.py
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     5410 2023-06-02 09:46:23.000000 cloudservices_rach-0.0.3/cloudservices_rach/pubsub.py
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     4458 2023-06-02 09:41:55.000000 cloudservices_rach-0.0.3/cloudservices_rach/queue.py
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     4619 2023-06-02 09:47:01.000000 cloudservices_rach-0.0.3/cloudservices_rach/sqs.py
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)     5295 2023-06-02 09:41:56.000000 cloudservices_rach-0.0.3/cloudservices_rach/storage.py
+drwxrwxr-x   0 r-mhjn    (1000) r-mhjn    (1000)        0 2023-06-02 09:55:56.579477 cloudservices_rach-0.0.3/cloudservices_rach.egg-info/
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      605 2023-06-02 09:55:56.000000 cloudservices_rach-0.0.3/cloudservices_rach.egg-info/PKG-INFO
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      396 2023-06-02 09:55:56.000000 cloudservices_rach-0.0.3/cloudservices_rach.egg-info/SOURCES.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)        1 2023-06-02 09:55:56.000000 cloudservices_rach-0.0.3/cloudservices_rach.egg-info/dependency_links.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      137 2023-06-02 09:55:56.000000 cloudservices_rach-0.0.3/cloudservices_rach.egg-info/requires.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       19 2023-06-02 09:55:56.000000 cloudservices_rach-0.0.3/cloudservices_rach.egg-info/top_level.txt
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)       38 2023-06-02 09:55:56.579477 cloudservices_rach-0.0.3/setup.cfg
+-rw-rw-r--   0 r-mhjn    (1000) r-mhjn    (1000)      867 2023-06-02 09:55:41.000000 cloudservices_rach-0.0.3/setup.py
```

### Comparing `cloudservices_rach-0.0.2/PKG-INFO` & `cloudservices_rach-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudservices_rach
-Version: 0.0.2
+Version: 0.0.3
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudservices_rach-0.0.2/cloudservices_rach/cloud_config.py` & `cloudservices_rach-0.0.3/cloudservices_rach/cloud_config.py`

 * *Files identical despite different names*

### Comparing `cloudservices_rach-0.0.2/cloudservices_rach/pubsub.py` & `cloudservices_rach-0.0.3/cloudservices_rach/pubsub.py`

 * *Files identical despite different names*

### Comparing `cloudservices_rach-0.0.2/cloudservices_rach/queue.py` & `cloudservices_rach-0.0.3/cloudservices_rach/queue.py`

 * *Files identical despite different names*

### Comparing `cloudservices_rach-0.0.2/cloudservices_rach/sqs.py` & `cloudservices_rach-0.0.3/cloudservices_rach/sqs.py`

 * *Files identical despite different names*

### Comparing `cloudservices_rach-0.0.2/cloudservices_rach/storage.py` & `cloudservices_rach-0.0.3/cloudservices_rach/storage.py`

 * *Files identical despite different names*

### Comparing `cloudservices_rach-0.0.2/cloudservices_rach.egg-info/PKG-INFO` & `cloudservices_rach-0.0.3/cloudservices_rach.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudservices-rach
-Version: 0.0.2
+Version: 0.0.3
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudservices_rach-0.0.2/setup.py` & `cloudservices_rach-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='cloudservices_rach',
-    version='0.0.2',
+    version='0.0.3',
     description='A sample Python project for rach pack',
     author='Rac',
     author_email='rachitmahajan6399@gmail.com',
     url='https://github.com/r-mhjn/QuizCreator',
     packages=['cloudservices_rach'],
-    install_requires=['google-auth==2.17.3','google-cloud-pubsub==2.13.0','boto3==1.14.60','botocore==1.17.60','apache-libcloud==3.7.0','PyPubSub==4.0.3'],
+    install_requires=['google-auth==2.17.3','google-cloud-pubsub==2.13.0','boto3==1.14.60','botocore==1.17.60','apache-libcloud==3.7.0','PyPubSub==4.0.3', 'pyparsing==3.0.9'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

