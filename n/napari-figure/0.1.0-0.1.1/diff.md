# Comparing `tmp/napari-figure-0.1.0.tar.gz` & `tmp/napari-figure-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-figure-0.1.0.tar", last modified: Fri Jun  2 08:29:09 2023, max compression
+gzip compressed data, was "napari-figure-0.1.1.tar", last modified: Fri Jun  2 11:00:50 2023, max compression
```

## Comparing `napari-figure-0.1.0.tar` & `napari-figure-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.609095 napari-figure-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.601095 napari-figure-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.601095 napari-figure-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-02 08:28:46.000000 napari-figure-0.1.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-02 08:28:46.000000 napari-figure-0.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.601095 napari-figure-0.1.0/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 08:28:46.000000 napari-figure-0.1.0/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-02 08:28:46.000000 napari-figure-0.1.0/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-02 08:28:46.000000 napari-figure-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-02 08:28:46.000000 napari-figure-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 08:28:46.000000 napari-figure-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-02 08:29:09.609095 napari-figure-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-02 08:28:46.000000 napari-figure-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.601095 napari-figure-0.1.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)  4040530 2023-06-02 08:28:46.000000 napari-figure-0.1.0/data/6chs_loading.tif
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 08:28:46.000000 napari-figure-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-02 08:29:09.609095 napari-figure-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-02 08:28:46.000000 napari-figure-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.601095 napari-figure-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.609095 napari-figure-0.1.0/src/napari_figure/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 08:28:46.000000 napari-figure-0.1.0/src/napari_figure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.609095 napari-figure-0.1.0/src/napari_figure/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:28:46.000000 napari-figure-0.1.0/src/napari_figure/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 08:28:46.000000 napari-figure-0.1.0/src/napari_figure/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 08:29:09.000000 napari-figure-0.1.0/src/napari_figure/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    24281 2023-06-02 08:28:46.000000 napari-figure-0.1.0/src/napari_figure/figure_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-02 08:28:46.000000 napari-figure-0.1.0/src/napari_figure/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:29:09.609095 napari-figure-0.1.0/src/napari_figure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-02 08:29:09.000000 napari-figure-0.1.0/src/napari_figure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 08:29:09.000000 napari-figure-0.1.0/src/napari_figure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:29:09.000000 napari-figure-0.1.0/src/napari_figure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 08:29:09.000000 napari-figure-0.1.0/src/napari_figure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 08:29:09.000000 napari-figure-0.1.0/src/napari_figure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 08:29:09.000000 napari-figure-0.1.0/src/napari_figure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-02 08:28:46.000000 napari-figure-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.754244 napari-figure-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.750244 napari-figure-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.750244 napari-figure-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-02 11:00:33.000000 napari-figure-0.1.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-02 11:00:33.000000 napari-figure-0.1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.750244 napari-figure-0.1.1/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 11:00:33.000000 napari-figure-0.1.1/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-02 11:00:33.000000 napari-figure-0.1.1/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-02 11:00:33.000000 napari-figure-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-02 11:00:33.000000 napari-figure-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 11:00:33.000000 napari-figure-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-02 11:00:50.754244 napari-figure-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-02 11:00:33.000000 napari-figure-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.750244 napari-figure-0.1.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  4040530 2023-06-02 11:00:33.000000 napari-figure-0.1.1/data/6chs_loading.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 11:00:33.000000 napari-figure-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-02 11:00:50.758244 napari-figure-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.750244 napari-figure-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.754244 napari-figure-0.1.1/src/napari_figure/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 11:00:33.000000 napari-figure-0.1.1/src/napari_figure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.754244 napari-figure-0.1.1/src/napari_figure/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:33.000000 napari-figure-0.1.1/src/napari_figure/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 11:00:33.000000 napari-figure-0.1.1/src/napari_figure/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 11:00:50.000000 napari-figure-0.1.1/src/napari_figure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24281 2023-06-02 11:00:33.000000 napari-figure-0.1.1/src/napari_figure/figure_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-02 11:00:33.000000 napari-figure-0.1.1/src/napari_figure/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:00:50.754244 napari-figure-0.1.1/src/napari_figure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-02 11:00:50.000000 napari-figure-0.1.1/src/napari_figure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-02 11:00:50.000000 napari-figure-0.1.1/src/napari_figure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:00:50.000000 napari-figure-0.1.1/src/napari_figure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 11:00:50.000000 napari-figure-0.1.1/src/napari_figure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 11:00:50.000000 napari-figure-0.1.1/src/napari_figure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:00:50.000000 napari-figure-0.1.1/src/napari_figure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-02 11:00:33.000000 napari-figure-0.1.1/tox.ini
```

### Comparing `napari-figure-0.1.0/.github/workflows/test_and_deploy.yml` & `napari-figure-0.1.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/.gitignore` & `napari-figure-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/.napari-hub/config.yml` & `napari-figure-0.1.1/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/.pre-commit-config.yaml` & `napari-figure-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/LICENSE` & `napari-figure-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/PKG-INFO` & `napari-figure-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: napari-figure
-Version: 0.1.0
+Version: 0.1.1
 Summary: Making Figure with napari more easily
-Home-page: https://github.com/romainGuiet/napari-figure
+Home-page: https://github.com/BIOP/napari-figure
 Author: romainGuiet
 Author-email: romain.guiet@epfl.ch
 License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/romainGuiet/napari-figure/issues
-Project-URL: Documentation, https://github.com/romainGuiet/napari-figure#README.md
-Project-URL: Source Code, https://github.com/romainGuiet/napari-figure
-Project-URL: User Support, https://github.com/romainGuiet/napari-figure/issues
+Project-URL: Bug Tracker, https://github.com/BIOP/napari-figure/issues
+Project-URL: Documentation, https://github.com/BIOP/napari-figure#README.md
+Project-URL: Source Code, https://github.com/BIOP/napari-figure
+Project-URL: User Support, https://github.com/BIOP/napari-figure/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-figure-0.1.0/README.md` & `napari-figure-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/data/6chs_loading.tif` & `napari-figure-0.1.1/data/6chs_loading.tif`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/setup.cfg` & `napari-figure-0.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = napari-figure
 description = Making Figure with napari more easily
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/romainGuiet/napari-figure
+url = https://github.com/BIOP/napari-figure
 author = romainGuiet
 author_email = romain.guiet@epfl.ch
 license = BSD-3-Clause
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Framework :: napari
@@ -18,18 +18,18 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Image Processing
 project_urls = 
-	Bug Tracker = https://github.com/romainGuiet/napari-figure/issues
-	Documentation = https://github.com/romainGuiet/napari-figure#README.md
-	Source Code = https://github.com/romainGuiet/napari-figure
-	User Support = https://github.com/romainGuiet/napari-figure/issues
+	Bug Tracker = https://github.com/BIOP/napari-figure/issues
+	Documentation = https://github.com/BIOP/napari-figure#README.md
+	Source Code = https://github.com/BIOP/napari-figure
+	User Support = https://github.com/BIOP/napari-figure/issues
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	qtpy
```

### Comparing `napari-figure-0.1.0/src/napari_figure/figure_widget.py` & `napari-figure-0.1.1/src/napari_figure/figure_widget.py`

 * *Files identical despite different names*

### Comparing `napari-figure-0.1.0/src/napari_figure.egg-info/PKG-INFO` & `napari-figure-0.1.1/src/napari_figure.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: napari-figure
-Version: 0.1.0
+Version: 0.1.1
 Summary: Making Figure with napari more easily
-Home-page: https://github.com/romainGuiet/napari-figure
+Home-page: https://github.com/BIOP/napari-figure
 Author: romainGuiet
 Author-email: romain.guiet@epfl.ch
 License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/romainGuiet/napari-figure/issues
-Project-URL: Documentation, https://github.com/romainGuiet/napari-figure#README.md
-Project-URL: Source Code, https://github.com/romainGuiet/napari-figure
-Project-URL: User Support, https://github.com/romainGuiet/napari-figure/issues
+Project-URL: Bug Tracker, https://github.com/BIOP/napari-figure/issues
+Project-URL: Documentation, https://github.com/BIOP/napari-figure#README.md
+Project-URL: Source Code, https://github.com/BIOP/napari-figure
+Project-URL: User Support, https://github.com/BIOP/napari-figure/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-figure-0.1.0/src/napari_figure.egg-info/SOURCES.txt` & `napari-figure-0.1.1/src/napari_figure.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
 .napari-hub/DESCRIPTION.md
 .napari-hub/config.yml
 data/6chs_loading.tif
 src/napari_figure/__init__.py
 src/napari_figure/_version.py
```

### Comparing `napari-figure-0.1.0/tox.ini` & `napari-figure-0.1.1/tox.ini`

 * *Files identical despite different names*

