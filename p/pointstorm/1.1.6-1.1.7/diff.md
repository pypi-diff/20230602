# Comparing `tmp/pointstorm-1.1.6.tar.gz` & `tmp/pointstorm-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointstorm-1.1.6.tar", last modified: Fri Jun  2 21:17:53 2023, max compression
+gzip compressed data, was "pointstorm-1.1.7.tar", last modified: Fri Jun  2 21:23:16 2023, max compression
```

## Comparing `pointstorm-1.1.6.tar` & `pointstorm-1.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.854223 pointstorm-1.1.6/
--rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.6/LICENSE
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:17:53.854045 pointstorm-1.1.6/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.6/README.md
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.851771 pointstorm-1.1.6/pointstorm/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.6/pointstorm/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.6/pointstorm/config.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.852680 pointstorm-1.1.6/pointstorm/destinations/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.6/pointstorm/destinations/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.853231 pointstorm-1.1.6/pointstorm/embedding/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.6/pointstorm/embedding/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.6/pointstorm/embedding/abstract.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.6/pointstorm/embedding/image.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.6/pointstorm/embedding/text.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.6/pointstorm/embedding/time.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.853348 pointstorm-1.1.6/pointstorm/ingestion/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.6/pointstorm/ingestion/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.853586 pointstorm-1.1.6/pointstorm/ingestion/cdc/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.6/pointstorm/ingestion/cdc/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.6/pointstorm/ingestion/cdc/debezium.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.853809 pointstorm-1.1.6/pointstorm/ingestion/event/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.6/pointstorm/ingestion/event/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)     3732 2023-06-02 19:44:33.000000 pointstorm-1.1.6/pointstorm/ingestion/event/kafka.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.6/pointstorm/monitoring.py
--rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.6/pointstorm/reference_db.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:17:53.852504 pointstorm-1.1.6/pointstorm.egg-info/
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:17:53.000000 pointstorm-1.1.6/pointstorm.egg-info/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-06-02 21:17:53.000000 pointstorm-1.1.6/pointstorm.egg-info/SOURCES.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-02 21:17:53.000000 pointstorm-1.1.6/pointstorm.egg-info/dependency_links.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-06-02 21:17:53.000000 pointstorm-1.1.6/pointstorm.egg-info/requires.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-02 21:17:53.000000 pointstorm-1.1.6/pointstorm.egg-info/top_level.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.6/pyproject.toml
--rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-02 21:17:53.854267 pointstorm-1.1.6/setup.cfg
--rw-r--r--   0 tesfa      (501) staff       (20)     1010 2023-06-02 21:16:30.000000 pointstorm-1.1.6/setup.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.728742 pointstorm-1.1.7/
+-rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.7/LICENSE
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:23:16.728578 pointstorm-1.1.7/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.7/README.md
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.726433 pointstorm-1.1.7/pointstorm/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.7/pointstorm/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.7/pointstorm/config.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727236 pointstorm-1.1.7/pointstorm/destinations/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.7/pointstorm/destinations/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727785 pointstorm-1.1.7/pointstorm/embedding/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.7/pointstorm/embedding/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.7/pointstorm/embedding/abstract.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.7/pointstorm/embedding/image.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.7/pointstorm/embedding/text.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.7/pointstorm/embedding/time.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727902 pointstorm-1.1.7/pointstorm/ingestion/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.7/pointstorm/ingestion/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.728129 pointstorm-1.1.7/pointstorm/ingestion/cdc/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.7/pointstorm/ingestion/cdc/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.7/pointstorm/ingestion/cdc/debezium.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.728359 pointstorm-1.1.7/pointstorm/ingestion/event/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.7/pointstorm/ingestion/event/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     3732 2023-06-02 19:44:33.000000 pointstorm-1.1.7/pointstorm/ingestion/event/kafka.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.7/pointstorm/monitoring.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.7/pointstorm/reference_db.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727090 pointstorm-1.1.7/pointstorm.egg-info/
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/requires.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/top_level.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.7/pyproject.toml
+-rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-02 21:23:16.728785 pointstorm-1.1.7/setup.cfg
+-rw-r--r--   0 tesfa      (501) staff       (20)     1010 2023-06-02 21:21:33.000000 pointstorm-1.1.7/setup.py
```

### Comparing `pointstorm-1.1.6/LICENSE` & `pointstorm-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.6/PKG-INFO` & `pointstorm-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.6
+Version: 1.1.7
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.6/README.md` & `pointstorm-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.6/pointstorm/ingestion/event/kafka.py` & `pointstorm-1.1.7/pointstorm/ingestion/event/kafka.py`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.6/pointstorm.egg-info/PKG-INFO` & `pointstorm-1.1.7/pointstorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.6
+Version: 1.1.7
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.6/pointstorm.egg-info/SOURCES.txt` & `pointstorm-1.1.7/pointstorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.6/setup.py` & `pointstorm-1.1.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     description="Embedding vectors for data on the move",
     author="xsfa",
     author_email="tesfaaog@gmail.com",
     url="https://github.com/xsfa/pointstorm",
     packages=find_packages(),
     install_requires=[
         'bytewax==0.16.0',
-        'requests>=2.31.0',
+        'requests>=2.28.0',
         'kafka-python==2.0.2',
         'confluent-kafka',
         'faker',
         'transformers',
         'torch'
     ],
     classifiers=[
```

