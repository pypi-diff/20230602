# Comparing `tmp/threefive-2.3.91.tar.gz` & `tmp/threefive-2.3.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threefive-2.3.91.tar", last modified: Tue May 16 17:15:57 2023, max compression
+gzip compressed data, was "threefive-2.3.93.tar", last modified: Thu Jun  1 22:05:30 2023, max compression
```

## Comparing `threefive-2.3.91.tar` & `threefive-2.3.93.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-16 17:15:57.036174 threefive-2.3.91/
--rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.91/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)    13135 2023-05-16 17:15:57.036174 threefive-2.3.91/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)    12564 2023-05-16 17:14:07.000000 threefive-2.3.91/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-16 17:15:57.032174 threefive-2.3.91/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.91/bin/threefive
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-16 17:15:57.036174 threefive-2.3.91/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.91/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-16 17:15:57.036174 threefive-2.3.91/threefive/
--rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/base.py
--rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/bitn.py
--rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/commands.py
--rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/crc.py
--rw-r--r--   0 a         (1000) a         (1000)    10561 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/cue.py
--rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/decode.py
--rw-r--r--   0 a         (1000) a         (1000)    13788 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/descriptors.py
--rw-r--r--   0 a         (1000) a         (1000)     2719 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/encode.py
--rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/packetdata.py
--rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/section.py
--rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/segment.py
--rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/segmentation.py
--rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/smoketest.py
--rw-r--r--   0 a         (1000) a         (1000)    18046 2023-05-16 17:14:07.000000 threefive-2.3.91/threefive/stream.py
--rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/stuff.py
--rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.91/threefive/upids.py
--rw-r--r--   0 a         (1000) a         (1000)       43 2023-05-16 17:15:50.000000 threefive-2.3.91/threefive/version.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-16 17:15:57.036174 threefive-2.3.91/threefive.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    13135 2023-05-16 17:15:56.000000 threefive-2.3.91/threefive.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      577 2023-05-16 17:15:56.000000 threefive-2.3.91/threefive.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-16 17:15:56.000000 threefive-2.3.91/threefive.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       24 2023-05-16 17:15:56.000000 threefive-2.3.91/threefive.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       10 2023-05-16 17:15:56.000000 threefive-2.3.91/threefive.egg-info/top_level.txt
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.829386 threefive-2.3.93/
+-rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.93/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)    13246 2023-06-01 22:05:30.829386 threefive-2.3.93/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)    12675 2023-06-01 22:04:12.000000 threefive-2.3.93/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.821387 threefive-2.3.93/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.93/bin/threefive
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-01 22:05:30.829386 threefive-2.3.93/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.93/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.825386 threefive-2.3.93/threefive/
+-rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/base.py
+-rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/bitn.py
+-rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/commands.py
+-rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/crc.py
+-rw-r--r--   0 a         (1000) a         (1000)    10704 2023-06-01 22:01:07.000000 threefive-2.3.93/threefive/cue.py
+-rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/decode.py
+-rw-r--r--   0 a         (1000) a         (1000)    13788 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/descriptors.py
+-rw-r--r--   0 a         (1000) a         (1000)     2719 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/encode.py
+-rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/packetdata.py
+-rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/section.py
+-rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/segment.py
+-rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/segmentation.py
+-rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/smoketest.py
+-rw-r--r--   0 a         (1000) a         (1000)    18046 2023-05-16 17:14:07.000000 threefive-2.3.93/threefive/stream.py
+-rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/stuff.py
+-rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.93/threefive/upids.py
+-rw-r--r--   0 a         (1000) a         (1000)       43 2023-06-01 22:04:12.000000 threefive-2.3.93/threefive/version.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 22:05:30.825386 threefive-2.3.93/threefive.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)    13246 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      577 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       24 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       10 2023-06-01 22:05:30.000000 threefive-2.3.93/threefive.egg-info/top_level.txt
```

### Comparing `threefive-2.3.91/LICENSE` & `threefive-2.3.93/LICENSE`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/PKG-INFO` & `threefive-2.3.93/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,10 @@
-Metadata-Version: 2.1
-Name: threefive
-Version: 2.3.91
-Summary: Pythonic SCTE35
-Home-page: https://github.com/futzu/threefive
-Author: Adrian and a Cast of Thousands.
-Author-email: spam@iodisco.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-## `threefive` `is` `the` `highest` `rated` `SCTE-35` `tool` . `Ever` .  <br/>                  `I` `swear` `.` 
-
-<details><summary><b>Latest Version is 2.3.89</b><i> (fix for me leaving stray files in the build)</i> </summary>
+<details><summary><b>Latest Version is 2.3.93</b><i> (workaround to handle Amazon not padding base64 correctly)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
 
@@ -505,9 +489,9 @@
 
 ### other threefive stuff
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
-  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need.*
+  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue. I am NOT the SCTE-35 Support Hotline. Do your own damn homework*
```

### Comparing `threefive-2.3.91/README.md` & `threefive-2.3.93/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,26 @@
-## `threefive` `is` `the` `highest` `rated` `SCTE-35` `tool` . `Ever` .  <br/>                  `I` `swear` `.` 
+Metadata-Version: 2.1
+Name: threefive
+Version: 2.3.93
+Summary: Pythonic SCTE35
+Home-page: https://github.com/futzu/threefive
+Author: Adrian and a Cast of Thousands.
+Author-email: spam@iodisco.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-<details><summary><b>Latest Version is 2.3.89</b><i> (fix for me leaving stray files in the build)</i> </summary>
+![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
+
+<details><summary><b>Latest Version is 2.3.93</b><i> (workaround to handle Amazon not padding base64 correctly)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
 
@@ -489,9 +505,9 @@
 
 ### other threefive stuff
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
-  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need.*
+  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue. I am NOT the SCTE-35 Support Hotline. Do your own damn homework*
```

### Comparing `threefive-2.3.91/bin/threefive` & `threefive-2.3.93/bin/threefive`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/setup.py` & `threefive-2.3.93/setup.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/__init__.py` & `threefive-2.3.93/threefive/__init__.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/base.py` & `threefive-2.3.93/threefive/base.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/bitn.py` & `threefive-2.3.93/threefive/bitn.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/commands.py` & `threefive-2.3.93/threefive/commands.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/crc.py` & `threefive-2.3.93/threefive/crc.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/cue.py` & `threefive-2.3.93/threefive/cue.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,20 @@
         """
         Cue.get_json returns the Cue instance
         data in json.
         """
         return json.dumps(self.get(), indent=4)
 
     @staticmethod
+    def fix_bad_b64(data):
+        while len(data) % 4 !=0:
+            data=data+'='
+        return data
+
+    @staticmethod
     def _mk_bits(data):
         """
         cue._mk_bits Converts
         Hex and Base64 strings into bytes.
         """
         if isinstance(data, bytes):
             return data[data.index(b"\xfc") :]
@@ -140,15 +146,15 @@
             return bites
         except (LookupError, TypeError, ValueError):
             if data[:2].lower() == "0x":
                 data = data[2:]
             if data[:2].lower() == "fc":
                 return bytes.fromhex(data)
         try:
-            return b64decode(data)
+            return b64decode(self.fix_bad_b64(data))
         except (LookupError, TypeError, ValueError):
             return data
 
     def _mk_descriptors(self, bites):
         """
         Cue._mk_descriptors parses
         Cue.info_section.descriptor_loop_length,
```

### Comparing `threefive-2.3.91/threefive/decode.py` & `threefive-2.3.93/threefive/decode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/descriptors.py` & `threefive-2.3.93/threefive/descriptors.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/encode.py` & `threefive-2.3.93/threefive/encode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/packetdata.py` & `threefive-2.3.93/threefive/packetdata.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/section.py` & `threefive-2.3.93/threefive/section.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/segment.py` & `threefive-2.3.93/threefive/segment.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/segmentation.py` & `threefive-2.3.93/threefive/segmentation.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/smoketest.py` & `threefive-2.3.93/threefive/smoketest.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/stream.py` & `threefive-2.3.93/threefive/stream.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive/upids.py` & `threefive-2.3.93/threefive/upids.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.91/threefive.egg-info/PKG-INFO` & `threefive-2.3.93/threefive.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.3.91
+Version: 2.3.93
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## `threefive` `is` `the` `highest` `rated` `SCTE-35` `tool` . `Ever` .  <br/>                  `I` `swear` `.` 
+![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-<details><summary><b>Latest Version is 2.3.89</b><i> (fix for me leaving stray files in the build)</i> </summary>
+<details><summary><b>Latest Version is 2.3.93</b><i> (workaround to handle Amazon not padding base64 correctly)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
 
@@ -505,9 +505,9 @@
 
 ### other threefive stuff
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
-  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need.*
+  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue. I am NOT the SCTE-35 Support Hotline. Do your own damn homework*
```

### Comparing `threefive-2.3.91/threefive.egg-info/SOURCES.txt` & `threefive-2.3.93/threefive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

