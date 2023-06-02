# Comparing `tmp/wicker-0.0.5.1.tar.gz` & `tmp/wicker-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicker-0.0.5.1.tar", last modified: Fri Jun  2 13:51:19 2023, max compression
+gzip compressed data, was "wicker-0.0.5a0.tar", last modified: Tue May 30 22:32:54 2023, max compression
```

## Comparing `wicker-0.0.5.1.tar` & `wicker-0.0.5a0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.414886 wicker-0.0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 13:51:11.000000 wicker-0.0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 13:51:11.000000 wicker-0.0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-02 13:51:19.414886 wicker-0.0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-02 13:51:11.000000 wicker-0.0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 13:51:11.000000 wicker-0.0.5.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-02 13:51:11.000000 wicker-0.0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-02 13:51:19.414886 wicker-0.0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 13:51:11.000000 wicker-0.0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.414886 wicker-0.0.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.406886 wicker-0.0.5.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/core/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    21017 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_column_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_numpy_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_s3_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-02 13:51:11.000000 wicker-0.0.5.1/tests/test_wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.406886 wicker-0.0.5.1/wicker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.410886 wicker-0.0.5.1/wicker/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/column_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/persistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.410886 wicker-0.0.5.1/wicker/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/plugins/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/plugins/flyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/plugins/spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/plugins/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.410886 wicker-0.0.5.1/wicker/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/schema/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/schema/dataloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/schema/dataparsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/schema/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/schema/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.410886 wicker-0.0.5.1/wicker/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/testing/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-02 13:51:11.000000 wicker-0.0.5.1/wicker/testing/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:51:19.414886 wicker-0.0.5.1/wicker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-02 13:51:19.000000 wicker-0.0.5.1/wicker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-02 13:51:19.000000 wicker-0.0.5.1/wicker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:51:19.000000 wicker-0.0.5.1/wicker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 13:51:19.000000 wicker-0.0.5.1/wicker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 13:51:19.000000 wicker-0.0.5.1/wicker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.101565 wicker-0.0.5a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 22:32:46.000000 wicker-0.0.5a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 22:32:46.000000 wicker-0.0.5a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 22:32:54.101565 wicker-0.0.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-30 22:32:46.000000 wicker-0.0.5a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 22:32:46.000000 wicker-0.0.5a0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-30 22:32:46.000000 wicker-0.0.5a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-30 22:32:54.101565 wicker-0.0.5a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 22:32:46.000000 wicker-0.0.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.101565 wicker-0.0.5a0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/core/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21017 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_column_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_numpy_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_s3_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-30 22:32:46.000000 wicker-0.0.5a0/tests/test_wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/column_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/persistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/flyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/plugins/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/dataloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/dataparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/schema/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.097565 wicker-0.0.5a0/wicker/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/testing/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-30 22:32:46.000000 wicker-0.0.5a0/wicker/testing/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:32:54.101565 wicker-0.0.5a0/wicker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 22:32:54.000000 wicker-0.0.5a0/wicker.egg-info/top_level.txt
```

### Comparing `wicker-0.0.5.1/LICENSE` & `wicker-0.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/PKG-INFO` & `wicker-0.0.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicker
-Version: 0.0.5.1
+Version: 0.0.5a0
 Summary: An open source framework for Machine Learning dataset storage and serving
 Home-page: https://github.com/woven-planet/Wicker
 Author: Jay Chia
 Author-email: jaychia94@gmail.com
 Project-URL: Bug Tracker, https://github.com/woven-planet/Wicker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wicker-0.0.5.1/README.md` & `wicker-0.0.5a0/README.md`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/setup.cfg` & `wicker-0.0.5a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/core/test_persistence.py` & `wicker-0.0.5a0/tests/core/test_persistence.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_avro_schema.py` & `wicker-0.0.5a0/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_column_files.py` & `wicker-0.0.5a0/tests/test_column_files.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_datasets.py` & `wicker-0.0.5a0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_filelock.py` & `wicker-0.0.5a0/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_numpy_codec.py` & `wicker-0.0.5a0/tests/test_numpy_codec.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_s3_storage.py` & `wicker-0.0.5a0/tests/test_s3_storage.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_shuffle.py` & `wicker-0.0.5a0/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_spark.py` & `wicker-0.0.5a0/tests/test_spark.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/tests/test_wandb.py` & `wicker-0.0.5a0/tests/test_wandb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/column_files.py` & `wicker-0.0.5a0/wicker/core/column_files.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/config.py` & `wicker-0.0.5a0/wicker/core/config.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/datasets.py` & `wicker-0.0.5a0/wicker/core/datasets.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/definitions.py` & `wicker-0.0.5a0/wicker/core/definitions.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/filelock.py` & `wicker-0.0.5a0/wicker/core/filelock.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/persistance.py` & `wicker-0.0.5a0/wicker/core/persistance.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/shuffle.py` & `wicker-0.0.5a0/wicker/core/shuffle.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/storage.py` & `wicker-0.0.5a0/wicker/core/storage.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/core/writer.py` & `wicker-0.0.5a0/wicker/core/writer.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/plugins/dynamodb.py` & `wicker-0.0.5a0/wicker/plugins/dynamodb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/plugins/flyte.py` & `wicker-0.0.5a0/wicker/plugins/flyte.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/plugins/spark.py` & `wicker-0.0.5a0/wicker/plugins/spark.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/plugins/wandb.py` & `wicker-0.0.5a0/wicker/plugins/wandb.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/schema/codecs.py` & `wicker-0.0.5a0/wicker/schema/codecs.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/schema/dataloading.py` & `wicker-0.0.5a0/wicker/schema/dataloading.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/schema/dataparsing.py` & `wicker-0.0.5a0/wicker/schema/dataparsing.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/schema/schema.py` & `wicker-0.0.5a0/wicker/schema/schema.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/schema/serialization.py` & `wicker-0.0.5a0/wicker/schema/serialization.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/schema/validation.py` & `wicker-0.0.5a0/wicker/schema/validation.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/testing/codecs.py` & `wicker-0.0.5a0/wicker/testing/codecs.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker/testing/storage.py` & `wicker-0.0.5a0/wicker/testing/storage.py`

 * *Files identical despite different names*

### Comparing `wicker-0.0.5.1/wicker.egg-info/PKG-INFO` & `wicker-0.0.5a0/wicker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicker
-Version: 0.0.5.1
+Version: 0.0.5a0
 Summary: An open source framework for Machine Learning dataset storage and serving
 Home-page: https://github.com/woven-planet/Wicker
 Author: Jay Chia
 Author-email: jaychia94@gmail.com
 Project-URL: Bug Tracker, https://github.com/woven-planet/Wicker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wicker-0.0.5.1/wicker.egg-info/SOURCES.txt` & `wicker-0.0.5a0/wicker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

