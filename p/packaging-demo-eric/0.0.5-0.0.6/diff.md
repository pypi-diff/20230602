# Comparing `tmp/packaging-demo-eric-0.0.5.tar.gz` & `tmp/packaging-demo-eric-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging-demo-eric-0.0.5.tar", last modified: Thu Jun  1 07:10:20 2023, max compression
+gzip compressed data, was "packaging-demo-eric-0.0.6.tar", last modified: Fri Jun  2 08:28:43 2023, max compression
```

## Comparing `packaging-demo-eric-0.0.5.tar` & `packaging-demo-eric-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/colorized_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo/my_folder/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/my_nested_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo/my_folder/sub_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/sub_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/sub_package/some_deeply_nested_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_other_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:43.076977 packaging-demo-eric-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 08:28:43.076977 packaging-demo-eric-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:43.076977 packaging-demo-eric-0.0.6/packaging_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/colorized_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/my_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:43.076977 packaging-demo-eric-0.0.6/packaging_demo/my_folder/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/my_folder/my_nested_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:43.076977 packaging-demo-eric-0.0.6/packaging_demo/my_folder/sub_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/my_folder/sub_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/my_folder/sub_package/some_deeply_nested_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/my_other_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/packaging_demo/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:43.076977 packaging-demo-eric-0.0.6/packaging_demo_eric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 08:28:43.000000 packaging-demo-eric-0.0.6/packaging_demo_eric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-02 08:28:43.000000 packaging-demo-eric-0.0.6/packaging_demo_eric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:28:43.000000 packaging-demo-eric-0.0.6/packaging_demo_eric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-02 08:28:43.000000 packaging-demo-eric-0.0.6/packaging_demo_eric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 08:28:43.000000 packaging-demo-eric-0.0.6/packaging_demo_eric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:28:43.076977 packaging-demo-eric-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 08:28:25.000000 packaging-demo-eric-0.0.6/version.txt
```

### Comparing `packaging-demo-eric-0.0.5/packaging_demo/states_info.py` & `packaging-demo-eric-0.0.6/packaging_demo/states_info.py`

 * *Files identical despite different names*

### Comparing `packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/SOURCES.txt` & `packaging-demo-eric-0.0.6/packaging_demo_eric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `packaging-demo-eric-0.0.5/pyproject.toml` & `packaging-demo-eric-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 release = ["build", "twine"]
 static-code-qa = ["pre-commit"]
 dev = ["packaging-demo-eric[test,release,static-code-qa]"]
 
-
 [tool.setuptools.dynamic]
 version = {file = "version.txt"}
 
 [tool.black]
 line-length = 119
 exclude = [
     "venv"
```

