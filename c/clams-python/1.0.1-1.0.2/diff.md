# Comparing `tmp/clams-python-1.0.1.tar.gz` & `tmp/clams-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.0.1.tar", last modified: Fri May 26 17:56:44 2023, max compression
+gzip compressed data, was "clams-python-1.0.2.tar", last modified: Fri Jun  2 02:42:07 2023, max compression
```

## Comparing `clams-python-1.0.1.tar` & `clams-python-1.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.257761 clams-python-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-26 17:56:13.000000 clams-python-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 17:56:13.000000 clams-python-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-26 17:56:44.257761 clams-python-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-26 17:56:13.000000 clams-python-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 17:56:13.000000 clams-python-1.0.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.249761 clams-python-1.0.1/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/gha/README.md.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-26 17:56:13.000000 clams-python-1.0.1/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.253761 clams-python-1.0.1/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 17:56:44.000000 clams-python-1.0.1/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.257761 clams-python-1.0.1/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-26 17:56:44.000000 clams-python-1.0.1/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-26 17:56:44.000000 clams-python-1.0.1/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:56:44.000000 clams-python-1.0.1/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 17:56:44.000000 clams-python-1.0.1/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-26 17:56:44.000000 clams-python-1.0.1/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 17:56:44.000000 clams-python-1.0.1/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 17:56:13.000000 clams-python-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:56:44.257761 clams-python-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-26 17:56:13.000000 clams-python-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:56:44.257761 clams-python-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-26 17:56:13.000000 clams-python-1.0.1/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-26 17:56:13.000000 clams-python-1.0.1/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.957961 clams-python-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-06-02 02:41:33.000000 clams-python-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 02:41:33.000000 clams-python-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-02 02:42:07.957961 clams-python-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-02 02:41:33.000000 clams-python-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 02:41:33.000000 clams-python-1.0.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/README.md.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.957961 clams-python-1.0.2/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 02:41:33.000000 clams-python-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 02:42:07.957961 clams-python-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-02 02:41:33.000000 clams-python-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.957961 clams-python-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-06-02 02:41:33.000000 clams-python-1.0.2/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-02 02:41:33.000000 clams-python-1.0.2/tests/test_clamscli.py
```

### Comparing `clams-python-1.0.1/LICENSE` & `clams-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/PKG-INFO` & `clams-python-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.1/README.md` & `clams-python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/__init__.py` & `clams-python-1.0.2/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/app/__init__.py` & `clams-python-1.0.2/clams/app/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/appmetadata/__init__.py` & `clams-python-1.0.2/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/__init__.py` & `clams-python-1.0.2/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/templates/app/.gitignore` & `clams-python-1.0.2/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/templates/app/Containerfile.template` & `clams-python-1.0.2/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/templates/app/README.md.template` & `clams-python-1.0.2/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/templates/app/app.py.template` & `clams-python-1.0.2/clams/develop/templates/app/app.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/templates/app/metadata.py.template` & `clams-python-1.0.2/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/templates/gha/README.md.template` & `clams-python-1.0.2/clams/develop/templates/gha/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.0.2/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/restify/__init__.py` & `clams-python-1.0.2/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams/source/__init__.py` & `clams-python-1.0.2/clams/source/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/clams_python.egg-info/PKG-INFO` & `clams-python-1.0.2/clams_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.1/clams_python.egg-info/SOURCES.txt` & `clams-python-1.0.2/clams_python.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup.py
 ./VERSION
 ./requirements.txt
 clams/__init__.py
 clams/app/__init__.py
 clams/appmetadata/__init__.py
 clams/develop/__init__.py
-clams/develop/templates/app/.dockerignore
-clams/develop/templates/app/.gitignore
+clams/develop/templates/app/.dockerignore.template
+clams/develop/templates/app/.gitignore.template
 clams/develop/templates/app/Containerfile.template
 clams/develop/templates/app/LICENSE.template
 clams/develop/templates/app/README.md.template
 clams/develop/templates/app/app.py.template
 clams/develop/templates/app/metadata.py.template
 clams/develop/templates/app/requirements.txt.template
 clams/develop/templates/gha/README.md.template
```

### Comparing `clams-python-1.0.1/setup.py` & `clams-python-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/tests/test_clamsapp.py` & `clams-python-1.0.2/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.1/tests/test_clamscli.py` & `clams-python-1.0.2/tests/test_clamscli.py`

 * *Files identical despite different names*

