# Comparing `tmp/kalm-0.6.0.tar.gz` & `tmp/kalm-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.6.0.tar", max compression
+gzip compressed data, was "kalm-0.6.1.tar", max compression
```

## Comparing `kalm-0.6.0.tar` & `kalm-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1878 2023-05-24 10:01:37.819325 kalm-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.6.0/src/kalm/__init__.py
--rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.0/src/kalm/jenkins.py
--rw-r--r--   0        0        0    32279 2023-05-09 12:32:33.321460 kalm-0.6.0/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.0/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.0/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.0/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     1878 2023-06-02 09:46:22.328227 kalm-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-09 13:19:17.365700 kalm-0.6.1/src/kalm/jenkins.py
+-rw-r--r--   0        0        0    32229 2023-06-02 09:23:56.840187 kalm-0.6.1/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.6.1/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.6.1/PKG-INFO
```

### Comparing `kalm-0.6.0/LICENSE.txt` & `kalm-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.6.0/pyproject.toml` & `kalm-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.6.0"
+version = "0.6.1"
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
-version = "0.6.0" 
+version = "0.6.1" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.6.0/src/kalm/__init__.py` & `kalm-0.6.1/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.0/src/kalm/kalm.py` & `kalm-0.6.1/src/kalm/kalm.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         try:
             invid = (awx_get_id("inventories", name, r))
         except:
             print("Unexpected error")
         if (invid != "" ):
           loop = False
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
-  url ="https://ansible.openknowit.com/api/v2/inventories/%s/variable_data/" % invid
+  url = os.getenv("TOWER_HOST") + "/api/v2/inventories/%s/" % invid
   resp = requests.put(url,headers=headers, json=variables)
   response = json.loads(resp.content)
   if (inventorytype == "netbox"):
     print("Create hosts in netbox")
     nbtoken = os.getenv("NBTOKEN")
     nburl = os.getenv("NBURL")
     nb = pynetbox.api(nburl, token=nbtoken)
@@ -193,15 +193,15 @@
   data = {
         "name": name,
         "description": description,
         "organization": orgid,
         "inventory": invid
        }
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
-  url ="https://ansible.openknowit.com/api/v2/hosts/"
+  url = os.getenv("TOWER_HOST") + "/api/v2/hosts/"
   resp = requests.post(url,headers=headers, json=data)
   response = json.loads(resp.content)
   try:
     hostid=response['id']
     prettyllog("manage", "host", name, organization, resp.status_code, "Host %s created with id: %s" % (name, hostid ))
   except:
     prettyllog("manage", "host", name, organization, resp.status_code, response)
@@ -274,30 +274,30 @@
   if (orgid == ""):
     headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
     data = {
           "name": name,
           "description": description,
           "max_hosts": max_hosts
          }
-    url ="https://ansible.openknowit.com/api/v2/organizations/"
+    url = os.getenv("TOWER_HOST") + "/api/v2/organizations/"
     resp = requests.post(url,headers=headers, json=data)
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
-    url ="https://ansible.openknowit.com/api/v2/organizations/%s" % orgid
+    url = os.getenv("TOWER_HOST") + "/api/v2/organizations/%s" % orgid
     resp = requests.put(url,headers=headers, json=data)
     response = json.loads(resp.content)
     prettyllog("manage", "organization", name, realm, resp.status_code, response)
   getawxdata("organizations", mytoken, r)
 
 
 ############################################################################################################################
@@ -311,16 +311,15 @@
       "name": name,
       "unified_job_template": unified_job_template,
       "description": description,
       "local_time_zone": tz,
       "dtstart": start['year'] + "-" + start['month'] + "-" + start['day'] + "T" + start['hour'] + ":" + start['minute'] + ":" + start['second']  + "Z",
       "rrule": "DTSTART;TZID=" + tz + ":" + start['year'] + start['month'] + start['day'] + "T" + start['hour'] + start['minute'] + start['second'] +" RRULE:INTERVAL=" + run_frequency + ";FREQ=" + run_every
     }
-
-  url ="https://ansible.openknowit.com/api/v2/schedules/"
+  url = os.getenv("TOWER_HOST") + "/api/v2/schedules/"
   resp = requests.post(url,headers=headers, json=data)
   response = json.loads(resp.content)
   try:
     schedid=response['id']
     prettyllog("manage", "schedule", name, organization, resp.status_code, schedid)
   except:
     prettyllog("manage", "schedule", name, organization, resp.status_code, response)
@@ -369,21 +368,21 @@
     "survey_enabled": "false",
     "become_enabled": "false",
     "diff_mode": "false",
     "allow_simultaneous": "false",
     "job_slice_count": 1
 }
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
-  url = "https://ansible.openknowit.com/api/v2/job_templates/"
+  url = os.getenv("TOWER_HOST") + "/api/v2/job_templates/"
   resp = requests.post(url,headers=headers, json=data)
   response = json.loads(resp.content)
   getawxdata("job_templates", mytoken, r)
   tmplid = awx_get_id("job_templates", name, r )
   if ( tmplid != "" ):
-    url = "https://ansible.openknowit.com/api/v2/job_templates/%s/" % tmplid
+    url = os.getenv("TOWER_HOST") + "/api/v2/job_templates/%s/" % tmplid
     resp = requests.put(url,headers=headers, json=data)
     response = json.loads(resp.content)
     try:
       tmplid=response['id']
       prettyllog("update", "template", name, organization, resp.status_code, tmplid)
     except:
       prettyllog("update", "template", name, organization, resp.status_code, response)
@@ -496,24 +495,24 @@
             "become_username": credential['privilege_escalation_username'],
             "become_password": credential['privilege_escalation_password']
           },
         "kind": credential['kind']
         }
 
   if ( credid == ""):
-    url = "https://ansible.openknowit.com/api/v2/credentials/"
+    url = os.getenv("TOWER_HOST") + "/api/v2/credentials/"
     resp = requests.post(url,headers=headers, json=data)
     response = json.loads(resp.content)
     try:
       credid=response['id']
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, credid)
     except:
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, response)
   else:
-    url = "https://ansible.openknowit.com/api/v2/credentials/%s/" % credid
+    url = os.getenv("TOWER_HOST") + "/api/v2/credentials/%s/" % credid
     resp = requests.put(url,headers=headers, json=data)
     response = json.loads(resp.content)
     try:
       credid=response['id']
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, credid)
     except:
       prettyllog("manage", "credential", credential['name'], organization, resp.status_code, response)
@@ -521,25 +520,25 @@
 
 
 ######################################
 # function: get  organization
 ######################################
 def awx_get_organization(orgid, mytoken, r):
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
-  url ="https://ansible.openknowit.com/api/v2/organizations/%s" % orgid
+  url = os.getenv("TOWER_HOST") + "/api/v2/organizations/%s" % orgid
   resp = requests.get(url,headers=headers)
   return   json.loads(resp.content)
 
 ######################################
 # function: get Project 
 ######################################
 def awx_get_project(projid, organization, mytoken, r):
   headers = {"User-agent": "python-awx-client", "Content-Type": "application/json","Authorization": "Bearer {}".format(mytoken)}
   orgid = (awx_get_id("organizations", organization, r))
-  url ="https://ansible.openknowit.com/api/v2/projects/%s" % projid
+  url = os.getenv("TOWER_HOST") + "/api/v2/projects/%s" % projid
   resp = requests.get(url,headers=headers)
   return   json.loads(resp.content)
 
 
 
 ######################################
 # function: Create Project 
@@ -559,15 +558,15 @@
         "scm_type": scm_type,
         "scm_url": scm_url,
         "organization": orgid,
         "scm_branch": scm_branch,
         "credential": credid
        }
   if (projid == ""):
-    url ="https://ansible.openknowit.com/api/v2/projects/"
+    url = os.getenv("TOWER_HOST") + "/api/v2/projects/"
     resp = requests.post(url,headers=headers, json=data)
     response = json.loads(resp.content)
     try:
       projid=response['id']
       prettyllog("manage", "project", name, organization, resp.status_code, projid)
     except:
       prettyllog("manage", "project", name, organization, resp.status_code, response)
@@ -583,15 +582,15 @@
         try:
           if( projectinfo['status'] == "successful"):
               loop = False
         except:
           print("Project status unknown")
 
   else:
-    url ="https://ansible.openknowit.com/api/v2/projects/%s/" % projid
+    url = os.getenv("TOWER_HOST") + "/api/v2/projects/%s/" % projid
     resp = requests.put(url,headers=headers, json=data)
     response = json.loads(resp.content)
     try:  
       projid = (awx_get_id("projects", name,r ))
       prettyllog("manage", "project", name, organization, resp.status_code, projid)
     except:
       prettyllog("manage", "project", name, organization, resp.status_code, response)
@@ -658,15 +657,15 @@
 
   ########################################################################################################################
   # organizations
   ########################################################################################################################
   for org in (config['organization']):
     prettyllog("loop","org", "config", org['name'], "000", "create organization")
     orgname = org['name']
-    key = "ansible.openknowit.com:organizations:orphan:" + orgname
+    key = os.getenv("TOWER_HOST") + ":organizations:name:" + orgname
     r.delete(key)
     max_hosts = org['meta']['max_hosts']
     default_environment = org['meta']['default_environment']
     description = org['meta']['description']
     awx_create_organization(orgname, description, max_hosts, default_environment, realm, mytoken, r)
     getawxdata("organizations", mytoken, r)
     orgid = awx_get_id("organizations", orgname, r)
@@ -681,15 +680,15 @@
 
     ######################################
     # Credentials   
     ######################################
     #try:
      # credentials = org['credentials']
      # for credential in credentials:
-      #  key = "ansible.openknowit.com:credentials:orphan:" + credential['name']
+      #  key = os.getenv("TOWER_HOST") +":credentials:orphan:" + credential['name']
     #   r.delete(key)
       #awx_create_credential( credential, orgname)
       #loop = True
       #while (loop):
       #  credid = awx_get_id("credentials", credential['name'])
       #  if ( credid != "" ):
       #    loop = False
@@ -704,15 +703,15 @@
       for project in projects:
         projectname = project['name']
         projectdesc = project['description']
         projecttype = project['scm_type']
         projecturl  = project['scm_url']
         projectbrnc = project['scm_branch']
         projectcred = project['credential']
-        key = "ansible.openknowit.com:projects:orphan:" + projectname
+        key = os.getenv("TOWER_HOST") +":projects:orphan:" + projectname
         r.delete(key)
         awx_create_project(projectname, projectdesc, projecttype, projecturl, projectbrnc, projectcred, orgname, mytoken, r)
         awx_get_id("projects", projectname, r)
         projid = (awx_get_id("projects", projectname, r))
     except:
       prettyllog("config", "initialize", "projects", orgname, "000",  "No projects found")
```

### Comparing `kalm-0.6.0/src/kalm/netbox.py` & `kalm-0.6.1/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.6.0/PKG-INFO` & `kalm-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.6.0
+Version: 0.6.1
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

