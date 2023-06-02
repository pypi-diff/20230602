# Comparing `tmp/pointstorm-1.1.4.tar.gz` & `tmp/pointstorm-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointstorm-1.1.4.tar", last modified: Fri Jun  2 19:49:59 2023, max compression
+gzip compressed data, was "pointstorm-1.1.5.tar", last modified: Fri Jun  2 21:12:53 2023, max compression
```

## Comparing `pointstorm-1.1.4.tar` & `pointstorm-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.724818 pointstorm-1.1.4/
--rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.4/LICENSE
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 19:49:59.724614 pointstorm-1.1.4/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.4/README.md
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.721956 pointstorm-1.1.4/pointstorm/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.4/pointstorm/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.4/pointstorm/config.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723030 pointstorm-1.1.4/pointstorm/destinations/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.4/pointstorm/destinations/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723641 pointstorm-1.1.4/pointstorm/embedding/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.4/pointstorm/embedding/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.4/pointstorm/embedding/abstract.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.4/pointstorm/embedding/image.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.4/pointstorm/embedding/text.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.4/pointstorm/embedding/time.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723740 pointstorm-1.1.4/pointstorm/ingestion/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.4/pointstorm/ingestion/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.723945 pointstorm-1.1.4/pointstorm/ingestion/cdc/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.4/pointstorm/ingestion/cdc/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.4/pointstorm/ingestion/cdc/debezium.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.724357 pointstorm-1.1.4/pointstorm/ingestion/event/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.4/pointstorm/ingestion/event/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)     3732 2023-06-02 19:44:33.000000 pointstorm-1.1.4/pointstorm/ingestion/event/kafka.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.4/pointstorm/monitoring.py
--rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.4/pointstorm/reference_db.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 19:49:59.722881 pointstorm-1.1.4/pointstorm.egg-info/
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/SOURCES.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/dependency_links.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/requires.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-02 19:49:59.000000 pointstorm-1.1.4/pointstorm.egg-info/top_level.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.4/pyproject.toml
--rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-02 19:49:59.724869 pointstorm-1.1.4/setup.cfg
--rw-r--r--   0 tesfa      (501) staff       (20)     1010 2023-05-20 01:20:43.000000 pointstorm-1.1.4/setup.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.087507 pointstorm-1.1.5/
+-rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.5/LICENSE
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:12:53.087325 pointstorm-1.1.5/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.5/README.md
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.084813 pointstorm-1.1.5/pointstorm/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.5/pointstorm/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.5/pointstorm/config.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.085652 pointstorm-1.1.5/pointstorm/destinations/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.5/pointstorm/destinations/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.086176 pointstorm-1.1.5/pointstorm/embedding/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.5/pointstorm/embedding/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.5/pointstorm/embedding/abstract.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.5/pointstorm/embedding/image.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.5/pointstorm/embedding/text.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.5/pointstorm/embedding/time.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.086380 pointstorm-1.1.5/pointstorm/ingestion/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.5/pointstorm/ingestion/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.086623 pointstorm-1.1.5/pointstorm/ingestion/cdc/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.5/pointstorm/ingestion/cdc/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.5/pointstorm/ingestion/cdc/debezium.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.086989 pointstorm-1.1.5/pointstorm/ingestion/event/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.5/pointstorm/ingestion/event/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     3732 2023-06-02 19:44:33.000000 pointstorm-1.1.5/pointstorm/ingestion/event/kafka.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.5/pointstorm/monitoring.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.5/pointstorm/reference_db.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:12:53.085540 pointstorm-1.1.5/pointstorm.egg-info/
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:12:53.000000 pointstorm-1.1.5/pointstorm.egg-info/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-06-02 21:12:53.000000 pointstorm-1.1.5/pointstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-02 21:12:53.000000 pointstorm-1.1.5/pointstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-06-02 21:12:53.000000 pointstorm-1.1.5/pointstorm.egg-info/requires.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-02 21:12:53.000000 pointstorm-1.1.5/pointstorm.egg-info/top_level.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.5/pyproject.toml
+-rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-02 21:12:53.087554 pointstorm-1.1.5/setup.cfg
+-rw-r--r--   0 tesfa      (501) staff       (20)     1010 2023-05-20 01:20:43.000000 pointstorm-1.1.5/setup.py
```

### Comparing `pointstorm-1.1.4/LICENSE` & `pointstorm-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.4/PKG-INFO` & `pointstorm-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.4
+Version: 1.1.5
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.4/README.md` & `pointstorm-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.4/pointstorm/ingestion/event/kafka.py` & `pointstorm-1.1.5/pointstorm/ingestion/event/kafka.py`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.4/pointstorm.egg-info/PKG-INFO` & `pointstorm-1.1.5/pointstorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.4
+Version: 1.1.5
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.4/pointstorm.egg-info/SOURCES.txt` & `pointstorm-1.1.5/pointstorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.4/setup.py` & `pointstorm-1.1.5/setup.py`

 * *Files identical despite different names*

