# Comparing `tmp/ec2_proxy-0.1.0.tar.gz` & `tmp/ec2_proxy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2_proxy-0.1.0.tar", last modified: Fri Jun  2 06:44:25 2023, max compression
+gzip compressed data, was "ec2_proxy-0.1.1.tar", last modified: Fri Jun  2 08:40:20 2023, max compression
```

## Comparing `ec2_proxy-0.1.0.tar` & `ec2_proxy-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 06:44:25.788850 ec2_proxy-0.1.0/
--rw-rw-rw-   0        0        0     3670 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0      599 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      252 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1851 2023-06-02 06:44:25.788850 ec2_proxy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      965 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-02 06:44:25.744657 ec2_proxy-0.1.0/docs/
--rw-rw-rw-   0        0        0      630 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0     4963 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      314 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1173 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      807 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       80 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-02 06:44:25.755235 ec2_proxy-0.1.0/ec2_proxy/
--rw-rw-rw-   0        0        0      179 2023-05-31 17:33:39.000000 ec2_proxy-0.1.0/ec2_proxy/__init__.py
--rw-rw-rw-   0        0        0     4964 2023-05-31 18:29:38.000000 ec2_proxy-0.1.0/ec2_proxy/ec2_proxy.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:44:25.784808 ec2_proxy-0.1.0/ec2_proxy.egg-info/
--rw-rw-rw-   0        0        0     1851 2023-06-02 06:44:25.000000 ec2_proxy-0.1.0/ec2_proxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-06-02 06:44:25.000000 ec2_proxy-0.1.0/ec2_proxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 06:44:25.000000 ec2_proxy-0.1.0/ec2_proxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 06:44:25.000000 ec2_proxy-0.1.0/ec2_proxy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-02 06:44:25.000000 ec2_proxy-0.1.0/ec2_proxy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2023-06-02 06:44:25.790849 ec2_proxy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1368 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:44:25.787842 ec2_proxy-0.1.0/tests/
--rw-rw-rw-   0        0        0       40 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      418 2023-06-02 06:40:47.000000 ec2_proxy-0.1.0/tests/test_ec2_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.233797 ec2_proxy-0.1.1/
+-rw-rw-rw-   0        0        0     3670 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-06-02 08:40:17.000000 ec2_proxy-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0      599 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1851 2023-06-02 08:40:20.234803 ec2_proxy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      965 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.208786 ec2_proxy-0.1.1/docs/
+-rw-rw-rw-   0        0        0      630 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0     4963 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      314 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1173 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      807 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       80 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.212792 ec2_proxy-0.1.1/ec2_proxy/
+-rw-rw-rw-   0        0        0      174 2023-06-02 08:40:13.000000 ec2_proxy-0.1.1/ec2_proxy/__init__.py
+-rw-rw-rw-   0        0        0     4964 2023-06-02 06:46:49.000000 ec2_proxy-0.1.1/ec2_proxy/ec2_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.229786 ec2_proxy-0.1.1/ec2_proxy.egg-info/
+-rw-rw-rw-   0        0        0     1851 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 06:44:25.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      404 2023-06-02 08:40:20.236796 ec2_proxy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1368 2023-06-02 08:40:10.000000 ec2_proxy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.232800 ec2_proxy-0.1.1/tests/
+-rw-rw-rw-   0        0        0       40 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/tests/test_ec2_proxy.py
```

### Comparing `ec2_proxy-0.1.0/CONTRIBUTING.rst` & `ec2_proxy-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/LICENSE` & `ec2_proxy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/PKG-INFO` & `ec2_proxy-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2_proxy
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides ability to use amazon aws as proxy with everchanging IP.
 Home-page: https://github.com/AG4lyf/ec2_proxy
 Author: Suraj Bhari
 Author-email: surajbhari159@gmail.com
 License: Apache Software License 2.0
 Keywords: ec2_proxy
 Platform: UNKNOWN
```

### Comparing `ec2_proxy-0.1.0/README.rst` & `ec2_proxy-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/docs/Makefile` & `ec2_proxy-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/docs/conf.py` & `ec2_proxy-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/docs/installation.rst` & `ec2_proxy-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/docs/make.bat` & `ec2_proxy-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/ec2_proxy/ec2_proxy.py` & `ec2_proxy-0.1.1/ec2_proxy/ec2_proxy.py`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.0/ec2_proxy.egg-info/PKG-INFO` & `ec2_proxy-0.1.1/ec2_proxy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-proxy
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides ability to use amazon aws as proxy with everchanging IP.
 Home-page: https://github.com/AG4lyf/ec2_proxy
 Author: Suraj Bhari
 Author-email: surajbhari159@gmail.com
 License: Apache Software License 2.0
 Keywords: ec2_proxy
 Platform: UNKNOWN
```

### Comparing `ec2_proxy-0.1.0/setup.py` & `ec2_proxy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='ec2_proxy',
     name='ec2_proxy',
     packages=find_packages(include=['ec2_proxy', 'ec2_proxy.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/AG4lyf/ec2_proxy',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

