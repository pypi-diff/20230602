# Comparing `tmp/ronnytest-0.2.8.tar.gz` & `tmp/ronnytest-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.2.8.tar", last modified: Mon May 29 11:11:05 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.3.0.tar", last modified: Fri Jun  2 08:21:20 2023, max compression
```

## Comparing `ronnytest-0.2.8.tar` & `ronnytest-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:11:05.000000 ronnytest-0.2.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-29 11:11:05.000000 ronnytest-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 11:11:05.000000 ronnytest-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-29 11:10:49.000000 ronnytest-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 08:21:20.000000 ronnytest-0.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 08:21:20.000000 ronnytest-0.3.0/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-06-02 08:21:20.000000 ronnytest-0.3.0/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 08:21:20.000000 ronnytest-0.3.0/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-02 08:21:20.000000 ronnytest-0.3.0/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 08:21:20.000000 ronnytest-0.3.0/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      220 2023-06-02 08:21:20.000000 ronnytest-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 08:21:20.000000 ronnytest-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-02 08:19:59.000000 ronnytest-0.3.0/setup.py
```

### Comparing `ronnytest-0.2.8/LICENSE` & `ronnytest-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.2.8/setup.py` & `ronnytest-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         raise RuntimeError('do not install!')
     
     _in_check_actions()
 
 
 setup(
     name = 'ronnytest',
-    version = '0.2.8',
+    version = '0.3.0',
     author = 'wxpay_sec_team',
     author_email = 'wxpay_sec_team@tencent.com',
     packages = find_packages(),
     install_requires=[""],
     tests_require=[],
 )
```

