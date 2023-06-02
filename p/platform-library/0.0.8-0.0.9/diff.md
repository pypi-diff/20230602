# Comparing `tmp/platform-library-0.0.8.tar.gz` & `tmp/platform-library-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-library-0.0.8.tar", last modified: Wed May 17 10:19:24 2023, max compression
+gzip compressed data, was "platform-library-0.0.9.tar", last modified: Fri Jun  2 08:15:08 2023, max compression
```

## Comparing `platform-library-0.0.8.tar` & `platform-library-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.637162 platform-library-0.0.8/
--rw-r--r--   0 Artyom     (501) staff       (20)     1078 2023-05-17 10:19:03.000000 platform-library-0.0.8/LICENSE
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-17 10:19:24.637008 platform-library-0.0.8/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.0.8/README-public.md
--rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.0.8/README.md
--rw-r--r--   0 Artyom     (501) staff       (20)      593 2023-05-17 10:18:00.000000 platform-library-0.0.8/pyproject.toml
--rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-05-17 10:19:24.637231 platform-library-0.0.8/setup.cfg
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.633459 platform-library-0.0.8/src/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.635109 platform-library-0.0.8/src/platform_library.egg-info/
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)      509 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/SOURCES.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/dependency_links.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       51 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/requires.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/top_level.txt
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.633645 platform-library-0.0.8/src/plib/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.635895 platform-library-0.0.8/src/plib/auth/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/encrypt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/jwt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/o2auth.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.636402 platform-library-0.0.8/src/plib/licensing/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.0.8/src/plib/licensing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     4037 2023-05-11 06:38:08.000000 platform-library-0.0.8/src/plib/licensing/api.py
--rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.0.8/src/plib/licensing/exceptions.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.636817 platform-library-0.0.8/src/plib/tracing/
--rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.0.8/src/plib/tracing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.0.8/src/plib/tracing/utils.py
+drwxrwxr-x   0 stranger  (1000) stranger  (1000)        0 2023-06-02 08:15:08.910954 platform-library-0.0.9/
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)     1078 2023-06-02 05:23:58.000000 platform-library-0.0.9/LICENSE
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)     1696 2023-06-02 08:15:08.910954 platform-library-0.0.9/PKG-INFO
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)       50 2023-06-02 05:23:58.000000 platform-library-0.0.9/README-public.md
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      524 2023-06-02 05:23:58.000000 platform-library-0.0.9/README.md
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      593 2023-06-02 08:14:54.000000 platform-library-0.0.9/pyproject.toml
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)       38 2023-06-02 08:15:08.910954 platform-library-0.0.9/setup.cfg
+drwxrwxr-x   0 stranger  (1000) stranger  (1000)        0 2023-06-02 08:15:08.906954 platform-library-0.0.9/src/
+drwxrwxr-x   0 stranger  (1000) stranger  (1000)        0 2023-06-02 08:15:08.910954 platform-library-0.0.9/src/platform_library.egg-info/
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)     1696 2023-06-02 08:15:08.000000 platform-library-0.0.9/src/platform_library.egg-info/PKG-INFO
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      538 2023-06-02 08:15:08.000000 platform-library-0.0.9/src/platform_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)        1 2023-06-02 08:15:08.000000 platform-library-0.0.9/src/platform_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)       51 2023-06-02 08:15:08.000000 platform-library-0.0.9/src/platform_library.egg-info/requires.txt
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)        5 2023-06-02 08:15:08.000000 platform-library-0.0.9/src/platform_library.egg-info/top_level.txt
+drwxrwxr-x   0 stranger  (1000) stranger  (1000)        0 2023-06-02 08:15:08.906954 platform-library-0.0.9/src/plib/
+drwxrwxr-x   0 stranger  (1000) stranger  (1000)        0 2023-06-02 08:15:08.910954 platform-library-0.0.9/src/plib/auth/
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)        0 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/auth/__init__.py
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      559 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/auth/encrypt.py
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      309 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/auth/jwt.py
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      682 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/auth/o2auth.py
+drwxrwxr-x   0 stranger  (1000) stranger  (1000)        0 2023-06-02 08:15:08.910954 platform-library-0.0.9/src/plib/licensing/
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)        0 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/licensing/__init__.py
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)     4714 2023-06-02 07:11:30.000000 platform-library-0.0.9/src/plib/licensing/api.py
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      553 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/licensing/exceptions.py
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)      134 2023-06-02 08:04:28.000000 platform-library-0.0.9/src/plib/licensing/models.py
+drwxrwxr-x   0 stranger  (1000) stranger  (1000)        0 2023-06-02 08:15:08.910954 platform-library-0.0.9/src/plib/tracing/
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)     2287 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/tracing/__init__.py
+-rw-rw-r--   0 stranger  (1000) stranger  (1000)     3007 2023-06-02 05:23:58.000000 platform-library-0.0.9/src/plib/tracing/utils.py
```

### Comparing `platform-library-0.0.8/LICENSE` & `platform-library-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.8/PKG-INFO` & `platform-library-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
         Copyright (c) 2023 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.0.8/README.md` & `platform-library-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.8/pyproject.toml` & `platform-library-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "platform-library"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Artyom Vakilov", email="a.vakilov@3divi.com" },
 ]
 
 description = "A library for easy developing 3DiVi Platform"
 readme = "README-public.md"
 license = { file="LICENSE" }
```

### Comparing `platform-library-0.0.8/src/platform_library.egg-info/PKG-INFO` & `platform-library-0.0.9/src/platform_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
         Copyright (c) 2023 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.0.8/src/plib/auth/encrypt.py` & `platform-library-0.0.9/src/plib/auth/encrypt.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.8/src/plib/auth/o2auth.py` & `platform-library-0.0.9/src/plib/auth/o2auth.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.8/src/plib/licensing/api.py` & `platform-library-0.0.9/src/plib/licensing/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Optional
 
 import requests
 
 from plib.auth.encrypt import Encryptor
 from plib.auth.jwt import encode_payload
+from plib.licensing.models import License as LicenseModel
 
-from .exceptions import LicenseLimitAttribute, LicenseServiceError, LicenseSignatureCorrupted
+from .exceptions import (LicenseLimitAttribute, LicenseServiceError,
+                         LicenseSignatureCorrupted)
 
 
 class License:
     def __init__(self,
                  url: str,
                  issuer: str,
                  jwt_key: str,
@@ -115,7 +117,33 @@
         res = self._post(data)
         res = res['makeTransaction']
 
         self._validate_signature(res['signature'])
 
         if res['__typename'] == 'TransactionLimitError':
             raise LicenseLimitAttribute(resource, res['limit'])
+
+    def license(self) -> LicenseModel:
+        query = '''
+            query license($signature: String!) {
+                license {
+                    status
+                    signature(key: $signature)
+                }
+            }
+        '''
+
+        data = {
+            'query': query,
+            'variables': {
+                'signature': self.__encryptor.signature
+            }
+        }
+
+        res = self._post(data)
+        res = res['license']
+
+        self._validate_signature(res['signature'])
+
+        return LicenseModel(
+            status=res['status']
+        )
```

### Comparing `platform-library-0.0.8/src/plib/licensing/exceptions.py` & `platform-library-0.0.9/src/plib/licensing/exceptions.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.8/src/plib/tracing/__init__.py` & `platform-library-0.0.9/src/plib/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.8/src/plib/tracing/utils.py` & `platform-library-0.0.9/src/plib/tracing/utils.py`

 * *Files identical despite different names*

