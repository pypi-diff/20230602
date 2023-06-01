# Comparing `tmp/circuitpython-laser-egismos-1.1.1.tar.gz` & `tmp/circuitpython-laser-egismos-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-laser-egismos-1.1.1.tar", last modified: Sun May 14 15:07:03 2023, max compression
+gzip compressed data, was "circuitpython-laser-egismos-1.2.0.tar", last modified: Thu Jun  1 22:14:08 2023, max compression
```

## Comparing `circuitpython-laser-egismos-1.1.1.tar` & `circuitpython-laser-egismos-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.878231 circuitpython-laser-egismos-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.882231 circuitpython-laser-egismos-1.1.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/examples/laser_egismos_async_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/examples/laser_egismos_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/laser_egismos.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.465186 circuitpython-laser-egismos-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.461186 circuitpython-laser-egismos-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.461186 circuitpython-laser-egismos-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.461186 circuitpython-laser-egismos-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.461186 circuitpython-laser-egismos-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-01 22:14:08.465186 circuitpython-laser-egismos-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.461186 circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-01 22:14:08.000000 circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-01 22:14:08.000000 circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:14:08.000000 circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 22:14:08.000000 circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 22:14:08.000000 circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.465186 circuitpython-laser-egismos-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.465186 circuitpython-laser-egismos-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:14:08.465186 circuitpython-laser-egismos-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 22:14:01.000000 circuitpython-laser-egismos-1.2.0/examples/laser_egismos_async_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-01 22:14:01.000000 circuitpython-laser-egismos-1.2.0/examples/laser_egismos_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-01 22:14:01.000000 circuitpython-laser-egismos-1.2.0/laser_egismos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-01 22:14:01.000000 circuitpython-laser-egismos-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-01 22:13:53.000000 circuitpython-laser-egismos-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 22:14:08.465186 circuitpython-laser-egismos-1.2.0/setup.cfg
```

### Comparing `circuitpython-laser-egismos-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-laser-egismos-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/.gitignore` & `circuitpython-laser-egismos-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/.pre-commit-config.yaml` & `circuitpython-laser-egismos-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/.pylintrc` & `circuitpython-laser-egismos-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/CODE_OF_CONDUCT.md` & `circuitpython-laser-egismos-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/LICENSE` & `circuitpython-laser-egismos-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-laser-egismos-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/LICENSES/MIT.txt` & `circuitpython-laser-egismos-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/LICENSES/Unlicense.txt` & `circuitpython-laser-egismos-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/PKG-INFO` & `circuitpython-laser-egismos-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-laser-egismos
-Version: 1.1.1
+Version: 1.2.0
 Summary: Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_laser_egismos
 Keywords: adafruit,blinka,circuitpython,micropython,laser_egismos,laser,egismos,rangefinder,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-laser-egismos-1.1.1/README.rst` & `circuitpython-laser-egismos-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/PKG-INFO` & `circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-laser-egismos
-Version: 1.1.1
+Version: 1.2.0
 Summary: Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_laser_egismos
 Keywords: adafruit,blinka,circuitpython,micropython,laser_egismos,laser,egismos,rangefinder,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/SOURCES.txt` & `circuitpython-laser-egismos-1.2.0/circuitpython_laser_egismos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/docs/_static/favicon.ico` & `circuitpython-laser-egismos-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/docs/conf.py` & `circuitpython-laser-egismos-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/docs/index.rst` & `circuitpython-laser-egismos-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/examples/laser_egismos_async_test.py` & `circuitpython-laser-egismos-1.2.0/examples/laser_egismos_async_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/examples/laser_egismos_simpletest.py` & `circuitpython-laser-egismos-1.2.0/examples/laser_egismos_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.1/laser_egismos.py` & `circuitpython-laser-egismos-1.2.0/laser_egismos.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,24 +20,28 @@
   *  `Egismos laser <https://www.egismos.com/laser-measuring-optoelectronics-module>`_
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 """
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 __repo__ = "https://github.com/furbrain/CircuitPython_laser_egismos.git"
 
+import time
+
 try:
     from typing import Sequence, Tuple
 except ImportError:
     pass
 
 import busio
 
+DEFAULT_TIMEOUT = 5.0
+
 
 class LaserError(RuntimeError):
     """
     An error from the laser module
     """
 
 
@@ -61,14 +65,20 @@
 
 class TooBrightError(LaserError):
     """
     Laser was too bright to get accurate reading
     """
 
 
+class LaserTimeOutError(LaserError):
+    """
+    Laser took too long to respond
+    """
+
+
 class _LaserBase:
     # pylint: disable=too-few-public-methods
     FRAME_END = 0xA8
     FRAME_START = 0xAA
     BUZZER_CONTROL = 0x47
     STOP_CONTINUOUS_MEASURE = 0x46
     CONTINUOUS_MEASURE = 0x45
@@ -77,24 +87,26 @@
     LASER_ON = 0x42
     READ_DEVICE_ERR = 0x08
     SET_SLAVE_ADDRESS = 0x41
     READ_SLAVE_ADDRESS = 0x04
     READ_DEV_TYPE = 0x02
     READ_SW_VERSION = 0x01
 
-    def __init__(self, uart: busio.UART, address=0x01):
+    def __init__(self, uart: busio.UART, address=0x01, timeout=DEFAULT_TIMEOUT):
         """
         Access an Egismos Laser distance module v2
 
         :param ~busio.UART uart: uart to use to connect. Should have baud rate set to 9600
         :param address: address to use, default is 0x01; you should only change this if
           using multiple devices
+        :param timeout: timeout to wait for a response from the device
         """
-        self.uart = uart
-        self.address = address
+        self.uart: busio.UART = uart
+        self.address: int = address
+        self.timeout: float = timeout
 
     def _build_frame(
         self, command: int, address=None, data: Sequence[int] = None
     ) -> bytes:
         """
         Build a frame that represents the given command
 
@@ -173,26 +185,31 @@
 class Laser(_LaserBase):
     """
     This is a driver for the Laser Module 2, produced by Egismos
     """
 
     def _read_frame(self):
         # wait for an AA to start
-        # F.I.X.M.E. this can hang - needs timeout option
+        timeout_due = time.monotonic() + self.timeout
         buffer = b"\x00"
         while buffer[0] != self.FRAME_START:
             buffer = self.uart.read(1) or b"\x00"
+            if time.monotonic() > timeout_due:
+                raise LaserTimeOutError("Timed Out waiting for FRAME_START")
         while buffer[-1] != self.FRAME_END:
             buffer += self.uart.read(1) or b""
+            if time.monotonic() > timeout_due:
+                raise LaserTimeOutError("Timed Out waiting for FRAME_END")
         return buffer
 
     def _send_and_receive(
         self, command: int, data: int = None, address: int = None
     ) -> bytes:
         frame = self._build_frame(command, address, data)
+        self.uart.reset_input_buffer()  # clear input before writing
         self.uart.write(frame)
         frame = self._read_frame()
         read_data = self._process_frame(address, command, frame)
         return read_data
 
     def _send_command_and_raise_on_failure(self, command, data=None):
         """
@@ -274,36 +291,42 @@
 
 
 class AsyncLaser(_LaserBase):
     """
     Same as `Laser`, but with async methods, requires the `asyncio` module
     """
 
-    def __init__(self, uart: busio.UART, address=0x01):
+    def __init__(self, uart: busio.UART, address=0x01, timeout=DEFAULT_TIMEOUT):
         # pylint: disable=import-outside-toplevel
         import asyncio
 
         uart.timeout = 0
-        super().__init__(uart, address)
+        super().__init__(uart, address, timeout)
         self.async_reader = asyncio.StreamReader(uart)
 
     async def _read_frame(self):
         buffer = b"\x00"
         while buffer[0] != self.FRAME_START:
             buffer = await self.async_reader.read(1) or b""
         while buffer[-1] != self.FRAME_END:
             buffer += await self.async_reader.read(1) or b""
         return buffer
 
     async def _send_and_receive(
         self, command: int, data: int = None, address: int = None
     ) -> bytes:
+        # pylint: disable=import-outside-toplevel
+        import asyncio
+
         frame = self._build_frame(command, address, data)
         self.uart.write(frame)
-        frame = await self._read_frame()
+        try:
+            frame = await asyncio.wait_for(self._read_frame(), self.timeout)
+        except asyncio.TimeoutError as exc:
+            raise LaserTimeOutError("Did not receive response within timeout") from exc
         read_data = self._process_frame(address, command, frame)
         return read_data
 
     async def _send_command_and_raise_on_failure(self, command, data=None):
         """
         Send a command, and raise `LaserCommandFailedError` if it does not succeed
         :param int command:
```

### Comparing `circuitpython-laser-egismos-1.1.1/pyproject.toml` & `circuitpython-laser-egismos-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-laser-egismos"
 description = "Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module"
-version = "1.1.1"
+version = "1.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_laser_egismos"}
 keywords = [
     "adafruit",
```

