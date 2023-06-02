# Comparing `tmp/impact-stack-observability-0.1.0.tar.gz` & `tmp/impact-stack-observability-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impact-stack-observability-0.1.0.tar", last modified: Thu Mar  2 10:04:08 2023, max compression
+gzip compressed data, was "impact-stack-observability-0.2.0.tar", last modified: Fri Jun  2 08:15:39 2023, max compression
```

## Comparing `impact-stack-observability-0.1.0.tar` & `impact-stack-observability-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-03-02 10:04:08.832260 impact-stack-observability-0.1.0/
--rw-r--r--   0 devel     (1001) devel     (1001)    35149 2023-01-23 11:48:29.000000 impact-stack-observability-0.1.0/LICENSE
--rw-r--r--   0 devel     (1001) devel     (1001)    44155 2023-03-02 10:04:08.832260 impact-stack-observability-0.1.0/PKG-INFO
--rw-r--r--   0 devel     (1001) devel     (1001)     2943 2023-03-02 10:03:47.000000 impact-stack-observability-0.1.0/README.md
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-03-02 10:04:08.828261 impact-stack-observability-0.1.0/impact_stack/
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-03-02 10:04:08.832260 impact-stack-observability-0.1.0/impact_stack/observability/
--rw-r--r--   0 devel     (1001) devel     (1001)       52 2023-02-27 12:07:54.000000 impact-stack-observability-0.1.0/impact_stack/observability/__init__.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-03-02 10:04:08.832260 impact-stack-observability-0.1.0/impact_stack/observability/health/
--rw-r--r--   0 devel     (1001) devel     (1001)      259 2023-03-01 13:04:56.000000 impact-stack-observability-0.1.0/impact_stack/observability/health/__init__.py
--rw-r--r--   0 devel     (1001) devel     (1001)     2495 2023-03-01 13:04:56.000000 impact-stack-observability-0.1.0/impact_stack/observability/health/blueprint.py
--rw-r--r--   0 devel     (1001) devel     (1001)     1548 2023-03-01 13:04:56.000000 impact-stack-observability-0.1.0/impact_stack/observability/health/checks.py
--rw-r--r--   0 devel     (1001) devel     (1001)     1741 2023-03-01 13:04:56.000000 impact-stack-observability-0.1.0/impact_stack/observability/health/extension.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-03-02 10:04:08.832260 impact-stack-observability-0.1.0/impact_stack_observability.egg-info/
--rw-r--r--   0 devel     (1001) devel     (1001)    44155 2023-03-02 10:04:08.000000 impact-stack-observability-0.1.0/impact_stack_observability.egg-info/PKG-INFO
--rw-r--r--   0 devel     (1001) devel     (1001)      504 2023-03-02 10:04:08.000000 impact-stack-observability-0.1.0/impact_stack_observability.egg-info/SOURCES.txt
--rw-r--r--   0 devel     (1001) devel     (1001)        1 2023-03-02 10:04:08.000000 impact-stack-observability-0.1.0/impact_stack_observability.egg-info/dependency_links.txt
--rw-r--r--   0 devel     (1001) devel     (1001)      130 2023-03-02 10:04:08.000000 impact-stack-observability-0.1.0/impact_stack_observability.egg-info/requires.txt
--rw-r--r--   0 devel     (1001) devel     (1001)       13 2023-03-02 10:04:08.000000 impact-stack-observability-0.1.0/impact_stack_observability.egg-info/top_level.txt
--rw-r--r--   0 devel     (1001) devel     (1001)     1446 2023-03-02 09:57:21.000000 impact-stack-observability-0.1.0/pyproject.toml
--rw-r--r--   0 devel     (1001) devel     (1001)       38 2023-03-02 10:04:08.832260 impact-stack-observability-0.1.0/setup.cfg
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/
+-rw-r--r--   0 devel     (1001) devel     (1001)    35149 2023-01-23 11:48:29.000000 impact-stack-observability-0.2.0/LICENSE
+-rw-r--r--   0 devel     (1001) devel     (1001)    44584 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/PKG-INFO
+-rw-r--r--   0 devel     (1001) devel     (1001)     3372 2023-06-02 08:09:11.000000 impact-stack-observability-0.2.0/README.md
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.789650 impact-stack-observability-0.2.0/impact_stack/
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.789650 impact-stack-observability-0.2.0/impact_stack/observability/
+-rw-r--r--   0 devel     (1001) devel     (1001)       52 2023-02-27 12:07:54.000000 impact-stack-observability-0.2.0/impact_stack/observability/__init__.py
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/impact_stack/observability/health/
+-rw-r--r--   0 devel     (1001) devel     (1001)      259 2023-03-13 13:19:20.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1001)     3214 2023-06-02 08:09:11.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/blueprint.py
+-rw-r--r--   0 devel     (1001) devel     (1001)     1548 2023-03-13 13:19:20.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/checks.py
+-rw-r--r--   0 devel     (1001) devel     (1001)     1741 2023-03-13 13:19:20.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/extension.py
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/
+-rw-r--r--   0 devel     (1001) devel     (1001)    44584 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/PKG-INFO
+-rw-r--r--   0 devel     (1001) devel     (1001)      504 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/SOURCES.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)        1 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/dependency_links.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)      130 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/requires.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)       13 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/top_level.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)     1446 2023-06-02 08:09:48.000000 impact-stack-observability-0.2.0/pyproject.toml
+-rw-r--r--   0 devel     (1001) devel     (1001)       38 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/setup.cfg
```

### Comparing `impact-stack-observability-0.1.0/LICENSE` & `impact-stack-observability-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `impact-stack-observability-0.1.0/PKG-INFO` & `impact-stack-observability-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impact-stack-observability
-Version: 0.1.0
+Version: 0.2.0
 Summary: Observability for Impact Stack
 Author-email: Alex Berger <alex@more-onion.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -814,7 +814,19 @@
     "GET",
     "https://api.example.com/v1/health/ping",
     200,  # expected response status code
     2.0,  # timeout
 )
 health.register_check("example", check_example)
 ```
+
+### Authorization
+
+A simple mechanism to prevent unrestricted calls to the `/health/` endpoint is
+using a shared secret in the HTTP calls.
+
+Set the required config variable `HEALTH_URL_SECRET` to a (random) string and
+use the GET param `auth` in calls to the endpoint.
+Returns `401` if the secret does not match.
+Raises a `RuntimeError` if not set.
+
+If the `HEALTH_URL_SECRET` is set to `None`, checking the secret is disabled.
```

### Comparing `impact-stack-observability-0.1.0/impact_stack/observability/health/blueprint.py` & `impact-stack-observability-0.2.0/impact_stack/observability/health/blueprint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 """Blueprint for the Health API."""
+
+import functools
+
 import flask
 
 bp = flask.Blueprint("health", __name__)
 
 
+@bp.record
+def deferred_check(state):
+    """Run on registering the blueprint.
+
+    This checks the sanity of the app config for this blueprint.
+    """
+    if "HEALTH_URL_SECRET" not in state.app.config:
+        raise RuntimeError("HEALTH_URL_SECRET not set")
+
+
 def filter_checks(requested_checks):
     """Filter checks from the checks map.
 
     Filter by:
     - "_defaults": check the default checks
     - a list of check names ("_defaults" is allowed).
     """
@@ -28,15 +41,29 @@
     """
     checks_map = (
         checks_map if checks_map is not None else flask.current_app.extensions["health"].checks
     )
     return {k: check() for (k, check) in checks_map.items()}
 
 
+def secret_required(func):
+    """Ensures that a shared secret is given as GET parameter."""
+
+    @functools.wraps(func)
+    def decorated_function(*args, **kwargs):
+        secret = flask.current_app.config.get("HEALTH_URL_SECRET", None)
+        if secret is not None and flask.request.args.get("auth", None) != secret:
+            flask.abort(401)
+        return func(*args, **kwargs)
+
+    return decorated_function
+
+
 @bp.route("/")
+@secret_required
 def health():
     """Health summary.
 
     Returns
     - 200 OK if all checks pass,
     - 503 Service Unavailable otherwise.
```

### Comparing `impact-stack-observability-0.1.0/impact_stack/observability/health/checks.py` & `impact-stack-observability-0.2.0/impact_stack/observability/health/checks.py`

 * *Files identical despite different names*

### Comparing `impact-stack-observability-0.1.0/impact_stack/observability/health/extension.py` & `impact-stack-observability-0.2.0/impact_stack/observability/health/extension.py`

 * *Files identical despite different names*

### Comparing `impact-stack-observability-0.1.0/impact_stack_observability.egg-info/PKG-INFO` & `impact-stack-observability-0.2.0/impact_stack_observability.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impact-stack-observability
-Version: 0.1.0
+Version: 0.2.0
 Summary: Observability for Impact Stack
 Author-email: Alex Berger <alex@more-onion.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -814,7 +814,19 @@
     "GET",
     "https://api.example.com/v1/health/ping",
     200,  # expected response status code
     2.0,  # timeout
 )
 health.register_check("example", check_example)
 ```
+
+### Authorization
+
+A simple mechanism to prevent unrestricted calls to the `/health/` endpoint is
+using a shared secret in the HTTP calls.
+
+Set the required config variable `HEALTH_URL_SECRET` to a (random) string and
+use the GET param `auth` in calls to the endpoint.
+Returns `401` if the secret does not match.
+Raises a `RuntimeError` if not set.
+
+If the `HEALTH_URL_SECRET` is set to `None`, checking the secret is disabled.
```

### Comparing `impact-stack-observability-0.1.0/pyproject.toml` & `impact-stack-observability-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "impact-stack-observability"
-version = "0.1.0"
+version = "0.2.0"
 description = "Observability for Impact Stack"
 dependencies = [
   "flask",
   "requests",
 ]
 authors = [
   { name = "Alex Berger", email = "alex@more-onion.com" },
```

