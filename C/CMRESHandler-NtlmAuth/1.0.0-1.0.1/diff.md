# Comparing `tmp/CMRESHandler-NtlmAuth-1.0.0.tar.gz` & `tmp/CMRESHandler-NtlmAuth-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMRESHandler-NtlmAuth-1.0.0.tar", last modified: Mon May 22 10:34:34 2023, max compression
+gzip compressed data, was "CMRESHandler-NtlmAuth-1.0.1.tar", last modified: Fri Jun  2 10:34:10 2023, max compression
```

## Comparing `CMRESHandler-NtlmAuth-1.0.0.tar` & `CMRESHandler-NtlmAuth-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:34:34.938430 CMRESHandler-NtlmAuth-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-22 10:34:34.920319 CMRESHandler-NtlmAuth-1.0.0/CMRESHandler_NtlmAuth.egg-info/
--rw-rw-rw-   0        0        0    10733 2023-05-22 10:34:34.000000 CMRESHandler-NtlmAuth-1.0.0/CMRESHandler_NtlmAuth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-05-22 10:34:34.000000 CMRESHandler-NtlmAuth-1.0.0/CMRESHandler_NtlmAuth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:34:34.000000 CMRESHandler-NtlmAuth-1.0.0/CMRESHandler_NtlmAuth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-22 10:34:34.000000 CMRESHandler-NtlmAuth-1.0.0/CMRESHandler_NtlmAuth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-22 10:34:34.000000 CMRESHandler-NtlmAuth-1.0.0/CMRESHandler_NtlmAuth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      574 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0    10733 2023-05-22 10:34:34.938430 CMRESHandler-NtlmAuth-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9421 2023-05-22 10:33:41.000000 CMRESHandler-NtlmAuth-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 10:34:34.920319 CMRESHandler-NtlmAuth-1.0.0/cmreslogging/
--rw-rw-rw-   0        0        0        0 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.0/cmreslogging/__init__.py
--rw-rw-rw-   0        0        0    15806 2023-05-22 10:33:41.000000 CMRESHandler-NtlmAuth-1.0.0/cmreslogging/handlers.py
--rw-rw-rw-   0        0        0      730 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.0/cmreslogging/serializers.py
--rw-rw-rw-   0        0        0       59 2023-05-22 10:34:34.938430 CMRESHandler-NtlmAuth-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4322 2023-05-22 10:33:41.000000 CMRESHandler-NtlmAuth-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:34:34.938430 CMRESHandler-NtlmAuth-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     9058 2023-05-22 10:33:41.000000 CMRESHandler-NtlmAuth-1.0.0/tests/test_cmreshandler.py
--rw-rw-rw-   0        0        0     3621 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.0/tests/test_cmresserializer.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.032390 CMRESHandler-NtlmAuth-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.018531 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/
+-rw-rw-rw-   0        0        0    10733 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      574 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0    10733 2023-06-02 10:34:10.033381 CMRESHandler-NtlmAuth-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9421 2023-06-02 10:27:33.000000 CMRESHandler-NtlmAuth-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.023522 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/
+-rw-rw-rw-   0        0        0        0 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/__init__.py
+-rw-rw-rw-   0        0        0    16250 2023-06-02 10:31:30.000000 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/handlers.py
+-rw-rw-rw-   0        0        0      730 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/serializers.py
+-rw-rw-rw-   0        0        0       59 2023-06-02 10:34:10.034770 CMRESHandler-NtlmAuth-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4322 2023-06-02 10:31:30.000000 CMRESHandler-NtlmAuth-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.030381 CMRESHandler-NtlmAuth-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-06-02 10:31:30.000000 CMRESHandler-NtlmAuth-1.0.1/tests/test_cmreshandler.py
+-rw-rw-rw-   0        0        0     3621 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/tests/test_cmresserializer.py
```

### Comparing `CMRESHandler-NtlmAuth-1.0.0/CMRESHandler_NtlmAuth.egg-info/PKG-INFO` & `CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMRESHandler-NtlmAuth
-Version: 1.0.0
+Version: 1.0.1
 Summary: Elasticsearch Log handler for the logging library
 Home-page: https://github.com/thoscilo/python-elasticsearch-logger/tree/release
 Author: Carlos Manzanedo Rueda
 Author-email: c.manaha@gmail.com
 License: Apache2
 Keywords: logging elasticsearch handler log django instrumentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `CMRESHandler-NtlmAuth-1.0.0/LICENSE.md` & `CMRESHandler-NtlmAuth-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CMRESHandler-NtlmAuth-1.0.0/PKG-INFO` & `CMRESHandler-NtlmAuth-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMRESHandler-NtlmAuth
-Version: 1.0.0
+Version: 1.0.1
 Summary: Elasticsearch Log handler for the logging library
 Home-page: https://github.com/thoscilo/python-elasticsearch-logger/tree/release
 Author: Carlos Manzanedo Rueda
 Author-email: c.manaha@gmail.com
 License: Apache2
 Keywords: logging elasticsearch handler log django instrumentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `CMRESHandler-NtlmAuth-1.0.0/README.md` & `CMRESHandler-NtlmAuth-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `CMRESHandler-NtlmAuth-1.0.0/cmreslogging/handlers.py` & `CMRESHandler-NtlmAuth-1.0.1/cmreslogging/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,19 +54,21 @@
     class IndexNameFrequency(Enum):
         """ Index type supported
         the handler supports
         - Daily indices
         - Weekly indices
         - Monthly indices
         - Year indices
+        - Append to one index
         """
         DAILY = 0
         WEEKLY = 1
         MONTHLY = 2
         YEARLY = 3
+        NONE = 4
 
     # Defaults for the class
     __DEFAULT_ELASTICSEARCH_HOST = [{'host': 'localhost', 'port': 9200, 'scheme': 'http'}]
     __DEFAULT_AUTH_USER = ''
     __DEFAULT_AUTH_PASSWD = ''
     __DEFAULT_AWS_ACCESS_KEY = ''
     __DEFAULT_AWS_SECRET_KEY = ''
@@ -117,19 +119,28 @@
     def _get_yearly_index_name(es_index_name):
         """ Return elasticsearch index name
         :param: index_name the prefix to be used in the index
         :return: A srting containing the elasticsearch indexname used which should include the date and specific year
         """
         return "{0!s}-{1!s}".format(es_index_name, datetime.datetime.now().strftime('%Y'))
 
+    @staticmethod
+    def _get_base_index_name(es_index_name):
+        """ Return elasticsearch index name
+        :param: index_name the prefix to be used in the index
+        :return: A srting containing the elasticsearch indexname used which should not include the date in any format
+        """
+        return es_index_name
+
     _INDEX_FREQUENCY_FUNCION_DICT = {
         IndexNameFrequency.DAILY: _get_daily_index_name,
         IndexNameFrequency.WEEKLY: _get_weekly_index_name,
         IndexNameFrequency.MONTHLY: _get_monthly_index_name,
-        IndexNameFrequency.YEARLY: _get_yearly_index_name
+        IndexNameFrequency.YEARLY: _get_yearly_index_name,
+        IndexNameFrequency.NONE:  _get_base_index_name,
     }
 
     def __init__(self,
                  hosts=__DEFAULT_ELASTICSEARCH_HOST,
                  auth_details=(__DEFAULT_AUTH_USER, __DEFAULT_AUTH_PASSWD),
                  aws_access_key=__DEFAULT_AWS_ACCESS_KEY,
                  aws_secret_key=__DEFAULT_AWS_SECRET_KEY,
```

### Comparing `CMRESHandler-NtlmAuth-1.0.0/cmreslogging/serializers.py` & `CMRESHandler-NtlmAuth-1.0.1/cmreslogging/serializers.py`

 * *Files identical despite different names*

### Comparing `CMRESHandler-NtlmAuth-1.0.0/setup.py` & `CMRESHandler-NtlmAuth-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 setup(
     name='CMRESHandler-NtlmAuth',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.0',
+    version='1.0.1',
 
     description='Elasticsearch Log handler for the logging library',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
 
     # The project's main homepage.
```

### Comparing `CMRESHandler-NtlmAuth-1.0.0/tests/test_cmreshandler.py` & `CMRESHandler-NtlmAuth-1.0.1/tests/test_cmreshandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,10 +180,22 @@
                                index_name_frequency=CMRESHandler.IndexNameFrequency.YEARLY,
                                raise_on_indexing_exceptions=True)
         self.assertEqual(
             handler._index_name_func.__func__(index_name),
             CMRESHandler._get_yearly_index_name(index_name)
         )
 
+        handler = CMRESHandler(hosts=[{'host': self.getESHost(),
+                                       'port': self.getESPort(),
+                                       'scheme': self.get_ES_scheme()}],
+                               auth_type=CMRESHandler.AuthType.NO_AUTH,
+                               es_index_name=index_name,
+                               index_name_frequency=CMRESHandler.IndexNameFrequency.NONE,
+                               raise_on_indexing_exceptions=True)
+        self.assertEqual(
+            handler._index_name_func.__func__(index_name),
+            CMRESHandler._get_base_index_name(index_name)
+        )
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `CMRESHandler-NtlmAuth-1.0.0/tests/test_cmresserializer.py` & `CMRESHandler-NtlmAuth-1.0.1/tests/test_cmresserializer.py`

 * *Files identical despite different names*

