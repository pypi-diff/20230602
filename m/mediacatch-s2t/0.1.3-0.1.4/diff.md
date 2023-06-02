# Comparing `tmp/mediacatch-s2t-0.1.3.tar.gz` & `tmp/mediacatch-s2t-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mediacatch-s2t/mediacatch-s2t/dist/.tmp-ue5_1kdb/mediacatch-s2t-0.1.3.tar", last modified: Fri Jun  2 09:03:17 2023, max compression
+gzip compressed data, was "/home/runner/work/mediacatch-s2t/mediacatch-s2t/dist/.tmp-zyrv6pil/mediacatch-s2t-0.1.4.tar", last modified: Fri Jun  2 09:10:48 2023, max compression
```

## Comparing `mediacatch-s2t-0.1.3.tar` & `mediacatch-s2t-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:17.000000 mediacatch-s2t-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/tests/test_multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 09:02:54.000000 mediacatch-s2t-0.1.3/tests/test_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:10:48.000000 mediacatch-s2t-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/tests/test_multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 09:10:29.000000 mediacatch-s2t-0.1.4/tests/test_uploader.py
```

### Comparing `mediacatch-s2t-0.1.3/LICENSE` & `mediacatch-s2t-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/PKG-INFO` & `mediacatch-s2t-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.1.3
+Version: 0.1.4
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mediacatch-s2t-0.1.3/README.md` & `mediacatch-s2t-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/pyproject.toml` & `mediacatch-s2t-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mediacatch-s2t"
-version = '0.1.3'
+version = '0.1.4'
 description = "Upload a media file and get the transcription link."
 readme = "README.md"
 authors = [{ name = "MediaCatch", email = "support@mediacatch.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mediacatch-s2t-0.1.3/src/mediacatch_s2t/__init__.py` & `mediacatch-s2t-0.1.4/src/mediacatch_s2t/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """MediaCatch speech-to-text file uploader.
 
 """
 
 # Version of the mc-s2t-mediacatch_s2t
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 import os
 
 URL: str = os.environ.get('MEDIACATCH_URL', 'https://s2t.mediacatch.io')
 SINGLE_UPLOAD_ENDPOINT: str = os.environ.get(
     'MEDIACATCH_PRESIGN_ENDPOINT',
     '/presigned-post-url')
```

### Comparing `mediacatch-s2t-0.1.3/src/mediacatch_s2t/__main__.py` & `mediacatch-s2t-0.1.4/src/mediacatch_s2t/__main__.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/src/mediacatch_s2t/helper.py` & `mediacatch-s2t-0.1.4/src/mediacatch_s2t/helper.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/src/mediacatch_s2t/uploader.py` & `mediacatch-s2t-0.1.4/src/mediacatch_s2t/uploader.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/PKG-INFO` & `mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.1.3
+Version: 0.1.4
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mediacatch-s2t-0.1.3/src/mediacatch_s2t.egg-info/SOURCES.txt` & `mediacatch-s2t-0.1.4/src/mediacatch_s2t.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/tests/test_helper.py` & `mediacatch-s2t-0.1.4/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/tests/test_multipart_upload.py` & `mediacatch-s2t-0.1.4/tests/test_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.1.3/tests/test_uploader.py` & `mediacatch-s2t-0.1.4/tests/test_uploader.py`

 * *Files identical despite different names*

