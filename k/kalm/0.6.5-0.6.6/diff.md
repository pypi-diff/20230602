# Comparing `tmp/kalm-0.6.5.tar.gz` & `tmp/kalm-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.6.5.tar", max compression
+gzip compressed data, was "kalm-0.6.6.tar", max compression
```

## Comparing `kalm-0.6.5.tar` & `kalm-0.6.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.5/LICENSE.txt
--rw-r--r--   0        0        0     1910 2023-06-02 11:01:34.750614 kalm-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    10461 2023-06-02 10:48:49.438130 kalm-0.6.5/src/kalm/__init__.py
--rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.5/src/kalm/jenkins.py
--rw-r--r--   0        0        0    32889 2023-06-02 11:00:00.282060 kalm-0.6.5/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.5/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.5/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.5/src/kalm/toolbox.py
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 kalm-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.6/LICENSE.txt
+-rw-r--r--   0        0        0     1910 2023-06-02 11:41:44.716727 kalm-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    10461 2023-06-02 10:48:49.438130 kalm-0.6.6/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.6/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    33245 2023-06-02 11:41:44.716727 kalm-0.6.6/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.6/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.6/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.6/src/kalm/toolbox.py
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 kalm-0.6.6/PKG-INFO
```

### Comparing `kalm-0.6.5/LICENSE.txt` & `kalm-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.6.5/pyproject.toml` & `kalm-0.6.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.6.5"
+version = "0.6.6"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
@@ -25,15 +25,15 @@
 python-jenkins = "^1.7.0"
 urllib3 = "^2.0.2"
 
 
 
 [project]
 name = "kalm"  
-version = "0.6.5" 
+version = "0.6.6" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.6.5/src/kalm/__init__.py` & `kalm-0.6.6/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.5/src/kalm/kalm.py` & `kalm-0.6.6/src/kalm/kalm.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,15 +398,19 @@
       prettyllog("update", "template", name, organization, resp.status_code, response)
   getawxdata("job_templates", mytoken, r)
   tmplid = awx_get_id("job_templates", name ,r )
   getawxdata("credentials", mytoken, r)
   credid = (awx_get_id("credentials", credential, r))
   print('associatecommand = "awx job_template associate %s --credential %s >/dev/null 2>/dev/null " % ( tmplid, credid)')
   print("We should not use any awx cli commands, but the API is not consisten and sometimes fails to set the credentials")
-  associatecommand = "/usr/local/bin/awx job_template associate %s --credential %s >/dev/null 2>/dev/null " % ( tmplid, credid)
+  if TLSVERIFY == False:
+    associatecommand = "/usr/local/bin/awx job_template associate %s --credential %s -k >/dev/null 2>/dev/null " % ( tmplid, credid)  
+  else:
+    associatecommand = "/usr/local/bin/awx job_template associate %s --credential %s >/dev/null 2>/dev/null " % ( tmplid, credid)
+    
   print(associatecommand)
   os.system(associatecommand)
   ############################################################################### end of create job template ##########################################
 
 
 ######################################
 # function:  Create Team
@@ -793,28 +797,31 @@
         awx_create_label(labelname, orgname, mytoken, r)
     except:
       prettyllog("config", "initialize", "labels", orgname, "000",  "No labels found")
 
     ######################################
     # Templates
     ######################################
+    print("Templates")
+    print("============================DEBUG==============================YY")
     try:
       templates = org['templates']
       for template in templates:
         templatename = template['name']
         templatedescription = template['description']
         templatejob_type = template['job_type']
         templateinventory =  template['inventory']
         templateproject = template['project']
         templateEE = template['EE']
         templatecredential = template['credentials']  
         templateplaybook = template['playbook']
         awx_create_template(templatename, templatedescription, templatejob_type, templateinventory, templateproject, templateEE, templatecredential, templateplaybook, orgname, mytoken, r)
     except:
       prettyllog("config", "initialize", "templates", orgname, "000",  "No templates found")
+    print("============================DEBUG==============================YY")
 
     ######################################
     # Schedules
     ######################################
     try:
       schedules = org['schedules']
       for schedule in schedules:
```

### Comparing `kalm-0.6.5/src/kalm/netbox.py` & `kalm-0.6.6/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.5/PKG-INFO` & `kalm-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.6.5
+Version: 0.6.6
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

