# Comparing `tmp/PySpeedMacro-0.0.0.7.tar.gz` & `tmp/PySpeedMacro-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\epicg\Desktop\PySpeedMacroRepos\PySpeedMacroPRERELEASE\dist\.tmp-a52xrymq\PySpeedMacro-0.0.0.7.tar", last modified: Tue Mar  7 03:45:00 2023, max compression
+gzip compressed data, was "C:\Users\epicg\Desktop\PySpeedMacroRepos\PySpeedMacroPRERELEASE\dist\.tmp-qim5irgv\PySpeedMacro-0.0.0.8.tar", last modified: Fri Jun  2 02:48:13 2023, max compression
```

## Comparing `PySpeedMacro-0.0.0.7.tar` & `PySpeedMacro-0.0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 03:45:00.335386 PySpeedMacro-0.0.0.7/
--rw-rw-rw-   0        0        0     1094 2023-03-05 16:30:01.000000 PySpeedMacro-0.0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2024 2023-03-07 03:45:00.335386 PySpeedMacro-0.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2023-03-05 18:01:27.000000 PySpeedMacro-0.0.0.7/README.md
--rw-rw-rw-   0        0        0      104 2023-03-05 15:57:09.000000 PySpeedMacro-0.0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      691 2023-03-07 03:45:00.335386 PySpeedMacro-0.0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-07 03:45:00.320066 PySpeedMacro-0.0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-03-07 03:45:00.328069 PySpeedMacro-0.0.0.7/src/PySpeedMacro/
--rw-rw-rw-   0        0        0     3459 2023-03-06 21:14:14.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro/PSMInterface.py
--rw-rw-rw-   0        0        0    18367 2023-03-07 03:42:43.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro/PSMMain.py
--rw-rw-rw-   0        0        0     2005 2023-02-28 20:36:29.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro/PSMMouse.py
--rw-rw-rw-   0        0        0      811 2023-03-05 19:16:18.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 03:45:00.332069 PySpeedMacro-0.0.0.7/src/PySpeedMacro.egg-info/
--rw-rw-rw-   0        0        0     2024 2023-03-07 03:45:00.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-03-07 03:45:00.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 03:45:00.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-07 03:45:00.000000 PySpeedMacro-0.0.0.7/src/PySpeedMacro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-07 03:45:00.334070 PySpeedMacro-0.0.0.7/tests/
--rw-rw-rw-   0        0        0     1983 2023-03-05 20:05:29.000000 PySpeedMacro-0.0.0.7/tests/testMore.py
--rw-rw-rw-   0        0        0       58 2023-03-06 00:17:44.000000 PySpeedMacro-0.0.0.7/tests/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:48:13.216685 PySpeedMacro-0.0.0.8/
+-rw-rw-rw-   0        0        0     1094 2023-03-05 16:30:01.000000 PySpeedMacro-0.0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2024 2023-06-02 02:48:13.216685 PySpeedMacro-0.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2023-06-02 02:42:34.000000 PySpeedMacro-0.0.0.8/README.md
+-rw-rw-rw-   0        0        0      104 2023-03-05 15:57:09.000000 PySpeedMacro-0.0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      691 2023-06-02 02:48:13.216685 PySpeedMacro-0.0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 02:48:13.200056 PySpeedMacro-0.0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 02:48:13.216685 PySpeedMacro-0.0.0.8/src/PySpeedMacro/
+-rw-rw-rw-   0        0        0     3459 2023-03-06 21:14:14.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro/PSMInterface.py
+-rw-rw-rw-   0        0        0    18367 2023-03-07 03:42:43.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro/PSMMain.py
+-rw-rw-rw-   0        0        0     2005 2023-02-28 20:36:29.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro/PSMMouse.py
+-rw-rw-rw-   0        0        0      811 2023-03-05 19:16:18.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:48:13.216685 PySpeedMacro-0.0.0.8/src/PySpeedMacro.egg-info/
+-rw-rw-rw-   0        0        0     2024 2023-06-02 02:48:13.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-06-02 02:48:13.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 02:48:13.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 02:48:13.000000 PySpeedMacro-0.0.0.8/src/PySpeedMacro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 02:48:13.216685 PySpeedMacro-0.0.0.8/tests/
+-rw-rw-rw-   0        0        0     1983 2023-03-05 20:05:29.000000 PySpeedMacro-0.0.0.8/tests/testMore.py
+-rw-rw-rw-   0        0        0       58 2023-03-06 00:17:44.000000 PySpeedMacro-0.0.0.8/tests/testing.py
```

### Comparing `PySpeedMacro-0.0.0.7/LICENSE` & `PySpeedMacro-0.0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PySpeedMacro-0.0.0.7/PKG-INFO` & `PySpeedMacro-0.0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySpeedMacro
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: A fast and easy library for scripting and macroing
 Home-page: https://github.com/BaneofRogue/PySpeedMacro
 Author: William Keller
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/BaneofRogue/PySpeedMacro/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PySpeedMacro-0.0.0.7/README.md` & `PySpeedMacro-0.0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PySpeedMacro-0.0.0.7/setup.cfg` & `PySpeedMacro-0.0.0.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7953 7065 6564 4d61 6372 6f0d   = PySpeedMacro.
 00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e30  .version = 0.0.0
-00000030: 2e37 0d0a 6175 7468 6f72 203d 2057 696c  .7..author = Wil
+00000030: 2e38 0d0a 6175 7468 6f72 203d 2057 696c  .8..author = Wil
 00000040: 6c69 616d 204b 656c 6c65 720d 0a61 7574  liam Keller..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6175 7468  hor_email = auth
 00000060: 6f72 4065 7861 6d70 6c65 2e63 6f6d 0d0a  or@example.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000080: 6661 7374 2061 6e64 2065 6173 7920 6c69  fast and easy li
 00000090: 6272 6172 7920 666f 7220 7363 7269 7074  brary for script
 000000a0: 696e 6720 616e 6420 6d61 6372 6f69 6e67  ing and macroing
```

### Comparing `PySpeedMacro-0.0.0.7/src/PySpeedMacro/PSMInterface.py` & `PySpeedMacro-0.0.0.8/src/PySpeedMacro/PSMInterface.py`

 * *Files identical despite different names*

### Comparing `PySpeedMacro-0.0.0.7/src/PySpeedMacro/PSMMain.py` & `PySpeedMacro-0.0.0.8/src/PySpeedMacro/PSMMain.py`

 * *Files identical despite different names*

### Comparing `PySpeedMacro-0.0.0.7/src/PySpeedMacro/PSMMouse.py` & `PySpeedMacro-0.0.0.8/src/PySpeedMacro/PSMMouse.py`

 * *Files identical despite different names*

### Comparing `PySpeedMacro-0.0.0.7/src/PySpeedMacro/__init__.py` & `PySpeedMacro-0.0.0.8/src/PySpeedMacro/__init__.py`

 * *Files identical despite different names*

### Comparing `PySpeedMacro-0.0.0.7/src/PySpeedMacro.egg-info/PKG-INFO` & `PySpeedMacro-0.0.0.8/src/PySpeedMacro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySpeedMacro
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: A fast and easy library for scripting and macroing
 Home-page: https://github.com/BaneofRogue/PySpeedMacro
 Author: William Keller
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/BaneofRogue/PySpeedMacro/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PySpeedMacro-0.0.0.7/tests/testMore.py` & `PySpeedMacro-0.0.0.8/tests/testMore.py`

 * *Files identical despite different names*

