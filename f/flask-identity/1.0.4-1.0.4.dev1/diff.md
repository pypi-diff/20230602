# Comparing `tmp/flask_identity-1.0.4.tar.gz` & `tmp/flask_identity-1.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_identity-1.0.4.tar", max compression
+gzip compressed data, was "flask_identity-1.0.4.dev1.tar", max compression
```

## Comparing `flask_identity-1.0.4.tar` & `flask_identity-1.0.4.dev1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1119 2023-05-29 12:41:30.306646 flask_identity-1.0.4/LICENSE.rst
--rw-r--r--   0        0        0     2604 2023-05-29 12:45:53.285419 flask_identity-1.0.4/README.rst
--rw-r--r--   0        0        0      905 2023-05-31 01:12:45.393303 flask_identity-1.0.4/flask_identity/__init__.py
--rw-r--r--   0        0        0     2244 2023-05-31 01:12:45.386633 flask_identity-1.0.4/flask_identity/_hash_context.py
--rw-r--r--   0        0        0     3346 2023-05-31 01:12:45.405665 flask_identity-1.0.4/flask_identity/_token_context.py
--rw-r--r--   0        0        0     1243 2023-05-31 01:12:45.379734 flask_identity-1.0.4/flask_identity/babels.py
--rw-r--r--   0        0        0      840 2023-05-31 01:12:45.404196 flask_identity-1.0.4/flask_identity/compats.py
--rw-r--r--   0        0        0     9850 2023-05-31 02:44:57.794012 flask_identity-1.0.4/flask_identity/config.py
--rw-r--r--   0        0        0    18080 2023-05-31 01:45:50.580150 flask_identity-1.0.4/flask_identity/core.py
--rw-r--r--   0        0        0    14012 2023-05-31 01:12:45.398245 flask_identity-1.0.4/flask_identity/datastore.py
--rw-r--r--   0        0        0     7829 2023-05-31 03:09:52.352538 flask_identity-1.0.4/flask_identity/decorators.py
--rw-r--r--   0        0        0     3898 2023-05-31 01:48:31.110407 flask_identity-1.0.4/flask_identity/forms.py
--rw-r--r--   0        0        0     5239 2023-05-31 01:12:45.344624 flask_identity-1.0.4/flask_identity/mixins.py
--rw-r--r--   0        0        0      823 2023-05-29 12:41:30.313443 flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1269 2023-05-29 12:41:30.313585 flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0     1076 2023-05-29 12:41:30.313677 flask_identity-1.0.4/flask_identity/translations/flask_identity.pot
--rw-r--r--   0        0        0      814 2023-05-29 12:41:30.313893 flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1264 2023-05-29 12:41:30.314002 flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0    10110 2023-05-31 01:12:45.347764 flask_identity-1.0.4/flask_identity/utils.py
--rw-r--r--   0        0        0     6203 2023-05-31 01:12:45.382128 flask_identity-1.0.4/flask_identity/views.py
--rw-r--r--   0        0        0     1743 2023-05-31 03:41:29.586482 flask_identity-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 flask_identity-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-05-29 12:41:30.306646 flask_identity-1.0.4.dev1/LICENSE.rst
+-rw-r--r--   0        0        0     2604 2023-05-29 12:45:53.285419 flask_identity-1.0.4.dev1/README.rst
+-rw-r--r--   0        0        0      905 2023-05-31 01:12:45.393303 flask_identity-1.0.4.dev1/flask_identity/__init__.py
+-rw-r--r--   0        0        0     2222 2023-06-02 01:05:10.615650 flask_identity-1.0.4.dev1/flask_identity/_hash_context.py
+-rw-r--r--   0        0        0     3324 2023-06-02 01:05:42.439171 flask_identity-1.0.4.dev1/flask_identity/_token_context.py
+-rw-r--r--   0        0        0     1243 2023-05-31 01:12:45.379734 flask_identity-1.0.4.dev1/flask_identity/babels.py
+-rw-r--r--   0        0        0      840 2023-05-31 01:12:45.404196 flask_identity-1.0.4.dev1/flask_identity/compats.py
+-rw-r--r--   0        0        0     9850 2023-05-31 02:44:57.794012 flask_identity-1.0.4.dev1/flask_identity/config.py
+-rw-r--r--   0        0        0    18003 2023-06-02 01:10:46.510671 flask_identity-1.0.4.dev1/flask_identity/core.py
+-rw-r--r--   0        0        0    14012 2023-05-31 01:12:45.398245 flask_identity-1.0.4.dev1/flask_identity/datastore.py
+-rw-r--r--   0        0        0     7829 2023-05-31 03:09:52.352538 flask_identity-1.0.4.dev1/flask_identity/decorators.py
+-rw-r--r--   0        0        0     3898 2023-05-31 01:48:31.110407 flask_identity-1.0.4.dev1/flask_identity/forms.py
+-rw-r--r--   0        0        0     5239 2023-05-31 01:12:45.344624 flask_identity-1.0.4.dev1/flask_identity/mixins.py
+-rw-r--r--   0        0        0      823 2023-05-29 12:41:30.313443 flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1269 2023-05-29 12:41:30.313585 flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0     1076 2023-05-29 12:41:30.313677 flask_identity-1.0.4.dev1/flask_identity/translations/flask_identity.pot
+-rw-r--r--   0        0        0      814 2023-05-29 12:41:30.313893 flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1264 2023-05-29 12:41:30.314002 flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0    10110 2023-05-31 01:12:45.347764 flask_identity-1.0.4.dev1/flask_identity/utils.py
+-rw-r--r--   0        0        0     6203 2023-05-31 01:12:45.382128 flask_identity-1.0.4.dev1/flask_identity/views.py
+-rw-r--r--   0        0        0     1747 2023-06-02 01:19:17.850269 flask_identity-1.0.4.dev1/pyproject.toml
+-rw-r--r--   0        0        0     4224 1970-01-01 00:00:00.000000 flask_identity-1.0.4.dev1/PKG-INFO
```

### Comparing `flask_identity-1.0.4/LICENSE.rst` & `flask_identity-1.0.4.dev1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/README.rst` & `flask_identity-1.0.4.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/__init__.py` & `flask_identity-1.0.4.dev1/flask_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/_hash_context.py` & `flask_identity-1.0.4.dev1/flask_identity/_hash_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 class HashContext(object):
     """
     | Class to generate/verify hash securitied string.
     | Hashed string can used to store context or any unencrypt context.
     """
 
     def __init__(self, app) -> None:
-        # Use the applications's SECRET_KEY as default.
-        secret_key = app.config.get('SECRET_KEY', None)
-        secret_key = app.config.get('IDENTITY_HASH_SALT', secret_key)
+        secret_key = app.config.get('IDENTITY_HASH_SALT', None)
 
-        if not secret_key:
+        if secret_key is None:
+            secret_key = app.config.get('SECRET_KEY', None)
+
+        if secret_key is None:
             raise SystemError('Config setting SECRET_KEY or IDENTITY_HASH_SALT is missing.')
 
         schemes = app.config.get('IDENTITY_HASH_SCHEMES', ['bcrypt'])
         schemes_keywords = app.config.get('IDENTITY_HASH_OPTIONS', {})
 
         # Create a passlib CryptContext
         self.crypt_context = CryptContext(schemes, **schemes_keywords)
```

### Comparing `flask_identity-1.0.4/flask_identity/_token_context.py` & `flask_identity-1.0.4.dev1/flask_identity/_token_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 class TokenContext(object):
     """
     | Class to generate/verify timestamped, signed and encrypted tokens.
     | Tokens can be used as cookie or request content.
     """
 
     def __init__(self, app) -> None:
-        # Use the applications's SECRET_KEY as default.
-        secret_key = app.config.get('SECRET_KEY', None)
-        secret_key = app.config.get('IDENTITY_TOKEN_SALT', secret_key)
+        secret_key = app.config.get('IDENTITY_TOKEN_SALT', None)
 
-        if not secret_key:
+        if secret_key is None:
+            secret_key = app.config.get('SECRET_KEY', None)
+
+        if secret_key is None:
             raise SystemError('Config setting SECRET_KEY or IDENTITY_TOKEN_SALT is missing.')
 
         # Print a warning if SECRET_KEY is too short
         key = secret_key.encode()
         if len(key) < 32:
             print('WARNING: Identity token secret key is shorter than 32 bytes.')
             key = key + b' ' * 32  # Make sure the key is at least 32 bytes long
```

### Comparing `flask_identity-1.0.4/flask_identity/babels.py` & `flask_identity-1.0.4.dev1/flask_identity/babels.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/compats.py` & `flask_identity-1.0.4.dev1/flask_identity/compats.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/config.py` & `flask_identity-1.0.4.dev1/flask_identity/config.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/core.py` & `flask_identity-1.0.4.dev1/flask_identity/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import logging
 
 from datetime import datetime, timedelta
 from hashlib import sha512
 from inspect import isclass
 
 # noinspection PyProtectedMember
-from flask import _request_ctx_stack, request, session, redirect, abort, render_template, current_app
+from flask import g, request, session, redirect, abort, render_template
 from werkzeug.routing import BuildError
 
 from ._hash_context import HashContext
 from ._token_context import TokenContext
 from .datastore import IdentityStore
 from .config import default_config
 from .mixins import AnonymousUserMixin
@@ -175,15 +175,15 @@
             self._register_blueprint = register_blueprint
 
         if register_blueprint:
             create_blueprint(self, __name__, app.json)
 
         self._i18n_domain = get_i18n_domain(app)
 
-        current_app.jinja_env.globals["_fsdomain"] = self._i18n_domain.gettext
+        app.jinja_env.globals["_fsdomain"] = self._i18n_domain.gettext
 
         # Verify that if Flask-Babel is installed
         if have_babel() and "babel" not in app.extensions:
             raise ValueError(
                 "Flask-Babel is installed but not initialized"
             )
 
@@ -301,16 +301,15 @@
         )
 
     def update_request_context_with_user(self, user=None):
         """
         :param user: User object
         :return: Store the given user as ctx.user.
         """
-        ctx = _request_ctx_stack.top
-        ctx.user = self._anonymous_user() if user is None else user
+        g.user = self._anonymous_user() if user is None else user
 
     @property
     def datastore(self) -> IdentityStore:
         """
         :return: The datastore of Identity Manager
         """
         return self._datastore
```

### Comparing `flask_identity-1.0.4/flask_identity/datastore.py` & `flask_identity-1.0.4.dev1/flask_identity/datastore.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/decorators.py` & `flask_identity-1.0.4.dev1/flask_identity/decorators.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/forms.py` & `flask_identity-1.0.4.dev1/flask_identity/forms.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/mixins.py` & `flask_identity-1.0.4.dev1/flask_identity/mixins.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.4.dev1/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/translations/flask_identity.pot` & `flask_identity-1.0.4.dev1/flask_identity/translations/flask_identity.pot`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.4.dev1/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/utils.py` & `flask_identity-1.0.4.dev1/flask_identity/utils.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/flask_identity/views.py` & `flask_identity-1.0.4.dev1/flask_identity/views.py`

 * *Files identical despite different names*

### Comparing `flask_identity-1.0.4/pyproject.toml` & `flask_identity-1.0.4.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
 priority = "supplemental"
 
 [tool.poetry]
 name = "Flask-Identity"
-version = "1.0.4"
+version = "1.0.4dev1"
 description = "A lightweight extension & library to security Flask applications quickly and simply."
 authors = ["SolardiaX <solardiax@hotmail.com>"]
 maintainers = ["SolardiaX <solardiax@hotmail.com>"]
 license = "MIT"
 readme="README.rst"
 repository="https://github.com/SolardiaX/flask-identity"
 homepage="https://github.com/SolardiaX/flask-identity"
```

### Comparing `flask_identity-1.0.4/PKG-INFO` & `flask_identity-1.0.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-identity
-Version: 1.0.4
+Version: 1.0.4.dev1
 Summary: A lightweight extension & library to security Flask applications quickly and simply.
 Home-page: https://github.com/SolardiaX/flask-identity
 License: MIT
 Author: SolardiaX
 Author-email: solardiax@hotmail.com
 Maintainer: SolardiaX
 Maintainer-email: solardiax@hotmail.com
```

