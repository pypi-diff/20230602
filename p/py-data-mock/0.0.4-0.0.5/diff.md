# Comparing `tmp/py-data-mock-0.0.4.tar.gz` & `tmp/py-data-mock-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-data-mock-0.0.4.tar", last modified: Thu May 25 18:20:24 2023, max compression
+gzip compressed data, was "py-data-mock-0.0.5.tar", last modified: Fri Jun  2 03:59:15 2023, max compression
```

## Comparing `py-data-mock-0.0.4.tar` & `py-data-mock-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.618970 py-data-mock-0.0.4/
--rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-22 15:46:15.000000 py-data-mock-0.0.4/LICENSE
--rw-r--r--   0 phtremblay (2028354092) 932231305      363 2023-05-25 18:20:24.618848 py-data-mock-0.0.4/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305     4391 2023-05-25 18:15:17.000000 py-data-mock-0.0.4/README.md
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.615912 py-data-mock-0.0.4/data_mock/
--rw-r--r--   0 phtremblay (2028354092) 932231305       53 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305       43 2023-05-22 18:27:30.000000 py-data-mock-0.0.4/data_mock/exceptions.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.614560 py-data-mock-0.0.4/data_mock/google/
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.614757 py-data-mock-0.0.4/data_mock/google/cloud/
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.616834 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/
--rw-r--r--   0 phtremblay (2028354092) 932231305      827 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     6323 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/client.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      301 2023-05-22 15:46:15.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/dataset.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     1427 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/enums.py
--rw-r--r--   0 phtremblay (2028354092) 932231305       85 2023-05-22 15:46:15.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/exceptions.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.617173 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/job/
--rw-r--r--   0 phtremblay (2028354092) 932231305      329 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/job/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      350 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/job/load.py
--rw-r--r--   0 phtremblay (2028354092) 932231305       80 2023-05-22 15:46:15.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/job/query.py
--rw-r--r--   0 phtremblay (2028354092) 932231305       22 2023-05-22 15:46:15.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/retry.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      201 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/schema.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     3013 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/data_mock/google/cloud/bigquery/table.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.617623 py-data-mock-0.0.4/data_mock/google/cloud/storage/
--rw-r--r--   0 phtremblay (2028354092) 932231305      110 2023-05-23 16:32:26.000000 py-data-mock-0.0.4/data_mock/google/cloud/storage/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     1228 2023-05-23 16:32:26.000000 py-data-mock-0.0.4/data_mock/google/cloud/storage/blob.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      522 2023-05-23 16:32:26.000000 py-data-mock-0.0.4/data_mock/google/cloud/storage/bucket.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      445 2023-05-23 16:32:26.000000 py-data-mock-0.0.4/data_mock/google/cloud/storage/client.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.617841 py-data-mock-0.0.4/data_mock/mock_helpers/
--rw-r--r--   0 phtremblay (2028354092) 932231305     2238 2023-05-25 18:15:17.000000 py-data-mock-0.0.4/data_mock/mock_helpers/provider.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      116 2023-05-23 16:32:26.000000 py-data-mock-0.0.4/data_mock/mock_helpers/writer.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.617961 py-data-mock-0.0.4/data_mock/scripts/
--rw-r--r--   0 phtremblay (2028354092) 932231305     2245 2023-05-22 15:46:15.000000 py-data-mock-0.0.4/data_mock/scripts/mkmock.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.618452 py-data-mock-0.0.4/py_data_mock.egg-info/
--rw-r--r--   0 phtremblay (2028354092) 932231305      363 2023-05-25 18:20:24.000000 py-data-mock-0.0.4/py_data_mock.egg-info/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      968 2023-05-25 18:20:24.000000 py-data-mock-0.0.4/py_data_mock.egg-info/SOURCES.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-25 18:20:24.000000 py-data-mock-0.0.4/py_data_mock.egg-info/dependency_links.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305      132 2023-05-25 18:20:24.000000 py-data-mock-0.0.4/py_data_mock.egg-info/top_level.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-25 18:20:24.619008 py-data-mock-0.0.4/setup.cfg
--rw-r--r--   0 phtremblay (2028354092) 932231305      649 2023-05-25 18:20:10.000000 py-data-mock-0.0.4/setup.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-25 18:20:24.618572 py-data-mock-0.0.4/tests/
--rw-r--r--   0 phtremblay (2028354092) 932231305     1167 2023-05-22 15:46:15.000000 py-data-mock-0.0.4/tests/test1.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/
+-rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-05-20 20:50:55.000000 py-data-mock-0.0.5/LICENSE
+-rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4391 2023-05-24 05:45:14.000000 py-data-mock-0.0.5/README.md
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/
+-rw-rw-r--   0 henry     (1000) henry     (1000)       53 2023-05-26 05:01:26.000000 py-data-mock-0.0.5/data_mock/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       43 2023-05-23 07:44:51.000000 py-data-mock-0.0.5/data_mock/exceptions.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.925548 py-data-mock-0.0.5/data_mock/google/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      827 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     6323 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/client.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      301 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/dataset.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1427 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/enums.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       85 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/exceptions.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      329 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      350 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/load.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       80 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/query.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)       22 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/retry.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      865 2023-05-26 05:01:26.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/schema.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3013 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/table.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/storage/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      110 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1228 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/blob.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      522 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/bucket.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      445 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/client.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/mock_helpers/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     8025 2023-06-02 02:05:27.000000 py-data-mock-0.0.5/data_mock/mock_helpers/generate_data.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2238 2023-05-25 03:01:07.000000 py-data-mock-0.0.5/data_mock/mock_helpers/provider.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      116 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/mock_helpers/writer.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/data_mock/scripts/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2245 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/scripts/mkmock.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/py_data_mock.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1008 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      132 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/top_level.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/setup.cfg
+-rw-rw-r--   0 henry     (1000) henry     (1000)      649 2023-05-26 05:01:26.000000 py-data-mock-0.0.5/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/tests/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1167 2023-05-20 20:54:11.000000 py-data-mock-0.0.5/tests/test1.py
```

### Comparing `py-data-mock-0.0.4/LICENSE` & `py-data-mock-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/README.md` & `py-data-mock-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/google/cloud/bigquery/__init__.py` & `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/google/cloud/bigquery/client.py` & `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/google/cloud/bigquery/enums.py` & `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/enums.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/google/cloud/bigquery/table.py` & `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/google/cloud/storage/blob.py` & `py-data-mock-0.0.5/data_mock/google/cloud/storage/blob.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/google/cloud/storage/bucket.py` & `py-data-mock-0.0.5/data_mock/google/cloud/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/mock_helpers/provider.py` & `py-data-mock-0.0.5/data_mock/mock_helpers/provider.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/data_mock/scripts/mkmock.py` & `py-data-mock-0.0.5/data_mock/scripts/mkmock.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.4/py_data_mock.egg-info/SOURCES.txt` & `py-data-mock-0.0.5/py_data_mock.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 data_mock/google/cloud/bigquery/job/__init__.py
 data_mock/google/cloud/bigquery/job/load.py
 data_mock/google/cloud/bigquery/job/query.py
 data_mock/google/cloud/storage/__init__.py
 data_mock/google/cloud/storage/blob.py
 data_mock/google/cloud/storage/bucket.py
 data_mock/google/cloud/storage/client.py
+data_mock/mock_helpers/generate_data.py
 data_mock/mock_helpers/provider.py
 data_mock/mock_helpers/writer.py
 data_mock/scripts/mkmock.py
 py_data_mock.egg-info/PKG-INFO
 py_data_mock.egg-info/SOURCES.txt
 py_data_mock.egg-info/dependency_links.txt
 py_data_mock.egg-info/top_level.txt
```

### Comparing `py-data-mock-0.0.4/setup.py` & `py-data-mock-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='py-data-mock',
-    version='0.0.4',    
+    version='0.0.5',    
     scripts=['data_mock/scripts/mkmock.py'],
     description='Mock Data',
     url='https://github.com/paulhtremblay/py-data-mock',
     author='Henry Tremblay',
     author_email='paulhtremblay@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['data_mock/google/cloud/bigquery/job', 'data_mock/google/cloud/bigquery',
```

### Comparing `py-data-mock-0.0.4/tests/test1.py` & `py-data-mock-0.0.5/tests/test1.py`

 * *Files identical despite different names*

