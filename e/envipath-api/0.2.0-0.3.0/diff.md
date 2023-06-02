# Comparing `tmp/envipath-api-0.2.0.tar.gz` & `tmp/envipath-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/envipath-api-0.2.0.tar", last modified: Fri Aug 28 20:51:32 2020, max compression
+gzip compressed data, was "envipath-api-0.3.0.tar", last modified: Fri Jun  2 09:32:53 2023, max compression
```

## Comparing `envipath-api-0.2.0.tar` & `envipath-api-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 me        (1000) me        (1000)        0 2020-08-28 20:51:32.000000 envipath-api-0.2.0/
-drwxrwxrwx   0 me        (1000) me        (1000)        0 2020-08-28 20:51:32.000000 envipath-api-0.2.0/envipath_api.egg-info/
--rwxrwxrwx   0 me        (1000) me        (1000)        1 2020-08-28 20:51:31.000000 envipath-api-0.2.0/envipath_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 me        (1000) me        (1000)        1 2020-02-24 17:15:26.000000 envipath-api-0.2.0/envipath_api.egg-info/not-zip-safe
--rwxrwxrwx   0 me        (1000) me        (1000)      263 2020-08-28 20:51:31.000000 envipath-api-0.2.0/envipath_api.egg-info/PKG-INFO
--rwxrwxrwx   0 me        (1000) me        (1000)       18 2020-08-28 20:51:31.000000 envipath-api-0.2.0/envipath_api.egg-info/requires.txt
--rwxrwxrwx   0 me        (1000) me        (1000)      253 2020-08-28 20:51:31.000000 envipath-api-0.2.0/envipath_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 me        (1000) me        (1000)        9 2020-08-28 20:51:31.000000 envipath-api-0.2.0/envipath_api.egg-info/top_level.txt
-drwxrwxrwx   0 me        (1000) me        (1000)        0 2020-08-28 20:51:32.000000 envipath-api-0.2.0/envirest/
--rwxrwxrwx   0 me        (1000) me        (1000)    42194 2020-08-28 16:05:02.000000 envipath-api-0.2.0/envirest/__init__.py
--rwxrwxrwx   0 me        (1000) me        (1000)      263 2020-08-28 20:51:32.000000 envipath-api-0.2.0/PKG-INFO
--rwxrwxrwx   0 me        (1000) me        (1000)       15 2020-01-23 17:12:49.000000 envipath-api-0.2.0/README.md
--rwxrwxrwx   0 me        (1000) me        (1000)       38 2020-08-28 20:51:32.000000 envipath-api-0.2.0/setup.cfg
--rwxrwxrwx   0 me        (1000) me        (1000)      386 2020-08-28 20:50:38.000000 envipath-api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:32:53.160146 envipath-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-02 09:32:12.000000 envipath-api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 09:32:53.160146 envipath-api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 09:32:12.000000 envipath-api-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:32:53.160146 envipath-api-0.3.0/envipath_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 09:32:53.000000 envipath-api-0.3.0/envipath_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-02 09:32:53.000000 envipath-api-0.3.0/envipath_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:32:53.000000 envipath-api-0.3.0/envipath_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:32:53.000000 envipath-api-0.3.0/envipath_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 09:32:53.000000 envipath-api-0.3.0/envipath_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 09:32:53.000000 envipath-api-0.3.0/envipath_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:32:53.160146 envipath-api-0.3.0/envirest/
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-06-02 09:32:12.000000 envipath-api-0.3.0/envirest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:32:53.160146 envipath-api-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-02 09:32:12.000000 envipath-api-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `envipath-api-0.2.0/envirest/__init__.py` & `envipath-api-0.3.0/envirest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import re
 from argparse import ArgumentParser
 
 from requests import Session
 from getpass import getpass
 
+
 DEFAULT_HOST = "envipath.org"
 ANONYMOUS = "anonymous"
 
 JSONHEADERS = {"Accept": "application/json"}
 TEXTHEADERS = {'Accept': 'text/plain'}
 
 
@@ -33,18 +34,18 @@
         logout(self.session, self.hosturl, verify=self.verify, secure=self.secure)
 
     def delete(self, url):
         if self.secure:
             url = url.replace("http://", "https://")
         r = self.session.delete(url, verify=self.verify)
         if r.status_code > 299:
-            raise Exception("Failed with status code {}, text:\n{}".format(r.status_code, r.text.decode()))
+            raise Exception("Failed with status code {}, text:\n{}".format(r.status_code, r.text))
 
-    def get(self, url):
-        return getjson(self.session, url, self.verify, secure=self.secure)
+    def get(self, url, timeout=None):
+        return getjson(self.session, url, self.verify, secure=self.secure, timeout=timeout)
 
     def post(self, url, data):
         return post(self.session, url, data, self.verify, secure=self.secure)
 
     def importpackage(self, jsonfile):
         importpackage(self.session, hosturl=self.hosturl, jsonfile=jsonfile,
                       verify=self.verify, secure=self.secure)
@@ -69,33 +70,38 @@
         return runRule(self.session, ruleurl=ruleurl, smiles=smiles,
                        verify=self.verify, secure=self.secure)
 
     def addscenario(self, objecturl, scenariourl):
         return addScenario(session=self.session, url=objecturl,
                            scenario=scenariourl, verify=self.verify, secure=self.secure)
 
-    def updatescenario(self, scenariourl,
+    def updatescenario(self, scenariourl, plainname=None, description=None, date=None,
                        soilsource=None, soiltexture1=None, soiltexture2=None,
                        soilclassificationsystem=None, redox=None, acidity=None, temperature=None,
                        waterstoragecapacity=None, humidity=None, omcontent=None, cec=None, bulkdens=None,
                        biomass=None, spikecompoundsmiles=None, spikeconcentration=None, halflife=None,
                        minormajor=None, proposedintermediate=None, confidencelevel=None,
-                       referringscenario=None, enzyme=None,
+                       referringscenario=None, enzyme=None, organism=None,
                        infotypes=[], infodata={}):
-        return updateScenario(self.session, scenario=scenariourl,
+        return updateScenario(self.session, scenario=scenariourl, plainname=plainname, description=description, date=date,
                               soilsource=soilsource, soiltexture1=soiltexture1, soiltexture2=soiltexture2,
                               soilclassificationsystem=soilclassificationsystem, redox=redox, acidity=acidity,
                               temperature=temperature, waterstoragecapacity=waterstoragecapacity, humidity=humidity,
                               omcontent=omcontent, cec=cec, bulkdens=bulkdens, biomass=biomass,
                               spikecompoundsmiles=spikecompoundsmiles, spikeconcentration=spikeconcentration,
                               halflife=halflife, minormajor=minormajor, proposedintermediate=proposedintermediate,
-                              confidencelevel=confidencelevel, referringscenario=referringscenario, enzyme=enzyme,
+                              confidencelevel=confidencelevel, referringscenario=referringscenario,
+                              enzyme=enzyme, organism=organism,
                               addInfoTypes=infotypes, addInfoInput=infodata,
                               verify=self.verify, secure=self.secure)
 
+    def removeAddInf(self, scenariourl, aiurl):
+        return remove_addinf(self.session, scenario_url=scenariourl, ai_url=aiurl,
+                             verify=self.verify, secure=self.secure)
+
     def createrule(self, packageurl,
             ruletype='SIMPLE',
             smirks=None,
             name=None,
             description=None,
             compositerule=None,
             simplerules=None,
@@ -197,15 +203,16 @@
             spikecompoundsmiles=None,
             spikeconcentration=None,
             halflife=None,
             minormajor=None,
             proposedintermediate=None,
             confidencelevel=None,
             referringscenario=None,
-            enzyme=None):
+            enzyme=None,
+            organism=None):
         return createScenario(self.session, packageurl,
             plainname=plainname,
             description=description,
             studydate=studydate,
             scenariotype=scenariotype,
             soilsource=soilsource,
             soiltexture1=soiltexture1,
@@ -224,14 +231,15 @@
             spikeconcentration=spikeconcentration,
             minormajor=minormajor,
             proposedintermediate=proposedintermediate,
             confidencelevel=confidencelevel,
             halflife=halflife,
             referringscenario=referringscenario,
             enzyme=enzyme,
+            organism=organism,
             verify=self.verify,
             secure=self.secure)
 
     def remove_ec_number(self, eclink_url):
         return remove_ec_number(self.session, eclink_url, verify=self.verify, secure=self.secure)
 
     def update_ec_number(self, eclink_url,
@@ -259,17 +267,17 @@
             name=name,
             linking_method=linking_method,
             evidence=evidence,
             description=description,
             verify=self.verify, secure=self.secure)
     
     def get_enviLink(self, package=None, rule=None):
-        if not package:
+        if package is None:
             package_url = self.findpackage('EAWAG-BBD')
-        elif package.starts_with(self.hosturl):
+        elif package.startswith(self.hosturl):
             package_url = package
         else:
             package_url = self.findpackage(package)
 
         rules = self.get('{}/rule'.format(package_url))['rule']
         if rule:
             rules = [r for r in rules if r['name'] == rule]
@@ -306,30 +314,32 @@
                     'linkingMethod': envi_link['linkingMethod'],
                     'evidence': evidence_name,
                     'evidence_link': evidence_link,
                 })
 
         return envi_links
 
+    def update_pathway(self, pathway_url, **kwargs):
+        return update_pathway(self.session, pathway_url, **kwargs)
+
 
 def login(hosturl, username, password, verify=True, secure=False):
     session = Session()
     data = {
         'hiddenMethod': 'login',
         'loginusername': username
     }
     if username != ANONYMOUS:
         data['loginpassword'] = (password or getpass())
 
     if secure:
         hosturl = hosturl.replace("http://", "https://")
 
-    response = session.post(hosturl, data=data, headers=TEXTHEADERS, allow_redirects=True,
+    session.post(hosturl, data=data, headers=TEXTHEADERS, allow_redirects=True,
                             verify=verify)
-    #print(response)
     return session
 
 
 # does not seem to have any effect
 # probably all wrong
 def logout(session, hosturl, verify=True, secure=False):
     data = {
@@ -366,24 +376,24 @@
     parser.add_argument('--package', dest='package', action='store', default=ANONYMOUS,
                         help='package name')
     parser.add_argument('--name', dest='name', action='store',
                         help='object name')
     return parser
 
 
-def getjson(session, url, verify=True, secure=False):
+def getjson(session, url, verify=True, secure=False, timeout=None):
     if secure:
         url = url.replace("http://", "https://")
     r = session.get(url, headers=JSONHEADERS, allow_redirects=True,
-                    verify=verify)
+                    verify=verify, timeout=timeout)
     return r.json()
 
 
-def get(session, url, verify=True, secure=False):
-    return getjson(session=session, url=url, verify=verify, secure=secure)
+def get(session, url, verify=True, secure=False, timeout=None):
+    return getjson(session=session, url=url, verify=verify, secure=secure, timeout=timeout)
 
 
 def post(session, url, data, verify=True, secure=False):
     if secure:
         url = url.replace("http://", "https://")
     r = session.post(url, data=data, headers=JSONHEADERS, allow_redirects=True,
                      verify=verify)
@@ -395,15 +405,14 @@
         url = object.replace("http://", "https://")
     else:
         url = object
     data = {"name": newname, "defaultName": "defaultName"}
     r = session.post(url, data=data, headers=JSONHEADERS, allow_redirects=True,
                      verify=verify)
     if r.json().get("name") != newname:
-        print(r.json())
         raise Exception("renaming to {} failed for {}".format(newname, object))
 
 
 def importpackage(session, hosturl, jsonfile, verify=True, secure=False):
     url = "{}/package".format(hosturl)
     if secure:
         url = url.replace("http://", "https://")
@@ -436,24 +445,35 @@
     if secure:
         ruleurl = ruleurl.replace("http://", "https://")
     r = session.post(ruleurl, data=data, headers=JSONHEADERS,
                      verify=verify)
     return r.content.decode().strip().split("\n")
 
 
-def updateScenario(session, scenario, soilsource=None, soiltexture1=None, soiltexture2=None,
+def updateScenario(session, scenario, plainname=None, description=None, date=None,
+        soilsource=None, soiltexture1=None, soiltexture2=None,
         soilclassificationsystem=None, redox=None, acidity=None, temperature=None,
         waterstoragecapacity=None, humidity=None, omcontent=None, cec=None, bulkdens=None,
         biomass=None, spikecompoundsmiles=None, spikeconcentration=None, halflife=None,
-        minormajor=None, proposedintermediate=None, confidencelevel=None, referringscenario=None, enzyme=None,
+        minormajor=None, proposedintermediate=None, confidencelevel=None, referringscenario=None,
+        enzyme=None, organism=None,
         addInfoTypes=[], addInfoInput={}, verify=True, secure=False):
     url = scenario
     if secure:
         url = url.replace("http://", "https://")
-    data = {"updateScenario": "true"}
+   
+    (year, month, day) = date.split('-') if date else (None, None, None)
+    data = {
+        "updateScenario": "true",
+        "scenarioName": plainname,
+        "scenarioDescription": description,
+        "dateYear": year,
+        "dateMonth": month,
+        "dateDay": day,
+    }
     addinfos = collectData(data,
         soilsource=soilsource,
         soiltexture1=soiltexture1,
         soiltexture2=soiltexture2,
         soilclassificationsystem=soilclassificationsystem,
         redox=redox,
         acidity=acidity,
@@ -467,15 +487,16 @@
         spikecompoundsmiles=spikecompoundsmiles,
         spikeconcentration=spikeconcentration,
         halflife=halflife,
         minormajor=minormajor,
         proposedintermediate=proposedintermediate,
         confidencelevel=confidencelevel,
         referringscenario=referringscenario,
-        enzyme=enzyme)
+        enzyme=enzyme,
+        organism=organism)
     for k,v in addInfoInput.items():
         data[k] = v
     if addinfos:
         data['adInfoTypes[]'] = ",".join(addinfos+addInfoTypes)
 
     r = session.post(url, data=data, headers=JSONHEADERS, allow_redirects=True,
                      verify=verify)
@@ -577,26 +598,30 @@
         halflife=None,
         minormajor=None,
         proposedintermediate=None,
         confidencelevel=None,
         referringscenario=None,
 
         enzyme=None,
+        organism=None,
 
         verify=True,
         secure=False):
 
     url = package+"/scenario"
     if secure:
         url = url.replace("http://", "https://")
+    year, month, day = studydate.split("-")
     data = {
         #scenario
         'studyname': plainname,
         'studydescription': description,
-        'date': studydate,
+        'dateYear': year,
+        'dateMonth': month,
+        'dateDay': day,
         'type': scenariotype,
     }
     addinfos = collectData(data=data,
         soilsource=soilsource,
         soiltexture1=soiltexture1,
         soiltexture2=soiltexture2,
         soilclassificationsystem=soilclassificationsystem,
@@ -612,15 +637,16 @@
         spikecompoundsmiles=spikecompoundsmiles,
         spikeconcentration=spikeconcentration,
         halflife=halflife,
         minormajor=minormajor,
         proposedintermediate=proposedintermediate,
         confidencelevel=confidencelevel,
         referringscenario=referringscenario,
-        enzyme=enzyme)
+        enzyme=enzyme,
+        organism=organism)
 
     # count the blessings
     if addinfos:
         data['adInfoTypes[]'] = ",".join(addinfos)
         # not sure about this one.
         # may this be the source of the referring scenario trouble?
         data['fullScenario'] = 'true'
@@ -648,15 +674,16 @@
         spikecompoundsmiles=None,
         spikeconcentration=None,
         halflife=None,
         minormajor=None,
         proposedintermediate=None,
         confidencelevel=None,
         referringscenario=None,
-        enzyme=None):
+        enzyme=None,
+        organism=None):
 
     addinfos = []
 
     # SOIL scenario
     if soilsource:
         addinfos.append('soilsource')
         data['soilsourcedata'] = soilsource
@@ -786,14 +813,18 @@
         data['referringscenario'] = referringscenario
 
     if not blankMap(enzyme):
         addinfos.append('enzyme')
         data['enzymeName'] = enzyme['name']
         data['enzymeECNumber'] = enzyme['ECNumber']
 
+    if organism:
+        addinfos.append('initorganism')
+        data['organism'] = organism
+
     return addinfos
 
 
 RULEURLSUFFIX = {'SIMPLE': 'rule',
                  'PARALLEL': 'parallel-rule',
                  'SEQUENTIAL': 'sequential-rule'}
 def createRule(session, packageurl, ruletype='SIMPLE',
@@ -942,15 +973,15 @@
                 break
         except Exception as ke:
             from sys import stderr
             stderr.write("ERROR: couldnt get completeness ({0}) on {1}\n".format(ke.__class__.__name__, pwurl))
             break
         import time
         time.sleep(5.0)
-        pw = getjson(session, pwurl, verify=verify, secure=secure)
+        pw = getjson(session, pwurl, verify=verify, secure=secure, timeout=None)
 
     return pw
 
 
 def addCompoundToPathway(session, pathwayurl, smiles, verify=True, secure=False):
     return createEntity(session, pathwayurl, 'node', properties={'nodeAsSmiles': smiles},
                         secure=secure, verify=verify, headers={"Accept": "application/json", "referer": pathwayurl})
@@ -1084,18 +1115,39 @@
     if edges:
         mut_data['edge'] = ';'.join(edges)
     if general:
         mut_data['evidence'] = ';'.join(general)
 
 
 def remove_ec_number(session, eclink_url, verify=True, secure=False):
+    pieces = eclink_url.split('/')
+    try:
+        assert len(pieces) == 9
+        assert pieces[7] == 'enzymelink'
+        assert pieces[5] in ['parallel-rule', 'sequential-rule', 'simple-rule']
+    except AssertionError:
+        raise ValueError("{} is not part of enviLink".format(eclink_url))
+
     if secure: eclink_url = eclink_url.replace("http://", "https://")
     session.delete(eclink_url, headers=JSONHEADERS, verify=verify)
 
 
+def remove_addinf(session, scenario_url, ai_url, verify=True, secure=False):
+    data={
+        'hidden': 'delete', 
+        'aiUri': ai_url,
+    }
+    if secure: scenario_url = scenario_url.replace("http://", "https://")
+    r = session.post(scenario_url, headers=JSONHEADERS, data=data, verify=verify)
+    if r.status_code < 300:
+        return r.json()
+    else:
+        raise Exception("Failed with status code {}, text:\n{}".format(r.status_code, r.text))
+
+
 def updateReaction(session, reaction_url,
         name=None,
         alias=None,
         description=None,
         related_rule=None,
         smirks=None,
         scenario=None,
@@ -1134,7 +1186,34 @@
     if description: data['description'] = description
     if related_rules: data['rules'] = related_rules
     if smirks: data['smirks'] = smirks
     if scenario: data['scenario'] = scenario
 
     response = session.post("{}/reaction".format(package_url), data=data, headers=JSONHEADERS, verify=verify)
     return respond_or_raise(response)
+
+
+def url_format(text):
+    return text\
+        .replace("\n", '<br>')\
+        .encode('UTF-8')
+
+
+def update_pathway(session, pathway_url, description=None, name=None, **kwargs):
+    headers = JSONHEADERS.copy()
+    headers["referer"] = pathway_url
+    
+    params = kwargs
+    
+    if description:
+        params['pathwayDescription'] = url_format(description)
+
+    if name:
+        params['pathwayName'] = url_format(name)
+
+    r = session.post(pathway_url, params=params,
+        headers=headers, allow_redirects=True, verify=False)
+
+    if r.status_code == 200:
+        return r.json()
+    else:
+        raise Exception(r.content.decode())
```

