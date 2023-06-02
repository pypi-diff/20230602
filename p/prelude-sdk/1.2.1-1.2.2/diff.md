# Comparing `tmp/prelude-sdk-1.2.1.tar.gz` & `tmp/prelude-sdk-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.2.1.tar", last modified: Tue May 23 21:45:27 2023, max compression
+gzip compressed data, was "prelude-sdk-1.2.2.tar", last modified: Fri Jun  2 17:12:33 2023, max compression
```

## Comparing `prelude-sdk-1.2.1.tar` & `prelude-sdk-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:45:27.291886 prelude-sdk-1.2.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-23 21:45:27.291936 prelude-sdk-1.2.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:45:27.287377 prelude-sdk-1.2.1/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.1/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:45:27.289543 prelude-sdk-1.2.1/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.1/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1479 2023-05-18 20:31:39.000000 prelude-sdk-1.2.1/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4923 2023-05-22 15:57:51.000000 prelude-sdk-1.2.1/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3266 2023-05-12 13:56:19.000000 prelude-sdk-1.2.1/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.2.1/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.1/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:45:27.290180 prelude-sdk-1.2.1/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.1/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.1/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2555 2023-05-22 15:57:51.000000 prelude-sdk-1.2.1/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:45:27.287908 prelude-sdk-1.2.1/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-23 21:45:27.000000 prelude-sdk-1.2.1/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      806 2023-05-23 21:45:27.000000 prelude-sdk-1.2.1/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-23 21:45:27.000000 prelude-sdk-1.2.1/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-05-23 21:45:27.000000 prelude-sdk-1.2.1/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-05-23 21:45:27.000000 prelude-sdk-1.2.1/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-05-23 21:45:27.292140 prelude-sdk-1.2.1/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:45:27.291622 prelude-sdk-1.2.1/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.1/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.1/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:45:27.291809 prelude-sdk-1.2.1/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.1/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1761 2023-05-23 21:42:11.000000 prelude-sdk-1.2.1/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4623 2023-05-23 21:42:11.000000 prelude-sdk-1.2.1/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3223 2023-05-23 21:42:11.000000 prelude-sdk-1.2.1/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      707 2023-05-23 21:42:11.000000 prelude-sdk-1.2.1/tests/test_partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.1/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.154370 prelude-sdk-1.2.2/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-02 17:12:33.154420 prelude-sdk-1.2.2/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.2/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.150192 prelude-sdk-1.2.2/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.151974 prelude-sdk-1.2.2/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1587 2023-06-02 13:58:42.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4923 2023-05-22 15:57:51.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3266 2023-05-12 13:56:19.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.152640 prelude-sdk-1.2.2/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2555 2023-05-22 15:57:51.000000 prelude-sdk-1.2.2/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.150769 prelude-sdk-1.2.2/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-02 17:12:33.154626 prelude-sdk-1.2.2/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.154086 prelude-sdk-1.2.2/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.2/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.154287 prelude-sdk-1.2.2/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1662 2023-06-01 16:01:25.000000 prelude-sdk-1.2.2/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4623 2023-05-23 21:42:11.000000 prelude-sdk-1.2.2/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3223 2023-05-23 21:42:11.000000 prelude-sdk-1.2.2/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.2.1/LICENSE` & `prelude-sdk-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/PKG-INFO` & `prelude-sdk-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.1/README.md` & `prelude-sdk-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.2.2/prelude_sdk/controllers/build_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
     def create_test(self, test_id, name, unit, advisory=None):
         """ Create or update a test """
         body = dict(name=name, unit=unit)
+
         if advisory:
             body['advisory'] = advisory
 
         res = requests.post(
             f'{self.account.hq}/build/tests/{test_id}',
             json=body,
             headers=self.account.headers,
@@ -34,14 +35,17 @@
         )
         if not res.status_code == 200:
             raise Exception(res.text)
 
     @verify_credentials
     def upload(self, test_id, filename, data, binary=False):
         """ Upload a test or attachment """
+        if len(data) > 1000000:
+            raise ValueError(f'File size must be under 1MB ({filename})')
+
         h = self.account.headers | ({'Content-Type': 'application/octet-stream'} if binary else {})
         res = requests.post(
             f'{self.account.hq}/build/tests/{test_id}/{filename}',
             data=data,
             headers=h,
             timeout=10
         )
```

### Comparing `prelude-sdk-1.2.1/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.2.2/prelude_sdk/controllers/detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.2.2/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.2.2/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/prelude_sdk/models/account.py` & `prelude-sdk-1.2.2/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/prelude_sdk/models/codes.py` & `prelude-sdk-1.2.2/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.2.2/prelude_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.1/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.2.2/prelude_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,10 +18,9 @@
 prelude_sdk/models/account.py
 prelude_sdk/models/codes.py
 tests/__init__.py
 tests/conftest.py
 tests/test_build_controller.py
 tests/test_detect_controller.py
 tests/test_iam_controller.py
-tests/test_partner_controller.py
 tests/test_probe_controller.py
 tests/templates/__init__.py
```

### Comparing `prelude-sdk-1.2.1/setup.cfg` & `prelude-sdk-1.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.2.1
+version = 1.2.2
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.2.1/tests/conftest.py` & `prelude-sdk-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/tests/test_build_controller.py` & `prelude-sdk-1.2.2/tests/test_build_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from importlib.resources import files
 
 from tests import templates as templates
 from prelude_sdk.controllers.build_controller import BuildController
 from prelude_sdk.controllers.detect_controller import DetectController
 
 
-@pytest.mark.order(after='test_partner_controller.py::TestPartnerController::test_detach_partner')
 class TestBuildController:
 
     def setup_class(self):
         """Setup the test class"""
         self.test_id = str(uuid.uuid4())
         self.test_name = 'test'
         self.build = BuildController(pytest.account)
```

### Comparing `prelude-sdk-1.2.1/tests/test_detect_controller.py` & `prelude-sdk-1.2.2/tests/test_detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/tests/test_iam_controller.py` & `prelude-sdk-1.2.2/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.1/tests/test_probe_controller.py` & `prelude-sdk-1.2.2/tests/test_probe_controller.py`

 * *Files identical despite different names*

