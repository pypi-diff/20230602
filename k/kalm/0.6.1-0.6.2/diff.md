# Comparing `tmp/kalm-0.6.1.tar.gz` & `tmp/kalm-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.6.1.tar", max compression
+gzip compressed data, was "kalm-0.6.2.tar", max compression
```

## Comparing `kalm-0.6.1.tar` & `kalm-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     1878 2023-06-02 09:46:22.328227 kalm-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/__init__.py
--rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.1/src/kalm/jenkins.py
--rw-r--r--   0        0        0    32229 2023-06-02 09:23:56.840187 kalm-0.6.1/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.2/LICENSE.txt
+-rw-r--r--   0        0        0     1878 2023-06-02 10:22:47.576992 kalm-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.2/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    32790 2023-06-02 10:22:47.576992 kalm-0.6.2/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.2/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.2/PKG-INFO
```

### Comparing `kalm-0.6.1/LICENSE.txt` & `kalm-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.6.1/pyproject.toml` & `kalm-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.6.1"
+version = "0.6.2"
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
-version = "0.6.1" 
+version = "0.6.2" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.6.1/src/kalm/__init__.py` & `kalm-0.6.2/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.1/src/kalm/kalm.py` & `kalm-0.6.2/src/kalm/kalm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import hvac
 import os
 import sys
 import datetime
 import pynetbox
 import datetime
 
+VERIFY_SSL = os.getenv("VERIFY_SSL", "false")
+if VERIFY_SSL == "false" or VERIFY_SSL == "False" or VERIFY_SSL == "FALSE" or VERIFY_SSL == "no" or VERIFY_SSL == "NO" or VERIFY_SSL == "No":
+  VERIFY_SSL = False
+else:
+  VERIFY_SSL = True
+
+
 def prettyllog(function, action, item, organization, statuscode, text):
   d_date = datetime.datetime.now()
   reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
   print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
 
   
 
@@ -67,15 +74,15 @@
 
 def getawxdata(item, mytoken, r):
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   url = os.getenv("TOWER_HOST") + "/api/v2/" + item
   intheloop = "first"
   while ( intheloop == "first" or intheloop != "out" ):
     try:
-      resp = requests.get(url,headers=headers)
+      resp = requests.get(url,headers=headers, verify=VERIFY_SSL)
     except:
       intheloop = "out"
     try:
       mydata = json.loads(resp.content)
     except:
       intheloop = "out"
     try:
@@ -113,15 +120,15 @@
 
   
 
 def awx_delete(item, name, mytoken, r):
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   itemid = (awx_get_id(item, name, r))
   url = os.getenv("TOWER_HOST") + "/api/v2/" + item + "/" + itemid
-  resp = requests.delete(url,headers=headers)
+  resp = requests.delete(url,headers=headers, verify=VERIFY_SSL)
 
 def awx_purge_orphans():
   orphans = r.keys("*:orphan:*")
   for orphan in orphans:
     mykey = orphan.decode().split(":")
     awx_delete(mykey[1],mykey[3])
 
@@ -130,15 +137,15 @@
   if ( orgid != "" ):
     data = {
        "name": name,
        "organization": orgid
        }
     headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
     url = os.getenv("TOWER_HOST") + "/api/v2/labels"
-    resp = requests.post(url,headers=headers, json=data)
+    resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
       
 
 
 def awx_create_inventory(name, description, organization, inventorytype, variables, mytoken, r):
   try:  
     invid = (awx_get_id("inventories", name, r))
   except:
@@ -149,30 +156,30 @@
           "name": name,
           "description": description,
           "inventorytype": inventorytype,
           "organization": orgid
          }
     headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
     url = os.getenv("TOWER_HOST") + "/api/v2/inventories/"
-    resp = requests.post(url,headers=headers, json=data)
+    resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     prettyllog("manage", "inventories", name, organization, resp.status_code, response)
     loop = True
     while ( loop ):
         print("looop")
         getawxdata("inventories", mytoken, r)
         try:
             invid = (awx_get_id("inventories", name, r))
         except:
             print("Unexpected error")
         if (invid != "" ):
           loop = False
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   url = os.getenv("TOWER_HOST") + "/api/v2/inventories/%s/" % invid
-  resp = requests.put(url,headers=headers, json=variables)
+  resp = requests.put(url,headers=headers, json=variables, verify=VERIFY_SSL)
   response = json.loads(resp.content)
   if (inventorytype == "netbox"):
     print("Create hosts in netbox")
     nbtoken = os.getenv("NBTOKEN")
     nburl = os.getenv("NBURL")
     nb = pynetbox.api(nburl, token=nbtoken)
     ipaddresses = nb.ipam.ip_addresses.all()
@@ -194,15 +201,15 @@
         "name": name,
         "description": description,
         "organization": orgid,
         "inventory": invid
        }
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   url = os.getenv("TOWER_HOST") + "/api/v2/hosts/"
-  resp = requests.post(url,headers=headers, json=data)
+  resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
   response = json.loads(resp.content)
   try:
     hostid=response['id']
     prettyllog("manage", "host", name, organization, resp.status_code, "Host %s created with id: %s" % (name, hostid ))
   except:
     prettyllog("manage", "host", name, organization, resp.status_code, response)
 
@@ -275,30 +282,30 @@
     headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
     data = {
           "name": name,
           "description": description,
           "max_hosts": max_hosts
          }
     url = os.getenv("TOWER_HOST") + "/api/v2/organizations/"
-    resp = requests.post(url,headers=headers, json=data)
+    resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     try:
       orgid=response['id']
       prettyllog("manage", "organization", name, realm, resp.status_code, "organization %s created with id %s" % (orgid))
     except:
       prettyllog("manage", "organization", name, realm, resp.status_code, response)
   else:    
     headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
     data = {
           "name": name,
           "description": description,
           "max_hosts": max_hosts
          }
     url = os.getenv("TOWER_HOST") + "/api/v2/organizations/%s" % orgid
-    resp = requests.put(url,headers=headers, json=data)
+    resp = requests.put(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     prettyllog("manage", "organization", name, realm, resp.status_code, response)
   getawxdata("organizations", mytoken, r)
 
 
 ############################################################################################################################
 # Create job schedule
@@ -312,15 +319,15 @@
       "unified_job_template": unified_job_template,
       "description": description,
       "local_time_zone": tz,
       "dtstart": start['year'] + "-" + start['month'] + "-" + start['day'] + "T" + start['hour'] + ":" + start['minute'] + ":" + start['second']  + "Z",
       "rrule": "DTSTART;TZID=" + tz + ":" + start['year'] + start['month'] + start['day'] + "T" + start['hour'] + start['minute'] + start['second'] +" RRULE:INTERVAL=" + run_frequency + ";FREQ=" + run_every
     }
   url = os.getenv("TOWER_HOST") + "/api/v2/schedules/"
-  resp = requests.post(url,headers=headers, json=data)
+  resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
   response = json.loads(resp.content)
   try:
     schedid=response['id']
     prettyllog("manage", "schedule", name, organization, resp.status_code, schedid)
   except:
     prettyllog("manage", "schedule", name, organization, resp.status_code, response)
 
@@ -369,21 +376,21 @@
     "become_enabled": "false",
     "diff_mode": "false",
     "allow_simultaneous": "false",
     "job_slice_count": 1
 }
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   url = os.getenv("TOWER_HOST") + "/api/v2/job_templates/"
-  resp = requests.post(url,headers=headers, json=data)
+  resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
   response = json.loads(resp.content)
   getawxdata("job_templates", mytoken, r)
   tmplid = awx_get_id("job_templates", name, r )
   if ( tmplid != "" ):
     url = os.getenv("TOWER_HOST") + "/api/v2/job_templates/%s/" % tmplid
-    resp = requests.put(url,headers=headers, json=data)
+    resp = requests.put(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     try:
       tmplid=response['id']
       prettyllog("update", "template", name, organization, resp.status_code, tmplid)
     except:
       prettyllog("update", "template", name, organization, resp.status_code, response)
   getawxdata("job_templates", mytoken, r)
@@ -496,24 +503,24 @@
             "become_password": credential['privilege_escalation_password']
           },
         "kind": credential['kind']
         }
 
   if ( credid == ""):
     url = os.getenv("TOWER_HOST") + "/api/v2/credentials/"
-    resp = requests.post(url,headers=headers, json=data)
+    resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     try:
       credid=response['id']
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, credid)
     except:
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, response)
   else:
     url = os.getenv("TOWER_HOST") + "/api/v2/credentials/%s/" % credid
-    resp = requests.put(url,headers=headers, json=data)
+    resp = requests.put(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     try:
       credid=response['id']
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, credid)
     except:
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, response)
   getawxdata("credentials", mytoken, r)
@@ -521,25 +528,25 @@
 
 ######################################
 # function: get  organization
 ######################################
 def awx_get_organization(orgid, mytoken, r):
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   url = os.getenv("TOWER_HOST") + "/api/v2/organizations/%s" % orgid
-  resp = requests.get(url,headers=headers)
+  resp = requests.get(url,headers=headers, verify=VERIFY_SSL)
   return   json.loads(resp.content)
 
 ######################################
 # function: get Project 
 ######################################
 def awx_get_project(projid, organization, mytoken, r):
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   orgid = (awx_get_id("organizations", organization, r))
   url = os.getenv("TOWER_HOST") + "/api/v2/projects/%s" % projid
-  resp = requests.get(url,headers=headers)
+  resp = requests.get(url,headers=headers,  verify=VERIFY_SSL)
   return   json.loads(resp.content)
 
 
 
 ######################################
 # function: Create Project 
 ######################################
@@ -559,15 +566,15 @@
         "scm_url": scm_url,
         "organization": orgid,
         "scm_branch": scm_branch,
         "credential": credid
        }
   if (projid == ""):
     url = os.getenv("TOWER_HOST") + "/api/v2/projects/"
-    resp = requests.post(url,headers=headers, json=data)
+    resp = requests.post(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     try:
       projid=response['id']
       prettyllog("manage", "project", name, organization, resp.status_code, projid)
     except:
       prettyllog("manage", "project", name, organization, resp.status_code, response)
     #loop until project is synced
@@ -583,15 +590,15 @@
           if( projectinfo['status'] == "successful"):
               loop = False
         except:
           print("Project status unknown")
 
   else:
     url = os.getenv("TOWER_HOST") + "/api/v2/projects/%s/" % projid
-    resp = requests.put(url,headers=headers, json=data)
+    resp = requests.put(url,headers=headers, json=data, verify=VERIFY_SSL)
     response = json.loads(resp.content)
     try:  
       projid = (awx_get_id("projects", name,r ))
       prettyllog("manage", "project", name, organization, resp.status_code, projid)
     except:
       prettyllog("manage", "project", name, organization, resp.status_code, response)
     getawxdata("projects", mytoken, r)
```

### Comparing `kalm-0.6.1/src/kalm/netbox.py` & `kalm-0.6.2/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.1/PKG-INFO` & `kalm-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.6.1
+Version: 0.6.2
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

