# Comparing `tmp/kalm-0.6.3.tar.gz` & `tmp/kalm-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.6.3.tar", max compression
+gzip compressed data, was "kalm-0.6.4.tar", max compression
```

## Comparing `kalm-0.6.3.tar` & `kalm-0.6.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.3/LICENSE.txt
--rw-r--r--   0        0        0     1878 2023-06-02 10:44:12.320508 kalm-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/__init__.py
--rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.3/src/kalm/jenkins.py
--rw-r--r--   0        0        0    32805 2023-06-02 10:44:12.320508 kalm-0.6.3/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.3/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.4/LICENSE.txt
+-rw-r--r--   0        0        0     1878 2023-06-02 10:48:49.438130 kalm-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    10461 2023-06-02 10:48:49.438130 kalm-0.6.4/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.4/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    32805 2023-06-02 10:44:12.320508 kalm-0.6.4/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.4/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.4/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.4/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.4/PKG-INFO
```

### Comparing `kalm-0.6.3/LICENSE.txt` & `kalm-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.6.3/pyproject.toml` & `kalm-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.6.3"
+version = "0.6.4"
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
-version = "0.6.3" 
+version = "0.6.4" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.6.3/src/kalm/__init__.py` & `kalm-0.6.4/src/kalm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         setupkalm(force)
 
     if args.action[0] == "service":
         r = redis.Redis()
         r.flushdb()
         servicefile = open("/etc/kalm/kalm.service.token", mode="r")
         token = servicefile.read()
+        token = token.replace("\n", "")
         while True:
             print("Daemon running")
             kalm.kalm(token, r)
             print("Daemon sleeping")
             time.sleep(60)
```

### Comparing `kalm-0.6.3/src/kalm/kalm.py` & `kalm-0.6.4/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.3/src/kalm/netbox.py` & `kalm-0.6.4/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.3/PKG-INFO` & `kalm-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.6.3
+Version: 0.6.4
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

