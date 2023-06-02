# Comparing `tmp/easypip-1.1.0.tar.gz` & `tmp/easypip-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypip-1.1.0.tar", last modified: Mon Mar 20 06:51:42 2023, max compression
+gzip compressed data, was "easypip-1.2.0.tar", last modified: Fri Jun  2 08:33:26 2023, max compression
```

## Comparing `easypip-1.1.0.tar` & `easypip-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 06:51:42.632417 easypip-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-20 06:51:42.632417 easypip-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-20 06:51:31.000000 easypip-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 06:51:42.632417 easypip-1.1.0/easypip/
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-20 06:51:31.000000 easypip-1.1.0/easypip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 06:51:42.632417 easypip-1.1.0/easypip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-20 06:51:42.000000 easypip-1.1.0/easypip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-20 06:51:42.000000 easypip-1.1.0/easypip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 06:51:42.000000 easypip-1.1.0/easypip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-20 06:51:42.000000 easypip-1.1.0/easypip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-20 06:51:42.000000 easypip-1.1.0/easypip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-20 06:51:42.632417 easypip-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-20 06:51:31.000000 easypip-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 08:33:11.000000 easypip-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 08:33:11.000000 easypip-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 08:33:11.000000 easypip-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 08:33:26.902344 easypip-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 08:33:11.000000 easypip-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 08:33:11.000000 easypip-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 08:33:26.906344 easypip-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 08:33:11.000000 easypip-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/src/easypip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-02 08:33:11.000000 easypip-1.2.0/src/easypip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:33:26.902344 easypip-1.2.0/src/easypip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 08:33:26.000000 easypip-1.2.0/src/easypip.egg-info/top_level.txt
```

### Comparing `easypip-1.1.0/easypip/__init__.py` & `easypip-1.2.0/src/easypip/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import subprocess
 from typing import List
 from pkg_resources import Requirement, parse_requirements
 from packaging.version import parse as parse_version
 import sys
 import importlib
 import logging
+from ._version import __version__
 
 
 class IPython(Enum):
     NONE = 0
     OTHER = 1
     IPYTHON = 2
     JUPYTER = 3
@@ -85,32 +86,39 @@
     def install(requirement: Requirement, extra_args: List[str] = []):
         logging.info("Installing %s", requirement)
         subprocess.check_call(
             [sys.executable, "-m", "pip", "install", str(requirement)] + extra_args
         )
         Installer._packages = None
 
-
-def easyimport(spec: str, ask=False):
-    reqs = [req for req in parse_requirements(spec)]
-    assert len(reqs) == 1, "only one package should be mentioned in the specification"
-    (req,) = reqs
-
+def _install(req: Requirement, ask: bool):
     if not Installer.has_requirement(req):
         if ask:
             answer = ""
             while answer not in ["y", "n"]:
-                answer = input(
-                    f"Module is not installed. Install {spec}? [y/n] "
-                ).lower()
-
+                answer = input(f"Module is not installed. Install {spec}? [y/n] ").lower()
+        
         if not ask or answer == "y":
             Installer.install(req)
         else:
             logging.warning("Not installing as required")
             return None
+        
+def easyinstall(spec: str, ask=False):
+    reqs = [req for req in parse_requirements(spec)]
+    assert len(reqs) == 1, "only one package should be mentioned in the specification"
+    req, = reqs
+    _install(req, ask)
+
+
+def easyimport(spec: str, ask=False):
+    reqs = [req for req in parse_requirements(spec)]
+    assert len(reqs) == 1, "only one package should be mentioned in the specification"
+    req, = reqs
+
+    _install(req, ask)
 
     return importlib.import_module(req.name)
 
 
 has_requirement = Installer.has_requirement
 install = Installer.install
```

