# Comparing `tmp/threefive-2.3.93.tar.gz` & `tmp/threefive-2.3.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threefive-2.3.93.tar", last modified: Thu Jun  1 22:05:30 2023, max compression
+gzip compressed data, was "threefive-2.3.95.tar", last modified: Thu Jun  1 23:43:37 2023, max compression
```

## Comparing `threefive-2.3.93.tar` & `threefive-2.3.95.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.829386 threefive-2.3.93/
--rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.93/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)    13246 2023-06-01 22:05:30.829386 threefive-2.3.93/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)    12675 2023-06-01 22:04:12.000000 threefive-2.3.93/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.821387 threefive-2.3.93/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.93/bin/threefive
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-01 22:05:30.829386 threefive-2.3.93/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.93/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.825386 threefive-2.3.93/threefive/
--rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/base.py
--rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/bitn.py
--rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/commands.py
--rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/crc.py
--rw-r--r--   0 a         (1000) a         (1000)    10704 2023-06-01 22:01:07.000000 threefive-2.3.93/threefive/cue.py
--rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/decode.py
--rw-r--r--   0 a         (1000) a         (1000)    13788 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/descriptors.py
--rw-r--r--   0 a         (1000) a         (1000)     2719 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/encode.py
--rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/packetdata.py
--rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/section.py
--rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/segment.py
--rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/segmentation.py
--rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/smoketest.py
--rw-r--r--   0 a         (1000) a         (1000)    18046 2023-05-16 17:14:07.000000 threefive-2.3.93/threefive/stream.py
--rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/stuff.py
--rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/upids.py
--rw-r--r--   0 a         (1000) a         (1000)       43 2023-06-01 22:04:12.000000 threefive-2.3.93/threefive/version.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.825386 threefive-2.3.93/threefive.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    13246 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      577 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       24 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       10 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/top_level.txt
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.213339 threefive-2.3.95/
+-rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.95/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)    13225 2023-06-01 23:43:37.213339 threefive-2.3.95/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)    12654 2023-06-01 23:43:28.000000 threefive-2.3.95/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.209338 threefive-2.3.95/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.95/bin/threefive
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-01 23:43:37.213339 threefive-2.3.95/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.95/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.213339 threefive-2.3.95/threefive/
+-rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/base.py
+-rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/bitn.py
+-rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/commands.py
+-rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/crc.py
+-rw-r--r--   0 a         (1000) a         (1000)    10691 2023-06-01 23:43:28.000000 threefive-2.3.95/threefive/cue.py
+-rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/decode.py
+-rw-r--r--   0 a         (1000) a         (1000)    13788 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/descriptors.py
+-rw-r--r--   0 a         (1000) a         (1000)     2719 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/encode.py
+-rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/packetdata.py
+-rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/section.py
+-rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/segment.py
+-rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/segmentation.py
+-rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/smoketest.py
+-rw-r--r--   0 a         (1000) a         (1000)    18046 2023-05-16 17:14:07.000000 threefive-2.3.95/threefive/stream.py
+-rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/stuff.py
+-rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/upids.py
+-rw-r--r--   0 a         (1000) a         (1000)       43 2023-06-01 23:43:28.000000 threefive-2.3.95/threefive/version.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.213339 threefive-2.3.95/threefive.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)    13225 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      577 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       24 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       10 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/top_level.txt
```

### Comparing `threefive-2.3.93/LICENSE` & `threefive-2.3.95/LICENSE`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/PKG-INFO` & `threefive-2.3.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.3.93
+Version: 2.3.95
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-<details><summary><b>Latest Version is 2.3.93</b><i> (workaround to handle Amazon not padding base64 correctly)</i> </summary>
+<details><summary><b>Latest Version is 2.3.95</b><i> (fix for me breaking base64 decoding)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
```

### Comparing `threefive-2.3.93/README.md` & `threefive-2.3.95/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-<details><summary><b>Latest Version is 2.3.93</b><i> (workaround to handle Amazon not padding base64 correctly)</i> </summary>
+<details><summary><b>Latest Version is 2.3.95</b><i> (fix for me breaking base64 decoding)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
```

### Comparing `threefive-2.3.93/bin/threefive` & `threefive-2.3.95/bin/threefive`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/setup.py` & `threefive-2.3.95/setup.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/__init__.py` & `threefive-2.3.95/threefive/__init__.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/base.py` & `threefive-2.3.95/threefive/base.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/bitn.py` & `threefive-2.3.95/threefive/bitn.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/commands.py` & `threefive-2.3.95/threefive/commands.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/crc.py` & `threefive-2.3.95/threefive/crc.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/cue.py` & `threefive-2.3.95/threefive/cue.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,16 +121,15 @@
 
     @staticmethod
     def fix_bad_b64(data):
         while len(data) % 4 !=0:
             data=data+'='
         return data
 
-    @staticmethod
-    def _mk_bits(data):
+    def _mk_bits(self,data):
         """
         cue._mk_bits Converts
         Hex and Base64 strings into bytes.
         """
         if isinstance(data, bytes):
             return data[data.index(b"\xfc") :]
         # handles int and unquoted hex
```

### Comparing `threefive-2.3.93/threefive/decode.py` & `threefive-2.3.95/threefive/decode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/descriptors.py` & `threefive-2.3.95/threefive/descriptors.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/encode.py` & `threefive-2.3.95/threefive/encode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/packetdata.py` & `threefive-2.3.95/threefive/packetdata.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/section.py` & `threefive-2.3.95/threefive/section.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/segment.py` & `threefive-2.3.95/threefive/segment.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/segmentation.py` & `threefive-2.3.95/threefive/segmentation.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/smoketest.py` & `threefive-2.3.95/threefive/smoketest.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/stream.py` & `threefive-2.3.95/threefive/stream.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive/upids.py` & `threefive-2.3.95/threefive/upids.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.93/threefive.egg-info/PKG-INFO` & `threefive-2.3.95/threefive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.3.93
+Version: 2.3.95
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-<details><summary><b>Latest Version is 2.3.93</b><i> (workaround to handle Amazon not padding base64 correctly)</i> </summary>
+<details><summary><b>Latest Version is 2.3.95</b><i> (fix for me breaking base64 decoding)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
```

### Comparing `threefive-2.3.93/threefive.egg-info/SOURCES.txt` & `threefive-2.3.95/threefive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

