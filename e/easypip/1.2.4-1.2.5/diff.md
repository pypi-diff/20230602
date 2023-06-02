# Comparing `tmp/easypip-1.2.4.tar.gz` & `tmp/easypip-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypip-1.2.4.tar", last modified: Fri Jun  2 13:19:41 2023, max compression
+gzip compressed data, was "easypip-1.2.5.tar", last modified: Fri Jun  2 13:23:45 2023, max compression
```

## Comparing `easypip-1.2.4.tar` & `easypip-1.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:41.987173 easypip-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:41.987173 easypip-1.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:41.987173 easypip-1.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 13:19:29.000000 easypip-1.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 13:19:29.000000 easypip-1.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 13:19:29.000000 easypip-1.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:19:41.987173 easypip-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 13:19:29.000000 easypip-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 13:19:29.000000 easypip-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 13:19:41.987173 easypip-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 13:19:29.000000 easypip-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:41.987173 easypip-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:41.987173 easypip-1.2.4/src/easypip/
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-02 13:19:29.000000 easypip-1.2.4/src/easypip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 13:19:41.000000 easypip-1.2.4/src/easypip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:41.987173 easypip-1.2.4/src/easypip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:19:41.000000 easypip-1.2.4/src/easypip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 13:19:41.000000 easypip-1.2.4/src/easypip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:19:41.000000 easypip-1.2.4/src/easypip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 13:19:41.000000 easypip-1.2.4/src/easypip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:23:45.698564 easypip-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:23:45.698564 easypip-1.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:23:45.698564 easypip-1.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 13:23:35.000000 easypip-1.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 13:23:35.000000 easypip-1.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-02 13:23:35.000000 easypip-1.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:23:45.698564 easypip-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-02 13:23:35.000000 easypip-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 13:23:35.000000 easypip-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-02 13:23:45.698564 easypip-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 13:23:35.000000 easypip-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:23:45.698564 easypip-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:23:45.698564 easypip-1.2.5/src/easypip/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-02 13:23:35.000000 easypip-1.2.5/src/easypip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 13:23:45.000000 easypip-1.2.5/src/easypip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:23:45.698564 easypip-1.2.5/src/easypip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 13:23:45.000000 easypip-1.2.5/src/easypip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 13:23:45.000000 easypip-1.2.5/src/easypip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:23:45.000000 easypip-1.2.5/src/easypip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 13:23:45.000000 easypip-1.2.5/src/easypip.egg-info/top_level.txt
```

### Comparing `easypip-1.2.4/.github/workflows/python-publish.yml` & `easypip-1.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.4/.gitignore` & `easypip-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `easypip-1.2.4/.pre-commit-config.yaml` & `easypip-1.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.4/pyproject.toml` & `easypip-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easypip-1.2.4/src/easypip/__init__.py` & `easypip-1.2.5/src/easypip/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             elif comparator == "<":
                 return version < desired_version
 
         return True
 
     @staticmethod
     def install(requirement: Requirement, extra_args: List[str] = []):
-        logging.info("Installing %s", requirement)
+        print(f"[easypip] Installing {requirement}", file=sys.stderr if is_notebook() else sys.stdout)
         try:
             subprocess.run(
                 [sys.executable, "-m", "pip", "install", str(requirement)] + extra_args,
                 capture_output=True, check=True
             )
         except subprocess.CalledProcessError as e:
             logging.error("pip install %s returned an error:", str(requirement))
```

