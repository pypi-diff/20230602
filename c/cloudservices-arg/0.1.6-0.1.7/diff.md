# Comparing `tmp/cloudservices_arg-0.1.6.tar.gz` & `tmp/cloudservices_arg-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudservices_arg-0.1.6.tar", last modified: Fri Jun  2 07:40:11 2023, max compression
+gzip compressed data, was "cloudservices_arg-0.1.7.tar", last modified: Fri Jun  2 07:50:16 2023, max compression
```

## Comparing `cloudservices_arg-0.1.6.tar` & `cloudservices_arg-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 07:40:11.830674 cloudservices_arg-0.1.6/
--rw-rw-rw-   0        0        0      562 2023-06-02 07:40:11.829206 cloudservices_arg-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 07:40:11.800970 cloudservices_arg-0.1.6/cloudservices_arg/
--rw-rw-rw-   0        0        0       68 2023-06-02 07:38:31.000000 cloudservices_arg-0.1.6/cloudservices_arg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 07:40:11.827160 cloudservices_arg-0.1.6/cloudservices_arg.egg-info/
--rw-rw-rw-   0        0        0      562 2023-06-02 07:40:11.000000 cloudservices_arg-0.1.6/cloudservices_arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-06-02 07:40:11.000000 cloudservices_arg-0.1.6/cloudservices_arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 07:40:11.000000 cloudservices_arg-0.1.6/cloudservices_arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-06-02 07:40:11.000000 cloudservices_arg-0.1.6/cloudservices_arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-02 07:40:11.000000 cloudservices_arg-0.1.6/cloudservices_arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 07:40:11.831165 cloudservices_arg-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-02 07:39:48.000000 cloudservices_arg-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:50:16.236681 cloudservices_arg-0.1.7/
+-rw-rw-rw-   0        0        0      562 2023-06-02 07:50:16.234580 cloudservices_arg-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 07:50:16.174536 cloudservices_arg-0.1.7/cloudservices_arg/
+-rw-rw-rw-   0        0        0      116 2023-06-02 07:49:11.000000 cloudservices_arg-0.1.7/cloudservices_arg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:50:16.231081 cloudservices_arg-0.1.7/cloudservices_arg.egg-info/
+-rw-rw-rw-   0        0        0      562 2023-06-02 07:50:15.000000 cloudservices_arg-0.1.7/cloudservices_arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-06-02 07:50:15.000000 cloudservices_arg-0.1.7/cloudservices_arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:50:15.000000 cloudservices_arg-0.1.7/cloudservices_arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2023-06-02 07:50:15.000000 cloudservices_arg-0.1.7/cloudservices_arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-02 07:50:15.000000 cloudservices_arg-0.1.7/cloudservices_arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 07:50:16.237183 cloudservices_arg-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-02 07:50:09.000000 cloudservices_arg-0.1.7/setup.py
```

### Comparing `cloudservices_arg-0.1.6/PKG-INFO` & `cloudservices_arg-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudservices_arg
-Version: 0.1.6
+Version: 0.1.7
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudservices_arg-0.1.6/cloudservices_arg.egg-info/PKG-INFO` & `cloudservices_arg-0.1.7/cloudservices_arg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudservices-arg
-Version: 0.1.6
+Version: 0.1.7
 Summary: A sample Python project for rach pack
 Home-page: https://github.com/r-mhjn/QuizCreator
 Author: Rac
 Author-email: rachitmahajan6399@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudservices_arg-0.1.6/setup.py` & `cloudservices_arg-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='cloudservices_arg',
-    version='0.1.6',
+    version='0.1.7',
     description='A sample Python project for rach pack',
     author='Rac',
     author_email='rachitmahajan6399@gmail.com',
     url='https://github.com/r-mhjn/QuizCreator',
     packages=['cloudservices_arg'],
     install_requires=['google-auth==2.17.3','google-cloud-pubsub==2.13.0','boto3==1.14.60','botocore==1.17.60','apache-libcloud==3.7.0','PyPubSub==4.0.3'],
     classifiers=[
```

