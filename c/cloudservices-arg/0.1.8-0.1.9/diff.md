# Comparing `tmp/cloudservices_arg-0.1.8.tar.gz` & `tmp/cloudservices_arg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudservices_arg-0.1.8.tar", last modified: Fri Jun  2 08:24:29 2023, max compression
+gzip compressed data, was "cloudservices_arg-0.1.9.tar", last modified: Fri Jun  2 09:51:21 2023, max compression
```

## Comparing `cloudservices_arg-0.1.8.tar` & `cloudservices_arg-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 08:24:29.810670 cloudservices_arg-0.1.8/
--rw-rw-rw-   0        0        0      562 2023-06-02 08:24:29.810171 cloudservices_arg-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 08:24:29.794166 cloudservices_arg-0.1.8/cloudservices_arg/
--rw-rw-rw-   0        0        0       80 2023-06-02 08:22:03.000000 cloudservices_arg-0.1.8/cloudservices_arg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:24:29.808168 cloudservices_arg-0.1.8/cloudservices_arg.egg-info/
--rw-rw-rw-   0        0        0      562 2023-06-02 08:24:29.000000 cloudservices_arg-0.1.8/cloudservices_arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-06-02 08:24:29.000000 cloudservices_arg-0.1.8/cloudservices_arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 08:24:29.000000 cloudservices_arg-0.1.8/cloudservices_arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-06-02 08:24:29.000000 cloudservices_arg-0.1.8/cloudservices_arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-02 08:24:29.000000 cloudservices_arg-0.1.8/cloudservices_arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 08:24:29.811170 cloudservices_arg-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-02 08:23:43.000000 cloudservices_arg-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:51:21.018020 cloudservices_arg-0.1.9/
+-rw-rw-rw-   0        0        0      562 2023-06-02 09:51:21.016009 cloudservices_arg-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 09:51:20.953268 cloudservices_arg-0.1.9/cloudservices_arg/
+-rw-rw-rw-   0        0        0       80 2023-06-02 08:22:03.000000 cloudservices_arg-0.1.9/cloudservices_arg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:51:21.003797 cloudservices_arg-0.1.9/cloudservices_arg/queueservice/
+-rw-rw-rw-   0        0        0       23 2023-06-02 08:43:35.000000 cloudservices_arg-0.1.9/cloudservices_arg/queueservice/__init__.py
+-rw-rw-rw-   0        0        0     5400 2023-06-02 07:46:21.000000 cloudservices_arg-0.1.9/cloudservices_arg/queueservice/pubsub.py
+-rw-rw-rw-   0        0        0     4446 2023-06-02 07:46:15.000000 cloudservices_arg-0.1.9/cloudservices_arg/queueservice/queue.py
+-rw-rw-rw-   0        0        0     4601 2023-06-02 07:46:39.000000 cloudservices_arg-0.1.9/cloudservices_arg/queueservice/sqs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:51:21.012925 cloudservices_arg-0.1.9/cloudservices_arg/storageservice/
+-rw-rw-rw-   0        0        0       27 2023-06-02 08:42:03.000000 cloudservices_arg-0.1.9/cloudservices_arg/storageservice/__init__.py
+-rw-rw-rw-   0        0        0     5283 2023-06-02 08:43:12.000000 cloudservices_arg-0.1.9/cloudservices_arg/storageservice/storage.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:51:20.990762 cloudservices_arg-0.1.9/cloudservices_arg.egg-info/
+-rw-rw-rw-   0        0        0      562 2023-06-02 09:51:20.000000 cloudservices_arg-0.1.9/cloudservices_arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-06-02 09:51:20.000000 cloudservices_arg-0.1.9/cloudservices_arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:51:20.000000 cloudservices_arg-0.1.9/cloudservices_arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2023-06-02 09:51:20.000000 cloudservices_arg-0.1.9/cloudservices_arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-02 09:51:20.000000 cloudservices_arg-0.1.9/cloudservices_arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:51:21.019021 cloudservices_arg-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      913 2023-06-02 09:51:11.000000 cloudservices_arg-0.1.9/setup.py
```

### Comparing `cloudservices_arg-0.1.8/PKG-INFO` & `cloudservices_arg-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudservices_arg
-Version: 0.1.8
+Version: 0.1.9
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudservices_arg-0.1.8/cloudservices_arg.egg-info/PKG-INFO` & `cloudservices_arg-0.1.9/cloudservices_arg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudservices-arg
-Version: 0.1.8
+Version: 0.1.9
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudservices_arg-0.1.8/setup.py` & `cloudservices_arg-0.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='cloudservices_arg',
-    version='0.1.8',
+    version='0.1.9',
     description='A sample Python project for rach pack',
     author='Rac',
     author_email='rachitmahajan6399@gmail.com',
     url='https://github.com/r-mhjn/QuizCreator',
-    packages=['cloudservices_arg'],
+    packages=['cloudservices_arg','cloudservices_arg.storageservice','cloudservices_arg.queueservice'],
     install_requires=['google-auth==2.17.3','google-cloud-pubsub==2.13.0','boto3==1.14.60','botocore==1.17.60','apache-libcloud==3.7.0','PyPubSub==4.0.3'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

