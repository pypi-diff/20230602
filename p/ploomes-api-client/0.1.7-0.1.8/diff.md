# Comparing `tmp/ploomes-api-client-0.1.7.tar.gz` & `tmp/ploomes-api-client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.1.7.tar", last modified: Thu Jun  1 21:49:44 2023, max compression
+gzip compressed data, was "ploomes-api-client-0.1.8.tar", last modified: Thu Jun  1 23:06:37 2023, max compression
```

## Comparing `ploomes-api-client-0.1.7.tar` & `ploomes-api-client-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 21:49:44.501585 ploomes-api-client-0.1.7/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.7/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-06-01 21:49:44.501431 ploomes-api-client-0.1.7/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.7/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 21:49:44.500456 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-06-01 21:49:44.000000 ploomes-api-client-0.1.7/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 21:49:44.500889 ploomes-api-client-0.1.7/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.7/ploomes_client/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    24693 2023-06-01 21:46:49.000000 ploomes-api-client-0.1.7/ploomes_client/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-01 21:49:44.501637 ploomes-api-client-0.1.7/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-01 21:49:43.000000 ploomes-api-client-0.1.7/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 23:06:37.369135 ploomes-api-client-0.1.8/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.8/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-06-01 23:06:37.369004 ploomes-api-client-0.1.8/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.8/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 23:06:37.368212 ploomes-api-client-0.1.8/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-06-01 23:06:37.000000 ploomes-api-client-0.1.8/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-06-01 23:06:37.000000 ploomes-api-client-0.1.8/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-01 23:06:37.000000 ploomes-api-client-0.1.8/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-06-01 23:06:37.000000 ploomes-api-client-0.1.8/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-06-01 23:06:37.000000 ploomes-api-client-0.1.8/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-01 23:06:37.368575 ploomes-api-client-0.1.8/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.8/ploomes_client/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    24765 2023-06-01 23:05:04.000000 ploomes-api-client-0.1.8/ploomes_client/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-01 23:06:37.369188 ploomes-api-client-0.1.8/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-01 23:05:19.000000 ploomes-api-client-0.1.8/setup.py
```

### Comparing `ploomes-api-client-0.1.7/LICENSE` & `ploomes-api-client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.7/PKG-INFO` & `ploomes-api-client-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.7/README.md` & `ploomes-api-client-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.7/ploomes_api_client.egg-info/PKG-INFO` & `ploomes-api-client-0.1.8/ploomes_api_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.7/ploomes_client/ploomes_client.py` & `ploomes-api-client-0.1.8/ploomes_client/ploomes_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,17 +284,17 @@
         if response.get('value'):
             return response['value'][0]['AvatarUrl']
         return None
 
     @retry
     @sleep_and_retry
     @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
-    def get_contacts(self, filter):
+    def get_contacts(self, _filter):
         response = []
-        url = f"{self.host}/Contacts?$top=300&$orderby=Id+desc,CNPJ&$expand=OtherProperties,Phones&$filter={filter}"
+        url = f"{self.host}/Contacts?$top=300&$orderby=Id+desc,CNPJ&$expand=OtherProperties,Phones&$filter={_filter}"
         while url:
             r = requests.get(url, headers=self.headers)
             data = r.json()
             if data.get('value'):
                 response += data["value"]
             url = data.get("@odata.nextLink")
         return response
@@ -318,24 +318,24 @@
         response = r.json()
         print(response)
         return response
 
     @retry
     @sleep_and_retry
     @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
-    def get_field(self, _filter):
-        r = requests.get(
-            f"{self.host}/Fields?$filter={_filter}&$expand=Type,OptionsTable($expand=Options)",
-            headers=self.headers,
-        )
-        response = r.json().get("value")
-        if response:
-            item = next(iter(response))
-            return item
-        return None
+    def get_fields(self, _filter, _expand="OtherProperties"):
+        response = []
+        url = f"{self.host}/Fields?$filter={_filter}&$expand={_expand}"
+        while url:
+            r = requests.get(url, headers=self.headers, timeout=5)
+            data = r.json()
+            if data.get('value'):
+                response += data["value"]
+            url = data.get("@odata.nextLink")
+        return response
 
     @retry
     @sleep_and_retry
     @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
     def get_field_options(self, table_id):
         r = requests.get(
             f"{self.host}/Fields@OptionsTables@Options?$filter=TableId+eq+{table_id}&$orderby=Name&$count=true&$top=10&$skip=0",
```

### Comparing `ploomes-api-client-0.1.7/setup.py` & `ploomes-api-client-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

