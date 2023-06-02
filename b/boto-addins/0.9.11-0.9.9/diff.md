# Comparing `tmp/boto_addins-0.9.11.tar.gz` & `tmp/boto_addins-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto_addins-0.9.11.tar", last modified: Fri Jun  2 14:48:48 2023, max compression
+gzip compressed data, was "dist/boto_addins-0.9.9.tar", last modified: Wed Nov  6 23:22:01 2019, max compression
```

## Comparing `boto_addins-0.9.11.tar` & `boto_addins-0.9.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 master     (501) staff       (20)        0 2023-06-02 14:48:48.874086 boto_addins-0.9.11/
--rw-r--r--   0 master     (501) staff       (20)     1067 2023-05-11 12:29:12.000000 boto_addins-0.9.11/LICENSE
--rw-r--r--   0 master     (501) staff       (20)      348 2023-06-02 14:48:48.873935 boto_addins-0.9.11/PKG-INFO
-drwxr-xr-x   0 master     (501) staff       (20)        0 2023-06-02 14:48:48.873101 boto_addins-0.9.11/boto_addins/
--rw-r--r--   0 master     (501) staff       (20)        0 2019-04-19 10:55:44.000000 boto_addins-0.9.11/boto_addins/__init__.py
--rw-r--r--   0 master     (501) staff       (20)     4038 2023-05-11 12:29:12.000000 boto_addins-0.9.11/boto_addins/lambda_.py
--rw-r--r--   0 master     (501) staff       (20)     7026 2023-06-02 14:47:39.000000 boto_addins-0.9.11/boto_addins/s3.py
-drwxr-xr-x   0 master     (501) staff       (20)        0 2023-06-02 14:48:48.873755 boto_addins-0.9.11/boto_addins.egg-info/
--rw-rw-r--   0 master     (501) staff       (20)      348 2023-06-02 14:48:48.000000 boto_addins-0.9.11/boto_addins.egg-info/PKG-INFO
--rw-rw-r--   0 master     (501) staff       (20)      255 2023-06-02 14:48:48.000000 boto_addins-0.9.11/boto_addins.egg-info/SOURCES.txt
--rw-rw-r--   0 master     (501) staff       (20)        1 2023-06-02 14:48:48.000000 boto_addins-0.9.11/boto_addins.egg-info/dependency_links.txt
--rw-rw-r--   0 master     (501) staff       (20)       42 2023-06-02 14:48:48.000000 boto_addins-0.9.11/boto_addins.egg-info/requires.txt
--rw-rw-r--   0 master     (501) staff       (20)       12 2023-06-02 14:48:48.000000 boto_addins-0.9.11/boto_addins.egg-info/top_level.txt
--rw-r--r--   0 master     (501) staff       (20)       38 2023-06-02 14:48:48.874155 boto_addins-0.9.11/setup.cfg
--rwxr-xr-x   0 master     (501) staff       (20)      523 2023-06-02 14:47:39.000000 boto_addins-0.9.11/setup.py
+drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-11-06 23:22:01.000000 boto_addins-0.9.9/
+-rw-r--r--   0 Master     (501) staff       (20)      336 2019-11-06 23:22:01.000000 boto_addins-0.9.9/PKG-INFO
+drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/
+-rw-r--r--   0 Master     (501) staff       (20)      336 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/PKG-INFO
+-rw-r--r--   0 Master     (501) staff       (20)      247 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/SOURCES.txt
+-rw-r--r--   0 Master     (501) staff       (20)       49 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/requires.txt
+-rw-r--r--   0 Master     (501) staff       (20)       12 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/top_level.txt
+-rw-r--r--   0 Master     (501) staff       (20)        1 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins.egg-info/dependency_links.txt
+drwxr-xr-x   0 Master     (501) staff       (20)        0 2019-11-06 23:22:01.000000 boto_addins-0.9.9/boto_addins/
+-rw-r--r--   0 Master     (501) staff       (20)     4079 2019-11-06 21:39:24.000000 boto_addins-0.9.9/boto_addins/lambda_.py
+-rw-r--r--   0 Master     (501) staff       (20)        0 2019-04-19 10:55:44.000000 boto_addins-0.9.9/boto_addins/__init__.py
+-rw-r--r--   0 Master     (501) staff       (20)     9145 2019-11-06 22:48:14.000000 boto_addins-0.9.9/boto_addins/s3.py
+-rwxr-xr-x   0 Master     (501) staff       (20)      529 2019-11-06 23:20:58.000000 boto_addins-0.9.9/setup.py
+-rw-r--r--   0 Master     (501) staff       (20)       59 2019-11-06 23:22:01.000000 boto_addins-0.9.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `boto_addins-0.9.11/boto_addins/lambda_.py` & `boto_addins-0.9.9/boto_addins/lambda_.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import unicode_literals
+
 import json
 from urllib.parse import quote
 
 from botocore.auth import SigV4Auth
 from botocore.awsrequest import AWSRequest
 from tornado.curl_httpclient import CurlAsyncHTTPClient
 from tornado.httpclient import HTTPRequest
```

### Comparing `boto_addins-0.9.11/boto_addins/s3.py` & `boto_addins-0.9.9/boto_addins/s3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from __future__ import unicode_literals
+
 import os
 import weakref
 import logging
 import xml.sax
 import socket
 from uuid import uuid4
 import asyncio
 from urllib.parse import quote
 
 from boto.handler import XmlHandler
 from boto.s3.acl import Policy
 from boto.s3.connection import S3Connection, Bucket, Key
-from tornado import httpclient, simple_httpclient, curl_httpclient
+from boto.utils import merge_meta
+from tornado import gen, httpclient, simple_httpclient, curl_httpclient
 
 
 logger = logging.getLogger(__name__)
 
 
 DATA_SIZE = 1024 * 1024
 S3_TEMP_URL_TTL = 300  # seconds
@@ -26,17 +29,17 @@
             bucket_class=AsyncBucket, *args, **kwargs)
 
     def get_bucket(self, bucket_name, validate=False, headers=None):
         # Do not validate by default.
         return super(AsyncS3Connection, self).get_bucket(
             bucket_name, validate, headers)
 
-    def generate_request(self, method, bucket='', key='',
-                         query_args=None, headers=None,
-                         content_length=None, attempts=1, **kwargs):
+    def generate_async_request(self, method, bucket='', key='',
+                               query_args=None, headers=None,
+                               content_length=None, attempts=1, **kwargs):
         if isinstance(bucket, self.bucket_class):
             bucket = bucket.name
         if isinstance(key, Key):
             key = key.name
         path = self.calling_format.build_path_base(bucket, key)
         auth_path = self.calling_format.build_auth_path(bucket, key)
         host = self.calling_format.build_host(self.server_name(), bucket)
@@ -49,47 +52,100 @@
         req.authorize(self)
 
         if content_length is None:
             del req.headers['Content-Length']
         else:
             req.headers['Content-Length'] = str(content_length)
 
-        request = httpclient.HTTPRequest(
+        async_request = httpclient.HTTPRequest(
             "{0.protocol}://{0.host}{0.path}".format(req),
             req.method, req.headers, **kwargs
         )
-        return fetch_request(request, attempts=attempts)
+        return fetch_request(async_request, attempts=attempts)
+
+    async def set_contents_from_file(self, bucket, key_name, fp, headers=None,
+                                     policy=None, encrypt_key=False,
+                                     metadata=None, attempts=3,
+                                     request_timeout=10 * 60):
+        headers = headers or {}
+        if policy:
+            headers[self.provider.acl_header] = policy
+        if encrypt_key:
+            headers[self.provider.server_side_encryption_header] = 'AES256'
+        if metadata is not None:
+            headers = merge_meta(headers, metadata, self.provider)
+
+        return await self.generate_async_request(
+            'PUT', bucket, key_name, headers=headers, body=fp.read(),
+            request_timeout=request_timeout, attempts=attempts,
+        )
+
+    async def copy_key(self, src_key, dst_key, temp_dir, metadata=None,
+                       policy=None, encrypt_key=False, headers=None,
+                       request_timeout=10 * 60):
+        headers = headers or {}
+        if policy:
+            headers[self.provider.acl_header] = policy
+        if encrypt_key:
+            headers[self.provider.server_side_encryption_header] = 'AES256'
+        if metadata is not None:
+            headers = merge_meta(headers, metadata, self.provider)
+
+        url = src_key.generate_url(S3_TEMP_URL_TTL)
+        destination = os.path.join(temp_dir, '_' + str(uuid4()))
+        await http_download(url, destination,
+                            request_timeout=request_timeout)
+
+        async def producer(write):
+            with open(destination, 'r') as f:
+                while True:
+                    data = f.read(DATA_SIZE)
+                    if not data:
+                        break
+                    await write(data)
+
+        try:
+            await self.generate_async_request(
+                'PUT', dst_key.bucket.name, dst_key.name,
+                headers=headers, body_producer=producer,
+                content_length=src_key.size,
+                # Timeout for whole request, not tcp.
+                request_timeout=request_timeout,
+            )
+        finally:
+            if os.path.exists(destination):
+                os.unlink(destination)
 
 
 class AsyncBucket(Bucket):
     def __init__(self, connection=None, name=None):
         self._downloading_files = weakref.WeakValueDictionary()
         super(AsyncBucket, self).__init__(connection, name, key_class=AsyncKey)
 
     async def get_key_contents(self, key_name, attempts=3, **kwargs):
-        return await self.connection.generate_request(
+        return await self.connection.generate_async_request(
             'GET', self.name, key_name, attempts=attempts, **kwargs
         )
 
     async def get_key(self, key_name, headers=None, version_id=None,
                       response_headers=None, attempts=3):
         query_args_l = []
         if version_id:
             query_args_l.append('versionId=%s' % version_id)
         if response_headers:
             for rk, rv in response_headers.items():
                 query_args_l.append('%s=%s' % (rk, quote(rv)))
 
         query_args = '&'.join(query_args_l) or None
         try:
-            response = await self.connection.generate_request(
+            response = await self.connection.generate_async_request(
                 'HEAD', self.name, key_name,
                 headers=headers, query_args=query_args, attempts=attempts,
             )
-        except httpclient.HTTPClientError as e:
+        except httpclient.HTTPError as e:
             if e.code == 404:
                 return False
             raise
         key = self.key_class(self)
         key.name = key_name
         clen = response.headers['content-length']
         key.size = int(clen) if clen else 0
@@ -97,15 +153,15 @@
 
     async def get_acl(self, key_name='', headers=None, version_id=None,
                       attempts=3):
         query_args = 'acl'
         if version_id:
             query_args += '&versionId=%s' % version_id
 
-        resp = await self.connection.generate_request(
+        resp = await self.connection.generate_async_request(
             'GET', self.name, key_name, query_args=query_args, headers=headers,
             attempts=attempts,
         )
 
         policy = Policy(self)
         h = XmlHandler(policy, self)
         xml.sax.parseString(resp.body, h)
@@ -147,38 +203,36 @@
     # Save exceptions history for further analysis
     except_history = []
 
     while attempts:
         wait_before_retry = 0
         try:
             resp = await client.fetch(request)
-        except httpclient.HTTPClientError as e:
+        except httpclient.HTTPError as e:
             # retry on s3 errors
             if e.code == 500:
                 wait_before_retry = 0.2
             elif e.code in (503, 599):
                 wait_before_retry = 1
             else:
-                if resp := e.response:
-                    # Put values to local variables for better logging in tb
-                    headers, body = resp.headers, resp.body  # noqa: F841
                 raise
             except_history.append(e)
         except socket.error as e:
             # retry
             except_history.append(e)
 
         else:
             return resp
 
-        if not (attempts := attempts - 1):
+        attempts -= 1
+        if not attempts:
             raise except_history[-1]
 
         if wait_before_retry:
-            await asyncio.sleep(wait_before_retry)
+            await gen.sleep(wait_before_retry)
         if retry_callback:
             await retry_callback(request, attempts)
 
 
 async def http_download(source, destination,
                         request_timeout=10 * 60, attempts=3):
     tmp_name = '{}.{}'.format(destination, str(uuid4())[:8])
```

### Comparing `boto_addins-0.9.11/setup.py` & `boto_addins-0.9.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name="boto_addins",
-    version="0.9.11",
+    version="0.9.9",
     author="Uploadcare",
     author_email="ak@uploadcare.com",
     description="Async proxy libraries for AWS services.",
     install_requires=[
         'tornado>=6.0.0',
-        'botocore>=1.13.0',
+        'tornado-botocore>=1.5.0',
         'boto',
         'YURL',
     ],
     keywords="aws amazon S3 storage "
              "lambda request-response invoke",
     url="http://packages.python.org/an_example_pypi_project",
     packages=['boto_addins'],
```

