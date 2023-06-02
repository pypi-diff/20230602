# Comparing `tmp/kalm-0.6.2.tar.gz` & `tmp/kalm-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.6.2.tar", max compression
+gzip compressed data, was "kalm-0.6.3.tar", max compression
```

## Comparing `kalm-0.6.2.tar` & `kalm-0.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     1878 2023-06-02 10:22:47.576992 kalm-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/__init__.py
--rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.2/src/kalm/jenkins.py
--rw-r--r--   0        0        0    32790 2023-06-02 10:22:47.576992 kalm-0.6.2/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.3/LICENSE.txt
+-rw-r--r--   0        0        0     1878 2023-06-02 10:44:12.320508 kalm-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.3/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    32805 2023-06-02 10:44:12.320508 kalm-0.6.3/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.3/PKG-INFO
```

### Comparing `kalm-0.6.2/LICENSE.txt` & `kalm-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.6.2/pyproject.toml` & `kalm-0.6.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.6.2"
+version = "0.6.3"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
@@ -24,15 +24,15 @@
 netbox = "^0.0.2"
 python-jenkins = "^1.7.0"
 
 
 
 [project]
 name = "kalm"  
-version = "0.6.2" 
+version = "0.6.3" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.6.2/src/kalm/__init__.py` & `kalm-0.6.3/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.2/src/kalm/kalm.py` & `kalm-0.6.3/src/kalm/kalm.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
 
   data = {
     "name": name,
     "description": description,
     "job_type": "run",
     "inventory": invid,
     "project": projid,
-    "playbook": playbook,
+    "playbook": "playbooks/" + playbook,
     "scm_branch": "",
     "credential": credid,
     "forks": 0,
     "limit": "",
     "verbosity": 0,
     "extra_vars": "",
     "job_tags": "",
```

### Comparing `kalm-0.6.2/src/kalm/netbox.py` & `kalm-0.6.3/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.2/PKG-INFO` & `kalm-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.6.2
+Version: 0.6.3
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

