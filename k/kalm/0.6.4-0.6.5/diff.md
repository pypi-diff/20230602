# Comparing `tmp/kalm-0.6.4.tar.gz` & `tmp/kalm-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.6.4.tar", max compression
+gzip compressed data, was "kalm-0.6.5.tar", max compression
```

## Comparing `kalm-0.6.4.tar` & `kalm-0.6.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.4/LICENSE.txt
--rw-r--r--   0        0        0     1878 2023-06-02 10:48:49.438130 kalm-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    10461 2023-06-02 10:48:49.438130 kalm-0.6.4/src/kalm/__init__.py
--rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.4/src/kalm/jenkins.py
--rw-r--r--   0        0        0    32805 2023-06-02 10:44:12.320508 kalm-0.6.4/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.4/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.4/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.4/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0     1910 2023-06-02 11:01:34.750614 kalm-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    10461 2023-06-02 10:48:49.438130 kalm-0.6.5/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.5/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    32889 2023-06-02 11:00:00.282060 kalm-0.6.5/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.5/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.5/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.5/src/kalm/toolbox.py
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 kalm-0.6.5/PKG-INFO
```

### Comparing `kalm-0.6.4/LICENSE.txt` & `kalm-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.6.4/pyproject.toml` & `kalm-0.6.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.6.4"
+version = "0.6.5"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
@@ -19,20 +19,21 @@
 mypy = "^0.910"
 redis = "^4.5.3"
 pynetbox = "^6.6.2"
 wheel = "^0.34.2"
 hvac = "^1.1.0"
 netbox = "^0.0.2"
 python-jenkins = "^1.7.0"
+urllib3 = "^2.0.2"
 
 
 
 [project]
 name = "kalm"  
-version = "0.6.4" 
+version = "0.6.5" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
@@ -54,15 +55,16 @@
 ]
 
 dependencies = [ # Optional
   "redis",
   "pynetbox",
   "wheel",
   "hvac",
-  "netbox"
+  "netbox",
+  "urllib3"
 ]
 
 [project.optional-dependencies] # Optional
 dev = ["check-manifest"]
 test = ["coverage"]
 
 [project.urls]  # Optional
```

### Comparing `kalm-0.6.4/src/kalm/__init__.py` & `kalm-0.6.5/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.4/src/kalm/kalm.py` & `kalm-0.6.5/src/kalm/kalm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 import json
 import requests
 import hvac
 import os
 import sys
 import datetime
 import pynetbox
+import urllib3
 import datetime
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
 VERIFY_SSL = os.getenv("VERIFY_SSL", "false")
 if VERIFY_SSL == "false" or VERIFY_SSL == "False" or VERIFY_SSL == "FALSE" or VERIFY_SSL == "no" or VERIFY_SSL == "NO" or VERIFY_SSL == "No":
   VERIFY_SSL = False
 else:
   VERIFY_SSL = True
```

### Comparing `kalm-0.6.4/src/kalm/netbox.py` & `kalm-0.6.5/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.4/PKG-INFO` & `kalm-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.6.4
+Version: 0.6.5
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,9 +17,10 @@
 Requires-Dist: mypy (>=0.910,<0.911)
 Requires-Dist: netbox (>=0.0.2,<0.0.3)
 Requires-Dist: pynetbox (>=6.6.2,<7.0.0)
 Requires-Dist: pytest (>=6.2,<7.0)
 Requires-Dist: python-jenkins (>=1.7.0,<2.0.0)
 Requires-Dist: redis (>=4.5.3,<5.0.0)
 Requires-Dist: requests (>=2.25,<3.0)
+Requires-Dist: urllib3 (>=2.0.2,<3.0.0)
 Requires-Dist: wheel (>=0.34.2,<0.35.0)
 Project-URL: Repository, https://github.com/miracle-as/openknowit_kalm.git
```

