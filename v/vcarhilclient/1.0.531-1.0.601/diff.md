# Comparing `tmp/vcarhilclient-1.0.531.tar.gz` & `tmp/vcarhilclient-1.0.601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcarhilclient-1.0.531.tar", last modified: Wed May 31 10:26:07 2023, max compression
+gzip compressed data, was "vcarhilclient-1.0.601.tar", last modified: Fri Jun  2 06:32:39 2023, max compression
```

## Comparing `vcarhilclient-1.0.531.tar` & `vcarhilclient-1.0.601.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 10:26:07.022249 vcarhilclient-1.0.531/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.531/LICENSE
--rw-rw-rw-   0        0        0     2644 2023-05-31 10:26:07.022249 vcarhilclient-1.0.531/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.531/README.md
--rw-rw-rw-   0        0        0       86 2023-05-31 10:26:07.023248 vcarhilclient-1.0.531/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-05-31 10:24:02.000000 vcarhilclient-1.0.531/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:26:07.006720 vcarhilclient-1.0.531/vcarhilclient/
--rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.531/vcarhilclient/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.531/vcarhilclient/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.531/vcarhilclient/drt_structures.py
--rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_ma.py
--rw-rw-rw-   0        0        0    50876 2023-05-31 10:22:11.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_mrt.py
--rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_project.py
--rw-rw-rw-   0        0        0    12059 2023-05-31 10:22:11.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_util.py
--rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.531/vcarhilclient/minio_handld.py
--rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.531/vcarhilclient/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.531/vcarhilclient/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:26:07.020238 vcarhilclient-1.0.531/vcarhilclient.egg-info/
--rw-rw-rw-   0        0        0     2644 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 06:32:39.163840 vcarhilclient-1.0.601/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.601/LICENSE
+-rw-rw-rw-   0        0        0     2596 2023-06-02 06:32:39.163840 vcarhilclient-1.0.601/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.601/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-02 06:32:39.164844 vcarhilclient-1.0.601/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-06-02 06:31:13.000000 vcarhilclient-1.0.601/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:32:39.151777 vcarhilclient-1.0.601/vcarhilclient/
+-rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.601/vcarhilclient/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.601/vcarhilclient/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.601/vcarhilclient/drt_structures.py
+-rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.601/vcarhilclient/kunyi_ma.py
+-rw-rw-rw-   0        0        0    50876 2023-05-31 10:22:11.000000 vcarhilclient-1.0.601/vcarhilclient/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.601/vcarhilclient/kunyi_project.py
+-rw-rw-rw-   0        0        0    12059 2023-05-31 10:22:11.000000 vcarhilclient-1.0.601/vcarhilclient/kunyi_util.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.601/vcarhilclient/minio_handld.py
+-rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.601/vcarhilclient/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.601/vcarhilclient/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:32:39.161842 vcarhilclient-1.0.601/vcarhilclient.egg-info/
+-rw-rw-rw-   0        0        0     2596 2023-06-02 06:32:38.000000 vcarhilclient-1.0.601/vcarhilclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-02 06:32:39.000000 vcarhilclient-1.0.601/vcarhilclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 06:32:38.000000 vcarhilclient-1.0.601/vcarhilclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-02 06:32:38.000000 vcarhilclient-1.0.601/vcarhilclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-02 06:32:38.000000 vcarhilclient-1.0.601/vcarhilclient.egg-info/top_level.txt
```

### Comparing `vcarhilclient-1.0.531/LICENSE` & `vcarhilclient-1.0.601/LICENSE`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/PKG-INFO` & `vcarhilclient-1.0.601/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.531
+Version: 1.0.601
 Summary: vcarhilclient
-Home-page: UNKNOWN
+Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +105,7 @@
 assert ec.value == 0
 
 # 18.Delete the experiment
 ec = my_mrt.delete_test_env("envName")
 
 assert ec.value == 0
 
-
-
```

### Comparing `vcarhilclient-1.0.531/README.md` & `vcarhilclient-1.0.601/README.md`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/setup.py` & `vcarhilclient-1.0.601/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vcarhilclient",  # 包名
-    version="1.0.531",
+    version="1.0.601",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="vcarhilclient",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `vcarhilclient-1.0.531/vcarhilclient/Enums.py` & `vcarhilclient-1.0.601/vcarhilclient/Enums.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient/kunyi_ma.py` & `vcarhilclient-1.0.601/vcarhilclient/kunyi_ma.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient/kunyi_mrt.py` & `vcarhilclient-1.0.601/vcarhilclient/kunyi_mrt.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient/kunyi_project.py` & `vcarhilclient-1.0.601/vcarhilclient/kunyi_project.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient/kunyi_util.py` & `vcarhilclient-1.0.601/vcarhilclient/kunyi_util.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient/minio_handld.py` & `vcarhilclient-1.0.601/vcarhilclient/minio_handld.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient/mrt_strunctures.py` & `vcarhilclient-1.0.601/vcarhilclient/mrt_strunctures.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient/signal_daq.py` & `vcarhilclient-1.0.601/vcarhilclient/signal_daq.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.531/vcarhilclient.egg-info/PKG-INFO` & `vcarhilclient-1.0.601/vcarhilclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.531
+Version: 1.0.601
 Summary: vcarhilclient
-Home-page: UNKNOWN
+Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +105,7 @@
 assert ec.value == 0
 
 # 18.Delete the experiment
 ec = my_mrt.delete_test_env("envName")
 
 assert ec.value == 0
 
-
-
```

