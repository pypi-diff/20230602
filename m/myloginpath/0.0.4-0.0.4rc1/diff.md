# Comparing `tmp/myloginpath-0.0.4.tar.gz` & `tmp/myloginpath-0.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myloginpath-0.0.4.tar", last modified: Fri Jun  2 04:06:53 2023, max compression
+gzip compressed data, was "myloginpath-0.0.4rc1.tar", last modified: Sun May 21 10:07:53 2023, max compression
```

## Comparing `myloginpath-0.0.4.tar` & `myloginpath-0.0.4rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-02 04:06:53.061133 myloginpath-0.0.4/
--rw-r--r--   0 inada-n    (502) staff       (20)       31 2018-05-08 09:21:49.000000 myloginpath-0.0.4/AUTHORS
--rw-r--r--   0 inada-n    (502) staff       (20)     1068 2018-05-08 09:19:28.000000 myloginpath-0.0.4/LICENSE.txt
--rw-r--r--   0 inada-n    (502) staff       (20)     2803 2023-06-02 04:06:53.061019 myloginpath-0.0.4/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      651 2021-09-15 08:39:27.000000 myloginpath-0.0.4/README.md
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-02 04:06:53.060656 myloginpath-0.0.4/myloginpath.egg-info/
--rw-r--r--   0 inada-n    (502) staff       (20)     2803 2023-06-02 04:06:53.000000 myloginpath-0.0.4/myloginpath.egg-info/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      273 2023-06-02 04:06:53.000000 myloginpath-0.0.4/myloginpath.egg-info/SOURCES.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-06-02 04:06:53.000000 myloginpath-0.0.4/myloginpath.egg-info/dependency_links.txt
--rw-r--r--   0 inada-n    (502) staff       (20)       13 2023-06-02 04:06:53.000000 myloginpath-0.0.4/myloginpath.egg-info/requires.txt
--rw-r--r--   0 inada-n    (502) staff       (20)       12 2023-06-02 04:06:53.000000 myloginpath-0.0.4/myloginpath.egg-info/top_level.txt
--rw-r--r--   0 inada-n    (502) staff       (20)     3867 2021-09-09 07:34:55.000000 myloginpath-0.0.4/myloginpath.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1043 2023-06-02 04:05:41.000000 myloginpath-0.0.4/pyproject.toml
--rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-06-02 04:06:53.061166 myloginpath-0.0.4/setup.cfg
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-02 04:06:53.060879 myloginpath-0.0.4/test/
--rw-r--r--   0 inada-n    (502) staff       (20)      716 2021-09-09 07:34:55.000000 myloginpath-0.0.4/test/test_decrypt.py
--rw-r--r--   0 inada-n    (502) staff       (20)      826 2021-09-09 07:34:55.000000 myloginpath-0.0.4/test/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/myloginpath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/myloginpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/test/test_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/test/test_parse.py
```

### Comparing `myloginpath-0.0.4/LICENSE.txt` & `myloginpath-0.0.4rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myloginpath-0.0.4/PKG-INFO` & `myloginpath-0.0.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myloginpath
-Version: 0.0.4
+Version: 0.0.4rc1
 Summary: MySQL login path file reader
 Author-email: Inada Naoki <songofacandy@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Inada Naoki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `myloginpath-0.0.4/README.md` & `myloginpath-0.0.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `myloginpath-0.0.4/myloginpath.egg-info/PKG-INFO` & `myloginpath-0.0.4rc1/myloginpath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myloginpath
-Version: 0.0.4
+Version: 0.0.4rc1
 Summary: MySQL login path file reader
 Author-email: Inada Naoki <songofacandy@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Inada Naoki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `myloginpath-0.0.4/myloginpath.py` & `myloginpath-0.0.4rc1/myloginpath.py`

 * *Files identical despite different names*

### Comparing `myloginpath-0.0.4/pyproject.toml` & `myloginpath-0.0.4rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "myloginpath"
-version = "0.0.4"
+version = "0.0.4rc1"
 description="MySQL login path file reader"
 
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     {name = "Inada Naoki", email = "songofacandy@gmail.com"}
 ]
```

### Comparing `myloginpath-0.0.4/test/test_decrypt.py` & `myloginpath-0.0.4rc1/test/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `myloginpath-0.0.4/test/test_parse.py` & `myloginpath-0.0.4rc1/test/test_parse.py`

 * *Files identical despite different names*

