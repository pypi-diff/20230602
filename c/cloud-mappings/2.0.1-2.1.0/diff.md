# Comparing `tmp/cloud-mappings-2.0.1.tar.gz` & `tmp/cloud-mappings-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cloud-mappings/cloud-mappings/dist/.tmp-p6odatm3/cloud-mappings-2.0.1.tar", last modified: Wed May 17 14:44:47 2023, max compression
+gzip compressed data, was "/home/runner/work/cloud-mappings/cloud-mappings/dist/.tmp-sx9t_8m1/cloud-mappings-2.1.0.tar", last modified: Fri Jun  2 01:14:49 2023, max compression
```

## Comparing `cloud-mappings-2.0.1.tar` & `cloud-mappings-2.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloud_mappings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloudmappings/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_cloudmappinginternal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/awss3storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azureblobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azuretablestorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/cloudmapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/cloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:47.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/serialisers/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-17 14:44:16.000000 cloud-mappings-2.0.1/src/cloudmappings/storageprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloud_mappings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloud_mappings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloud_mappings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloud_mappings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloud_mappings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloud_mappings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloudmappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/_cloudmappinginternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/awss3storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/azureblobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/azuretablestorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/cloudmapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/cloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:49.000000 cloud-mappings-2.1.0/src/cloudmappings/serialisers/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/serialisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/serialisers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/serialisers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/serialisers/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-06-02 01:14:16.000000 cloud-mappings-2.1.0/src/cloudmappings/storageprovider.py
```

### Comparing `cloud-mappings-2.0.1/LICENSE` & `cloud-mappings-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/PKG-INFO` & `cloud-mappings-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-mappings
-Version: 2.0.1
+Version: 2.1.0
 Summary: MutableMapping interfaces for common cloud storage providers
 Home-page: https://github.com/JJ11teen/cloud-mappings
 Author: Lucas Sargent
 Author-email: lucas.sargent@outlook.com
 Project-URL: Bug Tracker, https://github.com/JJ11teen/cloud-mappings/issues
 Keywords: mutable dict aws s3 azure gcp
 Classifier: Programming Language :: Python :: 3
@@ -153,14 +153,16 @@
 ### Mutable Properties:
 See the parameters of `CloudStorage.create_mapping()` above for their descriptions.
 * `read_blindly: bool`
 * `read_blindly_error: bool`
 * `read_blindly_default: Any`
 
 ### Immutable Properties:
+* `storage_provider: StorageProvider`
+  * An object that provides a consistent interface to the underlying storage provider (eg methods to read and write bytes to specific paths).
 * `etags: dict[str, str]`
   * An internal dictionary of etags used to ensure the `CloudMapping` is in sync with the cloud storage resource. The dict maps keys to their last synchronised etags.
   * This dictionary is used as the `CloudMapping's expected view of the cloud. It is used to determine if a key exists, and ensure that the value of each key is expected.
   * See: https://en.wikipedia.org/wiki/HTTP_ETag
 * `serialisation: CloudMappingSerialisation[T]`
   * Gets the serialiser configured to use for serialising and deserialising values.
 * `key_prefix: Optional[str]`
```

### Comparing `cloud-mappings-2.0.1/README.md` & `cloud-mappings-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -132,14 +132,16 @@
 ### Mutable Properties:
 See the parameters of `CloudStorage.create_mapping()` above for their descriptions.
 * `read_blindly: bool`
 * `read_blindly_error: bool`
 * `read_blindly_default: Any`
 
 ### Immutable Properties:
+* `storage_provider: StorageProvider`
+  * An object that provides a consistent interface to the underlying storage provider (eg methods to read and write bytes to specific paths).
 * `etags: dict[str, str]`
   * An internal dictionary of etags used to ensure the `CloudMapping` is in sync with the cloud storage resource. The dict maps keys to their last synchronised etags.
   * This dictionary is used as the `CloudMapping's expected view of the cloud. It is used to determine if a key exists, and ensure that the value of each key is expected.
   * See: https://en.wikipedia.org/wiki/HTTP_ETag
 * `serialisation: CloudMappingSerialisation[T]`
   * Gets the serialiser configured to use for serialising and deserialising values.
 * `key_prefix: Optional[str]`
```

### Comparing `cloud-mappings-2.0.1/setup.cfg` & `cloud-mappings-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloud_mappings.egg-info/PKG-INFO` & `cloud-mappings-2.1.0/src/cloud_mappings.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-mappings
-Version: 2.0.1
+Version: 2.1.0
 Summary: MutableMapping interfaces for common cloud storage providers
 Home-page: https://github.com/JJ11teen/cloud-mappings
 Author: Lucas Sargent
 Author-email: lucas.sargent@outlook.com
 Project-URL: Bug Tracker, https://github.com/JJ11teen/cloud-mappings/issues
 Keywords: mutable dict aws s3 azure gcp
 Classifier: Programming Language :: Python :: 3
@@ -153,14 +153,16 @@
 ### Mutable Properties:
 See the parameters of `CloudStorage.create_mapping()` above for their descriptions.
 * `read_blindly: bool`
 * `read_blindly_error: bool`
 * `read_blindly_default: Any`
 
 ### Immutable Properties:
+* `storage_provider: StorageProvider`
+  * An object that provides a consistent interface to the underlying storage provider (eg methods to read and write bytes to specific paths).
 * `etags: dict[str, str]`
   * An internal dictionary of etags used to ensure the `CloudMapping` is in sync with the cloud storage resource. The dict maps keys to their last synchronised etags.
   * This dictionary is used as the `CloudMapping's expected view of the cloud. It is used to determine if a key exists, and ensure that the value of each key is expected.
   * See: https://en.wikipedia.org/wiki/HTTP_ETag
 * `serialisation: CloudMappingSerialisation[T]`
   * Gets the serialiser configured to use for serialising and deserialising values.
 * `key_prefix: Optional[str]`
```

### Comparing `cloud-mappings-2.0.1/src/cloud_mappings.egg-info/SOURCES.txt` & `cloud-mappings-2.1.0/src/cloud_mappings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/_cloudmappinginternal.py` & `cloud-mappings-2.1.0/src/cloudmappings/_cloudmappinginternal.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     def sync_with_cloud(self, key_prefix: str = "") -> None:
         key_prefix = self._encode_key(key_prefix)
         self._etags.update(
             {self._decode_key(k): i for k, i in self._storage_provider.list_keys_and_etags(key_prefix).items()}
         )
 
     @property
+    def storage_provider(self) -> StorageProvider:
+        return self._storage_provider
+
+    @property
     def etags(self) -> Dict[str, str]:
         return self._etags
 
     @property
     def serialisation(self) -> CloudMappingSerialisation[T]:
         return self._serialisation
```

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/awss3storage.py` & `cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/awss3storage.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azureblobstorage.py` & `cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/azureblobstorage.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/azuretablestorage.py` & `cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/azuretablestorage.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/_storageproviders/googlecloudstorage.py` & `cloud-mappings-2.1.0/src/cloudmappings/_storageproviders/googlecloudstorage.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/cloudmapping.py` & `cloud-mappings-2.1.0/src/cloudmappings/cloudmapping.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, MutableMapping, Optional, TypeVar
 
 from cloudmappings.serialisers import CloudMappingSerialisation
+from cloudmappings.storageprovider import StorageProvider
 
 T = TypeVar("T")
 
 
 class CloudMapping(MutableMapping[str, T], ABC):
     """A cloud-mapping, a `MutableMapping` implementation backed by common cloud storage solutions.
     Implements the `MutableMapping` interface, can be used just as a standard `dict()`.
@@ -60,14 +61,22 @@
             Only sync keys beginning with the specified prefix, the key_prefix configured on the
             mapping is prepended in combination with this parameter.
         """
         pass
 
     @property
     @abstractmethod
+    def storage_provider(self) -> StorageProvider:
+        """The underlying StorageProvider for this CloudMapping. This can be used to create another
+        CloudMapping instance (for example for a different view of the data), or just to directly
+        interact with the Cloud resource.
+        """
+
+    @property
+    @abstractmethod
     def etags(self) -> Dict[str, str]:
         """An internal dictionary of etags used to ensure the `CloudMapping` is in sync with
         the cloud storage resource. The dict maps keys to their last synchronised etags.
 
         This dictionary is used as the `CloudMapping's expected view of the cloud. It is used
         to determine if a key exists, and ensure that the value of each key is expected.
```

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/cloudstorage.py` & `cloud-mappings-2.1.0/src/cloudmappings/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/errors.py` & `cloud-mappings-2.1.0/src/cloudmappings/errors.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/serialisers/core.py` & `cloud-mappings-2.1.0/src/cloudmappings/serialisers/core.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/serialisers/pandas.py` & `cloud-mappings-2.1.0/src/cloudmappings/serialisers/pandas.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/serialisers/serialisation.py` & `cloud-mappings-2.1.0/src/cloudmappings/serialisers/serialisation.py`

 * *Files identical despite different names*

### Comparing `cloud-mappings-2.0.1/src/cloudmappings/storageprovider.py` & `cloud-mappings-2.1.0/src/cloudmappings/storageprovider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Dict
 from urllib.parse import quote, unquote
 
 
 class StorageProvider(ABC):
+    """Provides a consistent interface for interacting with Cloud Storage Providers."""
+
     @abstractmethod
     def logical_name(self) -> str:
         """Returns a human readable string identifying the current implementation, and which
         logical cloud resouce it is currently mapping to. Does not include any credential or
         secret information.
 
         Returns
@@ -75,15 +77,15 @@
         Otherwise the etag will be used to ensure the data downloaded has a matching etag. If
         the etag does not match the latest cloud version, a `cloudmappings.errors.KeySyncError`
         will be raised.
 
         Parameters
         ----------
         key : str
-            The key specifying which data to download
+            The encoded key specifying which data to download
         etag : str or None
             Etag of the expected latest value in the cloud, or `None`
 
         Raises
         ------
         KeySyncError
             If an etag is specified and does not match the latest version in the cloud.
@@ -100,15 +102,15 @@
         """Upload data to cloud storage
 
         Uploads data at the specified key to cloud storage, only overwriting if the etag matches
 
         Parameters
         ----------
         key : str
-            The key specifying which data to download
+            The encoded key specifying which data to download
         etag : str or None
             Etag of the expected value in the cloud, `None` if it is expected that there is no
             existing data in the cloud
         data : bytes
             The data to upload to the cloud, in bytes
 
         Raises
@@ -132,15 +134,15 @@
         """Delete data from cloud storage.
 
         Deletes data at the specified key from cloud storage, only if the etag matches
 
         Parameters
         ----------
         key : str
-            The key specifying which data to delete
+            The encoded key specifying which data to delete
         etag : str or None
             Etag of the expected value in the cloud
 
         Raises
         ------
         KeySyncError
             When the etag specified does not match the value in the cloud
@@ -154,15 +156,16 @@
         Queries all keys and their associated etags from the cloud. Returns a dictionary mapping
         each key to its latest etag. If a `key_prefix` is specified only the keys beginning with
         this prefix will be queried and returned.
 
         Parameters
         ----------
         key_prefix : str, optional
-            A prefix specifying a subset of keys to query. If not given, all keys will be queried
+            An encoded prefix specifying a subset of keys to query. If not given, all keys will
+            be queried
 
         Returns
         -------
         Dict[str, str]
             A dictionary mapping each key in the cloud to it's latest etag
         """
         pass
```

