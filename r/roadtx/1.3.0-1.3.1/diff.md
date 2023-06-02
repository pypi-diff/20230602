# Comparing `tmp/roadtx-1.3.0.tar.gz` & `tmp/roadtx-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadtx-1.3.0.tar", last modified: Mon May 22 14:43:38 2023, max compression
+gzip compressed data, was "roadtx-1.3.1.tar", last modified: Fri Jun  2 13:39:09 2023, max compression
```

## Comparing `roadtx-1.3.0.tar` & `roadtx-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-05-22 14:43:38.582876 roadtx-1.3.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/roadtools/roadtx/
--rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-05-22 14:42:07.000000 roadtx-1.3.0/roadtools/roadtx/keepass.py
--rw-r--r--   0 vsts      (1001) docker     (123)    51917 2023-05-22 14:42:07.000000 roadtx-1.3.0/roadtools/roadtx/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12028 2023-05-22 14:42:07.000000 roadtx-1.3.0/roadtools/roadtx/selenium.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 14:43:38.582876 roadtx-1.3.0/roadtx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      301 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-22 14:43:35.000000 roadtx-1.3.0/roadtx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       66 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-22 14:43:38.000000 roadtx-1.3.0/roadtx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-22 14:43:38.582876 roadtx-1.3.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-22 14:42:07.000000 roadtx-1.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-02 13:39:09.951048 roadtx-1.3.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/roadtools/roadtx/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-06-02 13:37:39.000000 roadtx-1.3.1/roadtools/roadtx/keepass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    52146 2023-06-02 13:37:39.000000 roadtx-1.3.1/roadtools/roadtx/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12028 2023-06-02 13:37:39.000000 roadtx-1.3.1/roadtools/roadtx/selenium.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 13:39:09.951048 roadtx-1.3.1/roadtx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      301 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 13:39:07.000000 roadtx-1.3.1/roadtx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       66 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-02 13:39:09.000000 roadtx-1.3.1/roadtx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-02 13:39:09.951048 roadtx-1.3.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-06-02 13:37:39.000000 roadtx-1.3.1/setup.py
```

### Comparing `roadtx-1.3.0/PKG-INFO` & `roadtx-1.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.3.0
+Version: 1.3.1
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.3.0/roadtools/roadtx/keepass.py` & `roadtx-1.3.1/roadtools/roadtx/keepass.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.3.0/roadtools/roadtx/main.py` & `roadtx-1.3.1/roadtools/roadtx/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,18 @@
     browserprtauth_parser.add_argument('-s',
                                        '--scope',
                                        action='store',
                                        help='Scope to use. Will automatically switch to v2.0 auth endpoint if specified. If unsure use -r instead.')
     browserprtauth_parser.add_argument('-ru', '--redirect-url', action='store', metavar='URL',
                                        help='Redirect URL used when authenticating (default: https://login.microsoftonline.com/common/oauth2/nativeclient)',
                                        default="https://login.microsoftonline.com/common/oauth2/nativeclient")
+    browserprtauth_parser.add_argument('-t',
+                                       '--tenant',
+                                       action='store',
+                                       help='Tenant ID or domain to auth to')
     browserprtauth_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (default: roadtx.prt)')
     browserprtauth_parser.add_argument('--prt',
                                        action='store',
                                        help='Primary Refresh Token')
     browserprtauth_parser.add_argument('--prt-sessionkey',
                                        action='store',
                                        help='Primary Refresh Token session key (as hex key)')
```

### Comparing `roadtx-1.3.0/roadtools/roadtx/selenium.py` & `roadtx-1.3.1/roadtools/roadtx/selenium.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.3.0/roadtx.egg-info/PKG-INFO` & `roadtx-1.3.1/roadtx.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.3.0
+Version: 1.3.1
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.3.0/setup.py` & `roadtx-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadtx',
-      version='1.3.0',
+      version='1.3.1',
       description='ROADtools Token eXchange',
       author='Dirk-jan Mollema',
       author_email='dirkjan@outsidersecurity.nl',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
```

