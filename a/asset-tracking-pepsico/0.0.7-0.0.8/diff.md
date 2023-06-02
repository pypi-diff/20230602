# Comparing `tmp/asset_tracking_pepsico-0.0.7.tar.gz` & `tmp/asset_tracking_pepsico-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-0.0.7.tar", last modified: Wed May 31 15:55:06 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-0.0.8.tar", last modified: Fri Jun  2 09:25:59 2023, max compression
```

## Comparing `asset_tracking_pepsico-0.0.7.tar` & `asset_tracking_pepsico-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.353675 asset_tracking_pepsico-0.0.7/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.7/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:55:06.353241 asset_tracking_pepsico-0.0.7/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-0.0.7/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.349198 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4834 2023-05-31 15:34:12.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.352759 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6539 2023-05-31 15:54:17.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     3234 2023-05-31 14:40:13.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-31 15:55:06.352195 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       71 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-05-31 15:55:06.000000 asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      798 2023-05-31 15:54:41.000000 asset_tracking_pepsico-0.0.7/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-31 15:55:06.353822 asset_tracking_pepsico-0.0.7/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-02 09:25:59.616598 asset_tracking_pepsico-0.0.8/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-0.0.8/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-06-02 09:25:59.616308 asset_tracking_pepsico-0.0.8/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-0.0.8/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-02 09:25:59.612228 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4834 2023-05-31 15:34:12.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-02 09:25:59.615395 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6539 2023-05-31 15:54:17.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     3234 2023-05-31 14:40:13.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-02 09:25:59.614853 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-06-02 09:25:59.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-06-02 09:25:59.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-06-02 09:25:59.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       62 2023-06-02 09:25:59.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-06-02 09:25:59.000000 asset_tracking_pepsico-0.0.8/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      785 2023-06-02 09:24:14.000000 asset_tracking_pepsico-0.0.8/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-06-02 09:25:59.616708 asset_tracking_pepsico-0.0.8/setup.cfg
```

### Comparing `asset_tracking_pepsico-0.0.7/LICENSE` & `asset_tracking_pepsico-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.7/PKG-INFO` & `asset_tracking_pepsico-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_tracking_pepsico
-Version: 0.0.7
+Version: 0.0.8
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.7/README.md` & `asset_tracking_pepsico-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-0.0.8/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-0.0.7/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-0.0.8/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset-tracking-pepsico
-Version: 0.0.7
+Version: 0.0.8
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-0.0.7/pyproject.toml` & `asset_tracking_pepsico-0.0.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
 dependencies = [
   "azure-core",
   "azure-storage-blob",
   "requests",
   "requests-oauthlib",
   "toml",
-  "psycopg2"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 1 - Planning",
     "Operating System :: OS Independent",
 ]
```

