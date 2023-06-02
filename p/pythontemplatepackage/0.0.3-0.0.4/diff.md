# Comparing `tmp/pythontemplatepackage-0.0.3.tar.gz` & `tmp/pythontemplatepackage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythontemplatepackage-0.0.3.tar", last modified: Thu Jun  2 22:46:56 2022, max compression
+gzip compressed data, was "pythontemplatepackage-0.0.4.tar", last modified: Fri Jun  2 17:25:02 2023, max compression
```

## Comparing `pythontemplatepackage-0.0.3.tar` & `pythontemplatepackage-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 22:46:56.891962 pythontemplatepackage-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-02 22:46:41.000000 pythontemplatepackage-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7805 2022-06-02 22:46:56.891962 pythontemplatepackage-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7236 2022-06-02 22:46:41.000000 pythontemplatepackage-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 22:46:56.891962 pythontemplatepackage-0.0.3/pythontemplatepackage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 22:46:41.000000 pythontemplatepackage-0.0.3/pythontemplatepackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-06-02 22:46:41.000000 pythontemplatepackage-0.0.3/pythontemplatepackage/myclass.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 22:46:56.891962 pythontemplatepackage-0.0.3/pythontemplatepackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7805 2022-06-02 22:46:56.000000 pythontemplatepackage-0.0.3/pythontemplatepackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-06-02 22:46:56.000000 pythontemplatepackage-0.0.3/pythontemplatepackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 22:46:56.000000 pythontemplatepackage-0.0.3/pythontemplatepackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-02 22:46:56.000000 pythontemplatepackage-0.0.3/pythontemplatepackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-02 22:46:56.891962 pythontemplatepackage-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-06-02 22:46:41.000000 pythontemplatepackage-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:25:02.101091 pythontemplatepackage-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 17:24:52.000000 pythontemplatepackage-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-02 17:25:02.101091 pythontemplatepackage-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-02 17:24:52.000000 pythontemplatepackage-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:25:02.101091 pythontemplatepackage-0.0.4/pythontemplatepackage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:24:52.000000 pythontemplatepackage-0.0.4/pythontemplatepackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 17:24:52.000000 pythontemplatepackage-0.0.4/pythontemplatepackage/myclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:25:02.101091 pythontemplatepackage-0.0.4/pythontemplatepackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-02 17:25:02.000000 pythontemplatepackage-0.0.4/pythontemplatepackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-02 17:25:02.000000 pythontemplatepackage-0.0.4/pythontemplatepackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:25:02.000000 pythontemplatepackage-0.0.4/pythontemplatepackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 17:25:02.000000 pythontemplatepackage-0.0.4/pythontemplatepackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:25:02.101091 pythontemplatepackage-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-02 17:24:52.000000 pythontemplatepackage-0.0.4/setup.py
```

### Comparing `pythontemplatepackage-0.0.3/LICENSE` & `pythontemplatepackage-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pythontemplatepackage-0.0.3/PKG-INFO` & `pythontemplatepackage-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pythontemplatepackage
-Version: 0.0.3
+Version: 0.0.4
 Summary: A template repo for Python packages with GitHub actions and documentation
 Home-page: https://github.com/robert-lieck/pythontemplatepackage
 Author: Robert Lieck
 Author-email: robert.lieck@durham.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -133,8 +131,7 @@
 #### Publish via GitHub Pages
 
 To publish the documentation via GitHub pages, you have to:
 - create the `gh-pages` branch
 - enable GitHub pages on `gh-pages` branch using the `/` (root) directory.
 
 The `docs` action builds the documentation via `make html` and pushes it to the `gh-pages` branch. It does _not_ run `make doctest`, you have to do this locally to check.
-
```

### Comparing `pythontemplatepackage-0.0.3/README.md` & `pythontemplatepackage-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pythontemplatepackage-0.0.3/pythontemplatepackage.egg-info/PKG-INFO` & `pythontemplatepackage-0.0.4/pythontemplatepackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pythontemplatepackage
-Version: 0.0.3
+Version: 0.0.4
 Summary: A template repo for Python packages with GitHub actions and documentation
 Home-page: https://github.com/robert-lieck/pythontemplatepackage
 Author: Robert Lieck
 Author-email: robert.lieck@durham.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -133,8 +131,7 @@
 #### Publish via GitHub Pages
 
 To publish the documentation via GitHub pages, you have to:
 - create the `gh-pages` branch
 - enable GitHub pages on `gh-pages` branch using the `/` (root) directory.
 
 The `docs` action builds the documentation via `make html` and pushes it to the `gh-pages` branch. It does _not_ run `make doctest`, you have to do this locally to check.
-
```

### Comparing `pythontemplatepackage-0.0.3/setup.py` & `pythontemplatepackage-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read().splitlines()
 
 setuptools.setup(
     name="pythontemplatepackage",
-    version="0.0.3",
+    version="0.0.4",
     author="Robert Lieck",
     author_email="robert.lieck@durham.ac.uk",
     description="A template repo for Python packages with GitHub actions and documentation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/robert-lieck/pythontemplatepackage",
     packages=setuptools.find_packages(exclude=['tests']),
```

