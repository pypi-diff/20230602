# Comparing `tmp/appopener_test-1.0.tar.gz` & `tmp/appopener_test-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appopener_test-1.0.tar", last modified: Fri Jun  2 14:45:58 2023, max compression
+gzip compressed data, was "appopener_test-1.1.tar", last modified: Fri Jun  2 15:11:22 2023, max compression
```

## Comparing `appopener_test-1.0.tar` & `appopener_test-1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 14:45:58.938653 appopener_test-1.0/
--rw-rw-rw-   0        0        0     3850 2023-06-02 14:45:58.935663 appopener_test-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 14:45:58.760433 appopener_test-1.0/appopener_test/
--rw-rw-rw-   0        0        0      416 2023-06-02 14:43:30.000000 appopener_test-1.0/appopener_test/__init__.py
--rw-rw-rw-   0        0        0       62 2023-06-02 14:32:02.000000 appopener_test-1.0/appopener_test/__main__.py
--rw-rw-rw-   0        0        0     2596 2023-06-02 14:40:16.000000 appopener_test-1.0/appopener_test/check.py
--rw-rw-rw-   0        0        0      827 2023-06-02 14:32:02.000000 appopener_test-1.0/appopener_test/commands.py
--rw-rw-rw-   0        0        0     7421 2023-06-02 14:41:38.000000 appopener_test-1.0/appopener_test/update_list.py
-drwxrwxrwx   0        0        0        0 2023-06-02 14:45:58.932613 appopener_test-1.0/appopener_test.egg-info/
--rw-rw-rw-   0        0        0     3850 2023-06-02 14:45:58.000000 appopener_test-1.0/appopener_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-02 14:45:58.000000 appopener_test-1.0/appopener_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 14:45:58.000000 appopener_test-1.0/appopener_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 14:45:58.000000 appopener_test-1.0/appopener_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 14:45:58.000000 appopener_test-1.0/appopener_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 14:45:58.939650 appopener_test-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-02 14:35:00.000000 appopener_test-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:11:22.230567 appopener_test-1.1/
+-rw-rw-rw-   0        0        0     3850 2023-06-02 15:11:22.229499 appopener_test-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 15:11:22.209890 appopener_test-1.1/appopener_test/
+-rw-rw-rw-   0        0        0      416 2023-06-02 14:58:04.000000 appopener_test-1.1/appopener_test/__init__.py
+-rw-rw-rw-   0        0        0       62 2023-06-02 14:32:02.000000 appopener_test-1.1/appopener_test/__main__.py
+-rw-rw-rw-   0        0        0     2704 2023-06-02 15:10:34.000000 appopener_test-1.1/appopener_test/check.py
+-rw-rw-rw-   0        0        0      827 2023-06-02 14:32:02.000000 appopener_test-1.1/appopener_test/commands.py
+-rw-rw-rw-   0        0        0      534 2023-06-02 15:08:42.000000 appopener_test-1.1/appopener_test/old_style.py
+-rw-rw-rw-   0        0        0     7421 2023-06-02 14:41:38.000000 appopener_test-1.1/appopener_test/update_list.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:11:22.227049 appopener_test-1.1/appopener_test.egg-info/
+-rw-rw-rw-   0        0        0     3850 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 15:11:22.230567 appopener_test-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-02 14:35:00.000000 appopener_test-1.1/setup.py
```

### Comparing `appopener_test-1.0/PKG-INFO` & `appopener_test-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appopener_test
-Version: 1.0
+Version: 1.1
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `appopener_test-1.0/appopener_test/check.py` & `appopener_test-1.1/appopener_test/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os, json, re, sys, subprocess
 from . import update_list
+from . import old_style
 
 # check what os the library is running on
 def check_os():
     os_name = os.name
     if os_name != "nt":
         print("Exception error: AppOpener only works on windows.")
         exit()
@@ -44,28 +45,33 @@
 
 def create_file(print_text=True):
     if check_data == False:
         os.mkdir(main_path)
         # os.system(("attrib +h "+main_path))
     if print_text:
         print("LOADING APPS... (JUST ONCE)")
-    cmd = 'powershell -ExecutionPolicy Bypass "Get-StartApps|convertto-json"'
-    result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, encoding='utf-8')
-    apps = json.loads(result.stdout)
+    try:
+        cmd = 'powershell -ExecutionPolicy Bypass "Get-StartApps|convertto-json"'
+        result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, encoding='utf-8')
+        apps = json.loads(result.stdout)
+    except:
+        pass
+        apps = old_style.old_skool()
     names = {}
     for each in apps:
         names.update({each['Name'].lower():each['AppID']})
     with open((os.path.join(main_path,"data.json")),"w") as outfile:
         json.dump(names,outfile,indent = 4)
     setup_files()
 
 def check_json():
     if check_json_list == (False):
         create_file()
 
+
 # Make seperate file for appnames (to perform various features)
 def app_names():
     if check_app_names == (False):
         update_list.check_app_names()
     update_list.check_new_name()
     update_list.pre_change()
     update_list.modify()
```

### Comparing `appopener_test-1.0/appopener_test/commands.py` & `appopener_test-1.1/appopener_test/commands.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.0/appopener_test/update_list.py` & `appopener_test-1.1/appopener_test/update_list.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.0/appopener_test.egg-info/PKG-INFO` & `appopener_test-1.1/appopener_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appopener-test
-Version: 1.0
+Version: 1.1
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `appopener_test-1.0/setup.py` & `appopener_test-1.1/setup.py`

 * *Files identical despite different names*

