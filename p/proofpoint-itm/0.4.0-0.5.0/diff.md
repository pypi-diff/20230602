# Comparing `tmp/proofpoint_itm-0.4.0.tar.gz` & `tmp/proofpoint_itm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proofpoint_itm-0.4.0.tar", last modified: Wed May 17 01:46:14 2023, max compression
+gzip compressed data, was "proofpoint_itm-0.5.0.tar", last modified: Fri Jun  2 21:19:12 2023, max compression
```

## Comparing `proofpoint_itm-0.4.0.tar` & `proofpoint_itm-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-05-17 01:46:14.394376 proofpoint_itm-0.4.0/
--rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.4.0/LICENSE
--rw-r--r--   0 molden     (501) staff       (20)     8804 2023-05-17 01:46:14.394440 proofpoint_itm-0.4.0/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)     8184 2022-12-11 05:38:51.000000 proofpoint_itm-0.4.0/README.md
--rw-r--r--   0 molden     (501) staff       (20)       74 2023-05-17 01:46:14.394707 proofpoint_itm-0.4.0/setup.cfg
--rw-r--r--   0 molden     (501) staff       (20)      925 2023-05-16 22:46:17.000000 proofpoint_itm-0.4.0/setup.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-05-17 01:46:14.391217 proofpoint_itm-0.4.0/src/
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-05-17 01:46:14.393594 proofpoint_itm-0.4.0/src/proofpoint_itm/
--rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.4.0/src/proofpoint_itm/__init__.py
--rw-r--r--   0 molden     (501) staff       (20)     1359 2022-11-23 17:14:39.000000 proofpoint_itm-0.4.0/src/proofpoint_itm/auth.py
--rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.4.0/src/proofpoint_itm/classes.py
--rw-r--r--   0 molden     (501) staff       (20)    48886 2023-05-17 01:19:36.000000 proofpoint_itm-0.4.0/src/proofpoint_itm/client.py
--rw-r--r--   0 molden     (501) staff       (20)     2407 2022-11-23 17:14:48.000000 proofpoint_itm-0.4.0/src/proofpoint_itm/webclient.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-05-17 01:46:14.394267 proofpoint_itm-0.4.0/src/proofpoint_itm.egg-info/
--rw-r--r--   0 molden     (501) staff       (20)     8804 2023-05-17 01:46:14.000000 proofpoint_itm-0.4.0/src/proofpoint_itm.egg-info/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)      353 2023-05-17 01:46:14.000000 proofpoint_itm-0.4.0/src/proofpoint_itm.egg-info/SOURCES.txt
--rw-r--r--   0 molden     (501) staff       (20)        1 2023-05-17 01:46:14.000000 proofpoint_itm-0.4.0/src/proofpoint_itm.egg-info/dependency_links.txt
--rw-r--r--   0 molden     (501) staff       (20)       15 2023-05-17 01:46:14.000000 proofpoint_itm-0.4.0/src/proofpoint_itm.egg-info/top_level.txt
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.657489 proofpoint_itm-0.5.0/
+-rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.5.0/LICENSE
+-rw-r--r--   0 molden     (501) staff       (20)     1432 2023-06-02 21:19:12.657547 proofpoint_itm-0.5.0/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)      813 2023-05-17 16:06:21.000000 proofpoint_itm-0.5.0/README.md
+-rw-r--r--   0 molden     (501) staff       (20)       74 2023-06-02 21:19:12.657761 proofpoint_itm-0.5.0/setup.cfg
+-rw-r--r--   0 molden     (501) staff       (20)      925 2023-06-02 21:18:12.000000 proofpoint_itm-0.5.0/setup.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.654827 proofpoint_itm-0.5.0/src/
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.656834 proofpoint_itm-0.5.0/src/proofpoint_itm/
+-rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/__init__.py
+-rw-r--r--   0 molden     (501) staff       (20)     1359 2022-11-23 17:14:39.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/auth.py
+-rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/classes.py
+-rw-r--r--   0 molden     (501) staff       (20)    49995 2023-06-02 21:15:31.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/client.py
+-rw-r--r--   0 molden     (501) staff       (20)     2458 2023-06-02 21:10:35.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/webclient.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.657376 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/
+-rw-r--r--   0 molden     (501) staff       (20)     1432 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)      353 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/SOURCES.txt
+-rw-r--r--   0 molden     (501) staff       (20)        1 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/dependency_links.txt
+-rw-r--r--   0 molden     (501) staff       (20)       15 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/top_level.txt
```

### Comparing `proofpoint_itm-0.4.0/LICENSE` & `proofpoint_itm-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.4.0/setup.py` & `proofpoint_itm-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(name='proofpoint_itm',
-    version='0.4.0',
+    version='0.5.0',
     description='Proofpoint ITM API client library',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Mike Olden',
     author_email='michael.olden@oldendigital.com',
     url = 'https://github.com/drizzo-tech/proofpoint_itm',
     project_urls={
```

### Comparing `proofpoint_itm-0.4.0/src/proofpoint_itm/auth.py` & `proofpoint_itm-0.5.0/src/proofpoint_itm/auth.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.4.0/src/proofpoint_itm/classes.py` & `proofpoint_itm-0.5.0/src/proofpoint_itm/classes.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.4.0/src/proofpoint_itm/client.py` & `proofpoint_itm-0.5.0/src/proofpoint_itm/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,30 +34,31 @@
         Returns:
             ITMClient object
         """
         self.client_id = config['client_id']
         self.tenant_id = config['tenant_id']
         self.base_url = f"https://{config['tenant_id']}.explore.proofpoint.com"
         self.auth = itm_auth(config, verify=verify, scope=scope)
+        self.timeout = kwargs.get('timeout', 10)
 
     
     def get_endpoints(self, includes: str='*', kind: str='*', status: str='*',
                       headers: dict={}, count: bool=False) -> dict:
         """
         Fetches all endpoints of a given kind from the registry api
 
         Args:
             includes (str):
-                List of attributes to return, defaults to *
+                List of attributes to return, defaults to '*'
             kind (str): 
                 Type of agent to return,
-                Accepts *, agent:saas, or updater:saas, defaults to *
+                Accepts '*', 'agent:saas', or 'updater:saas', defaults to '*'
             status (str): 
                 Filter by agent status
-                Accepts: *, HEALTHY, UNHEALTHY, UNREACHABLE, DEAD, INACTIVE
+                Accepts: '*', HEALTHY, UNHEALTHY, UNREACHABLE, DEAD, INACTIVE
 
         Returns:
             dict: A list of endpoint objects
 
         """
         endpoint = '/v2/apis/registry/instances'
         url = self.base_url + endpoint
@@ -69,27 +70,27 @@
                   'status': status
                  }
 
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
 
         endpoints = []
         resp = webclient.get_request(
-                url, headers=headers, params=params)
+                url, headers=headers, params=params, timeout=self.timeout)
         total = resp['_meta']['stats']['total']
 
         if count:
             return total
 
         endpoints += resp['data']
         retrieved = len(endpoints)
 
         while retrieved < total:
             params['offset'] = params['offset'] + 100
             resp = webclient.get_request(
-                    url, headers=headers, params=params)
+                    url, headers=headers, params=params, timeout=self.timeout)
             endpoints += resp['data']
             retrieved = len(endpoints)
         
         return endpoints
 
 
     def get_rules(self, includes: str='*', headers: dict={}) -> list:
@@ -107,15 +108,15 @@
             list: A list of rules objects
 
         """
         endpoint = '/v2/apis/ruler/rules'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def get_rule(self, id_: str, includes: str='*', headers: dict={}) -> dict:
         """
         Query for rule by ID in the depot API
 
@@ -132,15 +133,15 @@
             dict: A dict of rule attributes
 
         """
         endpoint = f'/v2/apis/ruler/rules/{id_}'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp
 
 
     def update_rule(self, id_: str, rule: Rule, headers: dict={}, test: bool=False) -> dict:
         """
         Updates an existing rule from a proofpoint_itm.classes.Rule object
 
@@ -159,15 +160,15 @@
             dict: A dictionary containing the API response.
         """
         if test:
             return {'id': str(uuid.uuid4())}
         endpoint = f'/v2/apis/ruler/rules/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
-        resp = webclient.post_request(url, headers=headers, json_data=rule.as_dict(), method='PUT')
+        resp = webclient.post_request(url, headers=headers, json_data=rule.as_dict(), method='PUT', timeout=self.timeout)
         return resp
 
 
     def create_rule(self, rule: Rule, headers: dict={}, test=False) -> dict:
         """Create new rule
 
         Creates a new rule from a proofpoint_itm.classes.Rule object
@@ -186,37 +187,37 @@
         """
         if test:
             return {'id': str(uuid.uuid4())}
         endpoint = f'/v2/apis/ruler/rules'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
         data = {'data': [rule.as_dict()]}
-        resp = webclient.post_request(url, headers=headers, json_data=data, method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=data, method='POST', timeout=self.timeout)
         return resp
 
 
     def get_predicates(self, includes: str='*', headers: dict={}) -> list:
         """
         Query for all predicates in the depot API, does not return built-in
 
         Args:
             includes (str): 
                 Comma-separated list of attributes to include, default = *
             headers (dict): 
-                headers to include in the http request, if not provided
+                headers to include in the http request, if not 
                 a default header will be created with auth info
 
         Returns: 
             list: A list of predicate objects
         """
         endpoint = '/v2/apis/depot/predicates'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def get_predicate(self, id_: str, includes: str='*', headers: dict={}) -> dict:
         """
         Query for a single predicate by ID
 
@@ -232,15 +233,15 @@
         Returns:
             dict: A dict of predicate attributes
         """
         endpoint = f'/v2/apis/depot/predicates/{id_}'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp
 
 
     def get_conditions(self, includes: str='*', headers: dict={}) -> list:
         """
         Query for all custom match predicates (user created) that are not auto
         created from rules
@@ -282,15 +283,15 @@
 
         Returns:
             dict: A dictionary containing the API response.
         """
         endpoint = f'/v2/apis/depot/predicates/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
-        resp = webclient.post_request(url, headers=headers, json_data=predicate.as_dict(), method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=predicate.as_dict(), method='PATCH', timeout=self.timeout)
         return resp
 
     def overwrite_predicate(self, id_, predicate: Predicate, headers: dict={}, test: bool=False) -> dict:
         """
         Overwrite a predicate by ID, Performs a 'PUT' method call to the depot/predicate API
 
         Args:
@@ -306,15 +307,15 @@
 
         Returns:
             dict: A dictionary containing the API response.
         """
         endpoint = f'/v2/apis/depot/predicates/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
-        resp = webclient.post_request(url, headers=headers, json_data=predicate.as_dict(), method='PUT')
+        resp = webclient.post_request(url, headers=headers, json_data=predicate.as_dict(), method='PUT', timeout=self.timeout)
         return resp
 
 
     def create_predicate(self, predicate: Predicate, headers: dict={}, test: bool=False) -> dict:
         """
         Creates a new predicate from a proofpoint_itm.classes.Predicate object
 
@@ -333,15 +334,15 @@
         if test:
             return {'id': str(uuid.uuid4())}
         endpoint = f'/v2/apis/depot/predicates'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
 
         data = {'data': [predicate.as_dict()]}
-        resp = webclient.post_request(url, headers=headers, json_data=data, method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=data, method='POST', timeout=self.timeout)
         return resp
 
 
     def get_tags(self, includes: str='*', headers: dict={}) -> list:
         """
         Query for all tags in the depot API, does not return built-in tags
 
@@ -354,15 +355,15 @@
             list: A list of tags objects.
 
         """
         endpoint = '/v2/apis/depot/tags'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def get_tag(self, id_: str, includes: str='*', headers: dict={}) -> dict:
         """
         Get tag by ID.
 
@@ -376,15 +377,15 @@
             dict: A dictionary of tag information.
 
         """
         endpoint = f'/v2/apis/depot/tags/{id_}'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp
 
     def update_tag(self, id_: str, tag: Tag, headers: dict={}, test: bool=False) -> dict:
         """
         Update a tag.
 
         Args:
@@ -399,15 +400,15 @@
             dict: A dictionary containing the updated tag.
         """
         if test:
             return {'id': str(uuid.uuid4())}
         endpoint = f'/v2/apis/depot/tags/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
-        resp = webclient.post_request(url, headers=headers, json_data=tag.as_dict(), method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=tag.as_dict(), method='PATCH', timeout=self.timeout)
         return resp
 
     def create_tag(self, tag: Tag, headers: dict={}, test: bool=False) -> dict:
         """
         Create a new tag.
 
         Args:
@@ -421,15 +422,15 @@
 
         """
         if test:
             return {'id': str(uuid.uuid4())}
         endpoint = f'/v2/apis/depot/tags'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
-        resp = webclient.post_request(url, headers=headers, json_data=tag.as_dict(), method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=tag.as_dict(), method='POST', timeout=self.timeout)
         return resp
 
     def add_activity_tag(self, fqid, tag_id, headers: dict={}) -> dict:
         """
         Add a tag to an activity.
 
         Parameters:
@@ -442,15 +443,15 @@
             dict: A dictionary containing the API response.
 
         """
         endpoint = f'/v2/apis/activity/events/{fqid}'
         params = {'tagValue': tag_id}
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.post_request(url, headers=headers, method='PATCH', params=params)
+        resp = webclient.post_request(url, headers=headers, method='PATCH', params=params, timeout=self.timeout)
         return resp
     
     def add_activity_assignee(self, fqid, admin_id, headers: dict={}) -> dict:
         """
         Adds an assignee to an activity.
 
         Args:
@@ -463,15 +464,15 @@
             dict: A dictionary containing the API response.
 
         """
         endpoint = f'/v2/apis/activity/events/{fqid}/annotations/workflow/assignment'
         body = {'id': admin_id}
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.post_request(url, headers=headers, method='POST', json_data=body)
+        resp = webclient.post_request(url, headers=headers, method='POST', json_data=body, timeout=self.timeout)
         return resp
 
     def get_agent_policies(self, includes: str='*', headers: dict={}, params: dict=None) -> list:
         """
         Retrieves agent policies from the specified API endpoint.
 
         Args:
@@ -485,15 +486,15 @@
             list: A list containing the retrieved agent policies.
         """
         endpoint = '/v2/apis/registry/policies'
         url = self.base_url + endpoint
         if params is None:
             params = {'limit': 99, 'offset': 0, 'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def get_agent_policy(self, id_: str, includes: str='*', headers: dict={}, params: dict=None) -> dict:
         """
         Retrieves a specific agent policy based on the provided ID from the specified API endpoint.
 
@@ -509,15 +510,15 @@
             dict: A dictionary containing the retrieved agent policy.
         """
         endpoint = f'/v2/apis/registry/policies/{id_}'
         url = self.base_url + endpoint
         if params is None:
             params = {'limit': 99, 'offset': 0, 'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def update_agent_policy(self, id_, policy: AgentPolicy, headers: dict={}, test: bool=False) -> dict:
         """
         Update an Agent Policy by ID
         
@@ -536,15 +537,15 @@
             dict: A dictionary containing the updated agent policy.
         """
         if test:
             return {'status': 200, 'msg': 'success'}
         endpoint = f'/v2/apis/registry/policies/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.post_request(url, headers=headers, json_data=policy.as_dict(), method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=policy.as_dict(), method='PATCH', timeout=self.timeout)
         return resp
 
     def overwrite_agent_policy(self, id_, policy: AgentPolicy, headers: dict={}, test: bool=False) -> dict:
         """
         Overwrite an Agent Policy by ID
 
         Args:
@@ -562,15 +563,15 @@
             dict: A dictionary containing the updated agent policy.
         """
         if test:
             return {'status': 200, 'msg': 'success'}
         endpoint = f'/v2/apis/registry/policies/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.post_request(url, headers=headers, json_data=policy.as_dict(), method='PUT')
+        resp = webclient.post_request(url, headers=headers, json_data=policy.as_dict(), method='PUT', timeout=self.timeout)
         return resp
 
     def create_agent_policy(self, policy: AgentPolicy, headers: dict={}, test: bool=False) -> dict:
         """
         Create an new agent policy from a proofpoint_itm.classes.AgentPolicy object
         
         Args:
@@ -586,15 +587,15 @@
             dict: A dictionary containing the created agent policy.
         """
         if test:
             return {'status': 200, 'msg': 'success'}
         endpoint = f'/v2/apis/registry/policies'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.post_request(url, headers=headers, json_data=policy.as_dict(), method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=policy.as_dict(), method='POST', timeout=self.timeout)
         return resp
 
 
     def get_notification_policies(self, includes='*', headers={}) -> list:
         """
         Query for all notification policies in the notifications API
 
@@ -608,15 +609,15 @@
         Returns: 
             list: A list containing notification policies
         """
         endpoint = '/v2/apis/notification/target-groups'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def update_notification_policy(self, id_: str, target_group: TargetGroup, headers: dict={}, test: bool=False) -> dict:
         """Update existing notification policy (target-group)
 
         Updates an existing notification policy from a proofpoint_itm.classes.TargetGroup object
@@ -636,15 +637,15 @@
             dict: A dictionary containing the updated notification policy.
         """
         if test:
             return {'id': str(uuid.uuid4())}
         endpoint = f'/v2/apis/notification/target-groups/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
-        resp = webclient.post_request(url, headers=headers, json_data=target_group.as_dict(), method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=target_group.as_dict(), method='PATCH', timeout=self.timeout)
         return resp
 
 
     def create_notification_policy(self, target_group: TargetGroup, headers: dict={}, test: bool=False) -> dict:
         """Create new notification policy (target-group)
 
         Creates a new notification policy from a proofpoint_itm.classes.TargetGroup object
@@ -663,15 +664,15 @@
         """
         if test:
             return {'id': str(uuid.uuid4())}
         endpoint = '/v2/apis/notification/target-groups'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
         data = [target_group.as_dict()]
-        resp = webclient.post_request(url, headers=headers, json_data=data, method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=data, method='POST', timeout=self.timeout)
         return resp
 
     def get_dictionaries(self, headers: dict={}, includes: str='*') -> list:
         """
         Retrieve dictionaries from the API endpoint.
 
         Args:
@@ -684,15 +685,15 @@
             list: A list containing the retrieved dictionaries.
 
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/dictionaries'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def get_dictionary(self, id_: str, headers: dict={}, include: str=None) -> dict:
         """
         Retrieve a specific dictionary from the API endpoint.
 
@@ -709,15 +710,15 @@
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/dictionaries/{id_}'
         url = self.base_url + endpoint
         params = {}
         if include is not None:
             params['include'] = include
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
 
 
     def get_dictionary_terms(self, id_: str, headers: dict={}, includes: str='*') -> list:
         """
         Retrieve terms from a specific dictionary in the API endpoint.
 
@@ -732,15 +733,15 @@
             list: A list containing the retrieved terms.
 
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/dictionaries/{id_}/entries'
         url = self.base_url + endpoint
         params = {'includes': includes}
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.get_request(url, headers=headers, params=params)
+        resp = webclient.get_request(url, headers=headers, params=params, timeout=self.timeout)
         return resp['data']
     
 
     def update_dictionary(self, id_: str, dictionary: Dictionary, headers: dict={}) -> dict:
         """
         Update a dictionary.
 
@@ -753,15 +754,15 @@
         Returns:
             dict: A dictionary containing the updated dictionary.
 
     """
         endpoint = f'/v2/apis/ruler/configurations/dlp/dictionaries/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}",}
-        resp = webclient.post_request(url, headers=headers, json_data=dictionary.as_dict(), method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=dictionary.as_dict(), method='PATCH', timeout=self.timeout)
         return resp
 
 
     def create_dictionary(self, dictionary: Dictionary, headers: dict={}) -> dict:
         """
         Create a new dictionary.
 
@@ -774,15 +775,15 @@
         Returns:
             dict: A dictionary containing the created dictionary.
 
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/dictionaries'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.post_request(url, headers=headers, json_data=dictionary.as_dict(), method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=dictionary.as_dict(), method='POST', timeout=self.timeout)
         return resp
 
     def create_dictionaries(self, dictionaries: list=[], headers: dict={}) -> list:
         """
         Creates or updates a batch list of dictionaries
 
         Args:
@@ -794,15 +795,15 @@
             list: A list containing the created dictionaries.
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/dictionaries'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
         dictionary_list = [d.as_dict() for d in dictionaries]
         data = { 'data': dictionary_list }
-        resp = webclient.post_request(url, headers=headers, json_data=data, method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=data, method='PATCH', timeout=self.timeout)
         return resp
 
 
     def delete_dictionary(self, id_: str, headers: dict={}) -> dict:
         """
         Delete a dictionary.
 
@@ -814,15 +815,15 @@
         Returns:
             dict: A dictionary containing the API response.
 
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/dictionaries/{id_}'
         url = self.base_url + endpoint
         headers = {'Authorization': f"{self.auth.token['token_type']} {self.auth.access_token}"}
-        resp = webclient.delete_request(url, headers=headers)
+        resp = webclient.delete_request(url, headers=headers, timeout=self.timeout)
         return resp
 
 
     def update_event_workflow(self, fqid: str, status: str, headers: dict={}) -> dict:
         """Update workflow status of an alert/incident
         
         Args:
@@ -838,15 +839,15 @@
         url = self.base_url + endpoint
         data = {
             'state': {
                 'status': f'incident:status:{status}'
             }
         }
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=data, method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=data, method='PATCH', timeout=self.timeout)
         return resp
 
 
     def get_detectors(self, headers: dict={}) -> list:
         """
         Retrieve detectors from the API endpoint.
 
@@ -860,15 +861,15 @@
         Returns:
             list: A list containing the retrieved detectors.
 
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/detectors'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.get_request(url, headers=headers)
+        resp = webclient.get_request(url, headers=headers, timeout=self.timeout)
         return resp['data']
 
     def get_detector(self, id_: str, headers: dict={}) -> dict:
         """
         Retrieve a specific detector from the API endpoint.
 
         Args:
@@ -881,15 +882,15 @@
         Returns:
             dict: A dictionary containing the retrieved detector.
 
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/detectors/{id_}'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.get_request(url, headers=headers)
+        resp = webclient.get_request(url, headers=headers, timeout=self.timeout)
         return resp
 
     def update_detector(self, id_: str, detector: Detector, headers: dict={}) -> dict:
         """
         This method updates an existing detector with the provided ID based on a `Detector` object.
 
         Args:
@@ -904,15 +905,15 @@
         Returns:
             dict: A dictionary containing the API response.
 
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/detectors/{id_}'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=detector.as_dict(), method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=detector.as_dict(), method='PATCH', timeout=self.timeout)
         return resp
 
     def create_detector(self, detector: Detector, headers: dict={}) -> dict:
         """
         Create a new detector.
 
         Args:
@@ -925,15 +926,15 @@
         Returns:
             dict: A dictionary containing the API response.
 
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/detectors'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=detector.as_dict(), method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=detector.as_dict(), method='POST', timeout=self.timeout)
         return resp
 
     def get_detector_sets(self, headers: dict={}) -> list:
         """
         Retrieve detector sets from the API endpoint.
 
         Args:
@@ -944,15 +945,15 @@
         Returns:
             list: A list containing the retrieved detector sets.
 
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/detectorsets'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.get_request(url, headers=headers)
+        resp = webclient.get_request(url, headers=headers, timeout=self.timeout)
         return resp['data']
 
     def get_detector_set(self, id_: str, headers: dict={}) -> dict:
         """
         Retrieve a specific detector set from the API endpoint based on the provided ID.
 
         Args:
@@ -965,15 +966,15 @@
         Returns:
             dict: A dictionary containing the retrieved detector set.
 
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/detectorsets/{id_}'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.get_request(url, headers=headers)
+        resp = webclient.get_request(url, headers=headers, timeout=self.timeout)
         return resp
 
     def update_detector_set(self, id_: str, detector_set: DetectorSet, headers: dict={}) -> dict:
         """
         Update a detector set with the provided ID based on a `DetectorSet` object.
 
         Args:
@@ -988,15 +989,15 @@
         Returns:
             dict: A dictionary containing the updated detector set.
 
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/detectorsets/{id_}'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=detector_set.as_dict(), method='PATCH')
+        resp = webclient.post_request(url, headers=headers, json_data=detector_set.as_dict(), method='PATCH', timeout=self.timeout)
         return resp
 
     def create_detector_set(self, detector_set: DetectorSet, headers: dict={}) -> dict:
         """
         Create a new detector set.
 
         Args:
@@ -1009,15 +1010,15 @@
         Returns:
             dict: A dictionary containing the created detector set.
 
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/detectorsets'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=detector_set.as_dict(), method='POST')
+        resp = webclient.post_request(url, headers=headers, json_data=detector_set.as_dict(), method='POST', timeout=self.timeout)
         return resp
     
     def delete_detector_set(self, id_: str, headers: dict={}) -> dict:
         """
         Delete a detector set.
 
         Args:
@@ -1030,15 +1031,15 @@
         Returns:
             dict: A dictionary containing the API response.
 
         """
         endpoint = f'/v2/apis/ruler/configurations/dlp/detectorsets/{id_}'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.delete_request(url, headers=headers)
+        resp = webclient.delete_request(url, headers=headers, timeout=self.timeout)
         return resp
 
     def get_smartids(self, headers: dict={}) -> list:
         """
         Retrieve smart IDs from the API endpoint.
 
         Args:
@@ -1049,15 +1050,15 @@
         Returns:
             dict: A dictionary containing the retrieved smart IDs.
 
         """
         endpoint = '/v2/apis/ruler/configurations/dlp/smartids'
         url = self.base_url + endpoint
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.get_request(url, headers=headers)
+        resp = webclient.get_request(url, headers=headers, timeout=self.timeout)
         return resp['data']
 
     def publish_config(self, headers: dict={}, artifactID: str='activity', data: dict={}) -> dict:
         """
         This method publishes a configuration artifact triggers a configuration push.
 
         Args:
@@ -1100,15 +1101,15 @@
             dict: A dictionary containing the API response.
 
         """
         endpoint = '/v2/apis/depot/queries'
         url = self.base_url + endpoint
         params['entityTypes'] = entity
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params)
+        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params, timeout=self.timeout)
         return resp
 
     def notification_search(self, query: dict, entity: str, params: dict={}, headers: dict={}) -> dict:
         """
         Performs a search query against the depot API
 
         Args:
@@ -1128,15 +1129,15 @@
             dict: A dictionary containing the API response.
 
         """
         endpoint = '/v2/apis/notification/queries'
         url = self.base_url + endpoint
         params['entityTypes'] = entity
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params)
+        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params, timeout=self.timeout)
         return resp
 
     def ruler_search(self, query: str, entity: str, params: dict={}, headers: dict={}) -> dict:
         """
         Performs a search query against the ruler API
 
         Args:
@@ -1156,15 +1157,15 @@
             dict: A dictionary containing the API response.
 
         """
         endpoint = '/v2/apis/ruler/queries'
         url = self.base_url + endpoint
         params['entityTypes'] = entity
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params)
+        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params, timeout=self.timeout)
         return resp
 
     def activity_search(self, query: dict, entity: str, params: dict={}, headers: dict={}) -> dict:
         """
         Performs a search query against the activity API
 
         Args:
@@ -1184,15 +1185,15 @@
             dict: A dictionary containing the API response.
 
         """
         endpoint = '/v2/apis/activity/queries'
         url = self.base_url + endpoint
         params['entityTypes'] = entity
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
-        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params)
+        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params, timeout=self.timeout)
         return resp
     
     def registry_search(self, query: dict, entity: str, params: dict = None, headers: dict = None ) -> dict:
         """
         Performs a search query against the registry API
 
         Args:
@@ -1217,9 +1218,9 @@
             params = {}
         params['entityTypes'] = entity
 
         if headers is None:
             headers = {}
         headers['Authorization'] = f"{self.auth.token['token_type']} {self.auth.access_token}"
 
-        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params)
+        resp = webclient.post_request(url, headers=headers, json_data=query, method='POST', params=params, timeout=self.timeout)
         return resp
```

### Comparing `proofpoint_itm-0.4.0/src/proofpoint_itm/webclient.py` & `proofpoint_itm-0.5.0/src/proofpoint_itm/webclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Returns response as dict
     """
     if params:
         url_params = urlencode(params)
         url = url + '?' + url_params
 
-    resp = make_request(url, headers=headers, method='GET')
+    resp = make_request(url, headers=headers, method='GET', timeout=timeout)
     return resp
 
 
 def post_request(url, headers=None, data=None, json_data=None, method='POST', params={}, timeout=10):
     """
     perform a post request
     pass headers/data as standard python dictionary
@@ -36,30 +36,30 @@
         headers['Content-Type'] = 'application/json; charset=utf-8'
         data = json.dumps(json_data)
         data = data.encode('utf-8')
     elif data:
         data = urlencode(data)
         data = data.encode('utf-8')
 
-    resp = make_request(url, headers=headers, data=data, method=method)
+    resp = make_request(url, headers=headers, data=data, method=method, timeout=timeout)
     return resp
 
 def delete_request(url, headers=None, params=None, timeout=10):
     """
     Performs a delete request
     params = dictionary of parameters to be added to the end of url
     headers = dictionary of headers to include in the request
 
     Returns response as dict
     """
     if params:
         url_params = urlencode(params)
         url = url + '?' + url_params
 
-    resp = make_request(url, headers=headers, method='DELETE')
+    resp = make_request(url, headers=headers, method='DELETE', timeout=timeout)
     return resp
 
 def make_request(url, headers=None, data=None, method=None, timeout=10):
     """
     creates and submits the request
 
     returns response as dict
```

