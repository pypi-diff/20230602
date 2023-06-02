# Comparing `tmp/cf-remote-0.4.6.tar.gz` & `tmp/cf-remote-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf-remote-0.4.6.tar", last modified: Fri Mar 17 15:13:07 2023, max compression
+gzip compressed data, was "cf-remote-0.4.7.tar", last modified: Fri Jun  2 13:35:26 2023, max compression
```

## Comparing `cf-remote-0.4.6.tar` & `cf-remote-0.4.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:13:07.723950 cf-remote-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-17 15:12:56.000000 cf-remote-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-03-17 15:13:07.723950 cf-remote-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-03-17 15:12:56.000000 cf-remote-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:13:07.723950 cf-remote-0.4.6/cf_remote/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 15:13:07.000000 cf-remote-0.4.6/cf_remote/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/aramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/cloud_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-17 15:12:56.000000 cf-remote-0.4.6/cf_remote/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:13:07.723950 cf-remote-0.4.6/cf_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-03-17 15:13:07.000000 cf-remote-0.4.6/cf_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-17 15:13:07.000000 cf-remote-0.4.6/cf_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 15:13:07.000000 cf-remote-0.4.6/cf_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 15:13:07.000000 cf-remote-0.4.6/cf_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-17 15:13:07.000000 cf-remote-0.4.6/cf_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-17 15:13:07.000000 cf-remote-0.4.6/cf_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 15:13:07.723950 cf-remote-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-17 15:12:56.000000 cf-remote-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:13:07.723950 cf-remote-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 15:12:56.000000 cf-remote-0.4.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-17 15:12:56.000000 cf-remote-0.4.6/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-17 15:12:56.000000 cf-remote-0.4.6/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-17 15:12:56.000000 cf-remote-0.4.6/tests/test_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:26.922789 cf-remote-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 13:35:09.000000 cf-remote-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-02 13:35:26.922789 cf-remote-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-06-02 13:35:09.000000 cf-remote-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:26.922789 cf-remote-0.4.7/cf_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 13:35:26.000000 cf-remote-0.4.7/cf_remote/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/aramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/cloud_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-02 13:35:09.000000 cf-remote-0.4.7/cf_remote/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:26.922789 cf-remote-0.4.7/cf_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-02 13:35:26.000000 cf-remote-0.4.7/cf_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 13:35:26.000000 cf-remote-0.4.7/cf_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:35:26.000000 cf-remote-0.4.7/cf_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 13:35:26.000000 cf-remote-0.4.7/cf_remote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 13:35:26.000000 cf-remote-0.4.7/cf_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 13:35:26.000000 cf-remote-0.4.7/cf_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:35:26.922789 cf-remote-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-02 13:35:09.000000 cf-remote-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:26.922789 cf-remote-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:09.000000 cf-remote-0.4.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-02 13:35:09.000000 cf-remote-0.4.7/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-02 13:35:09.000000 cf-remote-0.4.7/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 13:35:09.000000 cf-remote-0.4.7/tests/test_ssh.py
```

### Comparing `cf-remote-0.4.6/LICENSE` & `cf-remote-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/PKG-INFO` & `cf-remote-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-remote
-Version: 0.4.6
+Version: 0.4.7
 Summary: Tooling to deploy CFEngine (and much more)
 Home-page: https://github.com/cfengine/cf-remote
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -210,15 +210,15 @@
 [sudo] password for ubuntu:
 CFEngine 3.15.3 (Enterprise) was successfully installed on 'localhost'
 ```
 
 ## Contribute
 
 Feel free to open pull requests to expand this documentation, add features or fix problems.
-You can also pick up an existing task or file an issue in [our bug tracker](https://tracker.mender.io/issues/?filter=11711).
+You can also pick up an existing task or file an issue in [our bug tracker](https://northerntech.atlassian.net/issues/?filter=10068).
 
 ## Development
 
 To install `cf-remote` so that it reflects any changes in this source directory use:
 
 ```
 $ pip install --editable .
```

### Comparing `cf-remote-0.4.6/README.md` & `cf-remote-0.4.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 [sudo] password for ubuntu:
 CFEngine 3.15.3 (Enterprise) was successfully installed on 'localhost'
 ```
 
 ## Contribute
 
 Feel free to open pull requests to expand this documentation, add features or fix problems.
-You can also pick up an existing task or file an issue in [our bug tracker](https://tracker.mender.io/issues/?filter=11711).
+You can also pick up an existing task or file an issue in [our bug tracker](https://northerntech.atlassian.net/issues/?filter=10068).
 
 ## Development
 
 To install `cf-remote` so that it reflects any changes in this source directory use:
 
 ```
 $ pip install --editable .
```

### Comparing `cf-remote-0.4.6/cf_remote/aramid.py` & `cf-remote-0.4.7/cf_remote/aramid.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/cloud_data.py` & `cf-remote-0.4.7/cf_remote/cloud_data.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/commands.py` & `cf-remote-0.4.7/cf_remote/commands.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/demo.py` & `cf-remote-0.4.7/cf_remote/demo.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/log.py` & `cf-remote-0.4.7/cf_remote/log.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/main.py` & `cf-remote-0.4.7/cf_remote/main.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/packages.py` & `cf-remote-0.4.7/cf_remote/packages.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/paths.py` & `cf-remote-0.4.7/cf_remote/paths.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/remote.py` & `cf-remote-0.4.7/cf_remote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
     if version:
         release = releases.pick_version(version)
 
     release.init_download()
 
     if not release.artifacts:
         log.error(
-            "The {} {} release is empty, visit tracker.mender.io to file a bug report".format(
+            "The {} {} release is empty, visit northerntech.atlassian.net to file a bug report".format(
                 version, edition
             )
         )
         return None
 
     artifacts = release.find(tags, extension)
     if not artifacts:
```

### Comparing `cf-remote-0.4.6/cf_remote/spawn.py` & `cf-remote-0.4.7/cf_remote/spawn.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/ssh.py` & `cf-remote-0.4.7/cf_remote/ssh.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/utils.py` & `cf-remote-0.4.7/cf_remote/utils.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/cf_remote/web.py` & `cf-remote-0.4.7/cf_remote/web.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import fcntl
 import urllib.request
-import requests
+import json
+from collections import OrderedDict
 from cf_remote.utils import write_json, mkdir, parse_json
 from cf_remote import log
 from cf_remote.paths import cf_remote_dir, cf_remote_packages_dir
 
 
 def get_json(url):
-    r = requests.get(url)
-    assert r.status_code >= 200 and r.status_code < 300
-    data = parse_json(r.text)
+    with urllib.request.urlopen(url) as r:
+        assert r.status >= 200 and r.status < 300
+        data = json.loads(r.read().decode(), object_pairs_hook=OrderedDict)
 
     filename = os.path.basename(url)
     dir = cf_remote_dir("json")
     path = os.path.join(dir, filename)
     log.debug("Saving '{}' to '{}'".format(url, path))
     write_json(path, data)
```

### Comparing `cf-remote-0.4.6/cf_remote.egg-info/PKG-INFO` & `cf-remote-0.4.7/cf_remote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-remote
-Version: 0.4.6
+Version: 0.4.7
 Summary: Tooling to deploy CFEngine (and much more)
 Home-page: https://github.com/cfengine/cf-remote
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -210,15 +210,15 @@
 [sudo] password for ubuntu:
 CFEngine 3.15.3 (Enterprise) was successfully installed on 'localhost'
 ```
 
 ## Contribute
 
 Feel free to open pull requests to expand this documentation, add features or fix problems.
-You can also pick up an existing task or file an issue in [our bug tracker](https://tracker.mender.io/issues/?filter=11711).
+You can also pick up an existing task or file an issue in [our bug tracker](https://northerntech.atlassian.net/issues/?filter=10068).
 
 ## Development
 
 To install `cf-remote` so that it reflects any changes in this source directory use:
 
 ```
 $ pip install --editable .
```

### Comparing `cf-remote-0.4.6/cf_remote.egg-info/SOURCES.txt` & `cf-remote-0.4.7/cf_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/setup.py` & `cf-remote-0.4.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,11 +42,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.5",
     entry_points={"console_scripts": ["cf-remote = cf_remote.main:main"]},
     install_requires=[
-        "requests >= 2.25.1",
         "apache-libcloud >= 3.3.1",
     ],
 )
```

### Comparing `cf-remote-0.4.6/tests/test_cache.py` & `cf-remote-0.4.7/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.6/tests/test_packages.py` & `cf-remote-0.4.7/tests/test_packages.py`

 * *Files identical despite different names*

