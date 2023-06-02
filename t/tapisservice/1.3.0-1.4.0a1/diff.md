# Comparing `tmp/tapisservice-1.3.0.tar.gz` & `tmp/tapisservice-1.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapisservice-1.3.0.tar", max compression
+gzip compressed data, was "tapisservice-1.4.0a1.tar", max compression
```

## Comparing `tapisservice-1.3.0.tar` & `tapisservice-1.4.0a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1086 2023-02-20 20:37:25.853989 tapisservice-1.3.0/README.md
--rw-r--r--   0        0        0      851 2023-03-02 02:56:39.450206 tapisservice-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2682 2023-03-02 02:56:30.926279 tapisservice-1.3.0/tapisservice/__init__.py
--rw-r--r--   0        0        0    35553 2023-03-02 02:13:30.138789 tapisservice-1.3.0/tapisservice/auth.py
--rw-r--r--   0        0        0     6379 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/config.py
--rw-r--r--   0        0        0     6311 2023-02-20 20:38:01.165617 tapisservice-1.3.0/tapisservice/configschema.json
--rw-r--r--   0        0        0     1040 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/errors.py
--rw-r--r--   0        0        0     1455 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/logs.py
--rw-r--r--   0        0        0      174 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/tapisdjango/__init__.py
--rw-r--r--   0        0        0       71 2022-10-28 20:28:11.884719 tapisservice-1.3.0/tapisservice/tapisfastapi/__init__.py
--rw-r--r--   0        0        0     3851 2022-05-03 16:51:03.395898 tapisservice-1.3.0/tapisservice/tapisfastapi/auth.py
--rw-r--r--   0        0        0     3090 2022-05-03 16:18:04.431729 tapisservice-1.3.0/tapisservice/tapisfastapi/utils.py
--rw-r--r--   0        0        0       45 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/tapisflask/__init__.py
--rw-r--r--   0        0        0     2826 2023-03-02 01:08:58.073370 tapisservice-1.3.0/tapisservice/tapisflask/auth.py
--rw-r--r--   0        0        0     1396 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/tapisflask/resources.py
--rw-r--r--   0        0        0     4185 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/tapisflask/utils.py
--rw-r--r--   0        0        0    15526 2023-02-20 20:38:01.165617 tapisservice-1.3.0/tapisservice/tenants.py
--rw-r--r--   0        0        0        0 2022-04-08 19:00:25.736057 tapisservice-1.3.0/tapisservice/utils.py
--rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 tapisservice-1.3.0/setup.py
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 tapisservice-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-02-20 20:37:25.853989 tapisservice-1.4.0a1/README.md
+-rw-r--r--   0        0        0      853 2023-06-02 19:29:13.091100 tapisservice-1.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2682 2023-03-02 05:07:52.208778 tapisservice-1.4.0a1/tapisservice/__init__.py
+-rw-r--r--   0        0        0    35545 2023-06-02 19:25:04.454134 tapisservice-1.4.0a1/tapisservice/auth.py
+-rw-r--r--   0        0        0     6379 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/config.py
+-rw-r--r--   0        0        0     6311 2023-02-20 20:38:01.165617 tapisservice-1.4.0a1/tapisservice/configschema.json
+-rw-r--r--   0        0        0     1040 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/errors.py
+-rw-r--r--   0        0        0     1455 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/logs.py
+-rw-r--r--   0        0        0      174 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisdjango/__init__.py
+-rw-r--r--   0        0        0       71 2022-10-28 20:28:11.884719 tapisservice-1.4.0a1/tapisservice/tapisfastapi/__init__.py
+-rw-r--r--   0        0        0     3851 2022-05-03 16:51:03.395898 tapisservice-1.4.0a1/tapisservice/tapisfastapi/auth.py
+-rw-r--r--   0        0        0     3090 2022-05-03 16:18:04.431729 tapisservice-1.4.0a1/tapisservice/tapisfastapi/utils.py
+-rw-r--r--   0        0        0       45 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisflask/__init__.py
+-rw-r--r--   0        0        0     2826 2023-03-02 01:08:58.073370 tapisservice-1.4.0a1/tapisservice/tapisflask/auth.py
+-rw-r--r--   0        0        0     1396 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisflask/resources.py
+-rw-r--r--   0        0        0     4185 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisflask/utils.py
+-rw-r--r--   0        0        0    15526 2023-02-20 20:38:01.165617 tapisservice-1.4.0a1/tapisservice/tenants.py
+-rw-r--r--   0        0        0        0 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/utils.py
+-rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 tapisservice-1.4.0a1/setup.py
+-rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 tapisservice-1.4.0a1/PKG-INFO
```

### Comparing `tapisservice-1.3.0/README.md` & `tapisservice-1.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/pyproject.toml` & `tapisservice-1.4.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tapisservice"
-version = "1.3.0"
+version = "1.4.0a1"
 description = "Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin."
 license = "BSD-4-Clause"
 authors = ["Joe Stubbs <jstubbs@tacc.utexas.edu>"]
 maintainers = ["Joe Stubbs <jstubbs@tacc.utexas.edu>",
 			   "Christian Garcia <cgarcia@tacc.utexas.edu>"]
 readme = "README.md"
 repository = "https://github.com/tapis-project/tapipy-tapisservice"
```

### Comparing `tapisservice-1.3.0/tapisservice/__init__.py` & `tapisservice-1.4.0a1/tapisservice/__init__.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/auth.py` & `tapisservice-1.4.0a1/tapisservice/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     kwargs: the kwargs passed to the __call__ function.
 
     This function makes the following updates to the prepared_request object:
     1. It sets the base URL for the request. 
     2. It sets the X-Tapis-Token header to the appropriate service token.
     3. It sets the X-Tapis-Tenant and X-Tapis-User headers.
     """
-    logger.debug(f"top of preprocess_service_request for operation: {operation.http_method.upper()}: {operation.op_desc.path_name}")
+    logger.debug(f"top of preprocess_service_request for operation: {operation.http_method.upper()}: {operation.path_name}")
     # for service requests, we must determine which site to use for the request. there are 3 cases.
     # first, the caller can explicitly set the _tapis_set_x_headers_from_service variable. this instructs the library
     # to use the service's site and name for setting the X-Tapis-Tenant and User headers when making the request.
     if '_tapis_set_x_headers_from_service' in kwargs and kwargs['_tapis_set_x_headers_from_service']:
         # in this case, we assume the tenant for the request is the admin tenant of the site the service belongs to.
         request_tenant_id = conf.service_tenant_id
         request_x_tapis_user = conf.service_name
```

### Comparing `tapisservice-1.3.0/tapisservice/config.py` & `tapisservice-1.4.0a1/tapisservice/config.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/configschema.json` & `tapisservice-1.4.0a1/tapisservice/configschema.json`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/errors.py` & `tapisservice-1.4.0a1/tapisservice/errors.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/logs.py` & `tapisservice-1.4.0a1/tapisservice/logs.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/tapisfastapi/auth.py` & `tapisservice-1.4.0a1/tapisservice/tapisfastapi/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/tapisfastapi/utils.py` & `tapisservice-1.4.0a1/tapisservice/tapisfastapi/utils.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/tapisflask/auth.py` & `tapisservice-1.4.0a1/tapisservice/tapisflask/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/tapisflask/resources.py` & `tapisservice-1.4.0a1/tapisservice/tapisflask/resources.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/tapisflask/utils.py` & `tapisservice-1.4.0a1/tapisservice/tapisflask/utils.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/tapisservice/tenants.py` & `tapisservice-1.4.0a1/tapisservice/tenants.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.3.0/setup.py` & `tapisservice-1.4.0a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pycryptodome>=3.6.0', 'tapipy>=1.1.1']
 
 setup_kwargs = {
     'name': 'tapisservice',
-    'version': '1.3.0',
+    'version': '1.4.0a1',
     'description': "Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin.",
     'long_description': 'Tapipy plugin granting Tapis service functionality using `import tapisservice`.\n\n\n## Automated Builds with Make and Poetry\nThis repository includes a Makefile to automate tasks such as building the images and running tests.\nIt depends on Poetry; see the docs for installing on your platform: https://python-poetry.org/docs/\n\nNote: On Ubunut 20 LTS (and maybe other platforms?) you might hit an issue trying to run the `poetry build` \ncommand with your version of virtualenv; see this issue: https://github.com/python-poetry/poetry/issues/2972\n\nThe workaround, as described in the issue, is to remove the version of virtualenv bundled with Ubuntu and install\nit with pip:\n\n```\n $ sudo apt remove --purge python3-virtualenv virtualenv\n $ sudo apt install python3-pip   # if necessary \n $ pip3 install -U virtualenv\n```\n\n## Running the Tests\n\nIn order to run the tests, you will need to populate the `config-dev-develop.json` file within the `tests` with the service password for `abaco` in develop. If you do not know how to get that password, ask for help on the tacc-cloud slack team.\n\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy-tapisservice',
```

### Comparing `tapisservice-1.3.0/PKG-INFO` & `tapisservice-1.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapisservice
-Version: 1.3.0
+Version: 1.4.0a1
 Summary: Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin.
 Home-page: https://github.com/tapis-project/tapipy-tapisservice
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
```

