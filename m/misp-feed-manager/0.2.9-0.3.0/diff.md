# Comparing `tmp/misp-feed-manager-0.2.9.tar.gz` & `tmp/misp-feed-manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misp-feed-manager-0.2.9.tar", last modified: Wed May 31 10:52:02 2023, max compression
+gzip compressed data, was "misp-feed-manager-0.3.0.tar", last modified: Fri Jun  2 09:13:14 2023, max compression
```

## Comparing `misp-feed-manager-0.2.9.tar` & `misp-feed-manager-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:52:02.518235 misp-feed-manager-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-31 10:52:02.518235 misp-feed-manager-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:52:02.514235 misp-feed-manager-0.2.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4436 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/bin/consume_feed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/bin/generate_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-31 10:52:02.518235 misp-feed-manager-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:52:02.514235 misp-feed-manager-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:52:02.518235 misp-feed-manager-0.2.9/src/feed_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/src/feed_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/src/feed_manager/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/src/feed_manager/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/src/feed_manager/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/src/feed_manager/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:52:02.518235 misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-31 10:52:02.000000 misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-31 10:52:02.000000 misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:52:02.000000 misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 10:52:02.000000 misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 10:52:02.000000 misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:52:02.518235 misp-feed-manager-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-31 10:51:52.000000 misp-feed-manager-0.2.9/tests/test_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4436 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/bin/consume_feed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/bin/generate_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/src/feed_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14623 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/tests/test_translator.py
```

### Comparing `misp-feed-manager-0.2.9/LICENSE` & `misp-feed-manager-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/PKG-INFO` & `misp-feed-manager-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misp-feed-manager
-Version: 0.2.9
+Version: 0.3.0
 Summary: Set of utilities to manage MISP feeds
 Home-page: https://github.com/vmware-labs/feed-manager-for-misp/
 Author: Stefano Ortolani
 Project-URL: Bug Tracker, https://github.com/vmware-labs/feed-manager-for-misp/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `misp-feed-manager-0.2.9/README.md` & `misp-feed-manager-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/bin/consume_feed.py` & `misp-feed-manager-0.3.0/bin/consume_feed.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/bin/generate_feed.py` & `misp-feed-manager-0.3.0/bin/generate_feed.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/pyproject.toml` & `misp-feed-manager-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/setup.cfg` & `misp-feed-manager-0.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = misp-feed-manager
-version = 0.2.9
+version = 0.3.0
 author = Stefano Ortolani
 description = Set of utilities to manage MISP feeds
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vmware-labs/feed-manager-for-misp/
 project_urls = 
 	Bug Tracker = https://github.com/vmware-labs/feed-manager-for-misp/issues
```

### Comparing `misp-feed-manager-0.2.9/src/feed_manager/__init__.py` & `misp-feed-manager-0.3.0/src/feed_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/src/feed_manager/consumer.py` & `misp-feed-manager-0.3.0/src/feed_manager/consumer.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/src/feed_manager/generator.py` & `misp-feed-manager-0.3.0/src/feed_manager/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     @abc.abstractmethod
     def parse_bucket(cls, date_str: str) -> datetime.datetime:
         """Given a bucket return the date time object."""
 
     @classmethod
     def get_bucket_from_timestamp(cls, timestamp: int) -> str:
         """Get the bucket given a timestamp."""
-        return cls.get_bucket(datetime.datetime.fromtimestamp(timestamp))
+        return cls.get_bucket(datetime.datetime.utcfromtimestamp(timestamp))
 
     @classmethod
     def get_event_metadata(
         cls,
         manifest: Dict,
         event_bucket: Optional[str] = None,
     ) -> FeedEventMetadata:
@@ -396,8 +396,10 @@
             second=0,
             microsecond=0,
         ).strftime(cls.BUCKET_FMT)
 
     @classmethod
     def parse_bucket(cls, date_str: str) -> datetime.datetime:
         """Implement interface"""
-        return datetime.datetime.strptime(date_str, cls.BUCKET_FMT)
+        return datetime.datetime.strptime(date_str, cls.BUCKET_FMT).replace(
+            tzinfo=datetime.timezone.utc
+        )
```

### Comparing `misp-feed-manager-0.2.9/src/feed_manager/storage.py` & `misp-feed-manager-0.3.0/src/feed_manager/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     path: Optional[str] = None,
     read_write: Optional[bool] = False,
 ):
     """Utility method to get the storage layer given some options."""
     logger = logging.getLogger(__name__)
     logger.info(
         "Creating storage layer with input_string='%s',path='%s',read_write=%s",
-        input_string, path, read_write,
+        input_string,
+        path,
+        read_write,
     )
 
     # http readers start with http
     if input_string.startswith("http"):
         return ReadOnlyHttpStorage(base_url=input_string)
 
     # local storage require a directory
```

### Comparing `misp-feed-manager-0.2.9/src/feed_manager/translator.py` & `misp-feed-manager-0.3.0/src/feed_manager/translator.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/PKG-INFO` & `misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misp-feed-manager
-Version: 0.2.9
+Version: 0.3.0
 Summary: Set of utilities to manage MISP feeds
 Home-page: https://github.com/vmware-labs/feed-manager-for-misp/
 Author: Stefano Ortolani
 Project-URL: Bug Tracker, https://github.com/vmware-labs/feed-manager-for-misp/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `misp-feed-manager-0.2.9/src/misp_feed_manager.egg-info/SOURCES.txt` & `misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/tests/test_storage.py` & `misp-feed-manager-0.3.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.2.9/tests/test_translator.py` & `misp-feed-manager-0.3.0/tests/test_translator.py`

 * *Files identical despite different names*

