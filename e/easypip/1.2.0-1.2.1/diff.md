# Comparing `tmp/easypip-1.2.0.tar.gz` & `tmp/easypip-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypip-1.2.0.tar", last modified: Fri Jun  2 08:33:26 2023, max compression
+gzip compressed data, was "easypip-1.2.1.tar", last modified: Fri Jun  2 09:22:10 2023, max compression
```

## Comparing `easypip-1.2.0.tar` & `easypip-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 08:33:11.000000 easypip-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 08:33:11.000000 easypip-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 08:33:11.000000 easypip-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 08:33:26.902344 easypip-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 08:33:11.000000 easypip-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 08:33:11.000000 easypip-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 08:33:26.906344 easypip-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 08:33:11.000000 easypip-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/src/easypip/
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-02 08:33:11.000000 easypip-1.2.0/src/easypip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/src/easypip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.674482 easypip-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 09:21:57.000000 easypip-1.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 09:21:57.000000 easypip-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 09:21:57.000000 easypip-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 09:22:10.678482 easypip-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 09:21:57.000000 easypip-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 09:21:57.000000 easypip-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 09:22:10.678482 easypip-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 09:21:57.000000 easypip-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/src/easypip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-02 09:21:57.000000 easypip-1.2.1/src/easypip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/src/easypip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/top_level.txt
```

### Comparing `easypip-1.2.0/.github/workflows/python-publish.yml` & `easypip-1.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.0/.gitignore` & `easypip-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `easypip-1.2.0/.pre-commit-config.yaml` & `easypip-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.0/pyproject.toml` & `easypip-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.0/src/easypip/__init__.py` & `easypip-1.2.1/src/easypip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         Installer._packages = None
 
 def _install(req: Requirement, ask: bool):
     if not Installer.has_requirement(req):
         if ask:
             answer = ""
             while answer not in ["y", "n"]:
-                answer = input(f"Module is not installed. Install {spec}? [y/n] ").lower()
+                answer = input(f"Module is not installed. Install {req.name}? [y/n] ").lower()
         
         if not ask or answer == "y":
             Installer.install(req)
         else:
             logging.warning("Not installing as required")
             return None
```

