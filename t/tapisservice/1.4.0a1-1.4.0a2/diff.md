# Comparing `tmp/tapisservice-1.4.0a1.tar.gz` & `tmp/tapisservice-1.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapisservice-1.4.0a1.tar", max compression
+gzip compressed data, was "tapisservice-1.4.0a2.tar", max compression
```

## Comparing `tapisservice-1.4.0a1.tar` & `tapisservice-1.4.0a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1086 2023-02-20 20:37:25.853989 tapisservice-1.4.0a1/README.md
--rw-r--r--   0        0        0      853 2023-06-02 19:29:13.091100 tapisservice-1.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     2682 2023-03-02 05:07:52.208778 tapisservice-1.4.0a1/tapisservice/__init__.py
--rw-r--r--   0        0        0    35545 2023-06-02 19:25:04.454134 tapisservice-1.4.0a1/tapisservice/auth.py
--rw-r--r--   0        0        0     6379 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/config.py
--rw-r--r--   0        0        0     6311 2023-02-20 20:38:01.165617 tapisservice-1.4.0a1/tapisservice/configschema.json
--rw-r--r--   0        0        0     1040 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/errors.py
--rw-r--r--   0        0        0     1455 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/logs.py
--rw-r--r--   0        0        0      174 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisdjango/__init__.py
--rw-r--r--   0        0        0       71 2022-10-28 20:28:11.884719 tapisservice-1.4.0a1/tapisservice/tapisfastapi/__init__.py
--rw-r--r--   0        0        0     3851 2022-05-03 16:51:03.395898 tapisservice-1.4.0a1/tapisservice/tapisfastapi/auth.py
--rw-r--r--   0        0        0     3090 2022-05-03 16:18:04.431729 tapisservice-1.4.0a1/tapisservice/tapisfastapi/utils.py
--rw-r--r--   0        0        0       45 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisflask/__init__.py
--rw-r--r--   0        0        0     2826 2023-03-02 01:08:58.073370 tapisservice-1.4.0a1/tapisservice/tapisflask/auth.py
--rw-r--r--   0        0        0     1396 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisflask/resources.py
--rw-r--r--   0        0        0     4185 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/tapisflask/utils.py
--rw-r--r--   0        0        0    15526 2023-02-20 20:38:01.165617 tapisservice-1.4.0a1/tapisservice/tenants.py
--rw-r--r--   0        0        0        0 2022-04-08 19:00:25.736057 tapisservice-1.4.0a1/tapisservice/utils.py
--rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 tapisservice-1.4.0a1/setup.py
--rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 tapisservice-1.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-02-20 20:37:25.853989 tapisservice-1.4.0a2/README.md
+-rw-r--r--   0        0        0      853 2023-06-02 20:46:52.665894 tapisservice-1.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2682 2023-03-02 05:07:52.208778 tapisservice-1.4.0a2/tapisservice/__init__.py
+-rw-r--r--   0        0        0    35545 2023-06-02 19:25:04.454134 tapisservice-1.4.0a2/tapisservice/auth.py
+-rw-r--r--   0        0        0     6379 2022-04-08 19:00:25.736057 tapisservice-1.4.0a2/tapisservice/config.py
+-rw-r--r--   0        0        0     6311 2023-02-20 20:38:01.165617 tapisservice-1.4.0a2/tapisservice/configschema.json
+-rw-r--r--   0        0        0     1040 2022-04-08 19:00:25.736057 tapisservice-1.4.0a2/tapisservice/errors.py
+-rw-r--r--   0        0        0     1455 2022-04-08 19:00:25.736057 tapisservice-1.4.0a2/tapisservice/logs.py
+-rw-r--r--   0        0        0      174 2022-04-08 19:00:25.736057 tapisservice-1.4.0a2/tapisservice/tapisdjango/__init__.py
+-rw-r--r--   0        0        0       71 2022-10-28 20:28:11.884719 tapisservice-1.4.0a2/tapisservice/tapisfastapi/__init__.py
+-rw-r--r--   0        0        0     3851 2022-05-03 16:51:03.395898 tapisservice-1.4.0a2/tapisservice/tapisfastapi/auth.py
+-rw-r--r--   0        0        0     3090 2022-05-03 16:18:04.431729 tapisservice-1.4.0a2/tapisservice/tapisfastapi/utils.py
+-rw-r--r--   0        0        0       45 2022-04-08 19:00:25.736057 tapisservice-1.4.0a2/tapisservice/tapisflask/__init__.py
+-rw-r--r--   0        0        0     2826 2023-03-02 01:08:58.073370 tapisservice-1.4.0a2/tapisservice/tapisflask/auth.py
+-rw-r--r--   0        0        0     1396 2022-04-08 19:00:25.736057 tapisservice-1.4.0a2/tapisservice/tapisflask/resources.py
+-rw-r--r--   0        0        0     4133 2023-06-02 20:44:02.907303 tapisservice-1.4.0a2/tapisservice/tapisflask/utils.py
+-rw-r--r--   0        0        0    15526 2023-02-20 20:38:01.165617 tapisservice-1.4.0a2/tapisservice/tenants.py
+-rw-r--r--   0        0        0        0 2022-04-08 19:00:25.736057 tapisservice-1.4.0a2/tapisservice/utils.py
+-rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 tapisservice-1.4.0a2/setup.py
+-rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 tapisservice-1.4.0a2/PKG-INFO
```

### Comparing `tapisservice-1.4.0a1/README.md` & `tapisservice-1.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/pyproject.toml` & `tapisservice-1.4.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tapisservice"
-version = "1.4.0a1"
+version = "1.4.0a2"
 description = "Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin."
 license = "BSD-4-Clause"
 authors = ["Joe Stubbs <jstubbs@tacc.utexas.edu>"]
 maintainers = ["Joe Stubbs <jstubbs@tacc.utexas.edu>",
 			   "Christian Garcia <cgarcia@tacc.utexas.edu>"]
 readme = "README.md"
 repository = "https://github.com/tapis-project/tapipy-tapisservice"
```

### Comparing `tapisservice-1.4.0a1/tapisservice/__init__.py` & `tapisservice-1.4.0a2/tapisservice/__init__.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/auth.py` & `tapisservice-1.4.0a2/tapisservice/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/config.py` & `tapisservice-1.4.0a2/tapisservice/config.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/configschema.json` & `tapisservice-1.4.0a2/tapisservice/configschema.json`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/errors.py` & `tapisservice-1.4.0a2/tapisservice/errors.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/logs.py` & `tapisservice-1.4.0a2/tapisservice/logs.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/tapisfastapi/auth.py` & `tapisservice-1.4.0a2/tapisservice/tapisfastapi/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/tapisfastapi/utils.py` & `tapisservice-1.4.0a2/tapisservice/tapisfastapi/utils.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/tapisflask/auth.py` & `tapisservice-1.4.0a2/tapisservice/tapisflask/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/tapisflask/resources.py` & `tapisservice-1.4.0a2/tapisservice/tapisflask/resources.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/tapisservice/tapisflask/utils.py` & `tapisservice-1.4.0a2/tapisservice/tapisflask/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import os
 import traceback
 
 # import flask.ext.restful.reqparse as reqparse
 from flask import jsonify, request
 from werkzeug.exceptions import ClientDisconnected
 from flask_restful import Api, reqparse
-from openapi_core import create_spec
+from openapi_core import Spec
 import sqlalchemy
 import yaml
 
 from tapisservice.config import conf
 from tapisservice.errors import BaseTapisError
 from tapisservice.logs import get_logger
 logger = get_logger(__name__)
 
 TAG = conf.version
 
 spec_path = os.environ.get("TAPIS_API_SPEC_PATH", '/home/tapis/service/resources/openapi_v3.yml')
 try:
-    spec_dict = yaml.safe_load(open(spec_path, 'r'))
-    spec = create_spec(spec_dict)
+    spec = Spec.from_file_path(spec_path)
 except Exception as e:
     msg = f"Could not find/parse API spec file at path: {spec_path}; additional information: {e}"
     print(msg)
     raise BaseTapisError(msg)
 
 flask_errors_dict = {
     'MethodNotAllowed': {
```

### Comparing `tapisservice-1.4.0a1/tapisservice/tenants.py` & `tapisservice-1.4.0a2/tapisservice/tenants.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a1/setup.py` & `tapisservice-1.4.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pycryptodome>=3.6.0', 'tapipy>=1.1.1']
 
 setup_kwargs = {
     'name': 'tapisservice',
-    'version': '1.4.0a1',
+    'version': '1.4.0a2',
     'description': "Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin.",
     'long_description': 'Tapipy plugin granting Tapis service functionality using `import tapisservice`.\n\n\n## Automated Builds with Make and Poetry\nThis repository includes a Makefile to automate tasks such as building the images and running tests.\nIt depends on Poetry; see the docs for installing on your platform: https://python-poetry.org/docs/\n\nNote: On Ubunut 20 LTS (and maybe other platforms?) you might hit an issue trying to run the `poetry build` \ncommand with your version of virtualenv; see this issue: https://github.com/python-poetry/poetry/issues/2972\n\nThe workaround, as described in the issue, is to remove the version of virtualenv bundled with Ubuntu and install\nit with pip:\n\n```\n $ sudo apt remove --purge python3-virtualenv virtualenv\n $ sudo apt install python3-pip   # if necessary \n $ pip3 install -U virtualenv\n```\n\n## Running the Tests\n\nIn order to run the tests, you will need to populate the `config-dev-develop.json` file within the `tests` with the service password for `abaco` in develop. If you do not know how to get that password, ask for help on the tacc-cloud slack team.\n\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy-tapisservice',
```

### Comparing `tapisservice-1.4.0a1/PKG-INFO` & `tapisservice-1.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapisservice
-Version: 1.4.0a1
+Version: 1.4.0a2
 Summary: Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin.
 Home-page: https://github.com/tapis-project/tapipy-tapisservice
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
```

