# Comparing `tmp/easypip-1.2.1.tar.gz` & `tmp/easypip-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypip-1.2.1.tar", last modified: Fri Jun  2 09:22:10 2023, max compression
+gzip compressed data, was "easypip-1.2.3.tar", last modified: Fri Jun  2 13:09:56 2023, max compression
```

## Comparing `easypip-1.2.1.tar` & `easypip-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.674482 easypip-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 09:21:57.000000 easypip-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 09:21:57.000000 easypip-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 09:21:57.000000 easypip-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 09:22:10.678482 easypip-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 09:21:57.000000 easypip-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 09:21:57.000000 easypip-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 09:22:10.678482 easypip-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 09:21:57.000000 easypip-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/src/easypip/
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-02 09:21:57.000000 easypip-1.2.1/src/easypip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:10.678482 easypip-1.2.1/src/easypip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 09:22:10.000000 easypip-1.2.1/src/easypip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:56.308678 easypip-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:56.304678 easypip-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:56.308678 easypip-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 13:09:43.000000 easypip-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 13:09:43.000000 easypip-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 13:09:43.000000 easypip-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:09:56.308678 easypip-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 13:09:43.000000 easypip-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 13:09:43.000000 easypip-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 13:09:56.308678 easypip-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 13:09:43.000000 easypip-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:56.304678 easypip-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:56.308678 easypip-1.2.3/src/easypip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-02 13:09:43.000000 easypip-1.2.3/src/easypip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 13:09:56.000000 easypip-1.2.3/src/easypip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:09:56.308678 easypip-1.2.3/src/easypip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:09:56.000000 easypip-1.2.3/src/easypip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 13:09:56.000000 easypip-1.2.3/src/easypip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:09:56.000000 easypip-1.2.3/src/easypip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 13:09:56.000000 easypip-1.2.3/src/easypip.egg-info/top_level.txt
```

### Comparing `easypip-1.2.1/.github/workflows/python-publish.yml` & `easypip-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.1/.gitignore` & `easypip-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `easypip-1.2.1/.pre-commit-config.yaml` & `easypip-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.1/pyproject.toml` & `easypip-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.1/src/easypip/__init__.py` & `easypip-1.2.3/src/easypip/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,17 +81,24 @@
                 return version < desired_version
 
         return True
 
     @staticmethod
     def install(requirement: Requirement, extra_args: List[str] = []):
         logging.info("Installing %s", requirement)
-        subprocess.check_call(
-            [sys.executable, "-m", "pip", "install", str(requirement)] + extra_args
-        )
+        try:
+            subprocess.run(
+                [sys.executable, "-m", "pip", "install", str(requirement)] + extra_args,
+                capture_output=True, check=True
+            )
+        except subprocess.CalledProcessError as e:
+            logging.error("pip install %s returned an error:", str(requirement))
+            logging.error("%s", e.stdout.decode("utf-8"))
+            logging.error("%s", e.stderr.decode("utf-8"))
+            raise
         Installer._packages = None
 
 def _install(req: Requirement, ask: bool):
     if not Installer.has_requirement(req):
         if ask:
             answer = ""
             while answer not in ["y", "n"]:
```

